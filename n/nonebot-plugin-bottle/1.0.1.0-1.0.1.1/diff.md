# Comparing `tmp/nonebot_plugin_bottle-1.0.1.0.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.1.0.tar` & `nonebot_plugin_bottle-1.0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7814 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/README.md
--rw-r--r--   0        0        0    20745 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    18547 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2647 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      625 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8577 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7814 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/README.md
+-rw-r--r--   0        0        0    20068 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    19027 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2646 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      968 2023-05-19 13:01:14.130806 nonebot_plugin_bottle-1.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8577 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.1.0/README.md` & `nonebot_plugin_bottle-1.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import asyncio
 
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot import require, on_command
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
-from nonebot.params import Depends, CommandArg, ArgStr
+from nonebot.params import ArgStr, Depends, CommandArg
 
 require("nonebot_plugin_datastore")
-from nonebot_plugin_datastore import get_session
 from sqlalchemy.ext.asyncio.session import AsyncSession
+from nonebot_plugin_datastore import get_session, create_session
 from nonebot.adapters.onebot.v11 import (
     GROUP,
     Bot,
     Message,
     ActionFailed,
     MessageEvent,
     MessageSegment,
@@ -25,14 +25,15 @@
 from .config import Config
 from .data_source import (
     ba,
     text_audit,
     bottle_manager,
     serialize_message,
     deserialize_message,
+    get_content_preview,
 )
 
 __plugin_meta__ = PluginMetadata(
     name="漂流瓶",
     description="群与群互通的漂流瓶插件",
     config=Config,
     usage=f"""
@@ -117,24 +118,15 @@
         user_id=event.user_id, session=session, include_del=False
     )
     if not bottles:
         await listb.finish("你还没有扔过漂流瓶哦～")
 
     bottles_info = []
     for bottle in bottles:
-        message_parts = deserialize_message(bottle.content)
-        content_preview = ""
-        for part in message_parts:
-            if part.type == "text":
-                # 文字截取
-                text = part.data["text"]
-                content_preview += text[:20] + "..." if len(text) > 20 else text
-            elif part.type == "image":
-                # 图片处理
-                content_preview += "[图片]"
+        content_preview = get_content_preview(bottle)
         bottles_info.append(f"#{bottle.id}：{content_preview}")
 
     messages = []
     total_bottles_info = f"您总共扔了{len(bottles_info)}个漂流瓶～\n"
     if len(bottles_info) > 10:
         i = 1
         while len(bottles_info) > 10:
@@ -411,44 +403,33 @@
     state: T_State,
     arg: Message = CommandArg(),
     session: AsyncSession = Depends(get_session),
 ):
     index = arg.extract_plain_text().strip()
     bottle = await get_bottle(index=index, matcher=matcher, session=session)
     if str(event.user_id) in bot.config.superusers or bottle.user_id == event.user_id:
-        message_parts = deserialize_message(bottle.content)
-        content_preview = ""
-        for part in message_parts:
-            if part.type == "text":
-                # 文字截取
-                text = part.data["text"]
-                content_preview += text[:20] + "..." if len(text) > 20 else text
-            elif part.type == "image":
-                # 图片处理
-                content_preview += "[图片]"
-        state["index"] = index
-        state["session"] = session
-        state["matcher"] = matcher
+        content_preview = get_content_preview(bottle)
+        state["index"] = int(index)
         await remove.send(f"你是否要删除漂流瓶（Y/N）？漂流瓶将会永久失去。（真的很久！）\n漂流瓶内容：{content_preview}")
     else:
         await remove.finish("删除失败！你没有相关的权限！")
 
 
 proceed = ["是", "Y", "Yes", "y", "yes"]
 
 
 @remove.got("prompt")
 async def _(state: T_State, conf: str = ArgStr("prompt")):
     if conf in proceed:
         index = state["index"]
-        matcher = state["matcher"]
-        session = state["session"]
-        bottle = await get_bottle(index=index, matcher=matcher, session=session)
-        bottle.is_del = True
-        await session.commit()
+        async with create_session() as session:
+            # 前面验证了id合法性后这里就直接拿了，由于是不同的会话所以必须重新获取（大概）
+            bottle = await bottle_manager.get_bottle(index=index, session=session)
+            bottle.is_del = True
+            await session.commit()
         await remove.send(f"成功删除 {index} 号漂流瓶！")
     else:
         await remove.finish("取消删除操作。")
 
 
 ###### SUPERUSER命令 ######
```

### Comparing `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 try:
     import ujson as json
 except:
     import json
 
 import re
 import time
+import asyncio
 import hashlib
 from pathlib import Path
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Sequence
 
 import httpx
-import asyncio
 import aiofiles
 from nonebot.log import logger
 from pydantic import parse_obj_as
 from sqlalchemy import func, text, select
 from sqlalchemy.ext.asyncio.session import AsyncSession
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot_plugin_datastore.db import get_engine, post_db_init, create_session
@@ -69,14 +69,28 @@
     for seg in message:
         if seg["type"] == "cached_image":
             seg["type"] = "image"
             seg["data"]["file"] = (cache_dir / seg["data"]["file"]).resolve().as_uri()
     return parse_obj_as(Message, message)
 
 
+def get_content_preview(bottle: Bottle) -> str:
+    message_parts = deserialize_message(bottle.content)
+    content_preview = ""
+    for part in message_parts:
+        if part.type == "text":
+            # 文字截取
+            text = part.data["text"]
+            content_preview += text[:20] + "..." if len(text) > 20 else text
+        elif part.type == "image":
+            # 图片处理
+            content_preview += "[图片]"
+    return content_preview
+
+
 @post_db_init
 async def _():
     old_data = data_dir / "data.json"
     if old_data.exists():
         logger.info("开始迁移旧漂流瓶数据")
         with open(old_data, "r", encoding="utf-8") as f:
             data = json.load(f)
```

### Comparing `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """init_db
 
 Revision ID: 449e066410fd
 Revises: 
 Create Date: 2023-03-10 14:34:07.064331
 
 """
-from alembic import op
 import sqlalchemy as sa
-
+from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "449e066410fd"
 down_revision = None
 branch_labels = None
 depends_on = None
```

### Comparing `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.1.1/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.1.0/PKG-INFO` & `nonebot_plugin_bottle-1.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.1.0
+Version: 1.0.1.1
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

