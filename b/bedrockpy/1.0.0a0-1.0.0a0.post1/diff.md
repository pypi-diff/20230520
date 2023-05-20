# Comparing `tmp/bedrockpy-1.0.0a0.tar.gz` & `tmp/bedrockpy-1.0.0a0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrockpy-1.0.0a0.tar", max compression
+gzip compressed data, was "bedrockpy-1.0.0a0.post1.tar", max compression
```

## Comparing `bedrockpy-1.0.0a0.tar` & `bedrockpy-1.0.0a0.post1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0     1071 2023-05-07 13:53:01.935072 bedrockpy-1.0.0a0/LICENSE.md
--rwxr-xr-x   0        0        0     1848 2023-05-16 14:59:55.736142 bedrockpy-1.0.0a0/README.md
--rwxr-xr-x   0        0        0     1681 2023-05-16 15:19:04.060713 bedrockpy-1.0.0a0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-02 13:46:17.293794 bedrockpy-1.0.0a0/src/bedrock/__init__.py
--rwxr-xr-x   0        0        0      780 2023-05-16 14:38:02.689959 bedrockpy-1.0.0a0/src/bedrock/_demo.py
--rwxr-xr-x   0        0        0     2336 2023-05-03 15:02:01.889213 bedrockpy-1.0.0a0/src/bedrock/consts.py
--rwxr-xr-x   0        0        0     9250 2023-05-06 12:00:20.149136 bedrockpy-1.0.0a0/src/bedrock/context.py
--rwxr-xr-x   0        0        0      505 2023-05-01 19:42:23.485482 bedrockpy-1.0.0a0/src/bedrock/events.py
--rwxr-xr-x   0        0        0     7516 2023-05-07 14:28:54.118786 bedrockpy-1.0.0a0/src/bedrock/ext/ui/__init__.py
--rwxr-xr-x   0        0        0     6863 2023-05-07 15:18:48.325559 bedrockpy-1.0.0a0/src/bedrock/ext/ui/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2023-04-29 13:27:19.399359 bedrockpy-1.0.0a0/src/bedrock/py.typed
--rwxr-xr-x   0        0        0      794 2023-05-01 20:12:55.354814 bedrockpy-1.0.0a0/src/bedrock/request.py
--rwxr-xr-x   0        0        0     1881 2023-05-05 14:47:44.619100 bedrockpy-1.0.0a0/src/bedrock/response.py
--rwxr-xr-x   0        0        0    12890 2023-05-07 13:11:27.237467 bedrockpy-1.0.0a0/src/bedrock/server.py
--rwxr-xr-x   0        0        0     2214 2023-05-16 14:59:44.248930 bedrockpy-1.0.0a0/src/bedrock/utils.py
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 bedrockpy-1.0.0a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2023-05-07 13:53:01.935072 bedrockpy-1.0.0a0.post1/LICENSE.md
+-rwxr-xr-x   0        0        0     1998 2023-05-20 12:40:27.800080 bedrockpy-1.0.0a0.post1/README.md
+-rwxr-xr-x   0        0        0     1809 2023-05-20 18:59:41.038990 bedrockpy-1.0.0a0.post1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-02 13:46:17.293794 bedrockpy-1.0.0a0.post1/src/bedrock/__init__.py
+-rwxr-xr-x   0        0        0      780 2023-05-16 14:38:02.689959 bedrockpy-1.0.0a0.post1/src/bedrock/_demo.py
+-rwxr-xr-x   0        0        0     2336 2023-05-03 15:02:01.889213 bedrockpy-1.0.0a0.post1/src/bedrock/consts.py
+-rwxr-xr-x   0        0        0     9250 2023-05-06 12:00:20.149136 bedrockpy-1.0.0a0.post1/src/bedrock/context.py
+-rwxr-xr-x   0        0        0      505 2023-05-01 19:42:23.485482 bedrockpy-1.0.0a0.post1/src/bedrock/events.py
+-rwxr-xr-x   0        0        0     7516 2023-05-07 14:28:54.118786 bedrockpy-1.0.0a0.post1/src/bedrock/ext/ui/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 13:27:19.399359 bedrockpy-1.0.0a0.post1/src/bedrock/py.typed
+-rwxr-xr-x   0        0        0      794 2023-05-01 20:12:55.354814 bedrockpy-1.0.0a0.post1/src/bedrock/request.py
+-rwxr-xr-x   0        0        0     1881 2023-05-05 14:47:44.619100 bedrockpy-1.0.0a0.post1/src/bedrock/response.py
+-rwxr-xr-x   0        0        0    12890 2023-05-07 13:11:27.237467 bedrockpy-1.0.0a0.post1/src/bedrock/server.py
+-rwxr-xr-x   0        0        0     3896 2023-05-20 12:07:51.156128 bedrockpy-1.0.0a0.post1/src/bedrock/utils.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 bedrockpy-1.0.0a0.post1/PKG-INFO
```

### Comparing `bedrockpy-1.0.0a0/LICENSE.md` & `bedrockpy-1.0.0a0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/README.md` & `bedrockpy-1.0.0a0.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 <!-- start brief-hook -->
 
 *bedrockpy* lets you create a websocket server that is able to interact
 with a player in a Minecraft game. As the name suggests: this project
 only works with the "Minecraft: Bedrock Edition".
 
