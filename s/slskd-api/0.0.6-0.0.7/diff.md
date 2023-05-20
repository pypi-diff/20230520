# Comparing `tmp/slskd-api-0.0.6.tar.gz` & `tmp/slskd-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slskd-api-0.0.6.tar", last modified: Thu May 18 22:10:48 2023, max compression
+gzip compressed data, was "slskd-api-0.0.7.tar", last modified: Sat May 20 08:17:15 2023, max compression
```

## Comparing `slskd-api-0.0.6.tar` & `slskd-api-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:10:48.214290 slskd-api-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-18 22:10:36.000000 slskd-api-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-18 22:10:48.214290 slskd-api-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 22:10:36.000000 slskd-api-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:10:48.214290 slskd-api-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-18 22:10:36.000000 slskd-api-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:10:48.214290 slskd-api-0.0.6/slskd_api/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:10:48.214290 slskd-api-0.0.6/slskd_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/public_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/searches.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/apis/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-18 22:10:36.000000 slskd-api-0.0.6/slskd_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:10:48.214290 slskd-api-0.0.6/slskd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-18 22:10:48.000000 slskd-api-0.0.6/slskd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 22:10:48.000000 slskd-api-0.0.6/slskd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:10:48.000000 slskd-api-0.0.6/slskd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 22:10:48.000000 slskd-api-0.0.6/slskd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 22:10:48.000000 slskd-api-0.0.6/slskd_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.831958 slskd-api-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-20 08:16:58.000000 slskd-api-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 08:17:15.831958 slskd-api-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-20 08:16:58.000000 slskd-api-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:17:15.831958 slskd-api-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-20 08:16:58.000000 slskd-api-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.827957 slskd-api-0.0.7/slskd_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.831958 slskd-api-0.0.7/slskd_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/public_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.827957 slskd-api-0.0.7/slskd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/top_level.txt
```

### Comparing `slskd-api-0.0.6/LICENSE.md` & `slskd-api-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/PKG-INFO` & `slskd-api-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 License: GNU Affero General Public License v3.0
 Project-URL: Documentation, https://slskd-api.readthedocs.io
 Project-URL: Source, https://github.com/bigoulours/slskd-python-api
 Project-URL: Funding, https://liberapay.com/bigoulours/donate
 Requires-Python: >=3.7
```

### Comparing `slskd-api-0.0.6/README.md` & `slskd-api-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/setup.py` & `slskd-api-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/__init__.py` & `slskd-api-0.0.7/slskd_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/application.py` & `slskd-api-0.0.7/slskd_api/apis/application.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,32 +10,34 @@
         Gets the current state of the application.
         """
         url = self.api_url + '/application'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-# Getting Error 'Unauthorized' even with admin API-Key:
-    # def stop(self):
-    #     """
-    #     Stops the application.
-    #     """
-    #     url = self.api_url + '/application'
-    #     response = requests.delete(url, headers=self.header)
-    #     return response.ok
+    def stop(self) -> bool:
+        """
+        Stops the application. Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
+        
+        :return: True if successful.
+        """
+        url = self.api_url + '/application'
+        response = requests.delete(url, headers=self.header)
+        return response.ok
     
 
-# Getting Error 'Unauthorized' even with admin API-Key:
-    # def restart(self):
-    #     """
-    #     Restarts the application.
-    #     """
-    #     url = self.api_url + '/application'
-    #     response = requests.put(url, headers=self.header)
-    #     return response.json()
+    def restart(self) -> bool:
+        """
+        Restarts the application. Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
+        
+        :return: True if successful.
+        """
+        url = self.api_url + '/application'
+        response = requests.put(url, headers=self.header)
+        return response.ok
     
 
     def version(self) -> str:
         """
         Gets the current application version.
         """
         url = self.api_url + '/application/version'
```

### Comparing `slskd-api-0.0.6/slskd_api/apis/conversations.py` & `slskd-api-0.0.7/slskd_api/apis/conversations.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/options.py` & `slskd-api-0.0.7/slskd_api/apis/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from .base import *
 
-class OptionsApi(BaseApi):
+class ServerApi(BaseApi):
     """
-    This class contains the methods to interact with the Options API.
+    This class contains the methods to interact with the Search API.
     """
 
-    def get(self) -> dict:
+    def connect(self) -> bool:
         """
-        Gets the current application options.
+        Connects the client.
+
+        :return: True if successful.
         """
