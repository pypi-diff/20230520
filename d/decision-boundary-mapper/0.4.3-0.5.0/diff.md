# Comparing `tmp/decision-boundary-mapper-0.4.3.tar.gz` & `tmp/decision-boundary-mapper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision-boundary-mapper-0.4.3.tar", last modified: Fri Mar 31 10:35:14 2023, max compression
+gzip compressed data, was "decision-boundary-mapper-0.5.0.tar", last modified: Sat May 20 06:03:27 2023, max compression
```

## Comparing `decision-boundary-mapper-0.4.3.tar` & `decision-boundary-mapper-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.412844 decision-boundary-mapper-0.4.3/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1071 2023-01-21 18:28:21.000000 decision-boundary-mapper-0.4.3/LICENSE.txt
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     4052 2023-03-31 10:35:14.412844 decision-boundary-mapper-0.4.3/PKG-INFO
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     3132 2023-02-18 17:47:25.000000 decision-boundary-mapper-0.4.3/README.md
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      107 2023-03-31 10:35:14.412844 decision-boundary-mapper-0.4.3/setup.cfg
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1775 2023-03-31 10:34:51.000000 decision-boundary-mapper-0.4.3/setup.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.384843 decision-boundary-mapper-0.4.3/src/
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.396844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.396844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.400843 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)    13866 2023-03-31 10:32:19.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/DBM.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      603 2023-01-21 18:28:21.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     5076 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/invNN.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1765 2023-02-18 17:47:25.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/projections.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)    39024 2023-03-31 10:22:26.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBMInterface.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     5965 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/NNinterface.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.400843 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     7903 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     9699 2023-03-31 10:32:34.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      604 2023-01-21 18:28:21.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      723 2023-02-19 10:35:45.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     6861 2023-03-25 08:39:51.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/tools.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.404844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)    51081 2023-03-31 10:08:24.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)    26589 2023-03-25 08:39:51.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/GUI.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      643 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/__init__.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.408844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     2729 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/Logger.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     3160 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerGUI.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1031 2023-02-18 13:26:48.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerInterface.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1806 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerModel.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      723 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      791 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/__init__.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.412844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     6407 2023-03-25 13:08:02.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/DBM_usage_example.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     5055 2023-03-25 13:03:46.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/SDBM_usage_example.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      728 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     3202 2023-03-25 12:17:12.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/utils.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.412844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/utils/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      738 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/utils/__init__.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     3938 2023-03-04 16:24:03.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/utils/dataReader.py
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1291 2023-02-18 17:47:25.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/utils/tools.py
-drwxrwxr-x   0 cristi    (1000) cristi    (1000)        0 2023-03-31 10:35:14.396844 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     4052 2023-03-31 10:35:14.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 cristi    (1000) cristi    (1000)     1604 2023-03-31 10:35:14.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 cristi    (1000) cristi    (1000)        1 2023-03-31 10:35:14.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 cristi    (1000) cristi    (1000)      144 2023-03-31 10:35:14.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/requires.txt
--rw-rw-r--   0 cristi    (1000) cristi    (1000)       25 2023-03-31 10:35:14.000000 decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.718901 decision-boundary-mapper-0.5.0/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1071 2023-03-30 08:17:56.000000 decision-boundary-mapper-0.5.0/LICENSE.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-05-20 06:03:27.719112 decision-boundary-mapper-0.5.0/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2818 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/README.md
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      107 2023-05-20 06:03:27.719660 decision-boundary-mapper-0.5.0/setup.cfg
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1737 2023-05-20 06:03:22.000000 decision-boundary-mapper-0.5.0/setup.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.703022 decision-boundary-mapper-0.5.0/src/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.705730 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.708838 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    43104 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5735 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractNN.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.710153 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    12647 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/DBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5108 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/NNInv.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      600 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1519 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/projections.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.711575 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7062 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     9850 2023-05-19 14:34:10.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7841 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SSNP.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      618 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    13834 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.714072 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    28700 2023-05-19 13:46:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    24678 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    20600 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    13781 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUIController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      641 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1906 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.715712 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2872 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/Logger.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3096 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1006 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerInterface.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1794 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerModel.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      721 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      826 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/__init__.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.717074 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     6454 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/DBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     4718 2023-05-19 14:34:53.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/SDBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      726 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3279 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.718595 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1351 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/config.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     4123 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/dataReader.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1296 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.707428 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1842 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)        1 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      144 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/requires.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)       25 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/top_level.txt
```

### Comparing `decision-boundary-mapper-0.4.3/LICENSE.txt` & `decision-boundary-mapper-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.4.3/PKG-INFO` & `decision-boundary-mapper-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.4.3
+Version: 0.5.0
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
         
         This is the package provides functionality for visualizing the classifiers decision boundaries.
         
         It is based on the work of Cristian Grosu for the master thesis project for 2023 at Utrecht University.
         If you use this package, please cite the following paper:
-        [placeholder for the paper]
+        `[PLACEHOLDER FOR THE PAPER](http://google.com/)`
         
         The package is available on PyPI and can be installed using pip: `pip install decision-boundary-mapper`
         
         ## Documentation
         
         See more details at `https://decisionboundarymapper.000webhostapp.com/`
         
@@ -28,26 +28,25 @@
         from decision_boundary_mapper import GUI
         
         GUI().start()
         ```
         
         2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
         Both examples use `MNIST` (handwritten digits) dataset.
-        The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `DBM_usage_example_2` uses `UMAP` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. After which a simple classifier is used to color each point of the `2D` projection.
-        The second example `SDM_usage_example` uses an Autoencoder Neural Network to project the data from the `nD` space to the `2D` space, then a simple classifier is used to color each point of the `2D` projection.
+        The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
         The examples can be found in the `examples` folder.
         
         ```python
         from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
         
         DBM_usage_example() # run the first example
         SDM_usage_example() # run the second example
         ```
         
-        3. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
+        1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
         The classes can be used as follows:
         
         ```python
         from decision_boundary_mapper import DBM, SDBM
         from matplotlib import pyplot as plt
         
         # load the data
@@ -56,18 +55,18 @@
         ...
         # create a simple neural network
         ...
         classifier = ... # for compatibility with the package the classifier should be constructed using tensorflow.keras
         ...
         
         dbm = DBM(classifier) # create a DBM object
-        img, img_confidence, _, _, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+        img, img_confidence, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
         
         sdbm = SDBM(classifier) # create a SDBM object
-        img, img_confidence, _, _, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+        img, img_confidence, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
         ...
         # visualize the decision boundaries
         plt.imshow(img)
         plt.show()
         
         ```
```

### Comparing `decision-boundary-mapper-0.4.3/README.md` & `decision-boundary-mapper-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Short Description
 
 This is the package provides functionality for visualizing the classifiers decision boundaries.
 
 It is based on the work of Cristian Grosu for the master thesis project for 2023 at Utrecht University.
 If you use this package, please cite the following paper:
-[placeholder for the paper]
+`[PLACEHOLDER FOR THE PAPER](http://google.com/)`
 
 The package is available on PyPI and can be installed using pip: `pip install decision-boundary-mapper`
 
 ## Documentation
 
 See more details at `https://decisionboundarymapper.000webhostapp.com/`
 
@@ -20,26 +20,25 @@
 from decision_boundary_mapper import GUI
 
 GUI().start()
 ```
 
 2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
 Both examples use `MNIST` (handwritten digits) dataset.
-The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `DBM_usage_example_2` uses `UMAP` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. After which a simple classifier is used to color each point of the `2D` projection.
-The second example `SDM_usage_example` uses an Autoencoder Neural Network to project the data from the `nD` space to the `2D` space, then a simple classifier is used to color each point of the `2D` projection.
+The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
 The examples can be found in the `examples` folder.
 
 ```python
 from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
 
 DBM_usage_example() # run the first example
 SDM_usage_example() # run the second example
 ```
 
-3. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
+1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
 The classes can be used as follows:
 
 ```python
 from decision_boundary_mapper import DBM, SDBM
 from matplotlib import pyplot as plt
 
 # load the data
@@ -48,18 +47,18 @@
 ...
 # create a simple neural network
 ...
 classifier = ... # for compatibility with the package the classifier should be constructed using tensorflow.keras
 ...
 
 dbm = DBM(classifier) # create a DBM object
-img, img_confidence, _, _, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+img, img_confidence, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
 
 sdbm = SDBM(classifier) # create a SDBM object
-img, img_confidence, _, _, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+img, img_confidence, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
 ...
 # visualize the decision boundaries
 plt.imshow(img)
 plt.show()
 
 ```
```

### Comparing `decision-boundary-mapper-0.4.3/setup.py` & `decision-boundary-mapper-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
@@ -21,38 +21,38 @@
 # remove the old documentation folder
 rmtree('docs', ignore_errors=True)
 
 os.system("pdoc --html src/decision_boundary_mapper -o docs")
 
 setup(
     name='decision-boundary-mapper',
-    version='0.4.3',
+    version='0.5.0',
     license='MIT',
     author="Cristian Grosu",
     author_email='c.grosu@students.uu.nl',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/cristi2019255/MasterThesis2023',
     keywords='Decision Boundary Mapper',
     description='A tool for visualizing the decision boundary of a machine learning model.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
-          'dask',
-          'keras',
-          'matplotlib',
-          'numba',
-          'numba_progress',
-          'numpy',
-          'opfython',
-          'Pillow',
-          'PySimpleGUI',
-          'pydot',
-          'scikit_learn',
-          'scipy',
-          'tensorflow',
-          'termcolor',
-          'tqdm',
-          'umap',
-          'umap-learn',
-      ],
-)
+        'dask',
+        'keras',
+        'matplotlib',
+        'numba',
+        'numba_progress',
+        'numpy',
+        'opfython',
+        'Pillow',
+        'PySimpleGUI',
+        'pydot',
+        'scikit_learn',
+        'scipy',
+        'tensorflow',
+        'termcolor',
+        'tqdm',
+        'umap',
+        'umap-learn',
+    ],
+)
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/DBM.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/DBM.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,282 +1,265 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 import numpy as np
 
-from .invNN import DEFAULT_MODEL_PATH, invNN
+from .NNInv import DEFAULT_MODEL_PATH, NNInv
 from .projections import PROJECTION_METHODS
 
 
-from ..DBMInterface import DBMInterface, DBM_DEFAULT_RESOLUTION, FAST_DBM_STRATEGIES
+from ..AbstractDBM import AbstractDBM, DBM_DEFAULT_RESOLUTION, FAST_DBM_STRATEGIES
 
-from ...utils import track_time_wrapper
+from ...utils import track_time_wrapper, TRAIN_DATA_POINT_MARKER, TEST_DATA_POINT_MARKER, TRAIN_2D_FILE_NAME, TEST_2D_FILE_NAME
 from ...Logger import LoggerInterface, Logger
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
+CUSTOM_PROJECTION_NAME = "Custom"
 
-class DBM(DBMInterface):
+class DBM(AbstractDBM):
     """
-    The Decision Boundary Map (DBM) class has methods for visualizing the decision boundaries of a classifier.
+    This is a class that generated the DBM
+    The core purpose of this class is to learn the inverse projection given a direct projection and construct the decision boundary map of a given classifier
+    
+    Public methods:
+        fit: Learns an inverse projection by training a neural network. \n
+        get_decision_boundary_map: Returns the decision boundary map for the given classifier. \n
 
-    Methods:
-        fit: Trains the classifier on the given data set.
-        get_decision_boundary_map: Returns the decision boundary map for the given classifier.
-        
     Example:
         >>> from DBM import DBM
+        >>> import matplotlib.pyplot as plt
         >>> classifier = ...
         >>> dbm = DBM(classifier)
-        >>> img, img_confidence, img_projection_errors, img_inverse_projection_errors, X2d_train, X2d_test = dbm.get_decision_boundary_map(X2d_train, Xnd_train, Y_train, X2d_test, Xnd_test, Y_test)
+        >>> img, img_confidence, encoded_2d_train, encoded_2d_test = dbm.get_decision_boundary_map(Xnd_train, Xnd_test, X2d_train, X2d_test)
         >>> plt.imshow(img)
         >>> plt.show()
     """
-    
-    def __init__(self, classifier, logger:LoggerInterface=None):
-        """ Initializes the DBM class.
+
+    def __init__(self, classifier, logger: LoggerInterface | None = None):
+        """ 
+        Initializes the DBM class.
 
         Args:
             classifier (tensorflow.keras.Model): The classifier to be used for the decision boundary map.
             logger (LoggerInterface, optional): The logger for outputting info messages. Defaults to console logging.
         """
         super().__init__(classifier, logger)
-        self.neural_network = None       
-    
-    @track_time_wrapper(logger=time_tracker_console)                                             
-    def fit(self, 
-            X2d: np.ndarray, Xnd: np.ndarray,            
-            epochs:int=300, batch_size:int=32, 
-            load_folder:str=DEFAULT_MODEL_PATH):
+        self.neural_network = None  # type: ignore
+
+    @track_time_wrapper(logger=time_tracker_console)
+    def fit(self,
+            X2d: np.ndarray, Xnd: np.ndarray,
+            epochs: int = 300, batch_size: int = 32,
+            load_folder: str = DEFAULT_MODEL_PATH):
         """ 
-        Trains the classifier on the given data set.
+        Learns the inverse projection on the given data set.
 
         Args:
             X2d (np.ndarray): Training data set 2D data got from the projection of the original data (e.g. PCA, t-SNE, UMAP)
             Xnd (np.ndarray): Training data set nD data (e.g. MNIST, CIFAR10) (i.e. the original data)
             epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 300.
             batch_size (int, optional): Train batch size. Defaults to 32.
-        
+
         Returns:
-            inverse_porjection_NN (invNN): The trained inverse projection neural network.
+            inverse_porjection_NN (NNInv): The trained inverse projection neural network.
         """
-        
-        inverse_projection_NN = invNN(classifier=self.classifier, folder_path=load_folder)
+
+        inverse_projection_NN = NNInv(folder_path=load_folder)
         inverse_projection_NN.fit(X2d, Xnd,
-                                  epochs=epochs, 
+                                  epochs=epochs,
                                   batch_size=batch_size)
         return inverse_projection_NN
-    
-    def generate_boundary_map(self, 
-                              Xnd_train: np.ndarray, Y_train: np.ndarray, 
-                              Xnd_test: np.ndarray, Y_test: np.ndarray,
-                              X2d_train: np.ndarray = None,
-                              X2d_test: np.ndarray = None,
-                              train_epochs:int=300, 
-                              train_batch_size:int=32,
-                              resolution:int=DBM_DEFAULT_RESOLUTION,
-                              use_fast_decoding:bool=False,
-                              fast_decoding_strategy:str=FAST_DBM_STRATEGIES[0],
-                              load_folder:str=DEFAULT_MODEL_PATH,
-                              projection:str='t-SNE'                              
-                              ):
-        """ Generates a 2D boundary map of the classifier's decision boundary.
+
+    def generate_boundary_map(self,
+                              Xnd_train: np.ndarray,
+                              Xnd_test: np.ndarray,
+                              X2d_train: np.ndarray | None = None,
+                              X2d_test: np.ndarray | None = None,
+                              nn_train_epochs: int = 300,
+                              nn_train_batch_size: int = 32,
+                              resolution: int = DBM_DEFAULT_RESOLUTION,
+                              fast_decoding_strategy: FAST_DBM_STRATEGIES = FAST_DBM_STRATEGIES.NONE,
+                              load_folder: str = DEFAULT_MODEL_PATH,
+                              projection: str = 't-SNE'):
+        """ 
+        Generates a 2D boundary map of the classifier's decision boundary.
 
         Args:
-            X_train (np.ndarray): Training data set
-            Y_train (np.ndarray): Training data labels
-            X_test (np.ndarray): Testing data set
-            Y_test (np.ndarray): Testing data labels
+            X_train (np.ndarray): Training data set (nD)
+            X_test (np.ndarray): Testing data set (nD)
             X2d_train (np.ndarray | None): The 2D projection of the training data. If None, the data is projected using the given projection method. Defaults to None.
             X2d_test (np.ndarray | None): The 2D projection of the testing data. If None, the data is projected using the given projection method. Defaults to None.            
-            train_epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 300.
-            train_batch_size (int, optional): Train batch size. Defaults to 32.
-            show_predictions (bool, optional): If set to true 10 prediction examples are shown. Defaults to True.
-            resolution (int, optional): _description_. Defaults to DBM_DEFAULT_RESOLUTION.
-            use_fast_decoding (bool, optional): If set to true the fast decoding method is used. Defaults to False.
+            nn_train_epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 300.
+            nn_train_batch_size (int, optional): Train batch size. Defaults to 32.
+            resolution (int, optional): The desired resolution of the DBM. Defaults to DBM_DEFAULT_RESOLUTION.
+            fast_decoding_strategy (FAST_DBM_STRATEGIES, optional): The strategy to use in generating the DBM. Defaults to FAST_DBM_STRATEGIES.NONE.
             load_folder (str, optional): The folder in which the model will be stored or if exists loaded from. Defaults to DEFAULT_MODEL_PATH
             projection (str, optional): The projection method to be used. Defaults to 't-SNE'.
-        
+
         Returns:
             img (np.array): A 2D numpy array with the decision boundary map, each element is an integer representing the class of the corresponding point.
             img_confidence (np.array): A 2D numpy array with the decision boundary map, each element is a float representing the confidence of the classifier for the corresponding point.
-            X2d_train (np.array): A 2D matrix representing the projection of the training data set, each element is an integer representing the class of the corresponding point.
-            X2d_test (np.array): A 2D matrix representing the projection of the testing data set, each element is an integer representing the class of the corresponding point.
-            space_nd (np.array): A 2D matrix representing the nD space in which the decision boundary map is generated.
-            history (dict): A dictionary containing the training history of the neural network.
-        
+            encoded_2d_train (np.array): An array representing the projection of the training data set, each element is a tuple representing the coordinates and the class of the corresponding point.
+            encoded_2d_test (np.array): An array representing the projection of the testing data set, each element is an tuple representing the coordinates and the class of the corresponding point.
+    
         Example:
             >>> dbm = DBM(classifier)
-            >>> img, img_confidence, X2d_train, X2d_test, history = dbm.generate_boundary_map(X_train, Y_train, X_test, Y_test)
+            >>> img, img_confidence, _, _ = dbm.generate_boundary_map(X_train, X_test)
             >>> fig, [ax1, ax2] = plt.subplots(1, 2, figsize=(10, 5))
             >>> ax1.imshow(img)
             >>> ax2.imshow(img_confidence)
             >>> plt.show()
         """
-        assert projection in ['t-SNE', 'PCA', 'UMAP']
-                
-        # creating a folder for the model if not present
-        if not os.path.exists(os.path.join(load_folder)):
-           os.makedirs(os.path.join(load_folder)) 
-        
+       
         if X2d_train is None or X2d_test is None:
+            assert projection in PROJECTION_METHODS.keys()
             Xnd_train_flatten = Xnd_train.reshape((Xnd_train.shape[0], -1))
             Xnd_test_flatten = Xnd_test.reshape((Xnd_test.shape[0], -1))
             X2d_train, X2d_test = self.__transform_2d__(Xnd_train_flatten, Xnd_test_flatten, load_folder, projection)
         else:
             # Normalize the data to be in the range of [0,1]
             X2d_train, X2d_test = self.__normalize_2d__(X2d_train, X2d_test)
-        
+            
+        # adding projection method to the end of the load_folder path
         if projection != load_folder.split(os.sep)[-1]:
             load_folder = os.path.join(load_folder, projection)
-        
+
+        # creating a folder for the model if not present
+        if not os.path.exists(os.path.join(load_folder)):
+            os.makedirs(os.path.join(load_folder))
+
+
         if self.neural_network is None:
-            X = np.concatenate((X2d_train, X2d_test), axis=0)
-            Y = np.concatenate((Xnd_train, Xnd_test), axis=0)
-            self.neural_network = self.fit(X, Y,
-                                          train_epochs, train_batch_size,
-                                          load_folder=load_folder)   
-        
+            X2d = np.concatenate((X2d_train, X2d_test), axis=0)
+            Xnd = np.concatenate((Xnd_train, Xnd_test), axis=0)
+            self.neural_network = self.fit(X2d, Xnd,
+                                           epochs = nn_train_epochs, 
+                                           batch_size = nn_train_batch_size,
+                                           load_folder=load_folder)
+
+        self.resolution = resolution
+
         self.console.log("Decoding the 2D space... 2D -> nD")
-        
-        save_img_path = os.path.join(load_folder, "boundary_map")
-        save_img_confidence_path = os.path.join(load_folder, "boundary_map_confidence")
-        
-        self.resolution = resolution   
-        
-        if use_fast_decoding:
-            save_img_path += "_fast"
-            save_img_confidence_path += "_fast"            
-            if fast_decoding_strategy == FAST_DBM_STRATEGIES[1]:
-                img, img_confidence = self._get_img_dbm_fast_confidences_strategy(resolution)
-            else:
-                img, img_confidence = self._get_img_dbm_fast_(resolution)                        
-        else:
-            img, img_confidence = self._get_img_dbm_(resolution)
-    
-        with open(f"{save_img_path}.npy", 'wb') as f:
-            np.save(f, img)
-        with open(f"{save_img_confidence_path}.npy", 'wb') as f:
-            np.save(f, img_confidence)        
-                 
+
+        img, img_confidence = self.get_dbm(fast_decoding_strategy, resolution, load_folder)
+
         self.X2d = np.concatenate((X2d_train, X2d_test), axis=0)
-        self.Xnd = np.concatenate((Xnd_train.reshape((Xnd_train.shape[0],-1)), Xnd_test.reshape((Xnd_test.shape[0],-1))), axis=0)
+        self.Xnd = np.concatenate((Xnd_train.reshape((Xnd_train.shape[0], -1)), Xnd_test.reshape((Xnd_test.shape[0], -1))), axis=0)
         self.console.log("Map the 2D embedding of the data to the 2D image")
-        
+
         # transform the encoded data to be in the range [0, resolution)
-        X2d_train *= (self.resolution - 1)
-        X2d_test *= (self.resolution - 1)
+        X2d_train *= (resolution - 1)
+        X2d_test *= (resolution - 1)
         X2d_train = X2d_train.astype(int)
         X2d_test = X2d_test.astype(int)
-        
+
         encoded_2d_train = np.zeros((len(X2d_train), 3))
         encoded_2d_test = np.zeros((len(X2d_test), 3))
-        
+
         for k in range(len(X2d_train)):
-            [i,j] = X2d_train[k]
-            encoded_2d_train[k] = [i, j, img[i,j]]
+            [i, j] = X2d_train[k]
+            encoded_2d_train[k] = [i, j, img[i, j]]
         for k in range(len(X2d_test)):
-            [i,j] = X2d_test[k]
-            encoded_2d_test[k] = [i, j, img[i,j]]            
-        
-        for [i,j] in X2d_test:        
-            img[i,j] = -2
-            img_confidence[i,j] = 1
-        for [i,j] in X2d_train:    
-            img[i,j] = -1
-            img_confidence[i,j] = 1
-        
-            
-        history_file_path = os.path.join(load_folder, "history.json")
-        history = {}
-        if os.path.exists(history_file_path):
-            with open(history_file_path, 'r') as f:
-                history = json.load(f)
-        
-        return (img, img_confidence, encoded_2d_train, encoded_2d_test, history)
-     
+            [i, j] = X2d_test[k]
+            encoded_2d_test[k] = [i, j, img[i, j]]
+
+        for [i, j] in X2d_test:
+            img[i, j] = TEST_DATA_POINT_MARKER
+            img_confidence[i, j] = 1
+        for [i, j] in X2d_train:
+            img[i, j] = TRAIN_DATA_POINT_MARKER
+            img_confidence[i, j] = 1
+
+        return (img, img_confidence, encoded_2d_train, encoded_2d_test)
+
     def _predict2dspace_(self, X2d: np.ndarray):
