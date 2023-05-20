# Comparing `tmp/ldimbenchmark-0.2.0.tar.gz` & `tmp/ldimbenchmark-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.2.0.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.1.tar", max compression
```

## Comparing `ldimbenchmark-0.2.0.tar` & `ldimbenchmark-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     3330 2023-05-16 20:22:12.027560 ldimbenchmark-0.2.0/README.md
--rw-r--r--   0        0        0     2359 2023-05-16 20:24:38.143954 ldimbenchmark-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0       60 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/__init__.py
--rw-r--r--   0        0        0    40101 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/benchmark.py
--rw-r--r--   0        0        0     6456 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
--rw-r--r--   0        0        0     8655 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
--rw-r--r--   0        0        0     3457 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
--rw-r--r--   0        0        0     7812 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
--rw-r--r--   0        0        0      195 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/__init__.py
--rw-r--r--   0        0        0     5117 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     6578 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0    10115 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/classes.py
--rw-r--r--   0        0        0     3928 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/cli.py
--rw-r--r--   0        0        0      176 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      211 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0    10884 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    17897 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0    11765 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     1285 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation_show.py
--rw-r--r--   0        0        0     2087 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0        0 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/__init__.py
--rw-r--r--   0        0        0     9939 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      880 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     1288 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/evaluation_metrics/__init__.py
--rw-r--r--   0        0        0     9680 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    12993 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      158 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    13338 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/dualmethod.py
--rw-r--r--   0        0        0    18958 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0    10445 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0     1171 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0     2033 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/random.py
--rw-r--r--   0        0        0        0 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/utils/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/utils/cusum.py
--rw-r--r--   0        0        0     8229 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/utilities.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.0/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-20 10:54:33.220180 ldimbenchmark-0.2.1/README.md
+-rw-r--r--   0        0        0     2359 2023-05-20 10:54:50.441393 ldimbenchmark-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    40659 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     6456 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8655 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3457 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7812 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     5440 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    17897 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-20 10:54:33.244181 ldimbenchmark-0.2.1/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    19401 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8229 2023-05-20 10:54:33.248182 ldimbenchmark-0.2.1/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.1/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.1/PKG-INFO
```

### Comparing `ldimbenchmark-0.2.0/README.md` & `ldimbenchmark-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/pyproject.toml` & `ldimbenchmark-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldimbenchmark"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["DanielHabenicht <daniel-habenicht@outlook.de>"]
 readme = "README.md"
 exclude = [
     "tests",
     "experiments"
 ]
