# Comparing `tmp/caafe-0.1.tar.gz` & `tmp/caafe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caafe-0.1.tar", last modified: Fri May 19 21:03:11 2023, max compression
+gzip compressed data, was "caafe-0.1.2.tar", last modified: Sat May 20 09:25:09 2023, max compression
```

## Comparing `caafe-0.1.tar` & `caafe-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:03:11.498392 caafe-0.1/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-19 21:02:53.000000 caafe-0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-19 21:03:11.498392 caafe-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      991 2023-05-19 21:02:53.000000 caafe-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:03:11.496392 caafe-0.1/caafe/
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-19 21:02:53.000000 caafe-0.1/caafe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11664 2023-05-19 21:02:53.000000 caafe-0.1/caafe/caafe.py
--rw-r--r--   0 root         (0) root         (0)     4055 2023-05-19 21:02:53.000000 caafe-0.1/caafe/caafe_evaluate.py
--rw-r--r--   0 root         (0) root         (0)    11094 2023-05-19 21:02:53.000000 caafe-0.1/caafe/data.py
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-19 21:02:53.000000 caafe-0.1/caafe/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-05-19 21:02:53.000000 caafe-0.1/caafe/feature_extension_baselines.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-05-19 21:02:53.000000 caafe-0.1/caafe/metrics.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-05-19 21:02:53.000000 caafe-0.1/caafe/plotting.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-19 21:02:53.000000 caafe-0.1/caafe/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-05-19 21:02:53.000000 caafe-0.1/caafe/run_llm_code.py
--rw-r--r--   0 root         (0) root         (0)     4079 2023-05-19 21:02:53.000000 caafe-0.1/caafe/sklearn_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:03:11.497392 caafe-0.1/caafe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-19 21:03:11.000000 caafe-0.1/caafe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-19 21:03:11.000000 caafe-0.1/caafe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:03:11.000000 caafe-0.1/caafe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-19 21:03:11.000000 caafe-0.1/caafe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-19 21:03:11.000000 caafe-0.1/caafe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 21:03:11.500393 caafe-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-19 21:02:53.000000 caafe-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:03:11.497392 caafe-0.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 21:02:53.000000 caafe-0.1/tests/test_sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-20 09:23:35.000000 caafe-0.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-20 09:25:09.129420 caafe-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-05-20 09:23:35.000000 caafe-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.128420 caafe-0.1.2/caafe/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11664 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/caafe.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/caafe_evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11093 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/data.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/feature_extension_baselines.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/plotting.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7895 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/run_llm_code.py
+-rw-r--r--   0 root         (0) root         (0)     5270 2023-05-20 09:23:35.000000 caafe-0.1.2/caafe/sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/caafe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-20 09:25:08.000000 caafe-0.1.2/caafe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 09:25:09.129420 caafe-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-20 09:25:03.000000 caafe-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 09:25:09.129420 caafe-0.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 09:23:35.000000 caafe-0.1.2/tests/test_sklearn_wrapper.py
```

### Comparing `caafe-0.1/PKG-INFO` & `caafe-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1
+Version: 0.1.2
 Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
@@ -13,25 +13,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE.txt
 
 ### Usage
