# Comparing `tmp/faster-coco-eval-1.3.1.tar.gz` & `tmp/faster-coco-eval-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-coco-eval-1.3.1.tar", last modified: Wed Mar  1 17:07:02 2023, max compression
+gzip compressed data, was "faster-coco-eval-1.3.2.tar", last modified: Sat May 20 11:10:37 2023, max compression
```

## Comparing `faster-coco-eval-1.3.1.tar` & `faster-coco-eval-1.3.2.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4529 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3904 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/faster_eval_api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/faster_eval_api/coco_eval/
--rw-r--r--   0 root         (0) root         (0)    23799 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp
--rw-r--r--   0 root         (0) root         (0)     3871 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/faster_eval_api/coco_eval/cocoeval.h
--rw-r--r--   0 root         (0) root         (0)     1630 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/faster_eval_api/faster_eval_api.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/mask/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/mask/common/
--rw-r--r--   0 root         (0) root         (0)     8308 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/mask/common/maskApi.c
--rw-r--r--   0 root         (0) root         (0)     2176 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/mask/common/maskApi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/csrc/mask/pycocotools/
--rw-r--r--   0 root         (0) root         (0)   655761 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/mask/pycocotools/_mask.c
--rw-r--r--   0 root         (0) root         (0)    11440 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/csrc/mask/pycocotools/_mask.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.199636 faster-coco-eval-1.3.1/faster_coco_eval/
--rw-r--r--   0 root         (0) root         (0)      123 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/faster_coco_eval/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15024 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/core/coco.py
--rw-r--r--   0 root         (0) root         (0)    27022 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/core/cocoeval.py
--rw-r--r--   0 root         (0) root         (0)     5502 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/core/faster_eval_api.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/core/mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/faster_coco_eval/extra/
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/extra/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16344 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/extra/curves.py
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/faster_coco_eval/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4529 2023-03-01 17:07:02.000000 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      789 2023-03-01 17:07:02.000000 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 17:07:02.000000 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 17:07:02.000000 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-01 17:07:02.000000 faster-coco-eval-1.3.1/faster_coco_eval.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 17:07:02.209636 faster-coco-eval-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5800 2023-03-01 17:06:26.000000 faster-coco-eval-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4166 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.629842 faster-coco-eval-1.3.2/csrc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.649842 faster-coco-eval-1.3.2/csrc/faster_eval_api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.649842 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/
+-rw-r--r--   0 root         (0) root         (0)    25495 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.h
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/faster_eval_api.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.629842 faster-coco-eval-1.3.2/csrc/mask/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.669842 faster-coco-eval-1.3.2/csrc/mask/common/
+-rw-r--r--   0 root         (0) root         (0)     8308 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/common/maskApi.c
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/common/maskApi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.669842 faster-coco-eval-1.3.2/csrc/mask/pycocotools/
+-rw-r--r--   0 root         (0) root         (0)   655761 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.c
+-rw-r--r--   0 root         (0) root         (0)    11440 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.679842 faster-coco-eval-1.3.2/faster_coco_eval/
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.689842 faster-coco-eval-1.3.2/faster_coco_eval/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15122 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/coco.py
+-rw-r--r--   0 root         (0) root         (0)    25709 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/cocoeval.py
+-rw-r--r--   0 root         (0) root         (0)    12261 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/faster_eval_api.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/faster_coco_eval/extra/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/curves.py
+-rw-r--r--   0 root         (0) root         (0)     9288 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/display.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/extra.py
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.679842 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5851 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/setup.py
```

### Comparing `faster-coco-eval-1.3.1/LICENSE` & `faster-coco-eval-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/PKG-INFO` & `faster-coco-eval-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.3.1
+Version: 1.3.2
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
 # Faster-COCO-Eval
 
 ## Disclaimer
