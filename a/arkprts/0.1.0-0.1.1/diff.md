# Comparing `tmp/arkprts-0.1.0.tar.gz` & `tmp/arkprts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.0.tar", last modified: Fri May 19 19:22:47 2023, max compression
+gzip compressed data, was "arkprts-0.1.1.tar", last modified: Sat May 20 18:07:04 2023, max compression
```

## Comparing `arkprts-0.1.0.tar` & `arkprts-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.245955 arkprts-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-05-19 19:22:47.244954 arkprts-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.164483 arkprts-0.1.0/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.0/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.0/arkprts/__main__.py
--rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.0/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.0/arkprts/errors.py
--rw-rw-rw-   0        0        0     6033 2023-05-19 18:45:31.000000 arkprts-0.1.0/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.230962 arkprts-0.1.0/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.0/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     2724 2023-05-19 18:41:28.000000 arkprts-0.1.0/arkprts/models/base.py
--rw-rw-rw-   0        0        0     8548 2023-05-19 19:13:33.000000 arkprts-0.1.0/arkprts/models/data.py
--rw-rw-rw-   0        0        0     6588 2023-05-19 18:47:58.000000 arkprts-0.1.0/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.0/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.218972 arkprts-0.1.0/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 19:22:47.246953 arkprts-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-19 19:21:52.000000 arkprts-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.241955 arkprts-0.1.0/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.0/tests/test_config.py
--rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.0/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.122009 arkprts-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-05-20 18:07:04.036059 arkprts-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 18:07:03.770616 arkprts-0.1.1/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.1/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.1/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.1/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.1/arkprts/errors.py
+-rw-rw-rw-   0        0        0     6033 2023-05-19 18:45:31.000000 arkprts-0.1.1/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.023065 arkprts-0.1.1/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.1/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     2734 2023-05-20 17:40:39.000000 arkprts-0.1.1/arkprts/models/base.py
+-rw-rw-rw-   0        0        0     8940 2023-05-20 17:53:56.000000 arkprts-0.1.1/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     6953 2023-05-20 17:54:10.000000 arkprts-0.1.1/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.1/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.003078 arkprts-0.1.1/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 18:07:03.000000 arkprts-0.1.1/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 18:07:04.122009 arkprts-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-05-20 18:05:29.000000 arkprts-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:07:04.032063 arkprts-0.1.1/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.1/tests/test_config.py
+-rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.1/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.0/LICENSE` & `arkprts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/PKG-INFO` & `arkprts-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.0/README.md` & `arkprts-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/arkprts/__main__.py` & `arkprts-0.1.1/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/arkprts/client.py` & `arkprts-0.1.1/arkprts/client.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/arkprts/errors.py` & `arkprts-0.1.1/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/arkprts/gamedata.py` & `arkprts-0.1.1/arkprts/gamedata.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/arkprts/models/base.py` & `arkprts-0.1.1/arkprts/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,17 @@
             _set_recursively(key, name, value)
             _set_recursively(item, name, value)
     elif isinstance(obj, typing.Sequence) and not isinstance(obj, str):
         for item in obj:  # pyright: ignore[reportUnknownVariableType]
             _set_recursively(item, name, value)
 
 
-def _to_snake_case(string: str) -> str:
-    """Convert camelCase to snake_case."""
-    return "".join(
-        ("_" if i and string[i].isupper() and not string[i : i + 2].isupper() else "") + x.lower()
-        for i, x in enumerate(string)
-    )
+def _to_camel_case(string: str) -> str:
+    """Convert snake_case to camelCase."""
+    return "".join(x.title() if i else x for i, x in enumerate(string.split("_")))
 
 
 class BaseModel(pydantic.BaseModel):
     """Client-aware pydantic base model."""
 
     client: Client = pydantic.Field(repr=False)
     """Client instance."""
@@ -56,27 +53,32 @@
 
 
 class DList(collections.UserList[typing.Any]):
     """Dot-accessed list."""
 
     def __getitem__(self, key: typing.Any) -> typing.Any:
         item = super().__getitem__(key)
+
         if isinstance(item, dict):
             item = DDict(item)  # pyright: ignore[reportUnknownArgumentType]
         elif isinstance(item, list):
             item = DList(item)  # pyright: ignore[reportUnknownArgumentType]
 
         return item
 
 
 class DDict(collections.UserDict[str, typing.Any]):
     """Dot-accessed dictionary."""
 
     def __getitem__(self, key: typing.Any) -> typing.Any:
-        item = super().__getitem__(_to_snake_case(key))
+        try:
+            item = super().__getitem__(key)
+        except KeyError:
+            item = super().__getitem__(_to_camel_case(key))
+
         if isinstance(item, dict):
             item = DDict(item)  # pyright: ignore[reportUnknownArgumentType]
         elif isinstance(item, list):
             item = DList(item)  # pyright: ignore[reportUnknownArgumentType]
 
         return item
```

### Comparing `arkprts-0.1.0/arkprts/models/data.py` & `arkprts-0.1.1/arkprts/models/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,24 @@
     char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
     """Operator group data."""
     char_mission: typing.Mapping[str, typing.Mapping[str, bool]] = pydantic.Field(alias="charMission")
     """Special operation missions."""
     addon: typing.Any
     """IDK."""
 
+    @pydantic.validator("chars", pre=True)  # pyright: ignore[reportUnknownMemberType]
+    def _fix_amiya(cls, value: typing.Any) -> typing.Any:
+        """Flatten amiya to only keep her guard form."""
+        for v in value.values():
+            if v and v.get("tmpl"):
+                current = v["tmpl"][v["currentTmpl"]]
+                v.update(current)
+
+        return value
+
 
 class Skins(base.BaseModel):
     """Operator skin data."""
 
     character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
     """Owned skins."""
     skin_ts: typing.Mapping[str, datetime.datetime] = pydantic.Field(alias="skinTs")
```

### Comparing `arkprts-0.1.0/arkprts/models/social.py` & `arkprts-0.1.1/arkprts/models/social.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,23 @@
     assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
     """Assist operator list."""
     last_online_time: datetime.datetime = pydantic.Field(alias="lastOnlineTime")
     """Last online time."""
     medal_board: MedalBoard = pydantic.Field(alias="medalBoard")
     """Medal board."""
 
+    @pydantic.validator("assist_char_list", pre=True, each_item=True)  # pyright: ignore[reportUnknownMemberType]
+    def _fix_amiya(cls, v: typing.Any) -> typing.Any:
+        """Flatten amiya to only keep her guard form."""
+        if v and v.get("tmpl"):
+            current = v["tmpl"][v["currentTmpl"]]
+            v.update(current)
+
+        return v
+
 
 class Player(PartialPlayer):
     """Player info."""
 
     register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
     """Account creation time."""
     main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
```

### Comparing `arkprts-0.1.0/arkprts.egg-info/PKG-INFO` & `arkprts-0.1.1/arkprts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.0
+Version: 0.1.1
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.0/pyproject.toml` & `arkprts-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.0/setup.py` & `arkprts-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.0",
+    version="0.1.1",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

