# Comparing `tmp/landmarkclassifier-2.0.2.tar.gz` & `tmp/landmarkclassifier-2.0.3.tar.gz`

## Comparing `landmarkclassifier-2.0.2.tar` & `landmarkclassifier-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/__init__.py
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/lm_base_clfs.py
--rw-r--r--   0        0        0    21923 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/tree.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/utils.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LANDMark/__init__.py
+-rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LANDMark/lm_base_clfs.py
+-rw-r--r--   0        0        0    23718 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LANDMark/tree.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LANDMark/utils.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/tests/test_landmark.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.3/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/.github/workflows/ci.yml` & `landmarkclassifier-2.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/.github/workflows/python-publish.yml` & `landmarkclassifier-2.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/LANDMark/LANDMark.py` & `landmarkclassifier-2.0.3/LANDMark/LANDMark.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,42 +14,44 @@
         self,
         n_estimators: int = 64,
         min_samples_in_leaf: int = 5,
         max_depth: int = -1,
         max_features: float = 0.80,
         min_gain: float = 0.0,
         impurity: str = "gain",
+        q: float = 1.5,
         use_oracle: bool = True,
         use_lm_l2: bool = True,
         use_lm_l1: bool = True,
         use_nnet: bool = True,
         nnet_min_samples: int = 32,
         use_etc: bool = True,
         etc_max_depth: int = 5,
         etc_max_trees: int = 128,
-        max_samples_tree: int = -1,
+        resampler = None,
         bootstrap: bool = False,
         n_jobs: int = 4,
     ):
         # Tree construction parameters
         self.n_estimators = n_estimators
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
         self.min_gain = min_gain
         self.impurity = impurity
+        self.q = q
         self.use_oracle = use_oracle
         self.use_lm_l2 = use_lm_l2
         self.use_lm_l1 = use_lm_l1
         self.use_nnet = use_nnet
         self.nnet_min_samples = nnet_min_samples
         self.use_etc = use_etc
         self.etc_max_depth = etc_max_depth
         self.etc_max_trees = etc_max_trees
