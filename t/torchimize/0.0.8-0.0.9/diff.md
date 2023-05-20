# Comparing `tmp/torchimize-0.0.8.tar.gz` & `tmp/torchimize-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchimize-0.0.8.tar", last modified: Mon May 23 23:25:01 2022, max compression
+gzip compressed data, was "torchimize-0.0.9.tar", last modified: Wed May 25 14:58:02 2022, max compression
```

## Comparing `torchimize-0.0.8.tar` & `torchimize-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35365 2022-05-23 23:24:10.000000 torchimize-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-23 23:25:01.282482 torchimize-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-05-23 23:24:10.000000 torchimize-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-23 23:25:01.282482 torchimize-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-05-23 23:24:10.000000 torchimize-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/emg_mm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/unit_test_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     3906 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/unit_test_analytical_jacobian.py
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/unit_test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/unit_test_raw_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-05-23 23:24:10.000000 torchimize-0.0.8/tests/unit_test_skewed_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/torchimize/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/torchimize/functions/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/gna_fun.py
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/gna_fun_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/lma_fun.py
--rw-r--r--   0 runner    (1001) docker     (121)     6527 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/functions/lma_fun_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/torchimize/optimizer/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4656 2022-05-23 23:24:10.000000 torchimize-0.0.8/torchimize/optimizer/gna_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 23:25:01.282482 torchimize-0.0.8/torchimize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-23 23:25:01.000000 torchimize-0.0.8/torchimize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.684136 torchimize-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35365 2022-05-25 14:57:06.000000 torchimize-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-25 14:58:02.684136 torchimize-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2022-05-25 14:57:06.000000 torchimize-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-25 14:58:02.684136 torchimize-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-05-25 14:57:06.000000 torchimize-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.680137 torchimize-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/emg_mm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/unit_test_all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3906 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/unit_test_analytical_jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7939 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/unit_test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/unit_test_raw_fit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-05-25 14:57:06.000000 torchimize-0.0.9/tests/unit_test_skewed_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.680137 torchimize-0.0.9/torchimize/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.680137 torchimize-0.0.9/torchimize/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/fun_dims.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/gna_fun.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/gna_fun_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/lma_fun.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5728 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/lma_fun_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/functions/newton_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.684136 torchimize-0.0.9/torchimize/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4656 2022-05-25 14:57:06.000000 torchimize-0.0.9/torchimize/optimizer/gna_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 14:58:02.680137 torchimize-0.0.9/torchimize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-25 14:58:02.000000 torchimize-0.0.9/torchimize.egg-info/top_level.txt
```

### Comparing `torchimize-0.0.8/LICENSE.md` & `torchimize-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/PKG-INFO` & `torchimize-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchimize
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimization Algorithms using Pytorch
 Home-page: http://github.com/hahnec/torchimize
 Author: Christopher Hahne
 Author-email: inbox@christopherhahne.de
 License: GNU GPL V3.0
 Description: torchimize contains implementations of the Gauss-Newton and Levenberg-Marquardt optimization algorithms using the PyTorch library. The main motivation for this project is to enable convex optimization on GPUs based on the torch.Tensor class, which (as of 2022) is widely used in the deep learning field. This package features the capability to minimize several least-squares optimization problems at each loop iteration in parallel.
 Keywords: pytorch torch optimization mathematical linear programming gauss newton levenberg marquardt
```

### Comparing `torchimize-0.0.8/README.rst` & `torchimize-0.0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -23,44 +23,54 @@
     from torchimize.functions import lsq_gna
     coeffs_list = lsq_gna(initials, cost_fun, args=(other_args,))
 
     # single levenberg-marquardt
     from torchimize.functions import lsq_lma
     coeffs_list = lsq_lma(initials, function=cost_fun, jac_function=jac_fun, args=(other_args,))
 
-    # parallel gauss-newton for batch-optimization at multiple costs
+    # parallel gauss-newton for several optimization problems at multiple costs
     from torchimize.functions import lsq_gna_parallel
     coeffs_list = lsq_gna_parallel(
                         p = initials_batch,
                         function = multi_cost_fun_batch,
                         jac_function = multi_jac_fun_batch,
                         args = (other_args,),
-                        wvec = torch.ones(5, device='cuda', dtype=torch.float64),
+                        wvec = torch.ones(5, device='cuda', dtype=initials_batch.dtype),
                         ftol = 1e-8,
                         ptol = 1e-8,
                         gtol = 1e-8,
-                        l = .1,
+                        l = 1.,
                         max_iter = 80,
                     )
 