@@ -74,14 +75,23 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.2
+
+- [x] rework math_matches function. moved to faster_eval_api
+- [x] Moved calculations from python to c++
+- [x] Separated extra classes
+- [x] Added new sample data
+- [x] append mIoU based on TP pred.
+- [x] append mAUC based on Coco pre/rec.
+
 ### v1.3.1
 
 - [x] rework mask code
 - [x] change np.float to float ([numpy deprecations](https://numpy.org/devdocs/release/1.20.0-notes.html#deprecations))
 
 ### v1.3.0
```

### Comparing `faster-coco-eval-1.3.1/README.md` & `faster-coco-eval-1.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,23 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.2
+
+- [x] rework math_matches function. moved to faster_eval_api
+- [x] Moved calculations from python to c++
+- [x] Separated extra classes
+- [x] Added new sample data
+- [x] append mIoU based on TP pred.
+- [x] append mAUC based on Coco pre/rec.
+
 ### v1.3.1
 
 - [x] rework mask code
 - [x] change np.float to float ([numpy deprecations](https://numpy.org/devdocs/release/1.20.0-notes.html#deprecations))
 
 ### v1.3.0
```

### Comparing `faster-coco-eval-1.3.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp` & `faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,24 @@
         const std::array<double, 2> &area_range,
         ImageEvaluation *results)
     {
       // Initialize memory to store return data matches and ignore
       const int num_iou_thresholds = iou_thresholds.size();
       const int num_ground_truth = ground_truth_sorted_indices.size();
       const int num_detections = detection_sorted_indices.size();
-      std::vector<uint64_t> ground_truth_matches(
-          num_iou_thresholds * num_ground_truth, 0);
+      // std::vector<uint64_t> ground_truth_matches(
+      // num_iou_thresholds * num_ground_truth, 0);
+      std::vector<uint64_t> &ground_truth_matches = results->ground_truth_matches;
+      ground_truth_matches.resize(num_iou_thresholds * num_ground_truth, 0);
+
+      std::vector<int> &ground_truth_orig_id = results->ground_truth_orig_id;
+      ground_truth_orig_id.resize(num_iou_thresholds * num_ground_truth, -1);
+
       std::vector<uint64_t> &detection_matches = results->detection_matches;
+
       std::vector<bool> &detection_ignores = results->detection_ignores;
       std::vector<bool> &ground_truth_ignores = results->ground_truth_ignores;
       detection_matches.resize(num_iou_thresholds * num_detections, 0);
       detection_ignores.resize(num_iou_thresholds * num_detections, false);
       ground_truth_ignores.resize(num_ground_truth);
       for (auto g = 0; g < num_ground_truth; ++g)
       {
@@ -131,14 +138,15 @@
           if (match >= 0)
           {
             detection_ignores[t * num_detections + d] = ground_truth_ignores[match];
             detection_matches[t * num_detections + d] =
                 ground_truth_instances[ground_truth_sorted_indices[match]].id;
             ground_truth_matches[t * num_ground_truth + match] =
                 detection_instances[detection_sorted_indices[d]].id;
+            ground_truth_orig_id[t * num_ground_truth + match] = (int)ground_truth_instances[ground_truth_sorted_indices[match]].id;
           }
 
           // set unmatched detections outside of area range to ignore
           const InstanceAnnotation &detection =
               detection_instances[detection_sorted_indices[d]];
           detection_ignores[t * num_detections + d] =
               detection_ignores[t * num_detections + d] ||
@@ -532,23 +540,43 @@
       localtime_s(&local_time, &rawtime);
 #else
       localtime_r(&rawtime, &local_time);
 #endif
       strftime(
           buffer.data(), 200, "%Y-%m-%d %H:%num_max_detections:%S", &local_time);
 
+      int evaluations_size = static_cast<int>(evaluations.size());
+
+      std::vector<uint64_t> out_detection_matches = {};
+      std::vector<uint64_t> out_ground_truth_matches = {};
+      std::vector<uint64_t> out_detection_ignores = {};
+      std::vector<int> out_ground_truth_orig_id = {};
+      // auto eval = evaluations[0];
+      for (auto eval : evaluations)
+      {
+        out_detection_matches.insert(out_detection_matches.end(), eval.detection_matches.begin(), eval.detection_matches.end());
+        out_ground_truth_matches.insert(out_ground_truth_matches.end(), eval.ground_truth_matches.begin(), eval.ground_truth_matches.end());
+        out_detection_ignores.insert(out_detection_ignores.end(), eval.detection_ignores.begin(), eval.detection_ignores.end());
+        out_ground_truth_orig_id.insert(out_ground_truth_orig_id.end(), eval.ground_truth_orig_id.begin(), eval.ground_truth_orig_id.end());
+      }
+
       return py::dict(
           "params"_a = params,
           "counts"_a = std::vector<int64_t>({num_iou_thresholds,
                                              num_recall_thresholds,
                                              num_categories,
                                              num_area_ranges,
                                              num_max_detections}),
           "date"_a = buffer,
           "precision"_a = precisions_out,
           "recall"_a = recalls_out,
-          "scores"_a = scores_out);
+          "scores"_a = scores_out,
+          "detection_matches"_a = out_detection_matches,
+          "detection_ignores"_a = out_detection_ignores,
+          "ground_truth_matches"_a = out_ground_truth_matches,
+          "ground_truth_orig_id"_a = out_ground_truth_orig_id,
+          "evaluations_size"_a = evaluations_size);
     }
 
   } // namespace COCOeval
 
 } // namespace coco_eval
```

### Comparing `faster-coco-eval-1.3.1/csrc/faster_eval_api/coco_eval/cocoeval.h` & `faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.h`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     // matches between detected and ground truth instances
     struct ImageEvaluation
     {
       // For each of the D detected instances, the id of the matched ground truth
       // instance, or 0 if unmatched
       std::vector<uint64_t> detection_matches;
 
+      std::vector<uint64_t> ground_truth_matches;
+      std::vector<int> ground_truth_orig_id;
       // The detection score of each of the D detected instances
       std::vector<double> detection_scores;
 
       // Marks whether or not each of G instances was ignored from evaluation (e.g.,
       // because it's outside area_range)
       std::vector<bool> ground_truth_ignores;
```

### Comparing `faster-coco-eval-1.3.1/csrc/faster_eval_api/faster_eval_api.cpp` & `faster-coco-eval-1.3.2/csrc/faster_eval_api/faster_eval_api.cpp`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/csrc/mask/common/maskApi.c` & `faster-coco-eval-1.3.2/csrc/mask/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/csrc/mask/common/maskApi.h` & `faster-coco-eval-1.3.2/csrc/mask/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/csrc/mask/pycocotools/_mask.c` & `faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.c`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/csrc/mask/pycocotools/_mask.pyx` & `faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.pyx`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/faster_coco_eval/core/coco.py` & `faster-coco-eval-1.3.2/faster_coco_eval/core/coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,21 @@
     def createIndex(self):
         # create index
         logger.debug('creating index...')
         anns, cats, imgs = {}, {}, {}
         imgToAnns, catToImgs = defaultdict(list), defaultdict(list)
         if 'annotations' in self.dataset:
             for ann in self.dataset['annotations']:
+                ann['image_id'] = int(ann['image_id'])
                 imgToAnns[ann['image_id']].append(ann)
                 anns[ann['id']] = ann
 
         if 'images' in self.dataset:
             for img in self.dataset['images']:
+                img['id'] = int(img['id'])
                 imgs[img['id']] = img
 
         if 'categories' in self.dataset:
             for cat in self.dataset['categories']:
                 cats[cat['id']] = cat
 
         if 'annotations' in self.dataset and 'categories' in self.dataset:
```

### Comparing `faster-coco-eval-1.3.1/faster_coco_eval/core/cocoeval.py` & `faster-coco-eval-1.3.2/faster_coco_eval/core/cocoeval.py`

 * *Files 3% similar despite different names*

```diff
@@ -352,16 +352,14 @@
         A = len(p.areaRng)
         M = len(p.maxDets)
         # -1 for the precision of absent categories
         precision = -np.ones((T, R, K, A, M))
         recall = -np.ones((T, K, A, M))
         scores = -np.ones((T, R, K, A, M))
 
-        tp_rate = -np.ones((T, R, K, A, M))
-
         # create dictionary for future indexing
         _pe = self._paramsEval
         catIds = _pe.catIds if _pe.useCats else [-1]
         setK = set(catIds)
         setA = set(map(tuple, _pe.areaRng))
         setM = set(_pe.maxDets)
         setI = set(_pe.imgIds)
@@ -370,16 +368,14 @@
         m_list = [m for n, m in enumerate(p.maxDets) if m in setM]
         a_list = [n for n, a in enumerate(
             map(lambda x: tuple(x), p.areaRng)) if a in setA]
         i_list = [n for n, i in enumerate(p.imgIds) if i in setI]
         I0 = len(_pe.imgIds)
         A0 = len(_pe.areaRng)
 
-        _matches = []
-
         # retrieve E at each category, area range, and max number of detections
         for k, k0 in enumerate(k_list):
             Nk = k0*A0*I0
             for a, a0 in enumerate(a_list):
                 Na = a0*I0
                 for m, maxDet in enumerate(m_list):
                     E = [self.evalImgs[Nk + Na + i] for i in i_list]
@@ -403,23 +399,14 @@
                     npig = np.count_nonzero(gtIg == 0)
                     if npig == 0:
                         continue
                     tps = np.logical_and(dtm,  np.logical_not(dtIg))
                     fps = np.logical_and(
                         np.logical_not(dtm), np.logical_not(dtIg))
 
-                    # detected ann ids
-                    dtm_ids = np.concatenate(
-                        [e['dtIds'][0:maxDet] for e in E])[inds]
-                    # gt ann ids
-                    gtm_ids = dtm.copy()
-                    # build batch gt, dt, is_tp
-                    _matches.append(
-                        np.vstack([gtm_ids, dtm_ids, tps]).astype(np.int32).T)
-
                     tp_sum = np.cumsum(tps, axis=1).astype(dtype=float)
                     fp_sum = np.cumsum(fps, axis=1).astype(dtype=float)
 
                     for t, (tp, fp) in enumerate(zip(tp_sum, fp_sum)):
                         tp = np.array(tp)
                         fp = np.array(fp)
                         nd = len(tp)
@@ -448,24 +435,21 @@
                                 q[ri] = pr[pi]
                                 ss[ri] = dtScoresSorted[pi]
                         except:
                             pass
                         precision[t, :, k, a, m] = np.array(q)
                         scores[t, :, k, a, m] = np.array(ss)
 
-        _matches = np.vstack(_matches)
-
         self.eval = {
             'params': p,
             'counts': [T, R, K, A, M],
             'date': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
             'precision': precision,
             'recall': recall,
             'scores': scores,
-            'matches': _matches,
         }
 
         toc = time.time()
         self.print_function('DONE (t={:0.2f}s).'.format(toc-tic))
 
     def summarize(self):
         '''
@@ -566,49 +550,24 @@
 
         self.all_stats = summarize()
         self.stats = self.all_stats[:12]
 
     def __str__(self):
         self.summarize()
 
-    @property
-    def stats_as_dict(self):
-        iouType = self.params.iouType
-        assert (iouType == 'segm' or iouType ==
-                'bbox'), f'{iouType=} not supported'
-
-        labels = [
-            "AP_all", "AP_50", "AP_75",
-            "AP_small", "AP_medium", "AP_large",
-            "AR_all", "AR_second", "AR_third",
-            "AR_small", "AR_medium", "AR_large", "AR_50", "AR_75"]
-
-        maxDets = self.params.maxDets
-        if len(maxDets) > 1:
-            labels[6] = f'AR_{maxDets[0]}'
-
-        if len(maxDets) >= 2:
-            labels[7] = f'AR_{maxDets[1]}'
-
-        if len(maxDets) >= 3:
-            labels[8] = f'AR_{maxDets[2]}'
-
-        return {_label: float(self.all_stats[i]) for i, _label in enumerate(labels)}
-
 
 class Params:
     '''
     Params for coco evaluation api
     '''
 
     def setDetParams(self):
         self.imgIds = []
         self.catIds = []
         # np.arange causes trouble.  the data point on arange is slightly larger than the true value
-        self.iouThr = [.5, .75]
         self.iouThrs = np.linspace(.5, 0.95, int(
             np.round((0.95 - .5) / .05)) + 1, endpoint=True)
         self.recThrs = np.linspace(.0, 1.00, int(
             np.round((1.00 - .0) / .01)) + 1, endpoint=True)
         self.maxDets = [1, 10, 100]
         self.areaRng = [[0 ** 2, 1e5 ** 2], [0 ** 2, 32 ** 2],
                         [32 ** 2, 96 ** 2], [96 ** 2, 1e5 ** 2]]
```

### Comparing `faster-coco-eval-1.3.1/faster_coco_eval/core/mask.py` & `faster-coco-eval-1.3.2/faster_coco_eval/core/mask.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.1/faster_coco_eval.egg-info/PKG-INFO` & `faster-coco-eval-1.3.2/faster_coco_eval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.3.1
+Version: 1.3.2
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
 # Faster-COCO-Eval
 
 ## Disclaimer
@@ -74,14 +75,23 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.2
+
+- [x] rework math_matches function. moved to faster_eval_api
+- [x] Moved calculations from python to c++
+- [x] Separated extra classes
+- [x] Added new sample data
+- [x] append mIoU based on TP pred.
+- [x] append mAUC based on Coco pre/rec.
+
 ### v1.3.1
 
 - [x] rework mask code
 - [x] change np.float to float ([numpy deprecations](https://numpy.org/devdocs/release/1.20.0-notes.html#deprecations))
 
 ### v1.3.0
```

### Comparing `faster-coco-eval-1.3.1/faster_coco_eval.egg-info/SOURCES.txt` & `faster-coco-eval-1.3.2/faster_coco_eval.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 faster_coco_eval.egg-info/top_level.txt
 faster_coco_eval/core/__init__.py
 faster_coco_eval/core/coco.py
 faster_coco_eval/core/cocoeval.py
 faster_coco_eval/core/faster_eval_api.py
 faster_coco_eval/core/mask.py
 faster_coco_eval/extra/__init__.py
-faster_coco_eval/extra/curves.py
+faster_coco_eval/extra/curves.py
+faster_coco_eval/extra/display.py
+faster_coco_eval/extra/extra.py
```

### Comparing `faster-coco-eval-1.3.1/setup.py` & `faster-coco-eval-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,16 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=parse_requirements('requirements/runtime.txt'),
     extras_require={
         'all': parse_requirements('requirements/optional.txt'),
     },
 )
```

