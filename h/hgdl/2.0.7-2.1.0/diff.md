# Comparing `tmp/hgdl-2.0.7.tar.gz` & `tmp/hgdl-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgdl-2.0.7.tar", last modified: Thu May  4 18:26:58 2023, max compression
+gzip compressed data, was "hgdl-2.1.0.tar", last modified: Fri May 19 22:24:01 2023, max compression
```

## Comparing `hgdl-2.0.7.tar` & `hgdl-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-04 18:26:45.000000 hgdl-2.0.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 18:26:45.000000 hgdl-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 18:26:45.000000 hgdl-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:26:58.813543 hgdl-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-04 18:26:45.000000 hgdl-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1432 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.809543 hgdl-2.0.7/hgdl/global_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/global_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/global_methods/global_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21372 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/hgdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/local_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/bump_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/dNewton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4328 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/local_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/meta_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11124 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/optima.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.809543 hgdl-2.0.7/hgdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-04 18:26:58.813543 hgdl-2.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-05-04 18:26:45.000000 hgdl-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_non_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1339 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_rosenbrock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel_BFGS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel_CG.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-04 18:26:45.000000 hgdl-2.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 22:23:52.000000 hgdl-2.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-19 22:23:52.000000 hgdl-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 22:23:52.000000 hgdl-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 22:24:01.255931 hgdl-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-19 22:23:52.000000 hgdl-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/global_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/global_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2611 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/global_methods/global_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16288 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/hgdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl/local_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2545 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/bump_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/dNewton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4466 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/local_methods/local_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/meta_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4107 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/optima.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-19 22:23:52.000000 hgdl-2.1.0/hgdl/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/hgdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 22:24:01.000000 hgdl-2.1.0/hgdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 22:24:01.255931 hgdl-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-05-19 22:23:52.000000 hgdl-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:24:01.255931 hgdl-2.1.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_non_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_rosenbrock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel_BFGS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-05-19 22:23:52.000000 hgdl-2.1.0/tests/test_schwefel_CG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-19 22:23:52.000000 hgdl-2.1.0/versioneer.py
```

### Comparing `hgdl-2.0.7/LICENSE` & `hgdl-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.7/PKG-INFO` & `hgdl-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.0.7
+Version: 2.1.0
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -41,19 +41,18 @@
 from hgdl.hgdl import HGDL as hgdl
 from hgdl.support_functions import *
 import dask.distributed as distributed
 
 bounds = np.array([[-500,500],[-500,500]])
 #dask_client = distributed.Client("10.0.0.184:8786")
 a = hgdl(schwefel, schwefel_gradient, bounds,
-        hess = schwefel_hessian,
         global_optimizer = "genetic",
-        local_optimizer = "dNewton",
+        local_optimizer = "dNewton", #put in local optimzers from scipy.optimize.minimize
         number_of_optima = 30000,
-        args = (1,1), radius = None, num_epochs = 100)
+        num_epochs = 100)
 
 x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
 a.optimize(x0 = x0)
 
 ###the thread is now released, but the work continues in the background
 
 a.get_latest() ##prints the current result whenever queried
```

### Comparing `hgdl-2.0.7/README.md` & `hgdl-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 from hgdl.hgdl import HGDL as hgdl
 from hgdl.support_functions import *
 import dask.distributed as distributed
 
 bounds = np.array([[-500,500],[-500,500]])
 #dask_client = distributed.Client("10.0.0.184:8786")
 a = hgdl(schwefel, schwefel_gradient, bounds,
-        hess = schwefel_hessian,
         global_optimizer = "genetic",
-        local_optimizer = "dNewton",
+        local_optimizer = "dNewton", #put in local optimzers from scipy.optimize.minimize
         number_of_optima = 30000,
-        args = (1,1), radius = None, num_epochs = 100)
+        num_epochs = 100)
 
 x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
 a.optimize(x0 = x0)
 
 ###the thread is now released, but the work continues in the background
 
 a.get_latest() ##prints the current result whenever queried
```

### Comparing `hgdl-2.0.7/hgdl/global_methods/global_optimizer.py` & `hgdl-2.1.0/hgdl/global_methods/global_optimizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,75 @@
 ##global optimizer for hgdl
 import numpy as np
