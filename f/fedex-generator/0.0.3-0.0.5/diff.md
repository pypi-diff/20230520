# Comparing `tmp/fedex_generator-0.0.3.tar.gz` & `tmp/fedex_generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex_generator-0.0.3.tar", last modified: Wed Jan 18 22:00:32 2023, max compression
+gzip compressed data, was "fedex_generator-0.0.5.tar", last modified: Sat May 20 16:29:38 2023, max compression
```

## Comparing `fedex_generator-0.0.3.tar` & `fedex_generator-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.308763 fedex_generator-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.308763 fedex_generator-0.0.3/src/fedex_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/src/fedex_generator/Measures/
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/BaseMeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/Bins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/DiversityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/ExceptionalityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/NormalizedDiversityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Measures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/src/fedex_generator/Operations/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Operations/Filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Operations/GroupBy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Operations/Join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Operations/Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/src/fedex_generator/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/commons/DatasetRelation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/commons/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/commons/kstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-01-18 22:00:03.000000 fedex_generator-0.0.3/src/fedex_generator/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:00:32.312763 fedex_generator-0.0.3/src/fedex_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-18 22:00:32.000000 fedex_generator-0.0.3/src/fedex_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-18 22:00:32.000000 fedex_generator-0.0.3/src/fedex_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 22:00:32.000000 fedex_generator-0.0.3/src/fedex_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-18 22:00:32.000000 fedex_generator-0.0.3/src/fedex_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-18 22:00:32.000000 fedex_generator-0.0.3/src/fedex_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/fedex_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/fedex_generator/Measures/
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/BaseMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/Bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/DiversityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/ExceptionalityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/NormalizedDiversityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Measures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/fedex_generator/Operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Operations/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Operations/GroupBy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Operations/Join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Operations/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/fedex_generator/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/commons/DatasetRelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/commons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/commons/kstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-20 16:29:25.000000 fedex_generator-0.0.5/src/fedex_generator/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:29:38.849079 fedex_generator-0.0.5/src/fedex_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-20 16:29:38.000000 fedex_generator-0.0.5/src/fedex_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-20 16:29:38.000000 fedex_generator-0.0.5/src/fedex_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:29:38.000000 fedex_generator-0.0.5/src/fedex_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-20 16:29:38.000000 fedex_generator-0.0.5/src/fedex_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 16:29:38.000000 fedex_generator-0.0.5/src/fedex_generator.egg-info/top_level.txt
```

### Comparing `fedex_generator-0.0.3/LICENSE` & `fedex_generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/PKG-INFO` & `fedex_generator-0.0.5/src/fedex_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fedex_generator
-Version: 0.0.3
+Name: fedex-generator
+Version: 0.0.5
 Project-URL: Git, https://github.com/analysis-bots/FEDEx_Generator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 
 # Fedex Genarator
```

### Comparing `fedex_generator-0.0.3/README.md` & `fedex_generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/setup.py` & `fedex_generator-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Measures/BaseMeasure.py` & `fedex_generator-0.0.5/src/fedex_generator/Measures/BaseMeasure.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,25 +160,35 @@
         if influence_var == 0:
             return 0.0
         influence_mean = np.mean(influence_vals_list)
 
         return (influence - influence_mean) / np.sqrt(influence_var)
 
     def calc_influence(self, brute_force=False, top_k=TOP_K_DEFAULT,
-                       figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None):
-        score_and_col = [(self.score_dict[col][2], col, self.score_dict[col][1], self.score_dict[col][3])
-                         for col in self.score_dict]
+                       figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None, deleted = None):###
+        if deleted:###
+            score_dict = deleted
+        else:
+            score_dict = self.score_dict
+                                    ###            
+        score_and_col = [(score_dict[col][2], col, score_dict[col][1], score_dict[col][3])
+                         for col in score_dict]
+      
+                         
         list_scores_sorted = score_and_col
         list_scores_sorted.sort()
-        K = top_k
+        K = top_k ###
+        if deleted:
+            K = len(deleted.keys())
+                        ####
         results_columns = ["score", "significance", "influence", "explanation", "bin", "influence_vals"]
         results = pd.DataFrame([], columns=results_columns)
         figures = []
         for score, max_col_name, bins, _ in list_scores_sorted[:-K - 1:-1]:
-            source_name, bins, score, _ = self.score_dict[max_col_name]
+            source_name, bins, score, _ = score_dict[max_col_name]
             for current_bin in bins.bins:
                 influence_vals = self.get_influence_col(max_col_name, current_bin, brute_force)
                 influence_vals_list = np.array(list(influence_vals.values()))
 
                 if np.all(np.isnan(influence_vals_list)):
                     continue
 
@@ -202,30 +212,31 @@
         influence_vals = results[skyline]["influence_vals"]
         scores = results[skyline]["score"]
 
         if len(scores) == 0:
             print(f'{source_name} dataset there is not interesting explanation')
             return
 
