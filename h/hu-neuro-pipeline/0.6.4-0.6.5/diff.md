# Comparing `tmp/hu-neuro-pipeline-0.6.4.tar.gz` & `tmp/hu-neuro-pipeline-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hu-neuro-pipeline-0.6.4.tar", last modified: Fri Jan 13 18:13:05 2023, max compression
+gzip compressed data, was "hu-neuro-pipeline-0.6.5.tar", last modified: Sat May 20 06:48:11 2023, max compression
```

## Comparing `hu-neuro-pipeline-0.6.4.tar` & `hu-neuro-pipeline-0.6.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.785810 hu-neuro-pipeline-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/.github/workflows/build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/docs/flowchart.odp
--rw-r--r--   0 runner    (1001) docker     (123)    31242 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/docs/inputs.md
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/docs/outputs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-13 18:13:05.000000 hu-neuro-pipeline-0.6.4/pipeline/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/averaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:13:05.781810 hu-neuro-pipeline-0.6.4/pipeline/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/datasets/ucap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/epoching.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/perm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pipeline/tfr.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 18:13:05.785810 hu-neuro-pipeline-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-13 18:12:56.000000 hu-neuro-pipeline-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.github/workflows/build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/flowchart.odp
+-rw-r--r--   0 runner    (1001) docker     (123)    30937 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/inputs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/outputs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/pipeline/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/pipeline/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/datasets/ucap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/setup.py
```

### Comparing `hu-neuro-pipeline-0.6.4/.github/workflows/build_publish.yml` & `hu-neuro-pipeline-0.6.5/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/LICENSE` & `hu-neuro-pipeline-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/PKG-INFO` & `hu-neuro-pipeline-0.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.4
-Summary: Single trial EEG pipeline at the Neurocognitive Psychology Lab, Humboldt-Universität zu Berlin
+Version: 0.6.5
+Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 
 # hu-neuro-pipeline
 
 ![PyPI](https://img.shields.io/pypi/v/hu-neuro-pipeline)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hu-neuro-pipeline)
 ![GitHub](https://img.shields.io/github/license/alexenge/hu-neuro-pipeline)
 
-Single trial EEG pipeline at the [Neurocognitive Psychology lab](https://www.psychology.hu-berlin.de/en/profship/nk), Humboldt-Universität zu Berlin
+Single trial EEG pipeline at the [Abdel Rahman Lab for Neurocognitive Psychology](https://abdelrahmanlab.com), Humboldt-Universität zu Berlin
 
 Based on Frömer, R., Maier, M., & Abdel Rahman, R. (2018).
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
@@ -33,27 +33,39 @@
 
 Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```bash
 python3 -m pip install hu-neuro-pipeline
 ```
 
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```bash
+python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+```
+
 ### 1.2 For R users
 
 First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
 
 ```r
 install.packages("reticulate")
 reticulate::install_miniconda()
 ```
 
 Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE, python_version = "3.8")
+reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 [Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
 
 <img src="https://i.imgur.com/WSj9t4b.png" width="400">
@@ -75,15 +87,16 @@
     triggers=[201, 202, 211, 212],
     skip_log_conditions={'semantics': 'filler'},
     components={'name': ['N400', 'P600'],
                 'tmin': [0.3, 0.5],
                 'tmax': [0.5, 0.9],
                 'roi': [['C1', 'Cz', 'C2', 'CP1', 'CPz', 'CP2'],
                         ['Fz', 'FC1', 'FC2', 'C1', 'Cz', 'C2']]},
-    average_by=['semantics', 'context', 'semantics/context'])
+    average_by={'related': 'semantics == "related"',
+                'unrelated': 'semantics == "unrelated"'})
 ```
 
 In this example we have specified:
 
 * The paths to the raw EEG data, to the behavioral log files, to the desired output directory, and to the BESA files for ocular correction
 
 * Four different EEG `triggers` corresponding to each of the four cells in the 2 × 2 design
@@ -115,15 +128,18 @@
         "tmin" = list(0.3, 0.5),
         "tmax" = list(0.5, 0.9),
         "roi" = list(
             c("C1", "Cz", "C2", "CP1", "CPz", "CP2"),
             c("Fz", "FC1", "FC2", "C1", "Cz", "C2")
         )
     ),
-    average_by = c("semantics", "context", "semantics/context")
+    average_by = list(
+        related = "semantics == 'related'",
+        unrelated = "semantics == 'unrelated'"
+    )
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
```

### Comparing `hu-neuro-pipeline-0.6.4/README.md` & `hu-neuro-pipeline-0.6.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hu-neuro-pipeline
 
 ![PyPI](https://img.shields.io/pypi/v/hu-neuro-pipeline)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hu-neuro-pipeline)
 ![GitHub](https://img.shields.io/github/license/alexenge/hu-neuro-pipeline)
 
-Single trial EEG pipeline at the [Neurocognitive Psychology lab](https://www.psychology.hu-berlin.de/en/profship/nk), Humboldt-Universität zu Berlin
+Single trial EEG pipeline at the [Abdel Rahman Lab for Neurocognitive Psychology](https://abdelrahmanlab.com), Humboldt-Universität zu Berlin
 
 Based on Frömer, R., Maier, M., & Abdel Rahman, R. (2018).
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
@@ -16,27 +16,39 @@
 
 Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```bash
 python3 -m pip install hu-neuro-pipeline
 ```
 
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```bash
+python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+```
+
 ### 1.2 For R users
 
 First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
 
 ```r
 install.packages("reticulate")
 reticulate::install_miniconda()
 ```
 
 Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE, python_version = "3.8")
+reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 [Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
 
 <img src="https://i.imgur.com/WSj9t4b.png" width="400">
@@ -58,15 +70,16 @@
     triggers=[201, 202, 211, 212],
     skip_log_conditions={'semantics': 'filler'},
     components={'name': ['N400', 'P600'],
                 'tmin': [0.3, 0.5],
                 'tmax': [0.5, 0.9],
                 'roi': [['C1', 'Cz', 'C2', 'CP1', 'CPz', 'CP2'],
                         ['Fz', 'FC1', 'FC2', 'C1', 'Cz', 'C2']]},
-    average_by=['semantics', 'context', 'semantics/context'])
+    average_by={'related': 'semantics == "related"',
+                'unrelated': 'semantics == "unrelated"'})
 ```
 
 In this example we have specified:
 
 * The paths to the raw EEG data, to the behavioral log files, to the desired output directory, and to the BESA files for ocular correction
 
 * Four different EEG `triggers` corresponding to each of the four cells in the 2 × 2 design
@@ -98,15 +111,18 @@
         "tmin" = list(0.3, 0.5),
         "tmax" = list(0.5, 0.9),
         "roi" = list(
             c("C1", "Cz", "C2", "CP1", "CPz", "CP2"),
             c("Fz", "FC1", "FC2", "C1", "Cz", "C2")
         )
     ),
-    average_by = c("semantics", "context", "semantics/context")
+    average_by = list(
+        related = "semantics == 'related'",
+        unrelated = "semantics == 'unrelated'"
+    )
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
```

### Comparing `hu-neuro-pipeline-0.6.4/docs/flowchart.odp` & `hu-neuro-pipeline-0.6.5/docs/flowchart.odp`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/docs/inputs.md` & `hu-neuro-pipeline-0.6.5/docs/inputs.md`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 | `['Results/EEG/cali/Vp01.matrix', ...]` | `c("Results/EEG/cali/Vp01.matrix", ...)` |
 | `'Results/EEG/cali'`                    | `"Results/EEG/cali"`                     |
 
 ### **`ica_method` (optional, default: `None`)**
 
 Method for Indepedent Component Analysis (ICA) to correct for eye movement artifacts.
 For valid methods, see [`mne.preprocessing.ICA`](https://mne.tools/stable/generated/mne.preprocessing.ICA.html).
-If set, an ICA decomposition will be performed on the low-pass filtered data and any ICA components that correlate substantially with VEOG and/or HEOG will be removed in a fully automatic fashion.
+If set, an ICA decomposition will be performed on a high-pass filtered copy of the data (cutoff = 1.0 Hz) and any ICA components that correlate substantially with VEOG and/or HEOG will be removed in a fully automatic fashion.
 If `None`, no ocular correction using ICA will be performed.
 
 | Python examples | R examples  |
 | --------------- | ----------- |
 | `None`          | `NULL`      |
 | `'fastica'`     | `"fastica"` |
 | `'infomax'`     | `"infomax"` |
@@ -348,27 +348,24 @@
 | ----------------------------------------------------------------------------------------------------------------------------------- |
 | `list("name" = list("P1", "N170"), "tmin" = list(0.08, 0.15), "tmax" = list(0.13, 0.2), "roi" = list(c("PO3", ...), c("P7", ...)))` |
 
 ## 5. Averaging options
 
 ### **`average_by` (recommended, default: `None`)**
 
-Column names from the log file for averaging.
-Can be a single column name, in which case by-participant condition averages (a.k.a. "evokeds") will be computed for each condition in this column.
-The resulting evokeds are useful for plotting and for running permutation tests (see the `perm_*` arguments below).
-If a list of column names, evokeds will be computed for each condition in each of these column (i.e., for all main effects).
-Interaction effects can be added by combining two or more column names with a `/` character.
-If `None`, do not use columns in the log file for averaging and use the `triggers` instead.
-
-| Python examples                                 | R examples                                       |
-| ----------------------------------------------- | ------------------------------------------------ |
-| `None`                                          | `NULL`                                           |
-| `'semantics'`                                   | `"semantics"`                                    |
-| `['semantics', 'context']`                      | `c("semantics", "context")`                      |
-| `['semantics', 'context', 'semantics/context']` | `c("semantics", "context", "semantics/context")` |
+(Combinations of) conditions to create per-participant averages for.
+These per-participant condition averages (a.k.a. ["evokeds"](https://mne.tools/stable/auto_tutorials/evoked/10_evoked_overview.html)) are useful for plotting and for running permutation tests (see the `perm_*` arguments below).
+Must be a dict where each key is a custom condition label of your choice and each value is a string expression that will be used to select the relevant trials for this condition based on columns in the log file (see examples below and the [pandas documentation on querying](https://pandas.pydata.org/docs/user_guide/indexing.html#indexing-query)).
+If `None`, the pipeline will not create any custom averages but will instead create averages for each value in `triggers`.
+
+| Python examples                                                                      | R examples                                                                              |
+| ------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
+| `None`                                                                               | `NULL`                                                                                  |
+| `{'related': 'semantics == "related"', 'unrelated': 'semantics == "unrelated"}`      | `list(related = "semantics == 'related'", unrelated = "semantics == 'unrelated'")`      |
+| `{'neg_unrel': 'context == "negative" & semantics == "unrelated" & rt < 3000', ...}` | `list(neg_unrel = "context == 'negative' & semantics == 'unrelated' & rt < 3000", ...)` |
 
 ## 6. Options for time-frequency analysis
 
 ### **`perform_tfr` (optional, default: `False`)**
 
 Whether or not to perform time-frequency analysis in addition to ERPs.
 
@@ -377,25 +374,22 @@
 | `False`         | `FALSE`    |
 | `True`          | `TRUE`     |
 
 ### **`tfr_subtract_evoked` (optional, default: `False`)**
 
 Whether or not to subtract evoked activity from epochs before computing the time-frequency representation.
 If `False`, the resulting spectral power will not just reflect induced activity but also evoked activity from the ERP.
-If `True`, the average ERP *across all epochs* is removed before computing spectral power.
-If a string, the average ERP *per condition* is removed before computing spectral power.
-This string can either be a single column name or a combination of column names seperated by `/`.
-The same string must also be present in `average_by`.
-
-| Python examples       | R examples            |
-| --------------------- | --------------------- |
-| `False`               | `FALSE`               |
-| `True`                | `TRUE`                |
-| `'semantics'`         | `"semantics"`         |
-| `'semantics/context'` | `"semantics/context"` |
+If `True`, the average ERP is removed before computing spectral power.
+The average ERP is computed separately for each condition in `average_by`.
+If `average_by` is `None`, the average ERP is computed across all epochs.
+
+| Python examples | R examples |
+| --------------- | ---------- |
+| `False`         | `FALSE`    |
+| `True`          | `TRUE`     |
 
 ### **`tfr_freqs` (optional, default: `np.linspace(4.0, 40.0, num=37)`)**
 
 The frequencies for the family of [Morlet wavelets](https://neuroimage.usc.edu/brainstorm/Tutorials/TimeFrequency#Morlet_wavelets).
 A larger number of frequencies will create smoother plots at the expense of taking longer to compute and needing more disk space.
 Note that the time-frequency representation is computed on the *unfiltered* epochs so that frequencies larger than `lowpass_freq` are possible.
 
@@ -464,22 +458,20 @@
 
 ## 7. Options for cluster-based permutation tests
 
 ### **`perm_contrasts` (optional, default: `None`)**
 
 Contrasts between conditions to test using cluster-based permutation tests (CBPTs).
 Must be one or multiple tuples, each containing exactly two condition labels.
-Each of these labels must be corresponding to one condition which can be found in one of the `condition_cols` (see above).
-Single condition labels can be used to test main effects (e.g., semantically related vs. unrelated) and multiple hierarchical labels (seperated by `'/'`) can be used to test nested effects (e.g., semantically related vs. unrelated *within* the emotionally negative context).
-In this case, the order of the levels must correspond to the order of the column names in `condition_cols`.
-
-| Python examples                                  | R examples                                             |
-| ------------------------------------------------ | ------------------------------------------------------ |
-| `[('related', 'unrelated')]`                     | `list(c("related", "unrelated"))`                      |
-| `[('related/negative'), ('unrelated/negative')]` | `list(c("related/negative"), c("unrelated/negative"))` |
+Each condition label must correspond to one of the dictionary keys specified in `average_by` or, if `average_by=None`, to one of the EEG triggers specified in `triggers`.
+
+| Python examples                | R examples                           |
+| ------------------------------ | ------------------------------------ |
+| `[('related', 'unrelated')]`   | `list(c("related", "unrelated"))`    |
+| `[('neg_unrel'), ('neg_rel')]` | `list(c("neg_unrel"), c("neg_rel"))` |
 
 ### **`perm_tmin` (optional, default: `0.`)**
 
 The starting time point (in s relative to stimulus onset) of the time window to consider for permutation testing.
 If `None`, all time points from the beginning of the epoch (including the prestimulus intervall) are used.
 Cropping the time window (based on *a priori* knowledge about plausible effects) can increase the sensitivity of the test.
```

### Comparing `hu-neuro-pipeline-0.6.4/docs/outputs.md` & `hu-neuro-pipeline-0.6.5/docs/outputs.md`

 * *Files 14% similar despite different names*

```diff
@@ -37,38 +37,55 @@
 +   N400 ~ semantics + (semantics | participant_id) + (semantics | item_id),
 +   data = trials
 + )
 ```
 
 ### **`evokeds` (file: `output_dir/ave.csv`)**
 
-This data frame contains the by-participant averaged ERPs at each time point, at each channel, and for each experimental condition (or combination of conditions) as specified via the `average_by` option.
+This data frame contains the per-participant and averaged ERPs at each time point, at each channel, and for each experimental condition (or combination of conditions) as specified via the `average_by` option.
 
 ```r
 > evokeds <- res[[2]]
 > head(evokeds)     
-  participant_id average_by semantics   time    Fp1    Fpz    Fp2 ...
-1         Vp0001  semantics   related -0.500 0.5549 0.9599 1.3789 ...
-2         Vp0001  semantics   related -0.496 0.4824 0.7980 1.2616 ...
-3         Vp0001  semantics   related -0.492 0.5179 0.6926 1.1960 ...
-4         Vp0001  semantics   related -0.488 0.5798 0.6537 1.1883 ...
-5         Vp0001  semantics   related -0.484 0.5479 0.6327 1.1621 ...
-6         Vp0001  semantics   related -0.480 0.3763 0.5591 1.0230 ...
+  participant_id   label                  query   time    Fp1    Fpz    Fp2 ...
+1         Vp0001 related semantics == "related" -0.500 0.5549 0.9599 1.3789 ...
+2         Vp0001 related semantics == "related" -0.496 0.4824 0.7980 1.2616 ...
+3         Vp0001 related semantics == "related" -0.492 0.5179 0.6926 1.1960 ...
+4         Vp0001 related semantics == "related" -0.488 0.5798 0.6537 1.1883 ...
+5         Vp0001 related semantics == "related" -0.484 0.5479 0.6327 1.1621 ...
+6         Vp0001 related semantics == "related" -0.480 0.3763 0.5591 1.0230 ...
 ```
 
-This data frame can be used, for instance, to plot the time course of the different semantic conditions as grand averages (together with their standard errors across participants):
+This data frame can be used, for instance, to plot the time course of the different semantic conditions as grand averages:
 
 ```r
 > library(dplyr)
 > library(ggplot2)
 > evokeds %>%
-+    filter(average_by == "semantics") %>%
-+    ggplot(aes(x = time, y = N400, color = semantics) +
-+    stat_summary(geom = "linerange", fun.data = mean_se, alpha = 0.1) +
-+    stat_summary(geom = "line", fun = mean)    
++   filter(label %in% c("related", "unrelated")) %>%
++   ggplot(aes(x = time, y = N400, color = label)) +
++   stat_summary(geom = "line", fun = mean)    
+```
+
+To add [within-participant standard errors](http://www.cookbook-r.com/Graphs/Plotting_means_and_error_bars_(ggplot2)/#error-bars-for-within-subjects-variables) as shaded regions around the waveforms:
+
+```r
+> evokeds %>%
++   Rmisc::summarySEwithin(
++     measurevar = "N400",
++     withinvars = c("label", "time"),
++     idvar = "participant_id"
++   ) %>%
++   mutate(time = as.numeric(as.character(time))) %>%
++   ggplot(aes(x = time, y = N400)) +
++   geom_ribbon(
++     aes(ymin = N400 - se, ymax = N400 + se, fill = label),
++     alpha = 0.2
++   ) +
++   geom_line(aes(color = label))
 ```
 
 ### **`config` (file: `output_dir/config.json`)**
 
 This file contains a dictionary-like representation of the input options that were used by the pipeline.
 It also lists rejected epochs per participant as well as automatically detected bad channels and ICA components (if applicable).
```

### Comparing `hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/PKG-INFO` & `hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.4
-Summary: Single trial EEG pipeline at the Neurocognitive Psychology Lab, Humboldt-Universität zu Berlin
+Version: 0.6.5
+Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 
 # hu-neuro-pipeline
 
 ![PyPI](https://img.shields.io/pypi/v/hu-neuro-pipeline)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hu-neuro-pipeline)
 ![GitHub](https://img.shields.io/github/license/alexenge/hu-neuro-pipeline)
 
-Single trial EEG pipeline at the [Neurocognitive Psychology lab](https://www.psychology.hu-berlin.de/en/profship/nk), Humboldt-Universität zu Berlin
+Single trial EEG pipeline at the [Abdel Rahman Lab for Neurocognitive Psychology](https://abdelrahmanlab.com), Humboldt-Universität zu Berlin
 
 Based on Frömer, R., Maier, M., & Abdel Rahman, R. (2018).
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
@@ -33,27 +33,39 @@
 
 Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```bash
 python3 -m pip install hu-neuro-pipeline
 ```
 
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```bash
+python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+```
+
 ### 1.2 For R users
 
 First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
 
 ```r
 install.packages("reticulate")
 reticulate::install_miniconda()
 ```
 
 Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE, python_version = "3.8")
+reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 [Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
 
 <img src="https://i.imgur.com/WSj9t4b.png" width="400">
@@ -75,15 +87,16 @@
     triggers=[201, 202, 211, 212],
     skip_log_conditions={'semantics': 'filler'},
     components={'name': ['N400', 'P600'],
                 'tmin': [0.3, 0.5],
                 'tmax': [0.5, 0.9],
                 'roi': [['C1', 'Cz', 'C2', 'CP1', 'CPz', 'CP2'],
                         ['Fz', 'FC1', 'FC2', 'C1', 'Cz', 'C2']]},
-    average_by=['semantics', 'context', 'semantics/context'])
+    average_by={'related': 'semantics == "related"',
+                'unrelated': 'semantics == "unrelated"'})
 ```
 
 In this example we have specified:
 
 * The paths to the raw EEG data, to the behavioral log files, to the desired output directory, and to the BESA files for ocular correction
 
 * Four different EEG `triggers` corresponding to each of the four cells in the 2 × 2 design
@@ -115,15 +128,18 @@
         "tmin" = list(0.3, 0.5),
         "tmax" = list(0.5, 0.9),
         "roi" = list(
             c("C1", "Cz", "C2", "CP1", "CPz", "CP2"),
             c("Fz", "FC1", "FC2", "C1", "Cz", "C2")
         )
     ),
-    average_by = c("semantics", "context", "semantics/context")
+    average_by = list(
+        related = "semantics == 'related'",
+        unrelated = "semantics == 'unrelated'"
+    )
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
```

### Comparing `hu-neuro-pipeline-0.6.4/hu_neuro_pipeline.egg-info/SOURCES.txt` & `hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/averaging.py` & `hu-neuro-pipeline-0.6.5/pipeline/averaging.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+import warnings
+
 import numpy as np
 import pandas as pd
 from mne import Epochs, Evoked, grand_average
+from mne.time_frequency import AverageTFR, EpochsTFR
 
 
 def compute_evokeds(epochs, average_by=None, bad_ixs=[], participant_id=None):
     """Computes condition averages (evokeds) based on triggers or columns."""
 
     # Average by triggers in case no log file columns were provided
     if average_by is None:
         all_evokeds, all_evokeds_df = compute_evokeds_triggers(
             epochs, bad_ixs, participant_id)
+    elif isinstance(average_by, dict):
+        all_evokeds, all_evokeds_df = compute_evokeds_queries(
+            epochs, average_by, bad_ixs, participant_id)
     else:
+        warnings.warn(
+            'Passing a list of column names to `average_by` will ' +
+            'be deprecated in a future version of the pipeline. ' +
+            'Please use a dict of  labels and log file queries ' +
+            'instead (see https://github.com/alexenge/hu-neuro-pipeline/blob/main/docs/inputs.md#average_by-recommended-default-none)')
         all_evokeds, all_evokeds_df = compute_evokeds_cols(
             epochs, average_by, bad_ixs, participant_id)
 
     return all_evokeds, all_evokeds_df
 
 
 def compute_evokeds_triggers(epochs, bad_ixs=[], participant_id=None):
@@ -38,14 +49,74 @@
 
     # Combine DataFrames
     all_evokeds_df = pd.concat(all_evokeds_dfs, ignore_index=True)
 
     return all_evokeds, all_evokeds_df
 
 
+def compute_evokeds_queries(epochs, queries, bad_ixs=[], participant_id=None):
+    """Computes condition averages (evokeds) based on log file queries."""
+
+    # Get indices of good epochs
+    good_ixs = [ix for ix in range(len(epochs)) if ix not in bad_ixs]
+
+    # Reset index so that trials start at 0
+    epochs.metadata.reset_index(drop=True, inplace=True)
+
+    # Create evokeds for each query
+    evokeds = []
+    evoked_dfs = []
+    for label, query in queries.items():
+
+        # Compute evokeds for trials that match the current query
+        evoked = compute_evoked_query(epochs[good_ixs], query, label)
+        evokeds.append(evoked)
+
+        # Convert to data frame
+        extra_cols = \
+            {'participant_id': participant_id, 'label': label, 'query': query}
+        evoked_df = evoked_to_df(evoked, extra_cols)
+        evoked_dfs.append(evoked_df)
+
+    # Combine data frames
+    evokeds_df = pd.concat(evoked_dfs, ignore_index=True)
+
+    return evokeds, evokeds_df
+
+
+def compute_evoked_query(epochs, query, label):
+    """Computes one condition average (evoked) based on a log file query."""
+
+    # Compute evokeds based on ERP or TFR epochs
+    if isinstance(epochs, EpochsTFR):
+        evoked = epochs[query].average()
+    else:  # `EpochsTFR.average()` has no `picks` argument
+        evoked = epochs[query].average(picks=['eeg', 'misc'])
+    evoked.comment = label
+
+    return evoked
+
+
+def evoked_to_df(evoked, extra_cols={}):
+    """Converts MNE's Evoked or AverageTFR to a pandas data frame."""
+
+    # Convert to data frame
+    if isinstance(evoked, AverageTFR):
+        evoked_df = evoked.to_data_frame()
+    else:  # `AverageTFR.to_data_frame()` has no `scalings` argument
+        evoked_df = \
+            evoked.to_data_frame(scalings={'eeg': 1e6, 'misc': 1e6})
+
+    # Optionally add extra columns
+    for column, value in reversed(extra_cols.items()):
+        evoked_df.insert(0, column, value)
+
+    return evoked_df
+
+
 def compute_evokeds_cols(
         epochs, average_by=None, bad_ixs=[], participant_id=None):
     """Computes condition averages (evokeds) based on log file columns."""
 
     # Make sure that provided values are stored in a list
     if isinstance(average_by, str):
         average_by = [average_by]
```

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/boilerplate.py` & `hu-neuro-pipeline-0.6.5/pipeline/boilerplate.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/datasets/ucap.py` & `hu-neuro-pipeline-0.6.5/pipeline/datasets/ucap.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/epoching.py` & `hu-neuro-pipeline-0.6.5/pipeline/epoching.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     if isinstance(triggers, list):
         triggers = {str(trigger): trigger for trigger in triggers}
     else:
         assert isinstance(triggers, dict), \
             '`triggers` must be either list or dict'
 
     # Make sure that trigger values are integers (R would pass them as floats)
-    triggers = {key: int(value) for key, value in triggers.items()}
-    event_id = triggers
+    event_id = {key: int(value) for key, value in triggers.items()}
 
     return event_id
 
 
 def read_log(log_file, skip_log_rows=None, skip_log_conditions=None):
     """Reads the behavioral log file with information about each EEG trial."""
 
@@ -83,15 +82,15 @@
         # ... or if the log and EEG trigers don't match up
         elif events_log[ix] != events_epochs[ix]:
             print(f'Log file (row index {ix}): Found missing EEG epoch')
             events_epochs.insert(ix, np.nan)
             previous_repaired = True
 
         # If they do match up, we check that the next trials do match as well
-        elif previous_repaired: 
+        elif previous_repaired:
             if events_log[ix:ix + depth] != events_epochs[ix:ix + depth]:
                 print(f'Log file (row index {ix}): Assuming missing EEG epoch')
                 events_epochs.insert(ix, np.nan)
             else:
                 previous_repaired = False
 
     # Remove trials with missing EEG epochs from the log file
@@ -123,15 +122,15 @@
 def get_bad_channels(epochs, threshold=3., by_event_type=True):
     """Automatically detects bad channels using their average standard error"""
 
     # Compute standard error for each condition seperately, then average...
     if by_event_type:
         ses = epochs.standard_error(by_event_type=True)
         ses = combine_evoked(ses, weights='nave')
-    
+
     # ... or directly compute standard error across all epochs
     else:
         ses = epochs.standard_error()
 
     # Average across time points for each channel
     ses = ses.data.mean(axis=1)
```

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/group.py` & `hu-neuro-pipeline-0.6.5/pipeline/group.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/io.py` & `hu-neuro-pipeline-0.6.5/pipeline/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,21 +61,25 @@
     assert path.isdir(dir_path), f'Didn\'t find directory `{dir_path}`!'
     files = []
     for extension in extensions:
         files += glob(f'{dir_path}/*.{extension}')
 
     # Sort naturally because some files might not have leading zeros
     if natsort_files:
-        natsort = lambda s: [
-            int(t) if t.isdigit() else t.lower() for t in re.split('(\d+)', s)]
         files = sorted(files, key=natsort)
 
     return files
 
 
+def natsort(s):
+    """Natural-sort list of strings to handle (non-)leading zeros."""
+
+    return [int(t) if t.isdigit() else t.lower() for t in re.split('(\d+)', s)]
+
+
 def convert_participant_input(input, participant_ids):
     """Converts different inputs (e.g., dict) into a per-participant list."""
 
     # If it's a dict, convert to list
     if isinstance(input, dict):
         participant_dict = {id: None for id in participant_ids}
         for id, values in input.items():
@@ -145,14 +149,15 @@
     participant_id_ = '' if participant_id == '' else f'{participant_id}_'
     suffix = 'epo'
 
     # Convert to DataFrame
     if to_df is True or to_df == 'both':
         scalings = {'eeg': 1e6, 'misc': 1e6}
         epochs_df = epochs.to_data_frame(scalings=scalings, time_format=None)
+        epochs_df = epochs_df.rename(columns={'condition': 'event_id'})
 
         # Add metadata from log file
         metadata_df = epochs.metadata.copy()
         metadata_df = metadata_df.drop([col for col in metadata_df.columns
                                         if col in epochs_df.columns], axis=1)
         n_samples = len(epochs.times)
         metadata_df = metadata_df.loc[metadata_df.index.repeat(n_samples)]
@@ -244,13 +249,13 @@
     print(f'Saving HTML report to {fname}')
     _ = report.save(fname, open_browser=False, overwrite=True)
 
 
 def package_versions():
     """Returns pipeline version and important dependency package versions."""
 
-    return({'python': python_version(),
-            'pipeline': pipeline_version,
-            'mne': mne_version,
-            'numpy': numpy_version,
-            'pandas': pandas_version,
-            'scikit-learn': sk_version})
+    return ({'python': python_version(),
+             'pipeline': pipeline_version,
+             'mne': mne_version,
+             'numpy': numpy_version,
+             'pandas': pandas_version,
+             'scikit-learn': sk_version})
```

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/participant.py` & `hu-neuro-pipeline-0.6.5/pipeline/participant.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,16 +161,18 @@
     if triggers_column is not None:
         log, missing_ixs = match_log_to_epochs(epochs, log, triggers_column)
         config['auto_missing_epochs'] = missing_ixs
     epochs.metadata = log
     epochs.metadata.insert(0, column='participant_id', value=participant_id)
 
     # If log file was provided as a DataFrame, convert to dict for config
-    if isinstance(config['log_file'], pd.DataFrame):
-        config['log_file'] = config['log_file'].to_dict(orient='list')
+    if isinstance(log_file, pd.DataFrame):
+        log_file = log_file.astype(object)  # Convert NaNs to null for JSON
+        log_file = log_file.where(pd.notnull(log_file), None)
+        config['log_file'] = log_file.to_dict(orient='list')
 
     # Get indices of bad epochs
     bad_ixs = get_bad_epochs(epochs, reject_peak_to_peak)
     config['auto_rejected_epochs'] = bad_ixs
 
     # Compute single trial mean ERP amplitudes and add to metadata
     trials = compute_single_trials(epochs, components, bad_ixs)
@@ -215,18 +217,15 @@
 
         # Copy original metadata
         epochs_unfilt.metadata = epochs.metadata.copy()
 
         # Optionally subtract evoked activity
         # See, e.g., https://doi.org/10.1016/j.neuroimage.2006.02.034
         if tfr_subtract_evoked:
-            subtract_cols = None if tfr_subtract_evoked is True \
-                else tfr_subtract_evoked
-            epochs_unfilt = subtract_evoked(
-                epochs_unfilt, evokeds, cols=subtract_cols)
+            epochs_unfilt = subtract_evoked(epochs_unfilt, average_by, evokeds)
 
         # Morlet wavelet convolution
         print('Doing time-frequency transform with Morlet wavelets')
         tfr = tfr_morlet(epochs_unfilt, tfr_freqs, tfr_cycles, use_fft=True,
                          return_itc=False, n_jobs=1, average=False)
 
         # First, divisive baseline correction using the full epoch
```

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/perm.py` & `hu-neuro-pipeline-0.6.5/pipeline/perm.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/preprocessing.py` & `hu-neuro-pipeline-0.6.5/pipeline/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/report.py` & `hu-neuro-pipeline-0.6.5/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.4/pipeline/tfr.py` & `hu-neuro-pipeline-0.6.5/pipeline/tfr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 import numpy as np
 import pandas as pd
 from mne import concatenate_epochs, set_log_level
 
 
-def subtract_evoked(epochs, evokeds=None, cols=None):
+def subtract_evoked(epochs, average_by=None, evokeds=None):
     """Subtracts evoked activity (across or by conditions) from epochs."""
 
     # If no columns were requested, subtract evoked activity across conditions
     set_log_level('ERROR')
-    if cols is None:
+    if average_by is None:
         print('Subtracting evoked activity')
         epochs = epochs.subtract_evoked()
-    
+
     # Otherwise subtract seperately for all (combinations of) conditions
     else:
-        print(f'Subtracting evoked activity per condition in \'{cols}\'')
-        epochs = subtract_evoked_cols(epochs, evokeds, cols)
+        print('Subtracting evoked activity per condition in `average_by`')
+        epochs = subtract_evoked_conditions(epochs, average_by, evokeds)
     set_log_level('INFO')
-    
+
     return epochs
 
 
-def subtract_evoked_cols(epochs, evokeds, cols):
+def subtract_evoked_conditions(epochs, average_by, evokeds):
     """Subtracts evoked activity (separately by conditions) from epochs."""
 
-    # Combine relevant columns
-    cols = cols.split('/')
-    cols_df = pd.DataFrame(epochs.metadata[cols])
-    cols_df = cols_df.astype('str')
-    ids = cols_df.agg('/'.join, axis=1).reset_index(drop=True)
-
-    # Loop over epochs
+    # Loop over epochs (painfully slow)
     epochs_subtracted = []
-    for ix, id in enumerate(ids):
+    for ix, _ in enumerate(epochs):
+        for query, evoked in zip(average_by.values(), evokeds):
+            if len(epochs[ix][query]) > 0:
+                epoch_subtracted = epochs[ix].subtract_evoked(evoked)
+                epochs_subtracted.append(epoch_subtracted)
 
-        # Subtract the relevant evoked from each epoch
-        evoked_id = [ev for ev in evokeds if ev.comment == id][0]
-        epoch_subtracted = epochs[ix].subtract_evoked(evoked_id)
-        epochs_subtracted.append(epoch_subtracted)
-    
-    # Combine list of subtracted epochs
-    epochs_subtracted = concatenate_epochs(epochs_subtracted)
-    
-    return epochs_subtracted
+    return concatenate_epochs(epochs_subtracted)
 
 
 def compute_single_trials_tfr(epochs, components, bad_ixs=None):
     """Computes single trial power for a dict of multiple components."""
 
     # Check that values in the dict are lists
     if not isinstance(components['name'], list):
```

### Comparing `hu-neuro-pipeline-0.6.4/setup.py` & `hu-neuro-pipeline-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         long_description = fh.read()
 
     # Actual setup
     setuptools.setup(
         name='hu-neuro-pipeline',
         author='Alexander Enge',
         author_email='alexander.enge@hu-berlin.de',
-        description='Single trial EEG pipeline at the Neurocognitive '
-                    'Psychology Lab, Humboldt-Universität zu Berlin',
+        description='Single trial EEG pipeline at the Abdel Rahman Lab for '
+                    'Neurocognitive Psychology, Humboldt-Universität zu Berlin',
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/alexenge/hu-neuro-pipeline',
         project_urls={
             'Issue trackers': 'https://github.com/alexenge/hu-neuro-pipeline/issues',
         },
         classifiers=[
```