-Use this colab notebook for a quickstart.
+[![DEMO VIDEO](https://i.makeagif.com/media/5-20-2023/E4RfRM.gif)](https://www.youtube.com/watch?v=6zCD48d3kNU)
 
-Use CAFE_minimal.ipynb for a minimal example of how to use CAAFE on your dataset.
+CAAFE lets you semi-automate your feature engineering process based on your explanations on the dataset and with the help of language models. It is based on the paper "LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering" by Hollmann, Müller, and Hutter (2023).
+CAAFE systematically verifies the generated features to ensure that only features that are actually useful are added to the dataset.
 
-Use CAAFE.ipynb to reproduce the experiments from the paper.
+To use CAAFE, first create a CAAFEClassifier object with the desired parameters:
+```
+caafe_clf = CAAFEClassifier(base_classifier=clf_no_feat_eng,
+                      llm_model="gpt-4",
+                      iterations=2)
+```
+Then, fit the classifier to your training data:
+```
+caafe_clf.fit_pandas(df_train,
+               target_column_name=target_column_name,
+               dataset_description=dataset_description,
+              disable_caafe=False
+              )
+```
+Finally, use the classifier to make predictions on your test data:
+```
+pred = caafe_clf.predict(df_test)
+```
 
-#### Choosing an Iterative Classifier
-The iterative classifier gets called in each 
+You can also try out the demo at: https://colab.research.google.com/drive/1mCA8xOAJZ4MaB_alZvyARTMjhl6RZf0a
 
-### Access Tokens
-#### OpenAI
+For a minimal example of how to use CAAFE on your dataset, use CAFE_minimal.ipynb. To reproduce the experiments from the paper, use CAAFE.ipynb.
 
 
 ### Paper
 Hollmann, N., Müller, S., & Hutter, F. (2023). LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering
 https://arxiv.org/abs/2305.03403
 
 ### License
```

### Comparing `caafe-0.1/caafe/caafe.py` & `caafe-0.1.2/caafe/caafe.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1/caafe/caafe_evaluate.py` & `caafe-0.1.2/caafe/caafe_evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import copy
 import pandas as pd
 import tabpfn
 import numpy as np
 from .data import get_X_y
-from .preprocessing import make_datasets_numeric
+from .preprocessing import make_datasets_numeric, make_dataset_numeric
 from sklearn.base import BaseEstimator
 
 
 def evaluate_dataset(
     df_train: pd.DataFrame,
     df_test: pd.DataFrame,
     prompt_id,
     name,
     method,
     metric_used,
     target_name,
     max_time=300,
     seed=0,
 ):
-    df_train, df_test = make_datasets_numeric(df_train, df_test, target_name)
+    df_train, df_test = copy.deepcopy(df_train), copy.deepcopy(df_test)
+    df_train, _, mappings = make_datasets_numeric(
+        df_train, None, target_name, return_mappings=True
+    )
+    df_test = make_dataset_numeric(df_test, mappings=mappings)
 
     if df_test is not None:
         test_x, test_y = get_X_y(df_test, target_name=target_name)
 
     x, y = get_X_y(df_train, target_name=target_name)
     feature_names = list(df_train.drop(target_name, axis=1).columns)
```

### Comparing `caafe-0.1/caafe/data.py` & `caafe-0.1.2/caafe/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         ]
     )
     description = str.join("\n\n", np.array(splits)[sel].tolist())
     return description
 
 
 def get_X_y(df_train, target_name):
-    y = torch.tensor(df_train[target_name].astype(bool).to_numpy())
+    y = torch.tensor(df_train[target_name].astype(int).to_numpy())
     x = torch.tensor(df_train.drop(target_name, axis=1).to_numpy())
 
     return x, y
 
 
 def get_data_split(ds, seed):
     def get_df(X, y):
```

### Comparing `caafe-0.1/caafe/evaluate.py` & `caafe-0.1.2/caafe/evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1/caafe/metrics.py` & `caafe-0.1.2/caafe/metrics.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1/caafe/plotting.py` & `caafe-0.1.2/caafe/plotting.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1/caafe/run_llm_code.py` & `caafe-0.1.2/caafe/run_llm_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 import copy
 import numpy as np
 from .preprocessing import convert_categorical_to_integer_f
+from typing import Any, Dict, Optional
+import pandas as pd
 
