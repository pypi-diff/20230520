# Comparing `tmp/YetAnotherModule-0.0.1.1.tar.gz` & `tmp/YetAnotherModule-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YetAnotherModule-0.0.1.1.tar", last modified: Sat May 20 16:31:11 2023, max compression
+gzip compressed data, was "YetAnotherModule-0.0.1.2.tar", last modified: Sat May 20 19:37:46 2023, max compression
```

## Comparing `YetAnotherModule-0.0.1.1.tar` & `YetAnotherModule-0.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/YAPM/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/Matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/Random.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.926689 YetAnotherModule-0.0.1.2/YAPM/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/Random.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/YAPM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 19:37:46.000000 YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:37:46.930689 YetAnotherModule-0.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-20 19:37:33.000000 YetAnotherModule-0.0.1.2/setup.py
```

### Comparing `YetAnotherModule-0.0.1.1/LICENSE` & `YetAnotherModule-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.1.1/PKG-INFO` & `YetAnotherModule-0.0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,23 +23,11 @@
 ## Downloading
 
 Run `pip install YetAnotherModule` to download from pip
 
 ### Importing
 ```python
 import YAPM
-a = YAPM.Matrix.Matrix(
-  [[1, 2, 3],
-   [4, 2, 4]]
-)
-
-b = YAPM.Matrix.Matrix(
-  [[9, 1],
-   [4, 1],
-   [3, 3]]
-)
-
-print((a * b))
 ```
 
 ## Licence
 This code is under the MIT licence. You can do whatever you want but I (Carson) am not liabile for anything that is done with this code.
```

### Comparing `YetAnotherModule-0.0.1.1/README.md` & `YetAnotherModule-0.0.1.2/YetAnotherModule.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-## Yet Another Python Module (YAPM)
-A module where I put random stuff. Feel free to update, add, or optimize stuff just keep the syntax the same.
-
-## Contributing
-If you want to contribue fork this repo and make a pull request.
-Make sure that your contribution
-
- - [ ] Keeps syntax the same (eg. function(a, b) should beable to be ran as function(a, b) without an error)
- - [ ] Useful
- - [ ] Doesn't make functions slower
-
-## Downloading
-
-Run `pip install YetAnotherModule` to download from pip
-
-### Importing
-```python
-import YAPM
-a = YAPM.Matrix.Matrix(
-  [[1, 2, 3],
-   [4, 2, 4]]
-)
-
-b = YAPM.Matrix.Matrix(
-  [[9, 1],
-   [4, 1],
-   [3, 3]]
-)
-
-print((a * b))
-```
-
-## Licence
-This code is under the MIT licence. You can do whatever you want but I (Carson) am not liabile for anything that is done with this code.
+Metadata-Version: 2.1
+Name: YetAnotherModule
+Version: 0.0.1.2
+Summary: Yet Another Python Module.
+Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
+Author: Carson
+Author-email: carsondpool@gmail.com
+License: LICENSE
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Yet Another Python Module (YAPM)
+A module where I put random stuff. Feel free to update, add, or optimize stuff just keep the syntax the same.
+
+## Contributing
+If you want to contribue fork this repo and make a pull request.
+Make sure that your contribution
+
+ - [ ] Keeps syntax the same (eg. function(a, b) should beable to be ran as function(a, b) without an error)
+ - [ ] Useful
+ - [ ] Doesn't make functions slower
+
+## Downloading
+
+Run `pip install YetAnotherModule` to download from pip
+
+### Importing
+```python
+import YAPM
+```
+
+## Licence
+This code is under the MIT licence. You can do whatever you want but I (Carson) am not liabile for anything that is done with this code.
```

### Comparing `YetAnotherModule-0.0.1.1/YAPM/Matrix.py` & `YetAnotherModule-0.0.1.2/YAPM/Matrix.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,38 +5,48 @@
 # Adds a matrix class
 # Used for math stuff.
 #
 
 # Multipling Rules
 # x=y
 