-import hgdl.misc as misc
 
+from .. import misc
 
-def run_global(x,y,bounds,method,number_of_offspring):
-    #print("Global optimizer: ", method)
-    if method == "genetic": return genetic_step(x,y,bounds,number_of_offspring)
-    elif method == "gauss": return gauss_step(x,y,bounds,number_of_offspring)
-    elif method =="random": return random_step(x,y,bounds,number_of_offspring)
-    elif method is callable: return method(x,y,bounds,number_of_offspring)
-    else: raise Exception("no global method specified")
-
-def gauss_step(x, y, bounds,n):
-    ####x is x where in bounds
-    x_new = []
-    y_new = []
-    #bounds = np.array(bounds)
-    for i in range(len(x)):
-        if misc.in_bounds(x[i],bounds): 
-            x_new.append(x[i])
-            y_new.append(y[i])
-    x = np.asarray(x_new)
-    y = np.asarray(y_new)
-    sorted_indices = np.argsort(y)
-    y = y[sorted_indices]
-    x = x[sorted_indices]
-    x = np.array(x[:-int(len(x)/2)])
-    y = np.array(y[:-int(len(x)/2)])
-    if len(x) == 0: x = np.random.uniform(low = bounds[:,0], high = bounds[:,1], size = (n, len(bounds)))
-    if len(x) < n: x = np.vstack([x,np.random.uniform(low = bounds[:,0], high = bounds[:,1], size = (n-len(x), len(bounds)))])
-    cov = np.cov(x.T)
-    mean= np.mean(x , axis = 0)
-    offspring = np.random.multivariate_normal(mean, cov, size = n)
-    for i in range(len(offspring)):
-        if not misc.in_bounds(offspring[i],bounds): 
-            offspring[i] = np.random.uniform(low = bounds[:,0],high = bounds[:,1], size = len(offspring[0]))
-    return offspring
 
-def random_step(x, y, bounds,n):
-    offspring = np.random.uniform(low = bounds[:,0], high = bounds[:,1], size = (n, len(bounds)))
+def run_global(x, y, bounds, method, number_of_offspring):
+    # print("Global optimizer: ", method)
+    if method == "genetic":
+        return genetic_step(x, y, bounds, number_of_offspring)
+    elif method == "random":
+        return random_step(x, y, bounds, number_of_offspring)
+    elif method is callable:
+        return method(x, y, bounds, number_of_offspring)
+    else:
+        raise Exception("no global method specified")
+
+
+def random_step(x, y, bounds, n):
+    offspring = np.random.uniform(low=bounds[:, 0], high=bounds[:, 1], size=(n, len(bounds)))
     return offspring
 
+
 ###########################################################################
 def genetic_step(X, y, bounds, numChoose):
     """
     Input:
     X is the individuals - points on a surface
     y is the performance - f(X)
     Notes:
     the children can be outside of the bounds!
     """
-    unfairness = 2.5
-    wildness = 0.05
+    unfairness = 100.
+    wildness = 0.0005
     N, k = X.shape
     # normalize the performances to (0,1)
     y -= np.amin(y)
     amax = np.amax(y)
     # if the distribution of performance has no width,
     #   give everyone an equal shot
-    if np.isclose(amax,0.):
-        p = np.ones(N)*1./N
+    if np.isclose(amax, 0.):
+        p = np.ones(N) * 1. / N
     else:
         y /= np.amax(y)
         y *= -1.
         y -= np.amin(y)
         y += 1
-        p = y/np.sum(y)
-    #This chooses from the sample based on the power law,
-    #allowing replacement means that the the individuals
-    #can have multiple kids
-    p = unfairness*np.power(p,unfairness-1)
+        p = y / np.sum(y)
+    # This chooses from the sample based on the power law,
+    # allowing replacement means that the individuals
+    # can have multiple kids
+    p = unfairness * np.power(p, unfairness - 1)
     p /= np.sum(p)
     if np.isnan(p).any():
         raise Exception("got isnans in GeneticStep")
     moms = np.random.choice(N, size=numChoose, replace=True, p=p)
     dads = np.random.choice(N, size=numChoose, replace=True, p=p)
     # calculate a perturbation to the median
     #   of each individual's parents
     perturbation = np.random.normal(
-            loc = 0.,
-            scale = wildness*(bounds[:,1]-bounds[:,0]),
-            size=(numChoose,k))
+        loc=0.,
+        scale=wildness * (bounds[:, 1] - bounds[:, 0]),
+        size=(numChoose, k))
     # the children are the median of their parents plus a perturbation