-
-def run_llm_code(code, df, convert_categorical_to_integer=True, fill_na=True):
+def run_llm_code(code: str, df: pd.DataFrame, convert_categorical_to_integer: Optional[bool] = True, fill_na: Optional[bool] = True) -> pd.DataFrame:
+    """
+    Executes the given code on the given dataframe and returns the resulting dataframe.
+
+    Parameters:
+    code (str): The code to execute.
+    df (pandas.DataFrame): The dataframe to execute the code on.
+    convert_categorical_to_integer (bool, optional): Whether to convert categorical columns to integer values. Defaults to True.
+    fill_na (bool, optional): Whether to fill NaN values in object columns with empty strings. Defaults to True.
+
+    Returns:
+    pandas.DataFrame: The resulting dataframe after executing the code.
+    """
     try:
         loc = {}
         df = copy.deepcopy(df)
 
         if fill_na and False:
             df.loc[:, (df.dtypes == object)] = df.loc[:, (df.dtypes == object)].fillna(
                 ""
@@ -28,15 +41,24 @@
     return df
 
 
 import ast
 import pandas as pd
 
 
-def check_ast(node):
+def check_ast(node: ast.AST) -> None:
+    """
+    Checks if the given AST node is allowed.
+
+    Parameters:
+    node (ast.AST): The AST node to check.
+
+    Raises:
+    ValueError: If the AST node is not allowed.
+    """
     allowed_nodes = {
         ast.Module,
         ast.Expr,
         ast.Load,
         ast.BinOp,
         ast.UnaryOp,
         ast.Add,
@@ -156,42 +178,45 @@
         "arange",
         "values",
         "linspace",
         # PD
         "mean",
         "sum",
         "contains",
+        "where",
         "min",
         "max",
         "median",
         "std",
         "sqrt",
         "pow",
         "iloc",
         "cut",
         "qcut",
         "inf",
         "nan",
         "isna",
         "map",
         "reshape",
+        "shape",
         "split",
         "var",
         "codes",
         "abs",
         "cumsum",
         "cumprod",
         "cummax",
         "cummin",
         "diff",
         "repeat",
         "index",
         "log",
         "log10",
         "log1p",
+        "slice",
         "exp",
         "expm1",
         "pow",
         "pct_change",
         "corr",
         "cov",
         "round",
```

### Comparing `caafe-0.1/caafe/sklearn_wrapper.py` & `caafe-0.1.2/caafe/sklearn_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from sklearn.utils.multiclass import unique_labels
 from .run_llm_code import run_llm_code
-from .preprocessing import make_datasets_numeric, split_target_column
+from .preprocessing import (
+    make_datasets_numeric,
+    split_target_column,
+    make_dataset_numeric,
+)
+from .data import get_X_y
 from .caafe import generate_features
 from .metrics import auc_metric, accuracy_metric
 import pandas as pd
 import numpy as np
 
 
 class CAAFEClassifier(BaseEstimator, ClassifierMixin):
+    """
+    A classifier that uses the CAAFE algorithm to generate features and a base classifier to make predictions.
+
+    Parameters:
+    base_classifier (object, optional): The base classifier to use. If None, a default TabPFNClassifier will be used. Defaults to None.
+    optimization_metric (str, optional): The metric to optimize during feature generation. Can be 'accuracy' or 'auc'. Defaults to 'accuracy'.
+    iterations (int, optional): The number of iterations to run the CAAFE algorithm. Defaults to 10.
+    llm_model (str, optional): The LLM model to use for generating features. Defaults to 'gpt-3.5-turbo'.
+    n_splits (int, optional): The number of cross-validation splits to use during feature generation. Defaults to 10.
+    n_repeats (int, optional): The number of times to repeat the cross-validation during feature generation. Defaults to 2.
+    """
     def __init__(
         self,
         base_classifier=None,
         optimization_metric="accuracy",
         iterations=10,
         llm_model="gpt-3.5-turbo",
         n_splits=10,
@@ -35,50 +51,49 @@
         self.llm_model = llm_model
         self.iterations = iterations
         self.optimization_metric = optimization_metric
         self.n_splits = n_splits
         self.n_repeats = n_repeats
 
     def fit_pandas(self, df, dataset_description, target_column_name, **kwargs):
-        X, y = df.drop(columns=[target_column_name]), df[target_column_name]
+        feature_columns = df.drop(columns=[target_column_name]).columns
+
+        X, y = (
+            df.drop(columns=[target_column_name]).values,
+            df[target_column_name].values,
+        )
         return self.fit(
-            X, y, dataset_description, X.columns, target_column_name, **kwargs
+            X, y, dataset_description, feature_columns, target_column_name, **kwargs
         )
 
     def fit(
         self, X, y, dataset_description, feature_names, target_name, disable_caafe=False
     ):
-
-        # Check that X and y have correct shape
-        X, y = check_X_y(X, y)
-
         self.dataset_description = dataset_description
         self.feature_names = list(feature_names)
         self.target_name = target_name
 
-        # Store the classes seen during fit
-        self.classes_ = unique_labels(y)
-
         self.X_ = X
         self.y_ = y
 
         ds = [
             "dataset",
             X,
             y,
             [],
             self.feature_names + [target_name],
             {},
             dataset_description,
         ]
         # Add X and y as one dataframe
         df_train = pd.DataFrame(
-            np.concatenate([X, y.reshape(-1, 1)], axis=1),
-            columns=self.feature_names + [target_name],
+            X,
+            columns=self.feature_names,
         )
+        df_train[target_name] = y
         if disable_caafe:
             self.code = ""
         else:
             self.code, prompt, messages = generate_features(
                 ds,
                 df_train,
                 model=self.llm_model,
@@ -91,40 +106,48 @@
             )
 
         df_train = run_llm_code(
             self.code,
             df_train,
         )
 
-        df_train, _ = make_datasets_numeric(
-            df_train, df_test=None, target_column=target_name
+        df_train, _, self.mappings = make_datasets_numeric(
+            df_train, df_test=None, target_column=target_name, return_mappings=True
         )
 
         df_train, y = split_target_column(df_train, target_name)
 
-        self.base_classifier.fit(df_train.values, y.values)
+        X, y = df_train.values, y.values.astype(int)
+        # Check that X and y have correct shape
+        X, y = check_X_y(X, y)
+
+        # Store the classes seen during fit
+        self.classes_ = unique_labels(y)
+
+        self.base_classifier.fit(X, y)
 
         # Return the classifier
         return self
 
     def predict_preprocess(self, X):
 
         # Check if fit has been called
         check_is_fitted(self)
 
         if type(X) != pd.DataFrame:
             X = pd.DataFrame(X, columns=self.X_.columns)
-
-        X = X[self.feature_names]
+        X, _ = split_target_column(X, self.target_name)
 
         X = run_llm_code(
             self.code,
             X,
         )
 
+        X = make_dataset_numeric(X, mappings=self.mappings)
+
         X = X.values
 
         # Input validation
         X = check_array(X)
 
         return X
```

### Comparing `caafe-0.1/caafe.egg-info/PKG-INFO` & `caafe-0.1.2/caafe.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1
+Version: 0.1.2
 Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
@@ -13,25 +13,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE.txt
 
 ### Usage
-Use this colab notebook for a quickstart.
+[![DEMO VIDEO](https://i.makeagif.com/media/5-20-2023/E4RfRM.gif)](https://www.youtube.com/watch?v=6zCD48d3kNU)
 
-Use CAFE_minimal.ipynb for a minimal example of how to use CAAFE on your dataset.
+CAAFE lets you semi-automate your feature engineering process based on your explanations on the dataset and with the help of language models. It is based on the paper "LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering" by Hollmann, Müller, and Hutter (2023).
+CAAFE systematically verifies the generated features to ensure that only features that are actually useful are added to the dataset.
 
-Use CAAFE.ipynb to reproduce the experiments from the paper.
+To use CAAFE, first create a CAAFEClassifier object with the desired parameters:
+```
+caafe_clf = CAAFEClassifier(base_classifier=clf_no_feat_eng,
+                      llm_model="gpt-4",
+                      iterations=2)
+```
+Then, fit the classifier to your training data:
+```
+caafe_clf.fit_pandas(df_train,
+               target_column_name=target_column_name,
+               dataset_description=dataset_description,
+              disable_caafe=False
+              )
+```
+Finally, use the classifier to make predictions on your test data:
+```
+pred = caafe_clf.predict(df_test)
+```
 
-#### Choosing an Iterative Classifier
-The iterative classifier gets called in each 
+You can also try out the demo at: https://colab.research.google.com/drive/1mCA8xOAJZ4MaB_alZvyARTMjhl6RZf0a
 
-### Access Tokens
-#### OpenAI
+For a minimal example of how to use CAAFE on your dataset, use CAFE_minimal.ipynb. To reproduce the experiments from the paper, use CAAFE.ipynb.
 
 
 ### Paper
 Hollmann, N., Müller, S., & Hutter, F. (2023). LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering
 https://arxiv.org/abs/2305.03403
 
 ### License
```

### Comparing `caafe-0.1/setup.py` & `caafe-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="caafe",
-    version="0.1",
+    version="0.1.2",
     packages=find_packages(),
     description="Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noah Hollmann, Samuel Müller, Frank Hutter",
     author_email="noah.homa@gmail.com",
     url="https://github.com/automl/CAAFE",
@@ -18,14 +18,14 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.7",
     install_requires=[
         "openai",
         "kaggle",
-        "openml==0.10.0",
+        "openml==0.12.0",
         "tabpfn",
     ],
     extras_require={
         "full": ["autofeat", "featuretools", "tabpfn[full]"],
     },
 )
```