+[![Documentation Status](https://readthedocs.org/projects/bedrockpy/badge/?version=latest)](https://bedrockpy.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/github/license/bedrock-ws/bedrockpy?style=flat-square)](https://github.com/bedrock-ws/bedrockpy/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/bedrockpy?style=flat-square)](https://pypi.org/project/bedrockpy)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/bedrockpy?style=flat-square)](https://pypi.org/project/bedrockpy)
 
 
 ## Quick Links
 
@@ -67,8 +68,9 @@
 pip install -U "bedrockpy[fast]"
 ```
 
 <!-- end installation-hook -->
 
 ---
 
-NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
+NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH
+MOJANG.
```

### Comparing `bedrockpy-1.0.0a0/pyproject.toml` & `bedrockpy-1.0.0a0.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bedrockpy"
-version = "1.0.0.a0"
+version = "1.0.0.a0.post1"
 description = "Minecraft: Bedrock Edition Websocket Server"
 authors = ["Jonas da Silva"]
 maintainers = [
     "Bedrock WS <bedrock-ws@proton.me>",
     "Jonas da Silva"
 ]
 license = "MIT"
@@ -21,39 +21,42 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Education",
     "Topic :: Games/Entertainment",
     "Typing :: Typed",
 ]
 packages = [{include = "bedrock", from = "src"}]
+include = ["src/bedrock/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 websockets = "^11.0.2"
 attrs = "^23.1.0"
 convert-case = "^1.1.1"
 
 sphinx = {version = "^6.2.1", optional = true}
 myst-parser = {version = "^1.0.0", extras = ["linkify"], optional = true}
 sphinx-copybutton = {version = "^0.5.2", optional = true}
 furo = {version = "^2023.3.27", optional = true}
 sphinxcontrib-mermaid = {version = "^0.8.1", optional = true}
+sphinxcontrib-video = {version = "^0.1.1", optional = true}
 
 mypy = {version = "^1.2.0", optional = true}
 tox = {version = "^4.5.1", optional = true}
 
 uvloop = {version = "^0.17.0", optional = true}
 
 [tool.poetry.extras]
 docs = [
     "sphinx",
     "myst-parser",
     "sphinx-copybutton",
     "furo",
     "sphinxcontrib-mermaid",
+    "sphinxcontrib-video",
 ]
 dev = [
     "mypy",
     "tox",
 ]
 fast = [
     "uvloop",
```

### Comparing `bedrockpy-1.0.0a0/src/bedrock/_demo.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/_demo.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/consts.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/consts.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/context.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/context.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/ext/ui/__init__.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/ext/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/request.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/request.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/response.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/response.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/server.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/server.py`

 * *Files identical despite different names*

### Comparing `bedrockpy-1.0.0a0/src/bedrock/utils.py` & `bedrockpy-1.0.0a0.post1/src/bedrock/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,60 @@
 from __future__ import annotations
 
 from enum import Enum
 import json
-from typing import NewType
+from typing import Iterable, Literal, Mapping, NewType
 
 from attrs import define
 
 
-def rawtext(text: str) -> str:
-    """Wraps text inside a rawtext JSON object.
+def rawtext(text: str | Iterable[
+    Mapping[
+        Literal["text"] | Literal["selector"],
+        str
+    ] | Mapping[
+        Literal["score"],
+        Mapping[
+            Literal["name"] | Literal["objective"],
+            str
+        ]
+    ]]) -> str:
+    """
+    Wraps text inside a rawtext JSON object which can be used for
+    ``/tellraw``, ``/titleraw`` etc.
     
     .. seealso:: https://wiki.bedrock.dev/commands/tellraw.html
+
+    Parameters
+    ----------
+    text
+        Either just a string or an iterable of mappings beeing
+        valid rawtext parts.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        >>> from bedrock.utils import rawtext
+        >>> rawtext('Hello World')
+        '{"rawtext": [{"text": "Hello, World"}]}'
+        >>> rawtext([{'text': 'Hello '}, {'selector': '@p[r=10]'}])
+        '{"rawtext": [{"text": "Hello "}, {"selectors": "@p[r=10]}]}'
+    
     """
-    return json.dumps({
-        "rawtext": [{"text": text}]
-    })
+    if isinstance(text, str):
+        return json.dumps({
+            "rawtext": [{"text": text}]
+        })
+    else:
+        return json.dumps({
+            "rawtext": text
+        })
+
 
 class TargetSelector(str, Enum):
     """
     A collection of target selectors that can be used within commands.
     
     .. seealso:: https://minecraft.fandom.com/wiki/Target_selectors
     """
@@ -59,26 +95,52 @@
     def __str__(self) -> str:
         return f"^{self.coord}"
 
     @classmethod
     def from_string(cls, value: str) -> LocalCoordinate:
         n = value.removeprefix("^")
         if len(n) != len(value):
-            raise ValueError("coordinate must start with a caret (^)")
+            raise ValueError("local coordinate must start with a caret (^)")
         return cls(numeric(n))
 
 
 WorldCoordinates = NewType(
-    "WorldCoordinates", tuple[WorldCoordinate, WorldCoordinate, WorldCoordinate]
+    "WorldCoordinates",
+    tuple[WorldCoordinate, WorldCoordinate, WorldCoordinate]
 )
 LocalCoordinates = NewType(
-    "LocalCoordinates", tuple[LocalCoordinate, LocalCoordinate, LocalCoordinate]
+    "LocalCoordinates",
+    tuple[LocalCoordinate, LocalCoordinate, LocalCoordinate]
 )
 
 
+def boolean(value: str) -> bool:
+    """Converts a string into a boolean.
+    
+    Parameters
+    ----------
+    value
+        The string to convert into a boolean.
+
+        * ``'y'``/``'yes'``/``'true'`` \N{RIGHTWARDS DOUBLE ARROW} ``True``
+        * ``'n'``/``'no'``/``'false'`` \N{RIGHTWARDS DOUBLE ARROW} ``False``
+
+        *The string is converted into lower case before comparing.*
+
+    Raises
+    ------
+    ValueError
+        The string cannot be converted into a boolean.
+    """
+    if value.lower() in {"y", "yes", "true"}:
+        return True
+    elif value.lower() in {"n", "no", "false"}:
+        return False
+    raise ValueError(f"cannot turn {value!r} into a boolean")
+
 def numeric(value: str) -> float:
     """
     Converts a string into an integer or if that fails into a floating
     point.
 
     Parameters
     ----------
@@ -89,8 +151,11 @@
     ------
     ValueError
         The string cannot be converted into a boolean.
     """
     try:
         return int(value)
     except ValueError:
-        return float(value)
+        try:
+            return float(value)
+        except ValueError as e:
+            raise e from None
```

### Comparing `bedrockpy-1.0.0a0/PKG-INFO` & `bedrockpy-1.0.0a0.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrockpy
-Version: 1.0.0a0
+Version: 1.0.0a0.post1
 Summary: Minecraft: Bedrock Edition Websocket Server
 Home-page: https://github.com/bedrock-ws/bedrockpy/
 License: MIT
 Keywords: bedrock,minecraft,websocket
 Author: Jonas da Silva
 Maintainer: Bedrock WS
 Maintainer-email: bedrock-ws@proton.me
@@ -29,14 +29,15 @@
 Requires-Dist: convert-case (>=1.1.1,<2.0.0)
 Requires-Dist: furo (>=2023.3.27,<2024.0.0) ; extra == "docs"
 Requires-Dist: mypy (>=1.2.0,<2.0.0) ; extra == "dev"
 Requires-Dist: myst-parser[linkify] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx (>=6.2.1,<7.0.0) ; extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid (>=0.8.1,<0.9.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-video (>=0.1.1,<0.2.0) ; extra == "docs"
 Requires-Dist: tox (>=4.5.1,<5.0.0) ; extra == "dev"
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; extra == "fast"
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Project-URL: Documentation, https://bedrockpy.readthedocs.io/
 Project-URL: Repository, https://github.com/bedrock-ws/bedrockpy/
 Description-Content-Type: text/markdown
 
@@ -49,14 +50,15 @@
 
 <!-- start brief-hook -->
 
 *bedrockpy* lets you create a websocket server that is able to interact
 with a player in a Minecraft game. As the name suggests: this project
 only works with the "Minecraft: Bedrock Edition".
 
+[![Documentation Status](https://readthedocs.org/projects/bedrockpy/badge/?version=latest)](https://bedrockpy.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/github/license/bedrock-ws/bedrockpy?style=flat-square)](https://github.com/bedrock-ws/bedrockpy/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/bedrockpy?style=flat-square)](https://pypi.org/project/bedrockpy)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/bedrockpy?style=flat-square)](https://pypi.org/project/bedrockpy)
 
 
 ## Quick Links
 
@@ -109,9 +111,10 @@
 pip install -U "bedrockpy[fast]"
 ```
 
 <!-- end installation-hook -->
 
 ---
 
-NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
+NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH
+MOJANG.
```