-    norm = p[moms]+p[dads]
-    weights = (p[moms]/norm, p[dads]/norm)
-    weighted_linear_sum = weights[0].reshape(-1,1)*X[moms] + weights[0].reshape(-1,1)*X[dads]
+    norm = p[moms] + p[dads]
+    weights = (p[moms] / norm, p[dads] / norm)
+    weighted_linear_sum = weights[0].reshape(-1, 1) * X[moms] + weights[0].reshape(-1, 1) * X[dads]
     children = weighted_linear_sum + perturbation
-    oob = np.logical_not([misc.in_bounds(x,bounds) for x in children])
+    oob = np.logical_not([misc.in_bounds(x, bounds) for x in children])
     children[oob] = misc.random_sample(np.sum(oob), k, bounds)
-    #print("=========================")
-    #print("Children in HGDL genetic alg.:", flush = True)
-    #print(children)
-    #print("=========================")
+    # print("=========================")
+    # print("Children in HGDL genetic alg.:", flush = True)
+    # print(children)
+    # print("=========================")
     return children
-
```

### Comparing `hgdl-2.0.7/hgdl/local_methods/bump_function.py` & `hgdl-2.1.0/hgdl/local_methods/bump_function.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 ###local optimizer for hgdl
 import numpy as np
-import hgdl.misc as misc
-import asyncio
-import time
-def b(x,x0,r):
+
+
+def deflated_grad(x, *args, grad_func=None, x_defl=[], radius=[]):
+    d = deflation_function(x, x_defl, radius)
+    return d * grad_func(x, *args)
+
+
+def deflated_hess(x, *args, grad_func=None, hess_func=None, x_defl=[], radius=[]):
+    d = deflation_function(x, x_defl, radius)
+    dg = deflation_function_gradient(x, x_defl, radius)
+    return (hess_func(x, *args) * d) + np.outer(grad_func(x, *args), dg)
+
+
+########################################################
+########################################################
+########################################################
+def b(x, x0, r):
     """
     evaluates the bump function
     x ... a point (1d numpy array)
-    x0 ... 1d numpy array of location of bump function
+    x0 ... 1d numpy array of location of bump function, a 2d numpy array
+
     returns the bump function b(x,x0) with radius r
     """
     d = np.sqrt((x - x0).T @ (x - x0))
-    a = 1.0-(d**2/r**2)
-    if a <= 0: return 0.0
-    else: return np.exp(-1.0/a) * np.exp(1.0)
+    a = 1.0 - (d ** 2 / r ** 2)
+    if a <= 0:
+        return 0.0
+    else:
+        return np.exp(-1.0 / a) * np.exp(1.0)
+
+
 ###########################################################################
-def b_grad(x,x0,r):
+def b_grad(x, x0, r):
     """evaluates the bump function gradient b(x,x0) with radius r
        x ... point
        x0... location of bump
        r ... radius of bump function
     """
     d = np.sqrt((x - x0).T @ (x - x0))
-    d2= (x - x0)
-    a = 1.0 - (d**2/r**2)
-    if a <= 0: return np.zeros((len(x)))
-    else: return (b(x,x0,r) * ((-2.0*d2)/(a**2))) / r**2
+    d2 = (x - x0)
+    a = 1.0 - (d ** 2 / r ** 2)
+    if a <= 0:
+        return np.zeros((len(x)))
+    else:
+        return (b(x, x0, r) * ((-2.0 * d2) / (a ** 2))) / r ** 2
+
+
 ###########################################################################
-def deflation_function(x,x0,r):
+def deflation_function(x, x0, r):
     """
     input:
         x is one point(1d numpy array)
         x0 is a a 2d array of locations of the bump function
     the return is the deflation operator, e.g. 1.0/(1.0 - bump(x,x0))
     """
     if len(x0) == 0: return 1.0
     s = 0.0
     for i in range(len(x0)):