-        """ Predicts the labels for the given 2D data set.
+        """ 
+        Predicts the labels for the given 2D data set.
 
         Args:
             X2d (np.ndarray): The 2D data set
-        
+
         Returns:
             predicted_labels (np.ndarray): The predicted labels for the given 2D data set
             predicted_confidence (np.ndarray): The predicted probabilities for the given 2D data set
-            spaceNd (np.ndarray): The decoded nD space
         """
         spaceNd = self.neural_network.decode(X2d, verbose=0)
-        predictions = self.classifier.predict(spaceNd, verbose=0)
+        predictions = self.classifier.predict(spaceNd, verbose=0)                     # type: ignore
         predicted_labels = np.array([np.argmax(p) for p in predictions])
         predicted_confidence = np.array([np.max(p) for p in predictions])
-        return predicted_labels, predicted_confidence
- 
-    def __transform_2d__(self, X_train: np.ndarray, X_test: np.ndarray, folder:str=DEFAULT_MODEL_PATH, projection:str='t-SNE'):
-        """ Transforms the given data to 2D using a projection method.
+        return predicted_labels, predicted_confidence, predictions
+
+    def __transform_2d__(self, X_train: np.ndarray, X_test: np.ndarray, folder: str = DEFAULT_MODEL_PATH, projection: str = 't-SNE'):
+        """ 
+        Transforms the given data to 2D using a projection method.
 
         Args:
             X_train (np.ndarray): The training data.
             X_test (np.ndarray): The test data.
             folder (str, optional): The folder where the 2D data will be stored. Defaults to DEFAULT_MODEL_PATH.
             projection (str, optional): The projection method to be used. Defaults to 't-SNE'.
-            
+
         Returns:
-            X2d (np.ndarray): The transformed data in 2D.
+            X2d_train (np.ndarray): The transformed train data in 2D.
+            X2d_test (np.ndarray): The transformed test data in 2D.
         """
-        self.console.log(f"Transforming the data to 2D using {projection}")        
+        self.console.log(f"Transforming the data to 2D using {projection}")
         X = np.concatenate((X_train, X_test), axis=0)
         X2d = PROJECTION_METHODS[projection](X)
-            
+
         self.console.log(f"Finished transforming the data to 2D using {projection}")
         X2d_train = X2d[:len(X_train)]
         X2d_test = X2d[len(X_train):]
-        
+
         # rescale to [0,1]
         X2d_train, X2d_test = self.__normalize_2d__(X2d_train, X2d_test)
         # ---------------------
         if not os.path.exists(os.path.join(folder)):
             os.makedirs(os.path.join(folder))
-            
-        file_path = os.path.join(folder, "train_2d.npy")
+
+        file_path = os.path.join(folder, TRAIN_2D_FILE_NAME)
         self.console.log("Saving the 2D data to the disk: " + file_path)
         with open(file_path, 'wb') as f:
             np.save(f, X2d_train)
-        
-        file_path = os.path.join(folder, "test_2d.npy")
+
+        file_path = os.path.join(folder, TEST_2D_FILE_NAME)
         self.console.log("Saving the 2D data to the disk: " + file_path)
         with open(file_path, 'wb') as f:
             np.save(f, X2d_test)
-        
+
         return X2d_train, X2d_test
-    
+
     def __normalize_2d__(self, X2d_train: np.ndarray, X2d_test: np.ndarray):
-        """ Normalizes the given 2D data to [0,1].
+        """ 
+        Normalizes the given 2D data to [0,1].
 
         Args:
             X2d_train (np.ndarray): training data
             X2d_test (np.ndarray): test data
 
         Returns:
             X2d_train (np.ndarray): normalized training data
             X2d_test (np.ndarray): normalized test data
         """
-        x_min = min(np.min(X2d_train[:,0]), np.min(X2d_test[:,0]))
-        y_min = min(np.min(X2d_train[:,1]), np.min(X2d_test[:,1]))
-        x_max = max(np.max(X2d_train[:,0]), np.max(X2d_test[:,0]))
-        y_max = max(np.max(X2d_train[:,1]), np.max(X2d_test[:,1]))
-        X2d_train = (X2d_train - np.array([x_min, y_min])) / np.array([x_max - x_min, y_max - y_min])
-        X2d_test = (X2d_test - np.array([x_min, y_min])) / np.array([x_max - x_min, y_max - y_min])
+        x_min = min(np.min(X2d_train[:, 0]), np.min(X2d_test[:, 0]))
+        y_min = min(np.min(X2d_train[:, 1]), np.min(X2d_test[:, 1]))
+        x_max = max(np.max(X2d_train[:, 0]), np.max(X2d_test[:, 0]))
+        y_max = max(np.max(X2d_train[:, 1]), np.max(X2d_test[:, 1]))
+        mins = np.array([x_min, y_min])
+        ranges = np.array([x_max - x_min, y_max - y_min])
+
+        X2d_train = (X2d_train - mins) / ranges  # type: ignore
+        X2d_test = (X2d_test - mins) / ranges   # type: ignore
         return X2d_train, X2d_test
-
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .DBM import DBM
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBM/invNN.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/NNInv.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,117 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 import numpy as np
 import os
 
-from ..NNinterface import NNinterface
+from ..AbstractNN import AbstractNN
 from ...Logger import LoggerInterface, LoggerModel
 
 DEFAULT_MODEL_PATH = os.path.join("tmp", "DBM")
-INVNN_NAME = "invNN"
+NNINV_NAME = "NNInv"
 DECODER_NAME = "decoder"
+DECODER_LOSS = "mean_squared_error"
 
-class invNN(NNinterface):
+class NNInv(AbstractNN):
     """
         Inverse Projection Neural Network.        
-        The inverse projection 2D -> nD. (Sequential model 2 -> 32 -> 64 -> 128 -> 512 -> nD)            
+        The inverse projection 2D -> nD. 
+        (Sequential model 2 -> 32 -> 64 -> 128 -> 512 -> nD)            
     """
-    
-    def __init__(self, 
-                 classifier = None, 
-                 logger: LoggerInterface = None, 
+
+    def __init__(self,
+                 logger: LoggerInterface | None = None,
                  folder_path: str = DEFAULT_MODEL_PATH):
         """
             Creates an inverse Projection Neural Network model.
         """
-        super().__init__(folder_path = folder_path, nn_name=INVNN_NAME, logger=logger)
-    
-    def __build__(self, output_shape:tuple = (2,2), show_summary:bool = False):
-        """Builds an invNN (Sequential 2D -> 32 -> 64 -> 128 -> 512 -> nD)
+        super().__init__(folder_path=folder_path, nn_name=NNINV_NAME, logger=logger)
+
+    def __build__(self, output_shape: tuple = (2, 2), show_summary: bool = False):
+        """
+        Builds an NNInv model
+        (Sequential 2D -> 32 -> 64 -> 128 -> 512 -> nD)
 
         Args:
             output_shape (tuple, optional): The output shape of the Nd data. Defaults to (2,2).
             show_summary (bool, optional): If True, the model summary will be printed. Defaults to False.
         """
-        
-        #assert len(output_shape) == 2, "Output shape must be a 2D tuple"
-        
-        DECODER_LOSS = "mean_squared_error"
-        
+
         # computing the output size
         output_size = 1
         for i in range(len(output_shape)):
             output_size *= output_shape[i]
-            
+
         self.decoder = tf.keras.Sequential([
-            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform', kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
-            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
+            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform',
+                                  kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
+            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
             tf.keras.layers.Dense(output_size, activation='sigmoid', kernel_initializer='he_uniform'),
             tf.keras.layers.Reshape(output_shape)
         ], name=DECODER_NAME)
-        
+
         input_layer = tf.keras.Input(shape=(2,), name="input")
-                                                                         
-        self.neural_network = tf.keras.models.Model(inputs=input_layer, 
-                                            outputs=[self.decoder(input_layer)], 
-                                            name=INVNN_NAME)
-        
-        self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(), 
-                            loss=DECODER_LOSS,
-                            metrics=["accuracy"])
-        
+
+        self.neural_network = tf.keras.models.Model(inputs=input_layer,
+                                                    outputs=[self.decoder(input_layer)],
+                                                    name=NNINV_NAME)
+
+        self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(),
+                                    loss=DECODER_LOSS,
+                                    metrics=["accuracy"])
+
         if show_summary:
             self.neural_network.summary()