-        if top_k > 1:
+        if K > 1: ###
             rows = math.ceil(len(scores) / figs_in_row)
             fig, axes = plt.subplots(rows, figs_in_row, figsize=(7 * figs_in_row, 8 * rows))
             for ax in axes.reshape(-1):
                 ax.set_axis_off()
         else:
             fig, axes = plt.subplots(figsize=(7, 7))
 
         title = title if title else self.build_operation_expression(source_name)
         fig.suptitle(title, fontsize=20)
 
         for index, (explanation, current_bin, current_influence_vals, score) in enumerate(
                 zip(explanations, bins, influence_vals, scores)):
 
+
             fig = self.draw_bar(current_bin, current_influence_vals, title=explanation,
-                                ax=axes.reshape(-1)[index] if top_k > 1 else axes, score=score, show_scores=show_scores)
+                                ax=axes.reshape(-1)[index] if K > 1 else axes, score=score, show_scores=show_scores) ###
             if fig:
                 figures.append(fig)
 
         plt.tight_layout()
         return figures if len(figures) > 0 else fig
 
     def calc_interestingness_only(self):
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Measures/Bins.py` & `fedex_generator-0.0.5/src/fedex_generator/Measures/Bins.py`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Measures/DiversityMeasure.py` & `fedex_generator-0.0.5/src/fedex_generator/Measures/DiversityMeasure.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     if items_to_bold is not None:
         items_to_bold = items_to_bold if utils.is_numeric(items_to_bold) else [utils.to_valid_latex(i) for i in
                                                                                items_to_bold]
 
     bar = ax.bar(ind, y, width, alpha=alpha)
     ax.set_xticks(ind)
     ax.set_xticklabels(tuple([str(i) for i in x]), rotation='vertical')
+    ax.set_ylim(min(y) - min(y) * 0.01, max(y) + max(y) * 0.001)
 
     if avg_line is not None:
         ax.axhline(avg_line, color='red', linewidth=1)
     if items_to_bold is not None:
         for item in items_to_bold:
             bar[x.index(item)].set_color('green')
     if head_values is not None:
@@ -192,15 +193,15 @@
         else:
             var_rel = 1.
 
         res = (var_res / var_rel) if var_rel != 0 else (0. if var_res == 0 else var_res)
         return 0 if np.isnan(res) else res
 
     def calc_measure_internal(self, bin: Bin):
-        result_column = bin.result_column.dropna()
+        result_column = bin.get_binned_result_column().dropna()
         if bin.name == "MultiIndexBin":
             operation = self.get_agg_func_from_name(result_column.name)
             result_column = result_column.groupby(bin.get_bin_name()).agg(operation)
         return self.calc_diversity(None if bin.source_column is None else bin.source_column.dropna(),
                                    result_column)
 
     def build_operation_expression(self, source_name):
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Measures/ExceptionalityMeasure.py` & `fedex_generator-0.0.5/src/fedex_generator/Measures/ExceptionalityMeasure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import math
 
 import numpy as np
+import pandas as pd
 
 from fedex_generator.commons import utils
 from fedex_generator.Measures.BaseMeasure import BaseMeasure, START_BOLD, END_BOLD
 from fedex_generator.Measures.Bins import Bin
 
 
+
 class ExceptionalityMeasure(BaseMeasure):
     def __init__(self):
         super().__init__()
 
     def draw_bar(self, bin_item: Bin, influence_vals: dict = None, title=None, ax=None, score=None,
                  show_scores: bool = False):
         res_col = bin_item.get_binned_result_column()
@@ -44,21 +46,23 @@
         label_tags = tuple([utils.to_valid_latex(bin_item.get_bin_representation(i)) for i in labels])
         tags_max_length = max([len(tag) for tag in label_tags])
         ax.set_xticklabels(label_tags, rotation='vertical' if tags_max_length >= 4 else 'horizontal')
 
         ax.set_xlabel(utils.to_valid_latex(bin_item.get_bin_name() + " values"), fontsize=20)
         ax.set_ylabel("frequency(\\%)", fontsize=16)
 
+
         if title is not None:
             if show_scores:
                 ax.set_title(f'score: {score}\n {utils.to_valid_latex(title)}', fontdict={'fontsize': 14})
             else:
                 ax.set_title(utils.to_valid_latex(title), fontdict={'fontsize': 14})
 
         ax.set_axis_on()
+        return bin_item.get_bin_name() ####
 
     def interestingness_only_explanation(self, source_col, result_col, col_name):
         if utils.is_categorical(source_col):
             vc = source_col.value_counts()
             source_max = utils.max_key(vc)
             vc = result_col.value_counts()
             result_max = utils.max_key(vc)
@@ -86,14 +90,16 @@
         r = r[r == r]
         return 0 if len(r) == 0 else utils.ks_2samp(s, r).statistic
 
     def calc_influence_col(self, current_bin: Bin):
         bin_values = current_bin.get_bin_values()
         source_col = current_bin.get_source_by_values(bin_values)
         res_col = current_bin.get_result_by_values(bin_values)
+        if len(bin_values) > 15:
+            bin_values = list(source_col.value_counts().nlargest(15).keys())
         score_all = ExceptionalityMeasure.kstest(source_col, res_col)
         influence = []
         for value in bin_values:
             source_col_only_list = current_bin.get_source_by_values([b for b in bin_values if b != value])
             res_col_only_list = current_bin.get_result_by_values([b for b in bin_values if b != value])
 
             score_without_bin = ExceptionalityMeasure.kstest(source_col_only_list, res_col_only_list)
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Measures/NormalizedDiversityMeasure.py` & `fedex_generator-0.0.5/src/fedex_generator/Measures/NormalizedDiversityMeasure.py`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Operations/GroupBy.py` & `fedex_generator-0.0.5/src/fedex_generator/Operations/GroupBy.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 continue
             yield attr, DatasetRelation(None, self.result_df, self.source_name)
 
     def get_source_col(self, filter_attr, filter_values, bins):
         return None
 
     def explain(self, schema=None, attributes=None, top_k=TOP_K_DEFAULT,
-                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None):
+                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None, corr_TH: float = 0.7):
         """
         Explain for group by operation
         :param schema: dictionary with new columns names, in case {'col_name': 'i'} will be ignored in the explanation
         :param attributes: only this attributes will be included in the explanation calculation
         :param top_k: top k explanations number, default one explanation only.
         :param show_scores: show scores on explanation
         :param figs_in_row: number of explanations figs in one row
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Operations/Join.py` & `fedex_generator-0.0.5/src/fedex_generator/Operations/Join.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         for attr in set(self.right_df.columns) - set(self.left_df.columns):
             if attr.lower() == "index":
                 continue
             yield attr, DatasetRelation(self.right_df, self.result_df, self.right_name)
 
     def explain(self, schema=None, attributes=None, top_k=TOP_K_DEFAULT,
-                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None):
+                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None, corr_TH: float = 0.7):
         """
         Explain for filter operation
 
         :param schema: dictionary with new columns names, in case {'col_name': 'i'} will be ignored in the explanation
         :param attributes: only this attributes will be included in the explanation calculation
         :param top_k: top k explanations number, default one explanation only.
         :param show_scores: show scores on explanation
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/Operations/Operation.py` & `fedex_generator-0.0.5/src/fedex_generator/Operations/Operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,21 +9,24 @@
     def set_bins_count(self, n):
         self.bins_count = n
 
     def get_bins_count(self):
         return self.bins_count
 
     def explain(self, schema=None, attributes=None, top_k=TOP_K_DEFAULT,
-                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None):
+                figs_in_row: int = DEFAULT_FIGS_IN_ROW, show_scores: bool = False, title: str = None, corr_TH: float = 0.7):
         """
         Explain for operation
         :param schema: dictionary with new columns names, in case {'col_name': 'i'} will be ignored in the explanation
         :param attributes: only this attributes will be included in the explanation calculation
         :param top_k: top k explanations number, default one explanation only.
         :param figs_in_row: number of explanations figs in one row
         :param show_scores: show scores on explanation
         :param title: explanation title
 
 
         :return: explain figures
         """
         raise NotImplementedError()