-        self.max_samples_tree = max_samples_tree
+        self.resampler = resampler
         self.bootstrap = bootstrap
 
         self.n_jobs = n_jobs
 
     def fit(self, X: np.ndarray, y: np.ndarray) -> LANDMarkClassifier:
         """
         Parameters
@@ -68,25 +70,26 @@
         self.estimators_ = Ensemble(
             base_estimator=MTree(
                 min_samples_in_leaf=self.min_samples_in_leaf,
                 max_depth=self.max_depth,
                 max_features=self.max_features,
                 min_gain=self.min_gain,
                 impurity=self.impurity,
+                q = self.q,
                 use_oracle=self.use_oracle,
                 bootstrap=self.bootstrap,
                 use_lm_l2=self.use_lm_l2,
                 use_lm_l1=self.use_lm_l1,
                 use_nnet=self.use_nnet,
                 nnet_min_samples=self.nnet_min_samples,
                 use_etc=self.use_etc,
                 etc_max_depth=self.etc_max_depth,
                 etc_max_trees=self.etc_max_trees,
             ),
-            max_samples_tree=self.max_samples_tree,
+            resampler=self.resampler,
             n_estimators=self.n_estimators,
             class_names=self.classes_,
             n_jobs=self.n_jobs,
         )
 
         self.estimators_.fit(X, y)
```

### Comparing `landmarkclassifier-2.0.2/LANDMark/lm_base_clfs.py` & `landmarkclassifier-2.0.3/LANDMark/lm_base_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/LANDMark/tree.py` & `landmarkclassifier-2.0.3/LANDMark/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,86 @@
     LMClassifier,
     RandomOracle,
     ANNClassifier,
     ETClassifier,
 )
 
 
-def purity_function(N, N_lab, L, R, y, purity_fun="gain"):
-    # Calculate Information Gain
-    if purity_fun == "gain":
-        L_outcome, L_counts = np.unique(y[L], return_counts=True)
-        L_prob = L_counts / L_counts.sum()
-        H_L = entropy(L_prob) * (L_counts.sum() / N)
-
-        R_outcome, R_counts = np.unique(y[R], return_counts=True)
-        R_prob = R_counts / R_counts.sum()
-        H_R = entropy(R_prob) * (R_counts.sum() / N)
+def tsallis_fun(N, N_lab, L, R, y, mode, q):
 
-        H_parent = entropy(N_lab)
+    if q == 1: #Special case
+        if "ratio" in mode.split("-"):
+            return entropy_fun(N, N_lab, L, R, y, "gain-ratio")
+
+        else:
+            return entropy_fun(N, N_lab, L, R, y, "gain")
+
+    scaler = 1 / (1 - q)
+
+    L_outcome, L_counts = np.unique(y[L], return_counts=True)
+    L_prob = L_counts / L_counts.sum()
+    H_L = (L_counts.sum() / N) * (scaler * (np.power(L_prob, q).sum() - 1))
+
+    R_outcome, R_counts = np.unique(y[R], return_counts=True)
+    R_prob = R_counts / R_counts.sum()
+    H_R = (R_counts.sum() / N) * (scaler * (np.power(R_prob, q).sum() - 1))
+
+    H_parent = scaler * (np.power(N_lab, q).sum() - 1)
+
+    IG = H_parent - H_R - H_L
+
+    if mode == "tsallis":
+
+        return IG
+
+    else:
+        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
+        norm_factor = 1 + (scaler * (np.power(norm_factor, q).sum() - 1))
+    
+        GR = IG / norm_factor
+
+        return GR
 
-        IG = H_parent - H_L - H_R
+
+def entropy_fun(N, N_lab, L, R, y, mode):
+    L_outcome, L_counts = np.unique(y[L], return_counts=True)
+    L_prob = L_counts / L_counts.sum()
+    H_L = entropy(L_prob) * (L_counts.sum() / N)
+
+    R_outcome, R_counts = np.unique(y[R], return_counts=True)
+    R_prob = R_counts / R_counts.sum()
+    H_R = entropy(R_prob) * (R_counts.sum() / N)
+
+    H_parent = entropy(N_lab)
+
+    IG = H_parent - H_L - H_R
+
+    if mode == "gain":
 
         return IG
 
+    else:
+        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
+        norm_factor = 1 + entropy(norm_factor)
+    
+        GR = IG / norm_factor
+
+        return GR
+
+
+def purity_function(N, N_lab, L, R, y, purity_fun, q):
+    
+    if purity_fun == "gain" or purity_fun == "gain-ratio":
+
+        return entropy_fun(N, N_lab, L, R, y, purity_fun)
+
+    elif purity_fun == "tsallis-gain-ratio" or purity_fun == "tsallis":
+
+        return tsallis_fun(N, N_lab, L, R, y, purity_fun, q)
+
 
 class PredictData:
     def __init__(self, node_lab):
         self.node_lab = node_lab
 
     def predict(self, X):
         predictions = np.asarray([self.node_lab for i in range(X.shape[0])])
@@ -68,14 +123,15 @@
                   X,
                   y,
                   min_samples_in_leaf,
                   max_depth,
                   max_features,
                   min_gain,
                   impurity,
+                  q,
                   use_lm_l2,
                   use_lm_l1,
                   use_nnet,
                   nnet_min_samples,
                   use_etc,
                   etc_max_depth,
                   etc_max_trees,
@@ -119,26 +175,27 @@
                 self.splitter = RandomOracle(n_feat=max_features).fit(X, y)
 
                 D = self.splitter.decision_function(X)
 
                 L = np.where(D > 0, True, False)
                 R = np.where(D <= 0, True, False)
 
-                IG = purity_function(counts_sum, counts_prob, L, R, y, impurity)
+                IG = purity_function(counts_sum, counts_prob, L, R, y, impurity, q)
 
                 self.gain = IG
 
                 # Recursivly split
                 self.left = Node().get_split(X[L], 
                                                  y[L],
                                                  min_samples_in_leaf = min_samples_in_leaf,
                                                  max_depth = max_depth,
                                                  max_features = max_features,
                                                  min_gain = min_gain,
                                                  impurity = impurity,
+                                                 q = q,
                                                  use_lm_l2 = use_lm_l2,
                                                  use_lm_l1 = use_lm_l1,
                                                  use_nnet = use_nnet,
                                                  nnet_min_samples = nnet_min_samples,
                                                  use_etc = use_etc,
                                                  etc_max_depth = etc_max_depth,
                                                  etc_max_trees = etc_max_trees,
@@ -149,14 +206,15 @@
                 self.right = Node().get_split(X[R], 
                                                   y[R],
                                                   min_samples_in_leaf = min_samples_in_leaf,
                                                   max_depth = max_depth,
                                                   max_features = max_features,
                                                   min_gain = min_gain,
                                                   impurity = impurity,
+                                                  q = q,
                                                   use_lm_l2 = use_lm_l2,
                                                   use_lm_l1 = use_lm_l1,
                                                   use_nnet = use_nnet,
                                                   nnet_min_samples = nnet_min_samples,
                                                   use_etc = use_etc,
                                                   etc_max_depth = etc_max_depth,
                                                   etc_max_trees = etc_max_trees,
@@ -188,15 +246,15 @@
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity
+                                counts_sum, counts_prob, L, R, y, impurity, q
                             )
 
                             gains.append(IG)
                             hyperplane_list.append((model, L, R))
                             model_type.append(model.model_type)
 
                 # Train Linear Models - L1 / ElasticNet
@@ -215,15 +273,15 @@
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity
+                                counts_sum, counts_prob, L, R, y, impurity, q
                             )
 
                             gains.append(IG)
                             hyperplane_list.append((model, L, R))
                             model_type.append(model.model_type)
 
                 # Train a Neural Network
@@ -240,15 +298,15 @@
 
                             X_L_n = X[L].shape[0]
                             X_R_n = X[R].shape[0]
 
                             # Calculate Information Gain
                             if X_L_n > 0 and X_R_n > 0:
                                 IG = purity_function(
-                                    counts_sum, counts_prob, L, R, y, impurity
+                                    counts_sum, counts_prob, L, R, y, impurity, q
                                 )
 
                                 gains.append(IG)
                                 hyperplane_list.append((model, L, R))
                                 model_type.append(model.model_type)
 
                 # Train Decision Tree Models
@@ -270,15 +328,15 @@
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
-                                counts_sum, counts_prob, L, R, y, impurity
+                                counts_sum, counts_prob, L, R, y, impurity, q
                             )
 
                             gains.append(IG)
                             hyperplane_list.append((model, L, R))
                             model_type.append(model.model_type)
 
                 gains = np.asarray(gains)
@@ -308,14 +366,15 @@
                     self.left = Node().get_split(X[L], 
                                                  y[L],
                                                  min_samples_in_leaf = min_samples_in_leaf,
                                                  max_depth = max_depth,
                                                  max_features = max_features,
                                                  min_gain = min_gain,
                                                  impurity = impurity,
+                                                 q = q,
                                                  use_lm_l2 = use_lm_l2,
                                                  use_lm_l1 = use_lm_l1,
                                                  use_nnet = use_nnet,
                                                  nnet_min_samples = nnet_min_samples,
                                                  use_etc = use_etc,
                                                  etc_max_depth = etc_max_depth,
                                                  etc_max_trees = etc_max_trees,
@@ -326,14 +385,15 @@
                     self.right = Node().get_split(X[R], 
                                                   y[R],
                                                   min_samples_in_leaf = min_samples_in_leaf,
                                                   max_depth = max_depth,
                                                   max_features = max_features,
                                                   min_gain = min_gain,
                                                   impurity = impurity,
+                                                  q = q,
                                                   use_lm_l2 = use_lm_l2,
                                                   use_lm_l1 = use_lm_l1,
                                                   use_nnet = use_nnet,
                                                   nnet_min_samples = nnet_min_samples,
                                                   use_etc = use_etc,
                                                   etc_max_depth = etc_max_depth,
                                                   etc_max_trees = etc_max_trees,
@@ -357,14 +417,15 @@
     def __init__(
         self,
         min_samples_in_leaf,
         max_depth,
         max_features,
         min_gain,
         impurity,
+        q,
         use_oracle,
         bootstrap,
         use_lm_l2,
         use_lm_l1,
         use_nnet,
         nnet_min_samples,
         use_etc,
@@ -372,14 +433,15 @@
         etc_max_trees,
     ):
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
         self.min_gain = min_gain
         self.impurity = impurity
+        self.q = q
         self.use_oracle = use_oracle
         self.bootstrap = bootstrap
         self.use_lm_l2 = use_lm_l2
         self.use_lm_l1 = use_lm_l1
         self.use_nnet = use_nnet
         self.nnet_min_samples = nnet_min_samples
         self.use_etc = use_etc
@@ -404,14 +466,15 @@
         tree.get_split(X=X_re, 
                        y=y_re,
                        min_samples_in_leaf = self.min_samples_in_leaf,
                        max_depth = self.max_depth,
                        max_features = self.max_features,
                        min_gain = self.min_gain,
                        impurity = self.impurity,
+                       q = self.q,
                        use_lm_l2 = self.use_lm_l2,
                        use_lm_l1 = self.use_lm_l1,
                        use_nnet = self.use_nnet,
                        nnet_min_samples = self.nnet_min_samples,
                        use_etc = self.use_etc,
                        etc_max_depth = self.etc_max_depth,
                        etc_max_trees = self.etc_max_trees,
```

### Comparing `landmarkclassifier-2.0.2/LANDMark/utils.py` & `landmarkclassifier-2.0.3/LANDMark/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 import numpy as np
 
 ##########################################################################################
 # For Bagging Classifier
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
-from sklearn.utils import resample
 from scipy.special import softmax
 from joblib import Parallel, delayed, parallel_backend
 
 
-def _parallel_build(estimator, X, y, max_samples_tree):
-    if X.shape[0] <= max_samples_tree or max_samples_tree == -1:
+def _parallel_build(estimator, X, y, resampler):
+    if isinstance(resampler, type(None)):
         X_trf = X
         y_trf = y
 
     else:
-        X_trf, y_trf = resample(
-            X, y, replace=True, n_samples=max_samples_tree, stratify=y
-        )
+        X_trf, y_trf = clone(resampler).fit_resample(X, y)
 
     trained_estimator = estimator.fit(X_trf, y_trf)
 
     return trained_estimator
 
 
 class Ensemble(ClassifierMixin, BaseEstimator):
     def __init__(
-        self, base_estimator, max_samples_tree, n_estimators, class_names, n_jobs
+        self, base_estimator, resampler, n_estimators, class_names, n_jobs
     ):
         self.base_estimator = base_estimator
-        self.max_samples_tree = max_samples_tree
+        self.resampler = resampler
         self.n_estimators = n_estimators
         self.classes_ = class_names
         self.n_jobs = n_jobs
 
     def fit(self, X, y):
 
         self.estimators_ = Parallel(n_jobs=self.n_jobs)(
             delayed(_parallel_build)(
-                clone(self.base_estimator), X, y, self.max_samples_tree
+                clone(self.base_estimator), X, y, self.resampler
             )
             for i in range(self.n_estimators)
         )
 
         return self
 
     def predict(self, X):
@@ -94,14 +91,15 @@
         #Ensure all probabilities sum to one
         prediction_probs = softmax(prediction_probs, axis = 1)
 
         return prediction_probs
 
 
 ##########################################################################################
+# For Neural Network Models
 import tensorflow as tf
 import keras.backend as K
 
 
 def get_centralized_gradients(optimizer, loss, params):
     """Compute the centralized gradients.
```

### Comparing `landmarkclassifier-2.0.2/docs/API.md` & `landmarkclassifier-2.0.3/docs/API.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/docs/CONTRIBUTING.md` & `landmarkclassifier-2.0.3/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/tests/test_landmark.py` & `landmarkclassifier-2.0.3/tests/test_landmark.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/.gitignore` & `landmarkclassifier-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/LICENSE` & `landmarkclassifier-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/README.md` & `landmarkclassifier-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.2/pyproject.toml` & `landmarkclassifier-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
@@ -63,11 +63,11 @@
     "pytest-cov"
 ]
 
 [tool.setuptools]
 py-modules = ["LANDMark"]
 
 [tool.pytest.ini_options]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 40"
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 30"
 
 [tool.coverage.run]
 source = ["LANDMark"]
```

### Comparing `landmarkclassifier-2.0.2/PKG-INFO` & `landmarkclassifier-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.2
+Version: 2.0.3
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
```