```

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/benchmark.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ldimbenchmark.benchmark.runners.BaseMethodRunner import MethodRunner
 from ldimbenchmark.datasets import Dataset
 import pandas as pd
 import numpy as np
 from typing import Dict, Literal, TypedDict, Union, List, Callable
 import os
 import logging
-from ldimbenchmark.constants import LDIM_BENCHMARK_CACHE_DIR
+from ldimbenchmark.constants import CPU_COUNT, LDIM_BENCHMARK_CACHE_DIR
 from glob import glob
 from ldimbenchmark.benchmark_evaluation import evaluate_leakages
 from tabulate import tabulate
 from ldimbenchmark.benchmark_complexity import run_benchmark_complexity
 import matplotlib.pyplot as plt
 import enlighten
 from ldimbenchmark.evaluation_metrics import (
@@ -469,18 +469,23 @@
                                 dataset_base_id
                             ] = hyperparameters_method_map[method_id][key]
                             # {
                             #     **hyperparameters_without_datasets,
                             #     **hyperparameters_method_map[method_id][key],
                             # }
             else:
-                for dataset_base_id in dataset_base_ids:
-                    hyperparameters_map[method_id][
-                        dataset_base_id
-                    ] = hyperparameters_method_map[method_id]
+                if len(dataset_base_ids) == 0:
+                    hyperparameters_map[method_id] = hyperparameters_method_map[
+                        method_id
+                    ]
+                else:
+                    for dataset_base_id in dataset_base_ids:
+                        hyperparameters_map[method_id][
+                            dataset_base_id
+                        ] = hyperparameters_method_map[method_id]
 
         # if method_id in hyperparameters:
         #     if dataset_base_id in hyperparameters[method_id]:
         #         hyperparameters = hyperparameters[method_id][dataset_base_id]
         #     else:
         #         hyperparameters = {
         #             k: v
@@ -527,29 +532,36 @@
     def run_complexity_analysis(
         self,
         methods,
         style: Literal["time", "junctions"],
     ):
         complexity_results_path = os.path.join(self.complexity_results_dir, style)
         os.makedirs(complexity_results_path, exist_ok=True)
+        hyperparameters_map = self._get_hyperparameters_for_methods_and_datasets(
+            hyperparameters=self.hyperparameters,
+            method_ids=[lmethod.name for lmethod in methods],
+            dataset_base_ids=[],
+        )
         if style == "time":
             return run_benchmark_complexity(
                 methods,
                 cache_dir=os.path.join(self.cache_dir, "datagen"),
                 out_folder=complexity_results_path,
                 style="time",
                 additionalOutput=self.debug,
+                hyperparameters=hyperparameters_map,
             )
         if style == "junctions":
             return run_benchmark_complexity(
                 methods,
                 cache_dir=os.path.join(self.cache_dir, "datagen"),
                 out_folder=complexity_results_path,
                 style="junctions",
                 additionalOutput=self.debug,
+                hyperparameters=hyperparameters_map,
             )
 
     def run_benchmark(
         self,
         evaluation_mode: Union["training", "evaluation"],
         use_cached=True,
         parallel=False,
@@ -655,15 +667,15 @@
             desc="Experiments",
             unit="experiments",
             count=num_experiments - len(self.experiments),
         )
         bar_experiments.refresh()
         # This line makes sure we can call update with an effect
         if parallel:
-            worker_num = os.cpu_count() - 1
+            worker_num = CPU_COUNT
             if parallel_max_workers > 0:
                 worker_num = parallel_max_workers
             try:
                 with ProcessPoolExecutor(max_workers=worker_num) as executor:
                     # submit all tasks and get future objects
                     futures = [
                         executor.submit(execute_experiment, runner)
@@ -958,15 +970,15 @@
         pbar2 = manager.counter(
             total=len(result["matched_leaks_list"]),
             desc="Graphs:",
             unit="graphs",
         )
         parallel = False
         if parallel:
-            with ProcessPoolExecutor(max_workers=os.cpu_count() - 1) as executor:
+            with ProcessPoolExecutor(max_workers=CPU_COUNT) as executor:
                 # submit all tasks and get future objects
                 futures = []
                 for leak_pair in result["matched_leaks_list"]:
                     future = executor.submit(
                         plot_leak,
                         loaded_datasets[result["dataset_id"]],
                         leak_pair=leak_pair,
```

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark_complexity.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         dataset.getTrainingBenchmarkData(),
         dataset.getEvaluationBenchmarkData(),
     )
 
 
 def run_benchmark_complexity(
     methods: List[LDIMMethodBase],
+    hyperparameters,
     cache_dir=os.path.join(LDIM_BENCHMARK_CACHE_DIR, "datagen"),
     out_folder="out/complexity",
     style=None,
     additionalOutput=False,
 ):
     """
     Run the benchmark for the given methods and datasets.
@@ -94,15 +95,23 @@
     )
     logging.info(" > Starting Complexity analysis")
     for method in methods:
         logging.info(f" - {method.name}")
 
         if additionalOutput:
             method.init_with_benchmark_params(
-                os.path.join(out_folder, "additional_output_path"), {}
+                additional_output_path=os.path.join(
+                    out_folder, "additional_output_path"
+                ),
+                hyperparameters=hyperparameters[method.name],
+            )
+        else:
+            method.init_with_benchmark_params(
+                additional_output_path=None,
+                hyperparameters=hyperparameters[method.name],
             )
 
         def runAlgorithmWithNetwork(n):
             method.prepare(datasets[n]["training"])
             method.detect_offline(datasets[n]["evaluation"])
 
         # Run Big-O
```

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/classes.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/cli.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/cli.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/analysis.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/analysis.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/classes.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/derivation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation_show.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/derivation_show.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/library.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_battledim.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/loaders/load_battledim.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_dataset_base.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/datasets/loaders/load_dataset_base.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/evaluation_metrics/__init__.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/evaluation_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/dualmethod.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/dualmethod.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/lila.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/lila.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,17 +296,27 @@
 
             else:
                 if self.hyperparameters["default_flow_sensor"] == "sum":
                     simple_training_data.flows[
                         "PUMP_1"
                     ] = simple_training_data.flows.sum(axis=1)
                 else:
-                    simple_training_data.flows["PUMP_1"] = simple_training_data.flows[
+                    if (
                         self.hyperparameters["default_flow_sensor"]
-                    ]
+                        in simple_training_data.flows.columns
+                    ):
+                        simple_training_data.flows[
+                            "PUMP_1"
+                        ] = simple_training_data.flows[
+                            self.hyperparameters["default_flow_sensor"]
+                        ]
+                    else:
+                        raise Exception(
+                            "No 'default_flow_sensor' hyperparameter given or the column does not exist."
+                        )
                 self._train(simple_training_data, start_time, end_time, dma="main")
 
     def detect_offline(
         self, evaluation_data: BenchmarkData
     ) -> List[BenchmarkLeakageResult]:
         simple_evaluation_data = simplifyBenchmarkData(
             evaluation_data,
```

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/mnf.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/mnf.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/null.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/random.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/random.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/utils/cusum.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/methods/utils/cusum.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/src/ldimbenchmark/utilities.py` & `ldimbenchmark-0.2.1/src/ldimbenchmark/utilities.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.0/setup.py` & `ldimbenchmark-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'wntr>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['ldimbenchmark = ldimbenchmark.cli:cli']}
 
 setup_kwargs = {
     'name': 'ldimbenchmark',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
     'long_description': '[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)\n[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)\n\n# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.\n\nIt provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\nfrom typing import List\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# python 3.10\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\npytest tests/test_derivation.py -k \'test_mything\'\npytest --testmon\npytest --snapshot-update\n\n# Pytest watch\nptw\nptw -- --testmon\n\n# Watch a file during development\nnpm install -g nodemon\nnodemon -L experiments/auto_hyperparameter.py\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/\nhttps://click.palletsprojects.com/en/8.1.x/\n\n```\nmkdocs serve\n```\n\n# TODO\n\nLDIMBenchmark:\nData Cleansing before working with them\n\n- per sensor type, e.g. waterflow (cut of at 0)\n- removing datapoints which are clearly a malfunction\n',
     'author': 'DanielHabenicht',
     'author_email': 'daniel-habenicht@outlook.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ldimbenchmark-0.2.0/PKG-INFO` & `ldimbenchmark-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldimbenchmark
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: DanielHabenicht
 Author-email: daniel-habenicht@outlook.de
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