+        
+    def present_deleted_correlated(self, figs_in_row: int = DEFAULT_FIGS_IN_ROW): #####
+        return NotImplementedError()
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/commons/DatasetRelation.py` & `fedex_generator-0.0.5/src/fedex_generator/commons/DatasetRelation.py`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/src/fedex_generator/commons/kstest.py` & `fedex_generator-0.0.5/src/fedex_generator/commons/kstest.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,14 +402,18 @@
     if mode not in ['auto', 'exact', 'asymp']:
         raise ValueError(f'Invalid value for mode: {mode}')
     alternative = {'t': 'two-sided', 'g': 'greater', 'l': 'less'}.get(
         alternative.lower()[0], alternative)
     if alternative not in ['two-sided', 'less', 'greater']:
         raise ValueError(f'Invalid value for alternative: {alternative}')
     MAX_AUTO_N = 10000  # 'auto' will attempt to be exact if n1,n2 <= MAX_AUTO_N
+    #np.random.shuffle(data1)
+    #np.random.shuffle(data2)
+    #data1 = data1[:5000]
+    #data2 = data2[:5000]
     if np.ma.is_masked(data1):
         data1 = data1.compressed()
     if np.ma.is_masked(data2):
         data2 = data2.compressed()
     data1 = np.sort(data1)
     data2 = np.sort(data2)
     n1 = data1.shape[0]
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator/commons/utils.py` & `fedex_generator-0.0.5/src/fedex_generator/commons/utils.py`

 * *Files identical despite different names*

### Comparing `fedex_generator-0.0.3/src/fedex_generator.egg-info/PKG-INFO` & `fedex_generator-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fedex-generator
-Version: 0.0.3
+Name: fedex_generator
+Version: 0.0.5
 Project-URL: Git, https://github.com/analysis-bots/FEDEx_Generator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 
 # Fedex Genarator
```

### Comparing `fedex_generator-0.0.3/src/fedex_generator.egg-info/SOURCES.txt` & `fedex_generator-0.0.5/src/fedex_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

