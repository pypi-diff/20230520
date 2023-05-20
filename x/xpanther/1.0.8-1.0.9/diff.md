# Comparing `tmp/xpanther-1.0.8.tar.gz` & `tmp/xpanther-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.0.8.tar", last modified: Fri May 19 18:14:05 2023, max compression
+gzip compressed data, was "xpanther-1.0.9.tar", last modified: Sat May 20 14:10:17 2023, max compression
```

## Comparing `xpanther-1.0.8.tar` & `xpanther-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.251338 xpanther-1.0.8/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     5475 2023-05-19 18:14:05.249321 xpanther-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5007 2023-05-19 18:13:20.000000 xpanther-1.0.8/README.md
--rw-rw-rw-   0        0        0      624 2023-05-19 17:53:50.000000 xpanther-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 18:14:05.251338 xpanther-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.206578 xpanther-1.0.8/xpanther/
--rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.8/xpanther/__init__.py
--rw-rw-rw-   0        0        0    19992 2023-05-19 17:48:05.000000 xpanther-1.0.8/xpanther/main.py
--rw-rw-rw-   0        0        0     4649 2023-05-19 17:53:16.000000 xpanther-1.0.8/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.247616 xpanther-1.0.8/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5475 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.930113 xpanther-1.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5539 2023-05-20 14:10:17.928337 xpanther-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.0.9/README.md
+-rw-rw-rw-   0        0        0      624 2023-05-20 14:06:27.000000 xpanther-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:10:17.930113 xpanther-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.879602 xpanther-1.0.9/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.9/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    19992 2023-05-19 17:48:05.000000 xpanther-1.0.9/xpanther/main.py
+-rw-rw-rw-   0        0        0     5411 2023-05-20 14:06:27.000000 xpanther-1.0.9/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.918523 xpanther-1.0.9/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5539 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.0.8/LICENSE` & `xpanther-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.8/PKG-INFO` & `xpanther-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.8
+Version: 1.0.9
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -98,15 +98,15 @@
 from xpanther import XPantherIDE
 ```
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
-#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again.
+#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.0.8/README.md` & `xpanther-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 from xpanther import XPantherIDE
 ```
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
-#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again.
+#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.0.8/pyproject.toml` & `xpanther-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Find Unique Xpath of any HTML/XML element"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xpanther-1.0.8/xpanther/main.py` & `xpanther-1.0.9/xpanther/main.py`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.8/xpanther/main_ide.py` & `xpanther-1.0.9/xpanther/main_ide.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from selenium import webdriver
 from xpanther import XPanther
 
 
 class XPantherIDE:
-    def __init__(self, page_url):
+    def __init__(self, page_url, custom_alert=True):
         self.__driver = webdriver.Chrome()
         self.__page_url = page_url
+        self.alert = custom_alert
 
     def wait_for_alert(self):
         for _ in range(100):
             try:
                 WebDriverWait(self.__driver, 1).until(ec.alert_is_present())
                 sleep(1)
             except TimeoutException:
@@ -65,34 +66,44 @@
                         current_url = new_url
                         self.__driver.execute_script(event_js)
                         self.__driver.execute_script(sweetalert_js)
                     return_value = WebDriverWait(self.__driver, 1).until(
                         lambda driver: self.__driver.execute_script(return_js)
                     )
                     if return_value:
-                        try:
-                            self.__driver.execute_script(
-                                """
-                                    Swal.fire({
-                                      position: 'top-end',
-                                      text: 'Capturing...',
-                                      })"""
-                            )
-                            xpath = XPanther(
-                                return_value[1], print_output=False, speed='fast'
-                            ).capture(return_value[0])[0]
-                            self.__driver.execute_script(
-                                f"""
-                                   Swal.fire({{
-                                      position: 'top-end',
-                                      text: '{xpath}',
-                                      timer: 10000,
-                                      }})"""
-                            )
-                        except WebDriverException:
+                        if self.alert:
+                            try:
+                                self.__driver.execute_script(
+                                    """
+                                        Swal.fire({
+                                          position: 'top-end',
+                                          text: 'Capturing...',
+                                          padding: '50'
+                                          })"""
+                                )
+                                xpath = XPanther(
+                                    return_value[1], print_output=False, speed='fast'
+                                ).capture(return_value[0])[0]
+                                self.__driver.execute_script(
+                                    f"""
+                                       Swal.fire({{
+                                          position: 'top-end',
+                                          text: '{xpath}',
+                                          timer: 10000,
+                                          padding: '50'
+                                          }})"""
+                                )
+                            except WebDriverException:
+                                self.__driver.execute_script("alert('Capturing...')")
+                                xpath = XPanther(
+                                    return_value[1], print_output=False, speed='fast'
+                                ).capture(return_value[0])[0]
+                                self.__driver.switch_to.alert.accept()
+                                self.__driver.execute_script(f"alert('{xpath}')")
+                        else:
                             self.__driver.execute_script("alert('Capturing...')")
                             xpath = XPanther(
                                 return_value[1], print_output=False, speed='fast'
                             ).capture(return_value[0])[0]
                             self.__driver.switch_to.alert.accept()
                             self.__driver.execute_script(f"alert('{xpath}')")
                         index += 1
```

### Comparing `xpanther-1.0.8/xpanther.egg-info/PKG-INFO` & `xpanther-1.0.9/xpanther.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.8
+Version: 1.0.9
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -98,15 +98,15 @@
 from xpanther import XPantherIDE
 ```
 Use:
 ```python
 XPantherIDE('page_url').start()
 ```   
     
-#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again.
+#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again. You can then just close the browser and the program terminates.
 
 ### **Both programs are open to improvements or new ideas!**
```