-class Matrix(): # 2d matrix
+
+class Matrix():  # 2d matrix
     """
     Creates A Matrix that can be used for many different math uses.
-     
-    :param MatrixValues: Sequence[Sequence[int]] - The values for the matrix (indexs y then x. like MatrixValues[y][x])
-    
-    :raises ValueError: MatrixValues isn't a 2d int list
+
+    :param MatrixValues:
+        Sequence[Sequence[int]] - The values for the matrix (indexs y then x.)
+
+    :raises ValueError:
+        MatrixValues isn't a 2d int list
     """
-    def __init__(self, MatrixValues: Sequence[Sequence[int]]):       
-        if not Random.RaisesError("int(Matrix[0][0])", GlobalVars = {"Matrix": MatrixValues})[0]:
+    def __init__(self, MatrixValues: Sequence[Sequence[int]]):
+        if not Random.RaisesError(
+            "int(Matrix[0][0])",
+            GlobalVars={"Matrix": MatrixValues}
+        )[0]:
             raise ValueError("Matrix has to be a Sequence[Sequence[int]]")
         self.matrix = MatrixValues
+
     def __mul__(self, other):
         """
         Multiply two matrices
         """
-        if not (Random.RaisesError("int(Matrix.matrix[0][0])", GlobalVars = {"Matrix": other})[0] and len(self.matrix[0]) == len(other.matrix)):
-            raise ValueError("X length of first matrix has to match Y length of second matrix. Or you arn't multiplying a matrix by a matrix or a class that has a matrix property that is a 2x2 list")
-        
-        MatrixValues = [[0]*len(other.matrix[0])]*len(self.matrix)
-        
+        if not len(self.matrix[0]) == len(other.matrix):
+            raise ValueError("X of first matrix needs to equal Y of second matrix.")
+        elif not Random.RaisesError("int(Matrix.matrix[0][0])", GlobalVars={"Matrix": other})[0]:
+            raise ValueError("Can only multiply a matrix by a matrix rn.")
+
+        MatrixValues = [[0] * len(other.matrix[0])] * len(self.matrix)
+
         for index, i in enumerate(self.matrix):
             values = [0] * len(other.matrix[0])
             for idx, b in enumerate(i):
                 for idx2, k in enumerate(other.matrix[idx]):
                     values[idx2] += int(b) * int(k)
             MatrixValues[index] = values
-            
+
         return (Matrix(MatrixValues))
+
     def __str__(self):
-        return str(self.matrix)   
+        return str(self.matrix)
```

### Comparing `YetAnotherModule-0.0.1.1/YAPM/Random.py` & `YetAnotherModule-0.0.1.2/YAPM/Random.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from collections.abc import Sequence
 
 #
 # Random Stuff
 #
 
-def RaisesError(code: str, Ignore: Sequence[Exception] = [None,], GlobalVars: dict[str, any] = {}):
+
+def RaisesError(code: str, Ignore: Sequence[Exception] = [], GlobalVars: dict[str, any] = {}):
     """
     Evaluates the code provited.
-    
+
     :param str code: str - The code to eval
     :param Sequence[Exception] Ignore: Exceptions to ignore
     :param dict[str, any] GlobalVars: Globals to pass into the eval function
 
     :returns:
         - Tuple[True, any] - Code ran without any errors. returns code result.
         - Tuple[True, Exception] - Code threw a error that is in the Ignored exceptions list
-        - Tuple[False, Exception] - Code threw a error that is not Ignored. 
-    
+        - Tuple[False, Exception] - Code threw a error that is not Ignored.'
+
     :raises:
         - ValueError - Ignore isn't a iterable
         - ValueError - GlobalVars isn't a dict
         - ValueError - Code isn't a string
     """
-    try: 
+    try:
         iter(Ignore)
-    except ValueError: 
+    except ValueError:
         raise ValueError("Ignore Should be an iterable")
-    try: 
+    try:
         dict(GlobalVars)
-    except ValueError: 
+    except ValueError:
         raise ValueError("GlobalVars Should be an dict")
     if not isinstance(code, str):
         raise ValueError("Code needs to be a string or isinstance(code, str) should return true")
-    
+
     try:
         Value = eval(compile(code, '<string>', 'eval'), GlobalVars)
     except Exception as e:
         if e in Ignore:
             return (True, e)
         else:
             return (False, e)
-    
+
     return (True, Value)
```

