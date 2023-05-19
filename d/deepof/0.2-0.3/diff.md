# Comparing `tmp/deepof-0.2.tar.gz` & `tmp/deepof-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepof-0.2.tar", last modified: Tue Mar 28 22:00:55 2023, max compression
+gzip compressed data, was "deepof-0.3.tar", last modified: Fri May 19 23:41:31 2023, max compression
```

## Comparing `deepof-0.2.tar` & `deepof-0.3.tar`

### file list

```diff
@@ -1,31 +1,50 @@
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-03-28 22:00:55.069121 deepof-0.2/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.2/LICENSE
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-28 21:31:36.000000 deepof-0.2/MANIFEST.in
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     7526 2023-03-28 22:00:55.068931 deepof-0.2/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     7021 2023-03-27 23:39:57.000000 deepof-0.2/README.md
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-03-28 22:00:55.051467 deepof-0.2/deepof/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.2/deepof/.DS_Store
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.2/deepof/__init__.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    24490 2023-03-15 13:01:49.000000 deepof-0.2/deepof/annotation_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    97000 2023-03-27 23:55:20.000000 deepof-0.2/deepof/data.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    18169 2023-03-27 23:39:57.000000 deepof-0.2/deepof/deepof_train_embeddings.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8461 2023-03-27 23:39:57.000000 deepof-0.2/deepof/hypermodels.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    60654 2023-03-27 23:39:57.000000 deepof-0.2/deepof/model_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    78975 2023-03-14 08:12:20.000000 deepof-0.2/deepof/models.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    41292 2023-03-27 23:39:57.000000 deepof-0.2/deepof/post_hoc.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-03-28 22:00:55.055694 deepof-0.2/deepof/trained_models/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.2/deepof/trained_models/.gitkeep
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-03-28 22:00:55.058749 deepof-0.2/deepof/trained_models/deepof_supervised/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028  1133126 2023-03-27 23:39:57.000000 deepof-0.2/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl
--rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-27 23:39:57.000000 deepof-0.2/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    54901 2023-03-28 06:27:23.000000 deepof-0.2/deepof/utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    93527 2023-03-27 23:39:57.000000 deepof-0.2/deepof/visuals.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-03-28 22:00:55.054847 deepof-0.2/deepof.egg-info/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     7526 2023-03-28 22:00:55.000000 deepof-0.2/deepof.egg-info/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      616 2023-03-28 22:00:55.000000 deepof-0.2/deepof.egg-info/SOURCES.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-03-28 22:00:55.000000 deepof-0.2/deepof.egg-info/dependency_links.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     4221 2023-03-28 22:00:55.000000 deepof-0.2/deepof.egg-info/requires.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-03-28 22:00:55.000000 deepof-0.2/deepof.egg-info/top_level.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     4014 2023-03-28 20:25:32.000000 deepof-0.2/requirements.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-03-28 22:00:55.069170 deepof-0.2/setup.cfg
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1409 2023-03-28 21:59:37.000000 deepof-0.2/setup.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.696934 deepof-0.3/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.3/LICENSE
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-30 11:55:09.000000 deepof-0.3/MANIFEST.in
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8054 2023-05-19 23:41:31.696753 deepof-0.3/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     7549 2023-05-19 23:29:37.000000 deepof-0.3/README.md
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.665871 deepof-0.3/deepof/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.3/deepof/.DS_Store
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.3/deepof/__init__.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.683150 deepof-0.3/deepof/__pycache__/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      104 2023-03-30 11:25:12.000000 deepof-0.3/deepof/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      153 2023-05-08 08:17:29.000000 deepof-0.3/deepof/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    22213 2023-05-18 15:08:03.000000 deepof-0.3/deepof/__pycache__/annotation_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    71530 2023-05-18 15:50:27.000000 deepof-0.3/deepof/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9319 2023-05-18 15:22:49.000000 deepof-0.3/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8804 2023-04-26 16:06:24.000000 deepof-0.3/deepof/__pycache__/hypermodels.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6353 2023-05-08 08:17:38.000000 deepof-0.3/deepof/__pycache__/hypermodels.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    14803 2023-04-26 16:06:24.000000 deepof-0.3/deepof/__pycache__/model_utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    48080 2023-05-18 14:45:02.000000 deepof-0.3/deepof/__pycache__/model_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9325 2023-04-26 16:06:24.000000 deepof-0.3/deepof/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    49614 2023-05-15 14:00:18.000000 deepof-0.3/deepof/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26124 2023-03-30 11:25:12.000000 deepof-0.3/deepof/__pycache__/pose_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    39561 2023-05-19 08:57:20.000000 deepof-0.3/deepof/__pycache__/post_hoc.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26524 2023-03-30 11:25:12.000000 deepof-0.3/deepof/__pycache__/preprocess.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    37167 2023-04-26 16:06:24.000000 deepof-0.3/deepof/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    50594 2023-05-16 22:09:07.000000 deepof-0.3/deepof/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     4586 2023-04-26 16:06:24.000000 deepof-0.3/deepof/__pycache__/visuals.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    69674 2023-05-18 15:09:24.000000 deepof-0.3/deepof/__pycache__/visuals.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26207 2023-05-18 15:07:58.000000 deepof-0.3/deepof/annotation_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    96978 2023-05-18 15:30:35.000000 deepof-0.3/deepof/data.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    15220 2023-05-08 09:59:43.000000 deepof-0.3/deepof/deepof_train_embeddings.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8274 2023-04-26 16:00:17.000000 deepof-0.3/deepof/hypermodels.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    61556 2023-05-18 14:42:25.000000 deepof-0.3/deepof/model_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    78665 2023-05-15 09:53:25.000000 deepof-0.3/deepof/models.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    48910 2023-05-19 08:27:16.000000 deepof-0.3/deepof/post_hoc.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.684196 deepof-0.3/deepof/trained_models/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.3/deepof/trained_models/.gitkeep
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.686809 deepof-0.3/deepof/trained_models/deepof_supervised/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028  1133126 2023-03-30 11:55:02.000000 deepof-0.3/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-30 11:55:02.000000 deepof-0.3/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    62958 2023-05-16 22:06:15.000000 deepof-0.3/deepof/utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028   100784 2023-05-18 15:07:45.000000 deepof-0.3/deepof/visuals.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-19 23:41:31.668802 deepof-0.3/deepof.egg-info/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8054 2023-05-19 23:41:31.000000 deepof-0.3/deepof.egg-info/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1413 2023-05-19 23:41:31.000000 deepof-0.3/deepof.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-05-19 23:41:31.000000 deepof-0.3/deepof.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      782 2023-05-19 23:41:31.000000 deepof-0.3/deepof.egg-info/requires.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-05-19 23:41:31.000000 deepof-0.3/deepof.egg-info/top_level.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      893 2023-05-19 23:41:15.000000 deepof-0.3/requirements.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-05-19 23:41:31.696980 deepof-0.3/setup.cfg
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1017 2023-05-19 23:27:52.000000 deepof-0.3/setup.py
```

### Comparing `deepof-0.2/LICENSE` & `deepof-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepof-0.2/PKG-INFO` & `deepof-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.2
+Version: 0.3
 Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
 Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
 Author: Lucas Miranda
 Author-email: lucas_miranda@psych.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.2-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.3-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
@@ -33,76 +33,83 @@
 basic social interactions) or to embed your data into a sequence-aware latent space to extract meaningful motifs in an
 unsupervised way! Both of these can be used within the package, for example, to automatically 
 compare user-defined experimental groups.
 
 ### How do I start?
 ##### Installation:
 
-The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof):
+The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof). Create and activate a virtual environment with Python >=3.9 and <3.11, for example using conda:
 
 ```bash
-   pip install deepof
+conda create -n deepof python=3.9
+```
+
+Then, activate the environment and install DeepOF:
+
+```bash
+conda activate deepof
+pip install deepof
 ```
 
 Alternatively, you can download our pre-built [Docker image](https://hub.docker.com/repository/docker/lucasmiranda42/deepof),
 which contains all compatible dependencies:
 
 ```bash
-   # download the latest available image
-   docker pull lucasmiranda42/deepof:latest
-   # run the image in interactive mode, enabling you to open python and import deepof
-   docker run -it lucasmiranda42/deepof
+# download the latest available image
+docker pull lucasmiranda42/deepof:latest
+# run the image in interactive mode, enabling you to open python and import deepof
+docker run -it lucasmiranda42/deepof
 ```
 
 Or use [poetry](https://python-poetry.org/):
 
 ```bash
-   # after installing poetry and clonning the DeepOF repository, just run
-   poetry install # from the main directory
+# after installing poetry and clonning the DeepOF repository, just run
+poetry install # from the main directory
 ```
 
 ##### Before we delve in:
 DeepOF relies heavily on DeepLabCut's output. Thorough tutorials on how to get started with DLC for pose estimation can be found [here](https://www.mousemotorlab.org/deeplabcut).
 Once your videos are processed and tagged, you can use DeepOF to extract and annotate your motion-tracking time-series. While many features in DeepOF can work regardless of the set of labels used, we currently recommend using videos from a top-down perspective, and follow our recommended
 set of labels (which can be found in the full documentation page). A pre-trained model capable of recognizing **C57Bl6** and **CD1** mice can be downloaded from [our repository](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/tree/master/models).
 
 ##### Basic usage:
 
 The main module with which you'll interact is called ```deepof.data```. Let's import it and create a project:
 
 ```python
-   import deepof.data
-   my_deepof_project = deepof.data.Project(
-      project_path=".", # Path where to create project files
-      video_path="/path/to/videos", # Path to DLC tracked videos
-      table_path="/path/to/tables", # Path to DLC output
-      project_name="my_deepof_project", # Name of the current project
-      exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
-    )
+import deepof.data
+my_deepof_project = deepof.data.Project(
+  project_path=".", # Path where to create project files
+  video_path="/path/to/videos", # Path to DLC tracked videos
+  table_path="/path/to/tables", # Path to DLC output
+  project_name="my_deepof_project", # Name of the current project
+  exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
+)
 ```
 
 This command will create a ```deepof.data.Project``` object storing all the necessary information to start. There are
 many parameters that we can set here, but let's stick to the basics for now.
 
 One you have this, you can run you project using the ```.create()``` method, which will do quite a lot of computing under
 the hood (load your data, smooth your trajectories, compute distances, angles, and areas between body parts, and save all
 results to disk). The returned object belongs to the ```deepof.data.Coordinates``` class.
 
 ```python
-   my_project = my_project.create(verbose=True)
+my_project = my_project.create(verbose=True)
 ```
 
 Once you have this, you can do several things! But let's first explore how the results of those computations mentioned
 are stored. To extract trajectories, distances, angles and/or areas, you can respectively type:
 
 ```python
-   my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
-   my_project_dists  = my_project.get_distances(speed=0)
-   my_project_angles = my_project.get_angles(speed=0)
-   my_project_areas = my_project.get_areas(speed=0)
+my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
+my_project_dists  = my_project.get_distances(speed=0)
+my_project_angles = my_project.get_angles(speed=0)
+my_project_areas = my_project.get_areas(speed=0)
 ```
 
 Here, the data are stored as ```deepof.data.table_dict``` instances. These are very similar to python dictionaries
 with experiment IDs as keys and pandas.DataFrame objects as values, with a few extra methods for convenience. Peeping
 into the parameters you see in the code block above, ```center``` centers your data (it can be either a boolean or
 one of the body parts in your model! in which case the coordinate origin will be fixed to the position of that point);
 ```polar``` makes the ```.get_coords()``` method return polar instead of Cartesian coordinates, and ```speed```
@@ -113,23 +120,33 @@
 with our unsupervised methods.
 
 As mentioned above, the two main analyses that you can run are supervised and unsupervised. They are executed by
 the ```.supervised_annotation()``` method, and the ```.deep_unsupervised_embedding()``` methods of the ```deepof.data.Coordinates```
 class, respectively.
 
 ```python
-   supervised_annot = my_project.supervised_annotation()
-   gmvae_embedding  = my_project.deep_unsupervised_embedding()
+supervised_annot = my_project.supervised_annotation()
+gmvae_embedding  = my_project.deep_unsupervised_embedding()
 ```
 
 The former returns a ```deepof.data.TableDict``` object, with a pandas.DataFrame per experiment containing a series of
 annotations. The latter is a bit more complicated: it returns a series of objects that depend on the model selected (we 
 offer three flavours of deep clustering models), and allow for further analysis comparing cluster expression and dynamics.
 
-That's it for this (very basic) introduction. Check out the tutorials [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+That's it for this (very basic) introduction. Check out the tutorials and [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+
+---
+### Issues
+
+If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
+
+---
+### Contributions
+
+We welcome contributions from the community! If you want to contribute to this project, please check out our [contribution guidelines](https://github.com/mlfpm/deepof/blob/master/CONTRIBUTING.md).
 
 ---
 
  This project has received funding from the European Union's Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No.  813533
  <div align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/255px-Flag_of_Europe.svg.png">
 </div>
```

### Comparing `deepof-0.2/README.md` & `deepof-0.3/deepof.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: deepof
+Version: 0.3
+Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
+Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
+Author: Lucas Miranda
+Author-email: lucas_miranda@psych.mpg.de
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.2-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.3-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
@@ -19,76 +33,83 @@
 basic social interactions) or to embed your data into a sequence-aware latent space to extract meaningful motifs in an
 unsupervised way! Both of these can be used within the package, for example, to automatically 
 compare user-defined experimental groups.
 
 ### How do I start?
 ##### Installation:
 
-The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof):
+The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof). Create and activate a virtual environment with Python >=3.9 and <3.11, for example using conda:
+
+```bash
+conda create -n deepof python=3.9
+```
+
+Then, activate the environment and install DeepOF:
 
 ```bash
-   pip install deepof
+conda activate deepof
+pip install deepof
 ```
 
 Alternatively, you can download our pre-built [Docker image](https://hub.docker.com/repository/docker/lucasmiranda42/deepof),
 which contains all compatible dependencies:
 
 ```bash
-   # download the latest available image
-   docker pull lucasmiranda42/deepof:latest
-   # run the image in interactive mode, enabling you to open python and import deepof
-   docker run -it lucasmiranda42/deepof
+# download the latest available image
+docker pull lucasmiranda42/deepof:latest
+# run the image in interactive mode, enabling you to open python and import deepof
+docker run -it lucasmiranda42/deepof
 ```
 
 Or use [poetry](https://python-poetry.org/):
 
 ```bash
-   # after installing poetry and clonning the DeepOF repository, just run
-   poetry install # from the main directory
+# after installing poetry and clonning the DeepOF repository, just run
+poetry install # from the main directory
 ```
 
 ##### Before we delve in:
 DeepOF relies heavily on DeepLabCut's output. Thorough tutorials on how to get started with DLC for pose estimation can be found [here](https://www.mousemotorlab.org/deeplabcut).
 Once your videos are processed and tagged, you can use DeepOF to extract and annotate your motion-tracking time-series. While many features in DeepOF can work regardless of the set of labels used, we currently recommend using videos from a top-down perspective, and follow our recommended
 set of labels (which can be found in the full documentation page). A pre-trained model capable of recognizing **C57Bl6** and **CD1** mice can be downloaded from [our repository](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/tree/master/models).
 
 ##### Basic usage:
 
 The main module with which you'll interact is called ```deepof.data```. Let's import it and create a project:
 
 ```python
-   import deepof.data
-   my_deepof_project = deepof.data.Project(
-      project_path=".", # Path where to create project files
-      video_path="/path/to/videos", # Path to DLC tracked videos
-      table_path="/path/to/tables", # Path to DLC output
-      project_name="my_deepof_project", # Name of the current project
-      exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
-    )
+import deepof.data
+my_deepof_project = deepof.data.Project(
+  project_path=".", # Path where to create project files
+  video_path="/path/to/videos", # Path to DLC tracked videos
+  table_path="/path/to/tables", # Path to DLC output
+  project_name="my_deepof_project", # Name of the current project
+  exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
+)
 ```
 
 This command will create a ```deepof.data.Project``` object storing all the necessary information to start. There are
 many parameters that we can set here, but let's stick to the basics for now.
 
 One you have this, you can run you project using the ```.create()``` method, which will do quite a lot of computing under
 the hood (load your data, smooth your trajectories, compute distances, angles, and areas between body parts, and save all
 results to disk). The returned object belongs to the ```deepof.data.Coordinates``` class.
 
 ```python
-   my_project = my_project.create(verbose=True)
+my_project = my_project.create(verbose=True)
 ```
 
 Once you have this, you can do several things! But let's first explore how the results of those computations mentioned
 are stored. To extract trajectories, distances, angles and/or areas, you can respectively type:
 
 ```python
-   my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
-   my_project_dists  = my_project.get_distances(speed=0)
-   my_project_angles = my_project.get_angles(speed=0)
-   my_project_areas = my_project.get_areas(speed=0)
+my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
+my_project_dists  = my_project.get_distances(speed=0)
+my_project_angles = my_project.get_angles(speed=0)
+my_project_areas = my_project.get_areas(speed=0)
 ```
 
 Here, the data are stored as ```deepof.data.table_dict``` instances. These are very similar to python dictionaries
 with experiment IDs as keys and pandas.DataFrame objects as values, with a few extra methods for convenience. Peeping
 into the parameters you see in the code block above, ```center``` centers your data (it can be either a boolean or
 one of the body parts in your model! in which case the coordinate origin will be fixed to the position of that point);
 ```polar``` makes the ```.get_coords()``` method return polar instead of Cartesian coordinates, and ```speed```
@@ -99,23 +120,33 @@
 with our unsupervised methods.
 
 As mentioned above, the two main analyses that you can run are supervised and unsupervised. They are executed by
 the ```.supervised_annotation()``` method, and the ```.deep_unsupervised_embedding()``` methods of the ```deepof.data.Coordinates```
 class, respectively.
 
 ```python
-   supervised_annot = my_project.supervised_annotation()
-   gmvae_embedding  = my_project.deep_unsupervised_embedding()
+supervised_annot = my_project.supervised_annotation()
+gmvae_embedding  = my_project.deep_unsupervised_embedding()
 ```
 
 The former returns a ```deepof.data.TableDict``` object, with a pandas.DataFrame per experiment containing a series of
 annotations. The latter is a bit more complicated: it returns a series of objects that depend on the model selected (we 
 offer three flavours of deep clustering models), and allow for further analysis comparing cluster expression and dynamics.
 
-That's it for this (very basic) introduction. Check out the tutorials [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+That's it for this (very basic) introduction. Check out the tutorials and [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+
+---
+### Issues
+
+If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
+
+---
+### Contributions
+
+We welcome contributions from the community! If you want to contribute to this project, please check out our [contribution guidelines](https://github.com/mlfpm/deepof/blob/master/CONTRIBUTING.md).
 
 ---
 
  This project has received funding from the European Union's Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No.  813533
  <div align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/255px-Flag_of_Europe.svg.png">
 </div>
```

### Comparing `deepof-0.2/deepof/.DS_Store` & `deepof-0.3/deepof/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.2/deepof/annotation_utils.py` & `deepof-0.3/deepof/annotation_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-"""
-
-Functions and general utilities for supervised pose estimation. See documentation for details
-
-"""
+"""Functions and general utilities for supervised pose estimation. See documentation for details."""
 
 import os
 import pickle
 import warnings
-from typing import Any, List, NewType
+from joblib import delayed, Parallel, parallel_backend
+from typing import Any, List, NewType, Union
 from shapely.geometry import Point, Polygon
 from sklearn.preprocessing import StandardScaler
+from tqdm import tqdm
 
 import cv2
 import numpy as np
 import pandas as pd
 import regex as re
 import sklearn.pipeline
 
@@ -34,29 +32,28 @@
     pos_dframe: pd.DataFrame,
     left: str,
     right: str,
     tol: float,
     arena_abs: int,
     arena_rel: int,
 ) -> np.array:
-    """Returns a boolean array that's True if the specified body parts are closer than tol.
+    """Return a boolean array that's True if the specified body parts are closer than tol.
 
-    Parameters:
-        - pos_dframe (pandas.DataFrame): DLC output as pandas.DataFrame; only applicable
-        to two-animal experiments.
-        - left (string): First member of the potential contact
-        - right (string): Second member of the potential contact
-        - tol (float): maximum distance for which a contact is reported
-        - arena_abs (int): length in mm of the diameter of the real arena
-        - arena_rel (int): length in pixels of the diameter of the arena in the video
+    Args:
+        pos_dframe (pandas.DataFrame): DLC output as pandas.DataFrame; only applicable to two-animal experiments.
+        left (string): First member of the potential contact
+        right (string): Second member of the potential contact
+        tol (float): maximum distance for which a contact is reported
+        arena_abs (int): length in mm of the diameter of the real arena
+        arena_rel (int): length in pixels of the diameter of the arena in the video
 
     Returns:
-        - contact_array (np.array): True if the distance between the two specified points
-        is less than tol, False otherwise"""
+        contact_array (np.array): True if the distance between the two specified points is less than tol, False otherwise
 
+    """
     close_contact = None
 
     if isinstance(right, str):
         close_contact = (
             np.linalg.norm(pos_dframe[left] - pos_dframe[right], axis=1) * arena_abs
         ) / arena_rel < tol
 
@@ -81,32 +78,31 @@
     right1: str,
     right2: str,
     tol: float,
     arena_abs: int,
     arena_rel: int,
     rev: bool = False,
 ) -> np.array:
-    """Returns a boolean array that's True if the specified body parts are closer than tol.
+    """Return a boolean array that's True if the specified body parts are closer than tol.
 
     Parameters:
-        - pos_dframe (pandas.DataFrame): DLC output as pandas.DataFrame; only applicable
-        to two-animal experiments.
-        - left1 (string): First contact point of animal 1
-        - left2 (string): Second contact point of animal 1
-        - right1 (string): First contact point of animal 2
-        - right2 (string): Second contact point of animal 2
-        - tol (float): maximum distance for which a contact is reported
-        - arena_abs (int): length in mm of the diameter of the real arena
-        - arena_rel (int): length in pixels of the diameter of the arena in the video
-        - rev (bool): reverses the default behaviour (nose2tail contact for both mice)
+        pos_dframe (pandas.DataFrame): DLC output as pandas.DataFrame; only applicable to two-animal experiments.
+        left1 (string): First contact point of animal 1
+        left2 (string): Second contact point of animal 1
+        right1 (string): First contact point of animal 2
+        right2 (string): Second contact point of animal 2
+        tol (float): maximum distance for which a contact is reported
+        arena_abs (int): length in mm of the diameter of the real arena
+        arena_rel (int): length in pixels of the diameter of the arena in the video
+        rev (bool): reverses the default behaviour (nose2tail contact for both mice)
 
     Returns:
-        - double_contact (np.array): True if the distance between the two specified points
-        is less than tol, False otherwise"""
+        double_contact (np.array): True if the distance between the two specified points is less than tol, False otherwise
 
+    """
     if rev:
         double_contact = (
             (np.linalg.norm(pos_dframe[right1] - pos_dframe[left2], axis=1) * arena_abs)
             / arena_rel
             < tol
         ) & (
             (np.linalg.norm(pos_dframe[right2] - pos_dframe[left1], axis=1) * arena_abs)
@@ -125,28 +121,30 @@
             < tol
         )
 
     return double_contact
 
 
 def rotate(origin, point, ang):
-    """Auxiliar function to climb_wall and sniff_object. Rotates x,y coordinates over a pivot"""
-
+    """Auxiliar function to climb_wall and sniff_object. Rotates x,y coordinates over a pivot."""
     ox, oy = origin
     px, py = point
 
     qx = ox + np.cos(ang) * (px - ox) - np.sin(ang) * (py - oy)
     qy = oy + np.sin(ang) * (px - ox) + np.cos(ang) * (py - oy)
     return qx, qy
 
 
 def outside_ellipse(x, y, e_center, e_axes, e_angle, threshold=0.0):
-    """Auxiliar function to climb_wall and sniff_object. Returns True if the passed x, y coordinates
-    are outside the ellipse denoted by e_center, e_axes and e_angle, with a certain threshold"""
+    """Auxiliar function to climb_wall and sniff_object.
 
+    Returns True if the passed x, y coordinates
+    are outside the ellipse denoted by e_center, e_axes and e_angle, with a certain threshold
+
+    """
     x, y = rotate(e_center, (x, y), np.radians(e_angle))
 
     term_x = (x - e_center[0]) ** 2 / (e_axes[0] + threshold) ** 2
     term_y = (y - e_center[1]) ** 2 / (e_axes[1] + threshold) ** 2
     return term_x + term_y > 1
 
 
@@ -154,30 +152,28 @@
     arena_type: str,
     arena: np.array,
     pos_dict: pd.DataFrame,
     tol: float,
     nose: str,
     centered_data: bool = False,
 ) -> np.array:
-    """Returns True if the specified mouse is climbing the wall
+    """Return True if the specified mouse is climbing the wall.
 
-    Parameters:
-        - arena_type (str): arena type; must be one of ['polygonal-manual', 'circular-autodetect']
-        - arena (np.array): contains arena location and shape details
-        - pos_dict (table_dict): position over time for all videos in a project
-        - tol (float): minimum tolerance to report a hit
-        - nose (str): indicates the name of the body part representing the nose of
-        the selected animal
-        - arena_dims (int): indicates radius of the real arena in mm
-        - centered_data (bool): indicates whether the input data is centered
+    Args:
+        arena_type (str): arena type; must be one of ['polygonal-manual', 'circular-autodetect']
+        arena (np.array): contains arena location and shape details
+        pos_dict (table_dict): position over time for all videos in a project
+        tol (float): minimum tolerance to report a hit
+        nose (str): indicates the name of the body part representing the nose of the selected animal
+        centered_data (bool): indicates whether the input data is centered
 
     Returns:
-        - climbing (np.array): boolean array. True if selected animal
-        is climbing the walls of the arena"""
+        climbing (np.array): boolean array. True if selected animal is climbing the walls of the arena
 
+    """
     nose = pos_dict[nose]
 
     if arena_type.startswith("circular"):
         center = np.zeros(2) if centered_data else np.array(arena[0])
         axes = arena[1]
         angle = arena[2]
         climbing = outside_ellipse(
@@ -211,33 +207,32 @@
     tol: float,
     tol_speed: float,
     nose: str,
     centered_data: bool = False,
     s_object: str = "arena",
     animal_id: str = "",
 ):
-    """Returns True if the specified mouse is sniffing an object
+    """Return True if the specified mouse is sniffing an object.
 
-    Parameters:
-        - speed_dframe (pandas.DataFrame): speed of body parts over time
-        - arena_type (str): arena type; must be one of ['polygonal-manual', 'circular-autodetect']
-        - arena (np.array): contains arena location and shape details
-        - pos_dict (table_dict): position over time for all videos in a project
-        - tol (float): minimum tolerance to report a hit
-        - nose (str): indicates the name of the body part representing the nose of
-        the selected animal
-        - arena_dims (int): indicates radius of the real arena in mm
-        - centered_data (bool): indicates whether the input data is centered
-        - object (str): indicates the object that the animal is sniffing.
-        Can be one of ['arena', 'partner']
+    Args:
+        speed_dframe (pandas.DataFrame): speed of body parts over time.
+        arena_type (str): arena type; must be one of ['polygonal-manual', 'circular-autodetect'].
+        arena (np.array): contains arena location and shape details.
+        pos_dict (table_dict): position over time for all videos in a project.
+        tol (float): minimum tolerance to report a hit.
+        nose (str): indicates the name of the body part representing the nose of the selected animal.
+        centered_data (bool): indicates whether the input data is centered.
+        s_object (str): indicates the object to sniff. Must be one of ['arena', 'object'].
+        animal_id (str): indicates the animal to sniff. Must be one of animal_ids.
+        tol_speed (float): minimum speed to report a hit.
 
     Returns:
-        - sniffing (np.array): boolean array. True if selected animal
-        is sniffing the selected object"""
+        sniffing (np.array): boolean array. True if selected animal is sniffing the selected object
 
+    """
     nose, nosing = pos_dict[nose], True
 
     if animal_id != "":
         animal_id += "_"
 
     if s_object == "arena":
         if arena_type.startswith("circular"):
@@ -286,71 +281,71 @@
     return sniffing
 
 
 def huddle(
     X_huddle: np.ndarray,
     huddle_estimator: sklearn.pipeline.Pipeline,
 ) -> np.array:
-    """Returns true when the mouse is huddling a pretrained model.
+    """Return true when the mouse is huddling a pretrained model.
 
-    Parameters:
-        - X_huddle (pandas.DataFrame): mouse features over time
-        - huddle_estimator (sklearn.pipeline.Pipeline): pre-trained model to predict feature occurrence
+    Args:
+        X_huddle (pandas.DataFrame): mouse features over time
+        huddle_estimator (sklearn.pipeline.Pipeline): pre-trained model to predict feature occurrence
 
     Returns:
         y_huddle (np.array): 1 if the animal is huddling, 0 otherwise
-    """
 
+    """
     # Concatenate all relevant data frames and predict using the pre-trained estimator
-    y_huddle = huddle_estimator.predict(StandardScaler().fit_transform(X_huddle))
-
+    X_mask = np.isnan(X_huddle).mean(axis=1) == 1
+    y_huddle = huddle_estimator.predict(
+        StandardScaler().fit_transform(np.nan_to_num(X_huddle))
+    )
+    y_huddle[X_mask] = np.nan
     return y_huddle
 
 
 def dig(
     pos_dframe: pd.DataFrame,
     speed_dframe: pd.DataFrame,
     dig_estimator: sklearn.pipeline.Pipeline,
 ):
-    """Returns true when the mouse is digging using a pretrained model.
+    """Return true when the mouse is digging using a pretrained model.
 
-    Parameters:
-        - pos_dframe (pandas.DataFrame): position of body parts over time
-        - speed_dframe (pandas.DataFrame): speed of body parts over time
-        - dig_estimator (sklearn.pipeline.Pipeline): pre-trained model to predict feature occurrence
+    Args:
+        pos_dframe (pandas.DataFrame): position of body parts over time
+        speed_dframe (pandas.DataFrame): speed of body parts over time
+        dig_estimator (sklearn.pipeline.Pipeline): pre-trained model to predict feature occurrence
 
     Returns:
         dig (np.array): True if the animal is digging, False otherwise
     """
-
     # Concatenate all relevant data frames and predict using the pre-trained estimator
     pass
 
 
 def look_around(
     speed_dframe: pd.DataFrame,
     likelihood_dframe: pd.DataFrame,
     tol_speed: float,
     tol_likelihood: float,
     animal_id: str = "",
 ):
-    """Returns true when the mouse is looking around using simple rules.
+    """Return true when the mouse is looking around using simple rules.
 
-    Parameters:
-        - speed_dframe (pandas.DataFrame): speed of body parts over time
-        - likelihood_dframe (pandas.DataFrame): likelihood of body part tracker over time,
-        as directly obtained from DeepLabCut
-        - tol_speed (float): Maximum tolerated speed for the center of the mouse
-        - tol_likelihood (float): Maximum tolerated likelihood for the nose (if the animal
-        is digging, the nose is momentarily occluded).
+    Args:
+        speed_dframe (pandas.DataFrame): speed of body parts over time
+        likelihood_dframe (pandas.DataFrame): likelihood of body part tracker over time, as directly obtained from DeepLabCut
+        tol_speed (float): Maximum tolerated speed for the center of the mouse
+        tol_likelihood (float): Maximum tolerated likelihood for the nose (if the animal is digging, the nose is momentarily occluded).
 
     Returns:
         lookaround (np.array): True if the animal is standing still and looking around, False otherwise
-    """
 
+    """
     if animal_id != "":
         animal_id += "_"
 
     speed = speed_dframe[animal_id + "Center"] < tol_speed
     nose_speed = speed_dframe[animal_id + "Center"] < speed_dframe[animal_id + "Nose"]
     nose_likelihood = likelihood_dframe[animal_id + "Nose"] > tol_likelihood
 
@@ -363,28 +358,30 @@
     distance_dframe: pd.DataFrame,
     position_dframe: pd.DataFrame,
     follower: str,
     followed: str,
     frames: int = 20,
     tol: float = 0,
 ) -> np.array:
-    """For multi animal videos only. Returns True if 'follower' is closer than tol to the path that
-    followed has walked over the last specified number of frames
+    """Return True if 'follower' is closer than tol to the path that followed has walked over the last specified number of frames.
+
+    For multi animal videos only.
 
-        Parameters:
-            - distance_dframe (pandas.DataFrame): distances between bodyparts; generated by the preprocess module
-            - position_dframe (pandas.DataFrame): position of bodyparts; generated by the preprocess module
-            - follower (str) identifier for the animal who's following
-            - followed (str) identifier for the animal who's followed
-            - frames (int) frames in which to track whether the process consistently occurs,
-            - tol (float) Maximum distance for which True is returned
+        Args:
+            distance_dframe (pandas.DataFrame): distances between bodyparts; generated by the preprocess module
+            position_dframe (pandas.DataFrame): position of bodyparts; generated by the preprocess module
+            follower (str) identifier for the animal who's following
+            followed (str) identifier for the animal who's followed
+            frames (int) frames in which to track whether the process consistently occurs,
+            tol (float) Maximum distance for which True is returned
 
         Returns:
-            - follow (np.array): boolean sequence, True if conditions are fulfilled, False otherwise"""
+            follow (np.array): boolean sequence, True if conditions are fulfilled, False otherwise
 
+    """
     # Check that follower is close enough to the path that followed has passed though in the last frames
     shift_dict = {
         i: position_dframe[followed + "_Tail_base"].shift(i) for i in range(frames)
     }
     dist_df = pd.DataFrame(
         {
             i: np.linalg.norm(
@@ -414,49 +411,47 @@
 
     return follow
 
 
 def max_behaviour(
     behaviour_dframe: pd.DataFrame, window_size: int = 10, stepped: bool = False
 ) -> np.array:
-    """Returns the most frequent behaviour in a window of window_size frames
+    """Return the most frequent behaviour in a window of window_size frames.
 
-    Parameters:
-            - behaviour_dframe (pd.DataFrame): boolean matrix containing occurrence
-            of tagged behaviours per frame in the video
-            - window_size (int): size of the window to use when computing
-            the maximum behaviour per time slot
-            - stepped (bool): sliding windows don't overlap if True. False by default
+    Args:
+        behaviour_dframe (pd.DataFrame): boolean matrix containing occurrence of tagged behaviours per frame in the video
+        window_size (int): size of the window to use when computing the maximum behaviour per time slot
+        stepped (bool): sliding windows don't overlap if True. False by default
 
     Returns:
-        - max_array (np.array): string array with the most common behaviour per instance
-        of the sliding window"""
+        max_array (np.array): string array with the most common behaviour per instance of the sliding window
 
+    """
     speeds = [col for col in behaviour_dframe.columns if "speed" in col.lower()]
 
     behaviour_dframe = behaviour_dframe.drop(speeds, axis=1).astype(float)
     win_array = behaviour_dframe.rolling(window_size, center=True).sum()
     if stepped:
         win_array = win_array[::window_size]
     max_array = win_array[1:].idxmax(axis=1)
 
     return np.array(max_array)
 
 
 # noinspection PyDefaultArgument
 def get_hparameters(hparams: dict = {}) -> dict:
-    """Returns the most frequent behaviour in a window of window_size frames
+    """Return the most frequent behaviour in a window of window_size frames.
 
-    Parameters:
-        - hparams (dict): dictionary containing hyperparameters to overwrite
+    Args:
+        hparams (dict): dictionary containing hyperparameters to overwrite
 
     Returns:
-        - defaults (dict): dictionary with overwritten parameters. Those not
-        specified in the input retain their default values"""
+        defaults (dict): dictionary with overwritten parameters. Those not specified in the input retain their default values
 
+    """
     defaults = {
         "speed_pause": 5,
         "climb_tol": 10,
         "close_contact_tol": 25,
         "side_contact_tol": 45,
         "follow_frames": 10,
         "follow_tol": 5,
@@ -468,25 +463,25 @@
         defaults[k] = v
 
     return defaults
 
 
 # noinspection PyDefaultArgument
 def frame_corners(w, h, corners: dict = {}):
-    """Returns a dictionary with the corner positions of the video frame
+    """Return a dictionary with the corner positions of the video frame.
 
-    Parameters:
-        - w (int): width of the frame in pixels
-        - h (int): height of the frame in pixels
-        - corners (dict): dictionary containing corners to overwrite
+    Args:
+        w (int): width of the frame in pixels
+        h (int): height of the frame in pixels
+        corners (dict): dictionary containing corners to overwrite
 
     Returns:
-        - defaults (dict): dictionary with overwriten parameters. Those not
-        specified in the input retain their default values"""
+        defaults (dict): dictionary with overwriten parameters. Those not specified in the input retain their default values
 
+    """
     defaults = {
         "downleft": (int(w * 0.3 / 10), int(h / 1.05)),
         "downright": (int(w * 6.5 / 10), int(h / 1.05)),
         "upleft": (int(w * 0.3 / 10), int(h / 20)),
         "upright": (int(w * 6.3 / 10), int(h / 20)),
     }
 
@@ -504,33 +499,33 @@
     dists: table_dict,
     speeds: table_dict,
     full_features: dict,
     video: str,
     trained_model_path: str = None,
     params: dict = {},
 ) -> pd.DataFrame:
-    """Outputs a dataframe with the registered motives per frame. If specified, produces a labeled
-    video displaying the information in real time
+    """Output a dataframe with the registered motives per frame.
 
-    Parameters:
-        - coord_object (deepof.data.coordinates): coordinates object containing the project information
-        - raw_coords (deepof.data.table_dict): table_dict with raw coordinates
-        - coords (deepof.data.table_dict): table_dict with already processed (centered and aligned) coordinates
-        - dists (deepof.data.table_dict): table_dict with already processed distances
-        - speeds (deepof.data.table_dict): table_dict with already processed speeds
-        - full_features (dict): dictionary with
-        - video (str): string name of the experiment to tag
-        - trained_model_path (str): path indicating where all pretrained models are located
-        - params (dict): dictionary to overwrite the default values of the parameters of the functions
-        that the rule-based pose estimation utilizes. See documentation for details.
+    If specified, produces a labeled video displaying the information in real time
+
+    Args:
+        coord_object (deepof.data.coordinates): coordinates object containing the project information
+        raw_coords (deepof.data.table_dict): table_dict with raw coordinates
+        coords (deepof.data.table_dict): table_dict with already processed (centered and aligned) coordinates
+        dists (deepof.data.table_dict): table_dict with already processed distances
+        speeds (deepof.data.table_dict): table_dict with already processed speeds
+        full_features (dict): dictionary with
+        video (str): string name of the experiment to tag
+        trained_model_path (str): path indicating where all pretrained models are located
+        params (dict): dictionary to overwrite the default values of the parameters of the functions that the rule-based pose estimation utilizes. See documentation for details.
 
     Returns:
-        - tag_df (pandas.DataFrame): table with traits as columns and frames as rows. Each
-        value is a boolean indicating trait detection at a given time"""
+        tag_df (pandas.DataFrame): table with traits as columns and frames as rows. Each value is a boolean indicating trait detection at a given time
 
+    """
     # Load pre-trained models for ML annotated traits
     with open(
         os.path.join(
             trained_model_path,
             "deepof_supervised",
             "deepof_supervised_huddle_estimator.pkl",
         ),
@@ -550,15 +545,14 @@
     # Extract useful information from coordinates object
     tracks = list(coord_object._tables.keys())
     vid_index = coord_object._videos.index(video)
 
     arena_params = coord_object._arena_params[vid_index]
     arena_type = coord_object._arena
 
-    params = get_hparameters(params)
     animal_ids = coord_object._animal_ids
     undercond = "_" if len(animal_ids) > 1 else ""
 
     try:
         vid_name = re.findall("(.*?)DLC", tracks[vid_index])[0]
     except IndexError:
         vid_name = tracks[vid_index]
@@ -586,15 +580,15 @@
         "Left_fhip",
         "Right_fhip",
         "Left_bhip",
         "Right_bhip",
     ]
 
     def onebyone_contact(bparts: List):
-        """Returns a smooth boolean array with 1to1 contacts between two mice"""
+        """Return a smooth boolean array with 1to1 contacts between two mice."""
         nonlocal raw_coords, animal_ids, params, arena_abs, arena_params
 
         try:
             left = animal_ids[0] + bparts[0]
         except TypeError:
             left = [animal_ids[0] + "_" + suffix for suffix in bparts[0]]
 
@@ -611,16 +605,15 @@
                 params["close_contact_tol"],
                 arena_abs,
                 arena_rel,
             )
         )
 
     def twobytwo_contact(rev):
-        """Returns a smooth boolean array with side by side contacts between two mice"""
-
+        """Return a smooth boolean array with side by side contacts between two mice."""
         nonlocal raw_coords, animal_ids, params, arena_abs, arena_params
         return deepof.utils.smooth_boolean_array(
             close_double_contact(
                 raw_coords,
                 animal_ids[0] + "_Nose",
                 animal_ids[0] + "_Tail_base",
                 animal_ids[1] + "_Nose",
@@ -629,14 +622,15 @@
                 rev=rev,
                 arena_abs=arena_abs,
                 arena_rel=arena_rel,
             )
         )
 
     def overall_speed(ovr_speeds, _id, ucond):
+        """Return the overall speed of a mouse."""
         bparts = [
             "Center",
             "Spine_1",
             "Spine_2",
             "Nose",
             "Left_ear",
             "Right_ear",
@@ -724,10 +718,58 @@
         tag_dict[_id + undercond + "speed"] = overall_speed(speeds, _id, undercond)
 
     tag_df = pd.DataFrame(tag_dict).fillna(0).astype(float)
 
     return tag_df
 
 
+def tagged_video_output(
+    coordinates: coordinates,
+    tag_dict: table_dict,
+    video_output: Union[str, List[str]] = "all",
+    frame_limit: int = None,
+    debug: bool = False,
+    n_jobs: int = 1,
+    params: dict = None,
+):  # pragma: no cover
+    """Output annotated videos.
+
+    Args:
+        coordinates: Coordinates object.
+        tag_dict: Dictionary with supervised annotations to render on the video.
+        video_output: List with the names of the videos to render, or 'all' (default) to render all videos.
+        frame_limit: Number of frames to render per output video. If None, all frames are rendered.
+        debug: If True, debugging information, such as arena fits and processed tracklets, are displayed.
+        n_jobs: Number of jobs to run in parallel.
+        params (dict): dictionary to overwrite the default values of the hyperparameters of the functions that the supervised pose estimation utilizes.
+    """
+
+    def output_video(idx):
+        """Output a single annotated video. Enclosed in a function to enable parallelization."""
+        deepof.visuals.annotate_video(
+            coordinates,
+            tag_dict=tag_dict[idx],
+            vid_index=list(coordinates._tables.keys()).index(idx),
+            debug=debug,
+            frame_limit=frame_limit,
+            params=params,
+        )
+        pbar.update(1)
+
+    if isinstance(video_output, list):
+        vid_idxs = video_output
+    elif video_output == "all":
+        vid_idxs = list(coordinates._tables.keys())
+    else:
+        raise AttributeError(
+            "Video output must be either 'all' or a list with the names of the videos to render"
+        )
+
+    pbar = tqdm(total=len(vid_idxs))
+    with parallel_backend("threading", n_jobs=n_jobs):
+        Parallel()(delayed(output_video)(key) for key in vid_idxs)
+    pbar.close()
+
+
 if __name__ == "__main__":
     # Ignore warnings with no downstream effect
     warnings.filterwarnings("ignore", message="All-NaN slice encountered")
```

### Comparing `deepof-0.2/deepof/data.py` & `deepof-0.3/deepof/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,30 @@
 """
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
 
 from collections import defaultdict
-from joblib import delayed, Parallel, parallel_backend
 from pkg_resources import resource_filename
 from shapely.geometry import Polygon
+from shutil import rmtree
 from sklearn import random_projection
 from sklearn.decomposition import KernelPCA
-from sklearn.experimental import enable_iterative_imputer  # noqa
-from sklearn.impute import IterativeImputer
 from sklearn.manifold import TSNE
 from sklearn.preprocessing import (
     MinMaxScaler,
     StandardScaler,
     RobustScaler,
     LabelEncoder,
 )
 from time import time
 from tqdm import tqdm
 from typing import Any, NewType, Union
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Any
 import copy
 import datetime
 import math
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import os
@@ -60,79 +58,80 @@
 coordinates = NewType("deepof_coordinates", Any)
 table_dict = NewType("deepof_table_dict", Any)
 
 
 # CLASSES FOR PREPROCESSING AND DATA WRANGLING
 
 
-def load_project(project_path: str) -> coordinates:
-    """Loads a pre-saved pickled Coordinates object.
+def load_project(project_path: str) -> coordinates:  # pragma: no cover
+    """Load a pre-saved pickled Coordinates object.
 
     Args:
         project_path (str): name of the file to load.
 
     Returns:
         Pre-run coordinates object.
 
     """
     with open(
         os.path.join(project_path, "Coordinates", "deepof_coordinates.pkl"), "rb"
     ) as handle:
-        return pickle.load(handle)
+        coordinates = pickle.load(handle)
+
+    coordinates._project_path = os.path.split(project_path)[0]
+    return coordinates
 
 
 class Project:
     """Class for loading and preprocessing DLC data of individual and multiple animals.
 
     All main computations are handled from here.
 
     """
 
     def __init__(
         self,
-        animal_ids: List = [""],
+        animal_ids: List = None,
         arena: str = "polygonal-manual",
-        enable_iterative_imputation: bool = True,
+        bodypart_graph: str = "deepof_14",
+        enable_iterative_imputation: bool = 250,
         exclude_bodyparts: List = tuple([""]),
         exp_conditions: dict = None,
         interpolate_outliers: bool = True,
         interpolation_limit: int = 5,
         interpolation_std: int = 3,
         likelihood_tol: float = 0.75,
         model: str = "mouse_topview",
         project_name: str = "deepof_project",
-        project_path: str = deepof.utils.os.path.join("."),
+        project_path: str = os.path.join("."),
         video_path: str = None,
         table_path: str = None,
         smooth_alpha: float = 1,
         table_format: str = "autodetect",
         video_format: str = ".mp4",
         video_scale: int = 1,
     ):
-        """Initializes a Project object.
+        """Initialize a Project object.
 
         Args:
             animal_ids (list): list of animal ids.
             arena (str): arena type. Can be one of "circular-autodetect", "circular-manual", or "polygon-manual".
-            enable_iterative_imputation (bool): whether to use iterative imputation for occluded body parts.
-            Recommended, but slow.
+            bodypart_graph (str): body part scheme to use for the analysis. Defaults to None, in which case the program will attempt to select it automatically based on the available body parts.
+            enable_iterative_imputation (bool): whether to use iterative imputation for occluded body parts. Recommended if several animals are present, but slower.
             exclude_bodyparts (list): list of bodyparts to exclude from analysis.
             exp_conditions (dict): dictionary with experiment IDs as keys and experimental conditions as values.
             interpolate_outliers (bool): whether to interpolate missing data.
             interpolation_limit (int): maximum number of missing frames to interpolate.
             interpolation_std (int): maximum number of standard deviations to interpolate.
             likelihood_tol (float): likelihood threshold for outlier detection.
-            model (str): model to use for pose estimation. Defaults to 'mouse_topview' (as described in the
-            documentation).
+            model (str): model to use for pose estimation. Defaults to 'mouse_topview' (as described in the documentation).
             project_name (str): name of the current project.
             project_path (str): path to the folder containing the DLC output data.
-            video_path (str): path where to find the videos to use. If not specified, deepof, assumes they are in your
-            project path.
-            table_path (str): path where to find the tracks to use. If not specified, deepof, assumes they are in your
-            project path.
+            video_path (str): path where to find the videos to use. If not specified, deepof, assumes they are in your project path.
+            table_path (str): path where to find the tracks to use. If not specified, deepof, assumes they are in your project path.
             smooth_alpha (float): smoothing intensity. The higher the value, the more smoothing.
             table_format (str): format of the table. Defaults to 'autodetect', but can be set to "csv" or "h5".
             video_format (str): video format. Defaults to '.mp4'.
             video_scale (int): diameter of the arena in mm (if the arena is round) or length of the first specified arena side (if the arena is polygonal).
 
         """
         # Set working paths
@@ -144,43 +143,44 @@
 
         # Detect files to load from disk
         self.table_format = table_format
         if self.table_format == "autodetect":
             ex = [i for i in os.listdir(self.table_path) if not i.startswith(".")][0]
             if ".h5" in ex:
                 self.table_format = ".h5"
-            elif ".csv" in ex:
+            elif ".csv" in ex:  # pragma: no cover
                 self.table_format = ".csv"
         self.videos = sorted(
             [
                 vid
-                for vid in deepof.utils.os.listdir(self.video_path)
+                for vid in os.listdir(self.video_path)
                 if vid.endswith(video_format) and not vid.startswith(".")
             ]
         )
         self.tables = sorted(
             [
                 tab
-                for tab in deepof.utils.os.listdir(self.table_path)
+                for tab in os.listdir(self.table_path)
                 if tab.endswith(self.table_format) and not tab.startswith(".")
             ]
         )
         assert len(self.videos) == len(
             self.tables
         ), "Unequal number of videos and tables. Please check your file structure"
 
         # Loads arena details and (if needed) detection models
         self.arena = arena
         self.arena_dims = video_scale
         self.ellipse_detection = None
 
         # Set the rest of the init parameters
         self.angles = True
-        self.animal_ids = animal_ids
+        self.animal_ids = animal_ids if animal_ids is not None else [""]
         self.areas = True
+        self.bodypart_graph = bodypart_graph
         self.connectivity = None
         self.distances = "all"
         self.ego = False
         self.exp_conditions = exp_conditions
         self.interpolate_outliers = interpolate_outliers
         self.interpolation_limit = interpolation_limit
         self.interpolation_std = interpolation_std
@@ -189,24 +189,23 @@
         self.smooth_alpha = smooth_alpha
         self.frame_rate = None
         self.video_format = video_format
         self.enable_iterative_imputation = enable_iterative_imputation
         self.exclude_bodyparts = exclude_bodyparts
 
     def __str__(self):  # pragma: no cover
-        """Prints the object to stdout."""
+        """Print the object to stdout."""
         return "deepof analysis of {} videos".format(len(self.videos))
 
     def __repr__(self):  # pragma: no cover
-        """Prints the object to stdout."""
+        """Print the object to stdout."""
         return "deepof analysis of {} videos".format(len(self.videos))
 
     def set_up_project_directory(self):
-        """Creates a project directory where to save all produced results."""
-
+        """Create a project directory where to save all produced results."""
         # Create a project directory, as well as subfolders for videos and tables
         project_path = os.path.join(self.project_path, self.project_name)
 
         if (
             len(
                 [
                     i
@@ -214,28 +213,28 @@
                     if i.endswith(self.video_format)
                 ]
             )
             == 0
         ):
             raise FileNotFoundError(
                 "There are no compatible videos in the specified directory."
-            )
+            )  # pragma: no cover
         if (
             len(
                 [
                     i
                     for i in os.listdir(self.table_path)
                     if i.endswith(self.table_format)
                 ]
             )
             == 0
         ):
             raise FileNotFoundError(
                 "There are no compatible tracks in the specified directory."
-            )
+            )  # pragma: no cover
 
         if not os.path.exists(project_path):
             os.makedirs(project_path)
             os.makedirs(os.path.join(self.project_path, self.project_name, "Videos"))
             os.makedirs(os.path.join(self.project_path, self.project_name, "Tables"))
             os.makedirs(
                 os.path.join(self.project_path, self.project_name, "Coordinates")
@@ -268,15 +267,15 @@
             self.table_path = os.path.join(
                 self.project_path, self.project_name, "Tables"
             )
 
         else:
             raise OSError(
                 "Project already exists. Delete it or specify a different name."
-            )
+            )  # pragma: no cover
 
     @property
     def distances(self):
         """List. If not 'all', sets the body parts among which the distances will be computed."""
         return self._distances
 
     @property
@@ -285,161 +284,78 @@
         return self._ego
 
     @property
     def angles(self):
         """Bool. Toggles angle computation. True by default. If turned off, enhances performance for big datasets."""
         return self._angles
 
-    def get_arena(self, tables, verbose=False) -> np.array:
-        """Returns the arena as recognised from the videos.
+    def get_arena(self, tables: list, verbose: bool = False) -> np.array:
+        """Return the arena as recognised from the videos.
 
         Args:
             tables (list): list of coordinate tables
             verbose (bool): if True, logs to console
 
         Returns:
             arena (np.ndarray): arena parameters, as recognised from the videos. The shape depends on the arena type
 
         """
         if verbose:
             print("Detecting arena...")
 
-        scales = []
-        arena_params = []
-        video_resolution = []
-
-        def get_first_length(arena_corners):
-            return math.dist(arena_corners[0], arena_corners[1])
-
-        if self.arena in ["polygonal-manual", "circular-manual"]:  # pragma: no cover
-
-            for i, video_path in enumerate(self.videos):
-                arena_corners, h, w = deepof.utils.extract_polygonal_arena_coordinates(
-                    os.path.join(
-                        self.project_path, self.project_name, "Videos", video_path
-                    ),
-                    self.arena,
-                    i,
-                    self.videos,
-                )
-
-                cur_scales = [
-                    *np.mean(arena_corners, axis=0).astype(int),
-                    get_first_length(arena_corners),
-                    self.arena_dims,
-                ]
-
-                cur_arena_params = arena_corners
-
-                if self.arena == "circular-manual":
-                    cur_arena_params = deepof.utils.fit_ellipse_to_polygon(
-                        cur_arena_params
-                    )
-
-                    scales.append(
-                        list(
-                            np.array(
-                                [
-                                    cur_arena_params[0][0],
-                                    cur_arena_params[0][1],
-                                    np.mean(
-                                        [cur_arena_params[1][0], cur_arena_params[1][1]]
-                                    )
-                                    * 2,
-                                ]
-                            )
-                        )
-                        + [self.arena_dims]
-                    )
-                else:
-                    scales.append(cur_scales)
-
-                arena_params.append(cur_arena_params)
-                video_resolution.append((h, w))
-
-        elif self.arena in ["circular-autodetect"]:
-
-            for vid_index, _ in enumerate(self.videos):
-                ellipse, h, w = deepof.utils.automatically_recognize_arena(
-                    videos=self.videos,
-                    tables=tables,
-                    vid_index=vid_index,
-                    path=self.video_path,
-                    arena_type=self.arena,
-                )
-
-                # scales contains the coordinates of the center of the arena,
-                # the absolute diameter measured from the video in pixels, and
-                # the provided diameter in mm (1 -default- equals not provided)
-                scales.append(
-                    list(
-                        np.array(
-                            [
-                                ellipse[0][0],
-                                ellipse[0][1],
-                                np.mean([ellipse[1][0], ellipse[1][1]]) * 2,
-                            ]
-                        )
-                    )
-                    + [self.arena_dims]
-                )
-                arena_params.append(ellipse)
-                video_resolution.append((h, w))
-
-        elif not self.arena:
-            return None, None, None
-
-        else:
-            raise NotImplementedError(
-                "arenas must be set to one of: 'polygonal-manual', 'circular-autodetect'"
-            )
-
-        return np.array(scales), arena_params, video_resolution
+        return deepof.utils.get_arenas(
+            self.arena,
+            self.arena_dims,
+            self.project_path,
+            self.project_name,
+            tables,
+            self.videos,
+        )
 
-    def load_tables(self, verbose: bool = True) -> deepof.utils.Tuple:
-        """Loads videos and tables into dictionaries.
+    def load_tables(self, verbose: bool = True) -> Tuple:
+        """Load videos and tables into dictionaries.
 
         Args:
             verbose (bool): If True, prints the progress of data loading.
 
         Returns:
             Tuple: A tuple containing the following a dictionary with all loaded tables per experiment,
             and another dictionary with DLC data quality.
 
         """
         if self.table_format not in [".h5", ".csv"]:
             raise NotImplementedError(
                 "Tracking files must be in either h5 or csv format"
-            )
+            )  # pragma: no cover
 
         if verbose:
             print("Loading trajectories...")
 
         tab_dict = {}
 
         if self.table_format == ".h5":
 
             tab_dict = {}
             for tab in self.tables:
                 loaded_tab = pd.read_hdf(
-                    deepof.utils.os.path.join(self.table_path, tab), dtype=float
+                    os.path.join(self.table_path, tab), dtype=float
                 )
 
                 # Adapt index to be compatible with downstream processing
                 loaded_tab = loaded_tab.T.reset_index(drop=False).T
                 loaded_tab.columns = loaded_tab.loc["scorer", :]
                 loaded_tab = loaded_tab.iloc[1:]
 
                 tab_dict[deepof.utils.re.findall("(.*?)DLC", tab)[0]] = loaded_tab
 
         elif self.table_format == ".csv":
 
             tab_dict = {
                 deepof.utils.re.findall("(.*?)DLC", tab)[0]: pd.read_csv(
-                    deepof.utils.os.path.join(self.table_path, tab),
+                    os.path.join(self.table_path, tab),
                     index_col=0,
                     low_memory=False,
                 )
                 for tab in self.tables
             }
 
         # Check in the files come from a multi-animal DLC project
@@ -463,16 +379,18 @@
                 [tab.iloc[i] for i in range(2)]
             )
             tab_copy = tab_copy.iloc[2:].astype(float)
             tab_dict[key] = tab_copy.reset_index(drop=True)
 
         # Update body part connectivity graph, taking detected or specified body parts into account
         model_dict = {
-            "{}mouse_topview".format(aid): deepof.utils.connect_mouse_topview(
-                aid, exclude_bodyparts=self.exclude_bodyparts
+            "{}mouse_topview".format(aid): deepof.utils.connect_mouse(
+                aid,
+                exclude_bodyparts=self.exclude_bodyparts,
+                graph_preset=self.bodypart_graph,
             )
             for aid in self.animal_ids
         }
         self.connectivity = {
             aid: model_dict[aid + self.model] for aid in self.animal_ids
         }
 
@@ -500,14 +418,16 @@
             x = tab.xs("x", level="coords", axis=1, drop_level=False)
             y = tab.xs("y", level="coords", axis=1, drop_level=False)
             lik = tab.xs("likelihood", level="coords", axis=1, drop_level=True)
 
             tab_dict[key] = pd.concat([x, y], axis=1).sort_index(axis=1)
             lik_dict[key] = lik.fillna(0.0)
 
+        lik_dict = TableDict(lik_dict, typ="quality", animal_ids=self.animal_ids)
+
         if self.smooth_alpha:
 
             if verbose:
                 print("Smoothing trajectories...")
 
             for key, tab in tab_dict.items():
                 cur_idx = tab.index
@@ -547,43 +467,23 @@
                 )
 
         if self.enable_iterative_imputation:
 
             if verbose:
                 print("Iterative imputation of ocluded bodyparts...")
 
-            for k, tab in tab_dict.items():
-
-                scaler = StandardScaler()
-                imputed = IterativeImputer(
-                    skip_complete=True,
-                    max_iter=self.enable_iterative_imputation,
-                    n_nearest_features=tab.shape[1] // len(self.animal_ids) - 1,
-                    tol=1e-1,
-                ).fit_transform(scaler.fit_transform(tab))
-                imputed = pd.DataFrame(
-                    scaler.inverse_transform(imputed),
-                    index=tab.index,
-                    columns=tab.loc[:, tab.isnull().mean(axis=0) != 1.0].columns,
-                )
+            tab_dict = deepof.utils.iterative_imputation(self, tab_dict, lik_dict)
 
-                tab.update(imputed)
-                tab_dict[k] = tab
-
-                if tab.shape != imputed.shape:
-                    warnings.warn(
-                        "Some of the body parts have zero measurements. Iterative imputation skips these,"
-                        " which could bring problems downstream. A possible solution could be to refine "
-                        "DLC tracklets."
-                    )
+        # Set table_dict to NaN if animals are missing
+        tab_dict = deepof.utils.set_missing_animals(self, tab_dict, lik_dict)
 
         return tab_dict, lik_dict
 
     def get_distances(self, tab_dict: dict, verbose: bool = True) -> dict:
-        """Computes the distances between all selected body parts over time. If ego is provided, it only returns distances to a specified bodypart.
+        """Compute the distances between all selected body parts over time. If ego is provided, it only returns distances to a specified bodypart.
 
         Args:
             tab_dict (dict): Dictionary of pandas DataFrames containing the trajectories of all bodyparts.
             verbose (bool): If True, prints progress. Defaults to True.
 
         Returns:
             dict: Dictionary of pandas DataFrames containing the distances between all bodyparts.
@@ -621,15 +521,15 @@
         # Restore original index
         for key in distance_dict.keys():
             distance_dict[key].index = tab_dict[key].index
 
         return distance_dict
 
     def get_angles(self, tab_dict: dict, verbose: bool = True) -> dict:
-        """Computes all the angles between adjacent bodypart trios per video and per frame in the data.
+        """Compute all the angles between adjacent bodypart trios per video and per frame in the data.
 
         Args:
             tab_dict (dict): Dictionary of pandas DataFrames containing the trajectories of all bodyparts.
             verbose (bool): If True, prints progress. Defaults to True.
 
         Returns:
             dict: Dictionary of pandas DataFrames containing the distances between all bodyparts.
@@ -671,15 +571,15 @@
         # Restore original index
         for key in angle_dict.keys():
             angle_dict[key].index = tab_dict[key].index
 
         return angle_dict
 
     def get_areas(self, tab_dict: dict, verbose: bool = True) -> dict:
-        """Computes all relevant areas (head, torso, back) per video and per frame in the data.
+        """Compute all relevant areas (head, torso, back) per video and per frame in the data.
 
         Args:
             tab_dict (dict): Dictionary of pandas DataFrames containing the trajectories of all bodyparts.
             verbose (bool): If True, prints progress. Defaults to True.
 
         Returns:
             dict: Dictionary of pandas DataFrames containing the distances between all bodyparts.
@@ -690,53 +590,59 @@
 
         areas_dict = {}
 
         for key, tab in tab_dict.items():
 
             exp_table = pd.DataFrame()
 
-            for id in self.animal_ids:
+            for aid in self.animal_ids:
 
-                if id == "":
-                    id = None
+                if aid == "":
+                    aid = None
 
                 # get the current table for the current animal
-                current_table = tab.loc[:, deepof.utils.filter_columns(tab.columns, id)]
+                current_table = tab.loc[
+                    :, deepof.utils.filter_columns(tab.columns, aid)
+                ]
                 current_table = current_table.apply(
-                    lambda x: deepof.utils.compute_areas(x, animal_id=id), axis=1
+                    lambda x: deepof.utils.compute_areas(x, animal_id=aid), axis=1
                 )
                 current_table = pd.DataFrame(
                     current_table.to_list(),
                     index=current_table.index,
                     columns=["head_area", "torso_area", "back_area", "full_area"],
                 ).add_prefix(
                     "{}{}".format(
-                        (id if id is not None else ""), ("_" if id is not None else "")
+                        (aid if aid is not None else ""),
+                        ("_" if aid is not None else ""),
                     )
                 )
 
                 exp_table = pd.concat([exp_table, current_table], axis=1)
 
             areas_dict[key] = exp_table
 
         return areas_dict
 
-    def create(self, verbose: bool = True) -> coordinates:
-        """Generates a deepof.Coordinates dataset using all the options specified during initialization.
+    def create(self, verbose: bool = True, force: bool = False) -> coordinates:
+        """Generate a deepof.Coordinates dataset using all the options specified during initialization.
 
         Args:
             verbose (bool): If True, prints progress. Defaults to True.
 
         Returns:
             coordinates: Deepof.Coordinates object containing the trajectories of all bodyparts.
 
         """
-
         if verbose:
             print("Setting up project directories...")
+
+        if force and os.path.exists(os.path.join(self.project_path, self.project_name)):
+            rmtree(os.path.join(self.project_path, self.project_name))
+
         self.set_up_project_directory()
         self.frame_rate = int(
             np.round(
                 pims.ImageIOReader(
                     os.path.join(self.video_path, self.videos[0])
                 ).frame_rate
             )
@@ -770,14 +676,15 @@
             project_path=self.project_path,
             project_name=self.project_name,
             angles=angles,
             animal_ids=self.animal_ids,
             areas=areas,
             arena=self.arena,
             arena_dims=self.arena_dims,
+            bodypart_graph=self.bodypart_graph,
             distances=distances,
             connectivity=self.connectivity,
             excluded_bodyparts=self.exclude_bodyparts,
             frame_rate=self.frame_rate,
             exp_conditions=self.exp_conditions,
             path=self.project_path,
             quality=quality,
@@ -786,23 +693,15 @@
             tables=tables,
             trained_model_path=self.trained_path,
             videos=self.videos,
             video_resolution=self.video_resolution,
         )
 
         # Save created coordinates to the project directory
-        coords.save(
-            filename=os.path.join(
-                self.project_path,
-                self.project_name,
-                "Coordinates",
-                "deepof_coordinates",
-            ),
-            timestamp=False,
-        )
+        coords.save(timestamp=False)
 
         if verbose:
             print("Done!")
 
         return coords
 
     @distances.setter
@@ -823,14 +722,15 @@
 
     def __init__(
         self,
         project_path: str,
         project_name: str,
         arena: str,
         arena_dims: np.array,
+        bodypart_graph: str,
         path: str,
         quality: dict,
         scales: np.ndarray,
         frame_rate: int,
         arena_params: List,
         tables: dict,
         trained_model_path: str,
@@ -847,14 +747,15 @@
         """Class for storing the results of a ran project. Methods are mostly setters and getters in charge of tidying up the generated tables.
 
         Args:
             project_name (str): name of the current project.
             project_path (str): path to the folder containing the DLC output data.
             arena (str): Type of arena used for the experiment. See deepof.data.Project for more information.
             arena_dims (np.array): Dimensions of the arena. See deepof.data.Project for more information.
+            bodypart_graph (nx.Graph): Graph containing the body part connectivity. See deepof.data.Project for more information.
             path (str): Path to the folder containing the results of the experiment.
             quality (dict): Dictionary containing the quality of the experiment. See deepof.data.Project for more information.
             scales (np.ndarray): Scales used for the experiment. See deepof.data.Project for more information.
             frame_rate (int): frame rate of the processed videos.
             arena_params (List): List containing the parameters of the arena. See deepof.data.Project for more information.
             tables (dict): Dictionary containing the tables of the experiment. See deepof.data.Project for more information.
             trained_model_path (str): Path to the trained models used for the supervised pipeline. For internal use only.
@@ -870,14 +771,15 @@
         """
         self._project_path = project_path
         self._project_name = project_name
         self._animal_ids = animal_ids
         self._arena = arena
         self._arena_params = arena_params
         self._arena_dims = arena_dims
+        self._bodypart_graph = bodypart_graph
         self._excluded = excluded_bodyparts
         self._exp_conditions = exp_conditions
         self._frame_rate = frame_rate
         self._path = path
         self._quality = quality
         self._scales = scales
         self._tables = tables
@@ -886,48 +788,43 @@
         self._video_resolution = video_resolution
         self._angles = angles
         self._areas = areas
         self._distances = distances
         self._connectivity = connectivity
 
     def __str__(self):  # pragma: no cover
-        """Prints the object to stdout."""
+        """Print the object to stdout."""
         return "deepof analysis of {} videos".format(len(self._videos))
 
     def __repr__(self):  # pragma: no cover
-        """Prints the object to stdout."""
+        """Print the object to stdout."""
         return "deepof analysis of {} videos".format(len(self._videos))
 
     def get_coords(
         self,
         center: str = False,
         polar: bool = False,
         speed: int = 0,
         align: str = False,
         align_inplace: bool = True,
         selected_id: str = None,
         propagate_labels: bool = False,
         propagate_annotations: Dict = False,
     ) -> table_dict:
-        """Returns a table_dict object with the coordinates of each animal as values.
+        """Return a table_dict object with the coordinates of each animal as values.
 
         Args:
-            center (str): Name of the body part to which the positions will be centered. If false,
-            the raw data is returned; if 'arena' (default), coordinates are centered in the pitch
+            center (str): Name of the body part to which the positions will be centered. If false, the raw data is returned; if 'arena' (default), coordinates are centered in the pitch
             polar (bool) States whether the coordinates should be converted to polar values.
-            speed (int): States the derivative of the positions to report. Speed is returned if 1, acceleration if 2,
-            jerk if 3, etc.
-            align (str): Selects the body part to which later processes will align the frames with
-            (see preprocess in table_dict documentation).
-            align_inplace (bool): Only valid if align is set. Aligns the vector that goes from the origin to the
-            selected body part with the y-axis, for all timepoints (default).
+            speed (int): States the derivative of the positions to report. Speed is returned if 1, acceleration if 2, jerk if 3, etc.
+            align (str): Selects the body part to which later processes will align the frames with (see preprocess in table_dict documentation).
+            align_inplace (bool): Only valid if align is set. Aligns the vector that goes from the origin to the selected body part with the y-axis, for all timepoints (default).
             selected_id (str): Selects a single animal on multi animal settings. Defaults to None (all animals are processed).
             propagate_labels (bool): If True, adds an extra feature for each video containing its phenotypic label
-            propagate_annotations (dict): If a dictionary is provided, supervised annotations are propagated through
-            the training dataset. This can be used for regularising the latent space based on already known traits.
+            propagate_annotations (dict): If a dictionary is provided, supervised annotations are propagated through the training dataset. This can be used for regularising the latent space based on already known traits.
 
         Returns:
             table_dict: A table_dict object containing the coordinates of each animal as values.
 
         """
         tabs = deepof.utils.deepcopy(self._tables)
         coord_1, coord_2 = "x", "y"
@@ -1039,24 +936,29 @@
         # Id selected_id was specified, selects coordinates of only one animal for further processing
         if selected_id is not None:
             for key, val in tabs.items():
                 tabs[key] = val.loc[
                     :, deepof.utils.filter_columns(val.columns, selected_id)
                 ]
 
+        # Set table_dict to NaN if animals are missing
+        tabs = deepof.utils.set_missing_animals(self, tabs, self.get_quality())
+
         if propagate_annotations:
             annotations = list(propagate_annotations.values())[0].columns
 
             for key, tab in tabs.items():
                 for ann in annotations:
                     tab.loc[:, ann] = propagate_annotations[key].loc[:, ann]
 
         if propagate_labels:
             for key, tab in tabs.items():
-                tab.loc[:, "pheno"] = self._exp_conditions[key]
+                tab.loc[:, "pheno"] = np.repeat(
+                    self._exp_conditions[key][propagate_labels].values, tab.shape[0]
+                )
 
         return TableDict(
             tabs,
             "coords",
             animal_ids=self._animal_ids,
             arena=self._arena,
             arena_dims=self._scales,
@@ -1072,21 +974,20 @@
         self,
         speed: int = 0,
         selected_id: str = None,
         filter_on_graph: bool = True,
         propagate_labels: bool = False,
         propagate_annotations: Dict = False,
     ) -> table_dict:
-        """Returns a table_dict object with the distances between body parts animal as values.
+        """Return a table_dict object with the distances between body parts animal as values.
 
         Args:
             speed (int): The derivative to use for speed.
             selected_id (str): The id of the animal to select.
-            filter_on_graph (bool): If True, only distances between connected nodes in the DeepOF graph representations
-            are kept. Otherwise, all distances between bodyparts are returned.
+            filter_on_graph (bool): If True, only distances between connected nodes in the DeepOF graph representations are kept. Otherwise, all distances between bodyparts are returned.
             propagate_labels (bool): If True, the pheno column will be propagated from the original data.
             propagate_annotations (Dict): A dictionary of annotations to propagate.
 
         Returns:
             table_dict: A table_dict object with the distances between body parts animal as values.
 
         """
@@ -1101,14 +1002,17 @@
 
             if selected_id is not None:
                 for key, val in tabs.items():
                     tabs[key] = val.loc[
                         :, deepof.utils.filter_columns(val.columns, selected_id)
                     ]
 
+            # Set table_dict to NaN if animals are missing
+            tabs = deepof.utils.set_missing_animals(self, tabs, self.get_quality())
+
             if propagate_labels:
                 for key, tab in tabs.items():
                     tab.loc[:, "pheno"] = self._exp_conditions[key]
 
             if propagate_annotations:
                 annotations = list(propagate_annotations.values())[0].columns
 
@@ -1121,16 +1025,17 @@
                 for key, tab in tabs.items():
                     tabs[key] = tab.loc[
                         :,
                         list(
                             set(
                                 [
                                     tuple(sorted(e))
-                                    for e in deepof.utils.connect_mouse_topview(
-                                        animal_ids=self._animal_ids
+                                    for e in deepof.utils.connect_mouse(
+                                        animal_ids=self._animal_ids,
+                                        graph_preset=self._bodypart_graph,
                                     ).edges
                                 ]
                             )
                             & set(tab.columns)
                         ),
                     ]
 
@@ -1152,15 +1057,15 @@
         self,
         degrees: bool = False,
         speed: int = 0,
         selected_id: str = None,
         propagate_labels: bool = False,
         propagate_annotations: Dict = False,
     ) -> table_dict:
-        """Returns a table_dict object with the angles between body parts animal as values.
+        """Return a table_dict object with the angles between body parts animal as values.
 
         Args:
             degrees (bool): If True (default), the angles will be in degrees. Otherwise they will be converted to radians.
             speed (int): The derivative to use for speed.
             selected_id (str): The id of the animal to select.
             propagate_labels (bool): If True, the pheno column will be propagated from the original data.
             propagate_annotations (Dict): A dictionary of annotations to propagate.
@@ -1182,14 +1087,17 @@
 
             if selected_id is not None:
                 for key, val in tabs.items():
                     tabs[key] = val.loc[
                         :, deepof.utils.filter_columns(val.columns, selected_id)
                     ]
 
+            # Set table_dict to NaN if animals are missing
+            tabs = deepof.utils.set_missing_animals(self, tabs, self.get_quality())
+
             if propagate_labels:
                 for key, tab in tabs.items():
                     tab["pheno"] = self._exp_conditions[key]
 
             if propagate_annotations:
                 annotations = list(propagate_annotations.values())[0].columns
 
@@ -1208,20 +1116,19 @@
             )
 
         raise ValueError(
             "Angles not computed. Read the documentation for more details"
         )  # pragma: no cover
 
     def get_areas(self, speed: int = 0, selected_id: str = "all") -> table_dict:
-        """Returns a table_dict object with all relevant areas (head, torso, back, full). Unless specified otherwise, the areas are computed for all animals.
+        """Return a table_dict object with all relevant areas (head, torso, back, full). Unless specified otherwise, the areas are computed for all animals.
 
         Args:
             speed (int): The derivative to use for speed.
-            selected_id (str): The id of the animal to select. "all" (default) computes the areas for all animals.
-            declared in self._animal_ids.
+            selected_id (str): The id of the animal to select. "all" (default) computes the areas for all animals. Declared in self._animal_ids.
 
         Returns:
             table_dict: A table_dict object with the areas of the body parts animal as values.
         """
         tabs = deepof.utils.deepcopy(self._areas)
 
         if self._areas is not None:
@@ -1231,40 +1138,43 @@
             else:
                 selected_ids = [selected_id]
 
             for key, tab in tabs.items():
 
                 exp_table = pd.DataFrame()
 
-                for id in selected_ids:
+                for aid in selected_ids:
 
-                    if id == "":
-                        id = None
+                    if aid == "":
+                        aid = None
 
                     # get the current table for the current animal
                     current_table = tab.loc[
-                        :, deepof.utils.filter_columns(tab.columns, id)
+                        :, deepof.utils.filter_columns(tab.columns, aid)
                     ]
                     exp_table = pd.concat([exp_table, current_table], axis=1)
 
                 tabs[key] = exp_table
 
+            if speed:
+                for key, tab in tabs.items():
+                    vel = deepof.utils.rolling_speed(tab, deriv=speed + 1, typ="angles")
+                    tabs[key] = vel
+
+            # Set table_dict to NaN if animals are missing
+            tabs = deepof.utils.set_missing_animals(self, tabs, self.get_quality())
+
             areas = TableDict(
                 tabs,
                 animal_ids=self._animal_ids,
                 connectivity=self._connectivity,
                 typ="areas",
                 exp_conditions=self._exp_conditions,
             )
 
-            if speed:
-                for key, tab in areas.items():
-                    vel = deepof.utils.rolling_speed(tab, deriv=speed + 1, typ="angles")
-                    areas[key] = vel
-
             return areas
 
         raise ValueError(
             "Areas not computed. Read the documentation for more details"
         )  # pragma: no cover
 
     def get_videos(self, play: bool = False):
@@ -1272,19 +1182,19 @@
         if play:  # pragma: no cover
             raise NotImplementedError
 
         return self._videos
 
     @property
     def get_exp_conditions(self):
-        """Returns the stored dictionary with experimental conditions per subject."""
+        """Return the stored dictionary with experimental conditions per subject."""
         return self._exp_conditions
 
     def load_exp_conditions(self, filepath):  # pragma: no cover
-        """Loads experimental conditions from a wide-format csv table.
+        """Load experimental conditions from a wide-format csv table.
 
         Args:
             filepath (str): Path to the file containing the experimental conditions.
 
         """
         exp_conditions = pd.read_csv(filepath, index_col=0)
         exp_conditions = {
@@ -1292,31 +1202,83 @@
                 exp_conditions.loc[exp_conditions.iloc[:, 0] == exp_id, :].iloc[0, 1:]
             ).T
             for exp_id in exp_conditions.iloc[:, 0]
         }
         self._exp_conditions = exp_conditions
 
     def get_quality(self):
-        """Retrieves a dictionary with the tagging quality per video, as reported by DLC."""
-        return self._quality
+        """Retrieve a dictionary with the tagging quality per video, as reported by DLC."""
+        return TableDict(self._quality, typ="quality", animal_ids=self._animal_ids)
 
     @property
     def get_arenas(self):
-        """Retrieves all available information associated with the arena."""
+        """Retrieve all available information associated with the arena."""
         return self._arena, [self._arena_dims], self._scales
 
+    def edit_arenas(
+        self, videos: list = None, arena_type: str = None, verbose: bool = True
+    ):  # pragma: no cover
+        """Tag the arena in the videos.
+
+        Args:
+            videos (list): A list of videos to reannotate. If None, all videos are loaded.
+            arena_type (str): The type of arena to use. Must be one of "polygonal-manual", "circular-manual", or "circular-autodetect". If None (default), the arena type specified when creating the project is used.
+            verbose (bool): Whether to print the progress of the annotation.
+
+        """
+        if videos is None:
+            videos = self._videos
+        if arena_type is None:
+            arena_type = self._arena
+
+        videos_renamed, vid_idcs = [], []
+        for vid_idx, vid_in in enumerate(self._videos):
+            for vid_out in videos:
+                if vid_out in vid_in:
+                    videos_renamed.append(vid_in)
+                    vid_idcs.append(vid_idx)
+
+        if verbose:
+            print(
+                "Editing {} arena{}".format(len(videos), "s" if len(videos) > 1 else "")
+            )
+
+        edited_scales, edited_arena_params, _ = deepof.utils.get_arenas(
+            arena=arena_type,
+            arena_dims=self._arena_dims,
+            project_path=self._project_path,
+            project_name=self._project_name,
+            tables=self._tables,
+            videos=videos_renamed,
+        )
+
+        if verbose:
+            print("Done!")
+
+        # update the scales and arena parameters
+        for vid_idx, vid in enumerate(videos):
+            self._scales[vid_idcs[vid_idx]] = edited_scales[vid_idx]
+            self._arena_params[vid_idcs[vid_idx]] = edited_arena_params[vid_idx]
+
+        self.save(timestamp=False)
+
     def save(self, filename: str = None, timestamp: bool = True):
-        """Saves the current state of the Coordinates object to a pickled file.
+        """Save the current state of the Coordinates object to a pickled file.
 
         Args:
             filename (str): Name of the pickled file to store. If no name is provided, a default is used.
             timestamp (bool): Whether to append a time stamp at the end of the output file name.
         """
         pkl_out = "{}{}.pkl".format(
-            (filename if filename is not None else "deepOF_Coordinates"),
+            os.path.join(
+                self._project_path,
+                self._project_name,
+                "Coordinates",
+                (filename if filename is not None else "deepof_coordinates"),
+            ),
             (f"_{int(time())}" if timestamp else ""),
         )
 
         with open(pkl_out, "wb") as handle:
             pickle.dump(self, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     def get_graph_dataset(
@@ -1325,28 +1287,23 @@
         precomputed_tab_dict: table_dict = None,
         center: str = False,
         polar: bool = False,
         align: str = None,
         preprocess: bool = True,
         **kwargs,
     ) -> table_dict:
-        """Generates a dataset with all specified features.
+        """Generate a dataset with all specified features.
 
         Args:
-            animal_id (str): Name of the animal to process. If None (default) all animals are included in a multi-animal
-            graph.
-            precomputed_tab_dict (table_dict): table_dict object for further graph processing. None (default) builds
-            it on the spot.
-            center (str): Name of the body part to which the positions will be centered. If false,
-            raw data is returned; if 'arena' (default), coordinates are centered on the pitch.
+            animal_id (str): Name of the animal to process. If None (default) all animals are included in a multi-animal graph.
+            precomputed_tab_dict (table_dict): table_dict object for further graph processing. None (default) builds it on the spot.
+            center (str): Name of the body part to which the positions will be centered. If false, raw data is returned; if 'arena' (default), coordinates are centered on the pitch.
             polar (bool) States whether the coordinates should be converted to polar values.
-            align (str): Selects the body part to which later processes will align the frames with
-            (see preprocess in table_dict documentation).
-            preprocess (bool): whether to preprocess the data to pass to autoencoders. If False, node features and
-            distance-weighted adjacency matrices on the raw data are returned.
+            align (str): Selects the body part to which later processes will align the frames with (see preprocess in table_dict documentation).
+            preprocess (bool): whether to preprocess the data to pass to autoencoders. If False, node features and distance-weighted adjacency matrices on the raw data are returned.
 
         Returns:
             merged_features: A graph-based dataset.
 
         """
         # Get all relevant features
         coords = self.get_coords(
@@ -1358,15 +1315,15 @@
         # Merge and extract names
         tab_dict = coords.merge(speeds, dists)
 
         if precomputed_tab_dict is not None:  # pragma: no cover
             tab_dict = precomputed_tab_dict
 
         # Get corresponding feature graph
-        graph = deepof.utils.connect_mouse_topview(
+        graph = deepof.utils.connect_mouse(
             animal_ids=(self._animal_ids if animal_id is None else animal_id),
             exclude_bodyparts=(
                 list(
                     set(
                         [
                             re.sub(
                                 r"|".join(
@@ -1378,14 +1335,15 @@
                             for bp in self._excluded
                         ]
                     )
                 )
                 if (self._animal_ids is not None and self._animal_ids[0])
                 else self._excluded
             ),
+            graph_preset=self._bodypart_graph,
         )
 
         tab_dict._connectivity = graph
         edge_feature_names = list(list(dists.values())[0].columns)
         feature_names = pd.Index([i for i in list(tab_dict.values())[0].columns])
         node_feature_names = (
             [(i, "x") for i in list(graph.nodes())]
@@ -1470,28 +1428,26 @@
         n_jobs: int = 1,
         propagate_labels: bool = False,
     ) -> table_dict:
         """Annotates coordinates with behavioral traits using a supervised pipeline.
 
         Args:
             params (Dict): A dictionary with the parameters to use for the pipeline. If unsure, leave empty.
-            video_output (bool): It outputs a fully annotated video for each experiment indicated in a list. If set to
-            "all", it will output all videos. False by default.
-            frame_limit (int): Only applies if video_output is not False. Indicates the maximum number of frames per
-            video to output.
-            debug (bool): Only applies if video_output is not False. If True, all videos will include debug information,
-            such as the detected arena and the preprocessed tracking tags.
+            video_output (bool): It outputs a fully annotated video for each experiment indicated in a list. If set to "all", it will output all videos. False by default.
+            frame_limit (int): Only applies if video_output is not False. Indicates the maximum number of frames per video to output.
+            debug (bool): Only applies if video_output is not False. If True, all videos will include debug information, such as the detected arena and the preprocessed tracking tags.
             n_jobs (int): Number of jobs to use for parallel processing.
             propagate_labels (bool): If True, the pheno column will be propagated from the original data.
 
         Returns:
             table_dict: A table_dict object with all supervised annotations per experiment as values.
 
         """
         tag_dict = {}
+        params = deepof.annotation_utils.get_hparameters(params)
         raw_coords = self.get_coords(center=None)
         coords = self.get_coords(center="Center", align="Spine_1")
         dists = self.get_distances()
         speeds = self.get_coords(speed=1)
         if len(self._animal_ids) <= 1:
             features_dict = (
                 deepof.post_hoc.align_deepof_kinematics_with_unsupervised_labels(
@@ -1527,39 +1483,39 @@
 
         if propagate_labels:  # pragma: no cover
             for key, tab in tag_dict.items():
                 tab["pheno"] = self._exp_conditions[key]
 
         if video_output:  # pragma: no cover
 
-            def output_video(idx):
-                """Outputs a single annotated video. Enclosed in a function to enable parallelization."""
-                deepof.visuals.annotate_video(
-                    self,
-                    tag_dict=tag_dict[idx],
-                    vid_index=list(self._tables.keys()).index(idx),
-                    debug=debug,
-                    frame_limit=frame_limit,
-                    params=params,
-                )
-                pbar.update(1)
+            deepof.annotation_utils.tagged_video_output(
+                self,
+                tag_dict,
+                video_output=video_output,
+                frame_limit=frame_limit,
+                debug=debug,
+                n_jobs=n_jobs,
+                params=params,
+            )
 
-            if isinstance(video_output, list):
-                vid_idxs = video_output
-            elif video_output == "all":
-                vid_idxs = list(self._tables.keys())
-            else:
-                raise AttributeError(
-                    "Video output must be either 'all' or a list with the names of the videos to render"
-                )
+        # Set table_dict to NaN if animals are missing
+        tag_dict = deepof.utils.set_missing_animals(
+            self,
+            tag_dict,
+            self.get_quality(),
+            animal_ids=self._animal_ids + ["supervised"],
+        )
 
-            pbar = tqdm(total=len(vid_idxs))
-            with parallel_backend("threading", n_jobs=n_jobs):
-                Parallel()(delayed(output_video)(key) for key in vid_idxs)
-            pbar.close()
+        # Add missing tags to all animals
+        presence_masks = deepof.utils.compute_animal_presence_mask(self.get_quality())
+        for tag in tag_dict:
+            for animal in self._animal_ids:
+                tag_dict[tag][
+                    "{}missing".format(("{}_".format(animal) if animal else ""))
+                ] = (1 - presence_masks[tag][animal].values)
 
         return TableDict(
             tag_dict,
             typ="supervised",
             animal_ids=self._animal_ids,
             arena=self._arena,
             arena_dims=self._arena_dims,
@@ -1604,38 +1560,33 @@
         Args:
             preprocessed_object (tuple): Tuple containing a preprocessed object (X_train, y_train, X_test, y_test).
             adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
             embedding_model (str): Name of the embedding model to use. Must be one of VQVAE (default), VaDE, or contrastive.
             encoder_type (str): Encoder architecture to use. Must be one of "recurrent", "TCN", and "transformer".
             batch_size (int): Batch size for training.
             latent_dim (int): Dimention size of the latent space.
-            epochs (int): Maximum number of epochs to train the model. Actual training might be shorter, as the model
-            will stop training when validation loss stops decreasing.
+            epochs (int): Maximum number of epochs to train the model. Actual training might be shorter, as the model will stop training when validation loss stops decreasing.
             log_history (bool): Whether to log the history of the model to TensorBoard.
             log_hparams (bool): Whether to log the hyperparameters of the model to TensorBoard.
             n_components (int): Number of latent clusters for the embedding model to use.
-            kmeans_loss (float): Weight of the gram loss, which adds a regularization term to VaDE and VQVAE models which
-            penalizes the correlation between the dimensions in the latent space.
+            kmeans_loss (float): Weight of the gram loss, which adds a regularization term to VaDE and VQVAE models which penalizes the correlation between the dimensions in the latent space.
             temperature (float): temperature parameter for the contrastive loss functions. Higher values put harsher penalties on negative pair similarity.
             contrastive_similarity_function (str): similarity function between positive and negative pairs. Must be one of 'cosine' (default), 'euclidean', 'dot', and 'edit'.
             contrastive_loss_function (str): contrastive loss function. Must be one of 'nce' (default), 'dcl', 'fc', and 'hard_dcl'. See specific documentation for details.
             beta (float): Beta (concentration) parameter for the hard_dcl contrastive loss. Higher values lead to 'harder' negative samples.
             tau (float): Tau parameter for the dcl and hard_dcl contrastive losses, indicating positive class probability.
             output_path (str): Path to save the trained model and all log files.
-            pretrained (str): Whether to load a pretrained model. If False, model is trained from scratch. If not,
-            must be the path to a saved model.
+            pretrained (str): Whether to load a pretrained model. If False, model is trained from scratch. If not, must be the path to a saved model.
             save_checkpoints (bool): Whether to save checkpoints of the model during training. Defaults to False.
             save_weights (bool): Whether to save the weights of the model during training. Defaults to True.
-            input_type (str): Type of the preprocessed_object passed as the first parameter. See deepof.data.TableDict
-            for more details.
+            input_type (str): Type of the preprocessed_object passed as the first parameter. See deepof.data.TableDict for more details.
             run (int): Run number for the model. Used to save the model and log files. Optional.
             kl_annealing_mode (str): Mode of the KL annealing. Must be one of "linear", or "sigmoid".
             kl_warmup (int): Number of epochs to warm up the KL annealing.
-            reg_cat_clusters (bool): whether to penalize uneven cluster membership in the latent space, by
-            minimizing the KL divergence between cluster membership and a uniform categorical distribution.
+            reg_cat_clusters (bool): whether to penalize uneven cluster membership in the latent space, by minimizing the KL divergence between cluster membership and a uniform categorical distribution.
             recluster (bool): whether to recluster after training using a Gaussian Mixture Model. Only valid for VaDE.
             interaction_regularization (float): weight of the interaction regularization term for all encoders.
             **kwargs: Additional keyword arguments to pass to the model.
 
         Returns:
             Tuple: Tuple containing all trained models. See specific model documentation under deepof.models for details.
         """
@@ -1723,31 +1674,29 @@
         center: str = None,
         connectivity: nx.Graph = None,
         polar: bool = None,
         exp_conditions: dict = None,
         propagate_labels: bool = False,
         propagate_annotations: Union[Dict, bool] = False,
     ):
-        """Main class for storing a single dataset as a dictionary with individuals as keys and pandas.DataFrames as values.
+        """Store single datasets as dictionaries with individuals as keys and pandas.DataFrames as values.
 
         Includes methods for generating training and testing datasets for the autoencoders.
 
         Args:
             tabs (Dict): Dictionary of pandas.DataFrames with individual experiments as keys.
             typ (str): Type of the dataset. Examples are "coords", "dists", and "angles". For logging purposes only.
             arena (str): Type of the arena. Must be one of "circular-autodetect", "circular-manual", or "polygon-manual". Handled internally.
             arena_dims (np.array): Dimensions of the arena in mm.
             animal_ids (list): list of animal ids.
             center (str): Type of the center. Handled internally.
             polar (bool): Whether the dataset is in polar coordinates. Handled internally.
             exp_conditions (dict): dictionary with experiment IDs as keys and experimental conditions as values.
-            propagate_labels (bool): Whether to propagate phenotypic labels from the original experiments to the
-            transformed dataset.
-            propagate_annotations (Dict): Dictionary of annotations to propagate. If provided, the supervised annotations
-            of the individual experiments are propagated to the dataset.
+            propagate_labels (bool): Whether to propagate phenotypic labels from the original experiments to the transformed dataset.
+            propagate_annotations (Dict): Dictionary of annotations to propagate. If provided, the supervised annotations of the individual experiments are propagated to the dataset.
 
         """
         super().__init__(tabs)
         self._type = typ
         self._center = center
         self._connectivity = connectivity
         self._polar = polar
@@ -1755,15 +1704,15 @@
         self._arena_dims = arena_dims
         self._animal_ids = animal_ids
         self._exp_conditions = exp_conditions
         self._propagate_labels = propagate_labels
         self._propagate_annotations = propagate_annotations
 
     def filter_videos(self, keys: list) -> table_dict:
-        """Returns a subset of the original table_dict object, containing only the specified keys.
+        """Return a subset of the original table_dict object, containing only the specified keys.
 
         Useful, for example, to select data coming from videos of a specified condition.
 
         Args:
             keys (list): List of keys to keep.
 
         Returns:
@@ -1774,18 +1723,52 @@
 
         return TableDict(
             {k: value for k, value in table.items() if k in keys},
             self._type,
             connectivity=self._connectivity,
             propagate_labels=self._propagate_labels,
             propagate_annotations=self._propagate_annotations,
+            exp_conditions=self._exp_conditions,
         )
 
+    def filter_condition(self, exp_filters: dict) -> table_dict:
+        """Return a subset of the original table_dict object, containing only videos belonging to the specified experimental condition.
+
+        Args:
+            exp_filters (dict): experimental conditions and values to filter on.
+
+        Returns:
+            TableDict: Subset of the original table_dict object, containing only the specified keys.
+        """
+        table = deepof.utils.deepcopy(self)
+
+        for exp_condition, exp_value in exp_filters.items():
+
+            filtered_table = {
+                k: value
+                for k, value in table.items()
+                if self._exp_conditions[k][exp_condition].values == exp_value
+            }
+            table = TableDict(
+                filtered_table,
+                self._type,
+                connectivity=self._connectivity,
+                propagate_labels=self._propagate_labels,
+                propagate_annotations=self._propagate_annotations,
+                exp_conditions={
+                    k: value
+                    for k, value in self._exp_conditions.items()
+                    if k in filtered_table.keys()
+                },
+            )
+
+        return table
+
     def _prepare_projection(self) -> np.ndarray:
-        """Returns a numpy ndarray from the preprocessing of the table_dict object, ready for projection into a lower dimensional space."""
+        """Return a numpy ndarray from the preprocessing of the table_dict object, ready for projection into a lower dimensional space."""
         labels = None
 
         # Takes care of propagated labels if present
         if self._propagate_labels:
             labels = {k: v.iloc[0, -1] for k, v in self.items()}
             labels = np.array([val for val in labels.values()])
 
@@ -1797,24 +1780,23 @@
         return X, labels
 
     def _projection(
         self,
         projection_type: str,
         n_components: int = 2,
         kernel: str = None,
-    ) -> deepof.utils.Tuple[deepof.utils.Any, deepof.utils.Any]:
-        """Returns a training set generated from the 2D original data (time x features) and a specified projection to an n_components space.
+    ) -> Tuple[Any, Any]:
+        """Return a training set generated from the 2D original data (time x features) and a specified projection to an n_components space.
 
         The sample parameter allows the user to randomly pick a subset of the data for performance or visualization reasons. For internal usage only.
 
         Args:
             projection_type (str): Projection to be used.
-            n_components: Number of components to project to.
-            kernel: Kernel to be used for the random and PCA algorithms.
-            perplexity: Perplexity parameter for the t-SNE algorithm.
+            n_components (int): Number of components to project to.
+            kernel (str): Kernel to be used for the random and PCA algorithms.
 
         Returns:
             tuple: Tuple containing projected data and projection type.
         """
         X, labels = self._prepare_projection()
 
         if projection_type == "random":
@@ -1831,33 +1813,31 @@
         if labels is not None:
             return X, labels, projection_type
 
         return X, projection_type
 
     def random_projection(
         self, n_components: int = 2, kernel: str = "linear"
-    ) -> deepof.utils.Tuple[deepof.utils.Any, deepof.utils.Any]:
-        """Returns a training set generated from the 2D original data (time x features) and a random projection to a n_components space.
+    ) -> Tuple[Any, Any]:
+        """Return a training set generated from the 2D original data (time x features) and a random projection to a n_components space.
 
         The sample parameter allows the user to randomly pick a subset of the data for
         performance or visualization reasons.
 
         Args:
             n_components (int): Number of components to project to. Default is 2.
             kernel (str): Kernel to be used for projections. Defaults to linear.
 
         Returns:
             tuple: Tuple containing projected data and projection type.
         """
         return self._projection("random", n_components=n_components, kernel=kernel)
 
-    def pca(
-        self, n_components: int = 2, kernel: str = "linear"
-    ) -> deepof.utils.Tuple[deepof.utils.Any, deepof.utils.Any]:
-        """Returns a training set generated from the 2D original data (time x features) and a PCA projection to a n_components space.
+    def pca(self, n_components: int = 2, kernel: str = "linear") -> Tuple[Any, Any]:
+        """Return a training set generated from the 2D original data (time x features) and a PCA projection to a n_components space.
 
         The sample parameter allows the user to randomly pick a subset of the data for
         performance or visualization reasons.
 
         Args:
             n_components (int): Number of components to project to. Default is 2.
             kernel (str): Kernel to be used for projections. Defaults to linear.
@@ -1866,16 +1846,16 @@
             tuple: Tuple containing projected data and projection type.
         """
         return self._projection("pca", n_components=n_components, kernel=kernel)
 
     def umap(
         self,
         n_components: int = 2,
-    ) -> deepof.utils.Tuple[deepof.utils.Any, deepof.utils.Any]:  # pragma: no cover
-        """Returns a training set generated from the 2D original data (time x features) and a PCA projection to a n_components space.
+    ) -> Tuple[Any, Any]:  # pragma: no cover
+        """Return a training set generated from the 2D original data (time x features) and a PCA projection to a n_components space.
 
         The sample parameter allows the user to randomly pick a subset of the data for
         performance or visualization reasons.
 
         Args:
             n_components (int): Number of components to project to. Default is 2.
             perplexity (int): Perplexity parameter for the t-SNE algorithm. Default is 30.
@@ -1886,21 +1866,20 @@
         """
         return self._projection(
             "umap",
             n_components=n_components,
         )
 
     def filter_id(self, selected_id: str = None) -> table_dict:
-        """Filters a TableDict object to keep only those columns related to the selected id.
+        """Filter a TableDict object to keep only those columns related to the selected id.
 
-        Leaves labels untouched if present.
+        Leave labels untouched if present.
 
         Args:
-            selected_id (str): select a single animal on multi animal settings. Defaults to None
-            (all animals are processed).
+            selected_id (str): select a single animal on multi animal settings. Defaults to None (all animals are processed).
 
         Returns:
             table_dict: Filtered TableDict object, keeping only the selected animal.
         """
         tabs = self.copy()
         for key, val in tabs.items():
             columns_to_keep = deepof.utils.filter_columns(val.columns, selected_id)
@@ -1910,18 +1889,19 @@
 
         return TableDict(
             tabs,
             typ=self._type,
             connectivity=self._connectivity,
             propagate_labels=self._propagate_labels,
             propagate_annotations=self._propagate_annotations,
+            exp_conditions=self._exp_conditions,
         )
 
     def merge(self, *args, ignore_index=False):
-        """Takes a number of table_dict objects and merges them to the current one.
+        """Take a number of table_dict objects and merges them to the current one.
 
         Returns a table_dict object of type 'merged'.
         Only annotations of the first table_dict object are kept.
 
         Args:
             *args (table_dict): table_dict objects to be merged.
             ignore_index (bool): ignore index when merging. Defaults to False.
@@ -1968,19 +1948,18 @@
         merged_tables._animal_ids = self._animal_ids
 
         return merged_tables
 
     def get_training_set(
         self, current_table_dict: table_dict, test_videos: int = 0
     ) -> tuple:
-        """Generates training and test sets as numpy.array objects for model training.
+        """Generate training and test sets as numpy.array objects for model training.
 
         Intended for internal usage only.
 
-
         Args:
             current_table_dict (table_dict): table_dict object containing the data to be used for training.
             test_videos (int): Number of videos to be used for testing. Defaults to 0.
 
         Returns:
             tuple: Tuple containing training data, training labels (if any), test data, and test labels (if any).
         """
@@ -2075,52 +2054,37 @@
         test_videos: int = 0,
         verbose: int = 0,
         shuffle: bool = False,
         filter_low_variance: bool = False,
         interpolate_normalized: int = 10,
         precomputed_breaks: dict = None,
     ) -> np.ndarray:
-        """Main method for preprocessing the loaded dataset before feeding to unsupervised embedding models.
+        """Preprocess the loaded dataset before feeding to unsupervised embedding models.
 
         Capable of returning training and test sets ready for model training.
 
         Args:
-            automatic_changepoints (str): specifies the changepoint detection kernel to use to rupture the
-            data across time using Pelt. Can be set to "rbf" (default), or "linear". If False, fixed-length ruptures are
-            appiled.
-            handle_ids (str): indicates the default action to handle multiple animals in the TableDict object. Must be
-            one of "concat" (body parts from different animals are treated as features) and "split" (different sliding windows
-            are created for each animal).
-            window_size (int): Minimum size of the applied ruptures. If automatic_changepoints is False,
-            specifies the size of the sliding window to pass through the data to generate training instances.
-            window_step (int): Specifies the minimum jump for the rupture algorithms. If automatic_changepoints is False,
-            specifies the step to take when sliding the aforementioned window. In this case, a value of 1 indicates
-            a true sliding window, and a value equal to window_size splits the data into non-overlapping chunks.
+            automatic_changepoints (str): specifies the changepoint detection kernel to use to rupture the data across time using Pelt. Can be set to "rbf" (default), or "linear". If False, fixed-length ruptures are appiled.
+            handle_ids (str): indicates the default action to handle multiple animals in the TableDict object. Must be one of "concat" (body parts from different animals are treated as features) and "split" (different sliding windows are created for each animal).
+            window_size (int): Minimum size of the applied ruptures. If automatic_changepoints is False, specifies the size of the sliding window to pass through the data to generate training instances.
+            window_step (int): Specifies the minimum jump for the rupture algorithms. If automatic_changepoints is False, specifies the step to take when sliding the aforementioned window. In this case, a value of 1 indicates a true sliding window, and a value equal to window_size splits the data into non-overlapping chunks.
             scale (str): Data scaling method. Must be one of 'standard', 'robust' (default; recommended) and 'minmax'.
             pretrained_scaler (Any): Pre-fit global scaler, trained on the whole dataset. Useful to process single videos.
             test_videos (int): Number of videos to use for testing. If 0, no test set is generated.
             verbose (int): Verbosity level. 0 (default) is silent, 1 prints progress, 2 prints debug information.
             shuffle (bool): Whether to shuffle the data before preprocessing. Defaults to False.
-            filter_low_variance (float): remove features with variance lower than the specified threshold. Useful to
-            get rid of the x axis of the body part used for alignment (which would introduce noise after standardization).
-            interpolate_normalized(int): if not 0, it specifies the number of standard deviations beyond which values will be
-            interpolated after normalization. Only used if scale is set to "standard".
+            filter_low_variance (float): remove features with variance lower than the specified threshold. Useful to get rid of the x axis of the body part used for alignment (which would introduce noise after standardization).
+            interpolate_normalized(int): if not 0, it specifies the number of standard deviations beyond which values will be interpolated after normalization. Only used if scale is set to "standard".
             precomputed_breaks (dict): If provided, changepoint detection is prevented, and provided breaks are used instead.
 
         Returns:
-            X_train (np.ndarray): 3D dataset with shape (instances, sliding_window_size, features)
-            generated from all training videos.
-            y_train (np.ndarray): 3D dataset with shape (instances, sliding_window_size, labels)
-            generated from all training videos. Note that no labels are use by default in the fully
-            unsupervised pipeline (in which case this is an empty array).
-            X_test (np.ndarray): 3D dataset with shape (instances, sliding_window_size, features)
-            generated from all test videos (0 by default).
-            y_test (np.ndarray): 3D dataset with shape (instances, sliding_window_size, labels)
-            generated from all test videos. Note that no labels are use by default in the fully
-            unsupervised pipeline (in which case this is an empty array).
+            X_train (np.ndarray): 3D dataset with shape (instances, sliding_window_size, features) generated from all training videos.
+            y_train (np.ndarray): 3D dataset with shape (instances, sliding_window_size, labels) generated from all training videos. Note that no labels are use by default in the fully unsupervised pipeline (in which case this is an empty array).
+            X_test (np.ndarray): 3D dataset with shape (instances, sliding_window_size, features) generated from all test videos (0 by default).
+            y_test (np.ndarray): 3D dataset with shape (instances, sliding_window_size, labels) generated from all test videos. Note that no labels are use by default in the fully unsupervised pipeline (in which case this is an empty array).
         """
         # Create a temporary copy of the current TableDict object,
         # to avoid modifying it in place
         table_temp = copy.deepcopy(self)
 
         assert handle_ids in [
             "concat",
```

### Comparing `deepof-0.2/deepof/deepof_train_embeddings.py` & `deepof-0.3/deepof/deepof_train_embeddings.py`

 * *Files 12% similar despite different names*

```diff
@@ -209,14 +209,21 @@
         "--run",
         "-rid",
         help="Sets the run ID of the experiment (for naming output files only). "
         "If 0 (default), uses a timestamp instead",
         type=int,
         default=0,
     )
+    parser.add_argument(
+        "--exp-condition-path",
+        "-ec",
+        help="If provided, loads the given experimental condition file. None by default.",
+        type=str,
+        default=None,
+    )
 
     args = parser.parse_args()
     current_GMT = time.gmtime()
     time_stamp = calendar.timegm(current_GMT)
 
     try:
         animal_ids = args.animal_ids
@@ -241,14 +248,15 @@
         train_path = os.path.abspath(args.train_path)
         tune = args.hyperparameter_tuning
         val_num = args.val_num
         window_size = args.window_size
         window_step = args.window_step
         max_epochs = args.max_epochs
         load_project = args.load_project
+        exp_condition_path = args.exp_condition_path
         run = args.run
 
     except TypeError:
         raise ValueError(
             "One or more mandatory arguments are missing. Use --help for details on how to run the CLI"
         )
 
@@ -256,17 +264,14 @@
         raise ValueError("Set a valid data path for the training to run")
 
     assert input_type in [
         "coords",
         "graph",
     ], "Invalid input type. Type python model_training.py -h for help."
 
-    # Loads model hyperparameters and treatment conditions, if available
-    treatment_dict = deepof.model_utils.load_treatments(train_path)
-
     # Logs hyperparameters  if specified on the --logparam CLI argument
     logparam = {"encoding": encoding_size, "k": n_components}
 
     if load_project is None:
         # noinspection PyTypeChecker
         project_coords = deepof.data.Project(
             animal_ids=animal_ids.split(","),
@@ -285,14 +290,18 @@
         )
 
         project_coords = project_coords.create(verbose=True)
 
     else:
         project_coords = deepof.data.load_project(load_project)
 
+    # If provided, load experimental conditions
+    if exp_condition_path is not None:
+        project_coords.load_exp_conditions(exp_condition_path)
+
     print("Preprocessing data...")
 
     if input_type == "coords":
 
         # Coordinates for training data
         to_preprocess = project_coords.get_coords(
             center="Center",
@@ -316,30 +325,29 @@
         print("Validation set shape:", preprocessed_object[2].shape)
 
     elif input_type == "graph":
 
         # Get graph dataset
         (
             preprocessed_object,
-            G,
+            adjacency_matrix,
             to_preprocess,
             global_scaler,
         ) = project_coords.get_graph_dataset(
             animal_id=animal_to_preprocess,
             center="Center",
             align="Spine_1",
             preprocess=True,
             window_size=window_size,
             window_step=window_step,
             automatic_changepoints=automatic_changepoints,
             test_videos=val_num,
             scale="standard",
             shuffle=True,
         )
-        adjacency_matrix = nx.adjacency_matrix(G).todense()
 
         print("Training node set shape:", preprocessed_object[0].shape)
         print("Training edge set shape:", preprocessed_object[1].shape)
         print("Validation node set shape:", preprocessed_object[3].shape)
         print("Validation edge set shape:", preprocessed_object[4].shape)
 
     print("Done!")
@@ -364,97 +372,22 @@
             # Parameters that control the training process
             kmeans_loss=kmeans_loss,
             reg_cat_clusters=cat_kl_loss,
             epochs=max_epochs,
             run=run,
         )
 
-        # Save data encoded with the current trained model
-        deep_encodings_per_video = {}
-        deep_assignments_per_video = {}
-        deep_breaks_per_video = {}
-
-        for key in to_preprocess.keys():
-
-            # Get preprocessed data for current video
-            if input_type == "coords":
-                curr_prep, _ = to_preprocess.filter_videos([key]).preprocess(
-                    window_size=window_size,
-                    window_step=1,
-                    automatic_changepoints=automatic_changepoints,
-                    pretrained_scaler=global_scaler,
-                    scale="standard",
-                    test_videos=0,
-                    shuffle=False,
-                )[0]
-                curr_adj = np.zeros(curr_prep.shape)
-
-            elif input_type == "graph":
-                curr_prep, _, _, _ = project_coords.get_graph_dataset(
-                    precomputed_tab_dict=to_preprocess.filter_videos([key]),
-                    animal_id=animal_to_preprocess,
-                    window_size=window_size,
-                    window_step=1,
-                    automatic_changepoints=automatic_changepoints,
-                    pretrained_scaler=global_scaler,
-                    scale="standard",
-                    test_videos=0,
-                    shuffle=False,
-                )
-                curr_adj = curr_prep[1]
-                curr_prep = curr_prep[0]
-
-            # Get breakpoints per video
-            deep_breaks_per_video[key] = (~np.all(curr_prep == 0, axis=2)).sum(axis=1)
-
-            # Get current model weights
-            curr_weights = trained_models.get_weights()
-
-            # Load weights into a newly created model, built with the current input shape
-            if embedding_model == "VQVAE":
-                curr_ae = deepof.models.VQVAE(
-                    input_shape=curr_prep.shape,
-                    edge_feature_shape=curr_adj.shape,
-                    adjacency_matrix=(
-                        None if input_type == "coords" else adjacency_matrix
-                    ),
-                    use_gnn=(input_type == "graph"),
-                    encoder_type=encoder_type,
-                    latent_dim=encoding_size,
-                    n_components=n_components,
-                )
-
-            elif embedding_model == "VaDE":
-                curr_ae = deepof.models.VaDE(
-                    input_shape=curr_prep.shape,
-                    edge_feature_shape=curr_adj.shape,
-                    adjacency_matrix=(
-                        None if input_type == "coords" else adjacency_matrix
-                    ),
-                    use_gnn=(input_type == "graph"),
-                    encoder_type=encoder_type,
-                    batch_size=batch_size,
-                    latent_dim=encoding_size,
-                    n_components=n_components,
-                    reg_cat_clusters=cat_kl_loss,
-                )
-
-            elif embedding_model == "Contrastive":
-                raise NotImplementedError
-
-            # noinspection PyUnboundLocalVariable
-            curr_ae.set_weights(curr_weights)
-
-            # Embed current video in the autoencoder and add to the dictionary
-            # noinspection PyUnboundLocalVariable
-            deep_encodings_per_video[key] = curr_ae.encoder([curr_prep, curr_adj])
-
-            # Obtain groupings for current video and add to the dictionary
-            # noinspection PyUnboundLocalVariable
-            deep_assignments_per_video[key] = curr_ae.grouper([curr_prep, curr_adj])
+        # Get embeddings, soft_counts, and breaks per video
+        embeddings, soft_counts, breaks = deepof.model_utils.embedding_per_video(
+            coordinates=my_deepof_project,
+            to_preprocess=to_preprocess,
+            model=trained_model,
+            animal_id=animal_to_preprocess,
+            global_scaler=global_scaler,
+        )
 
         with open(
             os.path.join(
                 output_path,
                 "deepof_unsupervised_{}_encoder_{}_encodings_input={}_k={}_latdim={}_changepoints_{}_kmeans_loss={}_run={}.pkl".format(
                     embedding_model,
                     encoder_type,
```

### Comparing `deepof-0.2/deepof/hypermodels.py` & `deepof-0.3/deepof/hypermodels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-"""
-
-keras_tuner hypermodels for hyperparameter tuning of deep autoencoders in deepof.models
-
-"""
+"""keras_tuner hypermodels for hyperparameter tuning of deep autoencoders in deepof.models."""
 
 from keras_tuner import HyperModel
 from typing import Any, List, NewType
 import numpy as np
 import tensorflow_probability as tfp
 
 import deepof.model_utils
@@ -22,34 +18,28 @@
 # DEFINE CUSTOM ANNOTATED TYPES #
 project = NewType("deepof_project", Any)
 coordinates = NewType("deepof_coordinates", Any)
 table_dict = NewType("deepof_table_dict", Any)
 
 
 class VaDE(HyperModel):
-    """
-
-    Hyperparameter tuning pipeline for deepof.models.VaDE
-
-    """
+    """Hyperparameter tuning pipeline for deepof.models.VaDE."""
 
     def __init__(
         self,
         input_shape: tuple,
         latent_dim: int,
         batch_size: int,
         n_components: int = 10,
         learn_rate: float = 1e-3,
         edge_feature_shape: tuple = None,
         use_gnn: bool = False,
         adjacency_matrix: np.ndarray = None,
     ):
-        """
-
-        VaDE hypermodel for hyperparameter tuning.
+        """Build VaDE hypermodel for hyperparameter tuning.
 
         Args:
             input_shape (tuple): shape of the input tensor.
             latent_dim (int): dimension of the latent space.
             batch_size (int): batch size for training.
             learn_rate (float): learning rate for the optimizer.
             n_components (int): number of components in the quantization space.
@@ -65,20 +55,15 @@
         self.learn_rate = learn_rate
         self.n_components = n_components
         self.edge_feature_shape = edge_feature_shape
         self.use_gnn = use_gnn
         self.adjacency_matrix = adjacency_matrix
 
     def get_hparams(self, hp):
-        """
-
-        Retrieve hyperparameters to tune
-
-        """
-
+        """Retrieve hyperparameters to tune."""
         # Architectural hyperparameters
         encoder = hp.Choice(
             "encoder", ["recurrent", "TCN", "transformer"], default="recurrent"
         )
         kmeans_loss = hp.Float(
             "kmeans_loss", min_value=0.0, max_value=1.0, sampling="linear"
         )
@@ -100,20 +85,15 @@
             kmeans_loss,
             kl_annealing_mode,
             kl_warmup_epochs,
             cluster_assignment_regularizer,
         )
 
     def build(self, hp):
-        """
-
-        Overrides Hypermodel's build method
-
-        """
-
+        """Override Hypermodel's build method."""
         # Hyperparameters to tune
         (
             encoder,
             kmeans_loss,
             kl_annealing_mode,
             kl_warmup_epochs,
             cluster_assignment_regularizer,
@@ -136,78 +116,61 @@
         )
         vade.compile()
 
         return vade
 
 
 class VQVAE(HyperModel):
-    """
-
-    Hyperparameter tuning pipeline for deepof.models.VQVAE
-
-    """
+    """Hyperparameter tuning pipeline for deepof.models.VQVAE."""
 
     def __init__(
         self,
         input_shape: tuple,
         latent_dim: int,
         n_components: int = 10,
         learn_rate: float = 1e-3,
         edge_feature_shape: tuple = None,
         use_gnn: bool = False,
         adjacency_matrix: np.ndarray = None,
     ):
-        """
-
-        VQVAE hypermodel for hyperparameter tuning.
+        """VQVAE hypermodel for hyperparameter tuning.
 
         Args:
             input_shape (tuple): shape of the input tensor.
             latent_dim (int): dimension of the latent space.
             learn_rate (float): learning rate for the optimizer.
             n_components (int): number of components in the quantization space.
             edge_feature_shape (tuple): shape of the edge feature tensor.
             use_gnn (bool): whether to use a graph neural network to encode the input data.
             adjacency_matrix (np.ndarray): adjacency matrix of the graph.
 
         """
-
         super().__init__()
         self.input_shape = input_shape
         self.latent_dim = latent_dim
         self.learn_rate = learn_rate
         self.n_components = n_components
         self.edge_feature_shape = edge_feature_shape
         self.use_gnn = use_gnn
         self.adjacency_matrix = adjacency_matrix
 
     def get_hparams(self, hp):
-        """
-
-        Retrieve hyperparameters to tune, including the encoder type and the weight of the kmeans loss.
-
-        """
-
+        """Retrieve hyperparameters to tune, including the encoder type and the weight of the kmeans loss."""
         # Architectural hyperparameters
         encoder = hp.Choice(
             "encoder", ["recurrent", "TCN", "transformer"], default="recurrent"
         )
         kmeans_loss = hp.Float(
             "kmeans_loss", min_value=0.0, max_value=1.0, sampling="linear"
         )
 
         return (encoder, kmeans_loss)
 
     def build(self, hp):
-        """
-
-        Overrides Hypermodel's build method
-
-        """
-
+        """Override Hypermodel's build method."""
         # Hyperparameters to tune
         (encoder, kmeans_loss) = self.get_hparams(hp)
 
         vqvae = deepof.models.VQVAE(
             input_shape=self.input_shape,
             edge_feature_shape=self.edge_feature_shape,
             adjacency_matrix=self.adjacency_matrix,
@@ -220,72 +183,55 @@
         )
         vqvae.compile()
 
         return vqvae
 
 
 class Contrastive(HyperModel):
-    """
-
-    Hyperparameter tuning pipeline for deepof.models.Contrastive
-
-    """
+    """Hyperparameter tuning pipeline for deepof.models.Contrastive."""
 
     def __init__(
         self,
         input_shape: tuple,
         latent_dim: int,
         learn_rate: float = 1e-3,
         edge_feature_shape: tuple = None,
         use_gnn: bool = False,
         adjacency_matrix: np.ndarray = None,
     ):
-        """
-
-        Contrastive hypermodel for hyperparameter tuning.
+        """Contrastive hypermodel for hyperparameter tuning.
 
         Args:
             input_shape (tuple): shape of the input tensor.
             latent_dim (int): dimension of the latent space.
             learn_rate (float): learning rate for the optimizer.
             edge_feature_shape (tuple): shape of the edge feature tensor.
             use_gnn (bool): whether to use a graph neural network to encode the input data.
             adjacency_matrix (np.ndarray): adjacency matrix of the graph.
 
         """
-
         super().__init__()
         self.input_shape = input_shape
         self.latent_dim = latent_dim
         self.learn_rate = learn_rate
         self.edge_feature_shape = edge_feature_shape
         self.use_gnn = use_gnn
         self.adjacency_matrix = adjacency_matrix
 
     def get_hparams(self, hp):
-        """
-
-        Retrieve hyperparameters to tune, including the encoder type and the weight of the kmeans loss.
-
-        """
-
+        """Retrieve hyperparameters to tune, including the encoder type and the weight of the kmeans loss."""
         # Architectural hyperparameters
         encoder = hp.Choice(
             "encoder", ["recurrent", "TCN", "transformer"], default="recurrent"
         )
 
         return encoder
 
     def build(self, hp):
-        """
-
-        Overrides Hypermodel's build method
-
-        """
-
+        """Override Hypermodel's build method."""
         # Hyperparameters to tune
         (encoder) = self.get_hparams(hp)
 
         contrastive = deepof.models.Contrastive(
             input_shape=self.input_shape,
             edge_feature_shape=self.edge_feature_shape,
             adjacency_matrix=self.adjacency_matrix,
```

### Comparing `deepof-0.2/deepof/model_utils.py` & `deepof-0.3/deepof/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-"""
-
-Utility functions for both training autoencoder models in deepof.models and tuning hyperparameters with deepof.hypermodels.
-
-"""
+"""Utility functions for both training autoencoder models in deepof.models and tuning hyperparameters with deepof.hypermodels."""
 
 from datetime import date, datetime
 from functools import partial
 from keras_tuner import BayesianOptimization, Hyperband, Objective
 from tensorboard.plugins.hparams import api as hp
 from tensorflow.keras.initializers import he_uniform
 from tensorflow.keras.layers import (
     Bidirectional,
     GRU,
     LayerNormalization,
     TimeDistributed,
 )
 from typing import Tuple, Union, Any, List, NewType
+import deepof.data
 import deepof.hypermodels
 import deepof.models
+import deepof.post_hoc
 import json
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 from spektral.layers import CensNetConv
 import tensorflow as tf
 import tensorflow.keras.backend as K
@@ -53,15 +51,15 @@
     loss_fn="nce",
     temperature=0.1,
     tau=0.1,
     beta=0.1,
     elimination_topk=0.1,
     attraction=False,
 ):  # pragma: no cover
-    """Selects and applies the contrastive loss function to be used in the Contrastive embedding models.
+    """Select and applies the contrastive loss function to be used in the Contrastive embedding models.
 
     Args:
         history: Tensor of shape (batch_size, seq_len, embedding_dim).
         future: Tensor of shape (batch_size, seq_len, embedding_dim).
         similarity: Function that computes the similarity between two tensors.
         loss_fn: String indicating the loss function to be used.
         temperature: Float indicating the temperature to be used in the specified loss function.
@@ -88,15 +86,14 @@
     elif loss_fn == "fc":
         loss, pos, neg = fc_loss(
             history,
             future,
             similarity,
             temperature,
             elimination_topk=elimination_topk,
-            attraction=attraction,
         )
     elif loss_fn == "hard_dcl":
         loss, pos, neg = hard_loss(
             history,
             future,
             similarity,
             temperature,
@@ -106,55 +103,48 @@
         )
 
     # noinspection PyUnboundLocalVariable
     return loss, pos, neg
 
 
 def _cosine_similarity(x, y):  # pragma: no cover
-    """Computes the cosine similarity between two tensors."""
-
+    """Compute the cosine similarity between two tensors."""
     v = tf.keras.losses.CosineSimilarity(
         axis=2, reduction=tf.keras.losses.Reduction.NONE
     )(tf.expand_dims(x, 1), tf.expand_dims(y, 0))
     return -v
 
 
 def _dot_similarity(x, y):  # pragma: no cover
-    """Computes the dot product between two tensors."""
-
+    """Compute the dot product between two tensors."""
     v = tf.tensordot(tf.expand_dims(x, 1), tf.expand_dims(tf.transpose(y), 0), axes=2)
 
     return v
 
 
 def _euclidean_similarity(x, y):  # pragma: no cover
-    """Computes the euclidean distance between two tensors."""
-
+    """Compute the euclidean distance between two tensors."""
     x1 = tf.expand_dims(x, 1)
     y1 = tf.expand_dims(y, 0)
     d = tf.sqrt(tf.reduce_sum(tf.square(x1 - y1), axis=2))
     s = 1 / (1 + d)
     return s
 
 
 def _edit_similarity(x, y):  # pragma: no cover
-    """Computes the edit distance between two tensors."""
-
+    """Compute the edit distance between two tensors."""
     x1 = tf.expand_dims(x, 1)
     y1 = tf.expand_dims(y, 0)
     d = tf.sqrt(tf.reduce_sum(tf.square(x1 - y1), axis=2))
     s = 1 / (1 + d)
     return s
 
 
 def nce_loss(history, future, similarity, temperature=0.1):  # pragma: no cover
-    """Computes the NCE loss function, as described in the paper "A Simple Framework for Contrastive
-    Learning of Visual Representations" (https://arxiv.org/abs/2002.05709).
-
-    """
+    """Compute the NCE loss function, as described in the paper "A Simple Framework for Contrastive Learning of Visual Representations" (https://arxiv.org/abs/2002.05709)."""
     criterion = tf.keras.losses.BinaryCrossentropy(
         from_logits=True, reduction=tf.keras.losses.Reduction.SUM
     )
 
     N = history.shape[0]
     sim = similarity(history, future)
     pos_sim = K.exp(tf.linalg.tensor_diag_part(sim) / temperature)
@@ -176,15 +166,15 @@
     mean_neg = K.mean(neg)
     return loss, mean_sim, mean_neg
 
 
 def dcl_loss(
     history, future, similarity, temperature=0.1, debiased=True, tau_plus=0.1
 ):  # pragma: no cover
-    """Computes the DCL loss function, as described in the paper "Debiased Contrastive Learning" (https://github.com/chingyaoc/DCL/)."""
+    """Compute the DCL loss function, as described in the paper "Debiased Contrastive Learning" (https://github.com/chingyaoc/DCL/)."""
     N = history.shape[0]
     sim = similarity(history, future)
     pos_sim = K.exp(tf.linalg.tensor_diag_part(sim) / temperature)
 
     tri_mask = np.ones(N**2, dtype=np.bool).reshape(N, N)
     tri_mask[np.diag_indices(N)] = False
     neg = tf.reshape(tf.boolean_mask(sim, tri_mask), [N, N - 1])
@@ -209,21 +199,21 @@
     # similarity of positive pairs (only for debug)
     mean_sim = K.mean(tf.linalg.tensor_diag_part(sim))
     mean_neg = K.mean(neg)
     return loss, mean_sim, mean_neg
 
 
 def fc_loss(
-    history, future, similarity, temperature=0.1, elimination_topk=0.1, attraction=False
+    history,
+    future,
+    similarity,
+    temperature=0.1,
+    elimination_topk=0.1,
 ):  # pragma: no cover
-    """Computes the FC loss function, as described in the paper "Fully-Contrastive Learning of Visual Representations"
-    (https://arxiv.org/abs/2004.11362).
-
-    """
-
+    """Compute the FC loss function, as described in the paper "Fully-Contrastive Learning of Visual Representations" (https://arxiv.org/abs/2004.11362)."""
     N = history.shape[0]
     if elimination_topk > 0.5:
         elimination_topk = 0.5
     elimination_topk = np.math.ceil(elimination_topk * N)
 
     sim = similarity(history, future) / temperature
 
@@ -253,18 +243,15 @@
     mean_neg = K.mean(neg) * temperature
     return loss, mean_sim, mean_neg
 
 
 def hard_loss(
     history, future, similarity, temperature, beta=0.0, debiased=True, tau_plus=0.1
 ):  # pragma: no cover
-    """Computes the Hard loss function, as described in the paper "Contrastive Learning with Hard Negative Samples"
-    (https://arxiv.org/abs/2011.03343).
-
-    """
+    """Compute the Hard loss function, as described in the paper "Contrastive Learning with Hard Negative Samples" (https://arxiv.org/abs/2011.03343)."""
     N = history.shape[0]
 
     sim = similarity(history, future)
     pos_sim = K.exp(tf.linalg.tensor_diag_part(sim) / temperature)
 
     tri_mask = np.ones(N**2, dtype=np.bool).reshape(N, N)
     tri_mask[np.diag_indices(N)] = False
@@ -292,25 +279,25 @@
     loss = K.mean(-tf.math.log(pos_sim / (pos_sim + Ng)))
     # similarity of positive pairs (only for debug)
     mean_sim = K.mean(tf.linalg.tensor_diag_part(sim))
     mean_neg = K.mean(neg)
     return loss, mean_sim, mean_neg
 
 
-def compute_kmeans_loss(latent_means, weight=1.0, batch_size=64):  # pragma: no cover
-    """
+def compute_kmeans_loss(
+    latent_means: tf.Tensor, weight: float = 1.0, batch_size: int = 64
+):  # pragma: no cover
+    """Add a penalty to the singular values of the Gram matrix of the latent means. It helps disentangle the latent space.
 
-    Adds a penalty to the singular values of the Gram matrix of the latent means. It helps disentangle the latent
-    space.
     Based on https://arxiv.org/pdf/1610.04794.pdf, and https://www.biorxiv.org/content/10.1101/2020.05.14.095430v3.
 
     Args:
-        latent_means: tensor containing the means of the latent distribution
-        weight: weight of the Gram loss in the total loss function
-        batch_size: batch size of the data to compute the kmeans loss for.
+        latent_means (tf.Tensor): tensor containing the means of the latent distribution
+        weight (float): weight of the Gram loss in the total loss function
+        batch_size (int): batch size of the data to compute the kmeans loss for.
 
     Returns:
         tf.Tensor: kmeans loss
 
     """
     gram_matrix = (tf.transpose(latent_means) @ latent_means) / tf.cast(
         batch_size, tf.float32
@@ -318,17 +305,15 @@
     s = tf.linalg.svd(gram_matrix, compute_uv=False)
     s = tf.sqrt(tf.maximum(s, 1e-9))
     return weight * tf.reduce_mean(s)
 
 
 @tf.function
 def get_k_nearest_neighbors(tensor, k, index):  # pragma: no cover
-    """
-
-    Retrieve indices of the k nearest neighbors in tensor to the vector with the specified index
+    """Retrieve indices of the k nearest neighbors in tensor to the vector with the specified index.
 
     Args:
         tensor (tf.Tensor): tensor to compute the k nearest neighbors for
         k (int): number of nearest neighbors to retrieve
         index (int): index of the vector to compute the k nearest neighbors for
 
     Returns:
@@ -340,73 +325,64 @@
     max_distance = tf.gather(tf.sort(distances), k)
     neighbourhood_mask = distances < max_distance
     return tf.squeeze(tf.where(neighbourhood_mask))
 
 
 @tf.function
 def compute_shannon_entropy(tensor):  # pragma: no cover
-    """
-
-    Computes Shannon entropy for a given tensor
+    """Compute Shannon entropy for a given tensor.
 
     Args:
         tensor (tf.Tensor): tensor to compute the entropy for
 
     Returns:
         tf.Tensor: entropy of the tensor
 
     """
-
     tensor = tf.cast(tensor, tf.dtypes.int32)
     bins = (
         tf.math.bincount(tensor, dtype=tf.dtypes.float32)
         / tf.cast(tf.shape(tensor), tf.dtypes.float32)[0]
     )
     return -tf.reduce_sum(bins * tf.math.log(bins + 1e-5))
 
 
 def plot_lr_vs_loss(rates, losses):  # pragma: no cover
-    """
-
-    Plots learing rate versus the loss function of the model
+    """Plot learning rate versus the loss function of the model.
 
     Args:
         rates (np.ndarray): array containing the learning rates to plot in the x-axis
         losses (np.ndarray): array containing the losses to plot in the y-axis
 
     """
-
     plt.plot(rates, losses)
     plt.gca().set_xscale("log")
     plt.hlines(min(losses), min(rates), max(rates))
     plt.axis([min(rates), max(rates), min(losses), (losses[0] + min(losses)) / 2])
     plt.xlabel("Learning rate")
     plt.ylabel("Loss")
 
 
 def get_angles(pos: int, i: int, d_model: int):
-    """
-
-    Auxiliary function for positional encoding computation.
+    """Auxiliary function for positional encoding computation.
 
     Args:
         pos (int): position in the sequence.
         i (int): number of sequences.
         d_model (int): dimensionality of the embeddings.
 
     """
-
     angle_rates = 1 / np.power(10000, (2 * (i // 2)) / np.float32(d_model))
     return pos * angle_rates
 
 
 def get_recurrent_block(
     x: tf.Tensor, latent_dim: int, gru_unroll: bool, bidirectional_merge: str
 ):
-    """Builds a recurrent embedding block, using a 1D convolution followed by two bidirectional GRU layers.
+    """Build a recurrent embedding block, using a 1D convolution followed by two bidirectional GRU layers.
 
     Args:
         x (tf.Tensor): Input tensor.
         latent_dim (int): Number of dimensions of the output tensor.
         gru_unroll (bool): whether to unroll the GRU layers. Defaults to False.
         bidirectional_merge (str): how to merge the forward and backward GRU layers. Defaults to "concat".
 
@@ -455,25 +431,21 @@
     )(encoder)
     encoder = LayerNormalization()(encoder)
 
     return tf.keras.models.Model(x, encoder)
 
 
 def positional_encoding(position: int, d_model: int):
-    """
-
-    Computes positional encodings, as in
-    https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf.
+    """Compute positional encodings, as in https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf.
 
     Args:
         position (int): position in the sequence.
         d_model (int): dimensionality of the embeddings.
 
     """
-
     angle_rads = get_angles(
         np.arange(position)[:, np.newaxis], np.arange(d_model)[np.newaxis, :], d_model
     )
 
     # apply sin to even indices in the array; 2i
     angle_rads[:, 0::2] = np.sin(angle_rads[:, 0::2])
 
@@ -482,56 +454,49 @@
 
     pos_encoding = angle_rads[np.newaxis, ...]
 
     return tf.cast(pos_encoding, dtype=tf.float32)
 
 
 def create_padding_mask(seq: tf.Tensor):
-    """
-
-    Creates a padding mask, with zeros where data is missing, and ones where data is available.
+    """Create a padding mask, with zeros where data is missing, and ones where data is available.
 
     Args:
         seq (tf.Tensor): Sequence to compute the mask on
 
     """
-
     seq = tf.cast(tf.math.equal(seq, 0), tf.float32)
 
     # add extra dimensions to add the padding to the attention logits.
     return tf.cast(1 - seq[:, tf.newaxis, tf.newaxis, :], tf.float32)
 
 
 def create_look_ahead_mask(size: int):
-    """
+    """Create a triangular matrix containing an increasing amount of ones from left to right on each subsequent row.
 
-    Creates a triangular matrix containing an increasing amount of ones from left to right on each subsequent row.
     Useful for transformer decoder, which allows it to go through the data in a sequential manner, without taking
     the future into account.
 
     Args:
         size (int): number of time steps in the sequence
 
     """
-
     mask = tf.linalg.band_part(tf.ones((size, size)), -1, 0)
     return tf.cast(mask, tf.float32)
 
 
 def create_masks(inp: tf.Tensor):
-    """
+    """Given an input sequence, it creates all necessary masks to pass it through the transformer architecture.
 
-    Given an input sequence, it creates all necessary masks to pass it through the transformer architecture.
     This includes encoder and decoder padding masks, and a look-ahead mask
 
     Args:
         inp (tf.Tensor): input sequence to create the masks for.
 
     """
-
     # Reduces the dimensionality of the mask to remove the feature dimension
     tar = inp[:, :, 0]
     inp = inp[:, :, 0]
 
     # Encoder padding mask
     enc_padding_mask = create_padding_mask(inp)
 
@@ -548,54 +513,48 @@
 
     return enc_padding_mask, combined_mask, dec_padding_mask
 
 
 def find_learning_rate(
     model, data, epochs=1, batch_size=32, min_rate=10**-8, max_rate=10**-1
 ):
-    """
-
-    Trains the provided model for an epoch with an exponentially increasing learning rate
+    """Train the provided model for an epoch with an exponentially increasing learning rate.
 
     Args:
         model (tf.keras.Model): model to train
         data (tuple): training data
         epochs (int): number of epochs to train the model for
         batch_size (int): batch size to use for training
         min_rate (float): minimum learning rate to consider
         max_rate (float): maximum learning rate to consider
 
     Returns:
         float: learning rate that resulted in the lowest loss
 
     """
-
     init_weights = model.get_weights()
     iterations = len(data)
     factor = K.exp(K.log(max_rate / min_rate) / iterations)
     init_lr = K.get_value(model.optimizer.lr)
     K.set_value(model.optimizer.lr, min_rate)
     exp_lr = ExponentialLearningRate(factor)
     model.fit(data, epochs=epochs, batch_size=batch_size, callbacks=[exp_lr])
     K.set_value(model.optimizer.lr, init_lr)
     model.set_weights(init_weights)
     return exp_lr.rates, exp_lr.losses
 
 
 @tf.function
 def get_hard_counts(soft_counts: tf.Tensor):
-    """
-
-    Computes hard counts per cluster in a differentiable way
+    """Compute hard counts per cluster in a differentiable way.
 
     Args:
         soft_counts (tf.Tensor): soft counts per cluster
 
     """
-
     max_per_row = tf.expand_dims(tf.reduce_max(soft_counts, axis=1), axis=1)
 
     mask = tf.cast(soft_counts == max_per_row, tf.float32)
     mask_forward = tf.multiply(soft_counts, mask)
     mask_complement = tf.multiply(1 / soft_counts, mask)
 
     binary_counts = tf.multiply(mask_forward, mask_complement)
@@ -603,28 +562,24 @@
     return tf.math.reduce_sum(binary_counts, axis=0) + 1
 
 
 @tf.function
 def cluster_frequencies_regularizer(
     soft_counts: tf.Tensor, k: int, n_samples: int = 1000
 ):
-    """
+    """Compute the KL divergence between the cluster assignment distribution and a uniform prior across clusters.
 
-    Computes the KL divergence between the cluster assignment distribution
-    and a uniform prior across clusters. While this assumes an equal distribution
-    between clusters, the prior can be tweaked to reflect domain knowledge.
+    While this assumes an equal distribution between clusters, the prior can be tweaked to reflect domain knowledge.
 
     Args:
         soft_counts (tf.Tensor): soft counts per cluster
         k (int): number of clusters
-        n_samples (int): number of samples to draw from the categorical distribution
-        modeling cluster assignments.
+        n_samples (int): number of samples to draw from the categorical distribution modeling cluster assignments.
 
     """
-
     hard_counts = get_hard_counts(soft_counts)
 
     dist_a = tfd.Categorical(probs=hard_counts / k)
     dist_b = tfd.Categorical(probs=tf.ones(k))
 
     z = dist_a.sample(n_samples)
 
@@ -637,17 +592,15 @@
     kmeans_loss: float = 1.0,
     input_type: str = False,
     cp: bool = False,
     logparam: dict = None,
     outpath: str = ".",
     run: int = False,
 ) -> List[Union[Any]]:
-    """
-
-    Generates callbacks used for model training.
+    """Generate callbacks used for model training.
 
     Args:
         embedding_model (str): name of the embedding model
         encoder_type (str): Architecture used for the encoder. Must be one of "recurrent", "TCN", and "transformer"
         kmeans_loss (float): Weight of the gram loss
         input_type (str): Input type to use for training
         cp (bool): Whether to use checkpointing or not
@@ -655,15 +608,14 @@
         outpath (str): Path to the output directory
         run (int): Run number to use for checkpointing
 
     Returns:
         List[Union[Any]]: List of callbacks to be used for training
 
     """
-
     run_ID = "{}{}{}{}{}{}{}".format(
         "deepof_unsupervised_{}_{}_encodings".format(embedding_model, encoder_type),
         ("_input_type={}".format(input_type if input_type else "coords")),
         ("_kmeans_loss={}".format(kmeans_loss)),
         ("_encoding={}".format(logparam["latent_dim"]) if logparam is not None else ""),
         ("_k={}".format(logparam["n_components"]) if logparam is not None else ""),
         ("_run={}".format(run) if run else ""),
@@ -691,101 +643,81 @@
         )
         callbacks.append(cp_callback)
 
     return callbacks
 
 
 class CustomStopper(tf.keras.callbacks.EarlyStopping):
-    """
-
-    Custom early stopping callback. Prevents the model from stopping before warmup is over.
-
-    """
+    """Custom early stopping callback. Prevents the model from stopping before warmup is over."""
 
     def __init__(self, start_epoch, *args, **kwargs):
-        """
-
-        Initializes the CustomStopper callback.
+        """Initialize the CustomStopper callback.
 
         Args:
             start_epoch: epoch from which performance will be taken into account when deciding whether to stop training.
             *args: arguments passed to the callback.
             **kwargs: keyword arguments passed to the callback.
 
         """
         super(CustomStopper, self).__init__(*args, **kwargs)
         self.start_epoch = start_epoch
 
     def get_config(self):  # pragma: no cover
-        """
-
-        Updates callback metadata
-
-        """
-
+        """Update callback metadata."""
         config = super().get_config().copy()
         config.update({"start_epoch": self.start_epoch})
         return config
 
     def on_epoch_end(self, epoch, logs=None):
-
+        """Check whether to stop training."""
         if epoch > self.start_epoch:
             super().on_epoch_end(epoch, logs)
 
 
 class ExponentialLearningRate(tf.keras.callbacks.Callback):
-    """
+    """Simple class that allows to grow learning rate exponentially during training.
 
-    Simple class that allows to grow learning rate exponentially during training.
     Used to trigger optimal learning rate search in deepof.train_utils.find_learning_rate.
 
     """
 
     def __init__(self, factor: float):
-        """
-
-        Initializes the exponential learning rate callback
+        """Initialize the exponential learning rate callback.
 
         Args:
             factor(float): factor by which to multiply the learning rate
 
         """
         super().__init__()
         self.factor = factor
         self.rates = []
         self.losses = []
 
     # noinspection PyMethodOverriding
     def on_batch_end(self, batch: int, logs: dict):
-        """
-
-        This callback acts after processing each batch
+        """Apply on batch end.
 
         Args:
             batch: batch number
             logs (dict): dictionary containing the loss for the current batch
 
         """
-
         self.rates.append(K.get_value(self.model.optimizer.lr))
         if "total_loss" in logs.keys():
             self.losses.append(logs["total_loss"])
         else:
             self.losses.append(logs["loss"])
         K.set_value(self.model.optimizer.lr, self.model.optimizer.lr * self.factor)
 
 
 class ProbabilisticDecoder(tf.keras.layers.Layer):
-    """
-
-    Maps the reconstruction output of a given decoder to a multivariate normal distribution.
-
-    """
+    """Map the reconstruction output of a given decoder to a multivariate normal distribution."""
 
     def __init__(self, input_shape, **kwargs):
+        """Initialize the probabilistic decoder."""
         super().__init__(**kwargs)
         self.time_distributer = tf.keras.layers.Dense(
             tfpl.IndependentNormal.params_size(input_shape[1:]) // 2
         )
         self.probabilistic_decoding = tfpl.DistributionLambda(
             make_distribution_fn=lambda decoded: tfd.Masked(
                 tfd.Independent(
@@ -810,98 +742,82 @@
                 ),
                 validity_mask=decoded[1],
             ),
             convert_to_tensor_fn="mean",
         )
 
     def call(self, inputs):  # pragma: no cover
-        """
-
-        Maps the reconstruction output of a given decoder to a multivariate normal distribution.
+        """Map the reconstruction output of a given decoder to a multivariate normal distribution.
 
         Args:
             inputs (tuple): tuple containing the reconstruction output and the validity mask
 
         Returns:
             tf.Tensor: multivariate normal distribution
 
         """
-
         hidden, validity_mask = inputs
 
         hidden = tf.keras.layers.TimeDistributed(self.time_distributer)(hidden)
         prob_decoded = self.probabilistic_decoding([hidden, validity_mask])
         scaled_prob_decoded = self.scaled_probabilistic_decoding(
             [prob_decoded, validity_mask]
         )
 
         return scaled_prob_decoded
 
 
 class ClusterControl(tf.keras.layers.Layer):
-    """
+    """Identity layer.
 
-    Identity layer that evaluates different clustering metrics between the components of the latent Gaussian Mixture
+    Evaluates different clustering metrics between the components of the latent Gaussian Mixture
     using the entropy of the nearest neighbourhood. If self.loss_weight > 0, it also adds a regularization
     penalty to the loss function which attempts to maximize the number of populated clusters during training.
 
     """
 
     def __init__(
         self,
         batch_size: int,
         n_components: int,
         encoding_dim: int,
         k: int = 15,
         *args,
         **kwargs,
     ):
-        """
-
-        Initializes the ClusterControl layer
+        """Initialize the ClusterControl layer.
 
         Args:
             batch_size (int): batch size of the model
             n_components (int): number of components in the latent Gaussian Mixture
             encoding_dim (int): dimension of the latent Gaussian Mixture
             k (int): number of nearest components of the latent Gaussian Mixture to consider
-            loss_weight (float): weight of the regularization penalty applied to the local entropy of each
-            training instance
+            loss_weight (float): weight of the regularization penalty applied to the local entropy of each training instance
             *args: additional positional arguments
             **kwargs: additional keyword arguments
 
         """
         super(ClusterControl, self).__init__(*args, **kwargs)
         self.batch_size = batch_size
         self.n_components = n_components
         self.enc = encoding_dim
         self.k = k
 
     def get_config(self):  # pragma: no cover
-        """
-
-        Updates Constraint metadata
-
-        """
-
+        """Update Constraint metadata."""
         config = super().get_config().copy()
         config.update({"batch_size": self.batch_size})
         config.update({"n_components": self.n_components})
         config.update({"enc": self.enc})
         config.update({"k": self.k})
         config.update({"loss_weight": self.loss_weight})
         return config
 
     def call(self, inputs):  # pragma: no cover
-        """
-
-        Updates Layer's call method
-
-        """
-
+        """Update Layer's call method."""
         encodings, categorical = inputs[0], inputs[1]
 
         hard_groups = tf.math.argmax(categorical, axis=1)
         max_groups = tf.reduce_max(categorical, axis=1)
 
         n_components = tf.cast(
             tf.shape(
@@ -915,30 +831,25 @@
             max_groups, aggregation="mean", name="confidence_in_selected_cluster"
         )
 
         return encodings
 
 
 class TransformerEncoderLayer(tf.keras.layers.Layer):
-    """
-
-    Transformer encoder layer. Based on https://www.tensorflow.org/text/tutorials/transformer.
-
-    """
+    """Transformer encoder layer. Based on https://www.tensorflow.org/text/tutorials/transformer."""
 
     def __init__(self, key_dim, num_heads, dff, rate=0.1):
-        """
-
-        Constructor for the transformer encoder layer.
+        """Construct the transformer encoder layer.
 
         Args:
             key_dim: dimensionality of the time series
             num_heads: number of heads of the multi-head-attention layers
             dff: dimensionality of the embeddings
             rate: dropout rate
+
         """
         super(TransformerEncoderLayer, self).__init__()
 
         self.mha = tf.keras.layers.MultiHeadAttention(
             num_heads=num_heads, key_dim=key_dim
         )
         self.ffn = tf.keras.Sequential(
@@ -952,15 +863,16 @@
 
         self.layernorm1 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
         self.layernorm2 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
 
         self.dropout1 = tf.keras.layers.Dropout(rate)
         self.dropout2 = tf.keras.layers.Dropout(rate)
 
-    def call(self, x, training, mask, return_scores=False):
+    def call(self, x, training, mask, return_scores=False):  # pragma: no cover
+        """Call the transformer encoder layer."""
         attn_output, attn_scores = self.mha(
             key=x, query=x, value=x, attention_mask=mask, return_attention_scores=True
         )  # (batch_size, input_seq_len, d_model)
         attn_output = self.dropout1(attn_output, training=training)
         out1 = self.layernorm1(x + attn_output)
 
         ffn_output = self.ffn(out1)
@@ -970,30 +882,25 @@
         if return_scores:  # pragma: no cover
             return out2, attn_scores
 
         return out2
 
 
 class TransformerDecoderLayer(tf.keras.layers.Layer):
-    """
-
-    Transformer decoder layer. Based on https://www.tensorflow.org/text/tutorials/transformer.
-
-    """
+    """Transformer decoder layer. Based on https://www.tensorflow.org/text/tutorials/transformer."""
 
     def __init__(self, key_dim, num_heads, dff, rate=0.1):
-        """
-
-        Constructor for the transformer decoder layer.
+        """Construct the transformer decoder layer.
 
         Args:
             key_dim: dimensionality of the time series
             num_heads: number of heads of the multi-head-attention layers
             dff: dimensionality of the embeddings
             rate: dropout rate
+
         """
         super(TransformerDecoderLayer, self).__init__()
 
         self.mha1 = tf.keras.layers.MultiHeadAttention(
             num_heads=num_heads, key_dim=key_dim
         )
         self.mha2 = tf.keras.layers.MultiHeadAttention(
@@ -1014,15 +921,15 @@
         self.dropout1 = tf.keras.layers.Dropout(rate)
         self.dropout2 = tf.keras.layers.Dropout(rate)
         self.dropout3 = tf.keras.layers.Dropout(rate)
 
     def call(
         self, x, enc_output, training, look_ahead_mask, padding_mask
     ):  # pragma: no cover
-
+        """Call the transformer decoder layer."""
         attn1, attn_weights_block1 = self.mha1(
             key=x,
             query=x,
             value=x,
             attention_mask=look_ahead_mask,
             return_attention_scores=True,
         )  # (batch_size, target_seq_len, d_model)
@@ -1044,17 +951,17 @@
         out3 = self.layernorm3(ffn_output + out2)
 
         return out3, attn_weights_block1, attn_weights_block2
 
 
 # noinspection PyCallingNonCallable
 class TransformerEncoder(tf.keras.layers.Layer):
-    """
+    """Transformer encoder.
 
-    Transformer encoder. Based on https://www.tensorflow.org/text/tutorials/transformer.
+    Based on https://www.tensorflow.org/text/tutorials/transformer.
     Adapted according to https://academic.oup.com/gigascience/article/8/11/giz134/5626377?login=true
     and https://arxiv.org/abs/1711.03905.
 
     """
 
     def __init__(
         self,
@@ -1062,26 +969,25 @@
         seq_dim,
         key_dim,
         num_heads,
         dff,
         maximum_position_encoding,
         rate=0.1,
     ):
-        """
-
-        Constructor for the transformer encoder.
+        """Construct the transformer encoder.
 
         Args:
             num_layers: number of transformer layers to include.
             seq_dim: dimensionality of the sequence embeddings
             key_dim: dimensionality of the time series
             num_heads: number of heads of the multi-head-attention layers used on the transformer encoder
             dff: dimensionality of the token embeddings
             maximum_position_encoding: maximum time series length
             rate: dropout rate
+
         """
         super(TransformerEncoder, self).__init__()
 
         self.rate = rate
         self.key_dim = key_dim
         self.num_layers = num_layers
         self.embedding = tf.keras.layers.Conv1D(
@@ -1090,16 +996,16 @@
         self.pos_encoding = positional_encoding(maximum_position_encoding, self.key_dim)
         self.enc_layers = [
             TransformerEncoderLayer(key_dim, num_heads, dff, rate)
             for _ in range(num_layers)
         ]
         self.dropout = tf.keras.layers.Dropout(self.rate)
 
-    def call(self, x, training):
-
+    def call(self, x, training):  # pragma: no cover
+        """Call the transformer encoder."""
         # compute mask on the fly
         mask, _, _ = create_masks(x)
         seq_len = tf.shape(x)[1]
 
         # adding embedding and position encoding.
         x = self.embedding(x)
         x *= tf.math.sqrt(tf.cast(self.key_dim, tf.float32))
@@ -1110,42 +1016,43 @@
             x = self.enc_layers[i](x, training, mask)
 
         return x
 
 
 # noinspection PyCallingNonCallable
 class TransformerDecoder(tf.keras.layers.Layer):
-    """
-    Transformer decoder. Based on https://www.tensorflow.org/text/tutorials/transformer.
+    """Transformer decoder.
+
+    Based on https://www.tensorflow.org/text/tutorials/transformer.
     Adapted according to https://academic.oup.com/gigascience/article/8/11/giz134/5626377?login=true
     and https://arxiv.org/abs/1711.03905.
+
     """
 
     def __init__(
         self,
         num_layers,
         seq_dim,
         key_dim,
         num_heads,
         dff,
         maximum_position_encoding,
         rate=0.1,
     ):
-        """
-
-        Constructor for the transformer decoder.
+        """Construct the transformer decoder.
 
         Args:
             num_layers: number of transformer layers to include.
             seq_dim: dimensionality of the sequence embeddings
             key_dim: dimensionality of the time series
             num_heads: number of heads of the multi-head-attention layers used on the transformer encoder
             dff: dimensionality of the token embeddings
             maximum_position_encoding: maximum time series length
             rate: dropout rate
+
         """
         super(TransformerDecoder, self).__init__()
 
         self.rate = rate
         self.key_dim = key_dim
         self.num_layers = num_layers
         self.embedding = tf.keras.layers.Conv1D(
@@ -1157,15 +1064,15 @@
             for _ in range(num_layers)
         ]
         self.dropout = tf.keras.layers.Dropout(self.rate)
 
     def call(
         self, x, enc_output, training, look_ahead_mask, padding_mask
     ):  # pragma: no cover
-
+        """Call the transformer decoder."""
         seq_len = tf.shape(x)[1]
         attention_weights = {}
         x = self.embedding(x)
         x *= tf.math.sqrt(tf.cast(self.key_dim, tf.float32))
         x += self.pos_encoding[:, :seq_len, :]
         x = self.dropout(x, training=training)
 
@@ -1176,24 +1083,23 @@
             attention_weights["decoder_layer{}_block1".format(i + 1)] = block1
             attention_weights["decoder_layer{}_block2".format(i + 1)] = block2
 
         return x, attention_weights
 
 
 def log_hyperparameters():
-    """
+    """Log hyperparameters in tensorboard.
 
     Blueprint for hyperparameter and metric logging in tensorboard during hyperparameter tuning
 
     Returns:
         logparams (list): List containing the hyperparameters to log in tensorboard.
         metrics (list): List containing the metrics to log in tensorboard.
 
     """
-
     logparams = [
         hp.HParam(
             "latent_dim",
             hp.Discrete([2, 4, 6, 8, 12, 16]),
             display_name="latent_dim",
             description="encoding size dimensionality",
         ),
@@ -1261,38 +1167,35 @@
 
     Trains the specified embedding model on the preprocessed data.
 
     Args:
         coordinates (np.ndarray): Coordinates of the data.
         preprocessed_object (tuple): Tuple containing the preprocessed data.
         adjacency_matrix (np.ndarray): adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-        embedding_model (str): Model to use to embed and cluster the data. Must be one of VQVAE (default), VaDE,
-        and contrastive.
+        embedding_model (str): Model to use to embed and cluster the data. Must be one of VQVAE (default), VaDE, and contrastive.
         encoder_type (str): Encoder architecture to use. Must be one of "recurrent", "TCN", and "transformer".
         batch_size (int): Batch size to use for training.
         latent_dim (int): Encoding size to use for training.
         epochs (int): Number of epochs to train the autoencoder for.
         log_history (bool): Whether to log the history of the autoencoder.
         log_hparams (bool): Whether to log the hyperparameters used for training.
         n_components (int): Number of components to fit to the data.
         output_path (str): Path to the output directory.
-        kmeans_loss (float): Weight of the gram loss, which adds a regularization term to VQVAE models which
-        penalizes the correlation between the dimensions in the latent space.
+        kmeans_loss (float): Weight of the gram loss, which adds a regularization term to VQVAE models which penalizes the correlation between the dimensions in the latent space.
         pretrained (str): Path to the pretrained weights to use for the autoencoder.
         save_checkpoints (bool): Whether to save checkpoints during training.
         save_weights (bool): Whether to save the weights of the autoencoder after training.
         input_type (str): Input type of the TableDict objects used for preprocessing. For logging purposes only.
         interaction_regularization (float): Weight of the interaction regularization term (L1 penalization to all features not related to interactions).
         run (int): Run number to use for logging.
 
         # VaDE Model specific parameters
         kl_annealing_mode (str): Mode to use for KL annealing. Must be one of "linear" (default), or "sigmoid".
         kl_warmup (int): Number of epochs during which KL is annealed.
-        reg_cat_clusters (bool): whether to penalize uneven cluster membership in the latent space, by
-        minimizing the KL divergence between cluster membership and a uniform categorical distribution.
+        reg_cat_clusters (bool): whether to penalize uneven cluster membership in the latent space, by minimizing the KL divergence between cluster membership and a uniform categorical distribution.
         recluster (bool): Whether to recluster the data after each training using a Gaussian Mixture Model.
 
         # Contrastive Model specific parameters
         temperature (float): temperature parameter for the contrastive loss functions. Higher values put harsher penalties on negative pair similarity.
         contrastive_similarity_function (str): similarity function between positive and negative pairs. Must be one of 'cosine' (default), 'euclidean', 'dot', and 'edit'.
         contrastive_loss_function (str): contrastive loss function. Must be one of 'nce' (default), 'dcl', 'fc', and 'hard_dcl'. See specific documentation for details.
         beta (float): Beta (concentration) parameter for the hard_dcl contrastive loss. Higher values lead to 'harder' negative samples.
@@ -1557,70 +1460,102 @@
     coordinates: coordinates,
     to_preprocess: table_dict,
     model: tf.keras.models.Model,
     scale: str = "standard",
     animal_id: str = None,
     ruptures: bool = False,
     global_scaler: Any = None,
+    **kwargs,
 ):  # pragma: no cover
-    """Uses a previously trained model to produce embeddings, soft_counts and breaks per experiment in table_dict format.
+    """Use a previously trained model to produce embeddings, soft_counts and breaks per experiment in table_dict format.
 
     Args:
         coordinates (coordinates): deepof.Coordinates object for the project at hand.
         to_preprocess (table_dict): dictionary with (merged) features to process.
-        scale (str): The type of scaler to use within animals. Defaults to 'standard', but can be changed to 'minmax', 'robust', or False.
-        Use the same that was used when training the original model.
+        scale (str): The type of scaler to use within animals. Defaults to 'standard', but can be changed to 'minmax', 'robust', or False. Use the same that was used when training the original model.
         animal_id (str): if more than one animal is present, provide the ID(s) of the animal(s) to include.
-        ruptures (bool): Whether to compute the breaks based on ruptures (with the length of all retrieved chunks
-        per experiment) or not (an all-ones vector per experiment is returned).
+        ruptures (bool): Whether to compute the breaks based on ruptures (with the length of all retrieved chunks per experiment) or not (an all-ones vector per experiment is returned).
         global_scaler (Any): trained global scaler produced when processing the original dataset.
         model (tf.keras.models.Model): trained deepof unsupervised model to run inference with.
+        **kwargs: additional arguments to pass to coordinates.get_graph_dataset().
 
     Returns:
         embeddings (table_dict): embeddings per experiment.
         soft_counts (table_dict): soft_counts per experiment.
         breaks (table_dict): breaks per experiment.
 
     """
     embeddings = {}
     soft_counts = {}
     breaks = {}
 
+    graph, contrastive = False, False
+    try:
+        if any([isinstance(i, CensNetConv) for i in model.encoder.layers[2].layers]):
+            graph = True
+    except AttributeError:
+        if any([isinstance(i, CensNetConv) for i in model.encoder.layers]):
+            graph, contrastive = True, True
+
+    window_size = model.layers[0].input_shape[0][1]
     for key in tqdm.tqdm(to_preprocess.keys()):
 
-        if any([isinstance(i, CensNetConv) for i in model.encoder.layers[2].layers]):
+        if graph:
             processed_exp, _, _, _ = coordinates.get_graph_dataset(
                 animal_id=animal_id,
                 precomputed_tab_dict=to_preprocess.filter_videos([key]),
                 preprocess=True,
                 scale=scale,
-                window_size=model.layers[0].input_shape[0][1],
+                window_size=window_size,
                 window_step=1,
                 shuffle=False,
                 pretrained_scaler=global_scaler,
             )
 
         else:
 
             processed_exp, _ = to_preprocess.filter_videos([key]).preprocess(
                 scale=scale,
-                window_size=model.layers[0].input_shape[0][1],
+                window_size=window_size,
                 window_step=1,
                 shuffle=False,
                 pretrained_scaler=global_scaler,
             )
 
         embeddings[key] = model.encoder([processed_exp[0], processed_exp[1]]).numpy()
-        soft_counts[key] = model.grouper([processed_exp[0], processed_exp[1]]).numpy()
         if ruptures:
             breaks[key] = (~np.all(processed_exp[0] == 0, axis=2)).sum(axis=1)
         else:
-            breaks[key] = np.ones(soft_counts[key].shape[0]).astype(int)
+            breaks[key] = np.ones(embeddings[key].shape[0]).astype(int)
 
-    return embeddings, soft_counts, breaks
+        if not contrastive:
+            soft_counts[key] = model.grouper(
+                [processed_exp[0], processed_exp[1]]
+            ).numpy()
+
+    if contrastive:
+        soft_counts = deepof.post_hoc.recluster(coordinates, embeddings, **kwargs)
+
+    return (
+        deepof.data.TableDict(
+            embeddings,
+            typ="unsupervised_embedding",
+            exp_conditions=coordinates.get_exp_conditions,
+        ),
+        deepof.data.TableDict(
+            soft_counts,
+            typ="unsupervised_counts",
+            exp_conditions=coordinates.get_exp_conditions,
+        ),
+        deepof.data.TableDict(
+            breaks,
+            typ="unsupervised_breaks",
+            exp_conditions=coordinates.get_exp_conditions,
+        ),
+    )
 
 
 def tune_search(
     preprocessed_object: tuple,
     adjacency_matrix: np.ndarray,
     encoding_size: int,
     embedding_model: str,
@@ -1630,42 +1565,37 @@
     project_name: str,
     callbacks: List,
     batch_size: int = 1024,
     n_epochs: int = 30,
     n_replicas: int = 1,
     outpath: str = "unsupervised_tuner_search",
 ) -> tuple:
-    """
-
-    Define the search space using keras-tuner and hyperband or bayesian optimization
+    """Define the search space using keras-tuner and hyperband or bayesian optimization.
 
     Args:
         preprocessed_object (tf.data.Dataset): Dataset object for training and validation.
         adjacency_matrix (np.ndarray): Adjacency matrix for the graph.
         encoding_size (int): Size of the encoding layer.
-        embedding_model (str): Model to use to embed and cluster the data. Must be one of VQVAE (default), VaDE,
-        and Contrastive.
+        embedding_model (str): Model to use to embed and cluster the data. Must be one of VQVAE (default), VaDE, and Contrastive.
         hypertun_trials (int): Number of hypertuning trials to run.
         hpt_type (str): Type of hypertuning to run. Must be one of "hyperband" or "bayesian".
         k (int): Number of clusters on the latent space.
-        kmeans_loss (float): Weight of the kmeans loss, which enforces disentanglement by penalizing the correlation
-        between dimensions in the latent space.
+        kmeans_loss (float): Weight of the kmeans loss, which enforces disentanglement by penalizing the correlation between dimensions in the latent space.
         project_name (str): Name of the project.
         callbacks (List): List of callbacks to use.
         batch_size (int): Batch size to use.
         n_epochs (int): Maximum number of epochs to train for.
         n_replicas (int): Number of replicas to use.
         outpath (str): Path to save the results.
 
     Returns:
         best_hparams (dict): Dictionary of the best hyperparameters.
         best_run (str): Name of the best run.
 
     """
-
     # Load data
     try:
         X_train, a_train, y_train, X_val, a_val, y_val = preprocessed_object
     except ValueError:
         X_train, y_train, X_val, y_val = preprocessed_object
         a_train, a_val = np.zeros(X_train.shape), np.zeros(X_val.shape)
```

### Comparing `deepof-0.2/deepof/models.py` & `deepof-0.3/deepof/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,28 @@
     adjacency_matrix: np.ndarray,
     latent_dim: int,
     use_gnn: bool = True,
     gru_unroll: bool = False,
     bidirectional_merge: str = "concat",
     interaction_regularization: float = 0.0,
 ):
-    """Returns a deep recurrent neural encoder.
+    """Return a deep recurrent neural encoder.
 
      Builds a neural network capable of encoding the motion tracking instances into a vector ready to be fed to
     one of the provided structured latent spaces.
 
     Args:
-        - input_shape (tuple): shape of the node features for the input data. Should be time x nodes x features.
-        - edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers.
-        Should be time x edges x features.
-        - adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
-        - latent_dim (int): dimension of the latent space.
-        - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-        as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-        - gru_unroll (bool): whether to unroll the GRU layers. Defaults to False.
-        - bidirectional_merge (str): how to merge the forward and backward GRU layers. Defaults to "concat".
-        - interaction_regularization (float): Regularization parameter for the interaction features.
+        input_shape (tuple): shape of the node features for the input data. Should be time x nodes x features.
+        edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers. Should be time x edges x features.
+        adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
+        latent_dim (int): dimension of the latent space.
+        use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+        gru_unroll (bool): whether to unroll the GRU layers. Defaults to False.
+        bidirectional_merge (str): how to merge the forward and backward GRU layers. Defaults to "concat".
+        interaction_regularization (float): Regularization parameter for the interaction features.
 
     Returns:
         keras.Model: a keras model that can be trained to encode motion tracking instances into a vector.
 
     """
     # Define feature and adjacency inputs
     x = Input(shape=input_shape)
@@ -153,29 +151,30 @@
 # noinspection PyCallingNonCallable
 def get_recurrent_decoder(
     input_shape: tuple,
     latent_dim: int,
     gru_unroll: bool = False,
     bidirectional_merge: str = "concat",
 ):
-    """Returns a recurrent neural decoder.
+    """Return a recurrent neural decoder.
 
     Builds a deep neural network capable of decoding the structured latent space generated by one of the compatible
     classes into a sequence of motion tracking instances, either reconstructing the original
     input, or generating new data from given clusters.
 
     Args:
         input_shape (tuple): shape of the input data
         latent_dim (int): dimensionality of the latent space
         gru_unroll (bool): whether to unroll the GRU layers. Defaults to False.
         bidirectional_merge (str): how to merge the forward and backward GRU layers. Defaults to "concat".
 
     Returns:
         keras.Model: a keras model that can be trained to decode the latent space into a series of motion tracking
         sequences.
+
     """
     # Define and instantiate generator
     g = Input(shape=latent_dim)  # Decoder input, shaped as the latent space
     x = Input(shape=input_shape)  # Encoder input, used to generate an output mask
     validity_mask = tf.math.logical_not(tf.reduce_all(x == 0.0, axis=2))
 
     generator = RepeatVector(input_shape[0])(g)
@@ -233,40 +232,40 @@
     conv_dilations: tuple = (1, 2, 4, 8),
     padding: str = "causal",
     use_skip_connections: bool = True,
     dropout_rate: int = 0,
     activation: str = "relu",
     interaction_regularization: float = 0.0,
 ):
-    """Returns a Temporal Convolutional Network (TCN) encoder.
+    """Return a Temporal Convolutional Network (TCN) encoder.
 
     Builds a neural network that can be used to encode motion tracking instances into a
     vector. Each layer contains a residual block with a convolutional layer and a skip connection. See the following
     paper for more details: https://arxiv.org/pdf/1803.01271.pdf
 
     Args:
-        - input_shape: shape of the input data
-        - edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers. Should be time x edges x features.
-        - adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
-        - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-        as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-        - latent_dim: dimensionality of the latent space
-        - conv_filters: number of filters in the TCN layers
-        - kernel_size: size of the convolutional kernels
-        - conv_stacks: number of TCN layers
-        - conv_dilations: list of dilation factors for each TCN layer
-        - padding: padding mode for the TCN layers
-        - use_skip_connections: whether to use skip connections between TCN layers
-        - dropout_rate: dropout rate for the TCN layers
-        - activation: activation function for the TCN layers
-        - interaction_regularization (float): Regularization parameter for the interaction features
+        input_shape: shape of the input data
+        edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers. Should be time x edges x features.
+        adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
+        use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+        latent_dim: dimensionality of the latent space
+        conv_filters: number of filters in the TCN layers
+        kernel_size: size of the convolutional kernels
+        conv_stacks: number of TCN layers
+        conv_dilations: list of dilation factors for each TCN layer
+        padding: padding mode for the TCN layers
+        use_skip_connections: whether to use skip connections between TCN layers
+        dropout_rate: dropout rate for the TCN layers
+        activation: activation function for the TCN layers
+        interaction_regularization (float): Regularization parameter for the interaction features
 
     Returns:
         keras.Model: a keras model that can be trained to encode a sequence of motion tracking instances into a latent
         space using temporal convolutional networks.
+
     """
     # Define feature and adjacency inputs
     x = Input(shape=input_shape)
     a = Input(shape=edge_feature_shape)
 
     if use_gnn:
         x_reshaped = tf.transpose(
@@ -380,35 +379,36 @@
     conv_stacks: int = 1,
     conv_dilations: tuple = (8, 4, 2, 1),
     padding: str = "causal",
     use_skip_connections: bool = True,
     dropout_rate: int = 0,
     activation: str = "relu",
 ):
-    """Returns a Temporal Convolutional Network (TCN) decoder.
+    """Return a Temporal Convolutional Network (TCN) decoder.
 
     Builds a neural network that can be used to decode a latent space into a sequence of
     motion tracking instances. Each layer contains a residual block with a convolutional layer and a skip connection. See
     the following paper for more details: https://arxiv.org/pdf/1803.01271.pdf,
 
     Args:
-        - input_shape: shape of the input data
-        - latent_dim: dimensionality of the latent space
-        - conv_filters: number of filters in the TCN layers
-        - kernel_size: size of the convolutional kernels
-        - conv_stacks: number of TCN layers
-        - conv_dilations: list of dilation factors for each TCN layer
-        - padding: padding mode for the TCN layers
-        - use_skip_connections: whether to use skip connections between TCN layers
-        - dropout_rate: dropout rate for the TCN layers
-        - activation: activation function for the TCN layers
+        input_shape: shape of the input data
+        latent_dim: dimensionality of the latent space
+        conv_filters: number of filters in the TCN layers
+        kernel_size: size of the convolutional kernels
+        conv_stacks: number of TCN layers
+        conv_dilations: list of dilation factors for each TCN layer
+        padding: padding mode for the TCN layers
+        use_skip_connections: whether to use skip connections between TCN layers
+        dropout_rate: dropout rate for the TCN layers
+        activation: activation function for the TCN layers
 
     Returns:
         keras.Model: a keras model that can be trained to decode a latent space into a sequence of motion tracking
         instances using temporal convolutional networks.
+
     """
     # Define and instantiate generator
     g = Input(shape=latent_dim)  # Decoder input, shaped as the latent space
     x = Input(shape=input_shape)  # Encoder input, used to generate an output mask
     validity_mask = tf.math.logical_not(tf.reduce_all(x == 0.0, axis=2))
 
     generator = tf.keras.layers.Dense(latent_dim)(g)
@@ -449,32 +449,32 @@
     use_gnn: bool = True,
     num_layers: int = 4,
     num_heads: int = 64,
     dff: int = 128,
     dropout_rate: float = 0.1,
     interaction_regularization: float = 0.0,
 ):
-    """Transformer encoder.
+    """Build a Transformer encoder.
 
     Based on https://www.tensorflow.org/text/tutorials/transformer.
     Adapted according to https://academic.oup.com/gigascience/article/8/11/giz134/5626377?login=true
     and https://arxiv.org/abs/1711.03905.
 
     Args:
-        - input_shape (tuple): shape of the input data
-        - edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers. Should be time x edges x features.
-        - adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
-        - latent_dim (int): dimensionality of the latent space
-        - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-        as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-        - num_layers (int): number of transformer layers to include
-        - num_heads (int): number of heads of the multi-head-attention layers used on the transformer encoder
-        - dff (int): dimensionality of the token embeddings
-        - dropout_rate (float): dropout rate
-        - interaction_regularization (float): regularization parameter for the interaction features
+        input_shape (tuple): shape of the input data
+        edge_feature_shape (tuple): shape of the adjacency matrix to use in the graph attention layers. Should be time x edges x features.
+        adjacency_matrix (np.ndarray): adjacency matrix for the mice connectivity graph. Shape should be nodes x nodes.
+        latent_dim (int): dimensionality of the latent space
+        use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+        num_layers (int): number of transformer layers to include
+        num_heads (int): number of heads of the multi-head-attention layers used on the transformer encoder
+        dff (int): dimensionality of the token embeddings
+        dropout_rate (float): dropout rate
+        interaction_regularization (float): regularization parameter for the interaction features
+
     """
     # Define feature and adjacency inputs
     x = Input(shape=input_shape)
     a = Input(shape=edge_feature_shape)
 
     if use_gnn:
         x_reshaped = tf.transpose(
@@ -590,27 +590,28 @@
 
     return tf.keras.models.Model([x, a], encoder, name="transformer_encoder")
 
 
 def get_transformer_decoder(
     input_shape, latent_dim, num_layers=2, num_heads=8, dff=128, dropout_rate=0.1
 ):
-    """Transformer decoder.
+    """Build a Transformer decoder.
 
     Based on https://www.tensorflow.org/text/tutorials/transformer.
     Adapted according to https://academic.oup.com/gigascience/article/8/11/giz134/5626377?login=true
     and https://arxiv.org/abs/1711.03905.
 
     Args:
         input_shape (tuple): shape of the input data
         latent_dim (int): dimensionality of the latent space
         num_layers (int): number of transformer layers to include
         num_heads (int): number of heads of the multi-head-attention layers used on the transformer encoder
         dff (int): dimensionality of the token embeddings
         dropout_rate (float): dropout rate
+
     """
     x = tf.keras.layers.Input(input_shape)
     g = tf.keras.layers.Input([latent_dim])
     validity_mask = tf.math.logical_not(tf.reduce_all(x == 0.0, axis=2))
 
     generator = tf.keras.layers.Dense(latent_dim)(g)
     generator = tf.keras.layers.BatchNormalization()(generator)
@@ -656,22 +657,23 @@
     Implementation based on https://keras.io/examples/generative/vq_vae/.
 
     """
 
     def __init__(
         self, n_components, embedding_dim, beta, kmeans_loss: float = 0.0, **kwargs
     ):
-        """Initializes the VQ layer.
+        """Initialize the VQ layer.
 
         Args:
             n_components (int): number of embeddings to use
             embedding_dim (int): dimensionality of the embeddings
             beta (float): beta value for the loss function
             kmeans_loss (float): regularization parameter for the Gram matrix
             **kwargs: additional arguments for the parent class
+
         """
         super(VectorQuantizer, self).__init__(**kwargs)
         self.embedding_dim = embedding_dim
         self.n_components = n_components
         self.beta = beta
         self.kmeans = kmeans_loss
 
@@ -682,15 +684,15 @@
                 shape=(self.embedding_dim, self.n_components), dtype="float32"
             ),
             trainable=True,
             name="vqvae_codebook",
         )
 
     def call(self, x):  # pragma: no cover
-        """Computes the VQ layer.
+        """Compute the VQ layer.
 
         Args:
             x (tf.Tensor): input tensor
 
         Returns:
                 x (tf.Tensor): output tensor
         """
@@ -736,16 +738,15 @@
     def get_code_indices(
         self, flattened_inputs, return_soft_counts=False
     ):  # pragma: no cover
         """Getter for the code indices at any given time.
 
         Args:
             flattened_inputs (tf.Tensor): flattened input tensor (encoder output)
-            return_soft_counts (bool): whether to return soft counts based on the distance to the codes, instead of
-            the code indices
+            return_soft_counts (bool): whether to return soft counts based on the distance to the codes, instead of the code indices
 
         Returns:
             encoding_indices (tf.Tensor): code indices tensor with cluster assignments.
         """
         # Compute L2-norm distance between inputs and codes at a given time
         similarity = tf.matmul(flattened_inputs, self.codebook)
         distances = (
@@ -776,36 +777,34 @@
     use_gnn: bool,
     n_components: int,
     beta: float = 1.0,
     kmeans_loss: float = 0.0,
     encoder_type: str = "recurrent",
     interaction_regularization: float = 0.0,
 ):
-    """Builds a Vector-Quantization variational autoencoder (VQ-VAE) model, adapted to the DeepOF setting.
+    """Build a Vector-Quantization variational autoencoder (VQ-VAE) model, adapted to the DeepOF setting.
 
     Args:
-        - input_shape (tuple): shape of the input to the encoder.
-        - edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
-        - adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-        - latent_dim (int): dimension of the latent space.
-        - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-        as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-        - n_components (int): number of embeddings in the embedding layer.
-        - beta (float): beta parameter of the VQ loss.
-        - kmeans_loss (float): regularization parameter for the Gram matrix.
-        - encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
-        - interaction_regularization (float): Regularization parameter for the interaction features.
+        input_shape (tuple): shape of the input to the encoder.
+        edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
+        adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
+        latent_dim (int): dimension of the latent space.
+        use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+        n_components (int): number of embeddings in the embedding layer.
+        beta (float): beta parameter of the VQ loss.
+        kmeans_loss (float): regularization parameter for the Gram matrix.
+        encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
+        interaction_regularization (float): Regularization parameter for the interaction features.
 
     Returns:
-        - encoder (tf.keras.Model): connected encoder of the VQ-VAE model.
-        Outputs a vector of shape (latent_dim,).
-        - decoder (tf.keras.Model): connected decoder of the VQ-VAE model.
-        - grouper (tf.keras.Model): connected embedder layer of the VQ-VAE model.
-        Outputs cluster indices of shape (batch_size,).
-        - vqvae (tf.keras.Model): complete VQ VAE model.
+        encoder (tf.keras.Model): connected encoder of the VQ-VAE model. Outputs a vector of shape (latent_dim,).
+        decoder (tf.keras.Model): connected decoder of the VQ-VAE model.
+        grouper (tf.keras.Model): connected embedder layer of the VQ-VAE model. Outputs cluster indices of shape (batch_size,).
+        vqvae (tf.keras.Model): complete VQ VAE model.
+
     """
     vq_layer = VectorQuantizer(
         n_components,
         latent_dim,
         beta=beta,
         kmeans_loss=kmeans_loss,
         name="vector_quantizer",
@@ -878,27 +877,28 @@
         beta: float = 1.0,
         kmeans_loss: float = 0.0,
         use_gnn: bool = True,
         encoder_type: str = "recurrent",
         interaction_regularization: float = 0.0,
         **kwargs,
     ):
-        """Initializes a VQ-VAE model.
+        """Initialize a VQ-VAE model.
 
         Args:
             input_shape (tuple): Shape of the input to the full model.
             edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
             adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
             latent_dim (int): Dimensionality of the latent space.
             n_components (int): Number of embeddings (clusters) in the embedding layer.
             beta (float): Beta parameter of the VQ loss, as described in the original VQVAE paper.
             kmeans_loss (float): Regularization parameter for the Gram matrix.
             encoder_type (str): Type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
             interaction_regularization (float): Regularization parameter for the interaction features.
             **kwargs: Additional keyword arguments.
+
         """
         super(VQVAE, self).__init__(**kwargs)
         self.seq_shape = input_shape
         self.edge_feature_shape = edge_feature_shape
         self.adjacency_matrix = adjacency_matrix
         self.latent_dim = latent_dim
         self.use_gnn = use_gnn
@@ -950,20 +950,20 @@
         self.val_vq_loss_tracker = tf.keras.metrics.Mean(name="val_vq_loss")
         self.val_cluster_population = tf.keras.metrics.Mean(
             name="val_number_of_populated_clusters"
         )
 
     @tf.function
     def call(self, inputs, **kwargs):
-        """Calls the VQVAE model."""
+        """Call the VQVAE model."""
         return self.vqvae(inputs, **kwargs)
 
     @property
     def metrics(self):  # pragma: no cover
-        """Initializes VQVAE tracked metrics."""
+        """Initialize VQVAE tracked metrics."""
         metrics = [
             self.total_loss_tracker,
             self.encoding_reconstruction_loss_tracker,
             self.reconstruction_loss_tracker,
             self.vq_loss_tracker,
             self.cluster_population,
             self.val_total_loss_tracker,
@@ -973,15 +973,15 @@
             self.val_cluster_population,
         ]
 
         return metrics
 
     @tf.function
     def train_step(self, data):  # pragma: no cover
-        """Performs a training step."""
+        """Perform a training step."""
         # Unpack data, repacking labels into a generator
         x, a, y = data
         if not isinstance(y, tuple):
             y = [y]
         y = (labels for labels in y)
 
         with tf.GradientTape() as tape:
@@ -1109,14 +1109,15 @@
 class GaussianMixtureLatent(tf.keras.models.Model):
     """Gaussian Mixture probabilistic latent space model.
 
     Used to represent the embedding of motion tracking data in a mixture of Gaussians
     with a provided number of components, with means, covariances and weights.
     Implementation based on VaDE (https://arxiv.org/abs/1611.05148)
     and VaDE-SC (https://openreview.net/forum?id=RQ428ZptQfU).
+
     """
 
     def __init__(
         self,
         input_shape: tuple,
         n_components: int,
         latent_dim: int,
@@ -1126,29 +1127,30 @@
         mc_kl: int = 100,
         mmd_warmup: int = 15,
         mmd_annealing_mode: str = "linear",
         kmeans_loss: float = 0.0,
         reg_cluster_variance: bool = False,
         **kwargs,
     ):
-        """Initializes the Gaussian Mixture Latent layer.
+        """Initialize the Gaussian Mixture Latent layer.
 
         Args:
             input_shape (tuple): shape of the input data
             n_components (int): number of components in the Gaussian mixture.
             latent_dim (int): dimensionality of the latent space.
             batch_size (int): batch size for training.
             kl_warmup (int): number of epochs to warm up the KL divergence.
             kl_annealing_mode (str): mode to use for annealing the KL divergence. Must be one of "linear" and "sigmoid".
             mc_kl (int): number of Monte Carlo samples to use for computing the KL divergence.
             mmd_warmup (int): number of epochs to warm up the MMD.
             mmd_annealing_mode (str): mode to use for annealing the MMD. Must be one of "linear" and "sigmoid".
             kmeans_loss (float): weight of the Gram matrix regularization loss.
             reg_cluster_variance (bool): whether to penalize uneven cluster variances in the latent space.
             **kwargs: keyword arguments passed to the parent class
+
         """
         super(GaussianMixtureLatent, self).__init__(**kwargs)
         self.seq_shape = input_shape
         self.n_components = n_components
         self.latent_dim = latent_dim
         self.batch_size = batch_size
         self.kl_warmup = kl_warmup
@@ -1202,15 +1204,15 @@
             self.kl_warmup * (self.seq_shape // self.batch_size), tf.int64
         )
         self._kl_weight = tf.Variable(
             1.0, trainable=False, dtype=tf.float32, name="kl_weight"
         )
 
     def call(self, inputs, training=False):  # pragma: no cover
-        """Computes the output of the layer."""
+        """Compute the output of the layer."""
         z_gauss_mean = self.z_gauss_mean(inputs)
         z_gauss_var = self.z_gauss_var(inputs)
 
         z = tfd.MultivariateNormalDiag(
             loc=z_gauss_mean, scale_diag=tf.math.sqrt(tf.math.exp(z_gauss_var))
         )
         z_sample = tf.squeeze(z.sample())
@@ -1317,40 +1319,38 @@
     kl_annealing_mode: str = "sigmoid",
     mc_kl: int = 100,
     kmeans_loss: float = 1.0,
     reg_cluster_variance: bool = False,
     encoder_type: str = "recurrent",
     interaction_regularization: float = 0.0,
 ):
-    """Builds a Gaussian mixture variational autoencoder (VaDE) model, adapted to the DeepOF setting.
+    """Build a Gaussian mixture variational autoencoder (VaDE) model, adapted to the DeepOF setting.
 
     Args:
-            - input_shape (tuple): shape of the input data.
-            - edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
-            - adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-            - latent_dim (int): dimensionality of the latent space.
-            - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-            as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-            - n_components (int): number of components in the Gaussian mixture.
-            - batch_size (int): batch size for training.
-            - kl_warmup: Number of iterations during which to warm up the KL divergence.
-            - kl_annealing_mode (str): mode to use for annealing the KL divergence. Must be one of "linear" and "sigmoid".
-            - mc_kl (int): number of Monte Carlo samples to use for computing the KL divergence.
-            - kmeans_loss (float): weight of the Gram matrix loss as described in deepof.model_utils.compute_kmeans_loss.
-            - reg_cluster_variance (bool): whether to penalize uneven cluster variances in the latent space.
-            - encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
-            - interaction_regularization (float): weight of the interaction regularization term.
+        input_shape (tuple): shape of the input data.
+        edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
+        adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
+        latent_dim (int): dimensionality of the latent space.
+        use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+        n_components (int): number of components in the Gaussian mixture.
+        batch_size (int): batch size for training.
+        kl_warmup (int): Number of iterations during which to warm up the KL divergence.
+        kl_annealing_mode (str): mode to use for annealing the KL divergence. Must be one of "linear" and "sigmoid".
+        mc_kl (int): number of Monte Carlo samples to use for computing the KL divergence.
+        kmeans_loss (float): weight of the Gram matrix loss as described in deepof.model_utils.compute_kmeans_loss.
+        reg_cluster_variance (bool): whether to penalize uneven cluster variances in the latent space.
+        encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
+        interaction_regularization (float): weight of the interaction regularization term.
 
     Returns:
-        - encoder (tf.keras.Model): connected encoder of the VQ-VAE model.
-        Outputs a vector of shape (latent_dim,).
-        - decoder (tf.keras.Model): connected decoder of the VQ-VAE model.
-        - grouper (tf.keras.Model): deep clustering branch of the VQ-VAE model. Outputs a vector of shape (n_components,).
-        for each training instance, corresponding to the soft counts for each cluster.
-        - vade (tf.keras.Model): complete VaDE model
+        encoder (tf.keras.Model): connected encoder of the VQ-VAE model. Outputs a vector of shape (latent_dim,).
+        decoder (tf.keras.Model): connected decoder of the VQ-VAE model.
+        grouper (tf.keras.Model): deep clustering branch of the VQ-VAE model. Outputs a vector of shape (n_components,) for each training instance, corresponding to the soft counts for each cluster.
+        vade (tf.keras.Model): complete VaDE model
+
     """
     if encoder_type == "recurrent":
         encoder = get_recurrent_encoder(
             input_shape=input_shape[1:],
             adjacency_matrix=adjacency_matrix,
             edge_feature_shape=edge_feature_shape[1:],
             latent_dim=latent_dim,
@@ -1423,28 +1423,26 @@
         adjacency_matrix: np.ndarray = None,
         use_gnn: bool = True,
         batch_size: int = 2048,
         bias_initializer: float = 0.0,
         encoder_type: str = "recurrent",
         **kwargs,
     ):
-
-        """Initializes a classifier model.
+        """Initialize a classifier model.
 
         Args:
-            - input_shape (tuple): shape of the input data.
-            - edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
-            - adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-            - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-            as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-            - batch_size (int): batch size for training.
-            - encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
-            - bias_initializer (float): value to initialize the bias of the last layer to (default: 0.0).
-        """
+            input_shape (tuple): shape of the input data.
+            edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
+            adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
+            use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+            batch_size (int): batch size for training.
+            encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
+            bias_initializer (float): value to initialize the bias of the last layer to (default: 0.0).
 
+        """
         super().__init__(**kwargs)
 
         if encoder_type == "recurrent":
             self.encoder = get_recurrent_encoder(
                 input_shape=input_shape[1:],
                 adjacency_matrix=adjacency_matrix,
                 edge_feature_shape=edge_feature_shape[1:],
@@ -1475,22 +1473,21 @@
             1,
             activation="sigmoid",
             name="classifier",
             bias_initializer=self.bias_initializer,
         )
 
     def call(self, inputs, training=None, mask=None):
-        """Forward pass of the classifier.
+        """Apply a forward pass of the classifier.
 
         Args:
             - inputs (tf.Tensor): input data.
             - training (bool): whether the model is in training mode.
             - mask (tf.Tensor): mask for the input data.
         """
-
         x = self.encoder(inputs)
         x = self.dense(x)
         x = self.dropout(x, training=training)
         x = self.clf(x)
 
         return x
 
@@ -1514,35 +1511,34 @@
         kmeans_loss: float = 1.0,
         reg_cat_clusters: float = 1.0,
         reg_cluster_variance: bool = False,
         encoder_type: str = "recurrent",
         interaction_regularization: float = 0.0,
         **kwargs,
     ):
-        """Initalizes a VaDE model.
+        """Init a VaDE model.
 
         Args:
-            - input_shape (tuple): Shape of the input to the full model.
-            - edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
-            - adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-            - batch_size (int): Batch size for training.
-            - latent_dim (int): Dimensionality of the latent space.
-            - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-            as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-            - kl_annealing_mode (str): Annealing mode for KL annealing. Can be one of 'linear' and 'sigmoid'.
-            - kl_warmup_epochs (int): Number of epochs to warmup KL annealing.
-            - montecarlo_kl (int): Number of Monte Carlo samples for KL divergence.
-            - n_components (int): Number of mixture components in the latent space.
-            - kmeans_loss (float): weight of the gram matrix regularization loss.
-            - reg_cat_clusters (bool): whether to use the penalized uneven cluster membership in the latent space, by
-            minimizing the KL divergence between cluster membership and a uniform categorical distribution.
-            - reg_cluster_variance (bool): whether to penalize uneven cluster variances in the latent space.
-            - encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
-            - interaction_regularization (float): Regularization parameter for the interaction features.
-            - **kwargs: Additional keyword arguments.
+            input_shape (tuple): Shape of the input to the full model.
+            edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
+            adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
+            batch_size (int): Batch size for training.
+            latent_dim (int): Dimensionality of the latent space.
+            use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+            kl_annealing_mode (str): Annealing mode for KL annealing. Can be one of 'linear' and 'sigmoid'.
+            kl_warmup_epochs (int): Number of epochs to warmup KL annealing.
+            montecarlo_kl (int): Number of Monte Carlo samples for KL divergence.
+            n_components (int): Number of mixture components in the latent space.
+            kmeans_loss (float): weight of the gram matrix regularization loss.
+            reg_cat_clusters (bool): whether to use the penalized uneven cluster membership in the latent space, by minimizing the KL divergence between cluster membership and a uniform categorical distribution.
+            reg_cluster_variance (bool): whether to penalize uneven cluster variances in the latent space.
+            encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
+            interaction_regularization (float): Regularization parameter for the interaction features.
+            **kwargs: Additional keyword arguments.
+
         """
         super(VaDE, self).__init__(**kwargs)
         self.seq_shape = input_shape
         self.edge_feature_shape = edge_feature_shape
         self.adjacency_matrix = adjacency_matrix
         self.batch_size = batch_size
         self.latent_dim = latent_dim
@@ -1617,41 +1613,41 @@
                 self.val_cat_cluster_loss_tracker,
             ]
 
         return metrics
 
     @property
     def get_gmm_params(self):
-
+        """Return the GMM parameters of the model."""
         # Get GMM parameters
         return {
             "means": self.grouper.get_layer("gaussian_mixture_latent").c_mu,
             "sigmas": tf.math.exp(
                 self.grouper.get_layer("gaussian_mixture_latent").log_c_sigma
             ),
             "weights": tf.math.softmax(
                 self.grouper.get_layer("gaussian_mixture_latent").prior
             ),
         }
 
     def set_pretrain_mode(self, switch):
+        """Set the pretrain mode of the model."""
         self.grouper.get_layer("gaussian_mixture_latent").pretrain.assign(switch)
 
     def pretrain(
         self,
         data,
         embed_x,
         embed_a,
         epochs=10,
         samples=10000,
         gmm_initialize=True,
         **kwargs,
     ):
-        """Runs a GMM directed pretraining of the encoder, to minimize the likelihood of getting stuck in a local minimum."""
-
+        """Run a GMM directed pretraining of the encoder, to minimize the likelihood of getting stuck in a local minimum."""
         # Turn on pretrain mode
         self.set_pretrain_mode(1.0)
 
         # pre-train
         self.fit(
             data,
             epochs=epochs,
@@ -1688,19 +1684,19 @@
                 tf.math.log(
                     tf.math.sqrt(tf.convert_to_tensor(value=sigma2, dtype=tf.float32))
                 )
             )
 
     @tf.function
     def call(self, inputs, **kwargs):
-        """Calls the VaDE model."""
+        """Call the VaDE model."""
         return self.vade(inputs, **kwargs)
 
     def train_step(self, data):  # pragma: no cover
-        """Performs a training step."""
+        """Perform a training step."""
         # Unpack data, repacking labels into a generator
         x, a, y = data
         if not isinstance(y, tuple):
             y = [y]
         y = (labels for labels in y)
 
         with tf.GradientTape() as tape:
@@ -1837,31 +1833,31 @@
         similarity_function: str = "cosine",
         loss_function: str = "nce",
         beta: float = 0.1,
         tau: float = 0.1,
         interaction_regularization: float = 0.0,
         **kwargs,
     ):
-        """Initalizes a self-supervised Contrastive embedding model.
+        """Init a self-supervised Contrastive embedding model.
 
         Args:
-            - input_shape (tuple): Shape of the input to the full model.
-            - edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
-            - adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
-            - encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
-            - latent_dim (int): Dimensionality of the latent space.
-            - use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds
-            as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
-            - temperature (float):
-            - similarity_function (str):
-            - loss_function (str):
-            - beta (float):
-            - tau (float):
-            - interaction_regularization (float): Regularization parameter for the interaction features.
-            - **kwargs: Additional keyword arguments.
+            input_shape (tuple): Shape of the input to the full model.
+            edge_feature_shape (tuple): shape of the edge feature matrix used for graph representations.
+            adjacency_matrix (np.ndarray): adjacency matrix of the connectivity graph to use.
+            encoder_type (str): type of encoder to use. Can be set to "recurrent" (default), "TCN", or "transformer".
+            latent_dim (int): Dimensionality of the latent space.
+            use_gnn (bool): If True, the encoder uses a graph representation of the input, with coordinates and speeds as node attributes, and distances as edge attributes. If False, a regular 3D tensor is used as input.
+            temperature (float):
+            similarity_function (str):
+            loss_function (str):
+            beta (float):
+            tau (float):
+            interaction_regularization (float): Regularization parameter for the interaction features.
+            **kwargs: Additional keyword arguments.
+
         """
         super(Contrastive, self).__init__(**kwargs)
         self.seq_shape = input_shape
         self.edge_feature_shape = edge_feature_shape
         self.adjacency_matrix = adjacency_matrix
         self.latent_dim = latent_dim
         self.use_gnn = use_gnn
@@ -1939,19 +1935,19 @@
             self.val_neg_sim_tracker,
         ]
 
         return metrics
 
     @tf.function
     def call(self, inputs, **kwargs):
-        """Calls the contrastive model."""
+        """Call the contrastive model."""
         return self.encoder(inputs, **kwargs)
 
     def train_step(self, data):  # pragma: no cover
-        """Performs a training step."""
+        """Perform a training step."""
         # Unpack data
         x, a, y = data
         if not isinstance(y, tuple):
             y = [
                 y
             ]  # Labels won't be used for now, but may come handy if exploring regularizers in the future
```

### Comparing `deepof-0.2/deepof/post_hoc.py` & `deepof-0.3/deepof/post_hoc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,239 @@
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-"""
-
-Data structures and functions for analyzing supervised and unsupervised model results.
-
-"""
+"""Data structures and functions for analyzing supervised and unsupervised model results."""
 
 from catboost import CatBoostClassifier
 from collections import Counter, defaultdict
 from imblearn.over_sampling import SMOTE
+from imblearn.pipeline import Pipeline
 from itertools import product
 from joblib import delayed, Parallel
 from multiprocessing import cpu_count
+from pomegranate.distributions import Normal
+from pomegranate.hmm import DenseHMM
 from scipy import stats
 from seglearn import feature_functions
 from seglearn.transform import FeatureRep
 from sklearn.decomposition import PCA
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import roc_auc_score
-from sklearn.model_selection import GroupKFold, cross_validate
+from sklearn.model_selection import GridSearchCV, GroupKFold, cross_validate
 from sklearn.neighbors import KernelDensity
-from imblearn.pipeline import Pipeline
 from sklearn.preprocessing import LabelEncoder, StandardScaler
 from tensorflow_probability import distributions as tfd
 from typing import Any, List, NewType, Union
 import numpy as np
+import os
 import ot
 import pandas as pd
+import pickle
 import scipy
 import shap
+import tqdm
 import umap
 
 import deepof.data
 
 # DEFINE CUSTOM ANNOTATED TYPES #
 project = NewType("deepof_project", Any)
 coordinates = NewType("deepof_coordinates", Any)
 table_dict = NewType("deepof_table_dict", Any)
 
 
+def _fit_hmm_range(concat_embeddings, states, min_states, max_states):
+    """Auxiliary function for fitting a range of HMMs with different number of states.
+
+    Args:
+        concat_embeddings (np.ndarray): Concatenated embeddings across all animal experiments.
+        states (str): Whether to use AIC or BIC to select the number of states.
+        min_states (int): Minimum number of states to use for the HMM.
+        max_states (int): Maximum number of states to use for the HMM.
+
+    """
+    hmm_models = []
+    model_selection = []
+    for i in tqdm.tqdm(range(min_states, max_states + 1)):
+
+        try:
+            model = DenseHMM([Normal() for _ in range(i)])
+            model = model.fit(concat_embeddings)
+            hmm_models.append(model)
+
+            # Compute AIC and BIC
+            n_features = concat_embeddings.shape[2]
+            n_params = i * (n_features + n_features * (n_features + 1) / 2) + i * (
+                i - 1
+            )
+            log_likelihood = float(model.log_probability(concat_embeddings).mean())
+            if states == "aic":
+                model_selection.append(2 * n_params - 2 * log_likelihood)
+            elif states == "bic":
+                model_selection.append(
+                    n_params * np.log(concat_embeddings.shape[0]) - 2 * log_likelihood
+                )
+
+        except np.linalg.LinAlgError:
+            model_selection.append(np.inf)
+
+    if states in ["aic", "bic"]:
+        hmm_model = hmm_models[np.argmin(model_selection)]
+    else:
+        hmm_model = hmm_models[0]
+
+    return hmm_model, model_selection
+
+
+def recluster(
+    coordinates: coordinates,
+    embeddings: table_dict,
+    soft_counts: table_dict = None,
+    min_confidence: float = 0.75,
+    states: Union[str, int] = "aic",
+    pretrained: Union[bool, str] = False,
+    min_states: int = 2,
+    max_states: int = 25,
+    save: bool = True,
+):
+    """Recluster the data using a HMM-based approach. If soft_counts is provided, the model will use the soft cluster assignments as priors for a semi-supervised HMM.
+
+    Args:
+        coordinates: deepOF project where the data is stored.
+        embeddings (table_dict): table dict with neural embeddings per animal experiment across time.
+        soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
+        min_confidence (float): minimum confidence the model should assign to a data point for the model to avoid resorting to a uniform prior around it.
+        states: Number of states to use for the HMM. If "aic" or "bic", the number of states is chosen by minimizing the AIC or BIC criteria (respectively) over a predefined range of states.
+        pretrained: Whether to use a pretrained model or not. If True, DeepOF will search for an existing file with the provided parameters. If a string, DeepOF will search for a file with the provided name.
+        min_states: Minimum number of states to use for the HMM if automatic search is enabled.
+        max_states: Maximum number of states to use for the HMM if automatic search is enabled.
+        save: Whether to save the trained model or not.
+
+    Returns:
+        soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time, using the new HMM-based segmentation on the embedding space.
+
+    """
+
+    # Expand dims of each element in the table dict, pad them all to the same length, and concatenate
+    model_selection = []
+    max_len = max([i.shape[0] for i in embeddings.values()])
+    concat_embeddings = np.concatenate(
+        [
+            np.expand_dims(np.pad(i, ((0, max_len - i.shape[0]), (0, 0))), axis=0)
+            for i in embeddings.values()
+        ]
+    )
+
+    # Load Pretrained model if necessary, or train a new one if not
+    if pretrained:  # pragma: no cover
+        if isinstance(pretrained, str):
+            hmm_model = pickle.load(open(pretrained, "rb"))
+        else:
+            hmm_model = pickle.load(
+                open(
+                    os.path.join(
+                        coordinates._project_path,
+                        coordinates._project_name,
+                        "Trained_models",
+                        +"hmm_trained_{}.pkl".format(states),
+                    ),
+                    "rb",
+                )
+            )
+
+    elif soft_counts is not None:
+        concat_soft_counts = np.concatenate(
+            [
+                np.expand_dims(
+                    np.pad(
+                        i,
+                        ((0, max_len - i.shape[0]), (0, 0)),
+                        constant_values=1 / list(soft_counts.values())[0].shape[1],
+                    ),
+                    axis=0,
+                )
+                for i in soft_counts.values()
+            ]
+        )
+        if min_confidence is not None:
+            for st in concat_soft_counts:
+                st[np.where(np.max(st, axis=1) <= min_confidence)[0]] = (
+                    1 / list(soft_counts.values())[0].shape[1]
+                )
+
+        # Initialize the model
+        hmm_model = DenseHMM([Normal() for _ in range(concat_soft_counts.shape[2])])
+
+        # Fit the model
+        hmm_model = hmm_model.fit(X=concat_embeddings, priors=concat_soft_counts)
+
+    else:
+
+        if isinstance(states, int):
+            min_states = max_states = states
+
+        # Fit a range of HMMs with different number of states
+        hmm_model, model_selection = _fit_hmm_range(
+            concat_embeddings, states, min_states, max_states
+        )
+
+    # Save the best model
+    if save:  # pragma: no cover
+        pickle.dump(
+            hmm_model,
+            open(
+                os.path.join(
+                    coordinates._project_path,
+                    coordinates._project_name,
+                    "Trained_models",
+                    "hmm_trained_{}.pkl".format(states),
+                ),
+                "wb",
+            ),
+        )
+
+    # Predict on each animal experiment
+    soft_counts = hmm_model.predict_proba(concat_embeddings)
+    soft_counts = deepof.data.TableDict(
+        {
+            key: np.array(soft_counts[i][: embeddings[key].shape[0]])
+            for i, key in enumerate(embeddings.keys())
+        },
+        typ="unsupervised_counts",
+        exp_conditions=coordinates.get_exp_conditions,
+    )
+
+    if len(model_selection) > 0:
+        return soft_counts, model_selection
+
+    return soft_counts
+
+
 def get_time_on_cluster(
     soft_counts: table_dict,
     breaks: table_dict,
     normalize: bool = True,
     reduce_dim: bool = False,
 ):
-    """
+    """Compute how much each animal spends on each cluster.
 
-    Given a set of cluster assignments and the corresponding breaks, computes how much each
-    animal spent on each cluster.
+    Requires a set of cluster assignments and their corresponding breaks.
 
     Args:
-        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
-        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
-        conditions, and the values are the breaks for each condition.
-        normalize (bool): Whether to normalize the time by the total number of frames in
-        each condition.
-        reduce_dim (bool): Whether to reduce the dimensionality of the embeddings to 2D. If False,
-        the embeddings are kept in their original dimensionality.
+        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
+        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental conditions, and the values are the breaks for each condition.
+        normalize (bool): Whether to normalize the time by the total number of frames in each condition.
+        reduce_dim (bool): Whether to reduce the dimensionality of the embeddings to 2D. If False, the embeddings are kept in their original dimensionality.
 
     Returns:
         A dataframe with the time spent on each cluster for each experiment.
 
     """
-
     # Reduce soft counts to hard assignments per video
     hard_counts = {key: np.argmax(value, axis=1) for key, value in soft_counts.items()}
 
     # Repeat cluster assignments using the break values
     hard_count_counters = {
         key: Counter(np.repeat(value, breaks[key]))
         for key, value in hard_counts.items()
@@ -98,33 +260,29 @@
             agg_pipeline.fit_transform(counter_df), index=counter_df.index
         )
 
     return counter_df
 
 
 def get_aggregated_embedding(
-    embedding: table_dict, reduce_dim: bool = False, agg: str = "mean"
+    embedding: np.ndarray, reduce_dim: bool = False, agg: str = "mean"
 ):
-    """
+    """Aggregate the embeddings of a set of videos, using the specified aggregation method.
 
-    Aggregates the embeddings of a set of videos, using the specified aggregation method.
     Instead of an embedding per chunk, the function returns an embedding per experiment.
 
     Args:
-        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        reduce_dim (bool): Whether to reduce the dimensionality of the embeddings to 2D. If False,
-        the embeddings are kept in their original dimensionality.
+        embedding (np.ndarray): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        reduce_dim (bool): Whether to reduce the dimensionality of the embeddings to 2D. If False, the embeddings are kept in their original dimensionality.
         agg (str): The aggregation method to use. Can be either "mean" or "median".
 
     Returns:
         A dataframe with the aggregated embeddings for each experiment.
 
     """
-
     # aggregate the provided embeddings and cast to a dataframe
     if agg == "mean":
         embedding = pd.DataFrame(
             {key: np.nanmean(value, axis=0) for key, value in embedding.items()}
         ).T
     elif agg == "median":
         embedding = pd.DataFrame(
@@ -148,35 +306,29 @@
     soft_counts: table_dict = None,
     breaks: table_dict = None,
     supervised_annotations: table_dict = None,
     bin_size: int = 0,
     bin_index: int = 0,
     precomputed: np.ndarray = None,
 ):
-    """
-
-    Selects a time bin and filters all relevant objects (embeddings, soft_counts and breaks).
+    """Select a time bin and filters all relevant objects (embeddings, soft_counts, breaks, and supervised annotations).
 
     Args:
-        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
-        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
-        conditions, and the values are the breaks for each condition.
+        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
+        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental conditions, and the values are the breaks for each condition.
         supervised_annotations (TableDict): table dict with supervised annotations per animal experiment across time.
         bin_size (int): The size of the time bin to select.
         bin_index (int): The index of the time bin to select.
-        precomputed (np.ndarray): Boolean array. If provided, ignores every othe parameter and just indexes each
-        experiment using the provided mask.
+        precomputed (np.ndarray): Boolean array. If provided, ignores every othe parameter and just indexes each experiment using the provided mask.
 
     Returns:
         A tuple of the filtered embeddings, soft counts, and breaks.
-    """
 
+    """
     # If precomputed, filter each experiment using the provided boolean array
     if supervised_annotations is None:
 
         if precomputed is not None:  # pragma: no cover
             breaks_mask_dict = {}
 
             for key in breaks.keys():
@@ -231,49 +383,34 @@
     step_bin: int = None,
     scan_mode: str = "growing_window",
     precomputed_bins: np.ndarray = None,
     agg: str = "mean",
     metric: str = "auc",
     n_jobs: int = cpu_count(),
 ):
-    """
-
-    Computes the distance between the embeddings of two conditions, using the specified
-    aggregation method.
+    """Compute the distance between the embeddings of two conditions, using the specified aggregation method.
 
     Args:
-        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
-        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
-        conditions, and the values are the breaks for each condition.
-        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the
-        names of the experiments, and the values are the names of their corresponding
-        experimental conditions.
+        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
+        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental conditions, and the values are the breaks for each condition.
+        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the names of the experiments, and the values are the names of their corresponding experimental conditions.
         start_bin (int): The index of the first bin to compute the distance for.
         end_bin (int): The index of the last bin to compute the distance for.
         step_bin (int): The step size of the bins to compute the distance for.
-        scan_mode (str): The mode to use for computing the distance. Can be one of "growing-window"
-        (used to select optimal binning), "per-bin" (used to evaluate how discriminability
-        evolves in subsequent bins of a specified size) or "precomputed", which requires a numpy ndarray
-        with bin IDs to be passed to precomputed_bins.
-        precomputed_bins (np.ndarray): numpy array with IDs mapping to different bins, not necessarily having
-        the same size. Difference across conditions for each of these bins will be reported.
+        scan_mode (str): The mode to use for computing the distance. Can be one of "growing-window" (used to select optimal binning), "per-bin" (used to evaluate how discriminability evolves in subsequent bins of a specified size) or "precomputed", which requires a numpy ndarray with bin IDs to be passed to precomputed_bins.
+        precomputed_bins (np.ndarray): numpy array with IDs mapping to different bins, not necessarily having the same size. Difference across conditions for each of these bins will be reported.
         agg (str): The aggregation method to use. Can be either "mean", "median", or "time_on_cluster".
-        metric (str): The distance metric to use. Can be either "auc" (where the reported 'distance'
-        is based on performance of a classifier when separating aggregated embeddings), or
-        "wasserstein" (which computes distances based on optimal transport).
+        metric (str): The distance metric to use. Can be either "auc" (where the reported 'distance' is based on performance of a classifier when separating aggregated embeddings), or "wasserstein" (which computes distances based on optimal transport).
         n_jobs (int): The number of jobs to use for parallel processing.
 
     Returns:
         An array with distances between conditions across the resulting time bins
 
     """
-
     # Divide the embeddings in as many corresponding bins, and compute distances
     def embedding_distance(bin_index):
 
         if scan_mode == "per-bin":
 
             cur_embedding, cur_soft_counts, cur_breaks, _ = select_time_bin(
                 embedding, soft_counts, breaks, bin_size=step_bin, bin_index=bin_index
@@ -324,39 +461,28 @@
     cur_embedding: table_dict,
     cur_soft_counts: table_dict,
     cur_breaks: table_dict,
     exp_conditions: dict,
     agg: str,
     metric: str,
 ):
-    """
-
-    Computes the distance between the embeddings of two conditions, using the specified
-    aggregation method.
+    """Compute the distance between the embeddings of two conditions, using the specified aggregation method.
 
     Args:
-        cur_embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        cur_soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
-        cur_breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
-        conditions, and the values are the breaks for each condition.
-        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the
-        names of the experiments, and the values are the names of their corresponding
-        experimental conditions.
+        cur_embedding (TableDict): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        cur_soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
+        cur_breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental conditions, and the values are the breaks for each condition.
+        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the names of the experiments, and the values are the names of their corresponding experimental conditions.
         agg (str): The aggregation method to use. Can be one of "time on cluster", "mean", or "median".
-        metric (str): The distance metric to use. Can be either "auc" (where the reported 'distance'
-        is based on performance of a classifier when separating aggregated embeddings), or
-        "wasserstein" (which computes distances based on optimal transport).
+        metric (str): The distance metric to use. Can be either "auc" (where the reported 'distance' is based on performance of a classifier when separating aggregated embeddings), or "wasserstein" (which computes distances based on optimal transport).
 
     Returns:
         The distance between the embeddings of the two conditions.
 
     """
-
     # Aggregate embeddings and add experimental conditions
     if agg == "time_on_cluster":
         aggregated_embeddings = get_time_on_cluster(
             cur_soft_counts, cur_breaks, reduce_dim=True
         )
     elif agg in ["mean", "median"]:
         aggregated_embeddings = get_aggregated_embedding(
@@ -401,44 +527,65 @@
             current_distance = ot.sliced_wasserstein_distance(
                 *arrays_to_compare, n_projections=10000
             )
 
     return current_distance
 
 
+def fit_normative_global_model(global_normal_embeddings: pd.DataFrame):
+    """Fit a global model to the normal embeddings.
+
+    Args:
+        global_normal_embeddings (pd.DataFrame): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+
+    Returns:
+        A fitted global model.
+
+    """
+    # Define the range of bandwidth values to search over
+    params = {"bandwidth": np.linspace(0.1, 10, 200)}
+
+    # Create an instance of the KernelDensity estimator
+    kde = KernelDensity(kernel="gaussian")
+
+    # Perform a grid search to find the optimal bandwidth value
+    grid_search = GridSearchCV(
+        kde, params, cv=np.minimum(10, global_normal_embeddings.shape[0])
+    )
+    grid_search.fit(global_normal_embeddings.values)
+
+    kd_estimation = KernelDensity(
+        kernel="gaussian", bandwidth=grid_search.best_params_["bandwidth"]
+    ).fit(global_normal_embeddings.values)
+
+    return kd_estimation
+
+
 def enrichment_across_conditions(
     embedding: table_dict = None,
     soft_counts: table_dict = None,
     breaks: table_dict = None,
     supervised_annotations: table_dict = None,
     exp_conditions: dict = None,
     bin_size: int = None,
     bin_index: int = None,
     precomputed: np.ndarray = None,
     normalize: bool = False,
 ):
-    """
-
-    Computes the population of each cluster across conditions.
+    """Compute the population of each cluster across conditions.
 
     Args:
-        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
+        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
         breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
         supervised_annotations (tableDict): table dict with supervised annotations per animal experiment across time.
-        conditions, and the values are the breaks for each condition.
-        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the
-        names of the experiments, and the values are the names of their corresponding
-        experimental conditions.
+        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the names of the experiments, and the values are the names of their corresponding experimental conditions.
         bin_size (int): The size of the time bins to use. If None, the embeddings are not binned.
         bin_index (int): The index of the bin to use. If None, the embeddings are not binned.
-        precomputed (np.ndarray): Boolean array. If provided, ignores every othe parameter and just indexes each
-        experiment using the provided mask.
+        precomputed (np.ndarray): Boolean array. If provided, ignores every othe parameter and just indexes each experiment using the provided mask.
         normalize (bool): Whether to normalize the population of each cluster across conditions.
 
     Returns:
         A long format dataframe with the population of each cluster across conditions.
 
     """
     # Select time bin and filter all relevant objects
@@ -475,27 +622,24 @@
 
     return counter_df.melt(
         id_vars=["exp condition"], var_name="cluster", value_name="time on cluster"
     )
 
 
 def get_transitions(state_sequence: list, n_states: int):
-    """
-
-    Computes the transitions between states in a state sequence.
+    """Compute the transitions between states in a state sequence.
 
     Args:
         state_sequence (list): A list of states.
         n_states (int): The number of states.
 
     Returns:
         The resulting transition matrix.
 
     """
-
     transition_matrix = np.zeros([n_states, n_states])
     for cur_state, next_state in zip(state_sequence[:-1], state_sequence[1:]):
         transition_matrix[cur_state, next_state] += 1
 
     return transition_matrix
 
 
@@ -506,39 +650,32 @@
     exp_conditions: dict,
     silence_diagonal: bool = False,
     bin_size: int = None,
     bin_index: int = None,
     aggregate: str = True,
     normalize: str = True,
 ):
-    """
-
-    Computes the transition matrices specific to each condition.
+    """Compute the transition matrices specific to each condition.
 
     Args:
-        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the
-        experimental conditions, and the values are the embeddings for each condition.
-        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the
-        experimental conditions, and the values are the soft counts for each condition.
-        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental
-        conditions, and the values are the breaks for each condition.
-        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the
-        names of the experiments, and the values are the names of their corresponding
+        embedding (TableDict): A dictionary of embeddings, where the keys are the names of the experimental conditions, and the values are the embeddings for each condition.
+        soft_counts (TableDict): A dictionary of soft counts, where the keys are the names of the experimental conditions, and the values are the soft counts for each condition.
+        breaks (TableDict): A dictionary of breaks, where the keys are the names of the experimental conditions, and the values are the breaks for each condition.
+        exp_conditions (dict): A dictionary of experimental conditions, where the keys are the names of the experiments, and the values are the names of their corresponding
         silence_diagonal (bool): If True, diagonal elements on the transition matrix are set to zero.
         bin_size (int): The size of the time bins to use. If None, the embeddings are not binned.
         bin_index (int): The index of the bin to use. If None, the embeddings are not binned.
         aggregate (str): Whether to aggregate the embeddings across time.
         normalize (str): Whether to normalize the population of each cluster across conditions.
 
     Returns:
         A dictionary of transition matrices, where the keys are the names of the experimental
         conditions, and the values are the transition matrices for each condition.
 
     """
-
     # Filter data to get desired subset
     if bin_size is not None and bin_index is not None:
         embedding, soft_counts, breaks, _ = select_time_bin(
             embedding,
             soft_counts,
             breaks,
             bin_size=bin_size,
@@ -578,32 +715,25 @@
 
     return transitions
 
 
 def compute_steady_state(
     transition_matrices: dict, return_entropy: bool = False, n_iters: int = 100000
 ):
-    """
-
-    Computes the steady state of each transition matrix provided in a dictionary.
+    """Compute the steady state of each transition matrix provided in a dictionary.
 
     Args:
-        transition_matrices (dict): A dictionary of transition matrices, where the keys are
-        the names of the experimental conditions, and the values are the transition matrices for each condition.
-        return_entropy (bool): Whether to return the entropy of the steady state. If False, the steady states themselves are
-        returned.
+        transition_matrices (dict): A dictionary of transition matrices, where the keys are the names of the experimental conditions, and the values are the transition matrices for each condition.
+        return_entropy (bool): Whether to return the entropy of the steady state. If False, the steady states themselves are returned.
         n_iters (int): The number of iterations to use for the Markov chain.
 
     Returns:
-        A dictionary of steady states, where the keys are the names of the experimental conditions, and the values are
-        the steady states for each condition. If return_entropy is True, values correspond to the entropy of each
-        steady state.
+        A dictionary of steady states, where the keys are the names of the experimental conditions, and the values are the steady states for each condition. If return_entropy is True, values correspond to the entropy of each steady state.
 
     """
-
     # Compute steady states by multiplying matrices by themselves n_iters times
     steady_states = {
         key: np.linalg.matrix_power(value, n_iters)
         for key, value in transition_matrices.items()
     }
 
     # Compute steady state probabilities per state
@@ -618,58 +748,57 @@
             key: stats.entropy(value) for key, value in steady_states.items()
         }
 
     return steady_states
 
 
 def compute_UMAP(embeddings, cluster_assignments):  # pragma: no cover
-
+    """Compute UMAP embeddings for visualization purposes."""
     lda = LinearDiscriminantAnalysis(
         n_components=np.min([embeddings.shape[1], len(set(cluster_assignments)) - 1]),
     )
     concat_embeddings = lda.fit_transform(embeddings, cluster_assignments)
 
     red = umap.UMAP(
         min_dist=0.99,
         n_components=2,
     ).fit(concat_embeddings)
 
     return lda, red
 
 
 def align_deepof_kinematics_with_unsupervised_labels(
-    deepof_project: project,
+    deepof_project: coordinates,
     kin_derivative: int = 1,
     include_feature_derivatives: bool = False,
     include_distances: bool = True,
     include_angles: bool = True,
     include_areas: bool = True,
     animal_id: str = None,
 ):
-    """
+    """Align kinematics with unsupervised labels.
 
     In order to annotate time chunks with as many relevant features as possible, this function aligns the kinematics
     of a deepof project (speed and acceleration of body parts, distances, and angles) with the hard cluster assignments
     obtained from the unsupervised pipeline.
 
     Args:
-        deepof_project (Project): A deepof.Project object.
+        deepof_project (coordinates): A deepof.Project object.
         kin_derivative (int): The order of the derivative to use for the kinematics. 1 = speed, 2 = acceleration, etc.
         include_feature_derivatives (bool): Whether to compute speed on distances, angles, and areas, if they are included.
         include_distances (bool): Whether to include distances in the alignment.
         include_angles (bool): Whether to include angles in the alignment.
         include_areas (bool): Whether to include areas in the alignment.
         animal_id (str): The animal ID to use, in case of multi-animal projects.
 
     Returns:
         A dictionary of aligned kinematics, where the keys are the names of the experimental conditions, and the
         values are the aligned kinematics for each condition.
 
     """
-
     # Compute speeds and accelerations per bodypart
     kinematic_features = defaultdict(pd.DataFrame)
 
     for der in range(kin_derivative + 1):
 
         cur_kinematics = deepof_project.get_coords(
             center="Center", align="Spine_1", speed=der
@@ -739,29 +868,24 @@
             )
 
     # Return aligned kinematics
     return deepof.data.TableDict(kinematic_features, typ="annotations")
 
 
 def chunk_summary_statistics(chunked_dataset: np.ndarray, body_part_names: list):
-    """
-
-    Extracts summary statistics from a chunked dataset using seglearn.
+    """Extract summary statistics from a chunked dataset using seglearn.
 
     Args:
-        chunked_dataset (np.ndarray): Preprocessed training set (of shape chunks x time x features),
-        where each entry corresponds to a time chunk of data.
+        chunked_dataset (np.ndarray): Preprocessed training set (of shape chunks x time x features), where each entry corresponds to a time chunk of data.
         body_part_names (list): A list of the names of the body parts.
 
     Returns:
         A dataframe of kinematic features, of shape chunks by features.
 
-
     """
-
     # Extract time series features with ts-learn and seglearn
     extracted_features = FeatureRep(feature_functions.base_features()).fit_transform(
         chunked_dataset
     )
 
     # Convert to data frame and add feature names
     extracted_features = pd.DataFrame(extracted_features)
@@ -770,61 +894,53 @@
     )
     extracted_features.columns = ["_".join(idx) for idx in columns]
 
     return extracted_features
 
 
 def annotate_time_chunks(
-    deepof_project: project,
+    deepof_project: coordinates,
     soft_counts: table_dict,
     breaks: table_dict,
     supervised_annotations: table_dict = None,
     window_size: int = None,
     window_step: int = 1,
     animal_id: str = None,
     samples: int = 10000,
     min_confidence: float = 0.0,
     kin_derivative: int = 1,
     include_distances: bool = True,
     include_angles: bool = True,
     include_areas: bool = True,
     aggregate: str = "mean",
 ):
-    """
+    """Annotate time chunks produced after change-point detection using the unsupervised pipeline.
 
-    Annotate time chunks produced after change-point detection using the unsupervised pipeline, using a set
-    of summary statistics coming from kinematics, distances, angles, and supervised labels when provided.
+    Uses a set of summary statistics coming from kinematics, distances, angles, and supervised labels when provided.
 
     Args:
-        deepof_project: Project object.
-        soft_counts: matrix with soft cluster assignments produced by the unsupervised pipeline.
-        breaks: the breaks for each condition.
-        supervised_annotations: set of supervised annotations produced by the supervised pipeline withing deepof.
-        window_size (int): Minimum size of the applied ruptures. If automatic_changepoints is False,
-        specifies the size of the sliding window to pass through the data to generate training instances. None defaults
-        to video frame-rate.
-        window_step (int): Specifies the minimum jump for the rupture algorithms. If automatic_changepoints is False,
-        specifies the step to take when sliding the aforementioned window. In this case, a value of 1 indicates
-        a true sliding window, and a value equal to window_size splits the data into non-overlapping chunks.
+        deepof_project (coordinates): Project object.
+        soft_counts (table_dict): matrix with soft cluster assignments produced by the unsupervised pipeline.
+        breaks (table_dict): the breaks for each condition.
+        supervised_annotations (table_dict): set of supervised annotations produced by the supervised pipeline withing deepof.
+        window_size (int): Minimum size of the applied ruptures. If automatic_changepoints is False, specifies the size of the sliding window to pass through the data to generate training instances. None defaults to video frame-rate.
+        window_step (int): Specifies the minimum jump for the rupture algorithms. If automatic_changepoints is False, specifies the step to take when sliding the aforementioned window. In this case, a value of 1 indicates a true sliding window, and a value equal to window_size splits the data into non-overlapping chunks.
         animal_id (str): The animal ID to use, in case of multi-animal projects.
-        samples (int): Time chunks samples to take to reduce computational time. Defaults to the minimum between
-        10000 and the number of available chunks.
+        samples (int): Time chunks samples to take to reduce computational time. Defaults to the minimum between 10000 and the number of available chunks.
         min_confidence (float): minimum confidence in cluster assignments used for quality control filtering.
-        kin_derivative: The order of the derivative to use for the kinematics. 1 = speed, 2 = acceleration, etc.
-        include_distances: Whether to include distances in the alignment. kin_derivative is taken into account.
-        include_angles: Whether to include angles in the alignment. kin_derivative is taken into account.
-        include_areas: Whether to include areas in the alignment. kin_derivative is taken into account.
-        aggregate: aggregation mode. Can be either "mean" (computationally cheapest), just use the average per feature,
-        or "seglearn" which runs a thorough feature extraction and selection pipeline on each time series.
+        kin_derivative (int): The order of the derivative to use for the kinematics. 1 = speed, 2 = acceleration, etc.
+        include_distances (bool): Whether to include distances in the alignment. kin_derivative is taken into account.
+        include_angles (bool): Whether to include angles in the alignment. kin_derivative is taken into account.
+        include_areas (bool): Whether to include areas in the alignment. kin_derivative is taken into account.
+        aggregate (str): aggregation mode. Can be either "mean" (computationally cheapest), just use the average per feature, or "seglearn" which runs a thorough feature extraction and selection pipeline on each time series.
 
     Returns:
         A dataframe of kinematic features, of shape chunks by features.
 
     """
-
     # Convert soft_counts to hard labels
     hard_counts = {key: np.argmax(value, axis=1) for key, value in soft_counts.items()}
     hard_counts = pd.Series(
         np.concatenate([value for value in hard_counts.values()], axis=0)
     )
 
     # Extract (annotated) kinematic features
@@ -854,14 +970,18 @@
         window_step=window_step,
         filter_low_variance=False,
         interpolate_normalized=False,
         automatic_changepoints=False,
         precomputed_breaks=breaks,
     )[0][0]
 
+    # Remove chunks with missing values
+    possible_idcs = ~np.isnan(comprehensive_features).any(axis=-1).any(axis=-1)
+    comprehensive_features = comprehensive_features[possible_idcs]
+
     def sample_from_breaks(breaks, idcs):
 
         # Sample from breaks, keeping each animal's identity
         cumulative_breaks = 0
         subset_breaks = {}
         for key in breaks.keys():
             subset_breaks[key] = breaks[key][
@@ -875,17 +995,17 @@
 
         return subset_breaks
 
     # Filter instances with less confidence that specified
     qual_filter = (
         np.concatenate([soft for soft in soft_counts.values()]).max(axis=1)
         > min_confidence
-    )
+    )[possible_idcs]
     comprehensive_features = comprehensive_features[qual_filter]
-    hard_counts = hard_counts[qual_filter].reset_index(drop=True)
+    hard_counts = hard_counts[possible_idcs][qual_filter].reset_index(drop=True)
     breaks = sample_from_breaks(breaks, np.where(qual_filter)[0])
 
     # Sample X and y matrices to increase computational efficiency
     if samples is not None:
         samples = np.minimum(samples, comprehensive_features.shape[0])
 
         random_idcs = np.random.choice(
@@ -915,15 +1035,15 @@
 
 
 def chunk_cv_splitter(
     chunk_stats: pd.DataFrame,
     breaks: dict,
     n_folds: int = None,
 ):
-    """
+    """Split a dataset into training and testing sets, grouped by video.
 
     Given a matrix with extracted features per chunk, returns a list containing
     a set of cross-validation folds, grouped by experimental video. This makes
     sure that chunks coming from the same experiment will never be leaked between
     training and testing sets.
 
     Args:
@@ -931,15 +1051,14 @@
         breaks (dict): dictionary containing ruprures per video.
         n_folds (int): number of cross-validation folds to compute.
 
     Returns:
         list containing a training and testing set per CV fold.
 
     """
-
     # Extract number of experiments/folds
     n_experiments = len(breaks)
 
     # Create a cross-validation loop, with one fold per video
     fold_lengths = np.array([len(value) for value in breaks.values()])
 
     # Repeat experiment indices across chunks, to generate a valid splitter
@@ -954,31 +1073,29 @@
 def train_supervised_cluster_detectors(
     chunk_stats: pd.DataFrame,
     hard_counts: np.ndarray,
     sampled_breaks: dict,
     n_folds: int = None,
     verbose: int = 1,
 ):  # pragma: no cover
-    """
+    """Train supervised models to detect clusters from kinematic features.
 
     Args:
         chunk_stats (pd.DataFrame): table with descriptive statistics for a series of sequences ('chunks').
         hard_counts (np.ndarray): cluster assignments for the corresponding 'chunk_stats' table.
         sampled_breaks (dict): sequence length of each chunk per experiment.
         n_folds (int): number of folds for cross validation. If None (default) leave-one-experiment-out CV is used.
         verbose (int): verbosity level. Must be an integer between 0 (nothing printed) and 3 (all is printed).
 
     Returns:
-        full_cluster_clf (imblearn.pipeline.Pipeline): trained supervised model on the full dataset, mapping chunk stats
-        to cluster assignments. Useful to run the SHAP explainability pipeline.
+        full_cluster_clf (imblearn.pipeline.Pipeline): trained supervised model on the full dataset, mapping chunk stats to cluster assignments. Useful to run the SHAP explainability pipeline.
         cluster_gbm_performance (dict): cross-validated dictionary containing trained estimators and performance metrics.
         groups (list): cross-validation indices. Data from the same animal are never shared between train and test sets.
 
     """
-
     groups = chunk_cv_splitter(chunk_stats, sampled_breaks, n_folds=n_folds)
 
     # Cross-validate GBM training across videos
     cluster_clf = Pipeline(
         [
             ("normalization", StandardScaler()),
             ("oversampling", SMOTE()),
@@ -1024,31 +1141,30 @@
 
 
 def explain_clusters(
     chunk_stats: pd.DataFrame,
     hard_counts: np.ndarray,
     full_cluster_clf: Pipeline,
     samples: int = 10000,
+    n_jobs: int = -1,
 ):  # pragma: no cover
-    """Computes SHAP feature importance for models mapping chunk_stats to cluster assignments.
+    """Compute SHAP feature importance for models mapping chunk_stats to cluster assignments.
 
     Args:
         chunk_stats (pd.DataFrame): matrix with statistics per chunk, sorted by experiment.
-        np.ndarray): cluster assignments for the corresponding 'chunk_stats' table.
         hard_counts (np.ndarray): cluster assignments for the corresponding 'chunk_stats' table.
-        full_cluster_clf (imblearn.pipeline.Pipeline): trained supervised model on the full dataset, mapping chunk stats
-        to cluster assignments.
+        full_cluster_clf (imblearn.pipeline.Pipeline): trained supervised model on the full dataset, mapping chunk stats to cluster assignments.
         samples (int): number of samples to draw from the original chunk_stats dataset.
+        n_jobs (int): number of parallel jobs to run. If -1 (default), all CPUs are used.
 
     Returns:
         shap_values (list): shap_values per cluster.
         explainer (shap.explainers._kernel.Kernel): trained SHAP KernelExplainer.
 
     """
-
     # Pass the data through the scaler and oversampler before computing SHAP values
     processed_stats = full_cluster_clf.named_steps["normalization"].transform(
         chunk_stats
     )
     processed_stats = full_cluster_clf.named_steps["oversampling"].fit_resample(
         processed_stats, hard_counts
     )[0]
@@ -1059,10 +1175,12 @@
     explainer = shap.KernelExplainer(
         full_cluster_clf.named_steps["classifier"].predict_proba,
         data=shap.kmeans(processed_stats, n_clusters),
         normalize=False,
     )
     if samples is not None and samples < chunk_stats.shape[0]:
         processed_stats = processed_stats.sample(samples)
-    shap_values = explainer.shap_values(processed_stats, nsamples=samples, n_jobs=-1)
+    shap_values = explainer.shap_values(
+        processed_stats, nsamples=samples, n_jobs=n_jobs
+    )
 
     return shap_values, explainer, processed_stats
```

### Comparing `deepof-0.2/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl` & `deepof-0.3/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl`

 * *Files identical despite different names*

### Comparing `deepof-0.2/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl` & `deepof-0.3/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl`

 * *Files identical despite different names*

### Comparing `deepof-0.2/deepof/utils.py` & `deepof-0.3/deepof/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-"""
-
-Functions and general utilities for the deepof package.
-
-"""
-
+"""Functions and general utilities for the deepof package."""
+import copy
 from copy import deepcopy
 from dask_image.imread import imread
 from itertools import combinations, product
 from joblib import Parallel, delayed
 from scipy.signal import savgol_filter
 from shapely.geometry import Polygon
 from sklearn import mixture
 from sklearn.feature_selection import VarianceThreshold
+from sklearn.experimental import enable_iterative_imputer  # noqa
+from sklearn.impute import IterativeImputer
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 from tqdm import tqdm
 from typing import Tuple, Any, List, Union, NewType
 import argparse
 import cv2
 import math
 import multiprocessing
 import networkx as nx
 import numpy as np
 import os
 import pandas as pd
 import regex as re
 import ruptures as rpt
 import tensorflow as tf
+import warnings
+
+import deepof.data
 
 # DEFINE CUSTOM ANNOTATED TYPES #
 project = NewType("deepof_project", Any)
 coordinates = NewType("deepof_coordinates", Any)
 table_dict = NewType("deepof_table_dict", Any)
 
 
 # CONNECTIVITY AND GRAPH REPRESENTATIONS
 
 
-def connect_mouse_topview(animal_ids=None, exclude_bodyparts: list = None) -> nx.Graph:
-    """
+def connect_mouse(
+    animal_ids=None, exclude_bodyparts: list = None, graph_preset: str = "deepof_14"
+) -> nx.Graph:
+    """Create a nx.Graph object with the connectivity of the bodyparts in the DLC topview model for a single mouse.
 
-    Creates a nx.Graph object with the connectivity of the bodyparts in the
-    DLC topview model for a single mouse. Used later for angle computing, among others.
+    Used later for angle computing, among others.
 
     Args:
         animal_ids (str): if more than one animal is tagged, specify the animal identyfier as a string.
         exclude_bodyparts (list): Remove the specified nodes from the graph.
+        graph_preset (str): Connectivity preset to use. Currently supported: "deepof_14" and "deepof_8".
 
     Returns:
         connectivity (nx.Graph)
 
     """
-
     if animal_ids is None:
         animal_ids = [""]
     if not isinstance(animal_ids, list):
         animal_ids = [animal_ids]
 
     connectivities = []
 
     for animal_id in animal_ids:
-        connectivity = {
-            "Nose": ["Left_ear", "Right_ear"],
-            "Spine_1": ["Center", "Left_ear", "Right_ear"],
-            "Center": ["Left_fhip", "Right_fhip", "Spine_2"],
-            "Spine_2": ["Left_bhip", "Right_bhip", "Tail_base"],
-            "Tail_base": ["Tail_1"],
-            "Tail_1": ["Tail_2"],
-            "Tail_2": ["Tail_tip"],
+        connectivity_dict = {
+            "deepof_14": {
+                "Nose": ["Left_ear", "Right_ear"],
+                "Spine_1": ["Center", "Left_ear", "Right_ear"],
+                "Center": ["Left_fhip", "Right_fhip", "Spine_2"],
+                "Spine_2": ["Left_bhip", "Right_bhip", "Tail_base"],
+                "Tail_base": ["Tail_1"],
+                "Tail_1": ["Tail_2"],
+                "Tail_2": ["Tail_tip"],
+            },
+            "deepof_8": {
+                "Nose": ["Left_ear", "Right_ear"],
+                "Center": [
+                    "Left_fhip",
+                    "Right_fhip",
+                    "Tail_base",
+                    "Left_ear",
+                    "Right_ear",
+                ],
+                "Tail_base": ["Tail_tip"],
+            },
         }
-        connectivity = nx.Graph(connectivity)
+        connectivity = nx.Graph(connectivity_dict[graph_preset])
 
         if animal_id:
             mapping = {
                 node: "{}_{}".format(animal_id, node) for node in connectivity.nodes()
             }
             if exclude_bodyparts is not None:
                 exclude = ["{}_{}".format(animal_id, exc) for exc in exclude_bodyparts]
@@ -109,15 +124,15 @@
             "{}_Nose".format(animal_ids[g - 1]), "{}_Tail_base".format(animal_ids[g])
         )
 
     return final_graph
 
 
 def edges_to_weithed_adj(adj: np.ndarray, edges: np.ndarray):
-    """Converts an edge feature matrix to a weighted adjacency matrix.
+    """Convert an edge feature matrix to a weighted adjacency matrix.
 
     Args:
         - adj (np.ndarray): binary adjacency matrix of the current graph.
         - edges (np.ndarray): edge feature matrix. Last two axes should be of shape nodes x features.
 
     """
     adj = np.repeat(np.expand_dims(adj.astype(float), axis=0), edges.shape[0], axis=0)
@@ -126,15 +141,15 @@
 
     adj[np.where(adj)] = np.concatenate([edges, edges[:, ::-1]], axis=-2).flatten()
 
     return adj
 
 
 def enumerate_all_bridges(G: nx.graph) -> list:
-    """Enumerates all 3-node connected sequences in the given graph.
+    """Enumerate all 3-node connected sequences in the given graph.
 
     Args:
         - G (nx.graph): Animal connectivity graph.
 
     Returns:
         bridges (list): List with all 3-node connected sequences in the provided graph.
 
@@ -152,87 +167,178 @@
 
 # QUALITY CONTROL AND PREPROCESSING #
 
 
 def str2bool(v: str) -> bool:
     """
 
-    Returns the passed string as a boolean.
+    Return the passed string as a boolean.
 
     Args:
         v (str): String to transform to boolean value.
 
     Returns:
         bool. If conversion is not possible, it raises an error
 
     """
-
     if isinstance(v, bool):
         return v  # pragma: no cover
     elif v.lower() in ("yes", "true", "t", "y", "1"):
         return True
     elif v.lower() in ("no", "false", "f", "n", "0"):
         return False
     raise argparse.ArgumentTypeError("Boolean compatible value expected.")
 
 
-def likelihood_qc(dframe: pd.DataFrame, threshold: float = 0.9) -> np.array:
+def compute_animal_presence_mask(
+    quality: table_dict, threshold: float = 0.5
+) -> table_dict:
+    """Compute a mask of the animal presence in the video.
+
+    Args:
+        quality (table_dict): Dictionary with the quality of the tracking for each body part and animal.
+        threshold (float): Threshold for the quality of the tracking. If the quality is below this threshold, the animal is considered to be absent.
+
+    Returns:
+        animal_presence_mask (table_dict): Dictionary with the animal presence mask for each bodypart and animal.
+
     """
+    animal_presence_mask = {}
 
-    Returns a DataFrame filtered dataframe, keeping only the rows entirely above the threshold.
+    for exp in quality.keys():
+        animal_presence_mask[exp] = {}
+        for animal_id in quality._animal_ids:
+            animal_presence_mask[exp][animal_id] = (
+                quality.filter_id(animal_id)[exp].median(axis=1) > threshold
+            ).astype(int)
+
+        animal_presence_mask[exp] = pd.DataFrame(animal_presence_mask[exp])
+
+    return deepof.data.TableDict(
+        animal_presence_mask, typ="animal_presence_mask", animal_ids=quality._animal_ids
+    )
+
+
+def iterative_imputation(project: project, tab_dict: dict, lik_dict: dict):
+    """Perform iterative imputation on occluded body parts. Run per animal and experiment.
 
     Args:
-        dframe (pandas.DataFrame): DeepLabCut output, with positions over time and associated likelihood.
-        threshold (float): Minimum acceptable confidence.
+        project (project): Project object.
+        tab_dict (dict): Dictionary with the coordinates of the body parts.
+        lik_dict (dict): Dictionary with the likelihood of the tracking for each body part and animal.
 
     Returns:
-        filt_mask (np.array): mask on the rows of dframe
+        tab_dict (dict): Dictionary with the coordinates of the body parts after imputation.
 
     """
+    presence_masks = compute_animal_presence_mask(lik_dict)
+    tab_dict = deepof.data.TableDict(
+        tab_dict, typ="coords", animal_ids=project.animal_ids
+    )
+    imputed_tabs = copy.deepcopy(tab_dict)
 
-    Likes = np.array([dframe[i]["likelihood"] for i in list(dframe.columns.levels[0])])
-    Likes = np.nan_to_num(Likes, nan=1.0)
-    filt_mask = np.all(Likes > threshold, axis=0)
+    for animal_id in project.animal_ids:
 
-    return filt_mask
+        for k, tab in tab_dict.filter_id(animal_id).items():
 
+            scaler = StandardScaler()
+            imputed = IterativeImputer(
+                skip_complete=True,
+                max_iter=project.enable_iterative_imputation,
+                n_nearest_features=tab.shape[1],
+                tol=1e-1,
+            ).fit_transform(
+                scaler.fit_transform(
+                    tab.iloc[np.where(presence_masks[k][animal_id].values)[0]]
+                )
+            )
+
+            imputed = pd.DataFrame(
+                scaler.inverse_transform(imputed),
+                index=tab.index[np.where(presence_masks[k][animal_id].values)[0]],
+                columns=tab.loc[:, tab.isnull().mean(axis=0) != 1.0].columns,
+            )
+
+            imputed_tabs[k].update(imputed)
+
+            if tab.shape[1] != imputed.shape[1]:
+                warnings.warn(
+                    "Some of the body parts have zero measurements. Iterative imputation skips these,"
+                    " which could bring problems downstream. A possible solution could be to refine "
+                    "DLC tracklets."
+                )
+
+    return imputed_tabs
+
+
+def set_missing_animals(
+    coordinates: project, tab_dict: dict, lik_dict: dict, animal_ids: list = None
+):
+    """Set the coordinates of the missing animals to NaN.
+
+    Args:
+        coordinates (project): Project object.
+        tab_dict (dict): Dictionary with the coordinates of the body parts.
+        lik_dict (dict): Dictionary with the likelihood of the tracking for each body part and animal.
+        animal_ids (list): List with the animal ids to remove. If None, all the animals with missing data are processed.
+
+    Returns:
+        tab_dict (dict): Dictionary with the coordinates of the body parts after removing missing animals.
 
-def bp2polar(tab: pd.DataFrame) -> pd.DataFrame:
     """
+    if animal_ids is None:
+        try:
+            animal_ids = coordinates.animal_ids
+        except AttributeError:
+            animal_ids = coordinates._animal_ids
+
+    presence_masks = compute_animal_presence_mask(lik_dict)
+    tab_dict = deepof.data.TableDict(tab_dict, typ="qc", animal_ids=animal_ids)
 
-    Returns the DataFrame in polar coordinates.
+    for animal_id in animal_ids:
+        for k, tab in tab_dict.filter_id(animal_id).items():
+            try:
+                missing_times = tab[presence_masks[k][animal_id] == 0]
+            except KeyError:
+                missing_times = tab[
+                    presence_masks[k].sum(axis=1) < (len(animal_ids) - 1)
+                ]
+
+            tab_dict[k].loc[missing_times.index, missing_times.columns] = np.nan
+
+    return tab_dict
+
+
+def bp2polar(tab: pd.DataFrame) -> pd.DataFrame:
+    """Return the DataFrame in polar coordinates.
 
     Args:
         tab (pandas.DataFrame): Table with cartesian coordinates.
 
     Returns:
         polar (pandas.DataFrame): Equivalent to input, but with values in polar coordinates.
 
     """
-
     tab_ = np.array(tab)
     complex_ = tab_[:, 0] + 1j * tab_[:, 1]
     polar = pd.DataFrame(np.array([abs(complex_), np.angle(complex_)]).T)
     polar.rename(columns={0: "rho", 1: "phi"}, inplace=True)
     return polar
 
 
 def tab2polar(cartesian_df: pd.DataFrame) -> pd.DataFrame:
-    """
-
-    Returns a pandas.DataFrame in which all the coordinates are polar.
+    """Return a pandas.DataFrame in which all the coordinates are polar.
 
     Args:
         cartesian_df (pandas.DataFrame): DataFrame containing tables with cartesian coordinates.
 
     Returns:
         result (pandas.DataFrame): Equivalent to input, but with values in polar coordinates.
 
     """
-
     result = []
     for df in list(cartesian_df.columns.levels[0]):
         result.append(bp2polar(cartesian_df[df]))
     result = pd.concat(result, axis=1)
     idx = pd.MultiIndex.from_product(
         [list(cartesian_df.columns.levels[0]), ["rho", "phi"]]
     )
@@ -240,69 +346,59 @@
     result.index = cartesian_df.index
     return result
 
 
 def compute_dist(
     pair_array: np.array, arena_abs: int = 1, arena_rel: int = 1
 ) -> pd.DataFrame:
-    """
-
-    Returns a pandas.DataFrame with the scaled distances between a pair of body parts.
+    """Return a pandas.DataFrame with the scaled distances between a pair of body parts.
 
     Args:
-        pair_array (numpy.array): np.array of shape N * 4 containing X, y positions.
-        over time for a given pair of body parts.
+        pair_array (numpy.array): np.array of shape N * 4 containing X, y positions over time for a given pair of body parts.
         arena_abs (int): Diameter of the real arena in cm.
         arena_rel (int): Diameter of the captured arena in pixels.
 
     Returns:
         result (pd.DataFrame): pandas.DataFrame with the absolute distances between a pair of body parts.
 
     """
-
     lim = 2 if pair_array.shape[1] == 4 else 1
     a, b = pair_array[:, :lim], pair_array[:, lim:]
     ab = a - b
 
     dist = np.sqrt(np.einsum("...i,...i", ab, ab))
     return pd.DataFrame(dist * arena_abs / arena_rel)
 
 
 def bpart_distance(
     dataframe: pd.DataFrame, arena_abs: int = 1, arena_rel: int = 1
 ) -> pd.DataFrame:
-    """
-
-    Returns a pandas.DataFrame with the scaled distances between all pairs of body parts.
+    """Return a pandas.DataFrame with the scaled distances between all pairs of body parts.
 
     Args:
-        dataframe (pandas.DataFrame): pd.DataFrame of shape N*(2*bp) containing X,y positions
-        over time for a given set of bp body parts.
+        dataframe (pandas.DataFrame): pd.DataFrame of shape N*(2*bp) containing X,y positions over time for a given set of bp body parts.
         arena_abs (int): Diameter of the real arena in cm.
         arena_rel (int): Diameter of the captured arena in pixels.
 
     Returns:
         result (pd.DataFrame): pandas.DataFrame with the absolute distances between all pairs of body parts.
 
     """
-
     indexes = combinations(dataframe.columns.levels[0], 2)
     dists = []
     for idx in indexes:
         dist = compute_dist(np.array(dataframe.loc[:, list(idx)]), arena_abs, arena_rel)
         dist.columns = [idx]
         dists.append(dist)
 
     return pd.concat(dists, axis=1)
 
 
 def angle(bpart_array: np.array) -> np.array:
-    """
-
-    Returns a numpy.ndarray with the angles between the provided instances.
+    """Return a numpy.ndarray with the angles between the provided instances.
 
     Args:
         bpart_array (numpy.array): 2D positions over time for a bodypart.
 
     Returns:
         ang (np.array): 1D angles between the three-point-instances.
 
@@ -317,25 +413,24 @@
     )
     ang = np.arccos(cosine_angle)
 
     return ang
 
 
 def compute_areas(coords, animal_id=None):
-    """
-    Computes relevant areas (head, torso, back, full) for the provided coordinates.
+    """Compute relevant areas (head, torso, back, full) for the provided coordinates.
+
     Args:
         coords: coordinates of the body parts for a single time point.
         animal_id: animal id for the provided coordinates, if any.
 
     Returns:
         areas: list including head, torso, back, and full areas for the provided coordinates.
 
     """
-
     head = ["Nose", "Left_ear", "Left_fhip", "Spine_1"]
 
     torso = ["Spine_1", "Right_fhip", "Spine_2", "Left_fhip"]
 
     back = ["Spine_1", "Right_bhip", "Spine_2", "Left_bhip"]
 
     full = [
@@ -366,56 +461,51 @@
 
     return areas
 
 
 def rotate(
     p: np.array, angles: np.array, origin: np.array = np.array([0, 0])
 ) -> np.array:
-    """
-
-    Returns a 2D numpy.ndarray with the initial values rotated by angles radians.
+    """Return a 2D numpy.ndarray with the initial values rotated by angles radians.
 
     Args:
         p (numpy.ndarray): 2D Array containing positions of bodyparts over time.
         angles (numpy.ndarray): Set of angles (in radians) to rotate p with.
         origin (numpy.ndarray): Rotation axis (zero vector by default).
 
     Returns:
         - rotated (numpy.ndarray): rotated positions over time
 
     """
-
     R = np.array([[np.cos(angles), -np.sin(angles)], [np.sin(angles), np.cos(angles)]])
 
     o = np.atleast_2d(origin)
     p = np.atleast_2d(p)
 
     rotated = np.squeeze((R @ (p.T - o.T) + o.T).T)
 
     return rotated
 
 
 # noinspection PyArgumentList
 def align_trajectories(data: np.array, mode: str = "all") -> np.array:
-    """
+    """Remove rotational variance on the trajectories.
 
-    Returns a numpy.array with the positions rotated in a way that the center (0 vector)
-    and the body part in the first column of data are aligned with the y axis.
+    Returns a numpy.array with the positions rotated in a way that the center (0 vector), and body part in the first
+    column of data are aligned with the y-axis.
 
     Args:
         data (numpy.ndarray): 3D array containing positions of body parts over time, where
         shape is N (sliding window instances) * m (sliding window size) * l (features)
-        mode (string): Specifies if *all* instances of each sliding window get
-        aligned, or only the *center*
+        mode (string): Specifies if *all* instances of each sliding window get aligned, or only the *center*
 
     Returns:
         aligned_trajs (np.ndarray): 2D aligned positions over time.
 
     """
-
     angles = np.zeros(data.shape[0])
     data = deepcopy(data)
     dshape = data.shape
 
     if mode == "center":
         center_time = (data.shape[1] - 1) // 2
         angles = np.arctan2(data[:, center_time, 0], data[:, center_time, 1])
@@ -510,31 +600,33 @@
 
     normalized_array = cur_scaler.fit_transform(feature_array)
     scalers.append(cur_scaler)
 
     return normalized_array
 
 
-def kleinberg(offsets, s=np.e, gamma=1.0, n=None, T=None, k=None):
-    """Kleinberg's algorithm (described in 'Bursty and Hierarchical Structure
-    in Streams'). The algorithm models activity bursts in a time series as an
+def kleinberg(
+    offsets: list, s: float = np.e, gamma: float = 1.0, n=None, T=None, k=None
+):
+    """Apply Kleinberg's algorithm (described in 'Bursty and Hierarchical Structure in Streams').
+
+    The algorithm models activity bursts in a time series as an
     infinite hidden Markov model.
 
     Taken from pybursts (https://github.com/romain-fontugne/pybursts/blob/master/pybursts/pybursts.py)
     and adapted for dependency compatibility reasons.
 
-    Input:
-        offsets: a list of time offsets (numeric)
-        s: the base of the exponential distribution that is used for modeling
-        the event frequencies
-        gamma: coefficient for the transition costs between states
-        n, T: to have a fixed cost function (not dependent of the given offsets).
-        Which is needed if you want to compare bursts for different inputs.
-        k: maximum burst level"""
+    Args:
+        offsets (list): a list of time offsets (numeric)
+        s (float): the base of the exponential distribution that is used for modeling the event frequencies
+        gamma (float): coefficient for the transition costs between states
+        n, T: to have a fixed cost function (not dependent of the given offsets). Which is needed if you want to compare bursts for different inputs.
+        k: maximum burst level
 
+    """
     if s <= 1:
         raise ValueError("s must be greater than 1!")
     if gamma <= 0:
         raise ValueError("gamma must be positive!")
     if not n is None and n <= 0:
         raise ValueError("n must be positive!")
     if not T is None and T <= 0:
@@ -645,27 +737,24 @@
         bursts[stack[stack_counter], 2] = offsets[np.size(gaps)]
         stack_counter -= 1
 
     return bursts
 
 
 def smooth_boolean_array(a: np.array, scale: int = 1) -> np.array:
-    """
-
-    Returns a boolean array in which isolated appearances of a feature are smoothed.
+    """Return a boolean array in which isolated appearances of a feature are smoothed.
 
     Args:
         a (numpy.ndarray): Boolean instances.
         scale (int): Kleinberg scale parameter. Higher values result in stricter smoothing.
 
     Returns:
         a (numpy.ndarray): Smoothened boolean instances.
 
     """
-
     offsets = np.where(a)[0]
     if len(offsets) == 0:
         return a  # no detected activity
 
     bursts = kleinberg(offsets, gamma=0.01)
     a = np.zeros(np.size(a), dtype=bool)
     for i in bursts:
@@ -706,38 +795,33 @@
     ]
     split_a = np.concatenate(split_a, axis=0)
 
     return split_a
 
 
 def rolling_window(
-    a: np.array,
+    a: np.ndarray,
     window_size: int,
     window_step: int,
     automatic_changepoints: str = False,
     precomputed_breaks: np.ndarray = None,
 ) -> np.ndarray:
-    """
-
-    Returns a 3D numpy.array with a sliding-window extra dimension.
+    """Return a 3D numpy.array with a sliding-window extra dimension.
 
     Args:
         a (np.ndarray): N (instances) * m (features) shape
         window_size (int): Size of the window to apply
         window_step (int): Step of the window to apply
-        automatic_changepoints (str): Changepoint detection algorithm to apply.
-        If False, applies a fixed sliding window.
-        precomputed_breaks (np.ndarray): Precomputed breaks to use, bypassing the changepoint detection algorithm.
-        None by default (break points are computed).
+        automatic_changepoints (str): Changepoint detection algorithm to apply. If False, applies a fixed sliding window.
+        precomputed_breaks (np.ndarray): Precomputed breaks to use, bypassing the changepoint detection algorithm. None by default (break points are computed).
 
     Returns:
         rolled_a (np.ndarray): N (sliding window instances) * l (sliding window size) * m (features)
 
     """
-
     breakpoints = None
 
     if automatic_changepoints:
         # Define change point detection model using ruptures
         # Remove dimensions with low variance (occurring when aligning the animals with the y axis)
         if precomputed_breaks is None:
             rpt_model = rpt.KernelCPD(
@@ -767,40 +851,33 @@
     to_rupture: np.ndarray,
     rupture_indices: list,
     automatic_changepoints: str,
     window_size: int,
     window_step: int,
     precomputed_breaks: dict = None,
 ) -> np.ndarray:
-    """
+    """Apply the rupture method independently to each experiment, and concatenate into a single dataset at the end.
 
-    Apply the rupture method independently to each experiment, and concatenate into a single dataset
-    at the end. Returns a dataset and the rupture indices, adapted to be used in a concatenated version
+    Returns a dataset and the rupture indices, adapted to be used in a concatenated version
     of the labels.
 
     Args:
         table_dict (deepof.data.table_dict): table_dict with all experiments.
         to_rupture (np.ndarray): Array with dataset to rupture.
         rupture_indices (list): Indices of tables to rupture. Useful to select training and test sets.
-        automatic_changepoints (str): Rupture method to apply.
-        If false, a sliding window of window_length * window_size is obtained.
-        If one of "l1", "l2" or "rbf", different automatic change point detection algorithms are applied
-        on each independent experiment.
-        window_size (int): If automatic_changepoints is False, specifies the length of the sliding window.
-        If not, it determines the minimum size of the obtained time series breaks.
-        window_step (int): If automatic_changepoints is False, specifies the stride of the sliding window.
-        If not, it determines the minimum step size of the obtained time series breaks.
+        automatic_changepoints (str): Rupture method to apply. If false, a sliding window of window_length * window_size is obtained. If one of "l1", "l2" or "rbf", different automatic change point detection algorithms are applied on each independent experiment.
+        window_size (int): If automatic_changepoints is False, specifies the length of the sliding window. If not, it determines the minimum size of the obtained time series breaks.
+        window_step (int): If automatic_changepoints is False, specifies the stride of the sliding window. If not, it determines the minimum step size of the obtained time series breaks.
         precomputed_breaks (dict): If provided, changepoint detection is prevented, and provided breaks are used instead.
 
     Returns:
         ruptured_dataset (np.ndarray): Dataset with all ruptures concatenated across the first axis.
         rupture_indices (list): Indices of ruptures.
 
     """
-
     # Generate a base ruptured training set and a set of breaks
     ruptured_dataset, break_indices = None, None
     cumulative_shape = 0
     # Iterate over all experiments and populate them
     for i, (key, tab) in enumerate(table_dict.items()):
         if i in rupture_indices:
             current_size = tab.shape[0]
@@ -852,72 +929,63 @@
 
     return ruptured_dataset, break_indices
 
 
 def smooth_mult_trajectory(
     series: np.array, alpha: int = 0, w_length: int = 11
 ) -> np.ndarray:
-    """
-
-    Returns a smoothed a trajectory using a Savitzky-Golay 1D filter.
+    """Return a smoothed a trajectory using a Savitzky-Golay 1D filter.
 
     Args:
         series (numpy.ndarray): 1D trajectory array with N (instances)
-        alpha (int): 0 <= alpha < w_length; indicates the difference between the degree of the polynomial and the window
-        length for the Savitzky-Golay filter used for smoothing. Higher values produce a worse fit, hence more smoothing.
-        w_length (int): Length of the sliding window to which the filter fit. Higher values yield a coarser fit,
-        hence more smoothing.
+        alpha (int): 0 <= alpha < w_length; indicates the difference between the degree of the polynomial and the window length for the Savitzky-Golay filter used for smoothing. Higher values produce a worse fit, hence more smoothing.
+        w_length (int): Length of the sliding window to which the filter fit. Higher values yield a coarser fit, hence more smoothing.
 
     Returns:
         smoothed_series (np.ndarray): smoothed version of the input, with equal shape
 
     """
-
     if alpha is None:
         return series
 
     smoothed_series = savgol_filter(
         series, polyorder=(w_length - alpha), window_length=w_length, axis=0
     )
 
     assert smoothed_series.shape == series.shape
 
     return smoothed_series
 
 
 def moving_average(time_series: pd.Series, lag: int = 5) -> pd.Series:
-    """
-
-    Fast implementation of a moving average function.
+    """Fast implementation of a moving average function.
 
     Args:
         time_series (pd.Series): Uni-variate time series to take the moving average of.
         lag (int): size of the convolution window used to compute the moving average.
 
     Returns:
         moving_avg (pd.Series): Uni-variate moving average over time_series.
 
     """
-
     moving_avg = np.convolve(time_series, np.ones(lag) / lag, mode="same")
 
     return moving_avg
 
 
 def mask_outliers(
     time_series: pd.DataFrame,
     likelihood: pd.DataFrame,
     likelihood_tolerance: float,
     lag: int,
     n_std: int,
     mode: str,
 ) -> pd.DataFrame:
-    """
+    """Return a mask over the bivariate trajectory of a body part, identifying as True all detected outliers.
 
-    Returns a mask over the bivariate trajectory of a body part, identifying as True all detected outliers.
     An outlier can be marked with one of two criteria: 1) the likelihood reported by DLC is below likelihood_tolerance,
     and/or 2) the deviation from a moving average model is greater than n_std.
 
     Args:
         time_series (pd.DataFrame): Bi-variate time series representing the x, y positions of a single body part
         likelihood (pd.DataFrame): Data frame with likelihood data per body part as extracted from deeplabcut
         likelihood_tolerance (float): Minimum tolerated likelihood, below which an outlier is called
@@ -925,15 +993,14 @@
         n_std (int): Number of standard deviations over the moving average to be considered an outlier
         mode (str): If "and" (default) both x and y have to be marked in order to call an outlier. If "or", one is enough.
 
     Returns
         mask (pd.DataFrame): Bi-variate mask over time_series. True indicates an outlier.
 
     """
-
     moving_avg_x = moving_average(time_series["x"], lag)
     moving_avg_y = moving_average(time_series["y"], lag)
 
     residuals_x = time_series["x"] - moving_avg_x
     residuals_y = time_series["y"] - moving_avg_y
 
     outlier_mask_x = np.abs(residuals_x) > np.mean(
@@ -958,33 +1025,29 @@
     likelihood: pd.DataFrame,
     likelihood_tolerance: float,
     exclude: str,
     lag: int,
     n_std: int,
     mode: str,
 ) -> pd.DataFrame:
-    """
-
-    Iterates over all body parts of experiment, and outputs a dataframe where all x, y positions are
-    replaced by a boolean mask, where True indicates an outlier.
+    """Iterate over all body parts of experiment, and outputs a dataframe where all x, y positions are replaced by a boolean mask, where True indicates an outlier.
 
     Args:
         experiment (pd.DataFrame): Data frame with time series representing the x, y positions of every body part
         likelihood (pd.DataFrame): Data frame with likelihood data per body part as extracted from deeplabcut
         likelihood_tolerance (float): Minimum tolerated likelihood, below which an outlier is called
         exclude (str): Body part to exclude from the analysis (to concatenate with bpart alignment)
         lag (int): Size of the convolution window used to compute the moving average
         n_std (int): Number of standard deviations over the moving average to be considered an outlier
         mode (str): If "and" (default) both x and y have to be marked in order to call an outlier. If "or", one is enough.
 
     Returns:
         full_mask (pd.DataFrame): Mask over all body parts in experiment. True indicates an outlier
 
     """
-
     body_parts = experiment.columns.levels[0]
     full_mask = experiment.copy()
 
     if exclude:
         full_mask.drop(exclude, axis=1, inplace=True)
 
     for bpart in body_parts:
@@ -1011,17 +1074,16 @@
     likelihood_tolerance: float,
     exclude: str = "",
     lag: int = 5,
     n_std: int = 3,
     mode: str = "or",
     limit: int = 10,
 ) -> pd.DataFrame:
-    """
+    """Mark all outliers in experiment and replaces them using a uni-variate linear interpolation approach.
 
-    Marks all outliers in experiment and replaces them using a uni-variate linear interpolation approach.
     Note that this approach only works for equally spaced data (constant camera acquisition rates).
 
     Args:
         experiment (pd.DataFrame): Data frame with time series representing the x, y positions of every body part.
         likelihood (pd.DataFrame): Data frame with likelihood data per body part as extracted from deeplabcut.
         likelihood_tolerance (float): Minimum tolerated likelihood, below which an outlier is called.
         exclude (str): Body part to exclude from the analysis (to concatenate with bpart alignment).
@@ -1030,15 +1092,14 @@
         mode (str): If "and" both x and y have to be marked in order to call an outlier. If "or" (default), one is enough.
         limit (int): Maximum of consecutive outliers to interpolate. Defaults to 10.
 
     Returns:
         interpolated_exp (pd.DataFrame): Interpolated version of experiment.
 
     """
-
     interpolated_exp = experiment.copy()
 
     # Creates a mask marking all outliers
     mask = full_outlier_mask(
         experiment, likelihood, likelihood_tolerance, exclude, lag, n_std, mode
     )
 
@@ -1051,80 +1112,192 @@
         [experiment.iloc[:lag, :], interpolated_exp.iloc[lag:, :]]
     )
 
     return interpolated_exp
 
 
 def filter_columns(columns: list, selected_id: str) -> list:
-    """
-
-    Given a set of TableDict columns, returns those that correspond to a given animal, specified in selected_id.
+    """Given a set of TableDict columns, returns those that correspond to a given animal, specified in selected_id.
 
     Args:
         columns (list): List of columns to filter.
         selected_id (str): Animal ID to filter for.
 
     Returns:
         filtered_columns (list): List of filtered columns.
 
     """
-
     if selected_id is None:
         return columns
 
     columns_to_keep = []
     for column in columns:
         # Speed transformed columns
+        if selected_id == "supervised" and column in [
+            "nose2nose",
+            "sidebyside",
+            "sidereside",
+        ]:
+            columns_to_keep.append(column)
         if type(column) == str and column.startswith(selected_id):
             columns_to_keep.append(column)
         # Raw coordinate columns
         if column[0].startswith(selected_id) and column[1] in ["x", "y", "rho", "phi"]:
             columns_to_keep.append(column)
         # Raw distance and angle columns
         elif len(column) in [2, 3] and all([i.startswith(selected_id) for i in column]):
             columns_to_keep.append(column)
         elif column[0].lower().startswith("pheno"):
             columns_to_keep.append(column)
 
     return columns_to_keep
 
 
+def get_arenas(
+    arena: str,
+    arena_dims: int,
+    project_path: str,
+    project_name: str,
+    tables: dict,
+    videos: list = None,
+):
+    """Extract arena parameters from a project or coordinates object.
+
+    Args:
+        arena (str): Arena type (must be either "polygonal-manual", "circular-manual", or "circular-autodetect").
+        arena_dims (int): Arena dimensions.
+        project_path (str): Path to project.
+        project_name (str): Name of project.
+        tables (dict): List of tables to extract arena parameters from.
+        videos (list): List of videos to extract arena parameters from. Defaults to None (all videos are used).
+
+    Returns:
+        arena_params (list): List of arena parameters.
+
+    """
+    scales = []
+    arena_params = []
+    video_resolution = []
+
+    def get_first_length(arena_corners):
+        return math.dist(arena_corners[0], arena_corners[1])
+
+    if arena in ["polygonal-manual", "circular-manual"]:  # pragma: no cover
+
+        for i, video_path in enumerate(videos):
+            arena_corners, h, w = extract_polygonal_arena_coordinates(
+                os.path.join(project_path, project_name, "Videos", video_path),
+                arena,
+                i,
+                videos,
+            )
+
+            cur_scales = [
+                *np.mean(arena_corners, axis=0).astype(int),
+                get_first_length(arena_corners),
+                arena_dims,
+            ]
+
+            cur_arena_params = arena_corners
+
+            if arena == "circular-manual":
+                cur_arena_params = fit_ellipse_to_polygon(cur_arena_params)
+
+                scales.append(
+                    list(
+                        np.array(
+                            [
+                                cur_arena_params[0][0],
+                                cur_arena_params[0][1],
+                                np.mean(
+                                    [cur_arena_params[1][0], cur_arena_params[1][1]]
+                                )
+                                * 2,
+                            ]
+                        )
+                    )
+                    + [arena_dims]
+                )
+            else:
+                scales.append(cur_scales)
+
+            arena_params.append(cur_arena_params)
+            video_resolution.append((h, w))
+
+    elif arena in ["circular-autodetect"]:
+
+        for vid_index, _ in enumerate(videos):
+            ellipse, h, w = automatically_recognize_arena(
+                videos=videos,
+                tables=tables,
+                vid_index=vid_index,
+                path=os.path.join(project_path, project_name, "Videos"),
+                arena_type=arena,
+            )
+
+            # scales contains the coordinates of the center of the arena,
+            # the absolute diameter measured from the video in pixels, and
+            # the provided diameter in mm (1 -default- equals not provided)
+            scales.append(
+                list(
+                    np.array(
+                        [
+                            ellipse[0][0],
+                            ellipse[0][1],
+                            np.mean([ellipse[1][0], ellipse[1][1]]) * 2,
+                        ]
+                    )
+                )
+                + [arena_dims]
+            )
+            arena_params.append(ellipse)
+            video_resolution.append((h, w))
+
+    elif not arena:
+        return None, None, None
+
+    else:  # pragma: no cover
+        raise NotImplementedError(
+            "arenas must be set to one of: 'polygonal-manual', 'circular-autodetect'"
+        )
+
+    return np.array(scales), arena_params, video_resolution
+
+
 # noinspection PyUnboundLocalVariable
 def automatically_recognize_arena(
     videos: list,
     vid_index: int,
     path: str = ".",
     tables: dict = None,
     recoglimit: int = 500,
     arena_type: str = "circular-autodetect",
 ) -> Tuple[np.array, int, int]:
-    """
+    """Return numpy.ndarray with information about the arena recognised from the first frames of the video.
 
-    Returns numpy.ndarray with information about the arena recognised from the first frames
-    of the video. WARNING: estimates won't be reliable if the camera moves along the video.
+    WARNING: estimates won't be reliable if the camera moves along the video.
 
     Args:
         videos (list): Relative paths of the videos to analise.
         vid_index (int): Element of videos list to use.
         path (str): Full path of the directory where the videos are.
         tables (dict): Dictionary with DLC time series in DataFrames as values.
         recoglimit (int): Number of frames to use for position estimates.
         potentially more accurate in poor lighting conditions.
         arena_type (string): Arena type; must be one of ['circular-autodetect', 'circular-manual', 'polygon-manual'].
 
     Returns:
         arena (np.ndarray): 1D-array containing information about the arena.
-        "circular-autodetect" (3-element-array) -> x-y position of the center and the radius.
-        "circular-manual" (3-element-array) -> x-y position of the center and the radius.
-        "polygon-manual" (2n-element-array) -> x-y position of each of the n the vertices of the polygon.
         h (int): Height of the video in pixels.
         w (int): Width of the video in pixels.
 
     """
-
+    # "circular-autodetect" (3-element-array) -> x-y position of the center and the radius.
+    # "circular-manual" (3-element-array) -> x-y position of the center and the radius.
+    # "polygonal-manual" (2n-element-array) -> x-y position of each of the n the vertices of the polygon.
     cap = cv2.VideoCapture(os.path.join(path, videos[vid_index]))
 
     if tables is not None:
         # Select relevant table to check animal positions; if animals are close to the arena, do not take those frames
         # into account
         centers = tables[list(tables.keys())[vid_index]].iloc[:recoglimit, :]
 
@@ -1175,44 +1348,40 @@
                 centers.to_numpy().reshape(-1, 2) - (w / 2, h / 2), axis=1
             ).reshape(-1, centers_shape[1] // 2),
             axis=1,
         )
         # Within the frame recognition limit, only the 1% less obstructed will contribute to the arena
         # fitting
         center_quantile = np.quantile(center_distances, 0.05)
-        arena = arena[center_distances < center_quantile]
-        weights = 1 / center_distances[center_distances < center_quantile]
+        arena = arena[center_distances <= center_quantile]
 
     # Compute the median across frames and return to tuple format for downstream compatibility
     arena = np.average(arena[~np.any(np.isnan(arena), axis=1)], axis=0)
     arena = (tuple(arena[:2].astype(int)), tuple(arena[2:4].astype(int)), arena[4])
 
     return arena, h, w
 
 
 def retrieve_corners_from_image(
     frame: np.ndarray, arena_type: str, cur_vid: int, videos: list
 ):  # pragma: no cover
-    """
+    """Open a window and waits for the user to click on all corners of the polygonal arena.
 
-    Opens a window and waits for the user to click on all corners of the polygonal arena.
     The user should click on the corners in sequential order.
 
     Args:
         frame (np.ndarray): Frame to display.
         arena_type (str): Type of arena to be used. Must be one of the following: "circular-manual", "polygon-manual".
         cur_vid (int): Index of the current video in the list of videos.
         videos (list): List of videos to be processed.
 
     Returns:
-
         corners (np.ndarray): nx2 array containing the x-y coordinates of all n corners.
 
     """
-
     corners = []
 
     def click_on_corners(event, x, y, flags, param):
         # Callback function to store the coordinates of the clicked points
         nonlocal corners, frame
 
         if event == cv2.EVENT_LBUTTONDOWN:
@@ -1296,88 +1465,77 @@
     # Return the corners
     return corners
 
 
 def extract_polygonal_arena_coordinates(
     video_path: str, arena_type: str, video_index: int, videos: list
 ):  # pragma: no cover
-    """
-
-    Reads a random frame from the selected video, and opens an interactive GUI to let the user delineate
-    the arena manually.
+    """Read a random frame from the selected video, and opens an interactive GUI to let the user delineate the arena manually.
 
     Args:
-        video_path: Path to the video file.
-        arena_type: Type of arena to be used. Must be one of the following: "circular-manual", "polygon-manual".
-        video_index: Index of the current video in the list of videos.
-        videos: List of videos to be processed.
+        video_path (str): Path to the video file.
+        arena_type (str): Type of arena to be used. Must be one of the following: "circular-manual", "polygon-manual".
+        video_index (int): Index of the current video in the list of videos.
+        videos (list): List of videos to be processed.
 
     Returns:
         np.ndarray: nx2 array containing the x-y coordinates of all n corners of the polygonal arena.
         int: Height of the video.
         int: Width of the video.
 
     """
-
     current_video = imread(video_path)
     current_frame = np.random.choice(current_video.shape[0])
 
     # Get and return the corners of the arena
     arena_corners = retrieve_corners_from_image(
         current_video[current_frame].compute(),
         arena_type,
         video_index,
         videos,
     )
     return arena_corners, current_video.shape[2], current_video.shape[1]
 
 
 def fit_ellipse_to_polygon(polygon: list):  # pragma: no cover
-    """
-
-    Fits an ellipse to the provided polygon.
+    """Fit an ellipse to the provided polygon.
 
     Args:
-        polygon: List of (x,y) coordinates of the corners of the polygon.
+        polygon (list): List of (x,y) coordinates of the corners of the polygon.
 
     Returns:
         tuple: (x,y) coordinates of the center of the ellipse.
         tuple: (a,b) semi-major and semi-minor axes of the ellipse.
         float: Angle of the ellipse.
 
     """
-
     # Detect the main ellipse containing the arena
     ellipse_params = cv2.fitEllipse(np.array(polygon))
 
     # Parameters to return
     center_coordinates = tuple([int(i) for i in ellipse_params[0]])
     axes_length = tuple([int(i) // 2 for i in ellipse_params[1]])
     ellipse_angle = ellipse_params[2]
 
     return center_coordinates, axes_length, ellipse_angle
 
 
 def circular_arena_recognition(
     frame: np.ndarray,
 ) -> np.array:
-    """
-
-    Returns x,y position of the center, the lengths of the major and minor axes,
-    and the angle of the recognised arena.
+    """Return x,y position of the center, the lengths of the major and minor axes, and the angle of the recognised arena.
 
     Args:
         frame (np.ndarray): numpy.ndarray representing an individual frame of a video
 
     Returns:
         circles (np.ndarray): 3-element-array containing x,y positions of the center
         of the arena, and a third value indicating the radius.
 
     """
-
     # Convert image to grayscale, threshold it and close it with a 5x5 kernel
     kernel = np.ones((5, 5))
     gray_image = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
     ret, thresh = cv2.threshold(gray_image, 255 // 4, 255, 0)
     for _ in range(5):
         thresh = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel)
 
@@ -1400,34 +1558,30 @@
     window: int = 3,
     rounds: int = 3,
     deriv: int = 1,
     center: str = None,
     shift: int = 2,
     typ: str = "coords",
 ) -> pd.DataFrame:
-    """
-
-    Returns the average speed over n frames in pixels per frame.
+    """Return the average speed over n frames in pixels per frame.
 
     Args:
         dframe (pandas.DataFrame): Position over time dataframe.
         window (int): Number of frames to average over.
         rounds (int): Float rounding decimals.
         deriv (int): Position derivative order; 1 for speed, 2 for acceleration, 3 for jerk, etc.
-        center (str): For internal usage only; solves an issue with pandas.MultiIndex that arises when centering frames
-        to a specific body part.
+        center (str): For internal usage only; solves an issue with pandas.MultiIndex that arises when centering frames to a specific body part.
         shift (int): Window shift for rolling speed calculation.
         typ (str): Type of dataset. Intended for internal usage only.
 
     Returns:
         speeds (pd.DataFrame): Data frame containing 2D speeds for each body part in the original data or their
         consequent derivatives.
 
     """
-
     original_shape = dframe.shape
     try:
         body_parts = dframe.columns.levels[0]
     except AttributeError:
         body_parts = dframe.columns
 
     speeds = pd.DataFrame
@@ -1466,15 +1620,15 @@
 def filter_short_bouts(
     cluster_assignments: np.ndarray,
     cluster_confidence: np.ndarray,
     confidence_indices: np.ndarray,
     min_confidence: float = 0.0,
     min_bout_duration: int = None,
 ):  # pragma: no cover
-    """Filters out cluster assignment bouts shorter than min_bout_duration.
+    """Filter out cluster assignment bouts shorter than min_bout_duration.
 
     Args:
         cluster_assignments (np.ndarray): Array of cluster assignments.
         cluster_confidence (np.ndarray): Array of cluster confidence values.
         confidence_indices (np.ndarray): Array of confidence indices.
         min_confidence (float): Minimum confidence value.
         min_bout_duration (int): Minimum bout duration in frames.
@@ -1513,29 +1667,25 @@
     )
 
 
 # MACHINE LEARNING FUNCTIONS #
 
 
 def gmm_compute(x: np.array, n_components: int, cv_type: str) -> list:
-    """
-
-    Fits a Gaussian Mixture Model to the provided data and returns evaluation metrics.
+    """Fit a Gaussian Mixture Model to the provided data and returns evaluation metrics.
 
     Args:
         x (numpy.ndarray): Data matrix to train the model
         n_components (int): Number of Gaussian components to use
-        cv_type (str): Covariance matrix type to use.
-        Must be one of "spherical", "tied", "diag", "full".
+        cv_type (str): Covariance matrix type to use. Must be one of "spherical", "tied", "diag", "full".
 
     Returns:
         - gmm_eval (list): model and associated BIC for downstream selection.
 
     """
-
     gmm = mixture.GaussianMixture(
         n_components=n_components,
         covariance_type=cv_type,
         max_iter=100000,
         init_params="kmeans",
     )
     gmm.fit(x)
@@ -1548,36 +1698,32 @@
     x: pd.DataFrame,
     n_components_range: range,
     part_size: int,
     n_runs: int = 100,
     n_cores: int = False,
     cv_types: Tuple = ("spherical", "tied", "diag", "full"),
 ) -> Tuple[List[list], List[np.ndarray], Union[int, Any]]:
-    """
+    """Run GMM clustering model selection on the specified X dataframe.
 
-    Runs GMM clustering model selection on the specified X dataframe, outputs the bic distribution per model,
-    a vector with the median BICs and an object with the overall best model.
+    Outputs the bic distribution per model, a vector with the median BICs and an object with the overall best model.
 
     Args:
         x (pandas.DataFrame): Data matrix to train the models
         n_components_range (range): Generator with numbers of components to evaluate
         n_runs (int): Number of bootstraps for each model
         part_size (int): Size of bootstrap samples for each model
         n_cores (int): Number of cores to use for computation
         cv_types (tuple): Covariance Matrices to try. All four available by default
 
     Returns:
-        - bic (list): All recorded BIC values for all attempted parameter combinations
-        (useful for plotting)
-        - m_bic(list): All minimum BIC values recorded throughout the process
-        (useful for plottinh)
-        - best_bic_gmm (sklearn.GMM): Unfitted version of the best found model
+        - bic (list): All recorded BIC values for all attempted parameter combinations (useful for plotting).
+        - m_bic(list): All minimum BIC values recorded throughout the process (useful for plottinh).
+        - best_bic_gmm (sklearn.GMM): Unfitted version of the best found model.
 
     """
-
     # Set the default of n_cores to the most efficient value
     if not n_cores:
         n_cores = min(multiprocessing.cpu_count(), n_runs)
 
     bic = []
     m_bic = []
     lowest_bic = np.inf
@@ -1611,28 +1757,26 @@
 
 def cluster_transition_matrix(
     cluster_sequence: np.array,
     nclusts: int,
     autocorrelation: bool = True,
     return_graph: bool = False,
 ) -> Tuple[Union[nx.Graph, Any], np.ndarray]:
-    """Computes the transition matrix between clusters and the autocorrelation in the sequence.
+    """Compute the transition matrix between clusters and the autocorrelation in the sequence.
 
     Args:
         cluster_sequence (numpy.array): Sequence of cluster assignments.
         nclusts (int): Number of clusters in the sequence.
         autocorrelation (bool): Whether to compute the autocorrelation of the sequence.
         return_graph (bool): Whether to return the transition matrix as an networkx.DiGraph object.
 
     Returns:
         trans_normed (numpy.ndarray / networkx.Graph): Transition matrix as numpy.ndarray or networkx.DiGraph.
-        autocorr (numpy.array): If autocorrelation is True, returns a numpy.ndarray with all autocorrelation
-        values on cluster assignment.
+        autocorr (numpy.array): If autocorrelation is True, returns a numpy.ndarray with all autocorrelation values on cluster assignment.
     """
-
     # Stores all possible transitions between clusters
     clusters = [str(i) for i in range(nclusts)]
     cluster_sequence = cluster_sequence.astype(str)
 
     trans = {t: 0 for t in product(clusters, clusters)}
     k = len(clusters)
```

### Comparing `deepof-0.2/deepof/visuals.py` & `deepof-0.3/deepof/visuals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """General plotting functions for the deepof package."""
 import collections
 
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
-from collections import defaultdict, Sequence
+from collections import defaultdict
+from collections.abc import Sequence
 from itertools import cycle, product, combinations
 from matplotlib.animation import FuncAnimation, FFMpegWriter
 from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 from matplotlib.patches import Ellipse
 from scipy.cluster.hierarchy import linkage, dendrogram
 from scipy.signal import savgol_filter
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
@@ -43,20 +44,19 @@
 
 # PLOTTING FUNCTIONS #
 
 
 def plot_arena(
     coordinates: coordinates, center: str, color: str, ax: Any, i: Union[int, str]
 ):
-    """Plots the arena in the given canvas.
+    """Plot the arena in the given canvas.
 
     Args:
         coordinates (coordinates): deepof Coordinates object.
-        center (str): Name of the body part to which the positions will be centered. If false,
-        the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
+        center (str): Name of the body part to which the positions will be centered. If false, the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
         color (str): color of the displayed arena.
         ax (Any): axes where to plot the arena.
         i (Union[int, str]): index of the animal to plot.
     """
     if isinstance(i, np.int64):
         arena = coordinates._arena_params[i]
 
@@ -115,29 +115,27 @@
     title: str = None,
     mask: np.ndarray = None,
     save: str = False,
     dpi: int = 200,
     ax: Any = None,
     **kwargs,
 ) -> plt.figure:
-    """Returns a heatmap of the movement of a specific bodypart in the arena.
+    """Return a heatmap of the movement of a specific bodypart in the arena.
 
     If more than one bodypart is passed, it returns one subplot for each.
 
     Args:
-        dframe (pandas.DataFrame): table_dict value with info to plot
-        bodyparts (List): bodyparts to represent (at least 1)
+        dframe (pandas.DataFrame): table_dict value with info to plot bodyparts (List): bodyparts to represent (at least 1)
         xlim (float): limits of the x-axis
         ylim (float): limits of the y-axis
         title (str): title of the figure
         mask (np.ndarray): mask to apply to the heatmap across time
         save (str): if provided, saves the figure to the specified file.
         dpi (int): dots per inch of the figure to create.
-        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided,
-        new figure will be created.
+        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, new figure will be created.
 
     Returns:
         heatmaps (plt.figure): figure with the specified characteristics
     """
     # noinspection PyTypeChecker
     if ax is None:
         heatmaps, ax = plt.subplots(
@@ -235,39 +233,39 @@
     exp_condition: str = None,
     condition_value: str = None,
     display_arena: bool = True,
     xlim: float = None,
     ylim: float = None,
     save: bool = False,
     experiment_id: int = "average",
+    bin_size: int = None,
+    bin_index: int = None,
     dpi: int = 100,
     ax: Any = None,
     show: bool = True,
     **kwargs,
 ) -> plt.figure:  # pragma: no cover
-    """Plots heatmaps of the specified body parts (bodyparts) of the specified animal (i).
+    """Plot heatmaps of the specified body parts (bodyparts) of the specified animal (i).
 
     Args:
         coordinates (coordinates): deepof Coordinates object.
         bodyparts (list): list of body parts to plot.
-        center (str): Name of the body part to which the positions will be centered. If false,
-        the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
-        align (str): Selects the body part to which later processes will align the frames with
-        (see preprocess in table_dict documentation).
+        center (str): Name of the body part to which the positions will be centered. If false, the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
+        align (str): Selects the body part to which later processes will align the frames with (see preprocess in table_dict documentation).
         exp_condition (str): Experimental condition to plot base filters on.
-        condition_value (str): Experimental condition value to plot. If available, it filters the
-        experiments to keep only those whose condition value matches the given string in the provided exp_condition.
+        condition_value (str): Experimental condition value to plot. If available, it filters the experiments to keep only those whose condition value matches the given string in the provided exp_condition.
         display_arena (bool): whether to plot a dashed line with an overlying arena perimeter. Defaults to True.
         xlim (float): x-axis limits.
         ylim (float): y-axis limits.
         save (str):  if provided, the figure is saved to the specified path.
         experiment_id (str): index of the animal to plot.
+        bin_size (int): bin size for time filtering.
+        bin_index (int): index of the bin of size bin_size to select along the time dimension.
         dpi (int): resolution of the figure.
-        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided,
-        a new figure will be created.
+        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, a new figure will be created.
         show (bool): whether to show the created figure. If False, returns al axes.
 
     Returns:
         heatmaps (plt.figure): figure with the specified characteristics
     """
     coords = coordinates.get_coords(center=center, align=align)
 
@@ -276,14 +274,25 @@
             [
                 k
                 for k, v in coordinates.get_exp_conditions.items()
                 if v[exp_condition].values == condition_value
             ]
         )
 
+    # Filter for specific time bin
+    if bin_size is not None:
+        bin_size = bin_size * coordinates._frame_rate
+        coords = {
+            key: val.iloc[
+                bin_size
+                * bin_index : np.minimum(val.shape[0], bin_size * (bin_index + 1))
+            ]
+            for key, val in coords.items()
+        }
+
     if not center:  # pragma: no cover
         warnings.warn("Heatmaps look better if you center the data")
 
     # Add experimental conditions to title, if provided
     title_suffix = experiment_id
     if coordinates.get_exp_conditions is not None and exp_condition is None:
         title_suffix += (
@@ -328,81 +337,105 @@
 
 def plot_gantt(
     coordinates: project,
     experiment_id: str,
     soft_counts: table_dict = None,
     supervised_annotations: table_dict = None,
     additional_checkpoints: pd.DataFrame = None,
+    signal_overlay: pd.Series = None,
+    behaviors_to_plot: list = None,
     save: bool = False,
 ):
-    """Returns a scatter plot of the passed projection. Allows for temporal and quality filtering, animal aggregation,
-    and changepoint detection size visualization.
+    """Return a scatter plot of the passed projection. Allows for temporal and quality filtering, animal aggregation, and changepoint detection size visualization.
 
     Args:
         coordinates (project): deepOF project where the data is stored.
         experiment_id (str): Name of the experiment to display.
         soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
-        supervised_annotations (table_dict): table dict with supervised annotations per video.
-        new figure will be created.
+        supervised_annotations (table_dict): table dict with supervised annotations per video. new figure will be created.
         additional_checkpoints (pd.DataFrame): table with additional checkpoints to plot.
+        signal_overlay (pd.Series): overlays a continuous signal with all selected behaviors. None by default.
+        behaviors_to_plot (list): list of behaviors to plot. If None, all behaviors are plotted.
         save (bool): Saves a time-stamped vectorized version of the figure if True.
 
     """
     # Determine plot type
     if soft_counts is None and supervised_annotations is not None:
         plot_type = "supervised"
     elif soft_counts is not None and supervised_annotations is None:
         plot_type = "unsupervised"
     else:
         plot_type = "mixed"
 
     if plot_type == "unsupervised":
         hard_counts = soft_counts[experiment_id].argmax(axis=1)
-        gantt = np.zeros([hard_counts.max() + 1, hard_counts.shape[0]])
+        n_features = hard_counts.max() + 1
+        if behaviors_to_plot is not None:
+            gantt = np.zeros([len(behaviors_to_plot), hard_counts.shape[0]])
+        else:
+            gantt = np.zeros([hard_counts.max() + 1, hard_counts.shape[0]])
 
     elif plot_type == "supervised":
-        row_shape = supervised_annotations[experiment_id].shape[1] - len(
-            [
-                col
-                for col in supervised_annotations[experiment_id].columns
-                if "speed" in col
-            ]
-        )
+        behavior_ids = [
+            col
+            for col in supervised_annotations[experiment_id].columns
+            if "speed" not in col
+        ]
+        n_features = len(behavior_ids)
+        row_shape = n_features if behaviors_to_plot is None else len(behaviors_to_plot)
         gantt = np.zeros(
             [
                 row_shape,
                 supervised_annotations[experiment_id].shape[0],
             ]
         )
 
     # If available, add additional checkpoints to the Gantt matrix
     if additional_checkpoints is not None:
         additional_checkpoints = additional_checkpoints.iloc[:, : gantt.shape[1]]
-        gantt = np.concatenate([gantt, additional_checkpoints], axis=0)
+        if behaviors_to_plot is not None:
+            gantt = np.zeros([len(behaviors_to_plot), hard_counts.shape[0]])
+        else:
+            gantt = np.concatenate([gantt, additional_checkpoints], axis=0)
 
     colors = np.tile(
         list(sns.color_palette("tab20").as_hex()), int(np.ceil(gantt.shape[0] / 20))
     )
 
     # Iterate over unsupervised clusters and plot
     rows = 0
 
-    for cluster, color in zip(range(gantt.shape[0]), colors):
+    for cluster, color in zip(range(n_features), colors):
 
         if plot_type == "unsupervised":
-            gantt[cluster] = hard_counts == cluster
+            if behaviors_to_plot is not None:
+                if cluster not in behaviors_to_plot:
+                    continue
+            gantt[rows] = hard_counts == cluster
         elif plot_type == "supervised":
+            if behaviors_to_plot is not None:
+                if behavior_ids[cluster] not in behaviors_to_plot:
+                    continue
             if "speed" in supervised_annotations[experiment_id].iloc[:, cluster].name:
                 continue
-            gantt[cluster] = supervised_annotations[experiment_id].iloc[:, cluster]
+            gantt[rows] = supervised_annotations[experiment_id].iloc[:, cluster]
 
         gantt_cp = gantt.copy()
-        gantt_cp[[i for i in range(gantt.shape[0]) if i != cluster]] = np.nan
-        plt.axhline(y=cluster, color="k", linewidth=0.5)
+        gantt_cp[[i for i in range(gantt.shape[0]) if i != rows]] = np.nan
+
+        if signal_overlay is not None:
+            standard_signal = (signal_overlay - signal_overlay.min()) / (
+                signal_overlay.max() - signal_overlay.min()
+            )
+            sns.lineplot(
+                x=signal_overlay.index, y=standard_signal + rows, color="black"
+            )
+
         rows += 1
+        plt.axhline(y=rows, color="k", linewidth=0.5)
 
         sns.heatmap(
             data=gantt_cp,
             cbar=False,
             cmap=LinearSegmentedColormap.from_list("deepof", ["white", color], N=2),
         )
 
@@ -419,29 +452,36 @@
                 data=gantt_cp,
                 cbar=False,
                 cmap=LinearSegmentedColormap.from_list(
                     "deepof", ["white", "black"], N=2
                 ),
             )
 
+    # Set ticks
+    if plot_type == "unsupervised":
+        behavior_ticks = np.array(
+            [
+                f"Cluster {cluster}"
+                for cluster in range(n_features)
+                if behaviors_to_plot is None or cluster in behaviors_to_plot
+            ]
+        )
+    elif plot_type == "supervised":
+        behavior_ticks = (
+            behavior_ids if behaviors_to_plot is None else behaviors_to_plot
+        )
+
     plt.xticks([])
+
     plt.yticks(
         np.array(range(gantt.shape[0])) + 0.5,
         # Concatenate cluster IDs and checkpoint names if they exist
         np.concatenate(
             [
-                (
-                    np.arange(hard_counts.max() + 1)
-                    if plot_type == "unsupervised"
-                    else [
-                        col
-                        for col in supervised_annotations[experiment_id].columns
-                        if "speed" not in col
-                    ]
-                ),
+                behavior_ticks,
                 np.array(additional_checkpoints.index)
                 if additional_checkpoints is not None
                 else [],
             ]
         ),
         rotation=0,
         fontsize=10,
@@ -484,15 +524,15 @@
     plot_proportions: bool = True,
     add_stats: str = "Mann-Whitney",
     # Quality selection parameters
     min_confidence: float = 0.0,
     # Time selection parameters
     bin_size: int = None,
     bin_index: int = 0,
-    precomputed: np.ndarray = None,
+    precomputed_bins: np.ndarray = None,
     # Visualization parameters
     exp_condition: str = None,
     exp_condition_order: list = None,
     normalize: bool = False,
     verbose: bool = False,
     ax: Any = None,
     save: bool = False,
@@ -501,26 +541,22 @@
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         embeddings (table_dict): table dict with neural embeddings per animal experiment across time.
         soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
         breaks (table_dict): table dict with changepoint detection breaks per experiment.
         supervised_annotations (table_dict): table dict with supervised annotations per animal experiment across time.
-        plot_proportions (bool): if supervised annotations are provided, display only traits that are measured
-        as proportions instead of real values. Useful to visualize traits with different scales.
-        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one
-        available is used.
-        exp_condition_order (list): Order in which to plot experimental conditions. If None (default), the order
-        is determined by the order of the keys in the table dict.
+        plot_proportions (bool): if supervised annotations are provided, display only traits that are measured as proportions instead of real values. Useful to visualize traits with different scales.
+        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one available is used.
+        exp_condition_order (list): Order in which to plot experimental conditions. If None (default), the order is determined by the order of the keys in the table dict.
         min_confidence (float): minimum confidence in cluster assignments used for quality control filtering.
         bin_size (int): bin size for time filtering.
         bin_index (int): index of the bin of size bin_size to select along the time dimension.
-        precomputed (np.ndarray): precomputed time bins. If provided, bin_size and bin_index are ignored.
-        add_stats (bool): whether to add stats to the plots. Defaults to True.
-        may hurt performance.
+        precomputed_bins (np.ndarray): precomputed time bins. If provided, bin_size and bin_index are ignored.
+        add_stats (str): test to use. Mann-Whitney (non-parametric) by default. See statsannotations documentation for details.
         verbose (bool): if True, prints test results and p-value cutoffs. False by default.
         ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, new figure will be created.
         save (bool): Saves a time-stamped vectorized version of the figure if True.
         normalize (bool): whether to represent time fractions or actual time in seconds on the y axis.
 
     """
     # Get requested experimental condition. If none is provided, default to the first one available.
@@ -552,15 +588,15 @@
         embedding=embeddings,
         soft_counts=soft_counts,
         breaks=breaks,
         supervised_annotations=supervised_annotations,
         exp_conditions=exp_conditions,
         bin_size=(coordinates._frame_rate * bin_size if bin_size is not None else None),
         bin_index=bin_index,
-        precomputed=precomputed,
+        precomputed=precomputed_bins,
         normalize=normalize,
     )
 
     if exp_condition_order is not None:
         enrichment["exp condition"] = pd.Categorical(
             enrichment["exp condition"], exp_condition_order
         )
@@ -591,34 +627,39 @@
 
     handles, labels = ax.get_legend_handles_labels()
     ax.legend(
         handles[2:], labels[2:], bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.0
     )
 
     if add_stats:
-        if supervised_annotations is None:
-            pairs = list(
-                product(
-                    set(np.concatenate(list(soft_counts.values())).argmax(axis=1)),
-                    set(exp_conditions.values()),
-                )
-            )
-        else:
-            pairs = list(
-                product(
-                    list(supervised_annotations.values())[0].columns,
-                    set(exp_conditions.values()),
-                )
+        pairs = list(
+            product(
+                set(
+                    np.concatenate(list(soft_counts.values())).argmax(axis=1)
+                    if supervised_annotations is None
+                    else list(supervised_annotations.values())[0].columns
+                ),
+                set(exp_conditions.values()),
             )
+        )
         pairs = [
-            list(map(tuple, p))
+            [list(i) for i in list(combinations(list(map(tuple, p)), 2))]
             for p in np.array(pairs)
-            .reshape([-1, 2, len(set(exp_conditions.values()))])
+            .reshape([-1, len(set(exp_conditions.values())), 2])
             .tolist()
         ]
+        pairs = [item for sublist in pairs for item in sublist]
+
+        # Remove elements from pairs if clusters are not present in the enrichment data frame
+        pairs = [
+            p
+            for p in pairs
+            if p[0][0] in enrichment["cluster"].values
+            and p[1][0] in enrichment["cluster"].values
+        ]
 
         annotator = Annotator(
             ax,
             pairs=pairs,
             data=enrichment,
             x="cluster",
             y="time on cluster",
@@ -673,26 +714,24 @@
     visualization="networks",
     silence_diagonal=False,
     cluster: bool = True,
     axes: list = None,
     save: bool = False,
     **kwargs,
 ):
-    """Computes and plots transition matrices for all data or per condition. Plots can be heatmaps or networks.
+    """Compute and plots transition matrices for all data or per condition. Plots can be heatmaps or networks.
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         embeddings (table_dict): table dict with neural embeddings per animal experiment across time.
         soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
         breaks (table_dict): table dict with changepoint detection breaks per experiment.
-        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one
-        available is used.
+        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one available is used.
         bin_size (int): bin size for time filtering.
-        bin_index (int): index of the bin of size bin_size to select along the time dimension.
-        new figure will be created.
+        bin_index (int): index of the bin of size bin_size to select along the time dimension. new figure will be created.
         visualization (str): visualization mode. Can be either 'networks', or 'heatmaps'.
         silence_diagonal (bool): If True, diagonals are set to zero.
         cluster (bool): If True (default) rows and columns on heatmaps are hierarchically clustered.
         axes (list): axes where to plot the current figure. If not provided, a new figure will be created.
         save (bool): Saves a time-stamped vectorized version of the figure if True.
 
     """
@@ -706,15 +745,15 @@
         }
 
     grouped_transitions = deepof.post_hoc.compute_transition_matrix_per_condition(
         embeddings,
         soft_counts,
         breaks,
         exp_conditions,
-        bin_size=bin_size,
+        bin_size=(coordinates._frame_rate * bin_size if bin_size is not None else None),
         bin_index=bin_index,
         silence_diagonal=silence_diagonal,
         aggregate=(exp_conditions is not None),
         normalize=True,
     )
 
     if exp_conditions is None:
@@ -831,51 +870,52 @@
     bin_index: int = 0,
     # Visualization parameters
     exp_condition: str = None,
     verbose: bool = False,
     ax: Any = None,
     save: bool = False,
 ):
-    """Computes and plots transition stationary distribution entropy per condition.
+    """Compute and plots transition stationary distribution entropy per condition.
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         embeddings (table_dict): table dict with neural embeddings per animal experiment across time.
         soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
         breaks (table_dict): table dict with changepoint detection breaks per experiment.
-        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one
-        available is used.
-        add_stats (bool): whether to add stats to the plots. Defaults to True.
+        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one available is used.
+        add_stats (str): test to use. Mann-Whitney (non-parametric) by default. See statsannotations documentation for details.
         bin_size (int): bin size for time filtering.
         bin_index (int): index of the bin of size bin_size to select along the time dimension.
         verbose (bool): if True, prints test results and p-value cutoffs. False by default.
-        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided,
-        new figure will be created.
+        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, new figure will be created.
         save (bool): Saves a time-stamped vectorized version of the figure if True.
 
     """
     # Get requested experimental condition. If none is provided, default to the first one available.
     if exp_condition is None:
         exp_conditions = {
             key: val.iloc[:, 0].values[0]
-            for key, val in coordinates.get_exp_conditions.items()
+            for key, val in embeddings._exp_conditions.items()
         }
     else:
         exp_conditions = {
             key: val.loc[:, exp_condition].values[0]
-            for key, val in coordinates.get_exp_conditions.items()
+            for key, val in embeddings._exp_conditions.items()
         }
 
+    soft_counts = soft_counts.filter_videos(embeddings.keys())
+    breaks = breaks.filter_videos(embeddings.keys())
+
     # Get ungrouped entropy scores for the full videos
     ungrouped_transitions = deepof.post_hoc.compute_transition_matrix_per_condition(
         embeddings,
         soft_counts,
         breaks,
         exp_conditions,
-        bin_size=bin_size,
+        bin_size=(bin_size * coordinates._frame_rate if bin_size is not None else None),
         bin_index=bin_index,
         aggregate=False,
         normalize=True,
     )
     ungrouped_entropy_scores = deepof.post_hoc.compute_steady_state(
         ungrouped_transitions, return_entropy=True, n_iters=10000
     )
@@ -946,52 +986,58 @@
 
 def _filter_embeddings(
     coordinates,
     embeddings,
     soft_counts,
     breaks,
     supervised_annotations,
-    use_keys,
     exp_condition,
     bin_size,
     bin_index,
+    precomputed_bins,
 ):
     """Auxiliary function to plot_embeddings. Filters all available data based on the provided keys and experimental condition."""
-
     # Get experimental conditions per video
-    if exp_condition is None:
-        exp_condition = list(coordinates.get_exp_conditions.values())[0].columns[0]
+    if embeddings is None and supervised_annotations is None:
+        raise ValueError(
+            "Either embeddings, soft_counts, and breaks or supervised_annotations must be provided."
+        )
 
-    concat_hue = [
-        i[exp_condition].values[0]
-        for i in list(coordinates.get_exp_conditions.values())
-    ]
+    try:
+        if exp_condition is None:
+            exp_condition = list(embeddings._exp_conditions.values())[0].columns[0]
+
+        concat_hue = [
+            coordinates.get_exp_conditions[i][exp_condition].values[0]
+            for i in list(embeddings.keys())
+        ]
+        soft_counts = soft_counts.filter_videos(embeddings.keys())
+        breaks = breaks.filter_videos(embeddings.keys())
+
+    except AttributeError:
+        if exp_condition is None:
+            exp_condition = list(supervised_annotations._exp_conditions.values())[
+                0
+            ].columns[0]
 
-    if use_keys is not None:
-        try:
-            try:
-                embeddings = {key: embeddings[key] for key in use_keys}
-                soft_counts = {key: soft_counts[key] for key in use_keys}
-                breaks = {key: breaks[key] for key in use_keys}
-            except AttributeError:
-                supervised_annotations = {
-                    key: supervised_annotations[key] for key in use_keys
-                }
-        except AttributeError:
-            raise ValueError(
-                "Either embeddings, soft_counts, and breaks or supervised_annotations must be provided."
-            )
         concat_hue = [
-            j
-            for i, j in zip(list(coordinates.get_exp_conditions.keys()), concat_hue)
-            if i in use_keys
+            coordinates.get_exp_conditions[i][exp_condition].values[0]
+            for i in list(supervised_annotations.keys())
         ]
 
     # Restrict embeddings, soft_counts and breaks to the selected time bin
-    if bin_size is not None:
+    if precomputed_bins is not None:
+        embeddings, soft_counts, breaks, _ = deepof.post_hoc.select_time_bin(
+            embeddings,
+            soft_counts,
+            breaks,
+            precomputed=(precomputed_bins == bin_index),
+        )
+
+    elif bin_size is not None:
         if embeddings is not None:
             embeddings, soft_counts, breaks, _ = deepof.post_hoc.select_time_bin(
                 embeddings,
                 soft_counts,
                 breaks,
                 bin_size=coordinates._frame_rate * bin_size,
                 bin_index=bin_index,
@@ -1026,82 +1072,211 @@
                 for key, val in supervised_annotations.items()
                 if key in coordinates.get_exp_conditions.keys()
             }
 
     return embeddings, soft_counts, breaks, supervised_annotations, concat_hue
 
 
+def plot_normative_log_likelihood(
+    embeddings: table_dict,
+    exp_condition: str,
+    embedding_dataset: pd.DataFrame,
+    normative_model: str,
+    ax: Any,
+    add_stats: str,
+    verbose: bool,
+):
+    """Plot a bar chart with normative log likelihoods per experimental condition, and compute statistics.
+
+    Args:
+        embeddings (table_dict): table dictionary containing unsupervised embeddings per animal.
+        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one available is used.
+        embedding_dataset (pd.DataFrame): global animal embeddings, alongside their respective experimental conditions
+        normative_model (str): Name of the cohort to use as controls. If provided, fits a Gaussian density to the control global animal embeddings, and reports the difference in likelihood across all instances of the provided experimental condition. Statistical parameters can be controlled via **kwargs (see full documentation for details).
+        ax (plt.AxesSubplot): matplotlib axes where to render the plot
+        add_stats (str): test to use. Mann-Whitney (non-parametric) by default. See statsannotations documentation for details.
+        verbose (bool): if True, prints test results and p-value cutoffs. False by default.
+
+    Returns:
+        embedding_dataset (pd.DataFrame): embedding data frame with added normative scores per sample
+
+    """
+    # Fit normative model to animals belonging to the control cohort
+    norm_density = deepof.post_hoc.fit_normative_global_model(
+        embedding_dataset.loc[
+            embedding_dataset["experimental condition"] == normative_model,
+            ["PCA-1", "PCA-2"],
+        ]
+    )
+
+    # Add normative log likelihood to the dataset
+    embedding_dataset["norm_scores"] = norm_density.score_samples(
+        embedding_dataset.loc[:, ["PCA-1", "PCA-2"]].values
+    )
+
+    # Center log likelihood values around the control mean
+    embedding_dataset["norm_scores"] -= embedding_dataset.loc[
+        embedding_dataset["experimental condition"] == normative_model,
+        "norm_scores",
+    ].mean()
+
+    # Add a second axis to the right of the main plot, and show the corresponding bar charts
+    if ax is None:
+        fig, (ax, ax2) = plt.subplots(
+            1, 2, figsize=(12, 6), gridspec_kw={"width_ratios": [3, 1]}
+        )
+
+    elif isinstance(ax, list):
+        ax, ax2 = ax
+
+    else:
+        raise ValueError(
+            "Passing normative_model produces two plots: a scatterplot with a PCA of the embeddings"
+            "themselves, and a barplot depicting the normative likelihood per condition. Instead of"
+            "a single ax, pass a list with two."
+        )
+
+    sns.boxplot(
+        data=embedding_dataset.sort_values(
+            "experimental condition",
+            key=lambda x: x == normative_model,
+            ascending=False,
+        ),
+        x="experimental condition",
+        y="norm_scores",
+        ax=ax2,
+    )
+    sns.stripplot(
+        data=embedding_dataset.sort_values(
+            "experimental condition",
+            key=lambda x: x == normative_model,
+            ascending=False,
+        ),
+        x="experimental condition",
+        y="norm_scores",
+        dodge=True,
+        color="black",
+        ax=ax2,
+    )
+
+    ax2.set_xlabel("")
+    ax2.set_ylabel("centered normative log likelihood")
+
+    # Add statistics
+    if exp_condition is None:
+        exp_conditions = {
+            key: val.iloc[:, 0].values[0]
+            for key, val in embeddings._exp_conditions.items()
+        }
+    else:
+        exp_conditions = {
+            key: val.loc[:, exp_condition].values[0]
+            for key, val in embeddings._exp_conditions.items()
+        }
+
+    embedding_dataset.index = embeddings._exp_conditions.keys()
+    embedding_dataset.sort_values(
+        "experimental condition",
+        key=lambda x: x == normative_model,
+        ascending=False,
+        inplace=True,
+    )
+
+    pairs = [
+        pair
+        for pair in list(combinations(set(exp_conditions.values()), 2))
+        if normative_model in pair
+    ]
+
+    annotator = Annotator(
+        pairs=pairs,
+        data=embedding_dataset,
+        x="experimental condition",
+        y="norm_scores",
+        ax=ax2,
+    )
+    annotator.configure(
+        test=add_stats,
+        verbose=verbose,
+    )
+    annotator.apply_and_annotate()
+
+    return embedding_dataset, False, ax
+
+
 def plot_embeddings(
     coordinates: coordinates,
     embeddings: table_dict = None,
     soft_counts: table_dict = None,
     breaks: table_dict = None,
     supervised_annotations: table_dict = None,
     # Quality selection parameters
     min_confidence: float = 0.0,
     # Time selection parameters
     bin_size: int = None,
     bin_index: int = 0,
+    precomputed_bins: np.ndarray = None,
+    # Normative modelling
+    normative_model: str = None,
+    add_stats: str = "Mann-Whitney",
+    verbose: bool = False,
     # Visualization design and data parameters
     exp_condition: str = None,
-    use_keys: list = None,
     aggregate_experiments: str = False,
     samples: int = 500,
     show_aggregated_density: bool = True,
     colour_by: str = "cluster",
     show_break_size_as_radius: bool = False,
     ax: Any = None,
     save: bool = False,
 ):
-    """Returns a scatter plot of the passed projection. Allows for temporal and quality filtering, animal aggregation,
-    and changepoint detection size visualization.
+    """Return a scatter plot of the passed projection. Allows for temporal and quality filtering, animal aggregation, and changepoint detection size visualization.
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         embeddings (table_dict): table dict with neural embeddings per animal experiment across time.
         soft_counts (table_dict): table dict with soft cluster assignments per animal experiment across time.
         breaks (table_dict): table dict with changepoint detection breaks per experiment.
         supervised_annotations (table_dict): table dict with supervised annotations per experiment.
-        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one
-        available is used.
-        use_keys (list): list of keys to use for plotting. If None (default), all keys are used.
+        exp_condition (str): Name of the experimental condition to use when plotting. If None (default) the first one available is used.
+        normative_model (str): Name of the cohort to use as controls. If provided, fits a Gaussian density to the control global animal embeddings, and reports the difference in likelihood across all instances of the provided experimental condition. Statistical parameters can be controlled via **kwargs (see full documentation for details).
+        add_stats (str): test to use. Mann-Whitney (non-parametric) by default. See statsannotations documentation for details.
+        verbose (bool): if True, prints test results and p-value cutoffs. False by default.
         min_confidence (float): minimum confidence in cluster assignments used for quality control filtering.
         bin_size (int): bin size for time filtering.
         bin_index (int): index of the bin of size bin_size to select along the time dimension.
+        precomputed_bins (np.ndarray): precomputed time bins. If provided, bin_size and bin_index are ignored.
         aggregate_experiments (str): Whether to aggregate embeddings by experiment (by time on cluster, mean, or median) or not (default).
-        samples (int): Number of samples to take from the time embeddings. None leads to plotting all time-points, which
-        may hurt performance.
+        samples (int): Number of samples to take from the time embeddings. None leads to plotting all time-points, which may hurt performance.
         show_aggregated_density (bool): if True, a density plot is added to the aggregated embeddings.
         colour_by (str): hue by which to colour the embeddings. Can be one of 'cluster' (default), 'exp_condition', or 'exp_id'.
-        show_break_size_as_radius (bool): Only usable when embeddings come from a model using changepoint detection. If True,
-        the size of each chunk is depicted as the radius of each dot.
-        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided,
-        new figure will be created.
+        show_break_size_as_radius (bool): Only usable when embeddings come from a model using changepoint detection. If True, the size of each chunk is depicted as the radius of each dot.
+        ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, new figure will be created.
         save (bool): Saves a time-stamped vectorized version of the figure if True.
 
     """
-
     # Filter embeddings, soft_counts, breaks and supervised_annotations based on the provided keys and experimental condition
     (
         emb_to_plot,
         counts_to_plot,
         breaks_to_plot,
         sup_annots_to_plot,
         concat_hue,
     ) = _filter_embeddings(
         coordinates,
         copy.deepcopy(embeddings),
         copy.deepcopy(soft_counts),
         copy.deepcopy(breaks),
         copy.deepcopy(supervised_annotations),
-        use_keys,
         exp_condition,
         bin_size,
         bin_index,
+        precomputed_bins,
     )
+    show = True
 
     # Plot unravelled temporal embeddings
     if not aggregate_experiments and emb_to_plot is not None:
 
         if samples is not None:
 
             # Sample per animal, to avoid alignment issues
@@ -1177,31 +1352,33 @@
                     emb_to_plot, agg=aggregate_experiments, reduce_dim=True
                 )
             else:
                 aggregated_embeddings = deepof.post_hoc.get_aggregated_embedding(
                     sup_annots_to_plot, agg=aggregate_experiments, reduce_dim=True
                 )
 
-        aggregated_embeddings = aggregated_embeddings.loc[
-            (coordinates.get_exp_conditions.keys() if use_keys is None else use_keys), :
-        ]
-
         # Generate unifier dataset using the reduced aggregated embeddings and experimental conditions
         embedding_dataset = pd.DataFrame(
             {
                 "PCA-1": aggregated_embeddings[0],
                 "PCA-2": aggregated_embeddings[1],
                 "experimental condition": concat_hue,
             }
         )
 
-        embedding_dataset.index = (
-            coordinates.get_exp_conditions.keys() if use_keys is None else use_keys
-        )
-        embedding_dataset.sort_values("experimental condition", inplace=True)
+        if normative_model:
+            embedding_dataset, show, ax = plot_normative_log_likelihood(
+                embeddings,
+                exp_condition,
+                embedding_dataset,
+                normative_model,
+                ax,
+                add_stats,
+                verbose,
+            )
 
     # Plot selected embeddings using the specified settings
     sns.scatterplot(
         data=embedding_dataset,
         x="{}-1".format("PCA" if aggregate_experiments else "UMAP"),
         y="{}-2".format("PCA" if aggregate_experiments else "UMAP"),
         ax=ax,
@@ -1254,15 +1431,15 @@
             )
         )
 
     title = "deepOF - {}supervised {}embedding".format(
         ("un" if sup_annots_to_plot is None else ""),
         ("aggregated " if aggregate_experiments else ""),
     )
-    if ax is not None:
+    if ax is not None or not show:
         ax.set_title(title, fontsize=15)
 
     else:
         plt.title(title, fontsize=15)
         plt.tight_layout()
         plt.show()
 
@@ -1271,15 +1448,15 @@
     embeddings: np.ndarray,
     cluster_assignments: np.ndarray = None,
     ax: Any = None,
     save: str = False,
     show: bool = True,
     dpi: int = 200,
 ) -> plt.figure:
-    """Returns a scatter plot of the passed projection. Each dot represents the trajectory of an entire animal.
+    """Return a scatter plot of the passed projection. Each dot represents the trajectory of an entire animal.
 
     If labels are propagated, it automatically colours all data points with their respective condition.
 
     Args:
         embeddings (tuple): sequence embeddings obtained with the unsupervised pipeline within deepof
         cluster_assignments (tuple): labels of the clusters. If None, aggregation method should be provided.
         ax: axes where to plot the arena.
@@ -1311,16 +1488,15 @@
     if not show:
         return ax
 
     plt.show()
 
 
 def _get_polygon_coords(data, animal_id=""):
-    """Generates polygons to animate for the indicated animal in the provided dataframe."""
-
+    """Generate polygons to animate for the indicated animal in the provided dataframe."""
     if animal_id:
         animal_id += "_"
 
     elif animal_id is None:
         animal_id = ""
 
     head = np.concatenate(
@@ -1365,15 +1541,14 @@
     min_confidence,
     min_bout_duration,
     cluster_assignments,
     embedding,
     selected_cluster,
 ):
     """Auxiliary function to process data for animation outputs."""
-
     data = coordinates.get_coords(center=center, align=align)
     cluster_embedding, concat_embedding = None, None
 
     # Filter requested animals
     if animal_id:
         data = data.filter_id(animal_id)
 
@@ -1497,40 +1672,33 @@
     embedding: Union[List, np.ndarray] = None,
     selected_cluster: np.ndarray = None,
     display_arena: bool = True,
     legend: bool = True,
     save: bool = None,
     dpi: int = 300,
 ):
-    """Renders a FuncAnimation object with embeddings and/or motion trajectories over time.
+    """Render a FuncAnimation object with embeddings and/or motion trajectories over time.
 
     Args:
         coordinates (coordinates): deepof Coordinates object.
         experiment_id (str): Name of the experiment to display.
         animal_id (list): ID list of animals to display. If None (default) it shows all animals.
-        center (str): Name of the body part to which the positions will be centered. If false,
-        the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
-        align (str): Selects the body part to which later processes will align the frames with
-        (see preprocess in table_dict documentation).
+        center (str): Name of the body part to which the positions will be centered. If false, the raw data is returned; if 'arena' (default), coordinates are centered in the pitch.
+        align (str): Selects the body part to which later processes will align the frames with (see preprocess in table_dict documentation).
         frame_limit (int): Number of frames to plot. If None, the entire video is rendered.
         min_confidence (float): Minimum confidence threshold to render a cluster assignment bout.
         min_bout_duration (int): Minimum number of frames to render a cluster assignment bout.
-        cluster_assignments (np.ndarray): contain sorted cluster assignments for all instances in data.
-        If provided together with selected_cluster, only instances of the specified component are returned.
-        Defaults to None.
-        only instances of the specified component are returned. Defaults to None.
-        embedding (Union[List, np.ndarray]): UMAP 2D embedding of the datapoints provided. If not None, a second animation
-        shows a parallel animation showing the currently selected embedding, colored by cluster if cluster_assignments
-        are available.
+        cluster_assignments (np.ndarray): contain sorted cluster assignments for all instances in data. If provided together with selected_cluster, only instances of the specified component are returned. Defaults to None.
+        embedding (Union[List, np.ndarray]): UMAP 2D embedding of the datapoints provided. If not None, a second animation shows a parallel animation with the currently selected embedding, colored by cluster if cluster_assignments are available.
         selected_cluster (int): cluster to filter. If provided together with cluster_assignments,
         display_arena (bool): whether to plot a dashed line with an overlying arena perimeter. Defaults to True.
-        legend (bool): whether to add a color-coded legend to multi-animal plots. Defaults to True when there are more
-        than one animal in the representation, False otherwise.
+        legend (bool): whether to add a color-coded legend to multi-animal plots. Defaults to True when there are more than one animal in the representation, False otherwise.
         save (str): name of the file where to save the produced animation.
         dpi (int): dots per inch of the figure to create.
+
     """
     # Get and process data to plot from coordinates object
     (
         data,
         x_dv,
         y_dv,
         embedding,
@@ -1732,24 +1900,25 @@
     cluster_gbm_performance: dict,
     hard_counts: np.ndarray,
     groups: list,
     save: bool = False,
     visualization: str = "confusion_matrix",
     ax: plt.Axes = None,
 ):
-    """Plots either a confusion matrix or a bar chart with balanced accuracy for cluster detection cross validated models.
+    """Plot either a confusion matrix or a bar chart with balanced accuracy for cluster detection cross validated models.
+
     Designed to be run after deepof.post_hoc.train_supervised_cluster_detectors (see documentation for details).
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         chunk_stats (pd.DataFrame): table with descriptive statistics for a series of sequences ('chunks').
         cluster_gbm_performance (dict): cross-validated dictionary containing trained estimators and performance metrics.
         hard_counts (np.ndarray): cluster assignments for the corresponding 'chunk_stats' table.
         groups (list): cross-validation indices. Data from the same animal are never shared between train and test sets.
-        save: name of the file where to save the produced figure.
+        save (bool): name of the file where to save the produced figure.
         visualization (str): plot to render. Must be one of 'confusion_matrix', or 'balanced_accuracy'.
         ax (plt.Axes): axis where to plot the figure. If None, a new figure is created.
 
     """
     n_clusters = len(np.unique(hard_counts))
     confusion_matrices = []
 
@@ -1778,27 +1947,26 @@
             cm, method="average", metric="euclidean"
         )  # computing the linkage
         row_order = dendrogram(row_link, no_plot=True)["leaves"]
         cm = cm.iloc[row_order, row_order]
 
         ax.set_title("Confusion matrix for multiclass state prediction")
         sns.heatmap(cm, annot=True, cmap="Blues", ax=ax)
-        ax.set_yticks(ax.get_yticks(), rotation=45)
+        ax.set_yticks(ax.get_yticks(), ax.get_yticklabels(), rotation=0)
 
     elif visualization == "balanced_accuracy":
 
         def compute_balanced_accuracy(cm, cluster_index):
             """
 
-            Computes balanced accuracy for a specific cluster given a confusion matrix
+            Compute balanced accuracy for a specific cluster given a confusion matrix.
 
             Formula: ((( TP / (TP+FN) + (TN/(TN+FP))) / 2
 
             """
-
             TP = cm[cluster_index, cluster_index]
             FP = cm[:, cluster_index].sum() - TP
             FN = cm[cluster_index, :].sum() - TP
             TN = cm.sum() - TP - FP - FN
 
             return ((TP / (TP + FN)) + (TN / (TN + FP))) / 2
 
@@ -1855,22 +2023,21 @@
     data_to_explain: pd.DataFrame,
     shap_values: list,
     cluster: Union[str, int] = "all",
     max_display: int = 10,
     save: str = False,
     show: bool = True,
 ):
-    """
+    """Plot a swarm plot of the SHAP values for a given cluster.
 
     Args:
         coordinates (coordinates): deepOF project where the data is stored.
         data_to_explain (pd.DataFrame): table with descriptive statistics for a series of sequences ('chunks').
         shap_values (list): shap_values per cluster.
-        cluster: cluster to plot. If "all" (default) global feature importance
-        across all clusters is depicted in a bar chart.
+        cluster (int): cluster to plot. If "all" (default) global feature importance across all clusters is depicted in a bar chart.
         max_display (int): maximum number of features to display.
         save (str): if provided, saves the figure to the specified file.
         show (bool): if True, shows the figure.
 
     """
     shap_vals = copy.deepcopy(shap_values)
 
@@ -1887,17 +2054,17 @@
 
     if save:
         plt.savefig(
             os.path.join(
                 coordinates._project_path,
                 coordinates._project_name,
                 "Figures",
-                "deepof_supervised_cluster_detection_SHAP{}_{}.pdf".format(
+                "deepof_supervised_cluster_detection_SHAP_cluster={}{}_{}.pdf".format(
+                    cluster,
                     (f"_{save}" if isinstance(save, str) else ""),
-                    visualization,
                     calendar.timegm(time.gmtime()),
                 ),
             )
         )
 
     if show:
         plt.show()
@@ -1908,15 +2075,15 @@
     out: Any,
     frame_mask: list,
     v_width: int,
     v_height: int,
     path: str,
     frame_limit: int = np.inf,
 ):
-    """Outputs a video with the frames corresponding to the cluster.
+    """Output a video with the frames corresponding to the cluster.
 
     Args:
         cap: video capture object
         out: video writer object
         frame_mask: list of booleans indicating whether a frame should be written
         v_width: video width
         v_height: video height
@@ -2115,46 +2282,36 @@
             except IndexError:
                 ret = False
 
     cap.release()
     cv2.destroyAllWindows()
 
 
-def output_supervised_annotated_video():
-    """Given a video, and supervised assignments per frame, outputs a video with the frames annotated.
-
-    Args:
-
-    """
-    pass
-
-
 def export_annotated_video(
     coordinates: coordinates,
     soft_counts: dict = None,
     breaks: dict = None,
     experiment_id: str = None,
     min_confidence: float = 0.75,
     min_bout_duration: int = None,
     frame_limit_per_video: int = np.inf,
     exp_conditions: dict = {},
     cluster_names: dict = {},
 ):
-    """Generic function to export annotated videos from both supervised and unsupervised pipelines.
+    """Export annotated videos from both supervised and unsupervised pipelines.
 
     Args:
         coordinates (coordinates): coordinates object for the current project. Used to get video paths.
         soft_counts (dict): dictionary with soft_counts per experiment.
         breaks (dict): dictionary with break lengths for each video.r
         experiment_id (str): if provided, data coming from a particular experiment is used. If not, all experiments are exported.
         min_confidence (float): minimum confidence threshold for a frame to be considered part of a cluster.
         min_bout_duration (int): Minimum number of frames to render a cluster assignment bout.
         frame_limit_per_video (int): number of frames to render per video. If None, all frames are included for all videos.
-        exp_conditions (dict): if provided, data coming from a particular condition is used. If not, all conditions are exported.
-        If a dictionary with more than one entry is provided, the intersection of all conditions (i.e. male, stressed) is used.
+        exp_conditions (dict): if provided, data coming from a particular condition is used. If not, all conditions are exported. If a dictionary with more than one entry is provided, the intersection of all conditions (i.e. male, stressed) is used.
         cluster_names (dict): dictionary with user-defined names for each cluster (useful to output interpretation).
 
     """
     # Create output directory if it doesn't exist
     proj_path = os.path.join(coordinates._project_path, coordinates._project_name)
     out_path = os.path.join(proj_path, "Out_videos")
     if not os.path.exists(out_path):
@@ -2171,16 +2328,15 @@
         - soft_counts[first_key].shape[0]
         + 1
     )
 
     def filter_experimental_conditions(
         coordinates: coordinates, videos: list, conditions: list
     ):
-        """Returns a list of videos that match the provided experimental conditions."""
-
+        """Return a list of videos that match the provided experimental conditions."""
         filtered_videos = videos
 
         for condition, state in conditions.items():
 
             filtered_videos = [
                 video
                 for video in filtered_videos
@@ -2266,29 +2422,31 @@
     exp_condition: str,
     embedding_aggregation_method: str = "median",
     distance_metric: str = "wasserstein",
     n_jobs: int = -1,
     save: bool = False,
     ax: Any = None,
 ):
-    """Plots the distance between conditions across a growing time window. Finds an optimal separation binning based on the
-    distance between conditions, and plots the distance between conditions across all non-overlapping bins. Useful, for example,
-    to measure habituation across time.
+    """Plot the distance between conditions across a growing time window.
+
+    Finds an optimal separation binning based on the distance between conditions, and plots it across all non-overlapping bins.
+    Useful, for example, to measure habituation over time.
 
     Args:
         coordinates (coordinates): coordinates object for the current project. Used to get video paths.
         embedding (dict): embedding object for the current project. Used to get video paths.
         soft_counts (dict): dictionary with soft_counts per experiment.
         breaks (dict): dictionary with break lengths for each video.
         exp_condition (str): experimental condition to use for the distance calculation.
         embedding_aggregation_method (str): method to use for aggregating the embedding. Options are 'time_on_cluster' and 'mean'.
         distance_metric (str): distance metric to use for the distance calculation. Options are 'wasserstein' and 'euclidean'.
         n_jobs (int): number of jobs to use for the distance calculation.
         save (bool): if True, saves the figure to the project directory.
         ax (plt.AxesSubplot): axes where to plot the current figure. If not provided, new figure will be created.
+
     """
     # Get distance between distributions across the growing window
     distance_array = deepof.post_hoc.condition_distance_binning(
         embedding,
         soft_counts,
         breaks,
         {
@@ -2419,37 +2577,39 @@
     undercond,
     hparams,
     arena,
     arena_type,
     debug,
     coords,
 ):
-    """Helper function for annotate_video. Annotates a given frame with on-screen information
-    about the recognised patterns"""
+    """Annotate a given frame with on-screen information about the recognised patterns.
 
+    Helper function for annotate_video. No public use intended.
+
+    """
     arena, w, h = arena
 
     def write_on_frame(text, pos, col=(255, 255, 255)):
-        """Partial closure over cv2.putText to avoid code repetition"""
+        """Partial closure over cv2.putText to avoid code repetition."""
         return cv2.putText(frame, text, pos, font, 0.75, col, 2)
 
     def conditional_flag():
-        """Returns a tag depending on a condition"""
+        """Return a tag depending on a condition."""
         if frame_speeds[animal_ids[0]] > frame_speeds[animal_ids[1]]:
             return left_flag
         return right_flag
 
     def conditional_pos():
-        """Returns a position depending on a condition"""
+        """Return a position depending on a condition."""
         if frame_speeds[animal_ids[0]] > frame_speeds[animal_ids[1]]:
             return corners["downleft"]
         return corners["downright"]
 
     def conditional_col(cond=None):
-        """Returns a colour depending on a condition"""
+        """Return a colour depending on a condition."""
         if cond is None:
             cond = frame_speeds[animal_ids[0]] > frame_speeds[animal_ids[1]]
         if cond:
             return 150, 255, 150
         return 150, 150, 255
 
     # Keep track of space usage in the output video
@@ -2580,36 +2740,29 @@
     coordinates: coordinates,
     tag_dict: pd.DataFrame,
     vid_index: int,
     frame_limit: int = np.inf,
     debug: bool = False,
     params: dict = {},
 ) -> True:
-    """Renders a version of the input video with all supervised taggings in place.
+    """Render a version of the input video with all supervised taggings in place.
 
-    Parameters:
-        - coordinates (deepof.preprocessing.coordinates): coordinates object containing the project information
-        - debug (bool): if True, several debugging attributes (such as used body parts and arena) are plotted in
-        the output video
-        - vid_index: for internal usage only; index of the video to tag in coordinates._videos
-        - frame_limit (float): limit the number of frames to output. Generates all annotated frames by default
-        - params (dict): dictionary to overwrite the default values of the hyperparameters of the functions
-        that the supervised pose estimation utilizes.
-
-    Returns:
-        True
+    Args:
+        coordinates (deepof.preprocessing.coordinates): coordinates object containing the project information.
+        debug (bool): if True, several debugging attributes (such as used body parts and arena) are plotted in the output video.
+        vid_index: for internal usage only; index of the video to tag in coordinates._videos.
+        frame_limit (float): limit the number of frames to output. Generates all annotated frames by default.
+        params (dict): dictionary to overwrite the default values of the hyperparameters of the functions that the supervised pose estimation utilizes.
 
     """
-
     # Extract useful information from coordinates object
     tracks = list(coordinates._tables.keys())
     videos = coordinates._videos
     path = os.path.join(coordinates._project_path, coordinates._project_name, "Videos")
 
-    params = deepof.annotation_utils.get_hparameters(params)
     animal_ids = coordinates._animal_ids
     undercond = "_" if len(animal_ids) > 1 else ""
 
     try:
         vid_name = re.findall("(.*)DLC", tracks[vid_index])[0]
     except IndexError:
         vid_name = tracks[vid_index]
```

### Comparing `deepof-0.2/deepof.egg-info/PKG-INFO` & `deepof-0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-Metadata-Version: 2.1
-Name: deepof
-Version: 0.2
-Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
-Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
-Author: Lucas Miranda
-Author-email: lucas_miranda@psych.mpg.de
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.2-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.3-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
@@ -33,76 +19,83 @@
 basic social interactions) or to embed your data into a sequence-aware latent space to extract meaningful motifs in an
 unsupervised way! Both of these can be used within the package, for example, to automatically 
 compare user-defined experimental groups.
 
 ### How do I start?
 ##### Installation:
 
-The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof):
+The easiest way to install DeepOF is to use [pip](https://pypi.org/project/deepof). Create and activate a virtual environment with Python >=3.9 and <3.11, for example using conda:
+
+```bash
+conda create -n deepof python=3.9
+```
+
+Then, activate the environment and install DeepOF:
 
 ```bash
-   pip install deepof
+conda activate deepof
+pip install deepof
 ```
 
 Alternatively, you can download our pre-built [Docker image](https://hub.docker.com/repository/docker/lucasmiranda42/deepof),
 which contains all compatible dependencies:
 
 ```bash
-   # download the latest available image
-   docker pull lucasmiranda42/deepof:latest
-   # run the image in interactive mode, enabling you to open python and import deepof
-   docker run -it lucasmiranda42/deepof
+# download the latest available image
+docker pull lucasmiranda42/deepof:latest
+# run the image in interactive mode, enabling you to open python and import deepof
+docker run -it lucasmiranda42/deepof
 ```
 
 Or use [poetry](https://python-poetry.org/):
 
 ```bash
-   # after installing poetry and clonning the DeepOF repository, just run
-   poetry install # from the main directory
+# after installing poetry and clonning the DeepOF repository, just run
+poetry install # from the main directory
 ```
 
 ##### Before we delve in:
 DeepOF relies heavily on DeepLabCut's output. Thorough tutorials on how to get started with DLC for pose estimation can be found [here](https://www.mousemotorlab.org/deeplabcut).
 Once your videos are processed and tagged, you can use DeepOF to extract and annotate your motion-tracking time-series. While many features in DeepOF can work regardless of the set of labels used, we currently recommend using videos from a top-down perspective, and follow our recommended
 set of labels (which can be found in the full documentation page). A pre-trained model capable of recognizing **C57Bl6** and **CD1** mice can be downloaded from [our repository](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/tree/master/models).
 
 ##### Basic usage:
 
 The main module with which you'll interact is called ```deepof.data```. Let's import it and create a project:
 
 ```python
-   import deepof.data
-   my_deepof_project = deepof.data.Project(
-      project_path=".", # Path where to create project files
-      video_path="/path/to/videos", # Path to DLC tracked videos
-      table_path="/path/to/tables", # Path to DLC output
-      project_name="my_deepof_project", # Name of the current project
-      exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
-    )
+import deepof.data
+my_deepof_project = deepof.data.Project(
+  project_path=".", # Path where to create project files
+  video_path="/path/to/videos", # Path to DLC tracked videos
+  table_path="/path/to/tables", # Path to DLC output
+  project_name="my_deepof_project", # Name of the current project
+  exp_conditions={exp_ID: exp_condition} # Dictionary containing one or more experimental conditions per provided video
+)
 ```
 
 This command will create a ```deepof.data.Project``` object storing all the necessary information to start. There are
 many parameters that we can set here, but let's stick to the basics for now.
 
 One you have this, you can run you project using the ```.create()``` method, which will do quite a lot of computing under
 the hood (load your data, smooth your trajectories, compute distances, angles, and areas between body parts, and save all
 results to disk). The returned object belongs to the ```deepof.data.Coordinates``` class.
 
 ```python
-   my_project = my_project.create(verbose=True)
+my_project = my_project.create(verbose=True)
 ```
 
 Once you have this, you can do several things! But let's first explore how the results of those computations mentioned
 are stored. To extract trajectories, distances, angles and/or areas, you can respectively type:
 
 ```python
-   my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
-   my_project_dists  = my_project.get_distances(speed=0)
-   my_project_angles = my_project.get_angles(speed=0)
-   my_project_areas = my_project.get_areas(speed=0)
+my_project_coords = my_project.get_coords(center="Center", polar=False, align="Nose", speed=0)
+my_project_dists  = my_project.get_distances(speed=0)
+my_project_angles = my_project.get_angles(speed=0)
+my_project_areas = my_project.get_areas(speed=0)
 ```
 
 Here, the data are stored as ```deepof.data.table_dict``` instances. These are very similar to python dictionaries
 with experiment IDs as keys and pandas.DataFrame objects as values, with a few extra methods for convenience. Peeping
 into the parameters you see in the code block above, ```center``` centers your data (it can be either a boolean or
 one of the body parts in your model! in which case the coordinate origin will be fixed to the position of that point);
 ```polar``` makes the ```.get_coords()``` method return polar instead of Cartesian coordinates, and ```speed```
@@ -113,23 +106,33 @@
 with our unsupervised methods.
 
 As mentioned above, the two main analyses that you can run are supervised and unsupervised. They are executed by
 the ```.supervised_annotation()``` method, and the ```.deep_unsupervised_embedding()``` methods of the ```deepof.data.Coordinates```
 class, respectively.
 
 ```python
-   supervised_annot = my_project.supervised_annotation()
-   gmvae_embedding  = my_project.deep_unsupervised_embedding()
+supervised_annot = my_project.supervised_annotation()
+gmvae_embedding  = my_project.deep_unsupervised_embedding()
 ```
 
 The former returns a ```deepof.data.TableDict``` object, with a pandas.DataFrame per experiment containing a series of
 annotations. The latter is a bit more complicated: it returns a series of objects that depend on the model selected (we 
 offer three flavours of deep clustering models), and allow for further analysis comparing cluster expression and dynamics.
 
-That's it for this (very basic) introduction. Check out the tutorials [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+That's it for this (very basic) introduction. Check out the tutorials and [full documentation](https://deepof.readthedocs.io/en/latest/index.html) for details!
+
+---
+### Issues
+
+If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
+
+---
+### Contributions
+
+We welcome contributions from the community! If you want to contribute to this project, please check out our [contribution guidelines](https://github.com/mlfpm/deepof/blob/master/CONTRIBUTING.md).
 
 ---
 
  This project has received funding from the European Union's Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No.  813533
  <div align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/255px-Flag_of_Europe.svg.png">
 </div>
```

