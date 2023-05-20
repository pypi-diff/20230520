# Comparing `tmp/similarity-learning-0.0.1.tar.gz` & `tmp/similarity-learning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity-learning-0.0.1.tar", last modified: Thu May 18 08:48:00 2023, max compression
+gzip compressed data, was "similarity-learning-0.0.2.tar", last modified: Sat May 20 11:12:58 2023, max compression
```

## Comparing `similarity-learning-0.0.1.tar` & `similarity-learning-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:48:00.190674 similarity-learning-0.0.1/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-18 07:33:16.000000 similarity-learning-0.0.1/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-01-20 02:50:04.000000 similarity-learning-0.0.1/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4126 2023-05-18 08:48:00.190674 similarity-learning-0.0.1/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2436 2023-05-15 14:25:56.000000 similarity-learning-0.0.1/README.md
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1026 2023-04-22 13:31:11.000000 similarity-learning-0.0.1/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 08:48:00.190674 similarity-learning-0.0.1/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-01-20 02:50:04.000000 similarity-learning-0.0.1/setup.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:48:00.186673 similarity-learning-0.0.1/similarity_learning/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    10970 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       72 2023-04-18 22:10:56.000000 similarity-learning-0.0.1/similarity_learning/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/facenet.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/feature_space_plotting.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1492 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/pair_matching.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2408 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/siamese.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5459 2023-05-15 20:22:15.000000 similarity-learning-0.0.1/similarity_learning/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:48:00.190674 similarity-learning-0.0.1/similarity_learning.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4126 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:42:39.000000 similarity-learning-0.0.1/similarity_learning.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       64 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-05-18 08:48:00.000000 similarity-learning-0.0.1/similarity_learning.egg-info/top_level.txt
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-18 07:33:16.000000 similarity-learning-0.0.2/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-01-20 02:50:04.000000 similarity-learning-0.0.2/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4124 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2434 2023-05-20 11:12:23.000000 similarity-learning-0.0.2/README.md
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1026 2023-05-20 11:11:56.000000 similarity-learning-0.0.2/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-01-20 02:50:04.000000 similarity-learning-0.0.2/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.400035 similarity-learning-0.0.2/similarity_learning/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    10970 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       72 2023-04-18 22:10:56.000000 similarity-learning-0.0.2/similarity_learning/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1064 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/facenet.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1255 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/feature_space_plotting.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1492 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/pair_matching.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2408 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/siamese.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5459 2023-05-20 11:12:51.000000 similarity-learning-0.0.2/similarity_learning/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:12:58.404034 similarity-learning-0.0.2/similarity_learning.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4124 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      617 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       81 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:42:39.000000 similarity-learning-0.0.2/similarity_learning.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       64 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       20 2023-05-20 11:12:58.000000 similarity-learning-0.0.2/similarity_learning.egg-info/top_level.txt
```

### Comparing `similarity-learning-0.0.1/LICENSE` & `similarity-learning-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/PKG-INFO` & `similarity-learning-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -58,43 +58,43 @@
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
             <div>
               <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [14/14 00:04&lt;00:00]
+              100.00% [14/14 00:05&lt;00:00]
             </div>
             
         