-        
-    def fit(self, 
+
+    def fit(self,
             x2d: np.ndarray, xNd: np.ndarray,
-            epochs:int = 300, batch_size:int = 32):
-        """ Fits the model to the specified data.
+            epochs: int = 300, batch_size: int = 32):
+        """ 
+        Fits the model to the specified data.
 
         Args:
             x2d (np.ndarray): Train input values (2D)
             xNd (np.ndarray): Train input values (nD)
             epochs (int, optional): The number of epochs. Defaults to 300.
             batch_size (int, optional): Data points used for one batch. Defaults to 32.
         """
         if self.neural_network is not None:
             self.console.log("Model already loaded. Skipping build.")
             return
-        
+
         self.console.log("Building model according to the data shape.")
         self.__build__(output_shape=xNd.shape[1:], show_summary=True)
-            
-        stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', min_delta=0.00001, mode='min', patience=20, restore_best_weights=True)
-        logger_callback = LoggerModel(name=INVNN_NAME, show_init=False, epochs=epochs)
+
+        stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode='min', patience=20, restore_best_weights=True)
+        logger_callback = LoggerModel(name=NNINV_NAME, show_init=False, epochs=epochs)
         self.console.log("Fitting model...")
 
-        hist = self.neural_network.fit(x2d, xNd, 
-                                epochs=epochs, 
-                                batch_size=batch_size, 
-                                shuffle=True,
-                                validation_split=0.2,
-                                callbacks=[stopping_callback, logger_callback],
-                                verbose=0)
+        hist = self.neural_network.fit(x2d, xNd,
+                                       epochs=epochs,
+                                       batch_size=batch_size,
+                                       shuffle=True,
+                                       validation_split=0.2,
+                                       callbacks=[stopping_callback,
+                                                  logger_callback],
+                                       verbose=0)
 
         self.console.log("Model fitted!")
-        self.save(hist)    
-        #self.show_predictions(dataNd=xNd_test, data2d=x2d_test, labels=y_test)
+        self.save(hist)
+        # self.show_predictions(dataNd=xNd_test, data2d=x2d_test, labels=y_test)
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/DBMInterface.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractDBM.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,563 +1,647 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import numpy as np
-from math import ceil, floor
 from queue import PriorityQueue
 from scipy import interpolate
 import dask.array as da
 from sklearn.neighbors import KDTree
 from numba_progress import ProgressBar
 import tensorflow as tf
 from tqdm import tqdm
+from enum import Enum
 
-from .tools import get_decode_pixel_priority, get_inv_proj_error, get_nd_indices_parallel, euclidean, get_proj_error_parallel, get_projection_errors_using_inverse_projection
-from ..utils import track_time_wrapper
+from .tools import binary_split, generate_windows, get_confidence_based_split, get_inv_proj_error, get_nd_indices_parallel, euclidean, get_pixel_priority, get_proj_error_parallel, get_projection_errors_using_inverse_projection, get_tasks_with_same_priority, get_window_borders
+from .AbstractNN import AbstractNN
+from ..utils import track_time_wrapper, INVERSE_PROJECTION_ERRORS_FILE, PROJECTION_ERRORS_INTERPOLATED_FILE, PROJECTION_ERRORS_INVERSE_PROJECTION_FILE
 from ..Logger import Logger, LoggerInterface
 
+DBM_DEFAULT_CHUNK_SIZE = 30000
 DBM_DEFAULT_RESOLUTION = 256
-FAST_DBM_STRATEGIES = ["binary_split", "confidence_split"]
+DEFAULT_WINDOW_SIZE = 8
+DBM_IMAGE_NAME = "boundary_map"
+DBM_CONFIDENCE_IMAGE_NAME = "boundary_map_confidence"
+
+PROJECTION_ERRORS_NEIGHBORS_NUMBER = 10
+
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
-class DBMInterface:
-    """ Decision Boundary Mapper Interface
-    
-    Methods to be implemented by the class that implements the DBMInterface:
-        fit (X_train, Y_train, X_test, Y_test, epochs=10, batch_size=128, load_folder = None)
-        generate_boundary_map (X_train, Y_train, X_test, Y_test, train_epochs=10, train_batch_size=128, resolution=DBM_DEFAULT_RESOLUTION)
+class FAST_DBM_STRATEGIES(Enum):
+    NONE = "none"
+    BINARY = "binary_split"
+    CONFIDENCE_BASED = "confidence_split"
+    HYBRID = "hybrid_split"
+
+    @classmethod
+    def list(cls):
+        return list(map(lambda c: c.value, cls))
+
+class AbstractDBM:
+    """ 
+    Decision Boundary Mapper Abstract class
+
+    Public methods that can be used:
+        refit_classifier \n
+        save_classifier  \n
+        load_classifier  \n
+        get_dbm          \n  
+        generate_inverse_projection_errors \n
+        generate_projection_errors         \n
+
+    Methods to be implemented by the class that implements this class:
         _predict2dspace_ (X)
-    
+
     Example of usage: 
-        class SuperBoundaryMapper(DBMInterface):
-            def fit (....):
+        class SuperBoundaryMapper(AbstractDBM):
+            def _predict2dspace_ (X):
                 # To be implemented
-            def generate_boundary_map (....):
-                # To be implemented
-            def _predict2dspace_ (....):
-                # To be implemented
-    """    
-    
-    def __init__(self, classifier, logger:LoggerInterface=None):
-        """Initializes the classifier and the logger
+    """
+
+    def __init__(self, classifier, logger: LoggerInterface | None = None):
+        """
+        Initializes the classifier and the logger
 
         Args:
-            classifier (Any): The classifier to be used
+            classifier (tf.keras.Model): The classifier to be used
             logger (LoggerInterface, optional): The logger for the outputting info messages. Defaults to None.
         """
         if logger is None:
             self.console = Logger(name="Decision Boundary Mapper - DBM")
         else:
             self.console = logger
-        
+
         self.console.log("Loaded classifier: " + classifier.name + "")
         self.classifier = classifier
-        
-    def fit(self, X_train:np.ndarray, Y_train:np.ndarray, 
-            X_test:np.ndarray, Y_test:np.ndarray,
-            epochs:int=10, batch_size:int=128, load_folder:bool = None):
-        """ Trains the classifier on the given data set.
-
-        Args:
-            X_train (np.ndarray): Training data set
-            Y_train (np.ndarray): Training data labels
-            X_test (np.ndarray): Testing data set
-            Y_test (np.ndarray): Testing data labels
-            epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 10.
-            batch_size (int, optional): Train batch size. Defaults to 128.
-        """
-        pass
-    
-    def refit_classifier(self, Xnd:np.ndarray, Y:np.ndarray, save_folder:str, epochs:int=2, batch_size:int=32):
-        """ Refits the classifier on the given data set.
+        self.neural_network: AbstractNN
+        self.X2d: np.ndarray
+        self.Xnd: np.ndarray
+        self.resolution: int
+
+    def refit_classifier(self, Xnd: np.ndarray, Y: np.ndarray, save_folder: str, epochs: int = 2, batch_size: int = 32):
+        """ 
+        Refits the classifier on the given data set.
 
         Args:             
-            Xnd (np.ndarray): 
-            Y (np.ndarray): 
+            Xnd (np.ndarray): The data set
+            Y (np.ndarray): The new labels
+            save_folder (str): Saving folder of the classifier
+            epochs (int, optional): Number of epochs. Defaults to 2.
+            batch_size (int): Number of training samples to be taken in a single batch. Defaults to 32.
         """
         self.console.log(f"Refiting classifier for {epochs} epochs and batch size {batch_size}, please wait...")
-        self.classifier.fit(Xnd, Y, epochs=epochs, batch_size=batch_size, verbose=0)
+        self.classifier.fit(Xnd, Y, epochs=epochs, batch_size=batch_size, verbose=0)  # type: ignore
         self.console.log("Finished refitting classifier")
-        self.console.log("Saving a copy of the retrained classifier...")
-        self.classifier.save(save_folder, save_format="tf")
-        self.console.log("A copy of the retrained classifier was saved!")
-    
-    def save_classifier(self, save_folder:str):
-        """ Saves a copy of the classifier.
+        self.save_classifier(save_folder=save_folder)
+
+    def save_classifier(self, save_folder: str):
+        """ 
+        Saves a copy of the classifier.
 
         Args:
             save_folder (str): The folder where the classifier will be saved
         """
-        self.classifier.save(save_folder, save_format="tf")
-    
-    def load_classifier(self, load_folder:str):
-        """ Loads a copy of the classifier.
+        self.console.log("Saving the classifier...")
+        self.classifier.save(save_folder, save_format="tf")  # type: ignore
+        self.console.log("A copy of the classifier was saved!")
+
+    def load_classifier(self, load_folder: str):
+        """ 
+        Loads a copy of the classifier.
 
         Args:
             load_folder (str): The folder where the classifier is saved
         """
         self.classifier = tf.keras.models.load_model(load_folder)
-    
-    def generate_boundary_map(self, 
-                              X_train:np.ndarray, Y_train:np.ndarray, 
-                              X_test:np.ndarray, Y_test:np.ndarray,
-                              train_epochs:int=10, train_batch_size:int=128,
-                              resolution:int=DBM_DEFAULT_RESOLUTION,
-                              use_fast_decoding:bool=False,
-                              projection:str=None
-                              ):
-        """ Generates a 2D boundary map of the classifier's decision boundary.
-
-        Args:
-            X_train (np.ndarray): Training data set
-            Y_train (np.ndarray): Training data labels
-            X_test (np.ndarray): Testing data set
-            Y_test (np.ndarray): Testing data labels
-            train_epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 10.
-            train_batch_size (int, optional): Train batch size. Defaults to 128.
-            show_predictions (bool, optional): If set to true 10 prediction examples are shown. Defaults to True.
-            resolution (int, optional): _description_. Defaults to DBM_DEFAULT_RESOLUTION = 256.
-            use_fast_decoding (bool, optional): If set to true the fast decoding algorithm is used. Defaults to False.
-            projection (str, optional): The projection to be used for the 2D space. Defaults to None.
-        Returns:
-            np.array: A 2D numpy array with the decision boundary map
-        
-        """
-        pass
-    
-    def _predict2dspace_(self, X2d: np.ndarray):
-        """ Predicts the labels for the given 2D data set.
+
+    def _predict2dspace_(self, X2d: np.ndarray | list[tuple[float, float]]) -> tuple:
+        """ 
+        Predicts the labels for the given 2D data set.
+        IMPORTANT: This method should be implemented by the classes that implement this class
 
         Args:
             X2d (np.ndarray): The 2D data set
-        
+
         Returns:
             predicted_labels (np.array): The predicted labels for the given 2D data set
-            predicted_confidences (np.array): The predicted probabilities for the given 2D data set
-            spaceNd (np.array): The decoded nD space
+            predicted_confidences (np.array): The predicted probabilities for the given 2D data set, for each data point the confidence is returned (i.e. the maximum probability)
+            predictions (np.array): The predicted probabilities for the given 2D data set, for each data point a list of probabilities is returned
         """
-        pass
-    
-    @track_time_wrapper(logger=time_tracker_console)
-    def generate_inverse_projection_errors(self, resolution:int, save_folder:str = None):
-        """ Calculates the inverse projection errors of the given data.
+        return None, None, None
+
+    def get_dbm(self, fast_decoding_strategy: FAST_DBM_STRATEGIES, resolution: int, load_folder: str) -> tuple:
+        """
+        Delegates the generation of the DBM to the according functionality based on the fast_decoding_strategy
 
         Args:
-            Xnd (np.array): The nd inverse projection of the data.
-        
+            fast_decoding_strategy (FAST_DBM_STRATEGIES): The strategy to use for the generation of the DBM
+            resolution (int): The desired resolution of the DBM image
+            load_folder (str): The folder in which we save the results
+
         Returns:
-            errors (np.ndarray): The inverse projection errors matrix of the given data. (resolution x resolution)
+            img (np.ndarray): The DBM image
+            img_confidence (np.ndarray): The DBM confidence image
         """
-            
-        self.console.log("Calculating the inverse projection errors of the given data")
-        errors = np.zeros((resolution, resolution))
-        
-        w, h = 1, 1
-        
-        i = 0
-                
-        current_row = np.array([(i / resolution, j / resolution) for j in range(resolution) ])
-        next_row = np.array([((i + 1) / resolution, j / resolution) for j in range(resolution) ])            
-        data_2d = np.concatenate((current_row, next_row))
-        data_nd = self.neural_network.decode(data_2d)
-        
-        previous_row_nd = None
-        current_row_nd = data_nd[:resolution]
-        next_row_nd = data_nd[resolution:]
-        
-        
-        for i in tqdm(range(resolution)):
-            for j in range(resolution):
-                dw = w if (j - w < 0) or (j + w >= resolution) else 2 * w
-                dh = h if (i - h < 0) or (i + h >= resolution) else 2 * h
-                xnd = current_row_nd[j] 
-                xl = current_row_nd[j-w] if j - w >= 0 else xnd
-                xr = current_row_nd[j+w] if j + w < resolution else xnd
-                yl = previous_row_nd[j] if previous_row_nd is not None else xnd
-                yr = next_row_nd[j] if next_row_nd is not None else xnd
-                                                
-                dx = (xl - xr) / dw
-                dy = (yl - yr) / dh  
-                errors[i,j] = get_inv_proj_error(dx, dy)
-            
-            previous_row_nd = current_row_nd
-            current_row_nd = next_row_nd
-            if i + 2 < resolution:
-                next_row = np.array([((i + 2) / resolution, j / resolution) for j in range(resolution) ])
-                next_row_nd = self.neural_network.decode(next_row)
-            else:
-                next_row_nd = None
-                
-        # normalizing the errors to be in the range [0,1]
-        errors = (errors - np.min(errors)) / (np.max(errors) - np.min(errors))
-        
-        if save_folder is not None:
-            self.console.log("Saving the inverse projection errors results")
-            save_path = os.path.join(save_folder, "inverse_projection_errors.npy")
-            with open(save_path, "wb") as f:
-                np.save(f, errors)
-            self.console.log("Saved inverse projection errors results!")
-            
-        return errors
-    
+        save_img_path = os.path.join(load_folder, DBM_IMAGE_NAME)
+        save_img_confidence_path = os.path.join(load_folder, DBM_CONFIDENCE_IMAGE_NAME)
+
+        match fast_decoding_strategy:
+            case FAST_DBM_STRATEGIES.NONE:
+                img, img_confidence = self._get_img_dbm_(resolution)
+            case FAST_DBM_STRATEGIES.BINARY:
+                save_img_path += f"_fast_{FAST_DBM_STRATEGIES.BINARY.value}"
+                save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.BINARY.value}"
+                img, img_confidence = self._get_img_dbm_fast_(resolution)
+            case FAST_DBM_STRATEGIES.CONFIDENCE_BASED:
+                save_img_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_BASED.value}"
+                save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_BASED.value}"
+                img, img_confidence = self._get_img_dbm_fast_confidences_strategy(resolution)
+            case FAST_DBM_STRATEGIES.HYBRID:
+                save_img_path += f"_fast_{FAST_DBM_STRATEGIES.HYBRID.value}"
+                save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.HYBRID.value}"
+                img, img_confidence = self._get_img_dbm_fast_hybrid_strategy(resolution)
+
+        with open(f"{save_img_path}.npy", 'wb') as f:
+            np.save(f, img)  # type: ignore
+        with open(f"{save_img_confidence_path}.npy", 'wb') as f:
+            np.save(f, img_confidence)  # type: ignore
+
+        return img, img_confidence  # type: ignore
+
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_(self, resolution:int):
-        """ This function generates the 2D image of the boundary map using the trained autoencoder and classifier.
+    def _get_img_dbm_(self, resolution: int):
+        """ 
+        This function generates the 2D image of the boundary map using the trained neural network and the classifier.
 
         Args:
             resolution (int): The resolution of the 2D image to be generated 
 
         Returns:
             img (np.array): The 2D image of the boundary map
             img_confidence (np.array): The confidence of map of each pixel of the 2D image of the boundary map
-            img_space_Nd (np.array): The nD space points
-      
+            
         Example:
             >>> img, img_confidence = self._get_img_dbm_(resolution = 100)
         """
         space2d = np.array([(i / resolution, j / resolution) for i in range(resolution) for j in range(resolution)])
         self.console.log("Predicting labels for the 2D boundary mapping using the nD data and the trained classifier...")
-        
-        chunk_size = 10000
-        chunks = (resolution * resolution) // chunk_size + 1        
+
+        chunk_size = DBM_DEFAULT_CHUNK_SIZE
+        chunks = (resolution * resolution) // chunk_size + 1
         space2d_chunks = np.array_split(space2d, chunks)
-        
+
         img, img_confidence = np.array([]), np.array([])
-        
+
         chunk_index = 0
         for space2d_chunk in space2d_chunks:
             chunk_index += 1
             self.console.log(f"Predicting labels for the 2D boundary mapping using the nD data and the trained classifier... (chunk {chunk_index}/{len(space2d_chunks)})")
-            predicted_labels, predicted_confidence = self._predict2dspace_(space2d_chunk)
+            predicted_labels, predicted_confidence, _ = self._predict2dspace_(space2d_chunk)
             img = np.concatenate((img, predicted_labels))
             img_confidence = np.concatenate((img_confidence, predicted_confidence))
-        
+
         img = img.reshape((resolution, resolution))
-        img_confidence = img_confidence.reshape((resolution, resolution))        
-        
+        img_confidence = img_confidence.reshape((resolution, resolution))
+
         return (img, img_confidence)
-    
+
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_fast_(self, resolution:int, computational_budget=None, interpolation_method:str="linear"):
+    def _get_img_dbm_fast_(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
         """
         This function generates the 2D image of the boundary map. It uses a fast algorithm to generate the image.
-        
-        ATTENTION: Highly recommended to use resolution = 2 ^ n, where n is an integer number (powers of 2).
-        
+
         Args:
             resolution (int): the resolution of the 2D image to be generated
             computational_budget (int, optional): The computational budget to be used. Defaults to None.
             interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
                                                   Defaults to "linear". The options are: "nearest", "linear", "cubic"
+            window_size (int, optional): The window size to be used. Defaults to 8.
+
         Returns:
             img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
             spaceNd: The nD space points
         Example:
             >>> img, img_confidence = self._get_img_dbm_fast_(resolution=32, computational_budget=1000)
         """
+        assert(window_size < resolution)
+        assert(window_size > 0)
+        assert(int(window_size) == window_size)
         # ------------------------------------------------------------
-        # Setting the initial parameters
-        WINDOW_SIZE = 8
-        NEIGHBORS_NUMBER = 4
-        
-        assert(resolution > WINDOW_SIZE)
-        
-        INITIAL_RESOLUTION = resolution // WINDOW_SIZE
-        
-        if computational_budget is None:
-            computational_budget = resolution * resolution
-        
-        assert(computational_budget > INITIAL_RESOLUTION * INITIAL_RESOLUTION)
-        INITIAL_COMPUTATIONAL_BUDGET = computational_budget
-        
-        if (resolution % INITIAL_RESOLUTION != 0):
-            self.console.warn(f"The required resolution is not a multiple of the initial window size ({WINDOW_SIZE} x {WINDOW_SIZE})")
-            self.console.log("The resolution will be set to the closest multiple of the window size")
-            resolution = INITIAL_RESOLUTION * WINDOW_SIZE
-            self.resolution = resolution   
-            self.console.log(f"Resolution was set to {resolution} x {resolution}")
-            
-        window_size = WINDOW_SIZE
-        # ------------------------------------------------------------
-        
-        # ------------------------------------------------------------
-        img = np.zeros((resolution, resolution))
+        INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
+
+        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(window_size=window_size, 
+                                                                                                        resolution=resolution, 
+                                                                                                        computational_budget=computational_budget,
+                                                                                                        confidence_interpolation_method=interpolation_method)
+           
+        # analyze the initial points and generate the priority queue
         priority_queue = PriorityQueue()
-        # ------------------------------------------------------------
-                
-        # ------------------------------------------------------------
-        # generate the initial points
-        self.console.log(f"Generating the initial central points within each window... total number of windows ({(INITIAL_RESOLUTION * INITIAL_RESOLUTION)})")
-        
-        space2d = [((i * window_size + window_size / 2 - 0.5) / resolution, (j * window_size + window_size / 2 - 0.5) / resolution) for i in range(INITIAL_RESOLUTION) for j in range(INITIAL_RESOLUTION)]
-        
-        predicted_labels, predicted_confidence = self._predict2dspace_(space2d)
-        
-        predictions = predicted_labels.reshape((INITIAL_RESOLUTION, INITIAL_RESOLUTION))
-        confidences = predicted_confidence.reshape((INITIAL_RESOLUTION, INITIAL_RESOLUTION))        
+        priority_queue = self._update_priority_queue_(priority_queue, img, indexes, sizes, labels)
         
-        # initialize the nD space
-        
-        computational_budget -= INITIAL_RESOLUTION * INITIAL_RESOLUTION
-                
-        # fill the initial points in the 2D image
-        for i in range(INITIAL_RESOLUTION):
-            for j in range(INITIAL_RESOLUTION):
-                x0, x1, y0, y1 = i * window_size, (i+1) * window_size, j * window_size, (j+1) * window_size
-                img[x0:x1, y0:y1] = predictions[i,j]
-        # -------------------------------------
-        
-        # collecting the indexes of the actual computed pixels in the 2D image and the confidence of each pixel
-        # creating an artificial border for the 2D confidence image
-        confidence_map = []
-        
-        if interpolation_method != "nearest":
-            border_indices = [(i * window_size + window_size / 2 - 0.5, 0) for i in range(INITIAL_RESOLUTION)] + \
-                            [(i * window_size + window_size / 2 - 0.5, resolution - 1) for i in range(INITIAL_RESOLUTION)] + \
-                            [(0, i * window_size + window_size / 2 - 0.5) for i in range(-1, INITIAL_RESOLUTION+1)] + \
-                            [(resolution - 1, i * window_size + window_size / 2 - 0.5) for i in range(-1, INITIAL_RESOLUTION + 1)]
-            
-            space2d_border = [(i / resolution, j / resolution) for (i,j) in border_indices]
-            _, confidences_border = self._predict2dspace_(space2d_border)
-            computational_budget -= len(space2d_border)
-            confidence_map = [(i, j, conf) for (i,j),conf in zip(border_indices, confidences_border)]
-                    
-        # analyze the initial points and generate the priority queue        
-        for i in range(INITIAL_RESOLUTION):
-            for j in range(INITIAL_RESOLUTION):
-                x, y = i * window_size + window_size / 2 - 0.5, j * window_size + window_size / 2 - 0.5
-                confidence_map.append((x,y,confidences[i,j]))                
-                priority = get_decode_pixel_priority(img, x, y, window_size, predictions[i,j])
-                if priority != -1:
-                    priority_queue.put((priority, (window_size, x, y)))
-
         # -------------------------------------
         # start the iterative process of filling the image
         self.console.log(f"Starting the iterative process of refining windows...")
-        while computational_budget > 0 and not priority_queue.empty():    
-            # take the highest priority task
-            priority, item = priority_queue.get()
-            
-            # getting all the items with the same priority
-            items = [item]
-            if not priority_queue.empty():
-                next_priority, next_item = priority_queue.get()
-                while priority == next_priority:
-                    items.append(next_item)
-                    if priority_queue.empty():
-                        break
-                    next_priority, next_item = priority_queue.get()
-                if priority != next_priority:
-                    priority_queue.put((next_priority, next_item))
-            
-            
+
+        while computational_budget > 0 and not priority_queue.empty():
+            # take the highest priority tasks
+            items = get_tasks_with_same_priority(priority_queue)
+
             space2d, indices = [], []
             single_points_space, single_points_indices = [], []
-            valid_items = []
-            
-            for item in items:            
-                (window_size, i, j) = item
+            window_sizes = []
+
+            for (w, h, i, j) in items:
                 
-                if window_size == 1:
-                    single_points_indices += [(int(i), int(j))]
-                    single_points_space += [(i / resolution, j / resolution)]
+                if w == 1 and h == 1:
+                    single_points_space.append((j / resolution, i / resolution))
+                    single_points_indices.append((int(j), int(i)))
                     continue
                 
-                window_size = window_size / NEIGHBORS_NUMBER
-                neighbors = [(i - window_size, j - window_size), (i - window_size, j + window_size), (i + window_size, j - window_size), (i + window_size, j + window_size)]
-                space2d += [(x / resolution, y / resolution) for (x, y) in neighbors]
-                indices += neighbors                                                
-                valid_items.append(item)
-            
-            
-            space = space2d + single_points_space
-            
+                neighbors, sizes = binary_split(i, j, w, h)
+                space2d += [(y / resolution, x / resolution) for (x, y) in neighbors]
+                window_sizes += sizes
+                indices += neighbors
+
+            space = single_points_space + space2d
+
             # check if the computational budget is enough and update it
             if computational_budget - len(space) < 0:
                 self.console.warn("Computational budget exceeded, stopping the process")
                 break
-            
-            computational_budget -= len(space)
-            
+
             # decode the space
-            predicted_labels, predicted_confidence = self._predict2dspace_(space)
-            # copy the image to a new one, the new image will be updated with the new labels, the old one will be used to calculate the priorities
-            new_img = np.copy(img)            
-            
+            predicted_labels, predicted_confidence, _ = self._predict2dspace_(space)
+            computational_budget -= len(space)
+
+            single_points_labels = predicted_labels[:len(single_points_space)]
+            single_points_confidence = predicted_confidence[:len(single_points_space)]
+            predicted_labels = predicted_labels[len(single_points_space):]
+            predicted_confidence = predicted_confidence[len(single_points_space):]
+         
+            # fill the new image with the new labels and update the priority queue
+            for (w, h), (x, y), label, conf in zip(window_sizes, indices, predicted_labels, predicted_confidence):
+                # all the pixels in the window are set to the same label
+                # starting from the top left corner of the window
+                # ending at the bottom right corner of the window
+                # the +1 is because the range function is not inclusive
+                confidence_map.append((y, x, conf))
+                x0, x1, y0, y1 = get_window_borders(x, y, w, h)
+                img[y0:y1 + 1, x0:x1 + 1] = label
+          
             # fill the new image with the single points
-            single_points_labels = predicted_labels[len(space2d):]
-            single_points_confidences  = predicted_confidence[len(space2d):]
-            #single_points_spaceNd = predicted_spaceNd[len(space2d):]
-            
             for i in range(len(single_points_indices)):
-                new_img[single_points_indices[i]] = single_points_labels[i]
-                #img_space_Nd[single_points_indices[i]] = single_points_spaceNd[i]
-                confidence_map.append((single_points_indices[i][0], single_points_indices[i][1], single_points_confidences[i]))                
-                           
-            predicted_labels = predicted_labels[:len(space2d)]
-            predicted_confidence = predicted_confidence[:len(space2d)]
-            #predicted_spaceNd = predicted_spaceNd[:len(space2d)] 
-            
-            # fill the new image with the new labels and update the priority queue
-            for index in range(len(valid_items)):
-                (window_size, i, j) = valid_items[index]
-                neighbors = indices[index*NEIGHBORS_NUMBER:(index+1)*NEIGHBORS_NUMBER]
-                neighbors_labels = predicted_labels[index*NEIGHBORS_NUMBER:(index+1)*NEIGHBORS_NUMBER]
-                confidences = predicted_confidence[index*NEIGHBORS_NUMBER:(index+1)*NEIGHBORS_NUMBER]
-                #spaceNd = predicted_spaceNd[index*NEIGHBORS_NUMBER:(index+1)*NEIGHBORS_NUMBER]
-                
-                new_window_size = window_size / NEIGHBORS_NUMBER
-                
-                for (x, y), label, conf in zip(neighbors, neighbors_labels, confidences):
-                    # all the pixels in the window are set to the same label
-                    # starting from the top left corner of the window
-                    # ending at the bottom right corner of the window
-                    # the +1 is because the range function is not inclusive
-                    confidence_map.append((x, y, conf))
-                    if new_window_size >= 1:
-                        x0, x1, y0, y1 = ceil(x-new_window_size), floor(x + new_window_size), ceil(y - new_window_size), floor(y + new_window_size)
-                        new_img[x0:x1 + 1, y0:y1 + 1] = label           
-                    else:
-                        new_img[int(x), int(y)] = label
-                
-                # update the priority queue after the window has been filled
-                for (x, y), label in zip(neighbors, neighbors_labels):
-                    priority = get_decode_pixel_priority(img, x, y, 2 * new_window_size, label)
-                    if priority != -1:
-                        priority_queue.put((priority, (2 * new_window_size, x, y)))
-            
-            # update the image        
-            img = new_img
-        
+                img[single_points_indices[i]] = single_points_labels[i]
+                confidence_map.append((single_points_indices[i][0], single_points_indices[i][1], single_points_confidence[i]))
+
+            # update the priority queue
+            priority_queue = self._update_priority_queue_(priority_queue, img, indices, window_sizes, predicted_labels)
+
         # summary
         self.console.log(f"Finished decoding the image, initial computational budget: {INITIAL_COMPUTATIONAL_BUDGET} computational budget left: {computational_budget}")
         self.console.log(f"Items left in the priority queue: {priority_queue.qsize()}")
-        
+
         # generating the confidence image using interpolation based on the confidence map
         img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
                                                             resolution=resolution,
                                                             method=interpolation_method).T
-        
 
         return img, img_confidence
 
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_fast_confidences_strategy(self, resolution:int, computational_budget=None, interpolation_method:str="linear"):
+    def _get_img_dbm_fast_confidences_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
         """
         This function generates the 2D image of the boundary map. It uses a fast algorithm that uses a confidence based strategy to generate the image.
-        
-        ATTENTION: Highly recommended to use resolution = 2 ^ n, where n is an integer number (powers of 2).
-        
+
         Args:
             resolution (int): the resolution of the 2D image to be generated
             computational_budget (int, optional): The computational budget to be used. Defaults to None.
             interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
                                                   Defaults to "linear". The options are: "nearest", "linear", "cubic"
+            window_size (int, optional): The window size to be used. Defaults to 8.
+
         Returns:
             img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
             spaceNd: The nD space points
         Example:
             >>> img, img_confidence = self._get_img_dbm_fast_confidences_strategy(resolution=32, computational_budget=1000)
         """
+        assert(window_size < resolution)
+        assert(window_size > 0)
+        assert(int(window_size) == window_size)
         # ------------------------------------------------------------
         # Setting the initial parameters
-        WINDOW_SIZE = 8
-        NEIGHBORS_NUMBER = 4
-        
-        assert(resolution > WINDOW_SIZE)
-        
-        INITIAL_RESOLUTION = resolution // WINDOW_SIZE
-        
-        if computational_budget is None:
-            computational_budget = resolution * resolution
-        
-        assert(computational_budget > INITIAL_RESOLUTION * INITIAL_RESOLUTION)
-        INITIAL_COMPUTATIONAL_BUDGET = computational_budget
-        
-        if (resolution % INITIAL_RESOLUTION != 0):
-            self.console.warn(f"The required resolution is not a multiple of the initial window size ({WINDOW_SIZE} x {WINDOW_SIZE})")
-            self.console.log("The resolution will be set to the closest multiple of the window size")
-            resolution = INITIAL_RESOLUTION * WINDOW_SIZE
-            self.resolution = resolution   
-            self.console.log(f"Resolution was set to {resolution} x {resolution}")
-            
-        window_size = WINDOW_SIZE
-        # ------------------------------------------------------------
-        
-        # ------------------------------------------------------------
-        img = np.zeros((resolution, resolution))
-        priority_queue = PriorityQueue()
+        INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
+
+        initial_resolution = resolution // window_size
+        img = np.zeros((resolution, resolution), dtype=np.int16)
+        img_indexes = np.zeros((resolution, resolution, 2), dtype=np.int16)
         # ------------------------------------------------------------
-                
+
         # ------------------------------------------------------------
         # generate the initial points
-        self.console.log(f"Generating the initial central points within each window... total number of windows ({(INITIAL_RESOLUTION * INITIAL_RESOLUTION)})")
-        
-        space2d = [((i * window_size + window_size / 2 - 0.5) / resolution, (j * window_size + window_size / 2 - 0.5) / resolution) for i in range(INITIAL_RESOLUTION) for j in range(INITIAL_RESOLUTION)]
-        
-        predicted_labels, predicted_confidence = self._predict2dspace_(space2d)
-        
-        predictions = predicted_labels.reshape((INITIAL_RESOLUTION, INITIAL_RESOLUTION))
-        confidences = predicted_confidence.reshape((INITIAL_RESOLUTION, INITIAL_RESOLUTION))        
-        
-        # initialize the nD space
+        indexes, sizes, initial_resolution = generate_windows(window_size, initial_resolution=initial_resolution, resolution=resolution)
+        space2d = np.array(indexes) / resolution  
+        predicted_labels, predicted_confidence, predicted_confidences = self._predict2dspace_(space2d)
+        pseudo_conf_img = np.zeros((resolution, resolution, len(predicted_confidences[0])))
+
+        computational_budget -= len(indexes)
+
+        # creating an artificial border for the 2D confidence image
+        confidence_map = self._generate_confidence_border_(window_size=window_size, initial_resolution=initial_resolution, resolution=resolution) if interpolation_method != "nearest" else []
+        computational_budget -= len(confidence_map)
+
+        # fill the initial points in the 2D image
+        for (w, h), (x, y), label, conf, confidences in zip(sizes, indexes, predicted_labels, predicted_confidence, predicted_confidences):
+            x0, x1, y0, y1 = get_window_borders(x, y, w, h)
+            img[x0:x1 + 1, y0:y1 + 1] = label
+            confidence_map.append((y, x, conf))
+      
+            img_indexes[x0:x1 + 1, y0:y1 + 1] = (y, x)
+            pseudo_conf_img[x0:x1 + 1, y0:y1 + 1, :] = confidences
+           
+        # analyze the initial points and generate the priority queue
+        priority_queue = PriorityQueue()
+        priority_queue = self._update_priority_queue_(priority_queue, img, indexes, sizes, predicted_labels)
         
-        computational_budget -= INITIAL_RESOLUTION * INITIAL_RESOLUTION
                 
-        # fill the initial points in the 2D image
-        for i in range(INITIAL_RESOLUTION):
-            for j in range(INITIAL_RESOLUTION):
-                x0, x1, y0, y1 = i * window_size, (i+1) * window_size, j * window_size, (j+1) * window_size
-                img[x0:x1, y0:y1] = predictions[i,j]
         # -------------------------------------
-        
-        # collecting the indexes of the actual computed pixels in the 2D image and the confidence of each pixel
-        # creating an artificial border for the 2D confidence image
-        confidence_map = []
-        
-        if interpolation_method != "nearest":
-            border_indices = [(i * window_size + window_size / 2 - 0.5, 0) for i in range(INITIAL_RESOLUTION)] + \
-                            [(i * window_size + window_size / 2 - 0.5, resolution - 1) for i in range(INITIAL_RESOLUTION)] + \
-                            [(0, i * window_size + window_size / 2 - 0.5) for i in range(-1, INITIAL_RESOLUTION+1)] + \
-                            [(resolution - 1, i * window_size + window_size / 2 - 0.5) for i in range(-1, INITIAL_RESOLUTION + 1)]
+        # start the iterative process of filling the image
+        self.console.log(f"Starting the iterative process of refining windows...")
+
+        iteration = 0
+        while computational_budget > 0 and not priority_queue.empty():
+            iteration += 1
+            print("Priority queue size: ", priority_queue.qsize())
+            # take the highest priority tasks
+            items = get_tasks_with_same_priority(priority_queue)
+
+            space2d, indices, window_sizes = [], [], []
+            single_points_space, single_points_indices = [], []
+
+            for (w, h, i, j) in items:
+                if w == 1 and h == 1:
+                    single_points_space.append((j / resolution, i / resolution))
+                    single_points_indices.append((int(j), int(i)))
+                    continue
+                
+                neighbors, sizes = get_confidence_based_split(img, pseudo_conf_img, img_indexes, i, j, w, h)
+                space2d += [(y / resolution, x / resolution) for (x, y) in neighbors]
+                window_sizes += sizes
+                indices += neighbors
+
+            space = single_points_space + space2d
+
+            # check if the computational budget is enough and update it
+            if computational_budget - len(space) < 0:
+                self.console.warn("Computational budget exceeded, stopping the process")
+                break
+
+            # decode the space
+            predicted_labels, predicted_confidence, predicted_confidences = self._predict2dspace_(space)
+            computational_budget -= len(space)
             
-            space2d_border = [(i / resolution, j / resolution) for (i,j) in border_indices]
-            _, confidences_border = self._predict2dspace_(space2d_border)
-            computational_budget -= len(space2d_border)
-            confidence_map = [(i, j, conf) for (i,j),conf in zip(border_indices, confidences_border)]
-        
-        #ATTENTION (!!!): This function is just a scratch for the confidence based strategy and it is not implemented yet
-        #TODO: implement the confidence based strategy here        
-        
+            single_points_labels = predicted_labels[:len(single_points_space)]
+            single_points_confidence = predicted_confidence[:len(single_points_space)]
+            single_points_confidences = predicted_confidences[:len(single_points_space)]
+            
+            predicted_labels = predicted_labels[len(single_points_space):]
+            predicted_confidence = predicted_confidence[len(single_points_space):]
+            predicted_confidences = predicted_confidences[len(single_points_space):]
+
+            # fill the new image with the new labels and update the priority queue
+            for (w, h), (x, y), label, conf, confidences in zip(window_sizes, indices, predicted_labels, predicted_confidence, predicted_confidences):
+                # all the pixels in the window are set to the same label
+                # starting from the top left corner of the window
+                # ending at the bottom right corner of the window
+                # the +1 is because the range function is not inclusive
+                confidence_map.append((y, x, conf))
+                x0, x1, y0, y1 = get_window_borders(x, y, w, h)
+                img[y0:y1 + 1, x0:x1 + 1] = label
+                
+                img_indexes[y0:y1 + 1, x0:x1 + 1] = (x,y)
+                pseudo_conf_img[y0:y1 + 1, x0:x1 + 1, :] = confidences
+
+            # fill the new image with the single points
+            for i in range(len(single_points_indices)):
+                img[single_points_indices[i]] = single_points_labels[i]
+                pseudo_conf_img[single_points_indices[i]] = single_points_confidences[i]
+                confidence_map.append((single_points_indices[i][0], single_points_indices[i][1], single_points_confidence[i]))
+
+            # update the priority queue
+            priority_queue = self._update_priority_queue_(priority_queue, img, indices, window_sizes, predicted_labels)
+
+
         # summary
         self.console.log(f"Finished decoding the image, initial computational budget: {INITIAL_COMPUTATIONAL_BUDGET} computational budget left: {computational_budget}")
         self.console.log(f"Items left in the priority queue: {priority_queue.qsize()}")
-        
+
         # generating the confidence image using interpolation based on the confidence map
         img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
                                                             resolution=resolution,
                                                             method=interpolation_method).T
