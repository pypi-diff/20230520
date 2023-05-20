# Comparing `tmp/scpi_pkg-2.2.2.tar.gz` & `tmp/scpi_pkg-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpi_pkg-2.2.2.tar", last modified: Wed Apr 19 17:17:01 2023, max compression
+gzip compressed data, was "scpi_pkg-2.2.3.tar", last modified: Sat May 20 00:54:44 2023, max compression
```

## Comparing `scpi_pkg-2.2.2.tar` & `scpi_pkg-2.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090963 scpi_pkg-2.2.2/
--rw-r--r--   0 fpalomba   (501) staff       (20)     1091 2021-11-18 19:45:12.000000 scpi_pkg-2.2.2/LICENSE
--rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-04-19 17:17:01.091024 scpi_pkg-2.2.2/PKG-INFO
--rw-r--r--   0 fpalomba   (501) staff       (20)     1887 2022-09-08 01:12:37.000000 scpi_pkg-2.2.2/README.md
--rw-r--r--   0 fpalomba   (501) staff       (20)      112 2022-03-01 16:03:56.000000 scpi_pkg-2.2.2/pyproject.toml
--rw-r--r--   0 fpalomba   (501) staff       (20)      964 2023-04-19 17:17:01.091293 scpi_pkg-2.2.2/setup.cfg
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.085061 scpi_pkg-2.2.2/src/
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090233 scpi_pkg-2.2.2/src/scpi_pkg/
--rw-r--r--   0 fpalomba   (501) staff       (20)        0 2021-11-18 15:59:04.000000 scpi_pkg-2.2.2/src/scpi_pkg/__init__.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    53510 2023-04-19 16:23:42.000000 scpi_pkg-2.2.2/src/scpi_pkg/funs.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    33356 2023-01-25 05:32:28.000000 scpi_pkg-2.2.2/src/scpi_pkg/scdata.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    35558 2023-01-25 05:37:18.000000 scpi_pkg-2.2.2/src/scpi_pkg/scdataMulti.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    32014 2023-03-13 23:34:41.000000 scpi_pkg-2.2.2/src/scpi_pkg/scest.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    79417 2023-03-14 19:15:00.000000 scpi_pkg-2.2.2/src/scpi_pkg/scpi.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    12752 2022-11-20 15:18:05.000000 scpi_pkg-2.2.2/src/scpi_pkg/scplot.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    29802 2023-01-25 21:32:03.000000 scpi_pkg-2.2.2/src/scpi_pkg/scplotMulti.py
--rw-r--r--   0 fpalomba   (501) staff       (20)       23 2023-03-14 19:25:03.000000 scpi_pkg-2.2.2/src/scpi_pkg/version.py
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090854 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/
--rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/PKG-INFO
--rw-r--r--   0 fpalomba   (501) staff       (20)      436 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)        1 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)      155 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/requires.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)        9 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-05-20 00:54:44.969693 scpi_pkg-2.2.3/
+-rw-r--r--   0 fpalomba   (501) staff       (20)     1091 2021-11-18 19:45:12.000000 scpi_pkg-2.2.3/LICENSE
+-rw-r--r--   0 fpalomba   (501) staff       (20)     2447 2023-05-20 00:54:44.969751 scpi_pkg-2.2.3/PKG-INFO
+-rw-r--r--   0 fpalomba   (501) staff       (20)     1842 2023-04-19 17:36:38.000000 scpi_pkg-2.2.3/README.md
+-rw-r--r--   0 fpalomba   (501) staff       (20)      112 2022-03-01 16:03:56.000000 scpi_pkg-2.2.3/pyproject.toml
+-rw-r--r--   0 fpalomba   (501) staff       (20)      964 2023-05-20 00:54:44.970022 scpi_pkg-2.2.3/setup.cfg
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-05-20 00:54:44.964541 scpi_pkg-2.2.3/src/
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-05-20 00:54:44.968934 scpi_pkg-2.2.3/src/scpi_pkg/
+-rw-r--r--   0 fpalomba   (501) staff       (20)        0 2021-11-18 15:59:04.000000 scpi_pkg-2.2.3/src/scpi_pkg/__init__.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    54524 2023-05-18 19:54:51.000000 scpi_pkg-2.2.3/src/scpi_pkg/funs.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    33280 2023-04-19 20:21:45.000000 scpi_pkg-2.2.3/src/scpi_pkg/scdata.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    35494 2023-04-19 22:26:23.000000 scpi_pkg-2.2.3/src/scpi_pkg/scdataMulti.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    32458 2023-05-18 18:39:31.000000 scpi_pkg-2.2.3/src/scpi_pkg/scest.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    79811 2023-05-18 19:54:25.000000 scpi_pkg-2.2.3/src/scpi_pkg/scpi.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    12681 2023-04-19 22:15:50.000000 scpi_pkg-2.2.3/src/scpi_pkg/scplot.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    29729 2023-04-19 22:15:57.000000 scpi_pkg-2.2.3/src/scpi_pkg/scplotMulti.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)       23 2023-04-20 20:45:05.000000 scpi_pkg-2.2.3/src/scpi_pkg/version.py
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-05-20 00:54:44.969566 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/
+-rw-r--r--   0 fpalomba   (501) staff       (20)     2447 2023-05-20 00:54:44.000000 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 fpalomba   (501) staff       (20)      436 2023-05-20 00:54:44.000000 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)        1 2023-05-20 00:54:44.000000 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)      155 2023-05-20 00:54:44.000000 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/requires.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)        9 2023-05-20 00:54:44.000000 scpi_pkg-2.2.3/src/scpi_pkg.egg-info/top_level.txt
```

### Comparing `scpi_pkg-2.2.2/LICENSE` & `scpi_pkg-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.2/PKG-INFO` & `scpi_pkg-2.2.3/src/scpi_pkg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scpi_pkg
-Version: 2.2.2
+Name: scpi-pkg
+Version: 2.2.3
 Summary: The package computes point estimates and prediction intervals for Synthetic Control methods as proposed in Cattaneo, Feng, and Titiunik (2021).
 Home-page: https://nppackages.github.io/scpi/
 Author: Filippo Palomba
 Author-email: fpalomba@princeton.edu
 Project-URL: Bug Tracker, https://nppackages.github.io/scpi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCPI_PKG
 
 The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
 