-        url = self.api_url + '/options'
-        response = requests.get(url, headers=self.header)
-        return response.json()
+        url = self.api_url + '/server'
+        response = requests.put(url, headers=self.header)
+        return response.ok
     
 
-    def get_startup(self) -> dict:
+    def disconnect(self) -> bool:
         """
-        Gets the application options provided at startup.
+        Disconnects the client.
+
+        :return: True if successful.
         """
-        url = self.api_url + '/options/startup'
-        response = requests.get(url, headers=self.header)
-        return response.json()
+        url = self.api_url + '/server'
+        response = requests.delete(url, headers=self.header, json='')
+        return response.ok
+    
 
-  
-# Getting error 'Unauthorized':
-    # def get_debug(self) -> dict:
-    #     """
-    #     Gets the debug view of the current application options.
-    #     """
-    #     url = self.api_url + '/options/debug'
-    #     response = requests.get(url, headers=self.header)
-    #     return response.json()
-    
+    def state(self) -> dict:
+        """
+        Retrieves the current state of the server.
+        """
+        url = self.api_url + '/server'
+        response = requests.get(url, headers=self.header)
+        return response.json()
```

### Comparing `slskd-api-0.0.6/slskd_api/apis/public_chat.py` & `slskd-api-0.0.7/slskd_api/apis/public_chat.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/relay.py` & `slskd-api-0.0.7/slskd_api/apis/relay.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/rooms.py` & `slskd-api-0.0.7/slskd_api/apis/rooms.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/searches.py` & `slskd-api-0.0.7/slskd_api/apis/searches.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/server.py` & `slskd-api-0.0.7/slskd_api/apis/shares.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,63 @@
 from .base import *
 
-class ServerApi(BaseApi):
+class SharesApi(BaseApi):
     """
-    This class contains the methods to interact with the Search API.
+    This class contains the methods to interact with the Shares API.
     """
 
-    def connect(self) -> bool:
+    def get_all(self) -> dict:
         """
-        Connects the client.
+        Gets the current list of shares.
+        """
+        url = self.api_url + '/shares'
+        response = requests.get(url, headers=self.header)
+        return response.json()
+    
+
+    def start_scan(self) -> bool:
+        """
+        Initiates a scan of the configured shares.
 
         :return: True if successful.
         """
-        url = self.api_url + '/server'
+        url = self.api_url + '/shares'
         response = requests.put(url, headers=self.header)
         return response.ok
     
 
-    def disconnect(self) -> bool:
+    def cancel_scan(self) -> bool:
         """
-        Disconnects the client.
+        Cancels a share scan, if one is running.
 
         :return: True if successful.
         """
-        url = self.api_url + '/server'
-        response = requests.delete(url, headers=self.header, json='')
+        url = self.api_url + '/shares'
+        response = requests.delete(url, headers=self.header)
         return response.ok
     
 
-    def state(self) -> dict:
+    def get(self, id: str) -> dict:
+        """
+        Gets the share associated with the specified id.
+        """
+        url = self.api_url + f'/shares/{id}'
+        response = requests.get(url, headers=self.header)
+        return response.json()
+    
+
+    def all_contents(self) -> list:
+        """
+        Returns a list of all shared directories and files.
+        """
+        url = self.api_url + '/shares/contents'
+        response = requests.get(url, headers=self.header)
+        return response.json()
+    
+
+    def contents(self, id: str) -> list:
         """
-        Retrieves the current state of the server.
+        Gets the contents of the share associated with the specified id.
         """
-        url = self.api_url + '/server'
+        url = self.api_url + f'/shares/{id}/contents'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.6/slskd_api/apis/session.py` & `slskd-api-0.0.7/slskd_api/apis/session.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/apis/shares.py` & `slskd-api-0.0.7/slskd_api/apis/users.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from .base import *
 
-class SharesApi(BaseApi):
+class UsersApi(BaseApi):
     """
-    This class contains the methods to interact with the Shares API.
+    This class contains the methods to interact with the Users API.
     """
 
-    def get_all(self) -> dict:
+    def address(self, username: str) -> dict:
         """
-        Gets the current list of shares.
+        Retrieves the address of the specified username.
         """
-        url = self.api_url + '/shares'
+        url = self.api_url + f'/users/{username}/endpoint'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def start_scan(self) -> bool:
+    def browse(self, username: str) -> dict:
         """
-        Initiates a scan of the configured shares.
-
-        :return: True if successful.
+        Retrieves the files shared by the specified username.
         """
