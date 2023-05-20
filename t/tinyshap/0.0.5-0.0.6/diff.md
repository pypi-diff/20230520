# Comparing `tmp/tinyshap-0.0.5.tar.gz` & `tmp/tinyshap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.5.tar", last modified: Thu May 18 16:39:58 2023, max compression
+gzip compressed data, was "tinyshap-0.0.6.tar", last modified: Sat May 20 20:00:48 2023, max compression
```

## Comparing `tinyshap-0.0.5.tar` & `tinyshap-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:39:58.729894 tinyshap-0.0.5/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.5/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-18 16:39:58.729894 tinyshap-0.0.5/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      946 2023-05-18 16:22:52.000000 tinyshap-0.0.5/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1118 2023-05-18 16:37:39.000000 tinyshap-0.0.5/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-18 16:39:58.729894 tinyshap-0.0.5/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:39:58.001849 tinyshap-0.0.5/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:39:58.289505 tinyshap-0.0.5/src/tinyshap/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.0.5/src/tinyshap/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3835 2023-05-18 16:22:52.000000 tinyshap-0.0.5/src/tinyshap/explainer.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:39:58.660929 tinyshap-0.0.5/src/tinyshap.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-18 16:39:57.000000 tinyshap-0.0.5/src/tinyshap.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      262 2023-05-18 16:39:57.000000 tinyshap-0.0.5/src/tinyshap.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-18 16:39:57.000000 tinyshap-0.0.5/src/tinyshap.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       34 2023-05-18 16:39:57.000000 tinyshap-0.0.5/src/tinyshap.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-18 16:39:57.000000 tinyshap-0.0.5/src/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:50.054555 tinyshap-0.0.6/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.6/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-20 20:00:50.054555 tinyshap-0.0.6/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      946 2023-05-18 16:22:52.000000 tinyshap-0.0.6/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1144 2023-05-20 19:59:07.000000 tinyshap-0.0.6/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-20 20:00:50.054555 tinyshap-0.0.6/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.679554 tinyshap-0.0.6/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.820179 tinyshap-0.0.6/src/tinyshap/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.0.6/src/tinyshap/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4036 2023-05-20 19:59:07.000000 tinyshap-0.0.6/src/tinyshap/explainer.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:49.992053 tinyshap-0.0.6/src/tinyshap.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      286 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       55 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-20 20:00:49.000000 tinyshap-0.0.6/src/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 20:00:50.023304 tinyshap-0.0.6/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2634 2023-05-20 19:59:07.000000 tinyshap-0.0.6/tests/test_explainer.py
```

### Comparing `tinyshap-0.0.5/LICENCE` & `tinyshap-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.5/PKG-INFO` & `tinyshap-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.5
+Version: 0.0.6
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinyshap-0.0.5/README.md` & `tinyshap-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.5/pyproject.toml` & `tinyshap-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'tinyshap'
-version = '0.0.5'
+version = '0.0.6'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.7'
 dependencies = [
   "pandas>=1.4.0",
   "scikit-learn>=1.1.1",
+  "constrainedlr>=0.0.8"
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

### Comparing `tinyshap-0.0.5/src/tinyshap/explainer.py` & `tinyshap-0.0.6/src/tinyshap/explainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from typing import List
 
 import numpy as np
 import pandas as pd
-from sklearn.linear_model import LinearRegression
+from constrainedlr import ConstrainedLinearRegression
 
 
 def shap_kernel(coalition: List[int], dim: int) -> float:
     size = sum(coalition)
     return (dim - 1) / (math.comb(dim, size) * size * (dim - size))
 
 
@@ -72,24 +72,26 @@
 
     def _explain_sample(self, x_test: np.ndarray) -> pd.Series:
         """
         Calculates SHAP values of a single sample using approximate KernelSHAP
         """
         assert x_test.ndim == 1
 
+        model_prediction = self.model(pd.DataFrame(x_test.reshape(1, -1), columns=self.X.columns))
+
         coalitions = self._generate_coalitions()
         feature_values = self._get_feature_values(coalitions, x_test)
         predictions = self.model(feature_values)
         weights = self._get_coalition_weights(coalitions)
 
-        lr = LinearRegression(fit_intercept=True)
-        lr.fit(coalitions, predictions, sample_weight=weights)
+        lr = ConstrainedLinearRegression(fit_intercept=True)
+        lr.fit(coalitions, predictions, sample_weight=weights, features_sum_constraint_equal=model_prediction)
         shap_values = pd.Series(data=lr.coef_, index=self.X.columns)
         shap_values["avg_prediction"] = lr.intercept_
         return shap_values
 
     def shap_values(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Calculates SHAP values of multiple samples in `X`
         """
-        shap_values = X.apply(self._explain_sample, axis=1)
+        shap_values = X.apply(lambda row: self._explain_sample(np.array(row.tolist())), axis=1)
         return shap_values
```

### Comparing `tinyshap-0.0.5/src/tinyshap.egg-info/PKG-INFO` & `tinyshap-0.0.6/src/tinyshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.5
+Version: 0.0.6
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

