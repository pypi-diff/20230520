# Comparing `tmp/acrod-1.1.0.tar.gz` & `tmp/acrod-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrod-1.1.0.tar", last modified: Sat May 20 11:47:05 2023, max compression
+gzip compressed data, was "acrod-1.1.1.tar", last modified: Sat May 20 11:58:21 2023, max compression
```

## Comparing `acrod-1.1.0.tar` & `acrod-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:47:05.422167 acrod-1.1.0/
--rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.0/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)    44788 2023-05-20 11:47:05.420608 acrod-1.1.0/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     3522 2023-05-20 11:46:15.000000 acrod-1.1.0/README.md
--rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-20 11:43:51.000000 acrod-1.1.0/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-20 11:47:05.423511 acrod-1.1.0/setup.cfg
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:47:05.393460 acrod-1.1.0/src/
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:47:05.401889 acrod-1.1.0/src/acrod/
--rw-r--r--   0 apple      (501) staff       (20)        0 2023-04-18 02:54:34.000000 acrod-1.1.0/src/acrod/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    42322 2023-05-20 08:16:37.000000 acrod-1.1.0/src/acrod/functions.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:47:05.411996 acrod-1.1.0/src/acrod.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    44788 2023-05-20 11:47:05.000000 acrod-1.1.0/src/acrod.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-20 11:47:05.000000 acrod-1.1.0/src/acrod.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-20 11:47:05.000000 acrod-1.1.0/src/acrod.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-20 11:47:05.000000 acrod-1.1.0/src/acrod.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-20 11:47:05.000000 acrod-1.1.0/src/acrod.egg-info/top_level.txt
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:47:05.413163 acrod-1.1.0/tests/
--rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:18:28.000000 acrod-1.1.0/tests/test_jacobian.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.046012 acrod-1.1.1/
+-rw-r--r--   0 apple      (501) staff       (20)    35149 2023-04-12 12:17:39.000000 acrod-1.1.1/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)    44790 2023-05-20 11:58:21.044962 acrod-1.1.1/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     3524 2023-05-20 11:54:40.000000 acrod-1.1.1/README.md
+-rw-r--r--   0 apple      (501) staff       (20)      873 2023-05-20 11:54:40.000000 acrod-1.1.1/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-05-20 11:58:21.046712 acrod-1.1.1/setup.cfg
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.009306 acrod-1.1.1/src/
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.019916 acrod-1.1.1/src/acrod/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2023-05-20 11:54:40.000000 acrod-1.1.1/src/acrod/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    42322 2023-05-20 11:54:40.000000 acrod-1.1.1/src/acrod/functions.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.032618 acrod-1.1.1/src/acrod.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)    44790 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      264 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       12 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        6 2023-05-20 11:58:20.000000 acrod-1.1.1/src/acrod.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-20 11:58:21.033871 acrod-1.1.1/tests/
+-rw-r--r--   0 apple      (501) staff       (20)   236428 2023-05-20 11:54:40.000000 acrod-1.1.1/tests/test_jacobian.py
```

### Comparing `acrod-1.1.0/LICENSE` & `acrod-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acrod-1.1.0/PKG-INFO` & `acrod-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -715,25 +715,28 @@
 
 Firstly, the required functions are imported as shown below.
 ```py
 from src.acrod.functions import jacobian
 from numpy import matrix
 ```
 
+
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
 jac = jacobian(M, robot_type = 'planar')
 ```
 
+
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
+
 Symbolic Jacobian is extracted from `jacobian_information` as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
@@ -758,35 +761,34 @@
 robot_dimensional_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}r_{(1,2)x} \\\\ r_{(1,2)y} \\\\ r_{(2,3)x} \\\\ r_{(2,3)y}\end{matrix}\right]$$
 
+
 Robot end-effector parameters can be viewed by running the below line.
 ```py
 robot_endeffector_parameters = jac.endeffector_variables_symbolic
 robot_endeffector_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}a_{x} \\\\ a_{y}\end{matrix}\right]$$
 
 #### Sample computation of Jacobian at the end-effector point $\textbf{a}=\hat{i}+2\hat{j}$ and at the configuration of $\textbf{r}\_{(1,2)}=3\hat{i}+4\hat{j}$ and $\textbf{r}\_{(2,3)}=5\hat{i}+6\hat{j}$
 
 For the given set of dimensional parameters of the robot, the numerical Jacobian can be computed as follows.
-
 ```py
 end_effector_point = [1,2]
 configuration_parameters = [3,4,5,6]
 jacobian_at_the_given_configuration = jacobian_function(end_effector_point, configuration_parameters)
 jacobian_at_the_given_configuration
 ```
 
 The output produced by running the above code, is shown below.
-
 ```py
 array([[ 2,  4],
        [-2, -4],
        [ 1,  1]])
 ```