-    # parallel levenberg-marquardt for batch-optimization at multiple costs
+    # parallel levenberg-marquardt for several optimization problems at multiple costs
     from torchimize.functions import lsq_lma_parallel
     coeffs_list = lsq_lma_parallel(
                         p = initials_batch,
                         function = multi_cost_fun_batch,
                         jac_function = multi_jac_fun_batch,
                         args = (other_args,),
-                        wvec = torch.ones(5, device='cuda', dtype=torch.float64),
+                        wvec = torch.ones(5, device='cuda', dtype=initials_batch.dtype),
                         ftol = 1e-8,
                         ptol = 1e-8,
                         gtol = 1e-8,
-                        meth = 'lev',
+                        meth = 'marq',
                         max_iter = 40,
                     )
 
+    # validate that your provided functions return correct tensor dimensionality
+    from torchimize.functions import test_fun_dims_parallel
+    ret = test_fun_dims_parallel(
+        p = initials_batch,
+        function = multi_cost_fun_batch,
+        jac_function = multi_jac_fun_batch,
+        args = (other_args,),
+        wvec = torch.ones(5, device='cuda', dtype=initials_batch.dtype),
+    )
+
 .. note::
     For simultaneous minimization of ``B`` optimization problems at a multiple of ``C`` costs, the ``function`` and ``jac_function`` arguments require to return a torch.Tensor type of ``B x C x N`` and ``B x C x N x P``, respectively. Here, ``N`` is the residual dimension and ``P`` represents the sought parameter number in each ``B x C``.
 
 For further details, see the |apidoc|_.
 
 
 .. substitutions
```

### Comparing `torchimize-0.0.8/setup.py` & `torchimize-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/tests/emg_mm.py` & `torchimize-0.0.9/tests/emg_mm.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/tests/unit_test_all.py` & `torchimize-0.0.9/tests/unit_test_all.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/tests/unit_test_analytical_jacobian.py` & `torchimize-0.0.9/tests/unit_test_analytical_jacobian.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/tests/unit_test_parallel.py` & `torchimize-0.0.9/tests/unit_test_parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,75 +115,82 @@
             alpha*pd_emg_wrt_eta(t, mu, sigma, eta),
         ]).T
 
         return jacobian
 
     def test_gna_emg_conditions(self):
 
-        coeffs = lsq_gna_parallel(
-            p = self.batch_initials,
-            function = self.multi_cost_batch,
-            jac_function = self.multi_jaco_batch,
-            args = (self.t, self.batch_data_channels),
-            wvec = torch.ones(2, device=self.device, dtype=torch.float64, requires_grad=False),
-            l = .1,
-            gtol = 1e-6,
-            max_iter = 199,
-        )
-
-        # assertion
-        ret_params = torch.allclose(coeffs[-1], self.gt_params, atol=1e-1)
-        self.assertTrue(ret_params, 'Coefficients deviate')
-        eps = torch.sum(self.cost_batch(coeffs[-1], t=self.t, y=self.batch_data_channels))
-        self.assertTrue(eps.cpu()/len(self.gt_params) < 1, 'Error exceeded 1')
-        self.assertTrue(len(coeffs) < 200, 'Number of iterations exceeded 200')
+        for p in [self.batch_initials.float(), self.batch_initials.double()]:
 
-    def test_gna_emg_plain(self):
-
-        multi_cost_batch_args = lambda p, t=self.t, y=self.batch_data_channels: self.multi_cost_batch(p_batch=p, t=t, y=y)
-        multi_jaco_batch_args = lambda p, t=self.t, y=self.batch_data_channels: self.multi_jaco_batch(p_batch=p, t=t, data=y)
+            coeffs = lsq_gna_parallel(
+                p = p,
+                function = self.multi_cost_batch,
+                jac_function = self.multi_jaco_batch,
+                args = (self.t.to(dtype=p.dtype), self.batch_data_channels.to(dtype=p.dtype)),
+                wvec = torch.ones(2, device=self.device, dtype=p.dtype, requires_grad=False),
+                l = .1,
+                gtol = 1e-6,
+                max_iter = 199,
+            )
 
