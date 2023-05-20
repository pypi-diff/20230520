# Comparing `tmp/denoising-diffusion-pytorch-1.5.8.tar.gz` & `tmp/denoising-diffusion-pytorch-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.5.8.tar", last modified: Mon May  8 05:12:44 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.6.0.tar", last modified: Sat May 20 01:58:40 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.5.8.tar` & `denoising-diffusion-pytorch-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:58:40.083531 denoising-diffusion-pytorch-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 01:58:40.083531 denoising-diffusion-pytorch-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:58:40.083531 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30764 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:58:40.083531 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 01:58:40.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 01:58:40.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:58:40.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 01:58:40.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 01:58:40.000000 denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 01:58:40.083531 denoising-diffusion-pytorch-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 01:58:29.000000 denoising-diffusion-pytorch-1.6.0/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.5.8/LICENSE` & `denoising-diffusion-pytorch-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/PKG-INFO` & `denoising-diffusion-pytorch-1.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.8
+Version: 1.6.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.8/README.md` & `denoising-diffusion-pytorch-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -307,7 +307,15 @@
 ```bibtex
 @inproceedings{Hang2023EfficientDT,
     title   = {Efficient Diffusion Training via Min-SNR Weighting Strategy},
     author  = {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han Hu and Xin Geng and Baining Guo},
     year    = {2023}
 }
 ```
+
+```bibtex
+@inproceedings{Lin2023CommonDN,
+    title   = {Common Diffusion Noise Schedules and Sample Steps are Flawed},
+    author  = {Shanchuan Lin and Bingchen Liu and Jiashi Li and Xiao Yang},
+    year    = {2023}
+}
+```
```

#### html2text {}

```diff
@@ -104,8 +104,11 @@
 ```bibtex @misc{https://doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/
 ARXIV.2302.01327}, url = {https://arxiv.org/abs/2302.01327}, author = {Kumar,
 Manoj and Dehghani, Mostafa and Houlsby, Neil}, title = {Dual PatchNorm},
 publisher = {arXiv}, year = {2023}, copyright = {Creative Commons Attribution
 4.0 International} } ``` ```bibtex @inproceedings{Hang2023EfficientDT, title =
 {Efficient Diffusion Training via Min-SNR Weighting Strategy}, author =
 {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han
-Hu and Xin Geng and Baining Guo}, year = {2023} } ```
+Hu and Xin Geng and Baining Guo}, year = {2023} } ``` ```bibtex @inproceedings
+{Lin2023CommonDN, title = {Common Diffusion Noise Schedules and Sample Steps
+are Flawed}, author = {Shanchuan Lin and Bingchen Liu and Jiashi Li and Xiao
+Yang}, year = {2023} } ```
```

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,30 +420,30 @@
     as proposed in https://openreview.net/forum?id=-NEXDKk8gZ
     """
     steps = timesteps + 1
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     alphas_cumprod = torch.cos((t + s) / (1 + s) * math.pi * 0.5) ** 2
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 0.999)
+    return torch.clip(betas, 0, 1.)
 
 def sigmoid_beta_schedule(timesteps, start = -3, end = 3, tau = 1, clamp_min = 1e-5):
     """
     sigmoid schedule
     proposed in https://arxiv.org/abs/2212.11972 - Figure 8
     better for images > 64x64, when used during training
     """
     steps = timesteps + 1
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     v_start = torch.tensor(start / tau).sigmoid()
     v_end = torch.tensor(end / tau).sigmoid()
     alphas_cumprod = (-((t * (end - start) + start) / tau).sigmoid() + v_end) / (v_end - v_start)
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 0.999)
+    return torch.clip(betas, 0, 1.)
 
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
```

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     as proposed in https://openreview.net/forum?id=-NEXDKk8gZ
     """
     steps = timesteps + 1
     x = torch.linspace(0, timesteps, steps, dtype = torch.float64)
     alphas_cumprod = torch.cos(((x / timesteps) + s) / (1 + s) * math.pi * 0.5) ** 2
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 0.999)
+    return torch.clip(betas, 0, 1.)
 
 class GaussianDiffusion1D(nn.Module):
     def __init__(
         self,
         model,
         *,
         seq_length,
```

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.8
+Version: 1.6.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.6.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.8/setup.py` & `denoising-diffusion-pytorch-1.6.0/setup.py`

 * *Files identical despite different names*