-        s += b(x,x0[i],r)
-    if s == 1.0:
-        print("Warning: Deflation operator = 0. Increase the deflation radius.", flush = True)
-        return 1.0/(1.-0.999999)
-    return 1.0/(1.0-s)
+        s += b(x, x0[i], r[i])
+    if s == 1.0: s = 0.99999
+    return 1.0 / (1.0 - s)
+
+
 ###########################################################################
-def deflation_function_gradient(x,x0,r):
+def deflation_function_gradient(x, x0, r):
     """
     input:
         x is one point(1d numpy array)
-        x0 is a a 2d array of locations of the bump function
+        x0 is a 2d array of locations of the bump function
     the return is the gradient of the deflation operator, e.g. (1.0/(1.0 - bump(x,x0)))'
     """
     if len(x0) == 0: return np.zeros((len(x)))
     s1 = 0.0
     s2 = np.zeros((len(x)))
     for i in range(len(x0)):
-        s1 += b(x,x0[i],r)
-        s2 += b_grad(x,x0[i],r)
-    if s1 == 1.0: return s2/((1.0-0.9999)**2)
-    return s2/((1.0-s1)**2)
-
-def deflated_grad(x, *args, grad_func = None, x_defl = [], radius = 0.01):
-    d = deflation_function(x,x_defl,radius)
-    return d*grad_func(x, *args)
-
-
-def deflated_hess(x,*args, grad_func = None, hess_func = None, x_defl = [], radius = 0.01):
-    d = deflation_function(x,x_defl,radius)
-    dg = deflation_function_gradient(x,x_defl,radius)
-    return (hess_func(x, *args)*d) + np.outer(grad_func(x, *args),dg)
-
+        s1 += b(x, x0[i], r[i])
+        s2 += b_grad(x, x0[i], r[i])
+    if s1 == 1.0: s1 = 0.99999
+    return s2 / ((1.0 - s1) ** 2)
```

### Comparing `hgdl-2.0.7/hgdl/local_methods/dNewton.py` & `hgdl-2.1.0/hgdl/local_methods/dNewton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,33 @@
 import numpy as np
-import hgdl.misc as misc
-import hgdl.local_methods.bump_function as defl
-import dask.distributed as distributed
 from loguru import logger
 
+from .. import misc
 
-def DNewton(func,grad,hess,bounds,x0,max_iter,tol,*args):
+
+def DNewton(func, grad, hess, bounds, x0, max_iter, tol, *args):
     e = np.inf
     gradient = np.ones((len(x0))) * np.inf
     counter = 0
     x = np.array(x0)
     grad_list = []
     while e > tol or np.max(abs(gradient)) > tol:
-        x = misc.project_onto_bounds(x,bounds)
-        x[abs(x)<1e-16] = 0.
-        gradient = grad(x,*args)
-        gradient[abs(gradient)<1e-16] = 0.
-        if hess: hessian  = hess(x,*args)
-        else: hessian = approximate_hessian(x,grad,*args)
+        x = misc.project_onto_bounds(x, bounds)
+        x[abs(x) < 1e-16] = 0.
+        gradient = grad(x, *args)
+        gradient[abs(gradient) < 1e-16] = 0.
+        hessian = hess(x, *args)
+        # hessian = 0.5 * hessian @ hessian.T
         hessian[abs(hessian) < 1e-16] = 0.
         grad_list.append(np.max(gradient))
-        try: gamma = np.linalg.solve(hessian,-gradient)
-        except Exception as error: gamma,a,b,c = np.linalg.lstsq(hessian,-gradient,rcond=None)
-        if any(gamma == np.nan) or any(gamma == np.inf): return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], False
+        try:
+            gamma = np.linalg.solve(hessian, -gradient)
+        except Exception as error:
+            gamma, a, b, c = np.linalg.lstsq(hessian, -gradient, rcond=None)
+        if any(gamma == np.nan) or any(gamma == np.inf): return x, func(x, *args), gradient, \
+        np.linalg.eig(hess(x, *args))[0], False
         x += gamma
         e = np.max(abs(gamma))