-        
 
         return img, img_confidence
 
-    def _generate_interpolated_image_(self, sparse_map, resolution, method='linear'):
-        """A private method that uses interpolation to generate the values for the 2D space image
+    @track_time_wrapper(logger=time_tracker_console)
+    def _get_img_dbm_fast_hybrid_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
+        """
+        This function generates the 2D image of the boundary map. It uses a fast algorithm that uses a binary split based strategy to generate the image.
+
+        Args:
+            resolution (int): the resolution of the 2D image to be generated
+            computational_budget (int, optional): The computational budget to be used. Defaults to None.
+            interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
+                                                  Defaults to "linear". The options are: "nearest", "linear", "cubic"
+            window_size (int, optional): The window size to be used. Defaults to 8.
+        Returns:
+            img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
+            spaceNd: The nD space points
+        Example:
+            >>> img, img_confidence = self._get_img_dbm_fast_hybrid_strategy(resolution=32, computational_budget=1000)
+        """
+        assert(window_size < resolution)
+        assert(window_size > 0)
+        assert(int(window_size) == window_size)
+        # ------------------------------------------------------------
+        # Setting the initial parameters
+        INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
+
+        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(window_size=window_size, 
+                                                                                                        resolution=resolution, 
+                                                                                                        computational_budget=computational_budget,
+                                                                                                        confidence_interpolation_method=interpolation_method)
+
+        # analyze the initial windows
+        items_to_decode = []
+        for index in range(len(indexes)):
+            (x, y), (w, h) = indexes[index], sizes[index]
+            priority = get_pixel_priority(img, y, x, w, h, labels[index])
+            if priority == -1:
+                continue
+            
+            items_to_decode.append((w, h, x, y))
+    
+  
+        # -------------------------------------
+        # start the process of filling the image
+        space, space_indices = [], []   
+        self.console.log(f"Starting the iterative process of refining windows...")
+        for (w, h, i, j) in items_to_decode:
+            x0, x1, y0, y1 = get_window_borders(i, j, w, h)
+            for y in range(y0, y1 + 1):
+                for x in range(x0, x1 + 1):
+                    space_indices.append((y, x))
+                    space.append((y / resolution, x / resolution))
+                
+        
+        # check if the computational budget is enough and update it
+        if computational_budget - len(space) < 0:
+            self.console.warn("Computational budget exceeded!")
+
+        # decode the space
+        predicted_labels, predicted_confidence, _ = self._predict2dspace_(space)  
+        computational_budget -= len(space)
+
+        
+        # fill the new image with the new labels
+        for (i, j), label, conf in zip(space_indices, predicted_labels, predicted_confidence):
+            confidence_map.append((i, j, conf))
+            img[i, j] = label
+
+        # summary
+        self.console.log(f"Finished decoding the image, initial computational budget: {INITIAL_COMPUTATIONAL_BUDGET} computational budget left: {computational_budget}")
+
+        # generating the confidence image using interpolation based on the confidence map
+        img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
+                                                            resolution=resolution,
+                                                            method=interpolation_method).T
+
+        return img, img_confidence
+
+    def _fill_initial_windows_(self, window_size: int, resolution: int, computational_budget: int, confidence_interpolation_method: str = "linear"):
+        
+        initial_resolution = resolution // window_size
+        img = np.zeros((resolution, resolution), dtype=np.int16)
+        # ------------------------------------------------------------
+
+        # ------------------------------------------------------------
+        # generate the initial points
+        indexes, sizes, initial_resolution = generate_windows(window_size, initial_resolution=initial_resolution, resolution=resolution)
+        # creating an artificial border for the 2D confidence image
+        confidence_map = self._generate_confidence_border_(window_size=window_size, initial_resolution=initial_resolution, resolution=resolution) if confidence_interpolation_method != "nearest" else []
+        computational_budget -= len(confidence_map)
+
+        # ------------------------------------------------------------   
+        space2d = np.array(indexes) / resolution  
+        predicted_labels, predicted_confidence, _ = self._predict2dspace_(space2d)
+      
+        computational_budget -= len(indexes)
+
+        # fill the initial points in the 2D image
+        for (w, h), (x, y), label, conf in zip(sizes, indexes, predicted_labels, predicted_confidence):
+            x0, x1, y0, y1 = get_window_borders(x, y, w, h)
+            img[x0:x1 + 1, y0:y1 + 1] = label
+            confidence_map.append((y, x, conf))
+        
+        return indexes, sizes, predicted_labels, computational_budget, img, confidence_map
+
+    def _generate_confidence_border_(self, window_size: int, initial_resolution: int, resolution: int):
+        border_indices = [(i * window_size + window_size / 2 - 0.5, 0) for i in range(initial_resolution)] + \
+                [(i * window_size + window_size / 2 - 0.5, resolution - 1) for i in range(initial_resolution)] + \
+                [(0, i * window_size + window_size / 2 - 0.5) for i in range(-1, initial_resolution + 1)] + \
+                [(resolution - 1, i * window_size + window_size / 2 - 0.5) for i in range(-1, initial_resolution + 1)]
+
+        space2d_border = np.array(border_indices) / resolution
+        _, confidences_border, _ = self._predict2dspace_(space2d_border)
+        confidence_map = [(i, j, conf) for (i, j), conf in zip(border_indices, confidences_border)]
+        return confidence_map
+
+    def _update_priority_queue_(self, priority_queue, img, indexes, sizes, labels):
+        for (w, h), (x, y), label in zip(sizes, indexes, labels):
+            priority = get_pixel_priority(img, y, x, w, h, label)
+            if priority != -1:
+                priority_queue.put((priority, (w, h, y, x)))
+        return priority_queue
+
+    @track_time_wrapper(logger=time_tracker_console)
+    def generate_inverse_projection_errors(self, resolution: int, save_folder: str | None = None):
+        """ 
+        Calculates the inverse projection errors of the given data.
+
+        Args:
+            resolution (int): The resolution of the errors image to generate
+            save_folder (str): The path of the folder in which we want to save the results. Defaults to None
+
+        Returns:
+            errors (np.ndarray): The inverse projection errors matrix of the given data. (resolution x resolution)
+        """
+
+        self.console.log("Calculating the inverse projection errors of the given data")
+        errors = np.zeros((resolution, resolution))
+
+        w, h = 1, 1
+
+        current_row = np.array([(0, j / resolution) for j in range(resolution)])
+        next_row = np.array([( 1 / resolution, j / resolution) for j in range(resolution)])
+        data_2d = np.concatenate((current_row, next_row))
+        data_nd = self.neural_network.decode(data_2d)
+
+        previous_row_nd = None
+        current_row_nd: np.ndarray = data_nd[:resolution]
+        next_row_nd: np.ndarray = data_nd[resolution:]
+
+        for i in tqdm(range(resolution)):
+            for j in range(resolution):
+                dw = w if (j - w < 0) or (j + w >= resolution) else 2 * w
+                dh = h if (i - h < 0) or (i + h >= resolution) else 2 * h
+                xnd = current_row_nd[j]
+                xl = current_row_nd[j-w] if j - w >= 0 else xnd
+                xr = current_row_nd[j+w] if j + w < resolution else xnd
+                yl = previous_row_nd[j] if previous_row_nd is not None else xnd
+                yr = next_row_nd[j] if next_row_nd is not None else xnd
+
+                dx = (xl - xr) / dw
+                dy = (yl - yr) / dh
+                errors[i, j] = get_inv_proj_error(dx, dy)
+
+            previous_row_nd = current_row_nd
+            current_row_nd = next_row_nd
+            if i + 2 < resolution:
+                next_row = np.array([((i + 2) / resolution, j / resolution) for j in range(resolution)])
+                next_row_nd = self.neural_network.decode(next_row)
+            else:
+                next_row_nd = None  # type: ignore
+
+        # normalizing the errors to be in the range [0,1]
+        errors = (errors - np.min(errors)) / (np.max(errors) - np.min(errors))
+
+        if save_folder is not None:
+            self.console.log("Saving the inverse projection errors results")
+            save_path = os.path.join(save_folder, INVERSE_PROJECTION_ERRORS_FILE)
+            with open(save_path, "wb") as f:
+                np.save(f, errors)
+            self.console.log("Saved inverse projection errors results!")
+
+        return errors
+
+    def _generate_interpolated_image_(self, sparse_map, resolution:int, method:str='linear'):
+        """
+        A private method that uses interpolation to generate the values for the 2D space image
            The sparse map is a list of tuples (x, y, data)
            The sparse map represents a structured but non uniform grid of data values
            Therefore usual rectangular interpolation methods are not suitable
            For the interpolation we use the scipy.interpolate.griddata function with the linear method
         Args:
             sparse_map (list): a list of tuples (x, y, data) where x and y are the coordinates of the pixel and data is the data value
             resolution (int): the resolution of the image we want to generate (the image will be a square image)
@@ -570,66 +654,73 @@
         for (x, y, z) in sparse_map:
             X.append(x)
             Y.append(y)
             Z.append(z)
         X, Y, Z = np.array(X), np.array(Y), np.array(Z)
         xi = np.linspace(0, resolution-1, resolution)
         yi = np.linspace(0, resolution-1, resolution)
-        return interpolate.griddata((X, Y), Z, (xi[None,:], yi[:,None]), method=method)
+        return interpolate.griddata((X, Y), Z, (xi[None, :], yi[:, None]), method=method)
 
     @track_time_wrapper(logger=time_tracker_console)
     def _generate_interpolation_rbf_(self, sparse_map, resolution, function='linear'):
         """A private method that uses interpolation to generate the values for the 2D space image
            The sparse map is a list of tuples (x, y, data) where x, y and data are in the range [0, 1]
-        
+
         Args:
             sparse_map (np.ndarray): a list of tuples (x, y, data) where x and y are the coordinates of the pixel and data is the data value
             resolution (int): the resolution of the image we want to generate (the image will be a square image)
             function (str, optional): Defaults to 'euclidean'.
         """
-        self.console.log("Computing the interpolated image using RBF interpolation...")
+        self.console.log(
+            "Computing the interpolated image using RBF interpolation...")
         X, Y, Z = [], [], []
         for (x, y, z) in sparse_map:
             X.append(x)
             Y.append(y)
             Z.append(z)
 
-        rbf = interpolate.Rbf(X, Y, Z, function=function) 
+        rbf = interpolate.Rbf(X, Y, Z, function=function)
         ti = np.linspace(0, 1, resolution)
         xx, yy = np.meshgrid(ti, ti)
-        # using dask to parallelize the computation of the rbf function
-        # the rbf function is applied to each pixel of the image
-        # the image is divided into chunks and each chunk is processed in parallel
-        # the result is then merged together
-        # the number of chunks is equal to the number of cores
+        
+        """
+            using dask to parallelize the computation of the rbf function
+            the rbf function is applied to each pixel of the image
+            the image is divided into chunks and each chunk is processed in parallel
+            the result is then merged together
+            the number of chunks is equal to the number of cores
+        """
         cores = 4
-        ix = da.from_array(xx, chunks=(1, cores))
-        iy = da.from_array(yy, chunks=(1, cores))
-        iz = da.map_blocks(rbf, ix, iy)
+
+        ix = da.from_array(xx, chunks=(1, cores))  # type: ignore
+        iy = da.from_array(yy, chunks=(1, cores))  # type: ignore
+        iz = da.map_blocks(rbf, ix, iy)            # type: ignore
         zz = iz.compute()
         self.console.log("Finished computing the interpolated image using RBF interpolation")
         return zz
-        
-    def generate_projection_errors(self, Xnd: np.ndarray = None, 
-                                   X2d: np.ndarray = None, 
-                                   resolution: int = None, 
-                                   use_interpolation:bool=True,
-                                   save_folder:str = None):
-        """ Calculates the projection errors of the given data.
+
+    def generate_projection_errors(self, 
+                                   Xnd: np.ndarray | None = None,
+                                   X2d: np.ndarray | None = None,
+                                   resolution: int | None = None,
+                                   use_interpolation: bool = True,
+                                   save_folder: str | None = None):
+        """ 
+        Calculates the projection errors of the given data.
 
         Args:
             Xnd (np.array): The data to be projected. The data must be in the range [0,1].
             X2d (np.array): The 2D projection of the data. The data must be in the range [0,1].
             resolution (int): The resolution of the 2D space.
             spaceNd (np.array): The nD space of the data.
             use_interpolation (bool): Whether to use interpolation to generate the projection errors or use the inverse projection. Defaults to interpolation usage
             save_folder (str): The folder path where to store the projection errors results. Defaults to None.
         Returns:
             errors (np.array): The projection errors matrix of the given data. 
-        
+
         Example:
             >>> from decision-boundary-mapper import SDBM
             >>> classifier = ...
             >>> Xnd = ...
             >>> X2d = ...
             >>> sdbm = SDBM(classifier)
             >>> errors = sdbm.get_projection_errors(Xnd, X2d)
@@ -637,109 +728,110 @@
             >>> plt.show()
             >>> ...
             >>> spaceNd = ...
             >>> errors = sdbm.get_projection_errors(Xnd, X2d, spaceNd=spaceNd, use_interpolation=False)
             >>> plt.imshow(errors)
             >>> plt.show()
         """
-        
+
         if Xnd is None:
             if self.Xnd is None:
                 self.console.error("No nD data provided and no data stored in the DBM object.")
                 raise ValueError("No nD data provided and no data stored in the DBM object.")
             Xnd = self.Xnd
         if X2d is None:
             if self.X2d is None:
                 self.console.error("No 2D data provided and no data stored in the DBM object.")
                 raise ValueError("No 2D data provided and no data stored in the DBM object.")
             X2d = self.X2d
         if resolution is None:
-            if self.resolution is None:   
+            if self.resolution is None:
                 self.console.error("The resolution of the 2D space is not set, try to call the method 'generate_boundary_map' first.")
                 raise Exception("The resolution of the 2D space is not set, try to call the method 'generate_boundary_map' first.")
             resolution = self.resolution
-        
-        assert len(X2d) == len(Xnd)    
+
+        assert len(X2d) == len(Xnd)
         X2d = X2d.reshape((X2d.shape[0], -1))
         Xnd = Xnd.reshape((Xnd.shape[0], -1))
-        
+
         assert X2d.shape[1] == 2
-        
+
         self.console.log("Calculating the projection errors of the given data, this might take a couple of minutes. Please wait...")
         if use_interpolation:
-            errors = self._generate_projection_errors_using_interpolation_(Xnd, X2d, resolution)                    
-        else:            
+            errors = self._generate_projection_errors_using_interpolation_(Xnd, X2d, resolution)
+        else:
             errors = self._generate_projection_errors_using_inverse_projection_(Xnd, X2d, resolution)
-        
+
         self.console.log("Finished computing the projection errors!")
         if save_folder is not None:
             self.console.log("Saving the projection errors results")
-            save_path = os.path.join(save_folder, "projection_errors_interpolated.npy") if use_interpolation else os.path.join(save_folder, "projection_errors_inv_proj.npy")
+            save_path = os.path.join(save_folder, PROJECTION_ERRORS_INTERPOLATED_FILE) if use_interpolation else os.path.join(save_folder, PROJECTION_ERRORS_INVERSE_PROJECTION_FILE)
             with open(save_path, "wb") as f:
                 np.save(f, errors)
             self.console.log("Saved projection errors results!")
-            
+
         return errors
-    
-    @track_time_wrapper(logger=time_tracker_console)    
-    def _generate_projection_errors_using_interpolation_(self, Xnd, X2d, resolution):  
-        errors = np.zeros((resolution,resolution))  
-        K = 10 # Number of nearest neighbors to consider when computing the errors
+
+    @track_time_wrapper(logger=time_tracker_console)
+    def _generate_projection_errors_using_interpolation_(self, Xnd, X2d, resolution):
+        errors = np.zeros((resolution, resolution))
+        K = PROJECTION_ERRORS_NEIGHBORS_NUMBER  # Number of nearest neighbors to consider when computing the errors
         metric = "euclidean"
-        
+
         self.console.log("Computing the 2D tree")
         tree = KDTree(X2d, metric=metric)
         self.console.log("Finished computing the 2D tree")
         self.console.log("Computing the 2D tree indices")
         indices_embedded = tree.query(X2d, k=len(X2d), return_distance=False)
         # Drop the actual point itself
         indices_embedded = indices_embedded[:, 1:]
         self.console.log("Finished computing the 2D tree indices")
-        
+
         self.console.log("Calculating the nD distance indices")
         indices_source = get_nd_indices_parallel(Xnd, metric=euclidean)
         self.console.log("Finished computing the nD distance indices")
-        
+
         sparse_map = []
         for k in range(len(X2d)):
             x, y = X2d[k]
-            sparse_map.append( (x, y, get_proj_error_parallel(indices_source[k], indices_embedded[k], k=K)))
-            
+            sparse_map.append((x, y, get_proj_error_parallel(indices_source[k], indices_embedded[k], k=K)))
+
         errors = self._generate_interpolation_rbf_(sparse_map, resolution, function='linear').T
-        
+
         # resize the errors in range [0,1]
         errors = (errors - errors.min()) / (errors.max() - errors.min())
-        
+
         return errors
-    
+
     @track_time_wrapper(logger=time_tracker_console)
-    def _generate_projection_errors_using_inverse_projection_(self, 
-                                                            Xnd: np.ndarray = None, 
-                                                            X2d: np.ndarray = None,                                                             
-                                                            resolution: int = 256):        
-        
-        K = 10 # Number of nearest neighbors to consider when computing the errors       
-        space2d = np.array([(i / resolution, j / resolution) for i in range(resolution) for j in range(resolution)]) # generate the 2D flatten space
-        
+    def _generate_projection_errors_using_inverse_projection_(self,
+                                                              Xnd: np.ndarray,
+                                                              X2d: np.ndarray,
+                                                              resolution: int = 256):
+
+        K = PROJECTION_ERRORS_NEIGHBORS_NUMBER  # Number of nearest neighbors to consider when computing the errors
+        space2d = np.array([(i / resolution, j / resolution) for i in range(resolution) for j in range(resolution)])  # generate the 2D flatten space
+
         errors = np.array([])
         # split space2d into chunks
-        chunks_number = resolution * resolution // 10000 + 1 # split the space into chunks of 10000 points max
+        # split the space into chunks of 10000 points max
+        chunks_number = resolution * resolution // DBM_DEFAULT_CHUNK_SIZE + 1
         self.console.log(f"Splitting the 2D space into {chunks_number} chunks")
         space2d_chunks = np.array_split(space2d, chunks_number)
-        
+
         chunk_index = 0
         for space2d_chunk in space2d_chunks:
             chunk_index += 1
             self.console.log(f"Computing the projection errors for chunk ({chunk_index}/{chunks_number}) of size: {(len(space2d_chunk))}")
-            spaceNd_chunk = self.neural_network.decode(space2d_chunk) # decode the 2D space to nD space        
-            spaceNd_chunk = spaceNd_chunk.reshape((spaceNd_chunk.shape[0], -1)) # flatten the space   
-                    
+            spaceNd_chunk = self.neural_network.decode(space2d_chunk)  # decode the 2D space to nD space
+            spaceNd_chunk = spaceNd_chunk.reshape((spaceNd_chunk.shape[0], -1))  # flatten the space
+
             with ProgressBar(total=len(space2d_chunk)) as progress:
                 errors_chunk = get_projection_errors_using_inverse_projection(Xnd=Xnd, X2d=X2d, spaceNd=spaceNd_chunk, space2d=space2d_chunk, k=K, progress=progress)
-        
+
             errors = np.concatenate((errors, errors_chunk))
-            
+
         # resize the errors in range [0,1]
-        errors = (errors - errors.min()) / (errors.max() - errors.min())        
-        errors = errors.reshape((resolution, resolution))        
-        
-        return errors
+        errors = (errors - errors.min()) / (errors.max() - errors.min())
+        errors = errors.reshape((resolution, resolution))
+
+        return errors
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/NNinterface.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractNN.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from math import sqrt
@@ -17,138 +17,139 @@
 import os
 import numpy as np
 import json
 import matplotlib.pyplot as plt
 
 from ..Logger import Logger, LoggerInterface
 
+TRAINING_HISTORY_FILE_NAME = "history.json"
 
-class NNinterface:
+class AbstractNN:
     """ 
-    Defines the interface for the neural networks used by the Decision Boundary Mapper.
-    
+    Defines an abstract class for the neural networks used by the Decision Boundary Mapper.
+
+    Public methods:
+        load \n
+        save \n
+        show_predictions \n
+
     Methods to be implemented by the classes that inherit from this class.
-    fit: Fits the model to the specified data.
-    encode: Encodes the input data. (optional)
+        encode: Encodes the input data.
     """
-    
-    def __init__(self, 
-                 folder_path: str,                 
-                 nn_name: str = "invNN", 
-                 logger: LoggerInterface = None):
-        """ Initializes the NN interface.
+
+    def __init__(self,
+                 folder_path: str,
+                 nn_name: str,
+                 logger: LoggerInterface | None = None):
+        """ 
+        Initializes an NN object.
 
         Args:
             folder_path (str): the folder path where the model will be saved/loaded.
-            classifier (tf.keras.model): The classifier model. Defaults to None.
-            nn_name (str, optional): Name of the neural network that uses the classifier. Defaults to "invNN".
+            nn_name (str): Name of the neural network that uses the classifier.
             logger (LoggerInterface, optional): Defaults to console logging.
 
         Raises:
             Exception: If the classifier is not provided.
         """
         if logger is not None:
             self.console = logger
         else:
             self.console = Logger(name=nn_name)
-                
+
         self.save_folder_path = folder_path
         self.nn_name = nn_name
         self.neural_network = None
-        
+
         try:
             self.load()
         except Exception as e:
             self.console.error("Error loading the model: {}".format(e))
             self.console.warn("The model will be built and trained from scratch.")
-            
-    def fit(self):
-        """ Fits the model to the specified data."""
-        raise NotImplementedError("The fit method is not implemented.")
-    
-    
+
     def load(self):
         """
             Loads an auto encoder from the specified folder path. With the .h5 extension.
             Args:
                 folder_path (str): The path to the folder where the model is saved.
         """
         try:
             self.neural_network = tf.keras.models.load_model(os.path.join(self.save_folder_path, self.nn_name), compile=False)
             self.console.log("NN loaded successfully")
         except Exception as e:
-            self.console.log(f"NN not found. Please check the path folder {self.save_folder_path} and make sure the model is saved there")        
+            self.console.log(
+                f"NN not found. Please check the path folder {self.save_folder_path} and make sure the model is saved there")
             raise e
