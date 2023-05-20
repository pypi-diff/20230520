# Comparing `tmp/PySciMath-1.5.3.tar.gz` & `tmp/PySciMath-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.3.tar", last modified: Sun May 14 06:48:17 2023, max compression
+gzip compressed data, was "PySciMath-1.5.4.tar", last modified: Sat May 20 11:55:54 2023, max compression
```

## Comparing `PySciMath-1.5.3.tar` & `PySciMath-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.606293 PySciMath-1.5.3/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2591 2023-05-14 06:48:17.605294 PySciMath-1.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.585351 PySciMath-1.5.3/PySciMath/
--rw-rw-rw-   0        0        0     2090 2023-05-12 06:15:13.000000 PySciMath-1.5.3/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    22383 2023-05-12 03:54:01.000000 PySciMath-1.5.3/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.3/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.5.3/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.3/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.3/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.602304 PySciMath-1.5.3/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2077 2023-05-14 06:47:22.000000 PySciMath-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 06:48:17.607289 PySciMath-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-14 06:47:18.000000 PySciMath-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.351907 PySciMath-1.5.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2611 2023-05-20 11:55:54.349910 PySciMath-1.5.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.334072 PySciMath-1.5.4/PySciMath/
+-rw-rw-rw-   0        0        0     2667 2023-05-20 11:39:33.000000 PySciMath-1.5.4/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    22263 2023-05-20 11:31:14.000000 PySciMath-1.5.4/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.4/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1266 2023-05-20 11:31:27.000000 PySciMath-1.5.4/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.4/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.4/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.347916 PySciMath-1.5.4/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2611 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2077 2023-05-20 11:50:42.000000 PySciMath-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 11:55:54.351907 PySciMath-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-05-20 11:54:07.000000 PySciMath-1.5.4/setup.py
```

### Comparing `PySciMath-1.5.3/LICENSE.txt` & `PySciMath-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.3/PKG-INFO` & `PySciMath-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.3
+Version: 1.5.4
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Math,Calculations
+Keywords: Math,Mathematics,Science,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PySciMath
 
 ## Introduction
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.3</br>
+**Version** - 1.5.4</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.3/PySciMath/Arithmetic.py` & `PySciMath-1.5.4/PySciMath/Arithmetic.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ''' This is the "Arithmetic" sub-module. '''
 
 # Imports
 import cmath
 
 # Constants
-iota = "Iota, which is also referred to as 'i'. It's value is √-1."
+iota = "Iota is also referred to as 'i'. It's value is √-1."
 
 # Functions - Simple Arithmetic Operations
 def add(num1, num2): return num1 + num2
 def subtract(num1, num2): return num1 - num2
 def multiply(num1, num2): return num1 * num2
 def divide(num1, num2): return num1 / num2
 def modulus(num1, num2): return num1 % num2
@@ -38,40 +38,68 @@
     f = 1
 
     for i in range(1, number + 1):
         f = f * i
 
     return f
 
-# Function 2 - HCF
+# Function 2 - Fibonacci
+def fibonacci(terms):
+    if (isinstance(terms, int)):
+        if (terms == 0):
+            return None
+        elif (terms == 1):
+            return [0]
+        elif (terms == 2):
+            return [0, 1]
+        else:
+            f = 0
+            s = 1
+
+            list = [f, s]
+
+            for i in range(2, terms):
+                t = f + s
+
+                list.append(t)
+
+                f = s
+                s = t
+
+            return list
+    else:
+        raise Exception("The 'terms' argument must be an integer.")
+
+# Function 3 - HCF
 def hcf(num1, num2):
     hcf = 1
 
     for i in range(1, min(num1, num2)):
         if num1 % i == 0 and num2 % i == 0:
             hcf = i
 
     return hcf
 
-# Function 3 - LCM
+# Function 4 - LCM
 def lcm(num1, num2):
     if (num1 > num2):
         greater = num1
     else:
         greater = num2
 
     while True:
         if ((greater % num1 == 0) and (greater % num2 == 0)):
             lcm = greater
             break
+
         greater += 1
 
     return lcm
 