-        logger.debug("dNewton step size: ", e, " max gradient: ",np.max(abs(gradient)))
-        #print("dNewton step size: ", e, " max gradient: ",np.max(abs(gradient)))
-        if counter > max_iter: return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], False#, "max_iter reached"
+        logger.debug("dNewton step size: ", e, " max gradient: ", np.max(abs(gradient)))
+        if counter > max_iter: return x, func(x, *args), gradient, np.linalg.eig(hess(x, *args))[0], False
         counter += 1
-    return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], True #, "converged"
-
-
-
-def approximate_hessian(x, grad, *args):
-    ##implements a first-order approximation
-    len_x = len(x)
-    hess = np.zeros((len_x,len_x))
-    epsilon = 1e-6
-    grad_x = grad(x, *args)
-    for i in range(len_x):
-        x_temp = np.array(x)
-        x_temp[i] = x_temp[i] + epsilon
-        hess[i,i:] = ((grad(x_temp,*args) - grad_x)/epsilon)[i:]
-    return hess + hess.T - np.diag(np.diag(hess))
-
-
-
-
-
-
-
+    return x, func(x, *args), gradient, np.linalg.eig(hess(x, *args))[0], True
```

### Comparing `hgdl-2.0.7/hgdl/local_methods/local_optimizer.py` & `hgdl-2.1.0/hgdl/local_methods/local_optimizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,125 @@
 import numpy as np
-import time
-
+from distributed import get_client
 from loguru import logger
-
-import hgdl.misc as misc
-import dask.distributed
-from distributed import Client, get_client, secede, rejoin, protocol
-import dask.distributed as distributed
-from hgdl.local_methods.dNewton import DNewton
 from scipy.optimize import minimize
-import hgdl.local_methods.bump_function as defl
+
+from . import bump_function as defl
+from .. import misc
+from . import dNewton as DNewton
+
+
+def run_local(d, optima, x0):
+    x_defl, f_defl, radii = optima.get_deflation_points(len(optima.list))
+    return run_local_optimizer(d, x0, x_defl, radii)
 
 
-def run_local(d,optima,x0):
-    x_defl,f_defl = optima.get_deflation_points(len(optima.list))
-    return run_local_optimizer(d,x0,x_defl)
 ###########################################################################
-def run_local_optimizer(d,x0,x_defl = []):
+def run_local_optimizer(d, x0, x_defl=[], radii=[]):
     """
     this function runs a deflated local methos for
     all the walkers.
     The loop below goes over every walker
     input:
         2d numpy array of initial positions
         2d numpy array of positions of deflations (optional, default = [])
     return:
         optima_locations, func values, gradient norms, eigenvalues, local_success(bool)
     """
     dim = d.dim
     number_of_walkers = d.number_of_walkers
 
     if len(x0) < number_of_walkers:
-        x0 = np.row_stack([x0,misc.random_population(d.bounds,number_of_walkers - len(x0))])
+        x0 = np.row_stack([x0, misc.random_population(d.bounds, number_of_walkers - len(x0))])
 
     client = get_client()
     tasks = []
