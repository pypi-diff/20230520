# Comparing `tmp/econuker-1.0.1.tar.gz` & `tmp/econuker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.1.tar", last modified: Sat May 20 00:50:30 2023, max compression
+gzip compressed data, was "econuker-1.0.2.tar", last modified: Sat May 20 01:06:03 2023, max compression
```

## Comparing `econuker-1.0.1.tar` & `econuker-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.465647 econuker-1.0.1/
--rw-rw-rw-   0        0        0      819 2023-05-20 00:50:30.459652 econuker-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1363 2023-05-20 00:27:36.000000 econuker-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.091457 econuker-1.0.1/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.1/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.1/econuker/__init__.py
--rw-rw-rw-   0        0        0    14765 2023-05-20 00:48:01.000000 econuker-1.0.1/econuker/async_client.py
--rw-rw-rw-   0        0        0    14264 2023-05-20 00:48:27.000000 econuker-1.0.1/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.432663 econuker-1.0.1/econuker.egg-info/
--rw-rw-rw-   0        0        0      819 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 00:50:28.000000 econuker-1.0.1/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 00:50:30.466643 econuker-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-05-20 00:49:23.000000 econuker-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 01:06:03.670528 econuker-1.0.2/
+-rw-rw-rw-   0        0        0      819 2023-05-20 01:06:03.668533 econuker-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1363 2023-05-20 00:27:36.000000 econuker-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 01:06:03.623661 econuker-1.0.2/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.2/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.2/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14369 2023-05-20 01:03:00.000000 econuker-1.0.2/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13860 2023-05-20 01:03:10.000000 econuker-1.0.2/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-20 01:06:03.664527 econuker-1.0.2/econuker.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-05-20 01:06:03.000000 econuker-1.0.2/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-20 01:06:03.000000 econuker-1.0.2/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 01:06:03.000000 econuker-1.0.2/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 01:06:03.000000 econuker-1.0.2/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 01:06:03.000000 econuker-1.0.2/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 01:06:03.670528 econuker-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-05-20 01:05:33.000000 econuker-1.0.2/setup.py
```

### Comparing `econuker-1.0.1/PKG-INFO` & `econuker-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.1
+Version: 1.0.2
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.1/README.md` & `econuker-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `econuker-1.0.1/econuker/Exceptions.py` & `econuker-1.0.2/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.1/econuker/async_client.py` & `econuker-1.0.2/econuker/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,51 @@
     elif response.status == 429:
         raise RateLimited(f"{await response.text()}")
     elif 200 <= response.status < 300:
         return False
     else:
         raise EconukerException(f"{await response.text()}")
 
+class Owner:
+    """
+    Owner object.
+
+    Attributes:
+        _raw (str): Raw owner data.
+        name (str): Owner name.
+        id (str): Owner ID.
+        nick (str, None): Owner nickname.
+        profile (str, None): Owner profile.
+    """
+
+    def __init__(self, data):
+        self._raw: str = data
+        self.name = data["name"]
+        self.id = data["id"]
+        self.nick = data.get("nick")
+        self.profile = data.get("profile")
+
+class ItemPrice:
+    """
+    ItemPrice object.
+
+    Attributes:
+        _raw (dict): Raw item price data, excluding worth.
+        _price_parts (str): Raw item price data split.
+        sell (str): The sell amount.
+        buy (str): The buy amount.
+        worth (str): The worth amount.
+    """
+
+    def __init__(self, price):
+        self._raw: dict = price
+        self._price_parts: list = price.split("|")
+        self.sell: str = self._price_parts[0].strip()
+        self.buy: str = self._price_parts[1].strip()
+        self.worth: str = None
 
 class Token:
     """
     Represents an authentication token.
 
     Args:
         authtoken (str): The authentication token.
@@ -198,33 +235,14 @@
             created_at (int): Epoch timestamp.
             timezone (str): The raw timezone of the server.
             slug (str): The server's slug.
             about (str, None): The server's "about me" information.
         """
 
         def __init__(self, data):
-            class Owner:
-                """
-                Owner object.
-
-                Attributes:
-                    _raw (str): Raw owner data.
-                    name (str): Owner name.
-                    id (str): Owner ID.
-                    nick (str, None): Owner nickname.
-                    profile (str, None): Owner profile.
-                """
-
-                def __init__(self, data):
-                    self._raw: str = data
-                    self.name = data["name"]
-                    self.id = data["id"]
-                    self.nick = data.get("nick")
-                    self.profile = data.get("profile")
-
             self._raw: dict = data
             self.id: str = data["id"]
             self.name: str = data["name"]
             self.owner: Owner = Owner(data["owner"])
             self.url: str = data["vanity_url"]
             self.verified: bool = data["verified"]
             self.created_at: int = data["created_at"]
@@ -298,43 +316,24 @@
             desc (str): An alias for the description.
             aliases (list): A list of all item aliases.
             _extradata (str): The extradata of the item.
             price (ItemPrice): Price data of the item.
         """
 
         def __init__(self, data):
-            class ItemPrice:
-                """
-                ItemPrice object.
-
-                Attributes:
-                    _raw (dict): Raw item price data, excluding worth.
-                    _price_parts (str): Raw item price data split.
-                    sell (str): The sell amount.
-                    buy (str): The buy amount.
-                    worth (str): The worth amount.
-                """
-
-                def __init__(self, price):
-                    self._raw: dict = price
-                    self._price_parts: list = price.split("|")
-                    self.sell: str = self._price_parts[0].strip()
-                    self.buy: str = self._price_parts[1].strip()
-                    self.worth: str = None
-
             self._raw: dict = data
             self._data: list = data.get(list(data.keys())[0])
             self.id: str = list(data.keys())[0]
             self.name: str = self._data[0]
             self.rarity: str = self._data[1]
             self.description: str = self._data[2]
             self.desc: str = self._data[2]
             self.aliases: list = self._data[3]
             self._extradata: str = self._data[4]
-            self.price: self.ItemPrice = self.ItemPrice(self._data[5])
+            self.price: ItemPrice = ItemPrice(self._data[5])
             self.price.worth: str = self._data[6]
 
     async def fetch_items(self, hidden: bool = True) -> ItemsResult:
         """
         Fetches all items.
 
         Args:
```