-        coeffs = lsq_gna_parallel_plain(
-            p = self.batch_initials,
-            function = multi_cost_batch_args,
-            jac_function = multi_jaco_batch_args,
-            wvec = torch.ones(2, device=self.device, dtype=torch.float64, requires_grad=False),
-            l = .1,
-            max_iter = 199,
-        )
-
-        # assertion
-        ret_params = torch.allclose(coeffs, self.gt_params, atol=1e-1)
-        self.assertTrue(ret_params, 'Coefficients deviate')
-        eps = torch.sum(multi_cost_batch_args(coeffs))
-        self.assertTrue(eps.cpu()/len(self.gt_params) < 1, 'Error exceeded 1')
-        self.assertTrue(len(coeffs) < 200, 'Number of iterations exceeded 200')
+            # assertion
+            ret_params = torch.allclose(coeffs[-1].double(), self.gt_params, atol=1e-1)
+            self.assertTrue(ret_params, 'Coefficients deviate')
+            eps = torch.sum(self.cost_batch(coeffs[-1].double(), t=self.t, y=self.batch_data_channels))
+            self.assertTrue(eps.cpu()/len(self.gt_params) < 1, 'Error exceeded 1')
+            self.assertTrue(len(coeffs) < 200, 'Number of iterations exceeded 200')
 
-    def test_lma_emg_conditions(self):
+    def test_gna_emg_plain(self):
 
-        from torchimize.functions.lma_fun_parallel import lsq_lma_parallel
 
-        for m in ['lev', 'marq']:
+        for p in [self.batch_initials.float(), self.batch_initials.double()]:
 