-    bf = client.scatter(d,workers = d.workers["walkers"])
-    for i in range(min(len(x0),number_of_walkers)):
-        logger.debug("Worker ",i," submitted")
-        #print("Worker ",i," submitted", flush = True)
+    bf = client.scatter(d, workers=d.workers["walkers"])
+    for i in range(min(len(x0), number_of_walkers)):
+        logger.debug("Worker ", i, " submitted")
         worker = d.workers["walkers"][(int(i - ((i // number_of_walkers) * number_of_walkers)))]
-        data = {"d":bf,"x0":x0[i],"x_defl":x_defl}
-        tasks.append(client.submit(local_method,data,workers = worker))
+        data = {"d": bf, "x0": x0[i], "x_defl": x_defl, "radius": radii}
+        tasks.append(client.submit(local_method, data, workers=worker))
 
     results = client.gather(tasks)
     number_of_walkers = len(tasks)
     x = np.empty((number_of_walkers, dim))
     f = np.empty((number_of_walkers))
-    Lg = np.empty((number_of_walkers, dim))
-    eig = np.empty((number_of_walkers,dim))
-    local_success = np.empty((number_of_walkers), dtype = bool)
+    g = np.empty((number_of_walkers, dim))
+    eig = np.empty((number_of_walkers, dim))
+    r = np.empty((number_of_walkers))
+    local_success = np.empty((number_of_walkers), dtype=bool)
 
     for i in range(len(tasks)):
-        x[i],f[i],Lg[i],eig[i],local_success[i] = results[i]
+        x[i], f[i], g[i], eig[i], r[i], local_success[i] = results[i]
         client.cancel(tasks[i])
         for j in range(i):
-            if np.linalg.norm(np.subtract(x[i],x[j])) < 2.0 * d.radius and local_success[j] == True:
+            if np.linalg.norm(np.subtract(x[i], x[j])) < r[i] and local_success[j] == True:
                 logger.warning("points converged too close to each other in HGDL; point removed")
-                local_success[j] = False; break
+                local_success[j] = False
         for j in range(len(x_defl)):
-            if np.linalg.norm(np.subtract(x[i],x_defl[j])) < 2.0 * d.radius and all(Lg[i] < 1e-5):
+            if np.linalg.norm(np.subtract(x[i], x_defl[j])) < radii[j] and all(g[i] < 1e-5):
                 logger.warning("local method converged within 2 x radius of a deflated position in HGDL")
                 local_success[i] = False
-    return x, f, Lg, eig, local_success
+    return x, f, g, eig, r, local_success
+
 
-def local_method(data, method = "dNewton"):
+def local_method(data, method="dNewton"):
     from functools import partial
     d = data["d"]
     x0 = np.array(data["x0"])
     e = np.inf
     local_success = True
     tol = d.tolerance
     x_defl = data["x_defl"]
+    r_defl = data["radius"]
     bounds = d.bounds
     max_iter = d.local_max_iter
     args = d.args
     method = d.local_optimizer
-    #augment grad, hess
-    Lgrad = partial(defl.deflated_grad, grad_func = d.Lgrad, x_defl = x_defl, radius = d.radius)
-    if callable(d.Lhess):
-        Lhess = partial(defl.deflated_hess, grad_func = d.Lgrad,
-                       hess_func = d.Lhess, x_defl = x_defl, radius = d.radius)
-    else:
-        Lhess = d.Lhess
+    constr = d.constr
+    # augment grad, hess
+    grad = partial(defl.deflated_grad, grad_func=d.grad, x_defl=x_defl, radius=r_defl)
+    hess = partial(defl.deflated_hess, grad_func=d.grad, hess_func=d.hess, x_defl=x_defl, radius=r_defl)
 
-    #call local methods
+    # call local methods
     if method == "dNewton":
-        x,L,Lg,eig,local_success = DNewton(d.L,Lgrad,Lhess,bounds,x0,max_iter,tol,*args)
-        f = d.func(x,*args)
+        x, f, g, eig, local_success = DNewton(d.func, grad, hess, bounds, x0, max_iter, tol, *args)
+        # f = d.func(x,*args)
+        r = 1. / np.min(eig)
 
     elif type(method) == str:
-        if d.constr: logger.warning("Deflated constraints are only supported by local optimizer 'DNewton'")
-        res = minimize(d.func, x0, args = args, method = method, jac = Lgrad, hess = Lhess,
-                       bounds = bounds, options = {"disp":False})
+        res = minimize(d.func, x0, args=args, method=method, jac=grad, hess=hess, bounds=bounds, constraints=constr,
+                       options={"disp": False})
         x = res["x"]
         f = res["fun"]
-        eig = np.ones(x.shape) * np.nan
-        Lg = res["jac"]
-        local_success = res["success"]
+        g = res["jac"]
+
+        local_success = False
+        if np.linalg.norm(g) < 1e-5:
+            local_success = True
+            eig = np.linalg.eig(hess(x, *args))[0]
+            r = 1. / np.min(eig)
+        else:
+            eig = np.array([0.0])
+            r = 0.0
+
 
     elif callable(method):
-        res = method(d.func,Lgrad,Lhess,bounds,x0,*args)
+        res = method(d.func, grad, hess, bounds, x0, *args)
         x = res["x"]
         f = res["fun"]
-        eig = np.ones(x.shape) * np.nan
-        Lg = res["jac"]
-        local_success = res["success"]
+        g = res["jac"]
+        local_success = False
+        if np.linalg.norm(g) < 1e-5:
+            local_success = True
+            eig = np.linalg.eig(hess(x, *args))[0]
+            r = 1. / np.min(eig)
+        else:
+            eig = np.array([0.0])
+            r = 0.0
 
+    else:
+        raise Exception("no local method specified")
 
-    else: raise Exception("no local method specified")
-
-    return x,f,Lg,np.real(eig),local_success
+    return x, f, g, np.real(eig), np.abs(r), local_success
 ###########################################################################
```

### Comparing `hgdl-2.0.7/hgdl/meta_data.py` & `hgdl-2.1.0/hgdl/meta_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-import numpy as np
-
-
 class meta_data:
     """
     this class contains all the data necessary to run the workers
     """
-    def __init__(self,obj):
-        self.workers = obj.workers    ###dictionary of host and walker workers
+
+    def __init__(self, obj):
+        self.workers = obj.workers  ###dictionary of host and walker workers
         self.x0 = obj.x0
         self.func = obj.func
         self.grad = obj.grad
         self.hess = obj.hess
-        self.L = obj.L
-        self.Lgrad = obj.Lgrad
-        self.Lhess = obj.Lhess
         self.bounds = obj.bounds
-        self.radius = obj.radius
-        self.dim_x = obj.dim_x
-        self.dim_k = obj.dim_k
-        self.dim = obj.dim_x + self.dim_k
+        self.dim = obj.dim
 
         self.local_max_iter = obj.local_max_iter
         self.number_of_walkers = obj.number_of_walkers
         self.num_epochs = obj.num_epochs
         self.global_optimizer = obj.global_optimizer
         self.local_optimizer = obj.local_optimizer
         self.args = obj.args
-        self.constr = obj.constr
         self.tolerance = obj.tolerance
+        self.constr = obj.constraints
```

### Comparing `hgdl-2.0.7/hgdl.egg-info/PKG-INFO` & `hgdl-2.1.0/hgdl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.0.7
+Version: 2.1.0
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -41,19 +41,18 @@
 from hgdl.hgdl import HGDL as hgdl
 from hgdl.support_functions import *
 import dask.distributed as distributed
 
 bounds = np.array([[-500,500],[-500,500]])
 #dask_client = distributed.Client("10.0.0.184:8786")
 a = hgdl(schwefel, schwefel_gradient, bounds,
-        hess = schwefel_hessian,
         global_optimizer = "genetic",
-        local_optimizer = "dNewton",
+        local_optimizer = "dNewton", #put in local optimzers from scipy.optimize.minimize
         number_of_optima = 30000,
-        args = (1,1), radius = None, num_epochs = 100)
+        num_epochs = 100)
 
 x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
 a.optimize(x0 = x0)
 
 ###the thread is now released, but the work continues in the background
 
 a.get_latest() ##prints the current result whenever queried
```

### Comparing `hgdl-2.0.7/hgdl.egg-info/SOURCES.txt` & `hgdl-2.1.0/hgdl.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 hgdl/__init__.py
 hgdl/_version.py
-hgdl/constraints.py
 hgdl/hgdl.py
 hgdl/meta_data.py
 hgdl/misc.py
 hgdl/optima.py
 hgdl/support_functions.py
 hgdl.egg-info/PKG-INFO
 hgdl.egg-info/SOURCES.txt
```

### Comparing `hgdl-2.0.7/setup.py` & `hgdl-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.7/tests/test_non_diff.py` & `hgdl-2.1.0/tests/test_non_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import time
 import dask.distributed as distributed
 
 
 
 def test_non_diff():
     #dask_client = distributed.Client("10.0.0.184:8786")
-    a = HGDL(non_diff, non_diff_grad, 
-             hess = non_diff_hess,bounds = [[-5,5],[-5,5]],
-            radius = 0.1, num_epochs = 5)
+    a = HGDL(non_diff, non_diff_grad,
+             hess = non_diff_hess,bounds = [[-5,5],[-5,5]], num_epochs = 5)
     a.optimize(dask_client = None)
     res = a.optima.list
 
     #print(a.optima_list)
     print("main thread submitted HGDL and will now sleep for 10 seconds")
     time.sleep(10)
     print("main thread asks for 10 best solutions:")
```

### Comparing `hgdl-2.0.7/tests/test_rosenbrock.py` & `hgdl-2.1.0/tests/test_rosenbrock.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,25 @@
     from hgdl.hgdl import HGDL
     from time import sleep, perf_counter
     print('this will create an hgdl object, sleep for 3'
             ' seconds, get the best result, sleep for 3 seconds,'
             'then get the final result.\n'
             'working on the epochs should happend even during sleeping\n'
             )
+    from scipy.optimize import NonlinearConstraint
+    def g1(x): return (np.linalg.norm(x)**2/10.0) - 2.0
+    nlc = NonlinearConstraint(g1, -np.inf, 0)
     bounds = np.array([[-2,2],[-2,2]])
-    a = HGDL(rosen, rosen_der,[[-2,2],[-2,2]], hess = rosen_hess, radius = 0.1, num_epochs = 10000)
+    a = hgdl(rosen, rosen_der, bounds, hess = rosen_hess,
+            global_optimizer = "random",
+            local_optimizer = "dNewton",
+            number_of_optima = 30000,
+            args = (), num_epochs = 1000,
+            constraints = (nlc,)
+            )
     x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
     a.optimize(x0 = x0)
 
 
     print("main thread submitted HGDL and will now sleep for 5 seconds")
     sleep(5)
     print("main thread asks for solutions:")
```

### Comparing `hgdl-2.0.7/tests/test_schwefel.py` & `hgdl-2.1.0/tests/test_schwefel_BFGS.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 
 
 def test_schwefel():
     arr  = 5
     brr  = 6
     bounds = np.array([[-500,500],[-500,500]])
     a = hgdl(schwefel, schwefel_gradient, bounds,
-            hess = schwefel_hessian,
             global_optimizer = "genetic",
-            local_optimizer = "dNewton",
-            number_of_optima = 30000,
-            args = (arr,brr), radius = None, num_epochs = 100)
+            local_optimizer = "BFGS",
+            number_of_optima = 30000, 
+            num_epochs = 100)
 
     x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
     print("starting positions: ")
     print(x0)
     print("--------------------")
     a.optimize(x0 = x0)
 
 
     #print(a.optima_list)
     print("main thread submitted HGDL and will now sleep for 2 seconds")
-    time.sleep(10)
+    time.sleep(2)
     print("main thread asks for 10 best solutions:")
     print(a.get_latest())
     print("main sleeps for another 2 seconds")
     time.sleep(2)
     print("main thread kills optimization")
     res = a.kill_client()
     print("hgdl was killed but I am waiting 2s")
```

### Comparing `hgdl-2.0.7/tests/test_schwefel_BFGS.py` & `hgdl-2.1.0/tests/test_schwefel.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 
 
 def test_schwefel():
     arr  = 5
     brr  = 6
     bounds = np.array([[-500,500],[-500,500]])
     a = hgdl(schwefel, schwefel_gradient, bounds,
-            hess = schwefel_hessian,
             global_optimizer = "genetic",
-            local_optimizer = "BFGS",
-            number_of_optima = 30000,
-            args = (arr,brr), radius = None, num_epochs = 100)
+            local_optimizer = "dNewton",
+            number_of_optima = 30000, 
+            num_epochs = 100)
 
     x0 = np.random.uniform(low = bounds[:, 0], high = bounds[:,1],size = (20,2))
     print("starting positions: ")
     print(x0)
     print("--------------------")
     a.optimize(x0 = x0)
 
 
     #print(a.optima_list)
     print("main thread submitted HGDL and will now sleep for 2 seconds")
-    time.sleep(2)
+    time.sleep(10)
     print("main thread asks for 10 best solutions:")
     print(a.get_latest())
     print("main sleeps for another 2 seconds")
     time.sleep(2)
     print("main thread kills optimization")
     res = a.kill_client()
     print("hgdl was killed but I am waiting 2s")
```

### Comparing `hgdl-2.0.7/versioneer.py` & `hgdl-2.1.0/versioneer.py`

 * *Files identical despite different names*

