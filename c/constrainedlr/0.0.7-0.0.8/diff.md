# Comparing `tmp/constrainedlr-0.0.7.tar.gz` & `tmp/constrainedlr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.0.7.tar", last modified: Sun May 14 20:45:44 2023, max compression
+gzip compressed data, was "constrainedlr-0.0.8.tar", last modified: Sat May 20 18:13:49 2023, max compression
```

## Comparing `constrainedlr-0.0.7.tar` & `constrainedlr-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.530480 constrainedlr-0.0.7/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.7/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-14 20:45:44.524474 constrainedlr-0.0.7/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1167 2023-05-14 20:43:16.000000 constrainedlr-0.0.7/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-14 20:44:03.000000 constrainedlr-0.0.7/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-14 20:45:44.533475 constrainedlr-0.0.7/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:43.912477 constrainedlr-0.0.7/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.131481 constrainedlr-0.0.7/src/constrainedlr/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.7/src/constrainedlr/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3560 2023-05-14 20:17:25.000000 constrainedlr-0.0.7/src/constrainedlr/model.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.408478 constrainedlr-0.0.7/src/constrainedlr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.461486 constrainedlr-0.0.7/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3083 2023-05-14 20:41:10.000000 constrainedlr-0.0.7/tests/test_fit.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.407065 constrainedlr-0.0.8/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.8/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-20 18:13:50.401059 constrainedlr-0.0.8/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1167 2023-05-14 20:43:16.000000 constrainedlr-0.0.8/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-20 18:09:58.000000 constrainedlr-0.0.8/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-20 18:13:50.409064 constrainedlr-0.0.8/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:49.745575 constrainedlr-0.0.8/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.002060 constrainedlr-0.0.8/src/constrainedlr/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.8/src/constrainedlr/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3924 2023-05-20 18:08:03.000000 constrainedlr-0.0.8/src/constrainedlr/model.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.284064 constrainedlr-0.0.8/src/constrainedlr.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.345069 constrainedlr-0.0.8/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3611 2023-05-20 18:08:03.000000 constrainedlr-0.0.8/tests/test_fit.py
```

### Comparing `constrainedlr-0.0.7/LICENCE` & `constrainedlr-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.0.7/PKG-INFO` & `constrainedlr-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `constrainedlr-0.0.7/README.md` & `constrainedlr-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.0.7/pyproject.toml` & `constrainedlr-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.0.7'
+version = '0.0.8'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `constrainedlr-0.0.7/src/constrainedlr/model.py` & `constrainedlr-0.0.8/src/constrainedlr/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,31 @@
         self.intercept_ = None
         self.alpha = alpha
 
     def fit(
         self,
         X: pd.DataFrame,
         y: np.ndarray,
+        sample_weight: np.ndarray = None,
         features_sign_constraints: dict = {},
         intercept_sign_constraint: int = 0,
         features_sum_constraint_equal: float = None,
     ) -> "ConstrainedLinearRegression":
         """
         Fits a linear model with constraints
 
         X : pandas.DataFrame of shape (n_samples, n_features)
             Training data.
 
         y : numpy.ndarray of shape (n_samples,)
             Target values.
 
+        sample_weight : numpy.ndarray of shape (n_samples,), default=None
+            Individual weights for each sample.
+
         features_sign_constraints : dict
             Dictionary with sign constraints. Keys must be from X's columns and values must take the values: -1, 0, 1
             indicating negative, unconstrained and positive sign respectively. Any column that is not present in the
             dictionary will default to 0.
 
         intercept_sign_constraint : int
             Indicates the sign of intercept, if present, and must take the values: -1, 0, 1
@@ -49,17 +53,24 @@
 
         # Augment features to fit intercept
         if self.fit_intercept:
             X_ = np.hstack([X_, np.ones(n_samples).reshape(-1, 1)])
 
         dim = X_.shape[1]
 
-        P = X_.T.dot(X_) + self.alpha * np.eye(dim)
+        # Weight matrix
+        if sample_weight is None:
+            W = np.eye(n_samples)
+        else:
+            W = np.diag(sample_weight)
+
+        # Quadratic program
+        P = X_.T.dot(W).dot(X_) + self.alpha * np.eye(dim)
         P = matrix(P)
-        q = (-y_.T.dot(X_)).T
+        q = (-y_.T.dot(W).dot(X_)).T
         q = matrix(q)
 
         features_sign_constraints_full = {feature: 0 for feature in X.columns}
         features_sign_constraints_full.update(features_sign_constraints)
         diag_values = list(features_sign_constraints_full.values())
         if self.fit_intercept:
             diag_values.append(intercept_sign_constraint)
```

### Comparing `constrainedlr-0.0.7/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.0.8/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `constrainedlr-0.0.7/tests/test_fit.py` & `constrainedlr-0.0.8/tests/test_fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,7 +91,23 @@
     clr.fit(X, y)
 
     ridge = Ridge(fit_intercept=True, alpha=1.0)
     ridge.fit(X, y)
 
     assert np.allclose(ridge.intercept_, clr.intercept_, rtol=0.01)
     assert np.allclose(ridge.coef_, clr.coef_, rtol=0.01)
+
+
+def test_sample_weight():
+    # Perform multiple tests since sample weights are produced randomly
+    np.random.seed(0)
+    for _ in range(10):
+        sample_weight = np.random.random(X.shape[0]) * 10
+
+        clr = ConstrainedLinearRegression()
+        clr.fit(X, y, sample_weight=sample_weight)
+
+        lr = LinearRegression()
+        lr.fit(X, y, sample_weight=sample_weight)
+
+        assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
+        assert np.allclose(lr.coef_, clr.coef_, atol=atol)
```