-        url = self.api_url + '/shares'
-        response = requests.put(url, headers=self.header)
-        return response.ok
+        url = self.api_url + f'/users/{username}/browse'
+        response = requests.get(url, headers=self.header)
+        return response.json()
     
 
-    def cancel_scan(self) -> bool:
-        """
-        Cancels a share scan, if one is running.
-
-        :return: True if successful.
-        """
-        url = self.api_url + '/shares'
-        response = requests.delete(url, headers=self.header)
-        return response.ok
+# Getting Error 404 'Not Found' 
+    # def browsing_status(self, username: str):
+    #     """
+    #     Retrieves the status of the current browse operation for the specified username, if any.
+    #     """
+    #     url = self.api_url + f'/users/{username}/browse/status'
+    #     response = requests.get(url, headers=self.header)
+    #     return response.json()
     
 
-    def get(self, id: str) -> dict:
+    def directory(self, username: str, directory: str) -> dict:
         """
-        Gets the share associated with the specified id.
+        Retrieves the files from the specified directory from the specified username.
         """
-        url = self.api_url + f'/shares/{id}'
-        response = requests.get(url, headers=self.header)
+        url = self.api_url + f'/users/{username}/directory'
+        data = {
+            "directory": directory
+        }
+        response = requests.post(url, headers=self.header, json=data)
         return response.json()
     
 
-    def all_contents(self) -> list:
+    def info(self, username: str) -> dict:
         """
-        Returns a list of all shared directories and files.
+        Retrieves information about the specified username.
         """
-        url = self.api_url + '/shares/contents'
+        url = self.api_url + f'/users/{username}/info'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def contents(self, id: str) -> list:
+    def status(self, username: str) -> dict:
         """
-        Gets the contents of the share associated with the specified id.
+        Retrieves status for the specified username.
         """
-        url = self.api_url + f'/shares/{id}/contents'
+        url = self.api_url + f'/users/{username}/status'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.6/slskd_api/apis/transfers.py` & `slskd-api-0.0.7/slskd_api/apis/transfers.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.6/slskd_api/client.py` & `slskd-api-0.0.7/slskd_api/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,39 @@
 from base64 import b64encode
 from slskd_api.apis import *
 
 class SlskdClient:
     """
     The main class that allows access to the different APIs of a slskd instance.
     An API-Key with appropriate permissions (`readwrite` for most use cases) must be set in slskd config file.
+    Alternatively, provide your username and password.
     Usage::
         slskd = slskd_api.SlskdClient(host, api_key, url_base)
         app_status = slskd.application.state()
     """
 
     def __init__(self,
                  host: str,
-                 api_key: str,
-                 url_base: str = '/'
+                 api_key: str = None,
+                 url_base: str = '/',
+                 username: str = None,
+                 password: str = None,
     ):
         api_url = reduce(urljoin, [host, f'{url_base}/', f'api/{API_VERSION}'])
-        header = {
-            'accept': '*/*',
-            'X-API-Key': api_key
-        }
+     
+        header = {'accept': '*/*'}
+
+        if api_key:
+            header['X-API-Key'] = api_key
+        elif username and password:
+            header['Authorization'] = 'Bearer ' + \
+                            SessionApi(api_url, header).login(username, password)['token']
+        else:
+            raise ValueError('Please provide an API-Key or a valid username/password pair.')
+        
         base_args = (api_url, header)
         
         self.application = ApplicationApi(*base_args)
         self.conversations = ConversationsApi(*base_args)
         self.logs = LogsApi(*base_args)
         self.options = OptionsApi(*base_args)
         self.public_chat = PublicChatApi(*base_args)
```

### Comparing `slskd-api-0.0.6/slskd_api.egg-info/PKG-INFO` & `slskd-api-0.0.7/slskd_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 License: GNU Affero General Public License v3.0
 Project-URL: Documentation, https://slskd-api.readthedocs.io
 Project-URL: Source, https://github.com/bigoulours/slskd-python-api
 Project-URL: Funding, https://liberapay.com/bigoulours/donate
 Requires-Python: >=3.7
```

### Comparing `slskd-api-0.0.6/slskd_api.egg-info/SOURCES.txt` & `slskd-api-0.0.7/slskd_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

