# Comparing `tmp/jax-relax-0.1.4.tar.gz` & `tmp/jax-relax-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-relax-0.1.4.tar", last modified: Wed May 10 18:35:03 2023, max compression
+gzip compressed data, was "jax-relax-0.1.5.tar", last modified: Sat May 20 00:54:43 2023, max compression
```

## Comparing `jax-relax-0.1.4.tar` & `jax-relax-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/
--rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.4/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.4/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     3356 2023-05-10 18:35:03.853624 jax-relax-0.1.4/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     2515 2023-05-04 04:04:49.000000 jax-relax-0.1.4/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     3356 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.4/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      208 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/_ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)    83777 2023-05-10 18:28:51.000000 jax-relax-0.1.4/relax/_modidx.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/data/
--rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/loader.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19263 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/scm.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19678 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1341 2023-05-03 15:57:46.000000 jax-relax-0.1.4/relax/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/logger.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      361 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2319 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11533 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/cchvae.py
--rw-r--r--   0 birk      (1000) birk      (1000)    13916 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/clue.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12640 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6125 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/diverse.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9245 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7204 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11619 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/vaecf.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3699 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7736 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/plots.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4788 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8433 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1159 2023-05-10 18:24:07.000000 jax-relax-0.1.4/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-10 18:35:03.853624 jax-relax-0.1.4/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2603 2023-05-03 15:57:46.000000 jax-relax-0.1.4/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/
+-rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.5/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.5/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-05-20 00:54:43.023699 jax-relax-0.1.5/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     2608 2023-05-13 23:13:26.000000 jax-relax-0.1.5/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/jax_relax.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     3371 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.5/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      217 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-20 00:54:42.000000 jax-relax-0.1.5/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/
+-rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/_ckpt_manager.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    84243 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/_modidx.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/data/
+-rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/loader.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19548 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/data/scm.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/docs.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19678 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/evaluate.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1341 2023-05-03 15:57:46.000000 jax-relax-0.1.5/relax/import_essentials.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/logger.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-20 00:54:43.023699 jax-relax-0.1.5/relax/methods/
+-rw-r--r--   0 birk      (1000) birk      (1000)      361 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2319 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11822 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/cchvae.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    14314 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/clue.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12640 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/counternet.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6125 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/diverse.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9245 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/proto.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6893 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/sphere.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11617 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/vaecf.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3699 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/methods/vanilla.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9921 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/plots.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4938 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/trainer.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     8433 2023-05-20 00:54:23.000000 jax-relax-0.1.5/relax/utils.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1130 2023-05-20 00:52:05.000000 jax-relax-0.1.5/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-20 00:54:43.023699 jax-relax-0.1.5/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     2603 2023-05-03 15:57:46.000000 jax-relax-0.1.5/setup.py
```

### Comparing `jax-relax-0.1.4/CONTRIBUTING.md` & `jax-relax-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/LICENSE` & `jax-relax-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/PKG-INFO` & `jax-relax-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.1.4
+Version: 0.1.5
 Summary: Jax-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/relax/tree/master/
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# ReLax
+ReLax
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-relax.svg) ![CI
 status](https://github.com/BirkhoffG/ReLax/actions/workflows/test.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/ReLax/actions/workflows/deploy.yaml/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/jax-relax.svg) ![GitHub
```

### Comparing `jax-relax-0.1.4/README.md` & `jax-relax-0.1.5/jax_relax.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,31 @@
-# ReLax
+Metadata-Version: 2.1
+Name: jax-relax
+Version: 0.1.5
+Summary: Jax-based Recourse Explanation Library
+Home-page: https://github.com/birkhoffg/relax/tree/master/
+Author: BirkhoffG
+Author-email: 26811230+BirkhoffG@users.noreply.github.com
+License: Apache Software License 2.0
+Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+ReLax
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ![Python](https://img.shields.io/pypi/pyversions/jax-relax.svg) ![CI
 status](https://github.com/BirkhoffG/ReLax/actions/workflows/test.yaml/badge.svg)
 ![Docs](https://github.com/BirkhoffG/ReLax/actions/workflows/deploy.yaml/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/jax-relax.svg) ![GitHub
```

### Comparing `jax-relax-0.1.4/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.1.5/jax_relax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/_ckpt_manager.py` & `jax-relax-0.1.5/relax/_ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/_modidx.py` & `jax-relax-0.1.5/relax/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,17 @@
                                                                                            'relax/methods/sphere.py'),
                                       'relax.methods.sphere._growing_spheres': ( 'methods/sphere.html#_growing_spheres',
                                                                                  'relax/methods/sphere.py'),
                                       'relax.methods.sphere.apply_immutable': ( 'methods/sphere.html#apply_immutable',
                                                                                 'relax/methods/sphere.py'),
                                       'relax.methods.sphere.cat_sample': ('methods/sphere.html#cat_sample', 'relax/methods/sphere.py'),
                                       'relax.methods.sphere.hyper_sphere_coordindates': ( 'methods/sphere.html#hyper_sphere_coordindates',
-                                                                                          'relax/methods/sphere.py')},
+                                                                                          'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.sample_categorical': ( 'methods/sphere.html#sample_categorical',
+                                                                                   'relax/methods/sphere.py')},
             'relax.methods.vaecf': { 'relax.methods.vaecf.Decoder': ('methods/vaecf.html#decoder', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.Decoder.__call__': ( 'methods/vaecf.html#decoder.__call__',
                                                                                'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.Decoder.__init__': ( 'methods/vaecf.html#decoder.__init__',
                                                                                'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.Encoder': ('methods/vaecf.html#encoder', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.Encoder.__call__': ( 'methods/vaecf.html#encoder.__call__',
@@ -639,15 +641,17 @@
                               'relax.module.PredictiveTrainingModule.pred_fn': ( 'training_module.html#predictivetrainingmodule.pred_fn',
                                                                                  'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.training_step': ( 'training_module.html#predictivetrainingmodule.training_step',
                                                                                        'relax/module.py'),
                               'relax.module.PredictiveTrainingModule.validation_step': ( 'training_module.html#predictivetrainingmodule.validation_step',
                                                                                          'relax/module.py'),
                               'relax.module.PredictiveTrainingModuleConfigs': ( 'training_module.html#predictivetrainingmoduleconfigs',
-                                                                                'relax/module.py')},
+                                                                                'relax/module.py'),
+                              'relax.module.download_model': ('learning.html#download_model', 'relax/module.py'),
+                              'relax.module.load_pred_model': ('learning.html#load_pred_model', 'relax/module.py')},
             'relax.plots': { 'relax.plots._barplot': ('plotting.html#_barplot', 'relax/plots.py'),
                              'relax.plots._diff': ('plotting.html#_diff', 'relax/plots.py'),
                              'relax.plots._process_exp': ('plotting.html#_process_exp', 'relax/plots.py'),
                              'relax.plots._stripplot': ('plotting.html#_stripplot', 'relax/plots.py'),
                              'relax.plots._swarmplot': ('plotting.html#_swarmplot', 'relax/plots.py'),
                              'relax.plots.individual_plot': ('plotting.html#individual_plot', 'relax/plots.py'),
                              'relax.plots.summary_plot': ('plotting.html#summary_plot', 'relax/plots.py')},
```

### Comparing `jax-relax-0.1.4/relax/data/loader.py` & `jax-relax-0.1.5/relax/data/loader.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/data/module.py` & `jax-relax-0.1.5/relax/data/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -453,68 +453,82 @@
     X, y = datamodule.train_dataset[:]
     size = int(len(X) * frac)
     return X[:size], y[:size]
 
 # %% ../../nbs/01_data.module.ipynb 47
 DEFAULT_DATA_CONFIGS = {
     'adult': {
-        'data' :'assets/data/s_adult.csv',
-        'conf' :'assets/configs/data_configs/adult.json',
+        'data' :'assets/adult/data.csv',
+        'conf' :'assets/adult/configs.json',
+        'model' :'assets/adult/model'
     },
     'heloc': {
-        'data': 'assets/data/s_home.csv',
-        'conf': 'assets/configs/data_configs/home.json'
+        'data': 'assets/heloc/data.csv',
+        'conf': 'assets/heloc/configs.json',
+        'model' :'assets/heloc/model'
     },
     'oulad': {
-        'data': 'assets/data/s_student.csv',
-        'conf': 'assets/configs/data_configs/student.json'
+        'data': 'assets/oulad/data.csv',
+        'conf': 'assets/oulad/configs.json',
+        'model' :'assets/oulad/model'
     },
     'credit': {
-        'data': 'assets/data/extra/s_credit_card.csv',
-        'conf': 'assets/configs/data_configs/credit_card.json'
+        'data': 'assets/credit/data.csv',
+        'conf': 'assets/credit/configs.json',
+        'model' :'assets/credit/model'
     },
     'cancer': {
-        'data': 'assets/data/extra/s_breast_cancer.csv',
-        'conf': 'assets/configs/data_configs/breast_cancer.json'
+        'data': 'assets/cancer/data.csv',
+        'conf': 'assets/cancer/configs.json',
+        'model' :'assets/cancer/model'
     },
     'student_performance': {
-        'data': 'assets/data/extra/s_student_performance.csv',
-        'conf': 'assets/configs/data_configs/student_performance.json'
+        'data': 'assets/student_performance/data.csv',
+        'conf': 'assets/student_performance/configs.json',
+        'model' :'assets/student_performance/model'
     },
     'titanic': {
-        'data': 'assets/data/extra/s_titanic.csv',
-        'conf': 'assets/configs/data_configs/titanic.json'
+        'data': 'assets/titanic/data.csv',
+        'conf': 'assets/titanic/configs.json',
+        'model' :'assets/titanic/model'
     },
     'german': {
-        'data': 'assets/data/extra/s_german_credit.csv',
-        'conf': 'assets/configs/data_configs/german_credit.json'
+        'data': 'assets/german/data.csv',
+        'conf': 'assets/german/configs.json',
+        'model' :'assets/german/model'
     },
     'spam': {
-        'data': 'assets/data/s_spam.csv',
-        'conf': 'assets/configs/data_configs/spam.json'
+        'data': 'assets/spam/data.csv',
+        'conf': 'assets/spam/configs.json',
+        'model' :'assets/spam/model'
     },
     'ozone': {
-        'data': 'assets/data/s_ozone.csv',
-        'conf': 'assets/configs/data_configs/ozone.json'
+        'data': 'assets/ozone/data.csv',
+        'conf': 'assets/ozone/configs.json',
+        'model' :'assets/ozone/model'
     },
     'qsar': {
-        'data': 'assets/data/s_qsar.csv',
-        'conf': 'assets/configs/data_configs/qsar.json'
+        'data': 'assets/qsar/data.csv',
+        'conf': 'assets/qsar/configs.json',
+        'model' :'assets/qsar/model'
     },
     'bioresponse': {
-        'data': 'assets/data/s_bioresponse.csv',
-        'conf': 'assets/configs/data_configs/bioresponse.json'
+        'data': 'assets/bioresponse/data.csv',
+        'conf': 'assets/bioresponse/configs.json',
+        'model' :'assets/bioresponse/model'
     },
     'churn': {
-        'data': 'assets/data/s_churn.csv',
-        'conf': 'assets/configs/data_configs/churn.json'
+        'data': 'assets/churn/data.csv',
+        'conf': 'assets/churn/configs.json',
+        'model' :'assets/churn/model'
     },
     'road': {
-        'data': 'assets/data/s_road.csv',
-        'conf': 'assets/configs/data_configs/road.json'
+        'data': 'assets/road/data.csv',
+        'conf': 'assets/road/configs.json',
+        'model' :'assets/road/model'
     }
 }
 
 # %% ../../nbs/01_data.module.ipynb 48
 def _validate_dataname(data_name: str):
     if data_name not in DEFAULT_DATA_CONFIGS.keys():
         raise ValueError(f'`data_name` must be one of {DEFAULT_DATA_CONFIGS.keys()}, '
@@ -534,20 +548,19 @@
     _data_path = DEFAULT_DATA_CONFIGS[data_name]['data']
     _conf_path = DEFAULT_DATA_CONFIGS[data_name]['conf']
     
     data_url = f"https://github.com/BirkhoffG/ReLax/raw/master/{_data_path}"
     conf_url = f"https://github.com/BirkhoffG/ReLax/raw/master/{_conf_path}"
 
     # create new dir
-    data_dir = Path(os.getcwd()) / "cf_data"
+    data_dir = Path(os.getcwd()) / "cf_data" / data_name
     if not data_dir.exists():
         os.makedirs(data_dir)
-    data_path = data_dir / f'{data_name}.csv'
-    conf_path = data_dir / f'{data_name}.json'
-
+    data_path = data_dir / 'data.csv'
+    conf_path = data_dir / 'configs.json'
 
     # download data/configs
     if not data_path.is_file():
         urlretrieve(data_url, data_path)    
     if not conf_path.is_file():
         urlretrieve(conf_url, conf_path)
```

### Comparing `jax-relax-0.1.4/relax/data/scm.py` & `jax-relax-0.1.5/relax/data/scm.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/docs.py` & `jax-relax-0.1.5/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/evaluate.py` & `jax-relax-0.1.5/relax/evaluate.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/import_essentials.py` & `jax-relax-0.1.5/relax/import_essentials.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/logger.py` & `jax-relax-0.1.5/relax/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/methods/base.py` & `jax-relax-0.1.5/relax/methods/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/methods/cchvae.py` & `jax-relax-0.1.5/relax/methods/cchvae.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     
     @partial(jax.jit, static_argnums=(0,))
     def loss(self, params, rng_key, x):
         mu_x, logvar_x, mu_z, logvar_z, z_rep = self.forward(params, rng_key, x)
         recon_loss = jnp.mean(optax.l2_loss(mu_x, x))
         # kl_loss = -0.5 * jnp.sum(1 + logvar_z - mu_z**2 - jnp.exp(logvar_z))
         kl_loss = -0.5 * jnp.sum(1 + logvar_z - jnp.power(mu_z, 2) - jnp.exp(logvar_z))
-        loss = recon_loss + kl_loss
+        loss = recon_loss + 0.3 * kl_loss
         return loss
 
     @partial(jax.jit, static_argnums=(0,))
     def _training_step(
         self, 
         params: Tuple[hk.Params, hk.Params],
         opt_state: optax.OptState, 
@@ -174,21 +174,20 @@
     max_steps: int,
     n_search_samples: int,
     step_size: float,
     cchvae_module: CHVAE,
     cchvae_params: Tuple[hk.Params, hk.Params],
     apply_fn: Callable,
 ):
-    @jit
     def cond_fn(state):
         count, cf, _ = state
         return jnp.logical_and(count < max_steps, jnp.array_equal(x, cf))
     
-    @jit
-    def body_fn(state):
+    @loop_tqdm(max_steps)
+    def body_fn(i, state):
         count, candidate_cf, rng = state
         rng_key, subkey_1, subkey_2 = jrand.split(rng, num=3)
         low, high = step_size * count, step_size * (count + 1)
         # STEP 1 -- SAMPLE POINTS on hyper sphere around instance
         latent_neighbors = _hyper_sphere_coordindates(
             subkey_1, z_rep, n_search_samples, high=high, low=low, p_norm=1
         )
@@ -198,32 +197,37 @@
         # STEP 2 -- COMPUTE l1 norms
         distances = jnp.abs(x_ce - x).sum(axis=1)
 
         # STEP 3 -- SELECT POINT with MINIMUM l1 norm
         y_candidates = pred_fn(x_ce).round().reshape(-1)
         indices = jnp.where(y_candidates != y_pred, 1, 0).astype(bool)
         distances = jnp.where(indices, distances, jnp.inf)
+
+        best_candidate_cf = x_ce[jnp.argmin(distances)].reshape(1, -1)
         
         candidate_cf = lax.cond(
-            jnp.any(indices),
-            lambda _: x_ce[jnp.argmin(distances)].reshape(1, -1),
+            distances.min() < jnp.abs(x - candidate_cf).sum(axis=1).min(),
+            lambda _: best_candidate_cf,
             lambda _: candidate_cf,
             None
         )
 
         count += 1
         return count, candidate_cf, rng_key
     
     y_pred = pred_fn(x).round().reshape(-1)
     z, _ = cchvae_module.encode(cchvae_params[0], rng_key, x)
     # z_rep = jnp.repeat(z.reshape(1, -1), n_search_samples, axis=0)
     z_rep = z.reshape(1, -1)
     rng_key, _ = jrand.split(rng_key)
-    state = (0, x, rng_key) # (count, candidate_cf, rng_key)
-    count, candidate_cf, rng_key = jax.lax.while_loop(cond_fn, body_fn, state)
+    # candidate_cf = jnp.array(x, copy=True)
+    candidate_cf = jnp.ones_like(x) * jnp.inf
+    state = (0, candidate_cf, rng_key) # (count, candidate_cf, rng_key)
+    # count, candidate_cf, rng_key = jax.lax.while_loop(cond_fn, body_fn, state)
+    count, candidate_cf, rng_key = lax.fori_loop(0, max_steps, body_fn, state)
     # while cond_fn(state):
     #     count, candidate_cf, rng_key = body_fn(state)
     # print(count)
     return candidate_cf
 
 # %% ../../nbs/methods/06_cchvae.ipynb 9
 class CCHVAEConfigs(BaseParser):
@@ -231,17 +235,17 @@
         [20, 16, 14, 12], description="Encoder hidden sizes"
     ) 
     dec_sizes: List[int] = Field(
         [12, 14, 16, 20], description="Decoder hidden sizes"
     )
     encoded_size: int = Field(5, description="Encoded size")
     lr: float = Field(0.001, description="Learning rate")
-    max_steps: int = Field(1000, description="Max steps")
+    max_steps: int = Field(100, description="Max steps")
     n_search_samples: int = Field(300, description="Number of generated candidate counterfactuals.")
-    step_size: float = Field(0.1, description="Step size")
+    step_size: float = Field(1, description="Step size")
     seed: int = Field(0, description="Seed for random number generator")
 
 # %% ../../nbs/methods/06_cchvae.ipynb 10
 class CCHVAE(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: CHVAE
     name: str = 'C-CHVAE'
```

### Comparing `jax-relax-0.1.4/relax/methods/clue.py` & `jax-relax-0.1.5/relax/methods/clue.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,31 +164,40 @@
         rng_key, key = jax.random.split(rng_key)
         prior = jrand.normal(key, (self.m_config.enc_sizes[-1],))
         return prior
     
     def compute_loss(self, params, rng_key, x, is_training=True):
         # @partial(jax.jit, static_argnums=(2, 3))
         def reconstruct_loss(x: Array, cf: Array, cat_idx: int, cat_arr: List[int]):
-            cont_loss = optax.l2_loss(x[:, :cat_idx], cf[:, :cat_idx])
-            cat_loss = []
-
-            def _cat_loss_f(start_end_idx):
-                start_idx, end_idx = start_end_idx
-                return optax.softmax_cross_entropy(
-                    cf[:, start_idx: end_idx], x[:, start_idx: end_idx]
-                ).reshape(-1, 1)
             
-            # for start_end_idx in start_end_indices:
-            for i, cat in enumerate(cat_arr):
-                start_end_idx = (cat_idx + i * cat, cat_idx + (i + 1) * cat)
-                cat_loss.append(_cat_loss_f(start_end_idx))
-            cat_loss = jnp.concatenate(cat_loss, axis=-1)
+            def compute_cat_loss(cat_arr):
+                if len(cat_arr) == 0: return jnp.zeros((x.shape[0], 0))
+                
+                cat_loss = []
+
+                def _cat_loss_f(start_end_idx):
+                    start_idx, end_idx = start_end_idx
+                    return optax.softmax_cross_entropy(
+                        cf[:, start_idx: end_idx], x[:, start_idx: end_idx]
+                    ).reshape(-1, 1)
+                
+                # for start_end_idx in start_end_indices:
+                start_idx = cat_idx
+                for i, cat in enumerate(cat_arr):
+                    end_idx = start_idx + cat
+                    start_end_idx = (start_idx, end_idx)
+                    cat_loss.append(_cat_loss_f(start_end_idx))
+                    start_idx = end_idx
+                cat_loss = jnp.concatenate(cat_loss, axis=-1)
+                return cat_loss
             
             # cat_loss = jax.vmap(jit(_cat_loss_f))(start_indices, end_indices)
             # cat_loss = jax.lax.scan(_cat_loss_f, 0., start_end_indices, len(start_end_indices))[1]
+            cont_loss = optax.l2_loss(x[:, :cat_idx], cf[:, :cat_idx])
+            cat_loss = compute_cat_loss(cat_arr)
             return jnp.concatenate([cont_loss, cat_loss], axis=-1).sum(-1)
         
         keys = jax.random.split(rng_key, 2)
         mu_z, logvar_z, reconstruct_x = self.sample(
             params, keys[0], x, mc_samples=1, is_training=is_training
         )
         kl_loss = -0.5 * (1 + logvar_z - jnp.power(mu_z, 2) - jnp.exp(logvar_z)).sum(-1)
@@ -292,14 +301,15 @@
             (uncertainty_weight + aleatoric_weight) * uncertainty 
             + prior_weight * loglik
             + distance_weight * dist
             + validity_weight * validity
         )
         return loss.mean()
     
+    @loop_tqdm(max_steps)
     def step(i, z_opt_state):
         z, opt_state = z_opt_state
         z_grad = jax.grad(compute_loss)(z, dec_params)
         z, opt_state = grad_update(z_grad, z, opt_state, opt)
         return z, opt_state
     
     enc_params, dec_params = vae_params
```

### Comparing `jax-relax-0.1.4/relax/methods/counternet.py` & `jax-relax-0.1.5/relax/methods/counternet.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/methods/diverse.py` & `jax-relax-0.1.5/relax/methods/diverse.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/methods/proto.py` & `jax-relax-0.1.5/relax/methods/proto.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/methods/vaecf.py` & `jax-relax-0.1.5/relax/methods/vaecf.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 class VAECFConfigs(VAECFModuleConfigs):
     pass
 
 # %% ../../nbs/methods/07_vaecf.ipynb 14
 class VAECF(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: VAECFModule
-    name: str = 'C-CHVAE'
+    name: str = 'VAECF'
 
     def __init__(self, m_config: Dict | VAECFConfigs = None):
         if m_config is None:
             m_config = VAECFConfigs()
         self.m_config = m_config
         self.module = VAECFModule(m_config.dict())
```

### Comparing `jax-relax-0.1.4/relax/methods/vanilla.py` & `jax-relax-0.1.5/relax/methods/vanilla.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/module.py` & `jax-relax-0.1.5/relax/module.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_training_module.ipynb.
 
 # %% ../nbs/03_training_module.ipynb 3
 from __future__ import annotations
 from .import_essentials import *
 from .data import TabularDataModule
+from .data.module import DEFAULT_DATA_CONFIGS
 from .logger import TensorboardLogger
-from .utils import validate_configs, sigmoid, accuracy, init_net_opt, grad_update, make_hk_module, show_doc as show_parser_doc
+from .utils import validate_configs, sigmoid, accuracy, init_net_opt, grad_update, make_hk_module, show_doc as show_parser_doc, load_json
+from ._ckpt_manager import load_checkpoint
 from fastcore.basics import patch
 from functools import partial
 from abc import ABC, abstractmethod
 from copy import deepcopy
+from urllib.request import urlretrieve
 
 # %% auto 0
-__all__ = ['BaseNetwork', 'DenseBlock', 'MLP', 'PredictiveModel', 'BaseTrainingModule', 'PredictiveTrainingModuleConfigs',
-           'PredictiveTrainingModule']
+__all__ = ['BaseNetwork', 'DenseBlock', 'MLP', 'PredictiveModel', 'BaseTrainingModule', 'PredictiveTrainingModuleConfigs', 'PredictiveTrainingModule', 'load_pred_model', 'download_model']
 
 # %% ../nbs/03_training_module.ipynb 5
 class BaseNetwork(ABC):
     """BaseNetwork needs a `is_training` argument"""
 
     def __call__(self, *, is_training: bool):
         pass
@@ -205,12 +207,70 @@
     def training_step(self, params, opt_state, rng_key, batch):
         params, opt_state, loss = self._training_step(params, opt_state, rng_key, batch)
         self.log_dict({"train/train_loss_1": loss.item()})
         return params, opt_state
 
     def validation_step(self, params, rng_key, batch):
         x, y = batch
-        y_pred = self.net.apply(params, rng_key, x, is_training=False)
+        y_pred = self.forward(params, rng_key, x, is_training=False)
         loss = self.loss_fn(params, rng_key, batch, is_training=False)
         logs = {"val/val_loss": loss.item(), "val/val_accuracy": accuracy(y, y_pred)}
         self.log_dict(logs)
 
+
+# %% ../nbs/04_learning.ipynb 7
+def load_pred_model(
+    data_name: str # The name of data
+    ) -> Tuple[hk.Params, PredictiveTrainingModule]:
+    """High-level util function for loading trained model."""
+
+    # validate data name
+    if data_name not in DEFAULT_DATA_CONFIGS.keys():
+        raise ValueError(f'`data_name` must be one of {DEFAULT_DATA_CONFIGS.keys()}, '
+            f'but got data_name={data_name}.')
+
+    # Download model
+    download_model(data_name)
+
+    # Fetch the sizes and lr from the configs file
+    data_dir = Path(os.getcwd()) / "cf_data" / data_name 
+    mlp_configs = load_json(data_dir / "configs.json" )['mlp_configs']
+    sizes = mlp_configs["sizes"]
+    lr = mlp_configs["lr"]
+
+    module = PredictiveTrainingModule({'sizes': sizes, 'lr': lr})
+    param = load_checkpoint(data_dir / "model")
+    return (param, module)
+
+
+def download_model(
+    data_name: str # The name of data
+    ):
+    """High-level util function for download trained model."""
+
+    # validate data name
+    if data_name not in DEFAULT_DATA_CONFIGS.keys():
+        raise ValueError(f'`data_name` must be one of {DEFAULT_DATA_CONFIGS.keys()}, '
+            f'but got data_name={data_name}.')
+
+    # get model urls
+    _model_path = f"assets/{data_name}/model"
+
+    # create new dir
+    data_dir = Path(os.getcwd()) / "cf_data"
+    if not data_dir.exists():
+        os.makedirs(data_dir)
+    model_path = data_dir / data_name / "model"
+    if not model_path.exists():
+        os.makedirs(model_path)
+    model_params_url = f"https://github.com/BirkhoffG/ReLax/raw/master/{_model_path}/params.npy"
+    model_tree_url = f"https://github.com/BirkhoffG/ReLax/raw/master/{_model_path}/tree.pkl"
+
+    # download trained model
+    params_path = os.path.join(model_path, "params.npy")
+    tree_path = os.path.join(model_path, "tree.pkl")
+    if not os.path.isfile(params_path):
+        urlretrieve(model_params_url, params_path)
+    if not os.path.isfile(tree_path):
+        urlretrieve(model_tree_url, tree_path)
+
+    return
```

### Comparing `jax-relax-0.1.4/relax/plots.py` & `jax-relax-0.1.5/relax/plots.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/relax/trainer.py` & `jax-relax-0.1.5/relax/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_learning.ipynb.
 
 # %% ../nbs/04_learning.ipynb 3
 from __future__ import annotations
 from .import_essentials import *
-from .data import TabularDataModule
-from .module import BaseTrainingModule
+from .data import TabularDataModule, load_data
+from .data.module import DEFAULT_DATA_CONFIGS
+from .module import BaseTrainingModule, PredictiveTrainingModule
 from .logger import TensorboardLogger
-from .utils import validate_configs
-from ._ckpt_manager import CheckpointManager
+from .utils import validate_configs, load_json
+from ._ckpt_manager import CheckpointManager, load_checkpoint
+from urllib.request import urlretrieve
 
 # %% auto 0
 __all__ = ['TrainingConfigs', 'train_model_with_states', 'train_model']
 
 # %% ../nbs/04_learning.ipynb 4
 class TrainingConfigs(BaseParser):
     """Configurator of `train_model`."""
```

### Comparing `jax-relax-0.1.4/relax/utils.py` & `jax-relax-0.1.5/relax/utils.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.4/settings.ini` & `jax-relax-0.1.5/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[DEFAULT]
-host = github
-lib_name = jax-relax
-user = birkhoffg
-description = Jax-based Recourse Explanation Library
-keywords = Jax, Recourse, Explanation, Interpretability, Machine Learning
-author = BirkhoffG
-author_email = 26811230+BirkhoffG@users.noreply.github.com
-copyright = Birkhoff Guo
-branch = master
-version = 0.1.4
-min_python = 3.8
-audience = Developers
-language = English
-custom_sidebar = true
-license = apache2
-status = 2
-requirements = matplotlib seaborn scikit-learn>=1.0.2,<1.4.0 pandas nbdev jupyter dm-haiku test_tube jax[cpu] tqdm optax pydantic>=1.9.0,<2 deprecation networkx jax-tqdm
-dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit
-nbs_path = nbs
-doc_path = _docs
-recursive = True
-doc_host = https://birkhoffg.github.io
-doc_baseurl = /ReLax/
-git_url = https://github.com/birkhoffg/relax/tree/master/
-lib_path = relax
-title = ReLax
-tst_flags = slow
-black_formatting = False
-readme_nb = index.ipynb
-allowed_metadata_keys = 
-allowed_cell_metadata_keys = 
-jupyter_hooks = True
-clean_ids = True
-clear_all = False
-put_version_in_init = True
-renderer = relax.docs.CustomizedMarkdownRenderer
-
+[DEFAULT]
+host = github
+lib_name = jax-relax
+user = birkhoffg
+description = Jax-based Recourse Explanation Library
+keywords = Jax, Recourse, Explanation, Interpretability, Machine Learning
+author = BirkhoffG
+author_email = 26811230+BirkhoffG@users.noreply.github.com
+copyright = Birkhoff Guo
+branch = master
+version = 0.1.5
+min_python = 3.8
+audience = Developers
+language = English
+custom_sidebar = true
+license = apache2
+status = 2
+requirements = matplotlib seaborn scikit-learn>=1.0.2,<1.4.0 pandas nbdev jupyter dm-haiku test_tube jax[cpu] tqdm optax pydantic>=1.9.0,<2 deprecation networkx jax-tqdm
+dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit datasets
+nbs_path = nbs
+doc_path = _docs
+recursive = True
+doc_host = https://birkhoffg.github.io
+doc_baseurl = /ReLax/
+git_url = https://github.com/birkhoffg/relax/tree/master/
+lib_path = relax
+title = ReLax
+tst_flags = slow
+black_formatting = False
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+put_version_in_init = True
+renderer = relax.docs.CustomizedMarkdownRenderer
+
```

### Comparing `jax-relax-0.1.4/setup.py` & `jax-relax-0.1.5/setup.py`

 * *Files identical despite different names*