-            (0.9800000190734863, 0.8493303656578064)
+            (1.0299999713897705, 0.8895089626312256)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.5396265387535095,0.8622449040412903]
+            (#2) [0.541471004486084,0.9005101919174194]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.29371750354766846,0.9285714030265808]
+            (#2) [0.2768465280532837,0.9464285969734192]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
         
@@ -103,15 +103,15 @@
         
         ``` python
         siamese.plot_distance_histogram(dls.valid)
         ```
         
             <div>
               <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [7/7 00:01&lt;00:00]
+              100.00% [7/7 00:02&lt;00:00]
             </div>
             
         
         ![](index_files/figure-commonmark/cell-10-output-2.png)
         
         See the rest of the docs for more examples, including more
         visualizations, comparison of loss functions, and facial recognition.
```

### Comparing `similarity-learning-0.0.1/README.md` & `similarity-learning-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
 siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
 siamese.fit_threshold(dls.train)
 ```
 
     <div>
       <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-      100.00% [14/14 00:04&lt;00:00]
+      100.00% [14/14 00:05&lt;00:00]
     </div>
     
 
-    (0.9800000190734863, 0.8493303656578064)
+    (1.0299999713897705, 0.8895089626312256)
 
 Let’s see how good it is:
 
 ``` python
 learn = Learner(dls, siamese, metrics=accuracy)
 learn.validate()
 ```
 
-    (#2) [0.5396265387535095,0.8622449040412903]
+    (#2) [0.541471004486084,0.9005101919174194]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-7-output-2.png)
 
 Not bad, but we can do better with finetuning:
 
 ``` python
 learn.fit(5, 1e-4)
 learn.validate()
 ```
 
-    (#2) [0.29371750354766846,0.9285714030265808]
+    (#2) [0.2768465280532837,0.9464285969734192]
 
 ``` python
 learn.show_results()
 ```
 
 ![](index_files/figure-commonmark/cell-9-output-2.png)
 
@@ -95,15 +95,15 @@
 
 ``` python
 siamese.plot_distance_histogram(dls.valid)
 ```
 
     <div>
       <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-      100.00% [7/7 00:01&lt;00:00]
+      100.00% [7/7 00:02&lt;00:00]
     </div>
     
 
 ![](index_files/figure-commonmark/cell-10-output-2.png)
 
 See the rest of the docs for more examples, including more
 visualizations, comparison of loss functions, and facial recognition.
```

### Comparing `similarity-learning-0.0.1/settings.ini` & `similarity-learning-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = similarity-learning
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = similarity_learning
```

### Comparing `similarity-learning-0.0.1/setup.py` & `similarity-learning-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/_modidx.py` & `similarity-learning-0.0.2/similarity_learning/_modidx.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/facenet.py` & `similarity-learning-0.0.2/similarity_learning/facenet.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/feature_space_plotting.py` & `similarity-learning-0.0.2/similarity_learning/feature_space_plotting.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/pair_matching.py` & `similarity-learning-0.0.2/similarity_learning/pair_matching.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/siamese.py` & `similarity-learning-0.0.2/similarity_learning/siamese.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning/utils.py` & `similarity-learning-0.0.2/similarity_learning/utils.py`

 * *Files identical despite different names*

### Comparing `similarity-learning-0.0.1/similarity_learning.egg-info/PKG-INFO` & `similarity-learning-0.0.2/similarity_learning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-learning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fastai based framework for similarity learning
 Home-page: https://github.com/Irad-Zehavi/similarity-learning
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: similarity-learning
         ================
@@ -58,43 +58,43 @@
         classifier = resnet34(weights=ResNet34_Weights.DEFAULT)
         siamese = ThresholdSiamese(create_body(model=classifier, cut=-1)).to(dls.device)
         siamese.fit_threshold(dls.train)
         ```
         
             <div>
               <progress value='14' class='' max='14' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [14/14 00:04&lt;00:00]
+              100.00% [14/14 00:05&lt;00:00]
             </div>
             
         
-            (0.9800000190734863, 0.8493303656578064)
+            (1.0299999713897705, 0.8895089626312256)
         
         Let’s see how good it is:
         
         ``` python
         learn = Learner(dls, siamese, metrics=accuracy)
         learn.validate()
         ```
         
-            (#2) [0.5396265387535095,0.8622449040412903]
+            (#2) [0.541471004486084,0.9005101919174194]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         Not bad, but we can do better with finetuning:
         
         ``` python
         learn.fit(5, 1e-4)
         learn.validate()
         ```
         
-            (#2) [0.29371750354766846,0.9285714030265808]
+            (#2) [0.2768465280532837,0.9464285969734192]
         
         ``` python
         learn.show_results()
         ```
         
         ![](index_files/figure-commonmark/cell-9-output-2.png)
         
@@ -103,15 +103,15 @@
         
         ``` python
         siamese.plot_distance_histogram(dls.valid)
         ```
         
             <div>
               <progress value='7' class='' max='7' style='width:300px; height:20px; vertical-align: middle;'></progress>
-              100.00% [7/7 00:01&lt;00:00]
+              100.00% [7/7 00:02&lt;00:00]
             </div>
             
         
         ![](index_files/figure-commonmark/cell-10-output-2.png)
         
         See the rest of the docs for more examples, including more
         visualizations, comparison of loss functions, and facial recognition.
```

### Comparing `similarity-learning-0.0.1/similarity_learning.egg-info/SOURCES.txt` & `similarity-learning-0.0.2/similarity_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