-    
-    def save(self, history = None):
+
+    def save(self, history=None):
         """
             Saves the model to the specified folder path. With the .tf extension.
-        """       
-        folder_path = self.save_folder_path 
+        """
+        folder_path = self.save_folder_path
         if not os.path.exists(folder_path):
             os.makedirs(folder_path)
-            
-        self.neural_network.save(os.path.join(folder_path, self.neural_network.name), save_format="tf")
+
+        path = os.path.join(folder_path, self.neural_network.name)  # type: ignore
+        self.neural_network.save(path, save_format="tf")            # type: ignore
         self.console.log(f"Model saved to {folder_path}")
-        
+
         if history is None:
             return
-        
-        with open(os.path.join(folder_path, "history.json"), "w") as f:
+
+        with open(os.path.join(folder_path, TRAINING_HISTORY_FILE_NAME), "w") as f:
             f.write(json.dumps(history.history))
             self.console.log(f"History saved to {folder_path}")
-        
-        
-    def show_predictions(self, dataNd: np.ndarray, labels: np.ndarray, data2d:np.ndarray = None, n_samples:int = 16):
+
+    def show_predictions(self, dataNd: np.ndarray, labels: np.ndarray, data2d: np.ndarray | None = None, n_samples: int = 16):
         """ Shows the predictions of the model. By taking first n_samples data points and comparing them to the actual labels.
 
         Args:
             dataNd (np.ndarray): N-dimensional data points.
             data2d (np.ndarray, optional): 2-dimensional data points. Defaults to None.
             labels (np.ndarray): Actual labels of the data points
             n_samples (int, optional): Number of samples to show. Defaults to 16.
         """
         if data2d is None:
             data2d = self.encode(dataNd)
-        
+
         decoded, predicted = self.decode(data2d)
         predicted_labels = np.argmax(predicted, axis=1)
-        
+
         plt.figure(figsize=(20, 10))
         m = int(sqrt(n_samples))
         n = m * m
-        
-        for i in range(1,2*n,2):
+
+        for i in range(1, 2*n, 2):
             plt.subplot(m, 2*m, i)
             plt.imshow(dataNd[i], cmap='gray')
-            plt.title(f"Actual: {labels[i]}", color='green' if predicted_labels[i] == labels[i] else 'red', fontsize=12)
+            plt.title(f"Actual: {labels[i]}", color='green' if predicted_labels[i]== labels[i] else 'red', fontsize=12)
             plt.axis('off')
             plt.subplot(m, 2*m, i+1)
             plt.imshow(decoded[i], cmap='gray')
             plt.title(f"Predicted: {predicted_labels[i]}", color='green' if predicted_labels[i] == labels[i] else 'red', fontsize=12)
             plt.axis('off')
-        
+
         plt.show()
-    
-    def decode(self, data: np.ndarray, verbose: int = 0):
+
+    def decode(self, data: np.ndarray, verbose: int = 0) -> np.ndarray:
         """ Decodes the data points.
 
         Args:
             data (np.ndarray): The data points to decode.
             verbose (int, optional): Verbosity mode. Defaults to 0.
-            
+
         Returns:
             Xnd, labels_predictions: The decoded data points and the predictions of the classifier.
         """
-        return self.neural_network.predict(data, verbose=verbose)
-    
-    def encode(self, data: np.ndarray, verbose: int = 0):
+        return self.neural_network.predict(data, verbose=verbose)  # type: ignore
+
+    def encode(self, data: np.ndarray, verbose: int = 0) -> np.ndarray:
         """ Encodes the data points.
 
         Args:
             data (np.ndarray): The data points to encode.
             verbose (int, optional): Verbosity mode. Defaults to 0.
 
         Returns:
             np.ndarray: The encoded 2D data points.
         """
-        return NotImplementedError("The encode method is not implemented.")
+        raise NotImplementedError("The encode method is not implemented.")
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SSNP.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,168 +1,176 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 import tensorflow as tf
 import numpy as np
 
-from ..NNinterface import NNinterface
+from ..AbstractNN import AbstractNN
 from ...Logger import LoggerInterface, LoggerModel
 
-DEFAULT_MODEL_PATH = os.path.join("tmp", "SDBM")
 DECODER_NAME = "decoder"
 ENCODER_NAME = "encoder"
-AUTOENCODER_NAME = "autoencoder"
+SSNP_NAME = "ssnp"
 CLASSIFIER_NAME = "classifier"
 
 DECODER_LOSS = "mean_squared_error"
 CLASSIFIER_LOSS = "sparse_categorical_crossentropy"
 DECODER_LOSS_WEIGHT = 1.0
 CLASSIFIER_LOSS_WEIGHT = 0.125
 
-class Autoencoder(NNinterface):
-    def __init__(self,                 
-                 folder_path:str = DEFAULT_MODEL_PATH, 
-                 logger:LoggerInterface = None):
-        """
-            Creates an autoencoder model.
-            Classifier: The classifier part of the autoencoder.
-            
+
+class SSNP(AbstractNN):
+    def __init__(self,
+                 folder_path: str,
+                 logger: LoggerInterface | None = None):
+        """
+            Creates an SSNP model.
+
             Args:
                 folder_path: The path to the folder where the model will be saved/loaded.
                 logger: The logger used to log the model's progress.
-                classifier: The classifier part of the autoencoder.
         """
-        super().__init__(folder_path=folder_path, logger=logger, nn_name=AUTOENCODER_NAME)                
-    
-    def __build__(self, input_shape:tuple = (28, 28), num_classes:int=10, show_summary:bool = False):
+        super().__init__(folder_path=folder_path, logger=logger, nn_name=SSNP_NAME)
+
+    def __build__(self, input_shape: tuple = (28, 28), num_classes: int = 10, show_summary: bool = False):
         """
             Assembles the autoencoder model and compiles it. 
-            
+
             Args:
                 input_shape: The input and output shape of the autoencoder.
                 show_summary: If True, the model summary will be printed.
         """
-        
+
+        output_size = 1
+        for i in range(len(input_shape)):
+            output_size *= input_shape[i]
+
+
         encoder = tf.keras.models.Sequential([
             tf.keras.layers.Flatten(),
-            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform', kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
-            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(2, activation='sigmoid', bias_initializer=tf.keras.initializers.Constant(0.01)),            
+            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform',
+                                  kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
+            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(
+                2, activation='sigmoid', bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
         ], name=ENCODER_NAME)
 
         decoder = tf.keras.models.Sequential([
-            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform', kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
-            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform', bias_initializer=tf.keras.initializers.Constant(0.01)),
-            tf.keras.layers.Dense(input_shape[0] * input_shape[1], activation='sigmoid'),
+            tf.keras.layers.Dense(32, activation='relu', kernel_initializer='he_uniform',
+                                  kernel_regularizer=tf.keras.regularizers.l2(0.0002)),
+            tf.keras.layers.Dense(64, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(128, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(512, activation='relu', kernel_initializer='he_uniform',
+                                  bias_initializer=tf.keras.initializers.Constant(0.01)),  # type: ignore
+            tf.keras.layers.Dense(output_size, activation='sigmoid'),
             tf.keras.layers.Reshape(input_shape)
-        ], name=DECODER_NAME)       
-        
+        ], name=DECODER_NAME)
+
         classifier = tf.keras.models.Sequential([
             tf.keras.layers.Flatten(),
             tf.keras.layers.Dense(num_classes, activation=tf.nn.softmax)
-        ], name=CLASSIFIER_NAME) 
-        
-        input_layer = tf.keras.Input(shape=input_shape, name="input")           
-        
+        ], name=CLASSIFIER_NAME)
+
+        input_layer = tf.keras.Input(shape=input_shape, name="input")
+
         encoder_output = encoder(input_layer)
         decoder_output = decoder(encoder_output)
         classifier_output = classifier(decoder_output)
-        
+
         self.neural_network = tf.keras.models.Model(inputs=input_layer,
                                                     outputs=[decoder_output, classifier_output],
-                                                    name=AUTOENCODER_NAME)
-        
-        self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(), 
-                                    loss = {DECODER_NAME:DECODER_LOSS,
-                                            CLASSIFIER_NAME:CLASSIFIER_LOSS},
-                                    loss_weights = {DECODER_NAME:DECODER_LOSS_WEIGHT,
-                                                    CLASSIFIER_NAME:CLASSIFIER_LOSS_WEIGHT},
-                                    metrics = {DECODER_NAME: "accuracy", CLASSIFIER_NAME: "accuracy"})
-        
+                                                    name=SSNP_NAME)
+
+        self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(),
+                                    loss={DECODER_NAME: DECODER_LOSS,
+                                          CLASSIFIER_NAME: CLASSIFIER_LOSS},
+                                    loss_weights={DECODER_NAME: DECODER_LOSS_WEIGHT,
+                                                  CLASSIFIER_NAME: CLASSIFIER_LOSS_WEIGHT},
+                                    metrics={DECODER_NAME: "accuracy", CLASSIFIER_NAME: "accuracy"})
+
         if show_summary:
             self.neural_network.summary()
-        
-        
-    def fit(self, X: np.ndarray, Y: np.ndarray,             
-            epochs:int = 10, batch_size:int = 128):
+
+    def fit(self, X: np.ndarray, Y: np.ndarray,
+            epochs: int = 10, batch_size: int = 128):
         """ Fits the model to the specified data.
 
         Args:
-            x_train (np.ndarray): Train input values
-            y_train (np.ndarray): Train target values
-            x_test (np.ndarray): Test input values
-            y_test (np.ndarray): Test target values
+            X (np.ndarray): Train input values
+            Y (np.ndarray): Train target values
             epochs (int, optional): The number of epochs. Defaults to 10.
             batch_size (int, optional): Data points used for one batch. Defaults to 128.
         """
         if self.neural_network is not None:
             self.console.log("Model already loaded. Skipping build.")
             self.encoder = self.neural_network.get_layer(ENCODER_NAME)
             self.decoder = self.neural_network.get_layer(DECODER_NAME)
             return
-        
-        
+
         self.console.log("Building model according to the data shape.")
         num_classes = len(np.unique(Y))
         self.__build__(input_shape=X.shape[1:], num_classes=num_classes, show_summary=True)
-            
-        stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', min_delta=0.00001, mode='min', patience=20, restore_best_weights=True)
-        logger_callback = LoggerModel(name=AUTOENCODER_NAME, show_init=False, epochs=epochs)
+
+        stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode='min', patience=20, restore_best_weights=True)
+        logger_callback = LoggerModel(name=SSNP_NAME, show_init=False, epochs=epochs)
 
         self.console.log("Fitting model...")
-        
-        history = self.neural_network.fit(X, [X, Y], 
-                            epochs=epochs, 
-                            batch_size=batch_size, 
-                            shuffle=True,
-                            validation_split=0.2,
-                            callbacks=[stopping_callback, logger_callback],
-                            verbose=0)
-        
+
+        history = self.neural_network.fit(X, [X, Y],
+                                          epochs=epochs,
+                                          batch_size=batch_size,
+                                          shuffle=True,
+                                          validation_split=0.2,
+                                          callbacks=[stopping_callback, logger_callback],
+                                          verbose=0)
+
         self.console.log("Model fitted!")
-        self.save(history)    
+        self.save(history)
         self.encoder = self.neural_network.get_layer(ENCODER_NAME)
         self.decoder = self.neural_network.get_layer(DECODER_NAME)
-            
-        #self.show_predictions(dataNd=x_test, labels=y_test)    
-           
-    def encode(self, data:np.ndarray, verbose:int = 0):
-        """ Encodes the data using the encoder part of the autoencoder.
+
+        # self.show_predictions(dataNd=x_test, labels=y_test)
+
+    def encode(self, data: np.ndarray, verbose: int = 0):
+        """ 
+        Encodes the data using the encoder part of the autoencoder.
 
         Args:
             data (np.ndarray): The data to encode.
             verbose (int, optional): Verbosity level. Defaults to 0.
 
         Returns:
             np.ndarray: The encoded 2D data.
         """
         return self.encoder.predict(data, verbose=verbose)
-        
-    def decode(self, data:np.ndarray, verbose:int = 0):
-        """ Decodes the data using the decoder part of the autoencoder.
+
+    def decode(self, data: np.ndarray, verbose: int = 0):
+        """ 
+        sDecodes the data using the decoder part of the autoencoder.
 
         Args:
             data (np.ndarray): The data to decode.
             verbose (int, optional): Verbosity level. Defaults to 0.
 
         Returns:
             np.ndarray: The decoded nD data.
         """
         xNd = self.decoder.predict(data, verbose=verbose)
         return xNd
-
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/DBM/SDBM/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .SDBM import SDBM
+from .GUI import GUI
+from .DBMPlotterGUI import DBMPlotterGUI
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/GUI.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterController.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,560 +9,633 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from shutil import rmtree
-import matplotlib.pyplot as plt
-import PySimpleGUI as sg
 import numpy as np
-from PIL import Image, ImageTk
-import tensorflow as tf
-from tensorflow.keras.utils import plot_model
-
-from .DBMPlotterGUI import DBMPlotterGUI
-from ..Logger import LoggerGUI, Logger
-from ..DBM import SDBM, DBM
-from ..utils import import_csv_dataset, import_mnist_dataset, import_cifar10_dataset, import_fashion_mnist_dataset
-
-sg.theme('DarkBlue1')
-TITLE = "Classifiers visualization tool"
-WINDOW_SIZE = (1150, 700)
-BLACK_COLOR = "#252526"
-BUTTON_PRIMARY_COLOR = "#007acc"
-WHITE_COLOR = "#ffffff"
-RIGHTS_MESSAGE = "© 2023 Cristian Grosu. All rights reserved."
-RIGHTS_MESSAGE_2 = "Made by Cristian Grosu for Utrecht University Master Thesis in 2023"
-APP_ICON_PATH = os.path.join(os.path.dirname(__file__), "assets", "main_icon.png")
-
-DEFAULT_DBM_IMAGE_PATH = os.path.join(os.getcwd(), "results", "MNIST", "2D_boundary_mapping.png") # unused
-TMP_FOLDER = os.path.join(os.getcwd(), "tmp")
-
-SAMPLES_LIMIT = 5000 # Limit the number of samples to be loaded from the dataset
-
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2' # Disable tensorflow logs
-
-"""
-0 = all messages are logged (default behavior)
-1 = INFO messages are not printed
-2 = INFO and WARNING messages are not printed
-3 = INFO, WARNING, and ERROR messages are not printed
-"""
-
-DBM_TECHNIQUES = {
-    "Autoencoder": SDBM,
-    "Inverse Projection": DBM,
-}
-
-PROJECTION_TECHNIQUES = [
-    "t-SNE",
-    "UMAP",
-    "PCA",
-]
-
-class GUI:
-    def __init__(self):
-        self.create_tmp_folder()
-        self.window = self.build()
-        self.logger = Logger(name = "GUI")
-            
-        # --------------- DBM ---------------
-        self.dbm_plotter_gui = None
-        self.dbm_logger = LoggerGUI(name = "DBM logger", output = self.window["-LOGGER-"], update_callback = self.window.refresh)        
-        
-        # --------------- Data set ----------
-        self.dataset_name = "Dataset"
-        self.X_train, self.Y_train = None, None
-        self.X_test, self.Y_test = None, None
-        
-        # --------------- Classifier --------
-        self.classifier = None
-    
-    def create_tmp_folder(self):
-        if not os.path.exists(TMP_FOLDER):
-            os.makedirs(TMP_FOLDER)
-    
-    def remove_tmp_folder(self):
-        if os.path.exists(TMP_FOLDER):
-            rmtree(TMP_FOLDER)
-            
-    def build(self):
-        window = sg.Window(TITLE, 
-                           layout=self._get_layout(), 
-                           size=WINDOW_SIZE,  
-                           icon=APP_ICON_PATH,                          
-                           resizable=False,
-                           )
-        window.finalize()
-        return window
+import json
+from math import sqrt
+from datetime import datetime
+import shutil
+from matplotlib.patches import Patch, Circle
+from matplotlib.offsetbox import OffsetImage, AnnotationBbox, TextArea
+
+from .. import Logger
+from ..utils import TRAIN_DATA_POINT_MARKER, TEST_DATA_POINT_MARKER, TRAIN_2D_FILE_NAME, TEST_2D_FILE_NAME, INVERSE_PROJECTION_ERRORS_FILE, PROJECTION_ERRORS_INTERPOLATED_FILE, PROJECTION_ERRORS_INVERSE_PROJECTION_FILE
+
+CLASSIFIER_PERFORMANCE_HISTORY_FILE = "classifier_performance.log"
+CLASSIFIER_REFIT_FOLDER = "refit_classifier"
+CLASSIFIER_STACKED_FOLDER = "stacked_classifier"
+CLASSIFIER_STACKED_LABELS_FILE = "classifier_old_labels.npy"
+CLASSIFIER_STACKED_LABELS_CHANGES_FILE = "classifier_old_labels_changes.npy"
+CLASSIFIER_STACKED_BOUNDARY_MAP_FILE = "classifier_old_boundary_map.npy"
+CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE = "classifier_old_boundary_map_confidence.npy"
+
+LABELS_CHANGES_FILE = "label_changes.json"
+
+EPOCHS_FOR_REFIT = 2
+
+class DBMPlotterController:
+    def __init__(self,
+                logger,
+                dbm_model,
+                img, img_confidence,
+                X_train, Y_train,
+                X_test, Y_test,
+                X_train_2d, X_test_2d,
+                encoded_train, encoded_test,
+                save_folder,
+                projection_technique,
+                ):
         
-    def start(self):
-        while True:
-            event, values = self.window.read()
-            
-            if event == "Exit" or event == sg.WIN_CLOSED:                
-                break
-            
-            self.handle_event(event, values)
-                
-        self.stop()
-    
-    def stop(self):
-        #self.logger.log("Removing tmp folder...")
-        #self.remove_tmp_folder()
-        self.logger.log("Closing the application...")
-        self.window.close()
+        if logger is None:
+            self.console = Logger(name="DBMPlotterController")
+        else:
+            self.console = logger
             
-    def _get_layout(self):                
-        data_files_list_column = [
-            [
-                sg.Text(text = "Data Folder"),
-                sg.In(enable_events=True, key="-FOLDER-", background_color=WHITE_COLOR, text_color=BLACK_COLOR, expand_x=True),
-                sg.FolderBrowse(button_text="Browse folder", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), initial_folder=os.getcwd()),
-            ],
-            [
-               sg.Text("Choose the data file from the list: ", expand_x=True),
-            ],
-            [   
-               sg.Text(key="-TOUT-", expand_x=True),            
-            ],
-            [
-                sg.Listbox(
-                    values=[], enable_events=True, key="-FILE LIST-", background_color=WHITE_COLOR, text_color=BLACK_COLOR, expand_x=True, expand_y=True
-                )
-            ],
-            [
-                sg.Button("Upload train data for DBM", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, key = "-UPLOAD TRAIN DATA BTN-"),
-                sg.Button("Upload test data for DBM", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, key = "-UPLOAD TEST DATA BTN-"),
-            ],
-            [   
-               sg.Text("Training data file: ", key="-TRAIN DATA FILE-",  expand_x=True),            
-            ],
-            [   
-               sg.Text("Training data shape: ", key="-TRAIN DATA SHAPE-", expand_x=True),            
-            ],
-            [   
-               sg.Text("Testing data file: ", key="-TEST DATA FILE-", expand_x=True),            
-            ],
-            [   
-               sg.Text("Testing data shape: ", key="-TEST DATA SHAPE-", expand_x=True),            
-            ],
-            [
-                sg.Button("Upload MNIST Data set", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, key = "-UPLOAD MNIST DATA BTN-"),
-            ],
-            [
-                sg.Button("Upload FASHION MNIST Data set", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, key = "-UPLOAD FASHION MNIST DATA BTN-"),
-            ],
-            [
-                sg.Button("Upload CIFAR10 Data set", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, key = "-UPLOAD CIFAR10 DATA BTN-"),
-            ],
-            [
-                sg.Text(text = "Classifier Folder"),
-                sg.In(enable_events=True, key="-CLASSIFIER FOLDER-", background_color=WHITE_COLOR, text_color=BLACK_COLOR, expand_x=True),
-                sg.FolderBrowse(button_text="Browse folder", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), initial_folder=os.getcwd()),
-            ],
-            [
-               sg.Text("Choose the classifier file(.h5) or folder from the list: ", expand_x=True),
-            ],
-            [   
-               sg.Text(key="-CLASSIFIER PATH TOUT-", expand_x=True),            
-            ],
-            [
-                sg.Listbox(
-                    values=[], enable_events=True, key="-CLASSIFIER FILE LIST-", background_color=WHITE_COLOR, text_color=BLACK_COLOR, expand_x=True, expand_y=True
-                )
-            ],
-            [
-                sg.Button("Upload classifier", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, visible=True, key = "-UPLOAD CLASSIFIER-"),
-            ],                                                
-            [
-                sg.Text("", expand_x=True)    
-            ],
-            [
-                sg.Text(RIGHTS_MESSAGE, expand_x=True),
-            ],
-            [
-                sg.Text(RIGHTS_MESSAGE_2, expand_x=True),
-            ]
+        # folder where to save the changes made to the data by the user
+        self.save_folder = save_folder
+        # projection technique used to generate the DBM
+        self.projection_technique = projection_technique
+        if self.projection_technique is not None:
+            self.save_folder = os.path.join(self.save_folder, self.projection_technique)
+        
+        self.inverse_projection_errors = None
+        self.projection_errors = None
+        self.positions_of_labels_changes = ([], [], [])
+
+        self.dbm_model = dbm_model
+        self.img = img
+        self.img_confidence = img_confidence
+        self.X_train = X_train
+        self.Y_train = Y_train
+        self.X_test = X_test
+        self.Y_test = Y_test
+        self.X_train_2d = X_train_2d
+        self.X_test_2d = X_test_2d
+        self.encoded_train = encoded_train
+        self.encoded_test = encoded_test
+        self.initialize()
+        
+    def initialize(self):
+        self.train_mapper, self.test_mapper = self.generate_encoded_mapping()
+        # --------------------- Others ------------------------------
+        self.expert_updates_labels_mapper = {}
+        self.motion_event_cid = None
+        self.click_event_cid = None
+        self.key_event_cid = None
+        self.release_event_cid = None
+        self.current_selected_point = None
+        self.current_selected_point_assigned_label = None
+        self.update_labels_by_circle_select = True
+        self.update_labels_circle = None
+    
+    def clear_resources(self):
+        files_to_delete = [
+            CLASSIFIER_PERFORMANCE_HISTORY_FILE,
+            LABELS_CHANGES_FILE,
+            CLASSIFIER_STACKED_BOUNDARY_MAP_FILE,
+            CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE,
+            CLASSIFIER_STACKED_LABELS_FILE,
+            CLASSIFIER_STACKED_LABELS_CHANGES_FILE
         ]