-
 ## Authors
- 
+
 Matias D. Cattaneo (<cattaneo@princeton.edu>)
 
 Yingjie Feng (<fengyj@sem.tsinghua.edu.cn>)
 
 Filippo Palomba (<fpalomba@princeton.edu>)
 
 Rocio Titiunik (<titiunik@princeton.edu>)
@@ -31,52 +30,53 @@
 ## Website
 
 https://nppackages.github.io/scpi/
 
 ## Installation
 
 To install/update use pip
+
 ```
 pip install scpi_pkg
 ```
 
 # Usage
+
 ```
 from from scpi_pkg.scdata import scdata
 from from scpi_pkg.scdataMulti import scdataMulti
 from scpi_pkg.scest import scest
 from scpi_pkg.scpi import scpi
 from scpi_pkg.scplot import scplot
 from scpi_pkg.scplotMulti import scplotMulti
 ```
 
 - Replication: [Germany reunification example](https://github.com/nppackages/scpi/blob/main/Python/scpi_illustration.py).
 
 ## Dependencies
 
-- cvxpy           (>= 1.1.18)
+- cvxpy          (>= 1.1.18)
 - dask            (>= 2021.04.0)
-- nlopt           (>= 2.7.0)
-- numpy           (>= 1.20.1)
-- pandas          (>= 1.2.4)
-- plotnine        (>= 0.8.0)
-- scikit-learn    (>= 0.24.1)
-- scipy           (>= 1.7.1)
-- statsmodels     (>= 0.12.2)
+- ecos            (>= 2.0.7)
+- luddite         (>= 1.0.2)
+- numpy         (>= 1.20.1)
+- pandas        (>= 1.5.0)
+- plotnine       (>= 0.8.0)
+- scikit-learn  (>= 0.24.1)
+- scipy            (>= 1.7.1)
+- statsmodels (>= 0.12.2)
 
 ## References
 
 For overviews and introductions, see [nppackages website](https://nppackages.github.io/).
 
 ### Software and Implementation
 
 - Cattaneo, Feng, Palomba, and Titiunik (2022) [scpi: Uncertainty Quantification for Synthetic Control Estimators](https://arxiv.org/abs/2202.05984).
 
-
 ### Technical and Methodological
 
-- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).<br>
-_Journal of the American Statistical Association_.
-
+- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).`<br>`
+  _Journal of the American Statistical Association_.
 - Cattaneo, Feng, Palomba, and Titiunik (2022): Uncertainty Quantification in Synthetic Controls with Staggered Treatment Adoption, working paper.
 
-<br><br>
+`<br><br>`
```

### Comparing `scpi_pkg-2.2.2/README.md` & `scpi_pkg-2.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# SCPI_PKG
-
-The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
-
-
-## Authors
- 
-Matias D. Cattaneo (<cattaneo@princeton.edu>)
-
-Yingjie Feng (<fengyj@sem.tsinghua.edu.cn>)
-
-Filippo Palomba (<fpalomba@princeton.edu>)
-
-Rocio Titiunik (<titiunik@princeton.edu>)
-
-## Website
-
-https://nppackages.github.io/scpi/
-
-## Installation
-
-To install/update use pip
-```
-pip install scpi_pkg
-```
-
-# Usage
-```
-from from scpi_pkg.scdata import scdata
-from from scpi_pkg.scdataMulti import scdataMulti
-from scpi_pkg.scest import scest
-from scpi_pkg.scpi import scpi
-from scpi_pkg.scplot import scplot
-from scpi_pkg.scplotMulti import scplotMulti
-```
-
-- Replication: [Germany reunification example](https://github.com/nppackages/scpi/blob/main/Python/scpi_illustration.py).
-
-## Dependencies
-
-- cvxpy           (>= 1.1.18)
-- dask            (>= 2021.04.0)
-- nlopt           (>= 2.7.0)
-- numpy           (>= 1.20.1)
-- pandas          (>= 1.2.4)
-- plotnine        (>= 0.8.0)
-- scikit-learn    (>= 0.24.1)
-- scipy           (>= 1.7.1)
-- statsmodels     (>= 0.12.2)
-
-## References
-
-For overviews and introductions, see [nppackages website](https://nppackages.github.io/).
-
-### Software and Implementation
-
-- Cattaneo, Feng, Palomba, and Titiunik (2022) [scpi: Uncertainty Quantification for Synthetic Control Estimators](https://arxiv.org/abs/2202.05984).
-
-
-### Technical and Methodological
-
-- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).<br>
-_Journal of the American Statistical Association_.
-
-- Cattaneo, Feng, Palomba, and Titiunik (2022): Uncertainty Quantification in Synthetic Controls with Staggered Treatment Adoption, working paper.
-
-<br><br>
+# SCPI_PKG
+
+The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
+
+## Authors
+
+Matias D. Cattaneo (<cattaneo@princeton.edu>)
+
+Yingjie Feng (<fengyj@sem.tsinghua.edu.cn>)
+
+Filippo Palomba (<fpalomba@princeton.edu>)
+
+Rocio Titiunik (<titiunik@princeton.edu>)
+
+## Website
+
+https://nppackages.github.io/scpi/
+
+## Installation
+
+To install/update use pip
+
+```
+pip install scpi_pkg
+```
+
+# Usage
+
+```
+from from scpi_pkg.scdata import scdata
+from from scpi_pkg.scdataMulti import scdataMulti
+from scpi_pkg.scest import scest
+from scpi_pkg.scpi import scpi
+from scpi_pkg.scplot import scplot
+from scpi_pkg.scplotMulti import scplotMulti
+```
+
+- Replication: [Germany reunification example](https://github.com/nppackages/scpi/blob/main/Python/scpi_illustration.py).
+
+## Dependencies
+
+- cvxpy          (>= 1.1.18)
+- dask            (>= 2021.04.0)
+- ecos            (>= 2.0.7)
+- luddite         (>= 1.0.2)
+- numpy         (>= 1.20.1)
+- pandas        (>= 1.5.0)
+- plotnine       (>= 0.8.0)
+- scikit-learn  (>= 0.24.1)
+- scipy            (>= 1.7.1)
+- statsmodels (>= 0.12.2)
+
+## References
+
+For overviews and introductions, see [nppackages website](https://nppackages.github.io/).
+
+### Software and Implementation
+
+- Cattaneo, Feng, Palomba, and Titiunik (2022) [scpi: Uncertainty Quantification for Synthetic Control Estimators](https://arxiv.org/abs/2202.05984).
+
+### Technical and Methodological
+
+- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).`<br>`
+  _Journal of the American Statistical Association_.
+- Cattaneo, Feng, Palomba, and Titiunik (2022): Uncertainty Quantification in Synthetic Controls with Staggered Treatment Adoption, working paper.
+
+`<br><br>`
```

### Comparing `scpi_pkg-2.2.2/setup.cfg` & `scpi_pkg-2.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/funs.py` & `scpi_pkg-2.2.3/src/scpi_pkg/funs.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,24 +431,27 @@
             constraints = [cvxpy.sum_squares(x[0:J]) <= cvxpy.power(w_constr['Q'], 2)]
 
     elif p == "L1-L2":
         constraints = [cvxpy.sum(x[0:J]) == w_constr['Q'], x[0:J] >= lb,
                        cvxpy.sum_squares(x[0:J]) <= cvxpy.power(w_constr['Q2'], 2)]
 
     prob = cvxpy.Problem(objective, constraints)
-    prob.solve()
 
+    if w_constr['name'] == 'lasso' or (p == "L1" and dire == "<="):
+        prob.solve(solver=cvxpy.OSQP)
+    else:
+        prob.solve(solver=cvxpy.ECOS)
     b = x.value
     alert = prob.status != 'optimal'
 
     if alert is True:
         raise Exception("Estimation algorithm not converged! The algorithm returned the value: " +
                         str(prob.status) + ". To check to what errors it corresponds" +
                         "go to 'https://www.cvxpy.org/tutorial/intro/index.html'. " +
-                        " Typically, this occurs because the problem is badly-scaled." +
+                        "Typically, this occurs because the problem is badly-scaled." +
                         "If so, scaling the data fixes the issue.")
 
     return b
 
 def b_est_multi(A, Z, J, KM, iota, w_constr, V):
 
     lb = w_constr[0]['lb']
@@ -496,15 +499,18 @@
         elif p == "L1-L2":
             constraints.append(cvxpy.sum(x[j_lb:j_ub]) == QQ[i])
             constraints.append(cvxpy.sum_squares(x[j_lb:j_ub]) <= QQ2[i] ** 2)
 
         j_lb = j_ub
 
     prob = cvxpy.Problem(objective, constraints)
-    prob.solve()
+    if w_constr[0]['name'] == 'lasso' or (p == "L1" and dire == "<="):
+        prob.solve(solver=cvxpy.OSQP)
+    else:
+        prob.solve(solver=cvxpy.ECOS)
 
     b = x.value
     alert = prob.status != 'optimal'
 
     if alert is True:
         raise Exception("Estimation algorithm not converged! The algorithm returned the value: " +
                         str(prob.status) + ". To check to what errors it corresponds" +
@@ -639,15 +645,18 @@
 
         # Construct the polynomial terms in B (e.des.0) and P (e.des.1)
         if e_order == 0:       # Simple mean
             ix = pandas.MultiIndex.from_product([[outcome_var], B.loc[(outcome_var,), :].index.tolist()])
             ix.rename(["feature", "Time"], inplace=True)
 
             e_des_0 = pandas.DataFrame(numpy.ones(T0), index=ix)
-            e_des_1 = pandas.DataFrame(numpy.ones(T1), index=P.index)
+            if effect == "time":
+                e_des_1 = pandas.DataFrame(numpy.ones(T1) / iota, index=P.index)
+            else:
+                e_des_1 = pandas.DataFrame(numpy.ones(T1), index=P.index)
 
         elif e_order > 0:  # Include covariates when predicting u_mean
             # Create first differences feature-by-feature of the matrix B (not of C!!)
             if coig_data is True:
                 B_diff = B - B.groupby('feature').shift(1)
                 e_des_0 = pandas.concat([B_diff, C], axis=1).loc[:, index]
 
@@ -664,16 +673,20 @@
             elif coig_data is False:
                 e_des_0 = Z.loc[:, index]
                 e_des_1 = P.loc[:, index]
 
             if constant is False:
                 e_des_0.insert(loc=len(e_des_0.columns), column='0_constant',
                                value=numpy.ones(len(e_des_0)))
-                e_des_1.insert(loc=len(e_des_1.columns), column='0_constant',
-                               value=numpy.ones(len(e_des_1)))
+                if effect == "time":
+                    e_des_1.insert(loc=len(e_des_1.columns), column='0_constant',
+                                   value=numpy.ones(len(e_des_1)) / iota)
+                else:
+                    e_des_1.insert(loc=len(e_des_1.columns), column='0_constant',
+                                   value=numpy.ones(len(e_des_1)))
 
         nolag = False
 
         if P_diff_pre is not None:
             e_des_1 = P_diff_pre.loc[:, index]
             nolag = True
 
@@ -964,15 +977,15 @@
 
         if verbose:
             print("")
             print("Closing working clusters...")
 
     return vsig
 
-def scpi_out(y, x, preds, e_method, alpha, e_lb_est, e_ub_est, effect):
+def scpi_out(y, x, preds, e_method, alpha, e_lb_est, e_ub_est, effect, out_feat):
     e_1 = e_2 = None
     idx = preds.index
     y = deepcopy(numpy.array(y))[:, 0]
     x = deepcopy(numpy.array(x))
     preds = deepcopy(numpy.array(preds))
 
     if e_lb_est is True or e_ub_est is True:
@@ -1078,30 +1091,37 @@
 
         if effect == "time":
             idx = idx.unique('Time')
 
         lb = pandas.DataFrame(lb, index=idx)
         ub = pandas.DataFrame(ub, index=idx)
 
+        # if model is heavily misspecified just give up on out-of-sample uncertainty
+        if out_feat is False:
+            if any(lb[0] > 0):
+                lb = pandas.DataFrame([lb.min()] * len(lb), index=idx)
+            if any(ub[0] < 0):
+                ub = pandas.DataFrame([ub.max()] * len(ub), index=idx)
+
     else:
         lb = None
         ub = None
 
     return lb, ub, e_1, e_2
 
 
 def simultaneousPredGet(vsig, T1, T1_tot, iota, u_alpha, e_alpha, e_res_na, e_des_0_na,
-                        e_des_1, w_lb_est, w_ub_est, w_bounds, w_name, effect):
+                        e_des_1, w_lb_est, w_ub_est, w_bounds, w_name, effect, out_feat):
 
     vsigLB = vsig[:, :T1_tot]
     vsigUB = vsig[:, T1_tot:]
 
     e_lb, e_ub, e_1, e_2 = scpi_out(y=e_res_na, x=e_des_0_na, preds=e_des_1,
                                     e_method="gaussian", alpha=e_alpha / 2,
-                                    e_lb_est=True, e_ub_est=True, effect=effect)
+                                    e_lb_est=True, e_ub_est=True, effect=effect, out_feat=out_feat)
 
     jmin = 0
     w_lb_joint = []
     w_ub_joint = []
     for i in range(iota):
         jmax = T1[i] + jmin
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scdata.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 16 09:59:24 2021
 
-@author: Filippo Palomba
-"""
 # Temporary code to suppress pandas FutureWarning
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import pandas
 pandas.options.mode.chained_assignment = None
 import pandas
@@ -37,41 +33,41 @@
     """
     Parameters
     ----------
     df : pandas.DataFrame
         a dataframe object containing the data to be processed
 
     id_var : str
-        a character with the name of the variable containing units' IDs
+        a character with the name of the variable containing units IDs
 
     time_var : str
         a character with the name of the time variable. The time variable has to be numpy.int64 or
         numpy.datetime64. Input a numeric time variable is suggested when working with
         yearly data, whereas for all other frequencies numpy.datetime64 type is preferred.
 
     outcome_var : str
         a character with the name of the outcome variable. The outcome variable has to be numeric.
 
     period_pre : array
         a numeric vector that identifies the pre-treatment period in time_var.
 
     period_post : array
-         a numeric vector that identifies the post-treatment period in time_var.
+        a numeric vector that identifies the post-treatment period in time_var.
 
     unit_tr : int
-         a scalar that identifies the treated unit in id_var.
+        a scalar that identifies the treated unit in id_var.
 
     unit_co : array
          a numeric vector that identifies the donor pool in id_var.
 
     features : list, default None
-         a character list containing the name of the feature variables used for estimation.
+        a character list containing the name of the feature variables used for estimation.
         If this option is not specified the default is features = outcome_var.
 
-     cov_adj : list, default None
+    cov_adj : list, default None
         a list specifying the names of the covariates to be used for adjustment for each feature. If the user wants
         to specify the same set of covariates for all features, a single list should be provided. If instead a
         different set of covariates per feature has to be specified, then a list of lists should be provided. Note that
         in this latter case the number of sub-lists must be equal to the number of features. Moreover, the order of the
         sub-lists matters, in the sense that the first sub-list is interpreted as the set of covariates for the first
         feature, and so on. Finally, the user can specify 'constant' and 'trend' as covariates even if they are not
         present in the loaded dataframe.
@@ -90,15 +86,15 @@
         a logical to print additional information in the console.
 
     report_missing : bool, default False
         a logical which prints the location of missing values if present. The default value is False.
 
     Returns
     -------
-    The function returns an object of class `scdata_output' containing the following objects
+    The function returns an object of class 'scdata_output' containing the following objects
 
     A : pandas.DataFrame
         a dataframe containing pre-treatment features of the treated unit.
 
     B : pandas.DataFrame
         a dataframe containing pre-treatment features of the control units.
 
@@ -174,14 +170,15 @@
     Controls with Staggered Treatment Adoption”.
 
     See Also
     --------
     scdataMulti, scest, scpi, scplot, scplotMulti
 
     """
+
     # Check main input is a dataframe
     if not isinstance(df, pandas.DataFrame):
         raise Exception('Data input should be a dataframe object!')
 
     data = deepcopy(df)
 
     # Store variable names and indexes
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scdataMulti.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scdataMulti.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Mar  7 15:47:09 2022
 
-@author: ux310uq-gl443t
-"""
 # Temporary code to suppress pandas FutureWarning
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import pandas
 pandas.options.mode.chained_assignment = None
 import pandas
@@ -114,15 +110,15 @@
         a scalar that indicates the number of periods of potential anticipation effects. If the user wants to specify
         this option indipendently for each treated unit, a dictionary must be provided instead of an integer value.
         Specifically, the dictionary must contain as many keys as the number of treated units in the data.
         Each key must correspond to the identifier (id_var) of one treated unit.
 
     Returns
     -------
-    The function returns an object of class `scdata_output' containing the following objects
+    The function returns an object of class 'scdata_output' containing the following objects
 
     A : pandas.DataFrame
         a dataframe containing pre-treatment features of the treated units.
 
     B : pandas.DataFrame
         a dataframe containing pre-treatment features of the control units.
 
@@ -133,19 +129,19 @@
         a dataframe whose rows are the vectors used to predict the out-of-sample series for the synthetic units.
 
     Y_df : pandas.DataFrame
         a dataframe containing the outcome variable for all units.
 
     Y_pre: pandas.DataFrame
         a dataframe containing the actual pre-treatment outcome for the treated unit(s). Note that this is the raw data,
-        therefore if effect is specified, Y_pre will not contain the aggregated data.
+        therefore if effect is specified, it will not contain the aggregated data.
 
     Y_post: pandas.DataFrame
         a dataframe containing the actual post-treatment outcome for the treated unit(s). Note that this is the raw data,
-        therefore if effect is specified, Y_pre will not contain the aggregated data.
+        therefore if effect is specified, it will not contain the aggregated data.
 
     Y_donors : pandas.DataFrame
         a dataframe containing the pre-treatment outcome of the control units.
 
     J : dict
         a dictionary containing the number of donors for each treated unit
 
@@ -196,17 +192,17 @@
 
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “scpi: Uncertainty Quantification for
     Synthetic Control Estimators”.
 
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “Uncertainty Quantification in Synthetic
     Controls with Staggered Treatment Adoption”.
 
-   See Also
+    See Also
     --------
-    scdata, scest, scpi, scplot
+    scdata, scest, scpi, scplot, scplotMulti
 
     """
 
     # Error Checking
 
     # Check main input is a dataframe
     if not isinstance(df, pandas.DataFrame):
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scest.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 16 11:08:57 2021
 
-@author: Filippo Palomba
-"""
 # Temporary code to suppress pandas FutureWarning
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import pandas
 pandas.options.mode.chained_assignment = None
 import numpy
 from copy import deepcopy
 from .funs import w_constr_prep, b_est, b_est_multi, V_prep, mat2dict, ix2rn
 from .scplot import scplot
 from .scplotMulti import scplotMulti
 
 
-def scest(df, w_constr=None, V="separate", plot=False):
+def scest(df, w_constr=None, V="separate", Vmat=None, plot=False):
 
-    '''
+    """
 
     Parameters
     ----------
     df : scdata_output
         a class scdata_output object, obtained by calling scdata
 
     w_constr : dictionary, default {"name": "simplex"}
@@ -31,26 +27,30 @@
         w_constr can contain up to four objects:
         - p, a string indicating the norm to be used (p should be one of "no norm", "L1", and "L2")
         - dir, a string indicating whether the constraint on the norm is an equality ("==") or inequality ("<=")
         - Q, a scalar defining the value of the constraint on the norm
         - lb, a scalar defining the lower bound on the weights. It can be either 0 or -numpy.inf.
         - name, a character selecting one of the default proposals.
 
-    V : str/numpy.array, default "separate"
+    V : str, default "separate"
         a weighting matrix to be used when minimizing the sum of squared residuals.
         The default is the identity matrix ("separate"), so equal weight is given to all observations.
         The other possibility is to specify V = "pooled" for the pooled fit.
 
+    Vmat : numpy.array, defaul None
+        a conformable weighting matrix to be used in the minimization of the sum of squared residuals. To check the proper
+        dimensions, we suggest to check the output of scdata or scdataMulti and inspect the dimensions of B and C.
+
     plot : bool, default False
         a logical specifying whether scplot should be called and a plot saved in the current working directory. For more
         options see scplot.
 
     Returns
     -------
-    The function returns an object of class `scest_output' containing the following objects
+    The function returns an object of class 'scest_output' containing the following objects
 
     w : pandas.DataFrame
         a dataframe containing the weights of the donors.
 
     r : pandas.DataFrame
         a dataframe containing the values of the covariates used for adjustment.
 
@@ -164,15 +164,15 @@
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “Uncertainty Quantification in Synthetic
     Controls with Staggered Treatment Adoption”.
 
     See Also
     --------
     scdata, scdataMulti, scpi, scplot, scplotMulti
 
-    '''
+    """
 
     if df.__class__.__name__ not in ['scdata_output', 'scdata_multi_output']:
         raise Exception("df should be the object returned by running scdata or scdataMulti!")
 
     w_names = []
     w_values = []
     if w_constr is not None:
@@ -224,27 +224,34 @@
     out_in_features = df.out_in_features
     outcome_var = df.outcome_var
 
     ##########################
     # Set up the estimation problem
 
     # Create weighting matrix
-    if not isinstance(V, (pandas.DataFrame, numpy.ndarray, str)):
-        raise Exception("The object V should be a string, a dataframe or a matrix!")
+    if not isinstance(V, str):
+        raise Exception("The object V should be a string! If you want to manually specify the weighting matrix " +
+                        "consider using the option 'Vmat'!")
+
+    if Vmat is not None:
+        if not isinstance(Vmat, (pandas.DataFrame, numpy.ndarray, str)):
+            raise Exception("The object Vmat should a pandas.dataframe or a numpy.array!")
+
+        else:
+            V_shape = numpy.shape(Vmat)
+            if V_shape[0] != len(B) or V_shape[1] != len(B):
+                raise Exception("The object Vmat should be of shape (" + str(len(B)) +
+                                "," + str(len(B)) + ")!")
 
-    if isinstance(V, (pandas.DataFrame, numpy.ndarray)):
-        V_shape = numpy.shape(V)
-        if V_shape[0] != len(B) or V_shape[1] != len(B):
-            raise Exception("The object V should be of shape (" + str(len(B)) +
-                            "," + str(len(B)) + ")!")
-        V_type = "separate"
-        V = pandas.DataFrame(V, index=B.index,
-                             columns=B.index.get_level_values('ID'))
+            Vmat = pandas.DataFrame(Vmat, index=B.index,
+                                    columns=B.index.get_level_values('ID'))
     else:
-        V = V_prep(V_type, B, T0_features, iota)
+        Vmat = V_prep(V_type, B, T0_features, iota)
+
+    V = Vmat
 
     # Estimate SC
     if class_type == "scpi_data":
         w_constr = w_constr_prep(w_constr, w_names, A, Z, V, J, KM)
         result = b_est(A=A, Z=Z, J=J, KM=KM, w_constr=w_constr, V=V)
         cnms = [c.split("_", 1)[1] for c in Z.columns.tolist()]
         idx = pandas.MultiIndex.from_product([df.treated_units, cnms], names=['ID', 'donor'])
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scpi.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Aug 17 14:46:14 2021
 
-@author: Filippo Palomba
-"""
 # Temporary code to suppress pandas FutureWarning
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 from statsmodels.tools.sm_exceptions import IterationLimitWarning
 warnings.filterwarnings("ignore", category=IterationLimitWarning)
 
 import pandas
@@ -25,14 +21,15 @@
 from .scplot import scplot
 from .scplotMulti import scplotMulti
 from scipy.linalg import sqrtm
 
 def scpi(data,
          w_constr=None,
          V="separate",
+         Vmat=None,
          P=None,
          u_missp=True,
          u_sigma="HC1",
          u_order=1,
          u_lags=0,
          u_design=None,
          u_alpha=0.05,
@@ -48,32 +45,37 @@
          cores=None,
          plot=False,
          w_bounds=None,
          e_bounds=None,
          verbose=True,
          pass_stata=False):
 
-    '''
+    """
     Parameters
     ----------
     data : scdata_output
         a class scdata_output object, obtained by calling scdata
 
     w_constr : dict, default {"name": "simplex"}
         a dictionary specifying the constraint set the estimated weights of the donors must belong to.
         w_constr can contain up to five objects:
         1. p, a scalar indicating the norm to be used (p should be one of "no norm", "L1", and "L2")
         2. dir, a string indicating whether the constraint on the norm is an equality ("==") or inequality ("<=")
         3. Q, a scalar defining the value of the constraint on the norm
         4. lb, a scalar defining the lower bound on the weights. It can be either 0 or -numpy.inf.
         5. name, a character selecting one of the default proposals.
 
-    V : numpy.array, default numpy.identity
-        an array specifying the weighting matrix to be used when minimizing the sum of squared residuals.
-        The default is the identity matrix, so equal weight is given to all observations.
+    V : str, default "separate"
+        a weighting matrix to be used when minimizing the sum of squared residuals.
+        The default is the identity matrix ("separate"), so equal weight is given to all observations.
+        The other possibility is to specify V = "pooled" for the pooled fit.
+
+    Vmat : numpy.array, defaul None
+        a conformable weighting matrix to be used in the minimization of the sum of squared residuals. To check the proper
+        dimensions, we suggest to check the output of scdata or scdataMulti and inspect the dimensions of B and C.
 
     P : numpy.array, default None
         a T_1 x (J+K_1) array containing the design matrix to be used to obtain the predicted.
         post-intervention outcome of the synthetic control unit. T_1 is the number of post-treatment periods,
         J is the size of the donor pool, and K_1 is the number of covariates used for adjustment in
         the outcome equation.
 
@@ -156,15 +158,15 @@
         if False prevents printing additional information in the console.
 
     pass_stat : bool, default False
         for internal use only.
 
     Returns
     -------
-    The function returns an object of class `scpi_output' containing the following objects
+    The function returns an object of class 'scpi_output' containing the following objects
 
     w : pandas.DataFrame
         a dataframe containing the weights of the donors.
 
     r : pandas.DataFrame
         a dataframe containing the values of the covariates used for adjustment.
 
@@ -359,30 +361,30 @@
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “Uncertainty Quantification in Synthetic
     Controls with Staggered Treatment Adoption”.
 
     See Also
     --------
     scdata, scdataMulti, scest, splot, scplotMulti
 
-    '''
+    """
 
     if data.__class__.__name__ not in ['scdata_output', 'scdata_multi_output']:
         raise Exception("data should be the object returned by running scdata or scdataMulti!")
 
     if data.__class__.__name__ == "scdata_output":
         class_type = "scpi_data"
     else:
         class_type = "scpi_data_multi"
 
     ######################################
     # Estimation of synthetic weights
     if pass_stata is False and verbose:
         print("-----------------------------------------------")
         print("Estimating Weights...")
-    sc_pred = scest(df=data, w_constr=w_constr, V=V)
+    sc_pred = scest(df=data, w_constr=w_constr, V=V, Vmat=Vmat)
 
     ######################################
     # Retrieve processed data from scest
 
     A = deepcopy(sc_pred.A)                 # Features of treated unit
     B = deepcopy(sc_pred.B)                 # Features of control units
     C = deepcopy(sc_pred.C)                 # Covariates for adjustment
@@ -986,15 +988,15 @@
     e_des_0_na.fillna(0, inplace=True)
     e_des_1.fillna(0, inplace=True)
 
     if e_method == 'gaussian' or e_method == 'all':
         e_lb_gau, e_ub_gau, e_1, e_2 = scpi_out(y=e_res_na, x=e_des_0_na, preds=e_des_1,
                                                 e_method="gaussian", alpha=e_alpha / 2,
                                                 e_lb_est=e_lb_est, e_ub_est=e_ub_est,
-                                                effect=sc_effect)
+                                                effect=sc_effect, out_feat=out_feat[tr])
 
         # Overwrite with user's input
         if e_lb_est is False:
             e_lb_gau = e_bounds[0]
         if e_ub_est is False:
             e_ub_gau = e_bounds[1]
 
@@ -1005,15 +1007,15 @@
         e_mean = e_1
         e_var = e_2
 
     if e_method == 'ls' or e_method == 'all':
         e_lb_ls, e_ub_ls, e_1, e_2 = scpi_out(y=e_res_na, x=e_des_0_na, preds=e_des_1,
                                               e_method="ls", alpha=e_alpha / 2,
                                               e_lb_est=e_lb_est, e_ub_est=e_ub_est,
-                                              effect=sc_effect)
+                                              effect=sc_effect, out_feat=out_feat[tr])
 
         # Overwrite with user's input
         if e_lb_est is False:
             e_lb_ls = e_bounds[0]
         if e_ub_est is False:
             e_ub_ls = e_bounds[1]
 
@@ -1028,15 +1030,15 @@
             e_ub_qreg = numpy.quantile(e_res_na, q=1 - e_alpha / 2)
             e_ub_qreg = pandas.DataFrame([e_ub_qreg] * len(w_lb), index=w_ub.index)
 
         else:
             e_lb_qreg, e_ub_qreg, e_1, e_2 = scpi_out(y=e_res_na, x=e_des_0_na, preds=e_des_1,
                                                       e_method="qreg", alpha=e_alpha / 2,
                                                       e_lb_est=e_lb_est, e_ub_est=e_ub_est,
-                                                      effect=sc_effect)
+                                                      effect=sc_effect, out_feat=out_feat[tr])
         # Overwrite with user's input
         if e_lb_est is False:
             e_lb_qreg = e_bounds[0]
         if e_ub_est is False:
             e_ub_qreg = e_bounds[1]
 
         sc_l_3 = sc_l_0.iloc[:, 0] + e_lb_qreg.iloc[:, 0] - epsk.iloc[:, 0]
@@ -1047,27 +1049,27 @@
     # Simultaneous Prediction Intervals (for each unit)
 
     if sc_effect == "unit-time":  # joint within unit
         T1val = [v for v in T1.values()]
         ML, MU = simultaneousPredGet(vsig, T1val, len(P_na), iota, u_alpha,
                                      e_alpha, e_res_na, e_des_0_na, e_des_1,
                                      w_lb_est, w_ub_est, w_bounds,
-                                     w_constr_aux[tr_units[0]]['name'], sc_effect)
+                                     w_constr_aux[tr_units[0]]['name'], sc_effect, out_feat)
 
     elif sc_effect == "unit":  # joint across units
         ML, MU = simultaneousPredGet(vsig, [len(P_na)], len(P_na), 1, u_alpha,
                                      e_alpha, e_res_na, e_des_0_na, e_des_1,
                                      w_lb_est, w_ub_est, w_bounds,
-                                     w_constr_aux[tr_units[0]]['name'], sc_effect)
+                                     w_constr_aux[tr_units[0]]['name'], sc_effect, out_feat)
 
     elif sc_effect == "time":  # joint within aggregate unit
         ML, MU = simultaneousPredGet(vsig, [len(P_na)], len(P_na), 1, u_alpha,
                                      e_alpha, e_res_na, e_des_0_na, e_des_1,
                                      w_lb_est, w_ub_est, w_bounds,
-                                     w_constr_aux[tr_units[0]]['name'], sc_effect)
+                                     w_constr_aux[tr_units[0]]['name'], sc_effect, out_feat)
 
     ML.set_index(P_na.index, inplace=True, append=False)
     MU.set_index(P_na.index, inplace=True, append=False)
 
     ###############################################
     # Store all bounds
     if sc_effect == "time":
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scplot.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Aug 25 07:55:26 2021
 
-@author: Filippo Palomba
-"""
 # Temporary code to suppress pandas FutureWarning
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import pandas
 pandas.options.mode.chained_assignment = None
@@ -24,20 +20,20 @@
            x_lab=None,
            y_lab=None,
            e_out=True,
            joint=False,
            e_method=None,
            save_data=None):
 
-    '''
+    """
     Parameters
     ----------
     result : scest_output/scpi_output
-        a class `scest_output' object, obtained by calling scest, or a class
-        `scpi_output' object, obtained by calling scpi
+        a class 'scest_output' object, obtained by calling scest, or a class
+        'scpi_output' object, obtained by calling scpi
 
     col_dots_t : str, default "black"
         string indicating the color of the time series marker for treated unit
 
     col_line_t : str, default "black"
         string indicating the color of the time series line for treated unit
 
@@ -86,15 +82,16 @@
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “Uncertainty Quantification in Synthetic
     Controls with Staggered Treatment Adoption”.
 
     See Also
     --------
     scdata, scdataMulti, scest, scpi, scplotMulti
 
-    '''
+    """
+
     class_input = result.__class__.__name__
 
     if class_input not in ['scest_output', 'scpi_output']:
         raise Exception("The object 'result' should be the output of scest or scpi!")
 
     if x_lab is None:
         x_lab = 'Time'
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg/scplotMulti.py` & `scpi_pkg-2.2.3/src/scpi_pkg/scplotMulti.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Jul 25 16:59:19 2022
-
-@author: Filippo Palomba
-"""
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 import pandas
 pandas.options.mode.chained_assignment = None
 import numpy
@@ -30,20 +25,21 @@
                 ncols=3,
                 dateBreaks='10 years',
                 dateFormat='%Y',
                 e_method_input=None,
                 save_data=None,
                 verbose=True):
 
-    '''
+    """
+
     Parameters
     ----------
     result : scest_output/scpi_output
-        a class `scest_multi_output' object, obtained by calling scest, or a class
-        `scpi_multi_output' object, obtained by calling scpi. The data object given as input to
+        a class 'scest_multi_output' object, obtained by calling scest, or a class
+        'scpi_multi_output' object, obtained by calling scpi. The data object given as input to
         this command has to be processed with scdataMulti.
 
     ptype : str, default "series"
         a string that specifies the type of plot to be produced. If set to 'treatment', then treatment effects are
         plotted. If set to 'series' (default), the actual and synthetic time series are reported.
 
     e_out : bool, default True
@@ -115,15 +111,15 @@
     Cattaneo, M. D., Palomba, F., Feng, Y., and Titiunik, R. (2022), “Uncertainty Quantification in Synthetic
     Controls with Staggered Treatment Adoption”.
 
     See Also
     --------
     scdata, scdataMulti, scest, scpi, scplot
 
-    '''
+    """
 
     class_input = result.__class__.__name__
 
     if class_input not in ['scest_multi_output', 'scpi_multi_output']:
         raise Exception("The object 'result' should be the output of scest or scpi " +
                         "when the data have been processed through scdataMulti!")
```

### Comparing `scpi_pkg-2.2.2/src/scpi_pkg.egg-info/PKG-INFO` & `scpi_pkg-2.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scpi-pkg
-Version: 2.2.2
+Name: scpi_pkg
+Version: 2.2.3
 Summary: The package computes point estimates and prediction intervals for Synthetic Control methods as proposed in Cattaneo, Feng, and Titiunik (2021).
 Home-page: https://nppackages.github.io/scpi/
 Author: Filippo Palomba
 Author-email: fpalomba@princeton.edu
 Project-URL: Bug Tracker, https://nppackages.github.io/scpi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCPI_PKG
 
 The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
 
-
 ## Authors
- 
+
 Matias D. Cattaneo (<cattaneo@princeton.edu>)
 
 Yingjie Feng (<fengyj@sem.tsinghua.edu.cn>)
 
 Filippo Palomba (<fpalomba@princeton.edu>)
 
 Rocio Titiunik (<titiunik@princeton.edu>)
@@ -31,52 +30,53 @@
 ## Website
 
 https://nppackages.github.io/scpi/
 
 ## Installation
 
 To install/update use pip
+
 ```
 pip install scpi_pkg
 ```
 
 # Usage
+
 ```
 from from scpi_pkg.scdata import scdata
 from from scpi_pkg.scdataMulti import scdataMulti
 from scpi_pkg.scest import scest
 from scpi_pkg.scpi import scpi
 from scpi_pkg.scplot import scplot
 from scpi_pkg.scplotMulti import scplotMulti
 ```
 
 - Replication: [Germany reunification example](https://github.com/nppackages/scpi/blob/main/Python/scpi_illustration.py).
 
 ## Dependencies
 
-- cvxpy           (>= 1.1.18)
+- cvxpy          (>= 1.1.18)
 - dask            (>= 2021.04.0)
-- nlopt           (>= 2.7.0)
-- numpy           (>= 1.20.1)
-- pandas          (>= 1.2.4)
-- plotnine        (>= 0.8.0)
-- scikit-learn    (>= 0.24.1)
-- scipy           (>= 1.7.1)
-- statsmodels     (>= 0.12.2)
+- ecos            (>= 2.0.7)
+- luddite         (>= 1.0.2)
+- numpy         (>= 1.20.1)
+- pandas        (>= 1.5.0)
+- plotnine       (>= 0.8.0)
+- scikit-learn  (>= 0.24.1)
+- scipy            (>= 1.7.1)
+- statsmodels (>= 0.12.2)
 
 ## References
 
 For overviews and introductions, see [nppackages website](https://nppackages.github.io/).
 
 ### Software and Implementation
 
 - Cattaneo, Feng, Palomba, and Titiunik (2022) [scpi: Uncertainty Quantification for Synthetic Control Estimators](https://arxiv.org/abs/2202.05984).
 
-
 ### Technical and Methodological
 
-- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).<br>
-_Journal of the American Statistical Association_.
-
+- Cattaneo, Feng, and Titiunik (2021): [Prediction Intervals for Synthetic Control Methods](https://cattaneo.princeton.edu/papers/Cattaneo-Feng-Titiunik_2021_JASA.pdf).`<br>`
+  _Journal of the American Statistical Association_.
 - Cattaneo, Feng, Palomba, and Titiunik (2022): Uncertainty Quantification in Synthetic Controls with Staggered Treatment Adoption, working paper.
 
-<br><br>
+`<br><br>`
```