-            coeffs = lsq_lma_parallel(
-                self.batch_initials,
-                function = self.multi_cost_batch,
-                jac_function = self.multi_jaco_batch,
-                args = (self.t, self.batch_data_channels),
-                wvec = torch.ones(2, device=self.device, dtype=torch.float64, requires_grad=False),
-                meth = m,
+            multi_cost_batch_args = lambda p: self.multi_cost_batch(p_batch=p, t=self.t.to(dtype=p.dtype), y=self.batch_data_channels.to(dtype=p.dtype))
+            multi_jaco_batch_args = lambda p: self.multi_jaco_batch(p_batch=p, t=self.t.to(dtype=p.dtype), data=self.batch_data_channels.to(dtype=p.dtype))
+            
+            coeffs = lsq_gna_parallel_plain(
+                p = p,
+                function = multi_cost_batch_args,
+                jac_function = multi_jaco_batch_args,
+                wvec = torch.ones(2, device=self.device, dtype=p.dtype, requires_grad=False),
+                l = .1,
                 max_iter = 199,
             )
 
             # assertion
-            ret_params = torch.allclose(coeffs[-1], self.gt_params, atol=1e-1)
+            ret_params = torch.allclose(coeffs.double(), self.gt_params, atol=1e-1)
             self.assertTrue(ret_params, 'Coefficients deviate')
-            eps = torch.sum(self.cost_batch(coeffs[-1], t=self.t, y=self.batch_data_channels))
+            eps = torch.sum(multi_cost_batch_args(coeffs.double()))
             self.assertTrue(eps.cpu()/len(self.gt_params) < 1, 'Error exceeded 1')
-            self.assertTrue(len(coeffs) < 40, 'Number of iterations exceeded 40')
+            self.assertTrue(len(coeffs) < 200, 'Number of iterations exceeded 200')
+
+    def test_lma_emg_conditions(self):
+
+        from torchimize.functions.lma_fun_parallel import lsq_lma_parallel
+
+        for p in [self.batch_initials.float(), self.batch_initials.double()]:
+            
+            for m in ['lev', 'marq']:
+
+                coeffs = lsq_lma_parallel(
+                    p = p,
+                    function = self.multi_cost_batch,
+                    jac_function = self.multi_jaco_batch,
+                    args = (self.t.to(dtype=p.dtype), self.batch_data_channels.to(dtype=p.dtype)),
+                    wvec = torch.ones(2, device=self.device, dtype=p.dtype, requires_grad=False),
+                    meth = m,
+                    max_iter = 199,
+                )
+
+                # assertion
+                ret_params = torch.allclose(coeffs[-1].double(), self.gt_params, atol=1e-1)
+                self.assertTrue(ret_params, 'Coefficients deviate')
+                eps = torch.sum(self.cost_batch(coeffs[-1].double(), t=self.t, y=self.batch_data_channels))
+                self.assertTrue(eps.cpu()/len(self.gt_params) < 1, 'Error exceeded 1')
+                self.assertTrue(len(coeffs) < 40, 'Number of iterations exceeded 40')
 
     def test_all(self):
 
         self.test_lma_emg_conditions()
         self.test_gna_emg_conditions()
         self.test_gna_emg_plain()
```

### Comparing `torchimize-0.0.8/tests/unit_test_raw_fit.py` & `torchimize-0.0.9/tests/unit_test_raw_fit.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/tests/unit_test_skewed_gaussian.py` & `torchimize-0.0.9/tests/unit_test_skewed_gaussian.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/torchimize/__init__.py` & `torchimize-0.0.9/torchimize/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
     You should have received a copy of the GNU General Public License
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `torchimize-0.0.8/torchimize/functions/gna_fun.py` & `torchimize-0.0.9/torchimize/functions/gna_fun.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/torchimize/functions/gna_fun_parallel.py` & `torchimize-0.0.9/torchimize/functions/gna_fun_parallel.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch
 from typing import Union, Callable, Tuple, List
 
 from torchimize.functions.jacobian import jacobian_approx_t
+from torchimize.functions.newton_parallel import newton_step_parallel
 
 
 def lsq_gna_parallel(
         p: torch.Tensor,
         function: Callable, 
         jac_function: Callable = None,
         args: Union[Tuple, List] = (),
@@ -75,55 +76,14 @@
         f_prev = f.clone()
         
         if gcon or pcon or fcon:
             break
 
     return p_list
 
-def test_fun_dims(        
-        p: torch.Tensor,
-        function: Callable, 
-        jac_function: Callable = None,
-        args: Union[Tuple, List] = (),
-        wvec: torch.Tensor = None,
-    ) -> bool:
-    """
-    Helper function to test whether dimensionality of output tensors suits the herein provided optimization functions.
-
-    :param p: initial value(s)
-    :param function: user-provided function which takes p (and additional arguments) as input
-    :param jac_fun: user-provided Jacobian function which takes p (and additional arguments) as input
-    :param args: optional arguments passed to function
-    """
-
-    if len(args) > 0:
-        # pass optional arguments to function
-        fun = lambda p: function(p, *args)
-    else:
-        fun = function
-
-    if jac_function is None:
-        # use numerical Jacobian if analytical is not provided
-        jac_fun = lambda p: jacobian_approx_t(p, f=fun)
-    else:
-        jac_fun = lambda p: jac_function(p, *args)
-    
-    assert len(p.shape) == 2, 'parameter tensor is supposed to have 2 dims, but has %s' % str(len(p.shape))
-
-    f = fun(p)
-    assert len(f.shape) == 3, 'residual tensor is supposed to have 3 dims, but has %s' % str(len(f.shape))
-
-    j = jac_fun(p)
-    assert len(j.shape) == 4, 'jacobian tensor is supposed to have 4 dims, but has %s' % str(len(j.shape))
-
-    # use weights of ones as default
-    wvec = torch.ones(f.shape[1], dtype=p.dtype, device=p.device, requires_grad=False) if wvec is None else wvec
-    assert len(wvec) == f.shape[1], 'weights vector length of %s is supposed to match cost number which is %s' % (str(len(wvec)), str(f.shape[1]))
-
-    return True
 
 def lsq_gna_parallel_plain(
         p: torch.Tensor,
         function: Callable, 
         jac_function: Callable,
         wvec: torch.Tensor,
         l: float = 1.,
@@ -161,17 +121,12 @@
     :param function: user-provided function which takes p (and additional arguments) as input
     :param jac_fun: user-provided Jacobian function which takes p (and additional arguments) as input
     :param wvec: weights vector used in reduction of multiple costs
     :param l: learning rate
     :return: list of results
     """
 
-    f = function(p)
-    j = jac_function(p)
-    gc = torch.einsum('bcnp,bcnp->bcp', j, f[..., None])
-    Hc = torch.einsum('bcnp,bcni->bcpi', j, j)
-    g = torch.einsum('bcp,c->bp', gc, wvec)
-    H = torch.einsum('bcpi,c->bpi', Hc, wvec)
-    h = -l*torch.linalg.lstsq(H, g, rcond=None, driver=None)[0]
-    p += h
-    
+    p, f, g, H = newton_step_parallel(p, function, jac_function, wvec)
+    h = torch.linalg.lstsq(H.double(), g.double(), rcond=None, driver=None)[0].to(dtype=p.dtype)
+    p -= l*h
+
     return p, f, g, h
```

### Comparing `torchimize-0.0.8/torchimize/functions/jacobian.py` & `torchimize-0.0.9/torchimize/functions/jacobian.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/torchimize/functions/lma_fun.py` & `torchimize-0.0.9/torchimize/functions/lma_fun.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/torchimize/functions/lma_fun_parallel.py` & `torchimize-0.0.9/torchimize/functions/lma_fun_parallel.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import torch 
 from typing import Union, Callable, List, Tuple
 
 from torchimize.functions.jacobian import jacobian_approx_t
+from torchimize.functions.newton_parallel import newton_step_parallel
 
 
 def lsq_lma_parallel(
         p: torch.Tensor,
         function: Callable, 
         jac_function: Callable = None,
         args: Union[Tuple, List] = (),
@@ -86,17 +87,18 @@
         lm_dg_step = lambda H, D: D * torch.max(torch.maximum(H.diagonal(dim1=2), D.diagonal(dim1=2)), dim=1)[0][..., None, None]
 
     p_list = []
     f_prev = torch.zeros(1, device=p.device, dtype=p.dtype)
     while len(p_list) < max_iter:
 
         # levenberg-marquardt step
-        p, f, g, H = newton_2nd_order_step(p, fun, jac_fun, wvec)
+        p, f, g, H = newton_step_parallel(p, fun, jac_fun, wvec)
         D = lm_dg_step(H, D)
-        h = -torch.linalg.lstsq(H+u[:, None, None]*D, g, rcond=None, driver=None)[0]
+        Hu = H+u[:, None, None]*D
+        h = -torch.linalg.lstsq(Hu.double(), g.double(), rcond=None, driver=None)[0].to(dtype=p.dtype)
         f_h = fun(p+h)
         rho_nom = torch.einsum('bcp,bci->bc', f, f).sum(1) - torch.einsum('bcp,bci->bc', f_h, f_h).sum(1)
         rho_denom = torch.einsum('bnp,bni->bi', h[..., None], (u[:, None]*h-g)[..., None])[..., 0]
         rho = rho_nom / rho_denom
         rho[rho_denom==0] = sinf[(rho_nom > 0).type(torch.int64)][rho_denom==0]
         u, v = lm_uv_step(rho, u, v)
         p[rho>0, ...] += h[rho>0, ...]
@@ -139,34 +141,7 @@
         gama: float,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
 
     u[rho < rho1] *= beta
     u[rho > rho2] /= gama
 
     return u, v
-
-
-def newton_2nd_order_step(        
-        p: torch.Tensor,
-        function: Callable,
-        jac_function: Callable,
-        wvec: torch.Tensor,
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
-
-    """
-    Newton second order step function for parallel least-squares fitting of non-linear functions
-
-    :param p: current guess
-    :param function: user-provided function which takes p (and additional arguments) as input
-    :param jac_fun: user-provided Jacobian function which takes p (and additional arguments) as input
-    :param wvec: weights vector used in reduction of multiple costs
-    :return: list of results
-    """
-
-    f = function(p)
-    j = jac_function(p)
-    gc = torch.einsum('bcnp,bcnp->bcp', j, f[..., None])
-    Hc = torch.einsum('bcnp,bcni->bcpi', j, j)
-    g = torch.einsum('bcp,c->bp', gc, wvec)
-    H = torch.einsum('bcpi,c->bpi', Hc, wvec)
-
-    return p, f, g, H
```

### Comparing `torchimize-0.0.8/torchimize/optimizer/gna_opt.py` & `torchimize-0.0.9/torchimize/optimizer/gna_opt.py`

 * *Files identical despite different names*

### Comparing `torchimize-0.0.8/torchimize.egg-info/PKG-INFO` & `torchimize-0.0.9/torchimize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchimize
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimization Algorithms using Pytorch
 Home-page: http://github.com/hahnec/torchimize
 Author: Christopher Hahne
 Author-email: inbox@christopherhahne.de
 License: GNU GPL V3.0
 Description: torchimize contains implementations of the Gauss-Newton and Levenberg-Marquardt optimization algorithms using the PyTorch library. The main motivation for this project is to enable convex optimization on GPUs based on the torch.Tensor class, which (as of 2022) is widely used in the deep learning field. This package features the capability to minimize several least-squares optimization problems at each loop iteration in parallel.
 Keywords: pytorch torch optimization mathematical linear programming gauss newton levenberg marquardt
```

### Comparing `torchimize-0.0.8/torchimize.egg-info/SOURCES.txt` & `torchimize-0.0.9/torchimize.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 torchimize.egg-info/PKG-INFO
 torchimize.egg-info/SOURCES.txt
 torchimize.egg-info/dependency_links.txt
 torchimize.egg-info/not-zip-safe
 torchimize.egg-info/requires.txt
 torchimize.egg-info/top_level.txt
 torchimize/functions/__init__.py
+torchimize/functions/fun_dims.py
 torchimize/functions/gna_fun.py
 torchimize/functions/gna_fun_parallel.py
 torchimize/functions/jacobian.py
 torchimize/functions/lma_fun.py
 torchimize/functions/lma_fun_parallel.py
+torchimize/functions/newton_parallel.py
 torchimize/optimizer/__init__.py
 torchimize/optimizer/gna_opt.py
```