-        
-        results_column = [
-            [
-                sg.Text("Which dbm technique would you like to use?", size=(45,1)),
-                sg.Combo(
-                    values=list(DBM_TECHNIQUES.keys()),
-                    default_value=list(DBM_TECHNIQUES.keys())[0],
-                    expand_x=True,
-                    key="-DBM TECHNIQUE-",
-                    enable_events=True,
-                    background_color=WHITE_COLOR, text_color=BLACK_COLOR,
-                ),
-            ],
-            [
-                sg.Text("Which Projection technique would you like to use?", size=(45,1), key="-PROJECTION TECHNIQUE TEXT-", visible=False),
-                sg.Combo(
-                    values = PROJECTION_TECHNIQUES,
-                    default_value = PROJECTION_TECHNIQUES[0],
-                    expand_x=True,
-                    key="-PROJECTION TECHNIQUE-",
-                    enable_events=True,
-                    visible=False,
-                    background_color=WHITE_COLOR, text_color=BLACK_COLOR,
-                ),
-            ],           
-            [
-                sg.Text("Show Decision Boundary Mapper NN history: ", expand_x=True, key="-DBM HISTORY TEXT-", visible=True),
-                sg.Checkbox("", default=False,  key="-DBM HISTORY CHECKBOX-", visible=True),
-            ],
-            #[
-            #    sg.Text("Image resolution of the Decision Boundary Mapper: ", size=(45,1), expand_x=True, key="-DBM IMAGE RESOLUTION TEXT-", visible=True),
-            #    sg.InputText("256", key="-DBM IMAGE RESOLUTION INPUT-", visible=True, background_color=WHITE_COLOR, text_color=BLACK_COLOR),
-            #],
-            [
-                sg.Button("Show the Decision Boundary Mapping", button_color=(WHITE_COLOR, BUTTON_PRIMARY_COLOR), expand_x=True, visible=False, key = "-DBM BTN-"),
-            ],
-            # ---------------------------------------------------------------------------------------------------                        
-            [sg.Text("Decision boundary map: ", visible=False, expand_x=True, key="-DBM TEXT-", justification='center')],
-            [sg.Text("Loading... ",  visible=False, expand_x=True, key="-DBM IMAGE LOADING-", justification='center')],
-            [sg.Image(key="-DBM IMAGE-", visible=False, expand_x=True, expand_y=True, enable_events=True)],                                                              
-            [
-                sg.HSeparator(),
-            ],
-            [
-                sg.Column([
-                    [sg.Text("Logger: ")],
-                    [sg.Multiline("",expand_x=True, expand_y=True, key="-LOGGER-", background_color=WHITE_COLOR, text_color=BLACK_COLOR, auto_size_text=True)],   
-                ], expand_x=True, expand_y=True),    
-            ]
-        ]
-        
-        layout = [
-            [
-                sg.Column(data_files_list_column, expand_x=True, expand_y=True),   
-                sg.VSeparator(),             
-                sg.Column(results_column, expand_x=True, expand_y=True),
-            ],
+
+        for file in files_to_delete:
+            file = os.path.join(self.save_folder, file)
+            if os.path.exists(file):
+                os.remove(file)
+
+        folders_to_delete = [
+            CLASSIFIER_STACKED_FOLDER
         ]
 
-        return layout
+        for folder in folders_to_delete:
+            folder = os.path.join(self.save_folder, folder)
+            if os.path.exists(folder):
+                shutil.rmtree(folder)
+
+    def build_2D_image(self, colors_mapper, class_name_mapper=lambda x: str(x)):
+        """Combines the img and the img_confidence into a single image.
+
+        Args:
+            img (np.ndarray): Label image.
+            img_confidence (np.ndarray): Confidence image.
+            colors_mapper (dict): Mapper of labels to colors.
+            class_name_mapper (function, optional): Describes how to map the data labels. Defaults to lambdax:str(x).
+            
+        Returns:
+            np.ndarray: The combined image.
+            patches: The legend patches.
+        """
+        img = self.img
+        color_img = np.zeros((img.shape[0], img.shape[1], 3))
+
+        for i, j in np.ndindex(img.shape):
+            color_img[i][j] = colors_mapper[img[i][j]]
+        values = np.unique(img)
+
+        patches = []
+        for value in values:
+            color = colors_mapper[value]
+            if value == TRAIN_DATA_POINT_MARKER:
+                label = "Original train data"
+            elif value == TEST_DATA_POINT_MARKER:
+                label = "Original test data"
+            else:
+                label = f"Value region: {class_name_mapper(value)}"
 
-    def handle_event(self, event, values):        
-        # Folder name was filled in, make a list of files in the folder
-        EVENTS = {
-            "-FOLDER-": self.handle_select_folder_event,
-            "-CLASSIFIER FOLDER-": self.handle_select_classifier_folder_event,
-            "-FILE LIST-": self.handle_file_list_event,
-            "-CLASSIFIER FILE LIST-": self.handle_classifier_file_list_event,
-            "-DBM TECHNIQUE-": self.handle_dbm_technique_event,
-            "-DBM BTN-": self.handle_get_decision_boundary_mapping_event,
-            "-DBM IMAGE-": self.handle_dbm_image_event,
-            "-PROJECTION TECHNIQUE-": self.handle_projection_technique_event,
-            "-UPLOAD TRAIN DATA BTN-": self.handle_upload_train_data_event,
-            "-UPLOAD TEST DATA BTN-": self.handle_upload_test_data_event,
-            "-UPLOAD MNIST DATA BTN-": self.handle_upload_mnist_data_event,
-            "-UPLOAD FASHION MNIST DATA BTN-": self.handle_upload_fashion_mnist_data_event,
-            "-UPLOAD CIFAR10 DATA BTN-": self.handle_upload_cifar10_data_event,
-            "-UPLOAD CLASSIFIER-": self.handle_upload_classifier_event,
-        }
-        
-        EVENTS[event](event, values)
+            patches.append(Patch(color=color, label=label))
 
-    def switch_visibility(self, elements, visible):
-        for x in elements:
-            self.window[x].update(visible=visible)            
-        self.window.refresh()
-
-    def handle_select_classifier_folder_event(self, event, values):
-        folder = values["-CLASSIFIER FOLDER-"]
-        try:
-            # Get list of files in folder
-            file_list = os.listdir(folder)
-        except:
-            file_list = []
-        
-        
-        fnames = [ f for f in file_list
-                   if (os.path.isfile(os.path.join(folder, f)) and (f.lower().endswith((".h5")))) or os.path.isdir(os.path.join(folder, f)) ]                
-            
-        self.window["-CLASSIFIER FILE LIST-"].update(fnames)
-    
-    def handle_select_folder_event(self, event, values):
-        folder = values["-FOLDER-"]
-        try:
-            # Get list of files in folder
-            file_list = os.listdir(folder)
-        except:
-            file_list = []
-
-        fnames = [ f for f in file_list
-                   if os.path.isfile(os.path.join(folder, f)) and (f.lower().endswith((".csv")) or f.lower().endswith((".txt")))
-                ]
-        self.window["-FILE LIST-"].update(fnames)
-    
-    def handle_file_list_event(self, event, values):
-        try:
-            filename = os.path.join(values["-FOLDER-"], values["-FILE LIST-"][0])
-            self.window["-TOUT-"].update(filename)
-        except Exception as e:
-            self.dbm_logger.error("Error while loading data file" + str(e))
-    
-    def handle_classifier_file_list_event(self, event, values):
-        try:
-            filename = os.path.join(values["-CLASSIFIER FOLDER-"], values["-CLASSIFIER FILE LIST-"][0])
-            self.window["-CLASSIFIER PATH TOUT-"].update(filename)
-        except Exception as e:
-                self.logger.error("Error while loading data file" + str(e))
-                
-    def handle_upload_classifier_event(self, event, values):       
-        try:
-            fname = os.path.join(values["-CLASSIFIER FOLDER-"], values["-CLASSIFIER FILE LIST-"][0])
-            self.classifier = tf.keras.models.load_model(fname)            
-            self.window["-CLASSIFIER PATH TOUT-"].update(fname)
-            self.logger.log("Classifier loaded successfully")
-            self.dbm_logger.log("Classifier loaded successfully")
-            if self.X_train is not None and self.Y_train is not None and self.X_test is not None and self.Y_test is not None:
-                self.switch_visibility(["-DBM BTN-"], True)
-        except Exception as e:
-            self.logger.error("Error while loading classifier" + str(e))
-        
-    def handle_upload_train_data_event(self, event, values):
-        try:
-            filename = os.path.join(
-                values["-FOLDER-"], values["-FILE LIST-"][0]
-            )
-            self.X_train, self.Y_train = import_csv_dataset(filename, limit=int(0.7*SAMPLES_LIMIT))
-            
-            self.num_classes = np.unique(self.Y_train).shape[0]
-            if self.classifier is not None and self.X_test is not None and self.Y_test is not None:
-                self.switch_visibility(["-DBM BTN-"], True)
-        
-            self.window["-TRAIN DATA FILE-"].update("Training data file: " + filename)
-            self.window["-TRAIN DATA SHAPE-"].update(f"Training data shape: X {self.X_train.shape} Y {self.Y_train.shape}")
-        except Exception as e:
-            self.dbm_logger.error("Error while loading data file" + str(e))
-            
-    def handle_upload_test_data_event(self, event, values):
-        try:
-            filename = os.path.join(
-                values["-FOLDER-"], values["-FILE LIST-"][0]
-            )
-            self.X_test, self.Y_test = import_csv_dataset(filename, limit=int(0.3*SAMPLES_LIMIT))
-            if self.classifier is not None and self.X_train is not None and self.Y_train is not None:
-                self.switch_visibility(["-DBM BTN-"], True)
-        
-            self.window["-TEST DATA FILE-"].update("Testing data file: " + filename)
-            self.window["-TEST DATA SHAPE-"].update(f"Testing data shape: X {self.X_test.shape} Y {self.Y_test.shape}")
-        except Exception as e:
-            self.dbm_logger.error("Error while loading data file" + str(e))
-    
-    def handle_upload_mnist_data_event(self, event, values):
-        (X_train, Y_train), (X_test, Y_test) = import_mnist_dataset()
-        
-        X_train = X_train.astype('float32') / 255
-        X_test = X_test.astype('float32') / 255
-        
-        X_train, Y_train = X_train[:int(0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
-        X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)], Y_test[:int(0.3*SAMPLES_LIMIT)]
-        
-        self.dataset_name = "MNIST"
-        self.X_train, self.Y_train, self.X_test, self.Y_test = X_train, Y_train, X_test, Y_test
-        self._post_uploading_processing_()     
-    
-    def handle_upload_fashion_mnist_data_event(self, event, values):
-        (X_train, Y_train), (X_test, Y_test) = import_fashion_mnist_dataset()
-        
-        X_train = X_train.astype('float32') / 255
-        X_test = X_test.astype('float32') / 255
-            
-        X_train, Y_train = X_train[:int(0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
-        X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)], Y_test[:int(0.3*SAMPLES_LIMIT)]
-        
-        self.dataset_name = "FASION_MNIST"
-        self.X_train, self.Y_train, self.X_test, self.Y_test = X_train, Y_train, X_test, Y_test
-        self._post_uploading_processing_()     
-    
-    def handle_upload_cifar10_data_event(self, event, values):
-        (X_train, Y_train), (X_test, Y_test) = import_cifar10_dataset()
-    
-        X_train, Y_train = X_train[:int(0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
-        X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)], Y_test[:int(0.3*SAMPLES_LIMIT)]
+        self.color_img = color_img
+        self.legend = patches
 
-        X_train = X_train.astype('float32') / 255
-        X_test = X_test.astype('float32') / 255        
-        
-        self.dataset_name = "CIFAR10"
-        self.X_train, self.Y_train, self.X_test, self.Y_test = X_train, Y_train, X_test, Y_test
-        self._post_uploading_processing_()
-    
-    def _post_uploading_processing_(self):        
-        self.num_classes = np.unique(self.Y_train).shape[0]
-        
-        self.window["-TRAIN DATA FILE-"].update(f"Training data: {self.dataset_name}")
-        self.window["-TRAIN DATA SHAPE-"].update(f"Training data shape: X {self.X_train.shape} Y {self.Y_train.shape}")
-        
-        self.window["-TEST DATA FILE-"].update(f"Testing data: {self.dataset_name}")
-        self.window["-TEST DATA SHAPE-"].update(f"Testing data shape: X {self.X_test.shape} Y {self.Y_test.shape}")
-        
-        if self.classifier is not None:
-            self.switch_visibility(["-DBM BTN-"], True)
-     
-    def handle_dbm_technique_event(self, event, values):
-        dbm_technique = values["-DBM TECHNIQUE-"]
-        if dbm_technique == "Inverse Projection":
-            self.switch_visibility(["-PROJECTION TECHNIQUE TEXT-", "-PROJECTION TECHNIQUE-"], True)
+        return color_img, patches
+
+    def generate_encoded_mapping(self):
+        """Generates a mapping of the encoded data to the original data.
+
+        Returns:
+            train_mapper (dict): Mapping of the encoded train data to the original train data.
+            test_mapper (dict): Mapping of the encoded test data to the original test data.
+        """
+        train_mapper = {}
+        for k in range(len(self.encoded_train)):
+            [i, j, _] = self.encoded_train[k]
+            train_mapper[f"{int(i)} {int(j)}"] = k
+
+        test_mapper = {}
+        for k in range(len(self.encoded_test)):
+            [i, j, _] = self.encoded_test[k]
+            test_mapper[f"{int(i)} {int(j)}"] = k
+
+        return train_mapper, test_mapper
+    
+    def get_classifier_performance_history(self):
+        path = os.path.join(self.save_folder, CLASSIFIER_PERFORMANCE_HISTORY_FILE)
+        if not os.path.isfile(path):
+            raise Exception("Classifier performance history file not found.")
+
+        times, accuracies, losses = [], [], []
+        with open(path, "r") as f:
+            for line in f.readlines():
+                line = line.strip()
+                if len(line) == 0:
+                    continue
+                _, time, _, acc, _, _, loss = line.replace("\n", "").replace("%", "").split(" ")
+                times.append(time)
+                accuracies.append(float(acc))
+                losses.append(float(loss))
+        return times, accuracies, losses
+    
+    def compute_classifier_metrics(self):
+        self.console.log("Evaluating classifier...")
+        loss, accuracy = self.dbm_model.classifier.evaluate(self.X_test, self.Y_test, verbose=0)
+        self.console.log(f"Classifier Accuracy: {(100 * accuracy):.2f}%  Loss: {loss:.2f}")
+
+        path = os.path.join(self.save_folder, CLASSIFIER_PERFORMANCE_HISTORY_FILE)
+
+        with open(path, "a") as f:
+            time = datetime.now().strftime("%D %H:%M:%S")
+            message = f"Accuracy: {(100 * accuracy):.2f}%  Loss: {loss:.2f}"
+            f.write(f"{time} {message}\n")
+        return accuracy, loss
+    
+    def pop_classifier_evaluation(self):
+        path = os.path.join(self.save_folder, CLASSIFIER_PERFORMANCE_HISTORY_FILE)
+        # removing the last line
+        with open(path, "r") as f:
+            lines = f.readlines()
+            lines = lines[:-1]
+        with open(path, "w") as f:
+            f.write("".join(lines))
+
+        if len(lines) == 0:
+            return None, None
+
+        last_line = lines[-1].replace("\n", "")
+        accuracy, loss = float(last_line.split("Accuracy: ")[1].split("%")[0]), float(last_line.split("Loss: ")[1])
+        return accuracy, loss
+    
+    def load_2d_projection(self):
+        if os.path.exists(os.path.join(self.save_folder, TRAIN_2D_FILE_NAME)) and os.path.exists(os.path.join(self.save_folder, TEST_2D_FILE_NAME)):
+            X2d_train = np.load(os.path.join(self.save_folder, TRAIN_2D_FILE_NAME))
+            X2d_test = np.load(os.path.join(self.save_folder, TEST_2D_FILE_NAME))
+            return X2d_train, X2d_test
+        return None, None
+    
+    def transform_changes(self, Y_train, expert_updates_labels_mapper, positions_of_labels_changes):
+        """
+        Returns:
+            position_changes (dict): a dictionary with old position as key and the new position as value
+            label_changes (dict): a dictionary with old and new positions as key and the new label as value
+        """
+        Y = np.copy(Y_train)
+        labels_changes = {}
+
+        pos_x, pos_y, alphas = positions_of_labels_changes
+
+        ALPHA_DECAY_ON_UPDATE = 0.05
+        alphas = [alpha - ALPHA_DECAY_ON_UPDATE if alpha > ALPHA_DECAY_ON_UPDATE else ALPHA_DECAY_ON_UPDATE for alpha in alphas]
+
+        for pos in expert_updates_labels_mapper:
+            k = self.train_mapper[pos]
+            pos_x = np.append(pos_x, int(pos.split(" ")[1]))
+            pos_y = np.append(pos_y, int(pos.split(" ")[0]))
+            alphas = np.append(alphas, 1)
+            y = expert_updates_labels_mapper[pos][0]
+            Y[k] = y
+            labels_changes[pos] = expert_updates_labels_mapper[pos][0]
+
+        positions_of_labels_changes = (pos_x, pos_y, alphas)
+
+        return Y, labels_changes, positions_of_labels_changes
+    
+    def save_labels_changes(self, folder: str = "tmp", label_changes={}):
+        if not os.path.exists(folder):
+            os.path.makedirs(folder)
+
+        with open(os.path.join(folder, LABELS_CHANGES_FILE), "a") as f:
+            f.write("\n" + "-" * 50 + "\n")
+            json.dump(label_changes, f, indent=2)
+
+    def compute_inverse_projection_errors(self):
+        possible_path = os.path.join(self.save_folder, INVERSE_PROJECTION_ERRORS_FILE)
+        # try to get projection errors from cache first
+        if os.path.exists(possible_path):
+            self.inverse_projection_errors = np.load(possible_path)
         else:
-            self.switch_visibility(["-PROJECTION TECHNIQUE TEXT-", "-PROJECTION TECHNIQUE-"], False)
+            self.inverse_projection_errors = self.dbm_model.generate_inverse_projection_errors(save_folder=self.save_folder, resolution=len(self.img))
             
-        self.logger.log(f"DBM technique: {dbm_technique}")
+    def compute_projection_errors(self, type = "non_interpolated"):
+        if type == "interpolated":
+            use_interpolation = True
+            file = PROJECTION_ERRORS_INTERPOLATED_FILE
+        elif type == "non_interpolated":
+            use_interpolation = False
+            file = PROJECTION_ERRORS_INVERSE_PROJECTION_FILE
+            
+        possible_path = os.path.join(self.save_folder, file)
+
+        # try to get projection errors from cache first
+        if os.path.exists(possible_path):
+            self.projection_errors = np.load(possible_path)
+        else:
+            self.projection_errors = self.dbm_model.generate_projection_errors(use_interpolation=use_interpolation, save_folder=self.save_folder)
 
-    def handle_projection_technique_event(self, event, values):
-        projection_technique = values["-PROJECTION TECHNIQUE-"]
-        self.logger.log(f"Projection technique: {projection_technique}") 
-        
-    def handle_dbm_image_event(self, event, values):
-        self.logger.log("Clicked on the dbm image")
-        if self.dbm_plotter_gui is None:
-            self.logger.warn("Nothing to show")
-            return
-        self.dbm_plotter_gui.start()
-                
-    def handle_get_decision_boundary_mapping_event(self, event, values):
-        if self.classifier is None:
-            self.dbm_logger.error("No classifier provided, impossible to generate the DBM...")
-            return
-        
-        if self.X_train is None or self.Y_train is None or self.X_test is None or self.Y_test is None:
-            self.dbm_logger.error("Data is incomplete impossible to generate the DBM...")
-            return 
-        
-        # update loading state
-        self.switch_visibility(["-DBM IMAGE-"], False)
-        self.switch_visibility(["-DBM TEXT-", "-DBM IMAGE LOADING-"], True)
-        
-        dbm = DBM_TECHNIQUES[values["-DBM TECHNIQUE-"]](classifier = self.classifier, logger = self.dbm_logger)
-        
-        projection_technique = values["-PROJECTION TECHNIQUE-"]        
-        show_dbm_history = values["-DBM HISTORY CHECKBOX-"]
-        resolution = 256 #values["-DBM IMAGE RESOLUTION INPUT-"]
-        
-        #if resolution.isdigit() and int(resolution) > 50 and int(resolution) < 800:
-        #    resolution = int(resolution)
-        #else:
-        #    self.dbm_logger.log("Invalid resolution, using default value 256, please enter a value between 50 and 800")
-        #    resolution = 256
+    def undo_changes(self):
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_FOLDER)):
+            raise Exception("Can not undo changes, no previous model found")
+
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_FILE)):
+            raise Exception("Can not undo changes, no previous labels found")
+
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_BOUNDARY_MAP_FILE)):
+            raise Exception("Can not undo changes, no previous boundary map found")
+
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE)):
+            raise Exception("Can not undo changes, no previous confidence map found")
+        
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_CHANGES_FILE)):
+            raise Exception("Can not undo changes, no previous labels changes found")
+        
+        if not os.path.exists(os.path.join(self.save_folder, CLASSIFIER_STACKED_FOLDER)):
+            raise Exception("Can not undo changes, no previous model found")
+
+        self.dbm_model.load_classifier(os.path.join(self.save_folder, CLASSIFIER_STACKED_FOLDER))
+
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_FILE), "rb") as f:
+            self.Y_train = np.load(f)
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_BOUNDARY_MAP_FILE), "rb") as f:
+            self.img = np.load(f)
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE), "rb") as f:
+            self.img_confidence = np.load(f)
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_CHANGES_FILE), "rb") as f:
+            self.positions_of_labels_changes = np.load(f)
+            
+        files_to_delete = [
+            CLASSIFIER_STACKED_LABELS_FILE,
+            CLASSIFIER_STACKED_BOUNDARY_MAP_FILE,
+            CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE,
+            CLASSIFIER_STACKED_LABELS_CHANGES_FILE
+        ]
+
+        for file in files_to_delete:
+            file = os.path.join(self.save_folder, file)
+            if os.path.exists(file):
+                os.remove(file)
+
+
+    def mix_image(self, show_color_map, show_confidence, show_inverse_projection_errors, show_projection_errors):
+        color_img = np.zeros((self.img.shape[0], self.img.shape[1], 3))
+        alphas = 1 + np.zeros((self.img.shape[0], self.img.shape[1]))
+        img = np.zeros((self.img.shape[0], self.img.shape[1], 4))
+
+        if show_color_map:
+            color_img = self.color_img
+
+        if show_confidence:
+            alphas = alphas * self.img_confidence
+        if show_inverse_projection_errors:
+            alphas = alphas * (1 - self.inverse_projection_errors)
+
+        if show_projection_errors and self.projection_errors is not None:
+            alphas = alphas * (1 - self.projection_errors)
+
+        img[:, :, :3] = color_img
+        img[:, :, 3] = alphas
+        return img
+    
+    def get_encoded_train_data(self):
+        return self.encoded_train
+    
+    def get_positions_of_labels_changes(self):
+        return self.positions_of_labels_changes
+    
+    def regenerate_boundary_map(self, Y_transformed, fast_decoding_strategy):
+        if self.projection_technique is None:
+            dbm_info = self.dbm_model.generate_boundary_map(
+                self.X_train,
+                Y_transformed,
+                self.X_test,
+                self.Y_test,
+                resolution=len(self.img),
+                fast_decoding_strategy=fast_decoding_strategy,
+                load_folder=self.save_folder
+            )
+        else:
+            if self.X_train_2d is None or self.X_test_2d is None:
+                self.X_train_2d, self.X_test_2d = self.load_2d_projection()
+            dbm_info = self.dbm_model.generate_boundary_map(
+                Xnd_train=self.X_train,
+                Xnd_test=self.X_test,
+                X2d_train=self.X_train_2d,
+                X2d_test=self.X_test_2d,
+                resolution=len(self.img),
+                fast_decoding_strategy=fast_decoding_strategy,
+                load_folder=self.save_folder,
+                projection=self.projection_technique
+            )
         
-        self.dbm_logger.log(f"DBM resolution: {resolution}")
+        img, img_confidence, encoded_train, encoded_test = dbm_info
         