```

### Comparing `acrod-1.1.0/README.md` & `acrod-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,25 +24,28 @@
 
 Firstly, the required functions are imported as shown below.
 ```py
 from src.acrod.functions import jacobian
 from numpy import matrix
 ```
 
+
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
 jac = jacobian(M, robot_type = 'planar')
 ```
 
+
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
+
 Symbolic Jacobian is extracted from `jacobian_information` as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
@@ -67,35 +70,34 @@
 robot_dimensional_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}r_{(1,2)x} \\\\ r_{(1,2)y} \\\\ r_{(2,3)x} \\\\ r_{(2,3)y}\end{matrix}\right]$$
 
+
 Robot end-effector parameters can be viewed by running the below line.
 ```py
 robot_endeffector_parameters = jac.endeffector_variables_symbolic
 robot_endeffector_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}a_{x} \\\\ a_{y}\end{matrix}\right]$$
 
 #### Sample computation of Jacobian at the end-effector point $\textbf{a}=\hat{i}+2\hat{j}$ and at the configuration of $\textbf{r}\_{(1,2)}=3\hat{i}+4\hat{j}$ and $\textbf{r}\_{(2,3)}=5\hat{i}+6\hat{j}$
 
 For the given set of dimensional parameters of the robot, the numerical Jacobian can be computed as follows.
-
 ```py
 end_effector_point = [1,2]
 configuration_parameters = [3,4,5,6]
 jacobian_at_the_given_configuration = jacobian_function(end_effector_point, configuration_parameters)
 jacobian_at_the_given_configuration
 ```
 
 The output produced by running the above code, is shown below.
-
 ```py
 array([[ 2,  4],
        [-2, -4],
        [ 1,  1]])
 ```
```

### Comparing `acrod-1.1.0/pyproject.toml` & `acrod-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acrod"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Suneesh Jacob Akkarapakam", email="suneeshjacob@gmail.com" },
   { name="Rituparna Datta", email="rituparndatta@gmail.com" }
 ]
 description = "Automatic Computation for Robot Design (ACRoD)"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `acrod-1.1.0/src/acrod/functions.py` & `acrod-1.1.1/src/acrod/functions.py`

 * *Files identical despite different names*

### Comparing `acrod-1.1.0/src/acrod.egg-info/PKG-INFO` & `acrod-1.1.1/src/acrod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrod
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automatic Computation for Robot Design (ACRoD)
 Author-email: Suneesh Jacob Akkarapakam <suneeshjacob@gmail.com>, Rituparna Datta <rituparndatta@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -715,25 +715,28 @@
 
 Firstly, the required functions are imported as shown below.
 ```py
 from src.acrod.functions import jacobian
 from numpy import matrix
 ```
 
+
 The robot-topology matrix for 3R planar serial manipulator is defined and jacobian information is processed via the imported jacobian class as follows.
 ```py
 M = matrix('9 1 0;1 9 1;0 1 9')
 jac = jacobian(M, robot_type = 'planar')
 ```
 
+
 Jacobian function is generated as shown below.
 ```py
 jacobian_function = jac.get_jacobian_function()
 ```
 
+
 Symbolic Jacobian is extracted from `jacobian_information` as follows.
 ```py
 symbolic_jacobian = jac.Ja
 symbolic_jacobian
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
@@ -758,35 +761,34 @@
 robot_dimensional_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}r_{(1,2)x} \\\\ r_{(1,2)y} \\\\ r_{(2,3)x} \\\\ r_{(2,3)y}\end{matrix}\right]$$
 
+
 Robot end-effector parameters can be viewed by running the below line.
 ```py
 robot_endeffector_parameters = jac.endeffector_variables_symbolic
 robot_endeffector_parameters
 ```
 
 In an ipynb file of JupyterLab, the above code would produce the following output.
 
 $$\left[\begin{matrix}a_{x} \\\\ a_{y}\end{matrix}\right]$$
 
 #### Sample computation of Jacobian at the end-effector point $\textbf{a}=\hat{i}+2\hat{j}$ and at the configuration of $\textbf{r}\_{(1,2)}=3\hat{i}+4\hat{j}$ and $\textbf{r}\_{(2,3)}=5\hat{i}+6\hat{j}$
 
 For the given set of dimensional parameters of the robot, the numerical Jacobian can be computed as follows.
-
 ```py
 end_effector_point = [1,2]
 configuration_parameters = [3,4,5,6]
 jacobian_at_the_given_configuration = jacobian_function(end_effector_point, configuration_parameters)
 jacobian_at_the_given_configuration
 ```
 
 The output produced by running the above code, is shown below.
-
 ```py
 array([[ 2,  4],
        [-2, -4],
        [ 1,  1]])
 ```
```

### Comparing `acrod-1.1.0/tests/test_jacobian.py` & `acrod-1.1.1/tests/test_jacobian.py`

 * *Files identical despite different names*