### Comparing `econuker-1.0.1/econuker/client.py` & `econuker-1.0.2/econuker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,50 @@
     elif response.status_code == 429:
         raise RateLimited(f"{response.content.decode()}")
     elif 200 <= response.status_code < 300:
         return False
     else:
         raise EconukerException(f"{response.content.decode()}")
 
+class Owner:
+    """
+    Owner object.
+
+    Attributes:
+        _raw (str): Raw owner data.
+        name (str): Owner name.
+        id (str): Owner ID.
+        nick (str, None): Owner nickname.
+        profile (str, None): Owner profile.
+    """
+
+    def __init__(self, data):
+        self._raw: str = data
+        self.name = data["name"]
+        self.id = data["id"]
+        self.nick = data.get("nick")
+        self.profile = data.get("profile")
+
+class ItemPrice:
+    """
+    ItemPrice object.
+
+    Attributes:
+        _raw (dict): Raw item price data, excluding worth.
+        _price_parts (str): Raw item price data split.
+        sell (str): The sell amount.
+        buy (str): The buy amount.
+        worth (str): The worth amount.
+    """
+    def __init__(self, price):
+        self._raw: dict = price
+        self._price_parts: list = price.split("|")
+        self.sell: str = self._price_parts[0].strip()
+        self.buy: str = self._price_parts[1].strip()
+        self.worth: str = None
 
 class Token:
     """
     Represents an authentication token.
 
     Args:
         authtoken (str): The authentication token.
@@ -202,37 +238,18 @@
             created_at (int): Epoch timestamp.
             timezone (str): The raw timezone of the server.
             slug (str): The server's slug.
             about (str, None): The server's "about me" information.
         """
 
         def __init__(self, data):
-            class Owner:
-                """
-                Owner object.
-
-                Attributes:
-                    _raw (str): Raw owner data.
-                    name (str): Owner name.
-                    id (str): Owner ID.
-                    nick (str, None): Owner nickname.
-                    profile (str, None): Owner profile.
-                """
-
-                def __init__(self, data):
-                    self._raw: str = data
-                    self.name = data["name"]
-                    self.id = data["id"]
-                    self.nick = data.get("nick")
-                    self.profile = data.get("profile")
-
             self._raw: dict = data
             self.id: str = data["id"]
             self.name: str = data["name"]
-            self.owner: self.Owner = self.Owner(data["owner"])
+            self.owner: Owner = Owner(data["owner"])
             self.url: str = data["vanity_url"]
             self.verified: bool = data["verified"]
             self.created_at: int = data["created_at"]
             self.timezone: str = data["timezone"]
             self.slug: str = data["slug"]
             self.about: str = data["about"]
     
@@ -298,41 +315,24 @@
             description (str): The item's description.
             desc (str): An alias for the description.
             aliases (list): A list of all item aliases.
             _extradata (str): The extradata of the item.
             price (ItemPrice): Price data of the item.
         """
         def __init__(self, data):
-            class ItemPrice:
-                """
-                ItemPrice object.
-
-                Attributes:
-                    _raw (dict): Raw item price data, excluding worth.
-                    _price_parts (str): Raw item price data split.
-                    sell (str): The sell amount.
-                    buy (str): The buy amount.
-                    worth (str): The worth amount.
-                """
-                def __init__(self, price):
-                    self._raw: dict = price
-                    self._price_parts: list = price.split("|")
-                    self.sell: str = self._price_parts[0].strip()
-                    self.buy: str = self._price_parts[1].strip()
-                    self.worth: str = None
             self._raw: dict = data
             self._data: list = data.get(list(data.keys())[0])
             self.id: str = list(data.keys())[0]
             self.name: str = self._data[0]
             self.rarity: str = self._data[1]
             self.description: str = self._data[2]
             self.desc: str = self._data[2]
             self.aliases: list = self._data[3]
             self._extradata: str = self._data[4]
-            self.price: self.ItemPrice = self.ItemPrice(self._data[5])
+            self.price: ItemPrice = ItemPrice(self._data[5])
             self.price.worth: str = self._data[6]
 
     def fetch_items(self, hidden:bool=True) -> ItemsResult:
         """
         Fetches all items.
 
         Args:
```

### Comparing `econuker-1.0.1/econuker.egg-info/PKG-INFO` & `econuker-1.0.2/econuker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.1
+Version: 1.0.2
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.1/setup.py` & `econuker-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='econuker',
-    version='1.0.1',
+    version='1.0.2',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description='A Python library for interacting with EcoNuker\'s API.',
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
     classifiers=[
```