-        TMP_FOLDER = os.path.join("tmp", self.dataset_name)
-        save_folder = TMP_FOLDER
-        if values["-DBM TECHNIQUE-"] == "Inverse Projection":
-            DEFAULT_MODEL_FOLDER = os.path.join(TMP_FOLDER, "DBM")        
-            
-            if not os.path.exists(os.path.join(DEFAULT_MODEL_FOLDER, projection_technique, "train_2d.npy")):
-                X_train_2d = None
+        self.img = img
+        self.img_confidence = img_confidence
+        self.encoded_train = encoded_train
+        self.encoded_test = encoded_test
+        self.Y_train = Y_transformed
+        self.initialize()
+        
+    def apply_labels_changes(self, decoding_strategy):
+        num_changes = len(self.expert_updates_labels_mapper)
+        if num_changes == 0:
+            raise Exception("No changes to apply")
+        if num_changes < 10:
+            raise Exception("Less than 10 changes to apply, please apply more changes")
+
+        # store the changes done so far so we can restore them when needed
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_CHANGES_FILE), "wb") as f:
+            np.save(f, self.positions_of_labels_changes)
+
+        self.console.log("Transforming changes...")
+        Y_transformed, label_changes, positions_of_labels_changes = self.transform_changes(self.Y_train, self.expert_updates_labels_mapper, self.positions_of_labels_changes)
+        self.positions_of_labels_changes = positions_of_labels_changes
+
+        self.console.log("Saving changes to a local folder...")
+        self.save_labels_changes(self.save_folder, label_changes=label_changes)
+
+        self.updates_logger.log("Applying changes... This might take a couple of seconds, after this the window will be closed")
+
+        save_folder = os.path.join(self.save_folder, CLASSIFIER_REFIT_FOLDER)
+
+        # store the old model so we can restore it when needed
+        self.dbm_model.save_classifier(save_folder=os.path.join(self.save_folder, CLASSIFIER_STACKED_FOLDER))
+        # store the old labels so we can restore them when needed
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_FILE), "wb") as f:
+            np.save(f, self.Y_train)
+
+        # store the old decision boundary map and confidence map so we can restore them when needed
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_BOUNDARY_MAP_FILE), "wb") as f:
+            np.save(f, self.img)
+        with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE), "wb") as f:
+            np.save(f, self.img_confidence)
+
+        self.dbm_model.refit_classifier(self.X_train, Y_transformed, save_folder=save_folder, epochs=EPOCHS_FOR_REFIT)
+        self.regenerate_boundary_map(Y_transformed, decoding_strategy)
+        
+    def set_dbm_model_logger(self, logger):
+        self.dbm_model.console = logger
+    
+    def set_updates_logger(self, logger):
+        self.updates_logger = logger
+    
+    def build_annotation_mapper(self, fig, ax):
+        """ Builds the annotation mapper.
+            This is used to display the data point label when hovering over the decision boundary.
+        """
+        image = OffsetImage(self.X_train[0], zoom=2, cmap="gray")
+        label = TextArea("Data point label: None")
+
+        annImage = AnnotationBbox(image, (0, 0), xybox=(50., 50.), xycoords='data', boxcoords="offset points",  pad=0.1,  arrowprops=dict(arrowstyle="->"))
+        annLabels = AnnotationBbox(label, (0, 0), xybox=(50., 50.), xycoords='data', boxcoords="offset points",  pad=0.3,  arrowprops=dict(arrowstyle="->"))
+
+        ax.add_artist(annImage)
+        ax.add_artist(annLabels)
+        annImage.set_visible(False)
+        annLabels.set_visible(False)
+
+        fig_width, fig_height = fig.get_size_inches() * fig.dpi
+
+        def display_annotation(event):
+            """Displays the annotation box when hovering over the decision boundary based on the mouse position."""
+            if event.inaxes == None:
+                return
+
+            j, i = int(event.xdata), int(event.ydata)
+
+            # change the annotation box position relative to mouse.
+            ws = (event.x > fig_width/2.)*-1 + (event.x <= fig_width/2.)
+            hs = (event.y > fig_height/2.)*-1 + (event.y <= fig_height/2.)
+            annImage.xybox = (50. * ws, 50. * hs)
+            annLabels.xybox = (-50. * ws, 50. * hs)
+            # make annotation box visible
+            annImage.set_visible(True)
+            # place it at the position of the event scatter point
+            annImage.xy = (j, i)
+
+            x_data, y_data = find_data_point(i, j)
+            if x_data is not None:
+                annImage.set_visible(True)
+                image.set_data(x_data)
             else:
-                with open(os.path.join(DEFAULT_MODEL_FOLDER, projection_technique, "train_2d.npy"), "rb") as f:
-                    X_train_2d = np.load(f)
-            if not os.path.exists(os.path.join(DEFAULT_MODEL_FOLDER, projection_technique, "test_2d.npy")):
-                X_test_2d = None
+                annImage.set_visible(False)
+
+            if y_data is not None:
+                annLabels.set_visible(True)
+                annLabels.xy = (j, i)
+                label.set_text(f"{y_data}")
             else:
-                with open(os.path.join(DEFAULT_MODEL_FOLDER, projection_technique, "test_2d.npy"), "rb") as f:
-                    X_test_2d = np.load(f)
-            save_folder = os.path.join(DEFAULT_MODEL_FOLDER, projection_technique)
-            dbm_info = dbm.generate_boundary_map(
-                                        self.X_train, 
-                                        self.Y_train, 
-                                        self.X_test, 
-                                        self.Y_test, 
-                                        X2d_train=X_train_2d,
-                                        X2d_test=X_test_2d,
-                                        resolution=resolution,
-                                        load_folder=DEFAULT_MODEL_FOLDER,
-                                        projection=projection_technique
-                                        )
-        else:
-            save_folder = os.path.join(TMP_FOLDER, "SDBM")
-            dbm_info = dbm.generate_boundary_map(
-                                        self.X_train, 
-                                        self.Y_train, 
-                                        self.X_test, 
-                                        self.Y_test, 
-                                        resolution=resolution,
-                                        load_folder=save_folder,
-                                        projection=projection_technique
-                                        )
+                annLabels.set_visible(False)
 
-        img, img_confidence, encoded_training_data, encoded_testing_data, training_history = dbm_info
-        
-        if show_dbm_history:
-            self.show_dbm_history(training_history)
-        
-        
-        # ---------------------------------
-        # create a GUI window for Decision Boundary Mapping
-        self.dbm_plotter_gui = DBMPlotterGUI(
-                                            dbm_model = dbm,
-                                            img = img,
-                                            img_confidence = img_confidence,
-                                            encoded_train = encoded_training_data, 
-                                            encoded_test = encoded_testing_data,
-                                            X_train = self.X_train,
-                                            Y_train = self.Y_train,
-                                            X_test = self.X_test,
-                                            Y_test = self.Y_test,                                            
-                                            main_gui=self, # reference to the main GUI
-                                            save_folder=save_folder,
-                                            projection_technique=projection_technique,
-                                            )
-        
-        # ---------------------------------
-        # update the dbm image
-        img = Image.fromarray(np.uint8(self.dbm_plotter_gui.color_img*255))
-        WINDOW_IMAGE_RESOLUTION = 256
-        img.thumbnail((WINDOW_IMAGE_RESOLUTION, WINDOW_IMAGE_RESOLUTION), Image.ANTIALIAS)
-        # Convert im to ImageTk.PhotoImage after window finalized
-        image = ImageTk.PhotoImage(image=img)        
-        self.window["-DBM IMAGE-"].update(data=image)
-                    
-        self.switch_visibility(["-DBM IMAGE LOADING-"], False)
-        self.switch_visibility(["-DBM IMAGE-"], True)
-    
-    def handle_changes_in_dbm_plotter(self):
-        # update loading state
-        self.switch_visibility(["-DBM IMAGE-"], False)
-        self.switch_visibility(["-DBM TEXT-", "-DBM IMAGE LOADING-"], True)
-        
-        # ---------------------------------
-        # update the dbm image
-        img = Image.fromarray(np.uint8(self.dbm_plotter_gui.color_img*255))
-        WINDOW_IMAGE_RESOLUTION = 256
-        img.thumbnail((WINDOW_IMAGE_RESOLUTION, WINDOW_IMAGE_RESOLUTION), Image.ANTIALIAS)
-        # Convert im to ImageTk.PhotoImage after window finalized
-        image = ImageTk.PhotoImage(image=img)        
-        self.window["-DBM IMAGE-"].update(data=image)
-                    
-        self.switch_visibility(["-DBM IMAGE LOADING-"], False)
-        self.switch_visibility(["-DBM IMAGE-"], True)
-    
-    def show_dbm_history(self, training_history):
-        # this is for plotting the training history
-        plt.close()
-        fig, [ax1, ax2, ax3] = plt.subplots(1, 3, figsize=(20, 5))
-        ax1.set_title("Loss")
-        ax1.plot(training_history["loss"], label="loss")
-        ax1.plot(training_history["val_loss"], label="val_loss")
-        ax1.legend()
-        
-        ax2.set_title("Decoder Accuracy")
-        ax2.plot(training_history["decoder_accuracy"], label="decoder_accuracy")
-        ax2.plot(training_history["val_decoder_accuracy"], label="val_decoder_accuracy")
-        ax2.legend()
-        
-        ax3.set_title("Classifier Accuracy")
-        ax3.plot(training_history["classifier_accuracy"], label="classifier_accuracy")
-        ax3.plot(training_history["val_classifier_accuracy"], label="val_classifier_accuracy")
-        ax3.legend()
-        
-        plt.show()
-    
+            fig.canvas.draw_idle()
+
+        def find_data_point(i, j):
+            # search for the data point in the encoded train data
+            if self.img[i][j] == TRAIN_DATA_POINT_MARKER:
+                k = self.train_mapper[f"{i} {j}"]
+                if f"{i} {j}" in self.expert_updates_labels_mapper:
+                    l = self.expert_updates_labels_mapper[f"{i} {j}"][0]
+                    return self.X_train[k], f"Label {self.Y_train[k]} \nClassifier label: {int(self.encoded_train[k][2])} \nExpert label: {l}"
+                return self.X_train[k], f"Label: {self.Y_train[k]} \nClassifier label: {int(self.encoded_train[k][2])}"
+
+            # search for the data point in the encoded test data
+            if self.img[i][j] == TEST_DATA_POINT_MARKER:
+                k = self.test_mapper[f"{i} {j}"]
+                return self.X_test[k], f"Classifier label: {int(self.encoded_test[k][2])}"
+
+            # generate the nD data point on the fly using the inverse projection
+            point = self.dbm_model.neural_network.decode([(i/self.img.shape[0], j/self.img.shape[1])])[0]
+            return point, None
+
+        def onclick(event):
+            """ Open the data point in a new window when clicked on a pixel in training or testing set based on mouse position."""
+            if event.inaxes == None:
+                return
+
+            if self.update_labels_by_circle_select:
+                onclick_circle_strategy(event)
+                return
+
+            self.console.log("Clicked on: " + str(event.xdata) + ", " + str(event.ydata))
+            j, i = int(event.xdata), int(event.ydata)
+
+            if self.img[i][j] != TRAIN_DATA_POINT_MARKER:
+                self.console.log("Data point not in training set")
+                return
+
+            # check if clicked on a data point that already was updated, then remove the update
+            if f"{i} {j}" in self.expert_updates_labels_mapper:
+                (_, point) = self.expert_updates_labels_mapper[f"{i} {j}"]
+                point.remove()
+                del self.expert_updates_labels_mapper[f"{i} {j}"]
+                fig.canvas.draw_idle()
+                self.updates_logger.log(f"Removed updates for point: ({j}, {i})")
+                return
+
+            # if clicked on a data point that was not updated, then add the update
+            self.current_selected_point = ax.plot(j, i, 'bo', markersize=5)[0]
+
+            # disable annotations on hover
+            # if self.motion_event_cid is not None:
+            #    fig.canvas.mpl_disconnect(self.motion_event_cid)
+            # disable on click event
+            if self.click_event_cid is not None:
+                fig.canvas.mpl_disconnect(self.click_event_cid)
+                self.click_event_cid = None
+
+            # enable key press events
+            self.key_event_cid = fig.canvas.mpl_connect('key_press_event', onkey)
+
+            fig.canvas.draw_idle()
+
+        def onkey(event):
+            if self.current_selected_point is None:
+                return
+
+            if event.key.isdigit():
+                self.current_selected_point_assigned_label = int(event.key)
+                return
+
+            (x, y) = self.current_selected_point.get_data()
+
+            if event.key == 'escape' or event.key == 'enter':
+                self.current_selected_point.remove()
+
+                if event.key == 'escape':
+                    self.updates_logger.log("Cancelled point move...")
+
+                elif event.key == 'enter':
+                    # showing the fix of the position
+                    self.current_selected_point = ax.plot(x, y, 'b^')[0]
+                    if self.current_selected_point_assigned_label is not None:
+                        self.updates_logger.log(f"Assigned label: {self.current_selected_point_assigned_label} to point: ({x[0]}, {y[0]})")
+                        self.expert_updates_labels_mapper[f"{y[0]} {x[0]}"] = (self.current_selected_point_assigned_label, self.current_selected_point)
+
+                self.current_selected_point = None
+                self.current_selected_point_assigned_label = None
+
+                self.motion_event_cid = fig.canvas.mpl_connect('motion_notify_event', display_annotation)
+                self.click_event_cid = fig.canvas.mpl_connect('button_press_event', onclick)
+                fig.canvas.mpl_disconnect(self.key_event_cid)
+                fig.canvas.draw_idle()
+                return
+
+        def onclick_circle_strategy(event):
+            self.console.log("Clicked on: " + str(event.xdata) + ", " + str(event.ydata))
+            x, y = int(event.xdata), int(event.ydata)
+            self.current_selected_point = (x, y)
+            self.release_event_cid = fig.canvas.mpl_connect('button_release_event', onrelease_circle_strategy)
+
+        def onrelease_circle_strategy(event):
+            if event.inaxes == None:
+                return
+            self.console.log("Released on: " + str(event.xdata) + ", " + str(event.ydata))
+            (x0, y0) = self.current_selected_point
+            x1, y1 = int(event.xdata), int(event.ydata)
+            (cx, cy) = (x0 + (x1 - x0)/2, y0 + (y1 - y0)/2)  # circle center
+            r = sqrt(((x1 - x0)/2)**2 + ((y1 - y0)/2)**2)   # circle radius
+            self.update_labels_circle = Circle((cx, cy), r, color='black', fill=False)
+            ax.add_artist(self.update_labels_circle)
+            self.key_event_cid = fig.canvas.mpl_connect('key_press_event', onkey_circle_strategy)
+            if self.release_event_cid is not None:
+                fig.canvas.mpl_disconnect(self.release_event_cid)
+            fig.canvas.draw_idle()
+
+        def onkey_circle_strategy(event):
+            if self.update_labels_circle is None:
+                return
+
+            if event.key.isdigit():
+                self.current_selected_point_assigned_label = int(event.key)
+                return
+
+            (x, y) = self.update_labels_circle.get_center()
+            r = self.update_labels_circle.get_radius()
+            if event.key == "enter" and self.current_selected_point_assigned_label is not None:
+                self.updates_logger.log(f"Assigned label: {self.current_selected_point_assigned_label} to circle: center ({x}, {y}), radius ({r})")
+                positions = find_points_in_circle((x, y), r)
+                for pos in positions:
+                    point = ax.plot(pos[0], pos[1], 'b^')[0]
+                    self.expert_updates_labels_mapper[f"{pos[1]} {pos[0]}"] = (self.current_selected_point_assigned_label, point)
+
+            if event.key == "backspace":
+                self.updates_logger.log(f"Removing changes in circle: center ({x},{y}), radius ({r})")
+                positions = find_points_in_circle((x, y), r)
+                for pos in positions:
+                    if f"{pos[1]} {pos[0]}" in self.expert_updates_labels_mapper:
+                        self.expert_updates_labels_mapper[f"{pos[1]} {pos[0]}"][1].remove()
+                        del self.expert_updates_labels_mapper[f"{pos[1]} {pos[0]}"]
+
+            self.update_labels_circle.remove()
+            self.update_labels_circle = None
+            fig.canvas.mpl_disconnect(self.key_event_cid)
+            fig.canvas.draw_idle()
+
+        def find_points_in_circle(circle_center, circle_radius):
+            (cx, cy) = circle_center
+            initial_x, initial_y = int(cx - circle_radius), int(cy - circle_radius)
+            final_x, final_y = int(cx + circle_radius) + 1, int(cy + circle_radius) + 1
+            initial_x = 0 if initial_x < 0 else initial_x
+            initial_y = 0 if initial_y < 0 else initial_y
+            final_x = self.img.shape[0] if final_x > self.img.shape[0] else final_x
+            final_y = self.img.shape[0] if final_y > self.img.shape[0] else final_y
+
+            positions = []
+            for x in range(initial_x, final_x):
+                for y in range(initial_y, final_y):
+                    if (self.img[y, x] == TRAIN_DATA_POINT_MARKER) and ((x - cx)**2 + (y - cy)**2 <= circle_radius**2):
+                        positions.append((x, y))
+            return positions
+
+        self.motion_event_cid = fig.canvas.mpl_connect('motion_notify_event', display_annotation)
+        self.click_event_cid = fig.canvas.mpl_connect('button_press_event', onclick)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/GUI/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .GUI import GUI
-from .DBMPlotterGUI import DBMPlotterGUI
+from .SDBM import SDBM, NNArchitecture
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/Logger.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/Logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 # Copyright 2022 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from datetime import datetime
 from termcolor import colored
 
 from .LoggerInterface import LoggerInterface
 
+
 class Logger(LoggerInterface):
     """ A console logger
         Prints the messages to the default console
     """
-    
-    def __init__(self, active:bool=True, name:str="Logger", info_color:str="magenta", show_init:bool=True):
+
+    def __init__(self, active: bool = True, name: str = "Logger", info_color: str = "magenta", show_init: bool = True):
         """ Initialize the logger
 
         Args:
             active (bool, optional): Defaults to True.
             name (str, optional): Defaults to "Logger".
+            info_color (str, optional): Defaults to "magenta". The color of the info message
+            show_init (bool, optional): Defaults to True. Show the initialization message
         """
         self.active = active
         self.name = name
         self.info_color = info_color
-        
-        if show_init:    
+
+        if show_init:
             sep = "=" * 30
             time = datetime.now().strftime("%H:%M:%S:%f")
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
-        
-        
-    def log(self, message:str):
+
+    def log(self, message: str):
         """ Log a message to the console
             Args:
                 message (str): the message to log
         """
         if self.active:
             time = datetime.now().strftime("%H:%M:%S:%f")
             print(colored(f"[INFO] [{time}] [{self.name}] {message}", self.info_color))
-    
-    def warn(self, message:str):
+
+    def warn(self, message: str):
         if self.active:
             time = datetime.now().strftime("%H:%M:%S:%f")
             print(colored(f"[WARNING] [{time}] [{self.name}] {message}", "yellow"))
-    
-    def error(self, message:str):
+
+    def error(self, message: str):
         if self.active:
             time = datetime.now().strftime("%H:%M:%S:%f")
             print(colored(f"[ERROR] [{time}] [{self.name}] {message}", "red"))
-    
-    def debug(self, message:str):
+
+    def debug(self, message: str):
         if self.active:
             time = datetime.now().strftime("%H:%M:%S:%f")
-            print(colored(f"[DEBUG] [{time}] [{self.name}] {message}","blue"))
-            
-    def success(self, message:str):
+            print(colored(f"[DEBUG] [{time}] [{self.name}] {message}", "blue"))
+
+    def success(self, message: str):
         if self.active:
             time = datetime.now().strftime("%H:%M:%S:%f")
-            print(colored(f"[SUCCESS] [{time}] [{self.name}] {message}", "green"))
+            print(colored(f"[SUCCESS] [{time}] [{self.name}] {message}", "green"))
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerGUI.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerGUI.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from termcolor import colored
 
 from .LoggerInterface import LoggerInterface
 
+
 class LoggerGUI(LoggerInterface):
     """ Logs the messages to the GUI.
     """
-    
-    def __init__(self, name:str="Logger", active:bool=True, output=None, update_callback=lambda x: x, info_color:str="magenta", show_init:bool=True):
+
+    def __init__(self, name: str = "Logger", active: bool = True, output=None, update_callback=lambda: "", info_color: str = "magenta", show_init: bool = True):
         """ Initialize the logger
 
         Args:
             name (str, optional): Defaults to "Logger".
             active (bool, optional): Defaults to True.
             output (any, optional): The GUI reference where the logger should display messages. Defaults to None.
             update_callback (python function, optional): The function that is called to update the GUI. Defaults to lambda x:x.
         """
         super().__init__()
 
-        self.active = active 
+        self.active = active
         self.name = name
         self.info_color = info_color
-    
+
         if output is not None:
             self.output = output
             self.update_callback = update_callback
         else:
             print("No output provided for LoggerGUI. LoggerGUI will not print anything.")
             self.active = False
-        
-        if show_init and self.active:    
+
+        if show_init and self.active:
             sep = "=" * 30
             time = datetime.now().strftime("%H:%M:%S:%f")
-            
+
             self.print(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color)
             self.print(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color)
             self.print(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color)
 
-
-    def print(self, message:str, color:str='magenta'):
+    def print(self, message: str, color: str = 'magenta'):
         if self.active:
             self.output.print(message, text_color=color)
             self.update_callback()
-            
-    def log(self, message:str):
+
+    def log(self, message: str):
         time = datetime.now().strftime("%H:%M:%S:%f")
         self.print(f"[INFO] [{time}] [{self.name}] {message}", self.info_color)
-    
-    def warn(self, message:str):
+
+    def warn(self, message: str):
         time = datetime.now().strftime("%H:%M:%S:%f")
         self.print(f"[WARNING] [{time}] [{self.name}] {message}", "yellow")
-    
-    
-    def error(self, message:str):
+
+    def error(self, message: str):
         time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[ERROR] [{time}] [{self.name}] {message}", "red")        
-    
-    def debug(self, message:str):
+        self.print(f"[ERROR] [{time}] [{self.name}] {message}", "red")
+
+    def debug(self, message: str):
         time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[DEBUG] [{time}] [{self.name}] {message}","blue")
-    
-        
-    def success(self, message:str):
+        self.print(f"[DEBUG] [{time}] [{self.name}] {message}", "blue")
+
+    def success(self, message: str):
         time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[SUCCESS] [{time}] [{self.name}] {message}", "green")
+        self.print(f"[SUCCESS] [{time}] [{self.name}] {message}", "green")
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerInterface.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerInterface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 class LoggerInterface:
     """ Interface for the logger class
     """
-    
-    def log(self, message:str):
+
+    def log(self, message: str):
         """ Log a message to the console
         Args:
             message (str): the message to log
         """
         pass
-        
-    def warn(self, message:str):
+
+    def warn(self, message: str):
+        pass
+
+    def error(self, message: str):
         pass
-    
-    def error(self, message:str):
+
+    def debug(self, message: str):
         pass
-    
-    def debug(self, message:str):
+
+    def success(self, message: str):
         pass
-        
-    def success(self, message:str):
-        pass
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/LoggerModel.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from termcolor import colored
 from tensorflow.keras.callbacks import Callback
 
+
 class LoggerModel(Callback):
-    def __init__(self, active:bool=True, name:str="Neural Network", info_color:str="magenta", show_init:bool=True, epochs:int=100):
+    def __init__(self, active: bool = True, name: str = "Neural Network", info_color: str = "magenta", show_init: bool = True, epochs: int = 100):
         """ Initialize the logger
 
         Args:
             active (bool, optional): Defaults to True.
             name (str, optional): Defaults to "Logger".
         """
         self.active = active
         self.name = name
         self.info_color = info_color
         self.epochs = epochs
-        if show_init:    
+        if show_init:
             sep = "=" * 30
             time = datetime.now().strftime("%H:%M:%S:%f")
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
-        
 
     def on_epoch_end(self, epoch, logs={}):
         if self.active:
             logs = ", ".join([f"{key}: {value:.4f}" for key, value in logs.items()])
             print(colored(f"[INFO] [{self.name}] [Epoch {epoch}/{self.epochs}] {logs}", self.info_color))
