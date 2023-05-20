# Comparing `tmp/torch-pp-0.0.1.dev0.tar.gz` & `tmp/torch-pp-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pp-0.0.1.dev0.tar", last modified: Sat May 20 03:18:06 2023, max compression
+gzip compressed data, was "torch-pp-0.0.2.dev0.tar", last modified: Sat May 20 19:35:29 2023, max compression
```

## Comparing `torch-pp-0.0.1.dev0.tar` & `torch-pp-0.0.2.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 03:18:06.655287 torch-pp-0.0.1.dev0/
--rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.1.dev0/LICENSE
--rw-rw-r--   0 roman     (1000) roman     (1000)      243 2023-05-20 03:18:06.655287 torch-pp-0.0.1.dev0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.1.dev0/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-05-20 03:18:06.655287 torch-pp-0.0.1.dev0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)      303 2023-05-20 03:18:06.000000 torch-pp-0.0.1.dev0/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 03:18:06.655287 torch-pp-0.0.1.dev0/torch_pp/
--rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.1.dev0/torch_pp/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3799 2023-05-20 02:36:16.000000 torch-pp-0.0.1.dev0/torch_pp/standardscaler.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 03:18:06.655287 torch-pp-0.0.1.dev0/torch_pp.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)      243 2023-05-20 03:18:06.000000 torch-pp-0.0.1.dev0/torch_pp.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      202 2023-05-20 03:18:06.000000 torch-pp-0.0.1.dev0/torch_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-05-20 03:18:06.000000 torch-pp-0.0.1.dev0/torch_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-05-20 03:18:06.000000 torch-pp-0.0.1.dev0/torch_pp.egg-info/top_level.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.2.dev0/LICENSE
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.2.dev0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-05-20 19:35:28.000000 torch-pp-0.0.2.dev0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/torch_pp/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.2.dev0/torch_pp/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3741 2023-05-20 19:35:11.000000 torch-pp-0.0.2.dev0/torch_pp/standardscaler.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/torch_pp.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      202 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/top_level.txt
```

### Comparing `torch-pp-0.0.1.dev0/LICENSE` & `torch-pp-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pp-0.0.1.dev0/torch_pp/standardscaler.py` & `torch-pp-0.0.2.dev0/torch_pp/standardscaler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,19 @@
 import torch
 
 
-def incremental_mean_and_var(x: torch.Tensor, last_mean: torch.Tensor, last_variance: torch.Tensor,
-                             last_sample_count: int):
-    new_sample_count = x.shape[0]
-    n_features = x.shape[1]
-    last_sum = last_mean.clone()
-    last_sum = torch.mul(last_sum, float(last_sample_count))
-    new_sum = torch.zeros(n_features)
-    for i in range(new_sample_count):
-        new_sum = torch.add(new_sum, x[i])
-
-    updated_sample_count = last_sample_count + new_sample_count
-    updated_mean = torch.add(last_sum, new_sum)
-    updated_mean = torch.mul(updated_mean, 1. / float(updated_sample_count))
-
-    new_unnormalized_variance = torch.zeros(n_features)
-    new_mean = torch.mul(new_sum, 1. / float(new_sample_count))
-
-    for i in range(new_sample_count):
-        tmp = torch.sub(x[i], new_mean)
-        tmp = torch.pow(tmp, 2)
-        new_unnormalized_variance = torch.add(new_unnormalized_variance, tmp)
-
-    if last_sample_count == 0:
-        updated_unnormalized_variance = new_unnormalized_variance.clone()
-    else:
-        last_over_new_count = float(last_sample_count) / float(new_sample_count)
-        last_unnormalized_variance = last_variance.clone()
-        last_unnormalized_variance = torch.mul(last_unnormalized_variance, float(last_sample_count))
-        tmp = last_sum.clone()
-        tmp = torch.mul(tmp, 1. / last_over_new_count)
-        tmp = torch.add(tmp, new_sum)
-        tmp = torch.pow(tmp, 2)
-        tmp = torch.mul(tmp, last_over_new_count / float(updated_sample_count))
-
-        updated_unnormalized_variance = last_unnormalized_variance.clone()
-        updated_unnormalized_variance = torch.add(updated_unnormalized_variance, new_unnormalized_variance)
-        updated_unnormalized_variance = torch.add(updated_unnormalized_variance, tmp)
-
-    updated_variance = updated_unnormalized_variance.clone()
-    updated_variance = torch.mul(updated_variance, 1. / float(updated_sample_count))
-
-    return updated_mean, updated_variance, updated_sample_count
-
-
-class StandardScaler(torch.nn.Module):
+class StandardScaler:
     n_samples_seen = 0
     scale, mean, var = None, None, None
 
