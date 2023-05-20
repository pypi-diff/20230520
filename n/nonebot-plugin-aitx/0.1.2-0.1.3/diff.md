# Comparing `tmp/nonebot_plugin_aitx-0.1.2.tar.gz` & `tmp/nonebot_plugin_aitx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aitx-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_aitx-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_aitx-0.1.2.tar` & `nonebot_plugin_aitx-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1843 2023-05-20 01:04:43.511853 nonebot_plugin_aitx-0.1.2/nonebot-plugin-aitx/__init__.py
--rw-r--r--   0        0        0      476 2023-05-20 01:55:29.092898 nonebot_plugin_aitx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      348 2023-05-20 01:15:21.570060 nonebot_plugin_aitx-0.1.2/README.md
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 nonebot_plugin_aitx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1889 2023-05-20 05:15:55.988825 nonebot_plugin_aitx-0.1.3/nonebot-plugin-aitx/__init__.py
+-rw-r--r--   0        0        0      476 2023-05-20 05:16:06.642278 nonebot_plugin_aitx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-05-20 01:15:21.570060 nonebot_plugin_aitx-0.1.3/README.md
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 nonebot_plugin_aitx-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_aitx-0.1.2/nonebot-plugin-aitx/__init__.py` & `nonebot_plugin_aitx-0.1.3/nonebot-plugin-aitx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from nonebot import on_message
 from nonebot.adapters.onebot.v11 import Bot, Event
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.rule import to_me
 
 import random
 ai_tx = on_message(priority=100,rule=to_me())
+config = nonebot.get_driver().config
+
 async def get_reply(s):
     try:
-        cred = credential.Credential("", "")##请在这里填写你的腾讯云api,填两个
+        cred = credential.Credential(str(config.TENCENT_SECRET_ID),str(config.TENCENT_SECRET_KEY))
         httpProfile = HttpProfile()
         httpProfile.endpoint = "nlp.tencentcloudapi.com"
 
         clientProfile = ClientProfile()
         clientProfile.httpProfile = httpProfile
         client = nlp_client.NlpClient(cred, "ap-guangzhou", clientProfile)
```

### Comparing `nonebot_plugin_aitx-0.1.2/PKG-INFO` & `nonebot_plugin_aitx-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-aitx
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于腾讯云接口的ai聊天
 Author: lcy
 Author-email: 863109569@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

