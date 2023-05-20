# Comparing `tmp/acrod-1.1.1.tar.gz` & `tmp/acrod-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrod-1.1.1.tar", last modified: Sat May 20 11:58:21 2023, max compression
+gzip compressed data, was "acrod-1.1.2.tar", last modified: Sat May 20 12:02:25 2023, max compression
```

## Comparing `acrod-1.1.1.tar` & `acrod-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.046012 acrod-1.1.1/
--rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.1/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)    44790 2023-05-20 11:58:21.044962 acrod-1.1.1/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     3524 2023-05-20 11:54:40.000000 acrod-1.1.1/README.md
--rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-20 11:54:40.000000 acrod-1.1.1/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-20 11:58:21.046712 acrod-1.1.1/setup.cfg
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.009306 acrod-1.1.1/src/
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.019916 acrod-1.1.1/src/acrod/
--rw-r--r--   0 apple      (501) staff       (20)        0 2023-05-20 11:54:40.000000 acrod-1.1.1/src/acrod/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    42322 2023-05-20 11:54:40.000000 acrod-1.1.1/src/acrod/functions.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.032618 acrod-1.1.1/src/acrod.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    44790 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/top_level.txt
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.033871 acrod-1.1.1/tests/
--rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:54:40.000000 acrod-1.1.1/tests/test_jacobian.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:02:25.126052 acrod-1.1.2/
+-rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.2/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)    44791 2023-05-20 12:02:25.125024 acrod-1.1.2/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     3525 2023-05-20 12:00:08.000000 acrod-1.1.2/README.md
+-rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-20 12:00:14.000000 acrod-1.1.2/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-20 12:02:25.126557 acrod-1.1.2/setup.cfg
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:02:25.090668 acrod-1.1.2/src/
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:02:25.099857 acrod-1.1.2/src/acrod/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2023-05-20 11:54:40.000000 acrod-1.1.2/src/acrod/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    42322 2023-05-20 11:54:40.000000 acrod-1.1.2/src/acrod/functions.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:02:25.110684 acrod-1.1.2/src/acrod.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)    44791 2023-05-20 12:02:25.000000 acrod-1.1.2/src/acrod.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-20 12:02:25.000000 acrod-1.1.2/src/acrod.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-20 12:02:25.000000 acrod-1.1.2/src/acrod.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-20 12:02:25.000000 acrod-1.1.2/src/acrod.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-20 12:02:25.000000 acrod-1.1.2/src/acrod.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 12:02:25.112545 acrod-1.1.2/tests/
+-rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:54:40.000000 acrod-1.1.2/tests/test_jacobian.py
```

### Comparing `acrod-1.1.1/LICENSE` & `acrod-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acrod-1.1.1/PKG-INFO` & `acrod-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,15 +701,15 @@
 
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
-$$left[\begin{matrix}
+$$\left[\begin{matrix}
 9 & 1 & 0 \\
 1 & 9 & 1 \\
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
```

### Comparing `acrod-1.1.1/README.md` & `acrod-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
-$$left[\begin{matrix}
+$$\left[\begin{matrix}
 9 & 1 & 0 \\
 1 & 9 & 1 \\
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
```

### Comparing `acrod-1.1.1/pyproject.toml` & `acrod-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acrod"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Suneesh Jacob Akkarapakam", email="suneeshjacob@gmail.com" },
   { name="Rituparna Datta", email="rituparndatta@gmail.com" }
 ]
 description = "Automatic Computation for Robot Design (ACRoD)"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `acrod-1.1.1/src/acrod/functions.py` & `acrod-1.1.2/src/acrod/functions.py`

 * *Files identical despite different names*

### Comparing `acrod-1.1.1/src/acrod.egg-info/PKG-INFO` & `acrod-1.1.2/src/acrod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,15 +701,15 @@
 
 ## Usage
 
 ### Jacobian for planar manipulators
 
 The topological information of a robot is to be specified by using its robot-topology matrix, as defined [here](Robot_Topology_Matrix.md). For a planar 2R serial manipulator, the robot topology matrix is given by
 
-$$left[\begin{matrix}
+$$\left[\begin{matrix}
 9 & 1 & 0 \\
 1 & 9 & 1 \\
 0 & 1 & 9
 \end{matrix}\right]$$
 
 The corresponding Jacobian function can be formulated as follows.
```

### Comparing `acrod-1.1.1/tests/test_jacobian.py` & `acrod-1.1.2/tests/test_jacobian.py`

 * *Files identical despite different names*