-    def __init__(self, with_mean=True, with_std=True, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, with_mean=True, with_std=True):
         self.with_mean = with_mean
         self.with_std = with_std
 
-    def forward(self, _input: torch.Tensor) -> torch.Tensor:
+    def fit_transform(self, _input: torch.Tensor) -> torch.Tensor:
         self.partial_fit(_input)
         return self.transform(_input)
 
     def reset(self):
         self.n_samples_seen = 0
         return self
 
@@ -77,25 +32,69 @@
         def fn(value):
             return value if value != 0 else 1
 
         self.scale = self.var.apply_(fn)
         self.scale = torch.sqrt(self.scale)
 
     def transform(self, x: torch.Tensor):
-        return self.__scale(x, lambda v, mean, scale: (v - mean) / scale)
+        return self.__transform(x, lambda v, mean, scale: (v - mean) / scale)
 
     def inverse_transform(self, x: torch.Tensor):
-        return self.__scale(x, lambda v, mean, scale: mean + v * scale)
+        return self.__transform(x, lambda v, mean, scale: mean + v * scale)
 
-    def __scale(self, x: torch.Tensor, fn):
+    def __transform(self, x: torch.Tensor, fn):
         x_out = x.clone()
         n_features = x.shape[1]
         for i in range(n_features):
             mean, scale = 0., 1.
             if self.with_mean:
                 mean = self.mean[i]
             if self.with_std:
                 scale = self.scale[i]
             for j in range(self.n_samples_seen):
                 x_out[j, i] = fn(x[j, i], mean, scale)
 
         return x_out
+
+
+def incremental_mean_and_var(x: torch.Tensor, last_mean: torch.Tensor, last_variance: torch.Tensor,
+                             last_sample_count: int):
+    new_sample_count = x.shape[0]
+    n_features = x.shape[1]
+    last_sum = last_mean.clone()
+    last_sum = torch.mul(last_sum, float(last_sample_count))
+    new_sum = torch.zeros(n_features)
+    for i in range(new_sample_count):
+        new_sum = torch.add(new_sum, x[i])
+
+    updated_sample_count = last_sample_count + new_sample_count
+    updated_mean = torch.add(last_sum, new_sum)
+    updated_mean = torch.mul(updated_mean, 1. / float(updated_sample_count))
+
+    new_unnormalized_variance = torch.zeros(n_features)
+    new_mean = torch.mul(new_sum, 1. / float(new_sample_count))
+
+    for i in range(new_sample_count):
+        tmp = torch.sub(x[i], new_mean)
+        tmp = torch.pow(tmp, 2)
+        new_unnormalized_variance = torch.add(new_unnormalized_variance, tmp)
+
+    if last_sample_count == 0:
+        updated_unnormalized_variance = new_unnormalized_variance.clone()
+    else:
+        last_over_new_count = float(last_sample_count) / float(new_sample_count)
+        last_unnormalized_variance = last_variance.clone()
+        last_unnormalized_variance = torch.mul(last_unnormalized_variance, float(last_sample_count))
+        tmp = last_sum.clone()
+        tmp = torch.mul(tmp, 1. / last_over_new_count)
+        tmp = torch.add(tmp, new_sum)
+        tmp = torch.pow(tmp, 2)
+        tmp = torch.mul(tmp, last_over_new_count / float(updated_sample_count))
+
+        updated_unnormalized_variance = last_unnormalized_variance.clone()
+        updated_unnormalized_variance = torch.add(updated_unnormalized_variance, new_unnormalized_variance)
+        updated_unnormalized_variance = torch.add(updated_unnormalized_variance, tmp)
+
+    updated_variance = updated_unnormalized_variance.clone()
+    updated_variance = torch.mul(updated_variance, 1. / float(updated_sample_count))
+
+    return updated_mean, updated_variance, updated_sample_count
```