-
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/Logger/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .Logger import Logger
 from .LoggerGUI import LoggerGUI
 from .LoggerInterface import LoggerInterface
-from .LoggerModel import LoggerModel
+from .LoggerModel import LoggerModel
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .Logger import Logger, LoggerGUI, LoggerInterface
-from .DBM import DBM, SDBM
-from .GUI import GUI
-from .examples import DBM_usage_example, SDBM_usage_example, DBM_usage_example_GUI, SDBM_usage_example_GUI
+from .DBM_usage_example import DBM_usage_example, DBM_usage_example_GUI
+from .SDBM_usage_example import SDBM_usage_example, SDBM_usage_example_GUI
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/DBM_usage_example.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/DBM_usage_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,140 +1,146 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 
-from ..DBM import DBM
+from ..DBM import DBM, FAST_DBM_STRATEGIES
 from ..GUI import DBMPlotterGUI
 
 from .utils import *
 
+
 def DBM_usage_example():
     # import the dataset
-    X_train, X_test, Y_train, Y_test = import_data()
-    
+    X_train, X_test, _, _ = import_data()
+
     # import the classifier
     classifier = import_classifier()
-    
+
     # create the DBM
     dbm = DBM(classifier=classifier)
-    
+
+    X2d_train, X2d_test = import_2d_data()
+
     # use the DBM to get the decision boundary map, if you don't have the 2D projection of the data
     # the DBM will get it for you, you just need to specify the projection method you would like to use (t-SNE, PCA or UMAP)
-    img, img_confidence, _, _, _ = dbm.generate_boundary_map(X_train, Y_train, 
-                                                                X_test, Y_test, 
-                                                                resolution=256, 
-                                                                load_folder=os.path.join("tmp", "MNIST", "DBM"),                                                                                                                             
-                                                                projection="t-SNE")
-    
+    img, img_confidence, _, _ = dbm.generate_boundary_map(X_train,
+                                                          X_test,
+                                                          X2d_train=X2d_train,
+                                                          X2d_test=X2d_test,
+                                                          resolution=256,
+                                                          load_folder=os.path.join("tmp", "MNIST", "DBM"),
+                                                          fast_decoding_strategy=FAST_DBM_STRATEGIES.NONE,
+                                                          )
+
     # if you have the 2D projection of the data, you can use the following function to get the decision boundary map
     """
     X2d_train, X2d_test = None, None # get the 2D projection of the data by yourself
-    img, img_confidence, _, _, _ = dbm.generate_boundary_map(X_train, Y_train, 
-                                                                X_test, Y_test,
-                                                                X2d_train=X2d_train, 
-                                                                X2d_test=X2d_test,
-                                                                load_folder=os.path.join("tmp", "MNIST", "DBM"), 
-                                                                use_fast_decoding=True,  
-                                                                resolution=256)
-    """                                                                  
-    
+    img, img_confidence, _, _ = dbm.generate_boundary_map(X_train,
+                                                          X_test,
+                                                          X2d_train=X2d_train, 
+                                                          X2d_test=X2d_test,
+                                                          load_folder=os.path.join("tmp", "MNIST", "DBM"), 
+                                                          resolution=256)
+    """
+
     # make the decision boundary map pretty, by adding the colors and the confidence
     COLORS_MAPPER = {
-        -2: [0,0,0], # setting original test data to black
-        -1: [1,1,1], # setting original train data to white
-        0: [1,0,0], 
-        1: [0,1,0], 
-        2: [0,0,1], 
-        3: [1,1,0], 
-        4: [0,1,1], 
-        5: [1,0,1], 
-        6: [0.5,0.5,0.5], 
-        7: [0.5,0,0], 
-        8: [0,0.5,0], 
-        9: [0,0,0.5]
+        -2: [0, 0, 0],  # setting original test data to black
+        -1: [1, 1, 1],  # setting original train data to white
+        0: [1, 0, 0],
+        1: [0, 1, 0],
+        2: [0, 0, 1],
+        3: [1, 1, 0],
+        4: [0, 1, 1],
+        5: [1, 0, 1],
+        6: [0.5, 0.5, 0.5],
+        7: [0.5, 0, 0],
+        8: [0, 0.5, 0],
+        9: [0, 0, 0.5]
     }
 
     color_img = np.zeros((img.shape[0], img.shape[1], 4))
-    for i, j in np.ndindex(img.shape):       
-        color_img[i,j] = COLORS_MAPPER[img[i,j]] + [img_confidence[i,j]]
-    
+    for i, j in np.ndindex(img.shape):
+        color_img[i, j] = COLORS_MAPPER[img[i, j]] + [img_confidence[i, j]]
+
     # plot the decision boundary map
     plt.title("Decision boundary map")
     plt.axis("off")
     plt.imshow(color_img)
     plt.show()
-    
-    
+
     # use the dbm to get the inverse projection errors
     img_inverse_projection_errors = dbm.generate_inverse_projection_errors(resolution=256)
     # plot the inverse projection errors
     fig, ax = plt.subplots()
     ax.set_title("Inverse projection errors")
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
     img_ax = ax.imshow(img_inverse_projection_errors)
     fig.colorbar(img_ax, ax=ax)
     plt.show()
-                                                           
+
     # use the dbm to get the projection errors
     img_projection_errors = dbm.generate_projection_errors()
     # plot the projection errors
     fig, ax = plt.subplots()
     ax.set_title("Projection errors")
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
     img_ax = ax.imshow(img_projection_errors)
     fig.colorbar(img_ax, ax=ax)
     plt.show()
-    
+
+
 def DBM_usage_example_GUI():
     # import the dataset
     X_train, X_test, Y_train, Y_test = import_data()
-    
+
     # import the classifier
     classifier = import_classifier()
-    
+
     # import the 2D projection of the data
     X2d_train, X2d_test = import_2d_data()
-    
+
     # create the DBM
     dbm = DBM(classifier=classifier)
-    
+
     # use the DBM to get the decision boundary map, if you don't have the 2D projection of the data
     # the DBM will get it for you, you just need to specify the projection method you would like to use (t-SNE, PCA or UMAP)
-    dbm_info = dbm.generate_boundary_map(X_train, Y_train, 
-                                         X_test, Y_test, 
-                                         X2d_train=X2d_train,
-                                         X2d_test=X2d_test,
-                                         resolution=256, 
-                                         load_folder=os.path.join("tmp", "MNIST", "DBM"),                                                                                                                             
-                                         projection="t-SNE")
-    
-    img, img_confidence, encoded_training_data, encoded_testing_data, training_history  = dbm_info
+    img, img_confidence, encoded_training_data, encoded_testing_data = dbm.generate_boundary_map(X_train,
+                                                                                                 X_test,
+                                                                                                 X2d_train=X2d_train,
+                                                                                                 X2d_test=X2d_test,
+                                                                                                 resolution=256,
+                                                                                                 load_folder=os.path.join("tmp", "MNIST", "DBM"),
+                                                                                                 projection = "t-SNE",
+                                                                                                 )
+
     
-    dbm_plotter_gui = DBMPlotterGUI(dbm_model = dbm,
-                                    img = img,
-                                    img_confidence = img_confidence,
-                                    encoded_train = encoded_training_data, 
-                                    encoded_test = encoded_testing_data,
-                                    X_train = X_train,
-                                    Y_train = Y_train,
-                                    X_test = X_test,
-                                    Y_test = Y_test,                                    
-                                    save_folder=os.path.join("tmp", "MNIST", "DBM"), # this is the folder where the DBM will save the changes in data the user makes
+    dbm_plotter_gui = DBMPlotterGUI(dbm_model=dbm,
+                                    img=img,
+                                    img_confidence=img_confidence,
+                                    encoded_train=encoded_training_data,
+                                    encoded_test=encoded_testing_data,
+                                    X_train=X_train,
+                                    Y_train=Y_train,
+                                    X_test=X_test,
+                                    Y_test=Y_test,
+                                    # this is the folder where the DBM will save the changes in data the user makes
+                                    save_folder=os.path.join("tmp", "MNIST", "DBM"),
                                     projection_technique="t-SNE",
                                     )
-    dbm_plotter_gui.start()
+    dbm_plotter_gui.start()
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/SDBM_usage_example.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/SDBM_usage_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,120 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-from ..DBM import SDBM
+from ..DBM import SDBM, NNArchitecture
 from ..GUI import DBMPlotterGUI
 
 from .utils import *
 
+
 def SDBM_usage_example():
     # import the dataset
     X_train, X_test, Y_train, Y_test = import_data()
-    
+
     # import the classifier
     classifier = import_classifier()
-    
+
     # create the DBM
     sdbm = SDBM(classifier=classifier)
-    
+
     # use the SDBM to get the decision boundary map
-    img, img_confidence, _, _, _ = sdbm.generate_boundary_map(X_train, Y_train, 
-                                                                X_test, Y_test,
-                                                                load_folder=os.path.join("tmp", "MNIST", "SDBM"),    
-                                                                resolution=256)
-    
-    
+    img, img_confidence, _, _ = sdbm.generate_boundary_map(X_train, Y_train,
+                                                           X_test, Y_test,
+                                                           nn_architecture=NNArchitecture.SSNP,
+                                                           load_folder=os.path.join("tmp", "MNIST", "SDBM"),
+                                                            resolution=256)
+
     # make the decision boundary map pretty, by adding the colors and the confidence
     COLORS_MAPPER = {
-        -2: [0,0,0], # setting original test data to black
-        -1: [1,1,1], # setting original train data to white
-        0: [1,0,0], 
-        1: [0,1,0], 
-        2: [0,0,1], 
-        3: [1,1,0], 
-        4: [0,1,1], 
-        5: [1,0,1], 
-        6: [0.5,0.5,0.5], 
-        7: [0.5,0,0], 
-        8: [0,0.5,0], 
-        9: [0,0,0.5]
+        -2: [0, 0, 0],  # setting original test data to black
+        -1: [1, 1, 1],  # setting original train data to white
+        0: [1, 0, 0],
+        1: [0, 1, 0],
+        2: [0, 0, 1],
+        3: [1, 1, 0],
+        4: [0, 1, 1],
+        5: [1, 0, 1],
+        6: [0.5, 0.5, 0.5],
+        7: [0.5, 0, 0],
+        8: [0, 0.5, 0],
+        9: [0, 0, 0.5]
     }
 
     color_img = np.zeros((img.shape[0], img.shape[1], 4))
-    for i, j in np.ndindex(img.shape):       
-        color_img[i,j] = COLORS_MAPPER[img[i,j]] + [img_confidence[i,j]]
-    
+    for i, j in np.ndindex(img.shape):
+        color_img[i, j] = COLORS_MAPPER[img[i, j]] + [img_confidence[i, j]]
+
     # plot the decision boundary map
     plt.title("Decision boundary map")
     plt.axis("off")
     plt.imshow(color_img)
     plt.show()
-    
+
     # use the SDBM to get the inverse projection errors
-    img_inverse_projection_errors = sdbm.generate_inverse_projection_errors(resolution=256)
+    img_inverse_projection_errors = sdbm.generate_inverse_projection_errors(
+        resolution=256)
     # plot the inverse projection errors
     fig, ax = plt.subplots()
     ax.set_title("Inverse projection errors")
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
     img_ax = ax.imshow(img_inverse_projection_errors)
     fig.colorbar(img_ax, ax=ax)
     plt.show()
-    
+
     # use the SDBM to get the projection errors
     img_projection_errors = sdbm.generate_projection_errors()
     # plot the projection errors
     fig, ax = plt.subplots()
     ax.set_title("Projection errors")
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
     img_ax = ax.imshow(img_projection_errors)
     fig.colorbar(img_ax, ax=ax)
     plt.show()
-    
+
+
 def SDBM_usage_example_GUI():
     # import the dataset
     X_train, X_test, Y_train, Y_test = import_data()
-    
-    Y = np.copy(Y_train)
-    
-    # use the opf to generate the labels for the training data if the data is not completely labelled
-    Y_train = opf(X_train=X_train, Y_train=Y_train)
-    
-    # generate a classifier
-    classifier = generate_classifier(X_train, Y_train)
-    
+
     # import the classifier
-    #classifier = import_classifier()
-    
+    classifier = import_classifier()
+
     # create the DBM
     sdbm = SDBM(classifier=classifier)
-    
-    
-    # use the DBM to get the decision boundary map, if you don't have the 2D projection of the data
-    # the DBM will get it for you, you just need to specify the projection method you would like to use (t-SNE, PCA or UMAP)
-    dbm_info = sdbm.generate_boundary_map(X_train, Y, 
-                                         X_test, Y_test,
-                                         resolution=256,
-                                         load_folder=os.path.join("tmp", "MNIST", "SDBM"),                                                                                                                             
-                                         )
-    
-    img, img_confidence, encoded_training_data, encoded_testing_data, training_history  = dbm_info
-    
-    dbm_plotter_gui = DBMPlotterGUI(dbm_model = sdbm,
-                                    img = img,
-                                    img_confidence = img_confidence,
-                                    encoded_train = encoded_training_data, 
-                                    encoded_test = encoded_testing_data,
-                                    X_train = X_train,
-                                    Y_train = Y_train,
-                                    X_test = X_test,
-                                    Y_test = Y_test,
-                                    save_folder=os.path.join("tmp", "MNIST", "SDBM"), # this is the folder where the DBM will save the changes in data the user makes                                    
+
+    # use the SDBM to get the decision boundary map
+    img, img_confidence, encoded_training_data, encoded_testing_data = sdbm.generate_boundary_map(X_train, Y_train,
+                                                                                                  X_test, Y_test,
+                                                                                                  resolution=256,
+                                                                                                  nn_architecture=NNArchitecture.SSNP,
+                                                                                                  load_folder=os.path.join("tmp", "MNIST", "SDBM"),
+                                                                                                  )
+
+    dbm_plotter_gui = DBMPlotterGUI(dbm_model=sdbm,
+                                    img=img,
+                                    img_confidence=img_confidence,
+                                    encoded_train=encoded_training_data,
+                                    encoded_test=encoded_testing_data,
+                                    X_train=X_train,
+                                    Y_train=Y_train,
+                                    X_test=X_test,
+                                    Y_test=Y_test,
+                                    save_folder=os.path.join("tmp", "MNIST", "SDBM"),
                                     )
-    dbm_plotter_gui.start()
+    dbm_plotter_gui.start()
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/__init__.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .DBM_usage_example import DBM_usage_example, DBM_usage_example_GUI
-from .SDBM_usage_example import SDBM_usage_example, SDBM_usage_example_GUI
+from .Logger import Logger, LoggerGUI, LoggerInterface
+from .DBM import DBM, SDBM, NNArchitecture, FAST_DBM_STRATEGIES
+from .GUI import GUI
+from .examples import DBM_usage_example, SDBM_usage_example, DBM_usage_example_GUI, SDBM_usage_example_GUI
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/examples/utils.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
@@ -18,70 +18,77 @@
 import opfython.math.general as g
 import opfython.stream.parser as p
 import opfython.stream.splitter as s
 from opfython.models import SemiSupervisedOPF
 
 from ..utils import import_mnist_dataset
 
+
 def import_data():
     # import the dataset
     (X_train, Y_train), (X_test, Y_test) = import_mnist_dataset()
-    
+
     # if needed perform some preprocessing
     SAMPLES_LIMIT = 5000
     X_train = X_train.astype('float32') / 255
-    X_test = X_test.astype('float32') / 255    
-    X_train, Y_train = X_train[:int(0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
-    X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)], Y_test[:int(0.3*SAMPLES_LIMIT)]
+    X_test = X_test.astype('float32') / 255
+    X_train, Y_train = X_train[:int(
+        0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
+    X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)
+                            ], Y_test[:int(0.3*SAMPLES_LIMIT)]
     return X_train, X_test, Y_train, Y_test
 
+
 def import_classifier():
     # upload a classifier
     # !!! the classifier must be a tf.keras.models.Model !!!
     # !!! change the next line with the path to your classifier !!!
     classifier_path = os.path.join("tmp", "MNIST", "classifier")
     classifier = tf.keras.models.load_model(classifier_path)
     return classifier
 
-def generate_classifier(X_train, Y_train):    
+
+def generate_classifier(X_train, Y_train):
     input_shape = X_train.shape[1:]
-    num_classes = len(np.unique(Y_train))    
-    
+    num_classes = len(np.unique(Y_train))
+
     classifier = tf.keras.models.Sequential([
         tf.keras.layers.Flatten(input_shape=input_shape),
         tf.keras.layers.Dense(num_classes, activation=tf.nn.softmax),
     ])
-    
-    classifier.compile(optimizer='adam', loss='sparse_categorical_crossentropy', metrics=['accuracy'])
+
+    classifier.compile(
+        optimizer='adam', loss='sparse_categorical_crossentropy', metrics=['accuracy'])
     classifier.fit(X_train, Y_train, epochs=20)
     return classifier
-    
+
 
 def opf(X_train, Y_train):
     pr_x = int(0.1*len(X_train))
     pr_y = int(0.1*len(Y_train))
-    X_train, X_unlabeled, Y_train, Y_unlabeled = X_train[:pr_x], X_train[pr_x:], Y_train[:pr_y], Y_train[pr_y:]
+    X_train, X_unlabeled, Y_train, Y_unlabeled = X_train[:
+                                                         pr_x], X_train[pr_x:], Y_train[:pr_y], Y_train[pr_y:]
 
     # Creates a SemiSupervisedOPF instance
-    opf = SemiSupervisedOPF(distance="log_squared_euclidean", pre_computed_distance=None)
+    opf = SemiSupervisedOPF(
+        distance="log_squared_euclidean", pre_computed_distance=None)
 
     # Fits training data along with unlabeled data into the semi-supervised classifier
     opf.fit(X_train, Y_train, X_unlabeled)
-    
+
     # Predicts new data
     preds = opf.predict(X_unlabeled)
-    
+
     # Calculating accuracy
     acc = g.opf_accuracy(Y_unlabeled, preds)
     print(f"OPF Accuracy: {acc}")
 
     return np.hstack((Y_train, preds))
 
 
 def import_2d_data(projection='t-SNE'):
     # upload the 2D projection of the data
     with open(os.path.join("tmp", "MNIST", "DBM", projection, "train_2d.npy"), "rb") as f:
         X2d_train = np.load(f)
     with open(os.path.join("tmp", "MNIST", "DBM", projection, "test_2d.npy"), "rb") as f:
         X2d_test = np.load(f)
     return X2d_train, X2d_test
-
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper/utils/tools.py` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright 2023 Cristian Grosu
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 from .. import LoggerInterface
 
-def track_time_wrapper(logger: LoggerInterface = None):
+
+def track_time_wrapper(logger: LoggerInterface | None = None):
     """ Decorator that tracks the time it takes for a function to run.
 
     Args:
         logger (LoggerInterface): The logger to use. If None, prints to stdout.
     """
     def function_wrapper(func):
         def wrapper(*args, **kwargs):
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/PKG-INFO` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.4.3
+Version: 0.5.0
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
         
         This is the package provides functionality for visualizing the classifiers decision boundaries.
         
         It is based on the work of Cristian Grosu for the master thesis project for 2023 at Utrecht University.
         If you use this package, please cite the following paper:
-        [placeholder for the paper]
+        `[PLACEHOLDER FOR THE PAPER](http://google.com/)`
         
         The package is available on PyPI and can be installed using pip: `pip install decision-boundary-mapper`
         
         ## Documentation
         
         See more details at `https://decisionboundarymapper.000webhostapp.com/`
         
@@ -28,26 +28,25 @@
         from decision_boundary_mapper import GUI
         
         GUI().start()
         ```
         
         2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
         Both examples use `MNIST` (handwritten digits) dataset.
-        The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `DBM_usage_example_2` uses `UMAP` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. After which a simple classifier is used to color each point of the `2D` projection.
-        The second example `SDM_usage_example` uses an Autoencoder Neural Network to project the data from the `nD` space to the `2D` space, then a simple classifier is used to color each point of the `2D` projection.
+        The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
         The examples can be found in the `examples` folder.
         
         ```python
         from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
         
         DBM_usage_example() # run the first example
         SDM_usage_example() # run the second example
         ```
         
-        3. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
+        1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
         The classes can be used as follows:
         
         ```python
         from decision_boundary_mapper import DBM, SDBM
         from matplotlib import pyplot as plt
         
         # load the data
@@ -56,18 +55,18 @@
         ...
         # create a simple neural network
         ...
         classifier = ... # for compatibility with the package the classifier should be constructed using tensorflow.keras
         ...
         
         dbm = DBM(classifier) # create a DBM object
-        img, img_confidence, _, _, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+        img, img_confidence, _, _ = dbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
         
         sdbm = SDBM(classifier) # create a SDBM object
-        img, img_confidence, _, _, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
+        img, img_confidence, _, _ = sdbm.generate_decision_boundary(X_train, y_train, X_test, y_test, resolution = 256) # generate the decision boundary
         ...
         # visualize the decision boundaries
         plt.imshow(img)
         plt.show()
         
         ```
```

### Comparing `decision-boundary-mapper-0.4.3/src/decision_boundary_mapper.egg-info/SOURCES.txt` & `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,38 @@
 setup.py
 src/decision_boundary_mapper/__init__.py
 src/decision_boundary_mapper.egg-info/PKG-INFO
 src/decision_boundary_mapper.egg-info/SOURCES.txt
 src/decision_boundary_mapper.egg-info/dependency_links.txt
 src/decision_boundary_mapper.egg-info/requires.txt
 src/decision_boundary_mapper.egg-info/top_level.txt
-src/decision_boundary_mapper/DBM/DBMInterface.py
-src/decision_boundary_mapper/DBM/NNinterface.py
+src/decision_boundary_mapper/DBM/AbstractDBM.py
+src/decision_boundary_mapper/DBM/AbstractNN.py
 src/decision_boundary_mapper/DBM/__init__.py
 src/decision_boundary_mapper/DBM/tools.py
 src/decision_boundary_mapper/DBM/DBM/DBM.py
+src/decision_boundary_mapper/DBM/DBM/NNInv.py
 src/decision_boundary_mapper/DBM/DBM/__init__.py
-src/decision_boundary_mapper/DBM/DBM/invNN.py
 src/decision_boundary_mapper/DBM/DBM/projections.py
 src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
 src/decision_boundary_mapper/DBM/SDBM/SDBM.py
+src/decision_boundary_mapper/DBM/SDBM/SSNP.py
 src/decision_boundary_mapper/DBM/SDBM/__init__.py
+src/decision_boundary_mapper/GUI/DBMPlotterController.py
 src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
 src/decision_boundary_mapper/GUI/GUI.py
+src/decision_boundary_mapper/GUI/GUIController.py
 src/decision_boundary_mapper/GUI/__init__.py
+src/decision_boundary_mapper/GUI/utils.py
 src/decision_boundary_mapper/Logger/Logger.py
 src/decision_boundary_mapper/Logger/LoggerGUI.py
 src/decision_boundary_mapper/Logger/LoggerInterface.py
 src/decision_boundary_mapper/Logger/LoggerModel.py
 src/decision_boundary_mapper/Logger/__init__.py
 src/decision_boundary_mapper/examples/DBM_usage_example.py
 src/decision_boundary_mapper/examples/SDBM_usage_example.py
 src/decision_boundary_mapper/examples/__init__.py
 src/decision_boundary_mapper/examples/utils.py
 src/decision_boundary_mapper/utils/__init__.py
+src/decision_boundary_mapper/utils/config.py
 src/decision_boundary_mapper/utils/dataReader.py
 src/decision_boundary_mapper/utils/tools.py
```