-# Function 4 - Prime
+# Function 5 - Prime
 def isPrime(number):
     isPrime = False
 
     if (number < 1):
         isPrime = False
     else:
         for i in range(2, int(number/2) + 1):
```

### Comparing `PySciMath-1.5.3/PySciMath/Geometry.py` & `PySciMath-1.5.4/PySciMath/Geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,69 +22,69 @@
             shape = kwargs["shape"]
 
             if (shape == "square"): # Square
                 if ("side" in keyList):
                     if (isinstance(kwargs["side"], (int, float))):
                         return kwargs["side"] * kwargs["side"]
                     else:
-                        raise Exception("The 'side' argument should be an integer or float.")
+                        raise Exception("The 'side' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a square, the 'side' argument should be present.")
+                    raise Exception("To check the area of a square, the 'side' argument must be present.")
             elif (shape == "rectangle"): # Rectangle
                 if ("length" in keyList and "width" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float))):
                         return kwargs["length"] * kwargs["width"]
                     else:
-                        raise Exception("The 'length' and 'width' arguments should be an integer or float.")
+                        raise Exception("The 'length' and 'width' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a rectangle, the 'length' and 'width' arguments should be present.")
+                    raise Exception("To check the area of a rectangle, the 'length' and 'width' arguments must be present.")
             elif (shape == "triangle"): # Triangle
                 if ("base" in keyList and "height" in keyList):
                     if (isinstance(kwargs["base"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 0.5 * kwargs["base"] * kwargs["height"]
                     else:
-                        raise Exception("The 'base' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'base' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a triangle, the 'base' and 'height' arguments should be present.")
+                    raise Exception("To check the area of a triangle, the 'base' and 'height' arguments must be present.")
             elif (shape == "circle"): # Circle
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         return 3.14 * Arithmetic.power(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer or float.")
+                        raise Exception("The 'radius' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a circle, the 'radius' argument should be present.")
+                    raise Exception("To check the area of a circle, the 'radius' argument must be present.")
             elif (shape == "parallelogram"): # Parallelogram
                 if ("base" in keyList and "height" in keyList):
                     if (isinstance(kwargs["base"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return kwargs["base"] * kwargs["height"]
                     else:
-                        raise Exception("The 'base' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'base' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a parallelogram, the 'base' and 'height' arguments should be present.")
+                    raise Exception("To check the area of a parallelogram, the 'base' and 'height' arguments must be present.")
             elif (shape == "trapezium"): # Trapezium
                 if ("base1" in keyList and "base2" in keyList and "height" in keyList):
                     if (isinstance(kwargs["base1"], (int, float)) and isinstance(kwargs["base2"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 0.5 * kwargs["height"] * (kwargs["base1"] + kwargs["base2"])
                     else:
-                        raise Exception("The 'base1', 'base2', and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'base1', 'base2', and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a trapezium, the 'base1', 'base2', and 'height' arguments should be present.")
+                    raise Exception("To check the area of a trapezium, the 'base1', 'base2', and 'height' arguments must be present.")
             elif (shape == "rhombus"): # Rhombus
                 if ("diagonal1" in keyList and "diagonal2" in keyList):
                     if (isinstance(kwargs["diagonal1"], (int, float)) and isinstance(kwargs["diagonal2"], (int, float))):
                         return (kwargs["diagonal1"] * kwargs["diagonal2"]) / 2
                     else:
-                        raise Exception("The 'diagonal' and 'diagonal2' arguments should be an integer or float.")
+                        raise Exception("The 'diagonal' and 'diagonal2' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the area of a rhombus, the 'diagonal1' and 'diagonal2' arguments should be present.")
+                    raise Exception("To check the area of a rhombus, the 'diagonal1' and 'diagonal2' arguments must be present.")
         else:
-            raise Exception("The 'shape' argument should be a square, rectangle, triangle, circle, parallelogram, trapezium, or rhombus.")
+            raise Exception("The 'shape' argument must be a square, rectangle, triangle, circle, parallelogram, trapezium, or rhombus.")
     else:
-        raise Exception("The 'shape' argument should be present in this function.")
+        raise Exception("The 'shape' argument must be present in this function.")
 
 # Function 2 - Volume (Areas and Volumes)
 def volume(**kwargs):
     shapeList = ["cube", "cuboid", "cone", "cylinder", "sphere", "hemisphere", "pyramid"]
     keyList = []
 
     for key, value in kwargs.items():
@@ -95,69 +95,69 @@
             shape = kwargs["shape"]
 
             if (shape == "cube"): # Cube
                 if ("side" in keyList):
                     if (isinstance(kwargs["side"], (int, float))):
                         return Arithmetic.power(kwargs["side"], 3)
                     else:
-                        raise Exception("The 'side' argument should be an integer or float.")
+                        raise Exception("The 'side' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a cube, the 'side' argument should be present.")
+                    raise Exception("To check the volume of a cube, the 'side' argument must be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return kwargs["length"] * kwargs["width"] * kwargs["height"]
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'length', 'width', and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a cuboid, the 'length', 'width', and 'height' arguments should be present.")
+                    raise Exception("To check the volume of a cuboid, the 'length', 'width', and 'height' arguments must be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return (1/3) * 3.14 * Arithmetic.power(kwargs["radius"], 2) * kwargs["height"]
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a cone, the 'radius' and 'height' arguments should be present.")
+                    raise Exception("To check the volume of a cone, the 'radius' and 'height' arguments must be present.")
             elif (shape == "cylinder"): # Cylinder
                 if ("radius" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return 3.14 * Arithmetic.power(kwargs["radius"], 2) * kwargs["height"]
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a cylinder, the 'radius' and 'height' arguments should be present.")
+                    raise Exception("To check the volume of a cylinder, the 'radius' and 'height' arguments must be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         return (4/3) * 3.14 * Arithmetic.power(kwargs["radius"], 3)
                     else:
-                        raise Exception("The 'radius' argument should be an integer or float.")
+                        raise Exception("The 'radius' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a sphere, the 'radius' argument should be present.")
+                    raise Exception("To check the volume of a sphere, the 'radius' argument must be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         return (2/3) * 3.14 * Arithmetic.power(kwargs["radius"], 3)
                     else:
-                        raise Exception("The 'radius' argument should be an integer or float.")
+                        raise Exception("The 'radius' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a hemisphere, the 'radius' argument should be present.")
+                    raise Exception("To check the volume of a hemisphere, the 'radius' argument must be present.")
             elif (shape == "pyramid"): # Pyramid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         return (length * width * height) / 3
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'length', 'width', and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the volume of a pyramid, the 'length', 'width', and 'height' arguments should be present.")
+                    raise Exception("To check the volume of a pyramid, the 'length', 'width', and 'height' arguments must be present.")
         else:
-            raise Exception("The 'shape' argument should be a cube, cuboid, cone, cylinder, sphere, hemisphere, or pyramid.")
+            raise Exception("The 'shape' argument must be a cube, cuboid, cone, cylinder, sphere, hemisphere, or pyramid.")
     else:
-        raise Exception("The 'shape' argument should be present in this function.")
+        raise Exception("The 'shape' argument must be present in this function.")
 
 # Function 3 - Surface Area (Areas and Volumes)
 def surfaceArea(**kwargs):
     shapeList = ["cube", "cuboid", "cone", "cylinder", "sphere", "hemisphere"]
     keyList = []
 
     for key, value in kwargs.items():
@@ -173,112 +173,112 @@
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 4 * Arithmetic.power(side, 2)
                                 else:
                                     return 6 * Arithmetic.power(side, 2)
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 6 * Arithmetic.power(kwargs["side"], 2)
                     else:
-                        raise Exception("The 'side' argument should be an integer or float.")
+                        raise Exception("The 'side' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a cube, the 'side' argument should be present.")
+                    raise Exception("To check the surface area of a cube, the 'side' argument must be present.")
             elif (shape == "cuboid"): # Cuboid
                 if ("length" in keyList and "width" in keyList and "height" in keyList):
                     if (isinstance(kwargs["length"], (int, float)) and isinstance(kwargs["width"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * kwargs["height"] * (kwargs["length"] + kwargs["width"])
                                 else:
                                     return 2 * ((kwargs["length"] * kwargs["width"]) + (kwargs["width"] * kwargs["height"]) + (kwargs["length"] * kwargs["height"]))
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 2 * ((kwargs["length"] * kwargs["width"]) + (kwargs["width"] * kwargs["height"]) + (kwargs["length"] * kwargs["height"]))
                     else:
-                        raise Exception("The 'length', 'width', and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'length', 'width', and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a cuboid, the 'length', 'width', and 'height' arguments should be present.")
+                    raise Exception("To check the surface area of a cuboid, the 'length', 'width', and 'height' arguments must be present.")
             elif (shape == "cone"): # Cone
                 if ("raidus" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         slantHeight = Arithmetic.squareRoot(Arithmetic.power(kwargs["radius"], 2) + Arithmetic.power(kwargs["height"], 2))
 
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 3.14 * kwargs["radius"] * slantHeight
                                 else:
                                     return 3.14 * kwargs["radius"] * (slantHeight + kwargs["radius"])
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 3.14 * kwargs["radius"] * (slantHeight + kwargs["radius"])
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a cone, the 'radius' and 'height' arguments should be present.")
+                    raise Exception("To check the surface area of a cone, the 'radius' and 'height' arguments must be present.")
             elif (shape == "cylinder"): # Cylinder
                 if ("radius" in keyList and "height" in keyList):
                     if (isinstance(kwargs["radius"], (int, float)) and isinstance(kwargs["height"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * 3.14 * kwargs["radius"] * kwargs["height"]
                                 else:
                                     return 2 * 3.14 * kwargs["radius"] * (kwargs["radius"] + kwargs["height"])
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 2 * 3.14 * kwargs["radius"] * (kwargs["radius"] + kwargs["height"])
                     else:
-                        raise Exception("The 'radius' and 'height' arguments should be an integer or float.")
+                        raise Exception("The 'radius' and 'height' arguments must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a cylinder, the 'radius' and 'height' arguments should be present.")
+                    raise Exception("To check the surface area of a cylinder, the 'radius' and 'height' arguments must be present.")
             elif (shape == "sphere"): # Sphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                                 else:
                                     return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 4 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer or float.")
+                        raise Exception("The 'radius' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a sphere, the 'radius' argument should be present.")
+                    raise Exception("To check the surface area of a sphere, the 'radius' argument must be present.")
             elif (shape == "hemisphere"): # Hemisphere
                 if ("radius" in keyList):
                     if (isinstance(kwargs["radius"], (int, float))):
                         if ("lateral" in keyList):
                             if (isinstance(kwargs["lateral"], bool)):
                                 if (kwargs["lateral"] == True):
                                     return 2 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                                 else:
                                     return 3 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                             else:
-                                raise Exception("The 'lateral' argument should be either True or False.")
+                                raise Exception("The 'lateral' argument must be either True or False.")
                         else:
                             return 3 * 3.14 * Arithmetic.power(kwargs["radius"], 2)
                     else:
-                        raise Exception("The 'radius' argument should be an integer or float.")
+                        raise Exception("The 'radius' argument must be an integer or float.")
                 else:
-                    raise Exception("To check the surface area of a hemisphere, the 'radius' argument should be present.")
+                    raise Exception("To check the surface area of a hemisphere, the 'radius' argument must be present.")
         else:
-            raise Exception("The 'shape' argument should be a cube, cuboid, cone, cylinder, sphere, or hemisphere.")
+            raise Exception("The 'shape' argument must be a cube, cuboid, cone, cylinder, sphere, or hemisphere.")
     else:
-        raise Exception("The 'shape' argument should be present in this function.")
+        raise Exception("The 'shape' argument must be present in this function.")
 
 # Function 4 - Distance (Coordinate Geometry)
 def distance(point1, point2):
     distance = None
 
     if (isinstance(point1, tuple) and  isinstance(point2, tuple)):
         if (len(point1) == 2 and len(point2) == 2 or len(point1) == 3 and len(point2) == 3):
@@ -299,17 +299,17 @@
 
                 newZ = z2 - z1
 
                 distance = Arithmetic.squareRoot(Arithmetic.power(newX, 2) + Arithmetic.power(newY, 2) + Arithmetic.power(newZ, 2))
 
             return distance
         else:
-            raise Exception("Both tuples should be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
+            raise Exception("Both tuples must be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
     else:
-        raise TypeError("Both Point 1 and Point 2 should be in the form of a tuple.")
+        raise TypeError("Both Point 1 and Point 2 must be in the form of a tuple.")
 
 # Function 5 - Is Collinear (Coordinate Geometry)
 def isCollinear(point1, point2, point3):
     isCollinear = False
 
     if (isinstance(point1, tuple) and isinstance(point2, tuple) and isinstance(point2, tuple)):
         if (len(point1) == 2 and len(point2) == 2 or len(point1) == 3 and len(point2) == 3):
@@ -320,17 +320,17 @@
             if (point1point3 == point1point2 + point2point3):
                 isCollinear = True
             else:
                 isCollinear = False
 
             return isCollinear
         else:
-            raise Exception("The 3 tuples should be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
+            raise Exception("The 3 tuples must be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂).")
     else:
-        raise TypeError("The 3 points should be in the form of a tuple.")
+        raise TypeError("The 3 points must be in the form of a tuple.")
 
 # Function 6 - Section (Coordinate Geometry)
 def section(point1, point2, ratio, typeOfSection="Internal"):
     section = None
 
     if (typeOfSection == "Internal" or typeOfSection == "External"):
         if (isinstance(point1, tuple) and  isinstance(point2, tuple) and isinstance(ratio, tuple)):
@@ -366,19 +366,19 @@
                         section2 = ((m * y2) - (n * y1)) / (m - n)
                         section3 = ((m * z2) - (n * z1)) / (m - n)
 
                     section = (section1, section2, section3)
 
                 return section
             else:
-                raise Exception("Both tuples should be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂). The ratio should be in the form (m, n).")
+                raise Exception("Both tuples must be in the form (x₁, y₁) and (x₂, y₂) or (x₁, y₁, z₁) and (x₂, y₂, z₂). The ratio must be in the form (m, n).")
         else:
-            raise TypeError("Point 1, Point 2, and the Ratio should be in the form of a tuple.")
+            raise TypeError("Point 1, Point 2, and the Ratio must be in the form of a tuple.")
     else:
-        raise Exception("The paramater 'typeOfSection' should be either Internal or External.")
+        raise Exception("The paramater 'typeOfSection' must be either Internal or External.")
 
 # Functions - Circles
 def circumference(radius): return 2 * 3.14 * radius
 def diameter(radius): return 2 * radius
 def areaOfSector(angle, radius): return (angle / 360) * 3.14 * Arithmetic.power(radius, 2)
 def arcLength(angle, radius): return (angle / 360) * circumference(radius)
```

### Comparing `PySciMath-1.5.3/PySciMath/Quadratic.py` & `PySciMath-1.5.4/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.3/PySciMath/Statistics.py` & `PySciMath-1.5.4/PySciMath/Statistics.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 def mean(data):
     if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             return sum(data) / len(data)
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
     else:
-        raise TypeError("The data should be in the form of a list, tuple, or set.")
+        raise TypeError("The data must be in the form of a list, tuple, or set.")
 
 # Function 2 - Mode
 def mode(data):
     if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             return max(data)
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
     else:
-        raise TypeError("The data should be in the form of a list, tuple, or set.")
+        raise TypeError("The data must be in the form of a list, tuple, or set.")
 
 # Function 3 - Median
 def median(data):
     if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             data.sort()
             mid = len(data) // 2
 
             return (data[mid] + data[~mid]) / 2
         else:
             raise Exception("The data can't be null and the sum of the data can't be zero.")
     else:
-        raise TypeError("The data should be in the form of a list, tuple, or set.")
+        raise TypeError("The data must be in the form of a list, tuple, or set.")
```

### Comparing `PySciMath-1.5.3/PySciMath/Trigonometry.py` & `PySciMath-1.5.4/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.3/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.4/PySciMath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.3
+Version: 1.5.4
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Math,Calculations
+Keywords: Math,Mathematics,Science,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PySciMath
 
 ## Introduction
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.3</br>
+**Version** - 1.5.4</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.3/README.md` & `PySciMath-1.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.3</br>
+**Version** - 1.5.4</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

