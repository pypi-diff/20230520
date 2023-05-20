# Comparing `tmp/denoising-diffusion-pytorch-1.6.1.tar.gz` & `tmp/denoising-diffusion-pytorch-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.6.1.tar", last modified: Sat May 20 15:13:55 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.6.2.tar", last modified: Sat May 20 16:40:31 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.6.1.tar` & `denoising-diffusion-pytorch-1.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:13:55.748082 denoising-diffusion-pytorch-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 15:13:55.748082 denoising-diffusion-pytorch-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:13:55.748082 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29256 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36915 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36395 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:13:55.748082 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 15:13:55.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 15:13:55.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:13:55.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 15:13:55.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 15:13:55.000000 denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:13:55.748082 denoising-diffusion-pytorch-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 15:13:43.000000 denoising-diffusion-pytorch-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.6.1/LICENSE` & `denoising-diffusion-pytorch-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/PKG-INFO` & `denoising-diffusion-pytorch-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.1
+Version: 1.6.2
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.1/README.md` & `denoising-diffusion-pytorch-1.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     dim = 64,
     dim_mults = (1, 2, 4, 8)
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
-    timesteps = 1000    # number of steps
+    timesteps = 1000,   # number of steps
+    loss_type = 'l1'    # L1 or L2
 )
 
 training_images = torch.rand(8, 3, 128, 128) # images are normalized from 0 to 1
 loss = diffusion(training_images)
 loss.backward()
 # after a lot of training
 
@@ -60,15 +61,16 @@
     dim_mults = (1, 2, 4, 8)
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
     timesteps = 1000,           # number of steps
-    sampling_timesteps = 250    # number of sampling timesteps (using ddim for faster inference [see citation for ddim paper])
+    sampling_timesteps = 250,   # number of sampling timesteps (using ddim for faster inference [see citation for ddim paper])
+    loss_type = 'l1'            # L1 or L2
 )
 
 trainer = Trainer(
     diffusion,
     'path/to/your/images',
     train_batch_size = 32,
     train_lr = 8e-5,
@@ -142,19 +144,17 @@
 
 # after a lot of training
 
 sampled_seq = diffusion.sample(batch_size = 4)
 sampled_seq.shape # (4, 32, 128)
 
 ```
-
 `Trainer1D` does not evaluate the generated samples in any way since the type of data is not known. 
 You could consider adding a suitable metric to the training loop yourself after doing an editable install of this package
 `pip install -e .`.
-
 ## Citations
 
 ```bibtex
 @inproceedings{NEURIPS2020_4c5bcfec,
     author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
     booktitle   = {Advances in Neural Information Processing Systems},
     editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
@@ -307,15 +307,7 @@
 ```bibtex
 @inproceedings{Hang2023EfficientDT,
     title   = {Efficient Diffusion Training via Min-SNR Weighting Strategy},
     author  = {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han Hu and Xin Geng and Baining Guo},
     year    = {2023}
 }
 ```
-
-```bibtex
-@inproceedings{Lin2023CommonDN,
-    title   = {Common Diffusion Noise Schedules and Sample Steps are Flawed},
-    author  = {Shanchuan Lin and Bingchen Liu and Jiashi Li and Xiao Yang},
-    year    = {2023}
-}
-```
```

#### html2text {}

```diff
@@ -9,39 +9,40 @@
 Research Scientists / Engineers from ð¤_Huggingface Update: Turns out none of
 the technicalities really matters at all | "Cold_Diffusion"_paper | Muse [./
 images/sample.png][Image] [![PyPI version](https://badge.fury.io/py/denoising-
 diffusion-pytorch.svg)](https://badge.fury.io/py/denoising-diffusion-pytorch)
 ## Install ```bash $ pip install denoising_diffusion_pytorch ``` ## Usage
 ```python import torch from denoising_diffusion_pytorch import Unet,
 GaussianDiffusion model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) ) diffusion
-= GaussianDiffusion( model, image_size = 128, timesteps = 1000 # number of
-steps ) training_images = torch.rand(8, 3, 128, 128) # images are normalized
-from 0 to 1 loss = diffusion(training_images) loss.backward() # after a lot of
-training sampled_images = diffusion.sample(batch_size = 4) sampled_images.shape
-# (4, 3, 128, 128) ``` Or, if you simply want to pass in a folder name and the
-desired image dimensions, you can use the `Trainer` class to easily train a
-model. ```python from denoising_diffusion_pytorch import Unet,
-GaussianDiffusion, Trainer model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) )
-diffusion = GaussianDiffusion( model, image_size = 128, timesteps = 1000, #
-number of steps sampling_timesteps = 250 # number of sampling timesteps (using
-ddim for faster inference [see citation for ddim paper]) ) trainer = Trainer
-( diffusion, 'path/to/your/images', train_batch_size = 32, train_lr = 8e-5,
-train_num_steps = 700000, # total training steps gradient_accumulate_every = 2,
-# gradient accumulation steps ema_decay = 0.995, # exponential moving average
-decay amp = True, # turn on mixed precision calculate_fid = True # whether to
-calculate fid during training ) trainer.train() ``` Samples and model
-checkpoints will be logged to `./results` periodically ## Multi-GPU Training
-The `Trainer` class is now equipped with ð¤_Accelerator. You can easily do
-multi-gpu training in two steps using their `accelerate` CLI At the project
-root directory, where the training script is, run ```python $ accelerate config
-``` Then, in the same directory ```python $ accelerate launch train.py ``` ##
-Miscellaneous ### 1D Sequence By popular request, a 1D Unet + Gaussian
-Diffusion implementation. ```python import torch from
-denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D model
-= Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
+= GaussianDiffusion( model, image_size = 128, timesteps = 1000, # number of
+steps loss_type = 'l1' # L1 or L2 ) training_images = torch.rand(8, 3, 128,
+128) # images are normalized from 0 to 1 loss = diffusion(training_images)
+loss.backward() # after a lot of training sampled_images = diffusion.sample
+(batch_size = 4) sampled_images.shape # (4, 3, 128, 128) ``` Or, if you simply
+want to pass in a folder name and the desired image dimensions, you can use the
+`Trainer` class to easily train a model. ```python from
+denoising_diffusion_pytorch import Unet, GaussianDiffusion, Trainer model =
+Unet( dim = 64, dim_mults = (1, 2, 4, 8) ) diffusion = GaussianDiffusion
+( model, image_size = 128, timesteps = 1000, # number of steps
+sampling_timesteps = 250, # number of sampling timesteps (using ddim for faster
+inference [see citation for ddim paper]) loss_type = 'l1' # L1 or L2 ) trainer
+= Trainer( diffusion, 'path/to/your/images', train_batch_size = 32, train_lr =
+8e-5, train_num_steps = 700000, # total training steps
+gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
+# exponential moving average decay amp = True, # turn on mixed precision
+calculate_fid = True # whether to calculate fid during training ) trainer.train
+() ``` Samples and model checkpoints will be logged to `./results` periodically
+## Multi-GPU Training The `Trainer` class is now equipped with ð¤
+Accelerator. You can easily do multi-gpu training in two steps using their
+`accelerate` CLI At the project root directory, where the training script is,
+run ```python $ accelerate config ``` Then, in the same directory ```python $
+accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
+request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
+model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
 GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000, objective =
 'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are normalized
 from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or using trainer
 trainer = Trainer1D( diffusion, dataset = training_seq, train_batch_size = 32,
 train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
@@ -103,11 +104,8 @@
 ```bibtex @misc{https://doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/
 ARXIV.2302.01327}, url = {https://arxiv.org/abs/2302.01327}, author = {Kumar,
 Manoj and Dehghani, Mostafa and Houlsby, Neil}, title = {Dual PatchNorm},
 publisher = {arXiv}, year = {2023}, copyright = {Creative Commons Attribution
 4.0 International} } ``` ```bibtex @inproceedings{Hang2023EfficientDT, title =
 {Efficient Diffusion Training via Min-SNR Weighting Strategy}, author =
 {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han
-Hu and Xin Geng and Baining Guo}, year = {2023} } ``` ```bibtex @inproceedings
-{Lin2023CommonDN, title = {Common Diffusion Noise Schedules and Sample Steps
-are Flawed}, author = {Shanchuan Lin and Bingchen Liu and Jiashi Li and Xiao
-Yang}, year = {2023} } ```
+Hu and Xin Geng and Baining Guo}, year = {2023} } ```
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import copy
 from pathlib import Path
 from random import random
-from functools import partial, wraps
+from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 
@@ -371,35 +371,23 @@
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     def forward_with_cond_scale(
         self,
         *args,
         cond_scale = 1.,
-        rescale_phi = 0.,
         **kwargs
     ):
         logits = self.forward(*args, cond_drop_prob = 0., **kwargs)
 
         if cond_scale == 1:
             return logits
 
         null_logits = self.forward(*args, cond_drop_prob = 1., **kwargs)
-        scaled_logits = null_logits + (logits - null_logits) * cond_scale
-
-        if rescale_phi <= 0:
-            return scaled_logits
-
-        # rescaling proposed in https://arxiv.org/abs/2305.08891 to prevent over-saturation
-        # works for both pixel and latent space, as opposed to only pixel space with the technique from Imagen
-        # they found 0.7 to work well empirically with a conditional scale of 6.
-
-        std_fn = partial(torch.std, dim = tuple(range(1, scaled_logits.ndim)), keepdim = True)
-        rescaled_logits = scaled_logits * (std_fn(logits) / std_fn(scaled_logits))
-        return rescaled_logits * rescale_phi + (1 - rescale_phi) * scaled_logits
+        return null_logits + (logits - null_logits) * cond_scale
 
     def forward(
         self,
         x,
         time,
         classes,
         cond_drop_prob = None
@@ -465,41 +453,14 @@
 # gaussian diffusion trainer class
 
 def extract(a, t, x_shape):
     b, *_ = t.shape
     out = a.gather(-1, t)
     return out.reshape(b, *((1,) * (len(x_shape) - 1)))
 
-def enforce_zero_terminal_snr(schedule_fn):
-    # algorithm 1 in https://arxiv.org/abs/2305.08891
-
-    @wraps(schedule_fn)
-    def inner(*args, **kwargs):
-        betas = schedule_fn(*args, **kwargs)
-        alphas = 1. - betas
-
-        alphas_cumprod = torch.cumprod(alphas, dim = 0)
-        alphas_cumprod = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
-
-        alphas_cumprod_sqrt = torch.sqrt(alphas_cumprod)
-
-        terminal_snr = alphas_cumprod_sqrt[-1].clone()
-
-        alphas_cumprod_sqrt -= terminal_snr # enforce zero terminal snr
-        alphas_cumprod_sqrt *= 1. / (1. - terminal_snr)
-
-        alphas_cumprod = alphas_cumprod_sqrt ** 2
-        alphas = alphas_cumprod[1:] / alphas_cumprod[:-1]
-        betas = 1. - alphas
-
-        return betas
-
-    return inner
-
-@enforce_zero_terminal_snr
 def linear_beta_schedule(timesteps):
     scale = 1000 / timesteps
     beta_start = scale * 0.0001
     beta_end = scale * 0.02
     return torch.linspace(beta_start, beta_end, timesteps, dtype = torch.float64)
 
 def cosine_beta_schedule(timesteps, s = 0.008):
@@ -508,15 +469,15 @@
     as proposed in https://openreview.net/forum?id=-NEXDKk8gZ
     """
     steps = timesteps + 1
     x = torch.linspace(0, timesteps, steps, dtype = torch.float64)
     alphas_cumprod = torch.cos(((x / timesteps) + s) / (1 + s) * math.pi * 0.5) ** 2
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 1.)
+    return torch.clip(betas, 0, 0.999)
 
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
@@ -641,16 +602,16 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, classes, cond_scale = 6., rescale_phi = 0.7, clip_x_start = False):
-        model_output = self.model.forward_with_cond_scale(x, t, classes, cond_scale = cond_scale, rescale_phi = rescale_phi)
+    def model_predictions(self, x, t, classes, cond_scale = 3., clip_x_start = False):
+        model_output = self.model.forward_with_cond_scale(x, t, classes, cond_scale = cond_scale)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
@@ -674,38 +635,38 @@
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
 
     @torch.no_grad()
-    def p_sample(self, x, t: int, classes, cond_scale = 6., rescale_phi = 0.7, clip_denoised = True):
+    def p_sample(self, x, t: int, classes, cond_scale = 3., clip_denoised = True):
         b, *_, device = *x.shape, x.device
         batched_times = torch.full((x.shape[0],), t, device = x.device, dtype = torch.long)
         model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, classes = classes, cond_scale = cond_scale, clip_denoised = clip_denoised)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
-    def p_sample_loop(self, classes, shape, cond_scale = 6., rescale_phi = 0.7):
+    def p_sample_loop(self, classes, shape, cond_scale = 3.):
         batch, device = shape[0], self.betas.device
 
         img = torch.randn(shape, device=device)
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             img, x_start = self.p_sample(img, t, classes, cond_scale)
 
         img = unnormalize_to_zero_to_one(img)
         return img
 
     @torch.no_grad()
-    def ddim_sample(self, classes, shape, cond_scale = 6., rescale_phi = 0.7, clip_denoised = True):
+    def ddim_sample(self, classes, shape, cond_scale = 3., clip_denoised = True):
         batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps=sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
@@ -761,14 +722,23 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
+    @property
+    def loss_fn(self):
+        if self.loss_type == 'l1':
+            return F.l1_loss
+        elif self.loss_type == 'l2':
+            return F.mse_loss
+        else:
+            raise ValueError(f'invalid loss type {self.loss_type}')
+
     def p_losses(self, x_start, t, *, classes, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -783,15 +753,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = F.mse_loss(model_out, target, reduction = 'none')
+        loss = self.loss_fn(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 class ContinuousTimeGaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         channels = 3,
+        loss_type = 'l1',
         noise_schedule = 'linear',
         num_sample_steps = 500,
         clip_sample_denoised = True,
         learned_schedule_net_hidden_dim = 1024,
         learned_noise_schedule_frac_gradient = 1.,   # between 0 and 1, determines what percentage of gradients go back, so one can update the learned noise schedule more slowly
         min_snr_loss_weight = False,
         min_snr_gamma = 5
@@ -133,14 +134,16 @@
         # image dimensions
 
         self.channels = channels
         self.image_size = image_size
 
         # continuous noise schedule related stuff
 
+        self.loss_type = loss_type
+
         if noise_schedule == 'linear':
             self.log_snr = beta_linear_log_snr
         elif noise_schedule == 'cosine':
             self.log_snr = alpha_cosine_log_snr
         elif noise_schedule == 'learned':
             log_snr_max, log_snr_min = [beta_linear_log_snr(torch.tensor([time])).item() for time in (0., 1.)]
 
@@ -163,14 +166,23 @@
         self.min_snr_loss_weight = min_snr_loss_weight
         self.min_snr_gamma = min_snr_gamma
 
     @property
     def device(self):
         return next(self.model.parameters()).device
 
+    @property
+    def loss_fn(self):
+        if self.loss_type == 'l1':
+            return F.l1_loss
+        elif self.loss_type == 'l2':
+            return F.mse_loss
+        else:
+            raise ValueError(f'invalid loss type {self.loss_type}')
+
     def p_mean_variance(self, x, time, time_next):
         # reviewer found an error in the equation in the paper (missing sigma)
         # following - https://openreview.net/forum?id=2LdBqxc1Yv&noteId=rIQgH0zKsRt
 
         log_snr = self.log_snr(time)
         log_snr_next = self.log_snr(time_next)
         c = -expm1(log_snr - log_snr_next)
@@ -250,15 +262,15 @@
 
     def p_losses(self, x_start, times, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         x, log_snr = self.q_sample(x_start = x_start, times = times, noise = noise)
         model_out = self.model(x, log_snr)
 
-        losses = F.mse_loss(model_out, noise, reduction = 'none')
+        losses = self.loss_fn(model_out, noise, reduction = 'none')
         losses = reduce(losses, 'b ... -> b', 'mean')
 
         if self.min_snr_loss_weight:
             snr = log_snr.exp()
             loss_weight = snr.clamp(min = self.min_snr_gamma) / snr
             losses = losses * loss_weight
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 import math
 import copy
 from pathlib import Path
 from random import random
-from functools import partial, wraps
+from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
-
 from torchvision import transforms as T, utils
 
-from einops import rearrange, reduce, repeat
+from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
-import numpy as np
-from pytorch_fid.inception import InceptionV3
-from pytorch_fid.fid_score import calculate_frechet_distance
-
-from denoising_diffusion_pytorch.version import __version__
+# from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
 
 # helpers functions
 
@@ -64,19 +59,14 @@
     return arr
 
 def convert_image_to_fn(img_type, image):
     if image.mode != img_type:
         return image.convert(img_type)
     return image
 
-def extract(a, t, x_shape):
-    b, *_ = t.shape
-    out = a.gather(-1, t)
-    return out.reshape(b, *((1,) * (len(x_shape) - 1)))
-
 # normalization functions
 
 def normalize_to_neg_one_to_one(img):
     return img * 2 - 1
 
 def unnormalize_to_zero_to_one(t):
     return (t + 1) * 0.5
@@ -399,43 +389,21 @@
             x = upsample(x)
 
         x = torch.cat((x, r), dim = 1)
 
         x = self.final_res_block(x, t)
         return self.final_conv(x)
 
-# scheduling functions
-
-def enforce_zero_terminal_snr(schedule_fn):
-    # algorithm 1 in https://arxiv.org/abs/2305.08891
-
-    @wraps(schedule_fn)
-    def inner(*args, **kwargs):
-        betas = schedule_fn(*args, **kwargs)
-        alphas = 1. - betas
-
-        alphas_cumprod = torch.cumprod(alphas, dim = 0)
-        alphas_cumprod = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
-
-        alphas_cumprod_sqrt = torch.sqrt(alphas_cumprod)
-
-        terminal_snr = alphas_cumprod_sqrt[-1].clone()
-
-        alphas_cumprod_sqrt -= terminal_snr # enforce zero terminal snr
-        alphas_cumprod_sqrt *= 1. / (1. - terminal_snr)
-
-        alphas_cumprod = alphas_cumprod_sqrt ** 2
-        alphas = alphas_cumprod[1:] / alphas_cumprod[:-1]
-        betas = 1. - alphas
-
-        return betas
+# gaussian diffusion trainer class
 
-    return inner
+def extract(a, t, x_shape):
+    b, *_ = t.shape
+    out = a.gather(-1, t)
+    return out.reshape(b, *((1,) * (len(x_shape) - 1)))
 
-@enforce_zero_terminal_snr
 def linear_beta_schedule(timesteps):
     """
     linear schedule, proposed in original ddpm paper
     """
     scale = 1000 / timesteps
     beta_start = scale * 0.0001
     beta_end = scale * 0.02
@@ -447,84 +415,82 @@
     as proposed in https://openreview.net/forum?id=-NEXDKk8gZ
     """
     steps = timesteps + 1
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     alphas_cumprod = torch.cos((t + s) / (1 + s) * math.pi * 0.5) ** 2
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 1.)
+    return torch.clip(betas, 0, 0.999)
 
-@enforce_zero_terminal_snr
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
-    return torch.clip(betas, 0, 1.)
-
-# gaussian diffusion trainer class
+    return torch.clip(betas, 0, 0.999)
+    
 
+    
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
+        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
-        min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
+        min_snr_loss_weight = False,
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
         self.model = model
-
         self.channels = self.model.channels
         self.self_condition = self.model.self_condition
 
         self.image_size = image_size
 
         self.objective = objective
 
         assert objective in {'pred_noise', 'pred_x0', 'pred_v'}, 'objective must be either pred_noise (predict noise) or pred_x0 (predict image start) or pred_v (predict v [v-parameterization as defined in appendix D of progressive distillation paper, used in imagen-video successfully])'
 
-        if callable(beta_schedule):
-            beta_schedule_fn = beta_schedule
-        elif beta_schedule == 'linear':
+        if beta_schedule == 'linear':
             beta_schedule_fn = linear_beta_schedule
         elif beta_schedule == 'cosine':
             beta_schedule_fn = cosine_beta_schedule
         elif beta_schedule == 'sigmoid':
             beta_schedule_fn = sigmoid_beta_schedule
         else:
             raise ValueError(f'unknown beta schedule {beta_schedule}')
 
         betas = beta_schedule_fn(timesteps, **schedule_fn_kwargs)
 
         alphas = 1. - betas
-        alphas_cumprod = torch.cumprod(alphas, dim = 0)
+        alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
+        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -537,18 +503,14 @@
         register_buffer('betas', betas)
         register_buffer('alphas_cumprod', alphas_cumprod)
         register_buffer('alphas_cumprod_prev', alphas_cumprod_prev)
 
         # calculations for diffusion q(x_t | x_{t-1}) and others
 
         register_buffer('sqrt_alphas_cumprod', torch.sqrt(alphas_cumprod))
-
-        terminal_snr = self.sqrt_alphas_cumprod[-1]
-        assert terminal_snr == 0, f'non-zero terminal SNR detected ({terminal_snr:.6f}), from https://arxiv.org/abs/2305.08891 paper - you can wrap your schedule function with `enforce_zero_terminal_snr` decorator'
-
         register_buffer('sqrt_one_minus_alphas_cumprod', torch.sqrt(1. - alphas_cumprod))
         register_buffer('log_one_minus_alphas_cumprod', torch.log(1. - alphas_cumprod))
         register_buffer('sqrt_recip_alphas_cumprod', torch.sqrt(1. / alphas_cumprod))
         register_buffer('sqrt_recipm1_alphas_cumprod', torch.sqrt(1. / alphas_cumprod - 1))
 
         # calculations for posterior q(x_{t-1} | x_t, x_0)
 
@@ -560,31 +522,30 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
-        # derive loss weight
-        # snr - signal noise ratio
+        # loss weight
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
-        # https://arxiv.org/abs/2303.09556
-
         maybe_clipped_snr = snr.clone()
         if min_snr_loss_weight:
             maybe_clipped_snr.clamp_(max = min_snr_gamma)
 
         if objective == 'pred_noise':
-            register_buffer('loss_weight', maybe_clipped_snr / snr)
+            loss_weight = maybe_clipped_snr / snr
         elif objective == 'pred_x0':
-            register_buffer('loss_weight', maybe_clipped_snr)
+            loss_weight = maybe_clipped_snr
         elif objective == 'pred_v':
-            register_buffer('loss_weight', maybe_clipped_snr / (snr + 1))
+            loss_weight = maybe_clipped_snr / (snr + 1)
+
+        register_buffer('loss_weight', loss_weight)
 
         # auto-normalization of data [0, 1] -> [-1, 1] - can turn off by setting it to be False
 
         self.normalize = normalize_to_neg_one_to_one if auto_normalize else identity
         self.unnormalize = unnormalize_to_zero_to_one if auto_normalize else identity
 
     def predict_start_from_noise(self, x_t, t, noise):
@@ -616,26 +577,23 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False, rederive_pred_noise = False):
+    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False):
         model_output = self.model(x, t, x_self_cond)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
-            if clip_x_start and rederive_pred_noise:
-                pred_noise = self.predict_noise_from_start(x, t, x_start)
-
         elif self.objective == 'pred_x0':
             x_start = model_output
             x_start = maybe_clip(x_start)
             pred_noise = self.predict_noise_from_start(x, t, x_start)
 
         elif self.objective == 'pred_v':
             v = model_output
@@ -650,90 +608,110 @@
         x_start = preds.pred_x_start
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
+     
+    def condition_mean(self, cond_fn, mean,variance, x, t, guidance_kwargs=None):
+        """
+        Compute the mean for the previous step, given a function cond_fn that
+        computes the gradient of a conditional log probability with respect to
+        x. In particular, cond_fn computes grad(log(p(y|x))), and we want to
+        condition on y.
+        This uses the conditioning strategy from Sohl-Dickstein et al. (2015).
+        """
+        gradient = cond_fn(x, t, **guidance_kwargs)
+        new_mean = (
+            mean.float() + variance * gradient.float()
+        )
+        print("gradient: ",(variance * gradient.float()).mean())
+        return new_mean
 
+        
     @torch.no_grad()
-    def p_sample(self, x, t: int, x_self_cond = None):
+    def p_sample(self, x, t: int, x_self_cond = None, cond_fn=None, guidance_kwargs=None):
         b, *_, device = *x.shape, x.device
         batched_times = torch.full((b,), t, device = x.device, dtype = torch.long)
-        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
+        model_mean, variance, model_log_variance, x_start = self.p_mean_variance(
+            x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True
+        )
+        if exists(cond_fn) and exists(guidance_kwargs):
+            model_mean = self.condition_mean(cond_fn, model_mean, variance, x, batched_times, guidance_kwargs)
+        
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
-    def p_sample_loop(self, shape, return_all_timesteps = False):
+    def p_sample_loop(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
         batch, device = shape[0], self.betas.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
-            img, x_start = self.p_sample(img, t, self_cond)
+            img, x_start = self.p_sample(img, t, self_cond, cond_fn, guidance_kwargs)
             imgs.append(img)
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def ddim_sample(self, shape, return_all_timesteps = False):
+    def ddim_sample(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
         batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps = sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for time, time_next in tqdm(time_pairs, desc = 'sampling loop time step'):
             time_cond = torch.full((batch,), time, device = device, dtype = torch.long)
             self_cond = x_start if self.self_condition else None
-            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True, rederive_pred_noise = True)
+            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True)
+
+            imgs.append(img)
 
             if time_next < 0:
                 img = x_start
-                imgs.append(img)
                 continue
 
             alpha = self.alphas_cumprod[time]
             alpha_next = self.alphas_cumprod[time_next]
 
             sigma = eta * ((1 - alpha / alpha_next) * (1 - alpha_next) / (1 - alpha)).sqrt()
             c = (1 - alpha_next - sigma ** 2).sqrt()
 
             noise = torch.randn_like(img)
 
             img = x_start * alpha_next.sqrt() + \
                   c * pred_noise + \
                   sigma * noise
 
-            imgs.append(img)
-
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def sample(self, batch_size = 16, return_all_timesteps = False):
+    def sample(self, batch_size = 16, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
         image_size, channels = self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps)
+        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps, cond_fn=cond_fn, guidance_kwargs=guidance_kwargs)
 
     @torch.no_grad()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
@@ -755,14 +733,23 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
+    @property
+    def loss_fn(self):
+        if self.loss_type == 'l1':
+            return F.l1_loss
+        elif self.loss_type == 'l2':
+            return F.mse_loss
+        else:
+            raise ValueError(f'invalid loss type {self.loss_type}')
+
     def p_losses(self, x_start, t, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -787,15 +774,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = F.mse_loss(model_out, target, reduction = 'none')
+        loss = self.loss_fn(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
@@ -857,45 +844,26 @@
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
         fp16 = False,
         split_batches = True,
-        convert_image_to = None,
-        calculate_fid = True,
-        inception_block_idx = 2048
+        convert_image_to = None
     ):
         super().__init__()
 
-        # accelerator
-
         self.accelerator = Accelerator(
             split_batches = split_batches,
             mixed_precision = 'fp16' if fp16 else 'no'
         )
 
         self.accelerator.native_amp = amp
 
-        # model
-
         self.model = diffusion_model
-        self.channels = diffusion_model.channels
-
-        # InceptionV3 for fid-score computation
-
-        self.inception_v3 = None
-
-        if calculate_fid:
-            assert inception_block_idx in InceptionV3.BLOCK_INDEX_BY_DIM
-            block_idx = InceptionV3.BLOCK_INDEX_BY_DIM[inception_block_idx]
-            self.inception_v3 = InceptionV3([block_idx])
-            self.inception_v3.to(self.device)
-
-        # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
 
         self.batch_size = train_batch_size
         self.gradient_accumulate_every = gradient_accumulate_every
@@ -915,31 +883,26 @@
 
         self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = adam_betas)
 
         # for logging results in a folder periodically
 
         if self.accelerator.is_main_process:
             self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
-            self.ema.to(self.device)
 
         self.results_folder = Path(results_folder)
         self.results_folder.mkdir(exist_ok = True)
 
         # step counter state
 
         self.step = 0
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
-    @property
-    def device(self):
-        return self.accelerator.device
-
     def save(self, milestone):
         if not self.accelerator.is_local_main_process:
             return
 
         data = {
             'step': self.step,
             'model': self.accelerator.get_state_dict(self.model),
@@ -958,48 +921,22 @@
         data = torch.load(str(self.results_folder / f'model-{milestone}.pt'), map_location=device)
 
         model = self.accelerator.unwrap_model(self.model)
         model.load_state_dict(data['model'])
 
         self.step = data['step']
         self.opt.load_state_dict(data['opt'])
-        if self.accelerator.is_main_process:
-            self.ema.load_state_dict(data["ema"])
+        self.ema.load_state_dict(data['ema'])
 
         if 'version' in data:
             print(f"loading from version {data['version']}")
 
         if exists(self.accelerator.scaler) and exists(data['scaler']):
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
-    @torch.no_grad()
-    def calculate_activation_statistics(self, samples):
-        assert exists(self.inception_v3)
-
-        features = self.inception_v3(samples)[0]
-        features = rearrange(features, '... 1 1 -> ...').cpu().numpy()
-
-        mu = np.mean(features, axis = 0)
-        sigma = np.cov(features, rowvar = False)
-        return mu, sigma
-
-    def fid_score(self, real_samples, fake_samples):
-
-        if self.channels == 1:
-            real_samples, fake_samples = map(lambda t: repeat(t, 'b 1 ... -> b c ...', c = 3), (real_samples, fake_samples))
-
-        min_batch = min(real_samples.shape[0], fake_samples.shape[0])
-        real_samples, fake_samples = map(lambda t: t[:min_batch], (real_samples, fake_samples))
-
-        m1, s1 = self.calculate_activation_statistics(real_samples)
-        m2, s2 = self.calculate_activation_statistics(fake_samples)
-
-        fid_value = calculate_frechet_distance(m1, s1, m2, s2)
-        return fid_value
-
     def train(self):
         accelerator = self.accelerator
         device = accelerator.device
 
         with tqdm(initial = self.step, total = self.train_num_steps, disable = not accelerator.is_main_process) as pbar:
 
             while self.step < self.train_num_steps:
@@ -1024,31 +961,86 @@
                 self.opt.step()
                 self.opt.zero_grad()
 
                 accelerator.wait_for_everyone()
 
                 self.step += 1
                 if accelerator.is_main_process:
+                    self.ema.to(device)
                     self.ema.update()
 
                     if self.step != 0 and self.step % self.save_and_sample_every == 0:
                         self.ema.ema_model.eval()
 
                         with torch.no_grad():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
 
                         all_images = torch.cat(all_images_list, dim = 0)
-
                         utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
                         self.save(milestone)
 
-                        # whether to calculate fid
-
-                        if exists(self.inception_v3):
-                            fid_score = self.fid_score(real_samples = data, fake_samples = all_images)
-                            accelerator.print(f'fid_score: {fid_score}')
-
                 pbar.update(1)
 
         accelerator.print('training complete')
+
+if __name__ == '__main__':
+    class Classifier(nn.Module):
+        def __init__(self, image_size, num_classes, t_dim=1) -> None:
+            super().__init__()
+            self.linear_t = nn.Linear(t_dim, num_classes)
+            self.linear_img = nn.Linear(image_size * image_size * 3, num_classes)
+        def forward(self, x, t):
+            """
+            Args:
+                x (_type_): [B, 3, N, N]
+                t (_type_): [B,]
+
+            Returns:
+                    logits [B, num_classes]
+            """
+            B = x.shape[0]
+            t = t.view(B, 1)
+            logits = self.linear_t(t.float()) + self.linear_img(x.view(x.shape[0], -1))
+            return logits
+        
+    def classifier_cond_fn(x, t, classifier, y, classifier_scale=1):
+        """
+        return the graident of the classifier outputing y wrt x.
+        formally expressed as d_log(classifier(x, t)) / dx
+        """
+        assert y is not None
+        with torch.enable_grad():
+            x_in = x.detach().requires_grad_(True)
+            logits = classifier(x_in, t)
+            log_probs = F.log_softmax(logits, dim=-1)
+            selected = log_probs[range(len(logits)), y.view(-1)]
+            grad = torch.autograd.grad(selected.sum(), x_in)[0] * classifier_scale
+            return grad
+        
+    
+    
+    model = Unet(
+        dim = 64,
+        dim_mults = (1, 2, 4, 8)
+    )
+    image_size = 128
+    diffusion = GaussianDiffusion(
+        model,
+        image_size = image_size,
+        timesteps = 1000,   # number of steps
+        loss_type = 'l1'    # L1 or L2
+    )
+
+    classifier = Classifier(image_size=image_size, num_classes=1000, t_dim=1)
+    batch_size = 4
+    sampled_images = diffusion.sample(
+        batch_size = batch_size,
+        cond_fn=classifier_cond_fn, 
+        guidance_kwargs={
+            "classifier":classifier,
+            "y":torch.fill(torch.zeros(batch_size), 1).long(),
+            "classifier_scale":1,
+        }
+    )
+    sampled_images.shape # (4, 3, 128, 128)
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,24 +403,25 @@
     as proposed in https://openreview.net/forum?id=-NEXDKk8gZ
     """
     steps = timesteps + 1
     x = torch.linspace(0, timesteps, steps, dtype = torch.float64)
     alphas_cumprod = torch.cos(((x / timesteps) + s) / (1 + s) * math.pi * 0.5) ** 2
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
-    return torch.clip(betas, 0, 1.)
+    return torch.clip(betas, 0, 0.999)
 
 class GaussianDiffusion1D(nn.Module):
     def __init__(
         self,
         model,
         *,
         seq_length,
         timesteps = 1000,
         sampling_timesteps = None,
+        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'cosine',
         ddim_sampling_eta = 0.,
         auto_normalize = True
     ):
         super().__init__()
         self.model = model
@@ -442,14 +443,15 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
+        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -661,14 +663,23 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
+    @property
+    def loss_fn(self):
+        if self.loss_type == 'l1':
+            return F.l1_loss
+        elif self.loss_type == 'l2':
+            return F.mse_loss
+        else:
+            raise ValueError(f'invalid loss type {self.loss_type}')
+
     def p_losses(self, x_start, t, noise = None):
         b, c, n = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -693,15 +704,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = F.mse_loss(model_out, target, reduction = 'none')
+        loss = self.loss_fn(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, n, device, seq_length, = *img.shape, img.device, self.seq_length
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
+
 from torchvision import transforms as T, utils
 
-from einops import rearrange, reduce
+from einops import rearrange, reduce, repeat
 from einops.layers.torch import Rearrange
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
-# from denoising_diffusion_pytorch.version import __version__
+import numpy as np
+from pytorch_fid.inception import InceptionV3
+from pytorch_fid.fid_score import calculate_frechet_distance
+
+from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
 
 # helpers functions
 
@@ -431,38 +436,38 @@
     t = torch.linspace(0, timesteps, steps, dtype = torch.float64) / timesteps
     v_start = torch.tensor(start / tau).sigmoid()
     v_end = torch.tensor(end / tau).sigmoid()
     alphas_cumprod = (-((t * (end - start) + start) / tau).sigmoid() + v_end) / (v_end - v_start)
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
     return torch.clip(betas, 0, 0.999)
-    
 
-    
 class GaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
+        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
-        min_snr_loss_weight = False,
+        min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
         self.model = model
+
         self.channels = self.model.channels
         self.self_condition = self.model.self_condition
 
         self.image_size = image_size
 
         self.objective = objective
 
@@ -481,14 +486,15 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
+        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -520,30 +526,31 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
-        # loss weight
+        # derive loss weight
+        # snr - signal noise ratio
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
+        # https://arxiv.org/abs/2303.09556
+
         maybe_clipped_snr = snr.clone()
         if min_snr_loss_weight:
             maybe_clipped_snr.clamp_(max = min_snr_gamma)
 
         if objective == 'pred_noise':
-            loss_weight = maybe_clipped_snr / snr
+            register_buffer('loss_weight', maybe_clipped_snr / snr)
         elif objective == 'pred_x0':
-            loss_weight = maybe_clipped_snr
+            register_buffer('loss_weight', maybe_clipped_snr)
         elif objective == 'pred_v':
-            loss_weight = maybe_clipped_snr / (snr + 1)
-
-        register_buffer('loss_weight', loss_weight)
+            register_buffer('loss_weight', maybe_clipped_snr / (snr + 1))
 
         # auto-normalization of data [0, 1] -> [-1, 1] - can turn off by setting it to be False
 
         self.normalize = normalize_to_neg_one_to_one if auto_normalize else identity
         self.unnormalize = unnormalize_to_zero_to_one if auto_normalize else identity
 
     def predict_start_from_noise(self, x_t, t, noise):
@@ -575,23 +582,26 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False):
+    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False, rederive_pred_noise = False):
         model_output = self.model(x, t, x_self_cond)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
+            if clip_x_start and rederive_pred_noise:
+                pred_noise = self.predict_noise_from_start(x, t, x_start)
+
         elif self.objective == 'pred_x0':
             x_start = model_output
             x_start = maybe_clip(x_start)
             pred_noise = self.predict_noise_from_start(x, t, x_start)
 
         elif self.objective == 'pred_v':
             v = model_output
@@ -606,110 +616,90 @@
         x_start = preds.pred_x_start
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
-     
-    def condition_mean(self, cond_fn, mean,variance, x, t, guidance_kwargs=None):
-        """
-        Compute the mean for the previous step, given a function cond_fn that
-        computes the gradient of a conditional log probability with respect to
-        x. In particular, cond_fn computes grad(log(p(y|x))), and we want to
-        condition on y.
-        This uses the conditioning strategy from Sohl-Dickstein et al. (2015).
-        """
-        gradient = cond_fn(x, t, **guidance_kwargs)
-        new_mean = (
-            mean.float() + variance * gradient.float()
-        )
-        print("gradient: ",(variance * gradient.float()).mean())
-        return new_mean
 
-        
     @torch.no_grad()
-    def p_sample(self, x, t: int, x_self_cond = None, cond_fn=None, guidance_kwargs=None):
+    def p_sample(self, x, t: int, x_self_cond = None):
         b, *_, device = *x.shape, x.device
         batched_times = torch.full((b,), t, device = x.device, dtype = torch.long)
-        model_mean, variance, model_log_variance, x_start = self.p_mean_variance(
-            x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True
-        )
-        if exists(cond_fn) and exists(guidance_kwargs):
-            model_mean = self.condition_mean(cond_fn, model_mean, variance, x, batched_times, guidance_kwargs)
-        
+        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
-    def p_sample_loop(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+    def p_sample_loop(self, shape, return_all_timesteps = False):
         batch, device = shape[0], self.betas.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
-            img, x_start = self.p_sample(img, t, self_cond, cond_fn, guidance_kwargs)
+            img, x_start = self.p_sample(img, t, self_cond)
             imgs.append(img)
 
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def ddim_sample(self, shape, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+    def ddim_sample(self, shape, return_all_timesteps = False):
         batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps = sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for time, time_next in tqdm(time_pairs, desc = 'sampling loop time step'):
             time_cond = torch.full((batch,), time, device = device, dtype = torch.long)
             self_cond = x_start if self.self_condition else None
-            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True)
-
-            imgs.append(img)
+            pred_noise, x_start, *_ = self.model_predictions(img, time_cond, self_cond, clip_x_start = True, rederive_pred_noise = True)
 
             if time_next < 0:
                 img = x_start
+                imgs.append(img)
                 continue
 
             alpha = self.alphas_cumprod[time]
             alpha_next = self.alphas_cumprod[time_next]
 
             sigma = eta * ((1 - alpha / alpha_next) * (1 - alpha_next) / (1 - alpha)).sqrt()
             c = (1 - alpha_next - sigma ** 2).sqrt()
 
             noise = torch.randn_like(img)
 
             img = x_start * alpha_next.sqrt() + \
                   c * pred_noise + \
                   sigma * noise
 
+            imgs.append(img)
+
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
-    def sample(self, batch_size = 16, return_all_timesteps = False, cond_fn=None, guidance_kwargs=None):
+    def sample(self, batch_size = 16, return_all_timesteps = False):
         image_size, channels = self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps, cond_fn=cond_fn, guidance_kwargs=guidance_kwargs)
+        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps)
 
     @torch.no_grad()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
@@ -731,14 +721,23 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
+    @property
+    def loss_fn(self):
+        if self.loss_type == 'l1':
+            return F.l1_loss
+        elif self.loss_type == 'l2':
+            return F.mse_loss
+        else:
+            raise ValueError(f'invalid loss type {self.loss_type}')
+
     def p_losses(self, x_start, t, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -763,15 +762,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = F.mse_loss(model_out, target, reduction = 'none')
+        loss = self.loss_fn(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
@@ -833,26 +832,45 @@
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
         fp16 = False,
         split_batches = True,
-        convert_image_to = None
+        convert_image_to = None,
+        calculate_fid = True,
+        inception_block_idx = 2048
     ):
         super().__init__()
 
+        # accelerator
+
         self.accelerator = Accelerator(
             split_batches = split_batches,
             mixed_precision = 'fp16' if fp16 else 'no'
         )
 
         self.accelerator.native_amp = amp
 
+        # model
+
         self.model = diffusion_model
+        self.channels = diffusion_model.channels
+
+        # InceptionV3 for fid-score computation
+
+        self.inception_v3 = None
+
+        if calculate_fid:
+            assert inception_block_idx in InceptionV3.BLOCK_INDEX_BY_DIM
+            block_idx = InceptionV3.BLOCK_INDEX_BY_DIM[inception_block_idx]
+            self.inception_v3 = InceptionV3([block_idx])
+            self.inception_v3.to(self.device)
+
+        # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
 
         self.batch_size = train_batch_size
         self.gradient_accumulate_every = gradient_accumulate_every
@@ -872,26 +890,31 @@
 
         self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = adam_betas)
 
         # for logging results in a folder periodically
 
         if self.accelerator.is_main_process:
             self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
+            self.ema.to(self.device)
 
         self.results_folder = Path(results_folder)
         self.results_folder.mkdir(exist_ok = True)
 
         # step counter state
 
         self.step = 0
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
+    @property
+    def device(self):
+        return self.accelerator.device
+
     def save(self, milestone):
         if not self.accelerator.is_local_main_process:
             return
 
         data = {
             'step': self.step,
             'model': self.accelerator.get_state_dict(self.model),
@@ -910,22 +933,48 @@
         data = torch.load(str(self.results_folder / f'model-{milestone}.pt'), map_location=device)
 
         model = self.accelerator.unwrap_model(self.model)
         model.load_state_dict(data['model'])
 
         self.step = data['step']
         self.opt.load_state_dict(data['opt'])
-        self.ema.load_state_dict(data['ema'])
+        if self.accelerator.is_main_process:
+            self.ema.load_state_dict(data["ema"])
 
         if 'version' in data:
             print(f"loading from version {data['version']}")
 
         if exists(self.accelerator.scaler) and exists(data['scaler']):
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
+    @torch.no_grad()
+    def calculate_activation_statistics(self, samples):
+        assert exists(self.inception_v3)
+
+        features = self.inception_v3(samples)[0]
+        features = rearrange(features, '... 1 1 -> ...').cpu().numpy()
+
+        mu = np.mean(features, axis = 0)
+        sigma = np.cov(features, rowvar = False)
+        return mu, sigma
+
+    def fid_score(self, real_samples, fake_samples):
+
+        if self.channels == 1:
+            real_samples, fake_samples = map(lambda t: repeat(t, 'b 1 ... -> b c ...', c = 3), (real_samples, fake_samples))
+
+        min_batch = min(real_samples.shape[0], fake_samples.shape[0])
+        real_samples, fake_samples = map(lambda t: t[:min_batch], (real_samples, fake_samples))
+
+        m1, s1 = self.calculate_activation_statistics(real_samples)
+        m2, s2 = self.calculate_activation_statistics(fake_samples)
+
+        fid_value = calculate_frechet_distance(m1, s1, m2, s2)
+        return fid_value
+
     def train(self):
         accelerator = self.accelerator
         device = accelerator.device
 
         with tqdm(initial = self.step, total = self.train_num_steps, disable = not accelerator.is_main_process) as pbar:
 
             while self.step < self.train_num_steps:
@@ -950,85 +999,31 @@
                 self.opt.step()
                 self.opt.zero_grad()
 
                 accelerator.wait_for_everyone()
 
                 self.step += 1
                 if accelerator.is_main_process:
-                    self.ema.to(device)
                     self.ema.update()
 
                     if self.step != 0 and self.step % self.save_and_sample_every == 0:
                         self.ema.ema_model.eval()
 
                         with torch.no_grad():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
 
                         all_images = torch.cat(all_images_list, dim = 0)
+
                         utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
                         self.save(milestone)
 
-                pbar.update(1)
+                        # whether to calculate fid
 
-        accelerator.print('training complete')
+                        if exists(self.inception_v3):
+                            fid_score = self.fid_score(real_samples = data, fake_samples = all_images)
+                            accelerator.print(f'fid_score: {fid_score}')
 
-if __name__ == '__main__':
-    class Classifier(nn.Module):
-        def __init__(self, image_size, num_classes, t_dim=1) -> None:
-            super().__init__()
-            self.linear_t = nn.Linear(t_dim, num_classes)
-            self.linear_img = nn.Linear(image_size * image_size * 3, num_classes)
-        def forward(self, x, t):
-            """
-            Args:
-                x (_type_): [B, 3, N, N]
-                t (_type_): [B,]
-
-            Returns:
-                    logits [B, num_classes]
-            """
-            B = x.shape[0]
-            t = t.view(B, 1)
-            logits = self.linear_t(t.float()) + self.linear_img(x.view(x.shape[0], -1))
-            return logits
-        
-    def classifier_cond_fn(x, t, classifier, y, classifier_scale=1):
-        """
-        return the graident of the classifier outputing y wrt x.
-        formally expressed as d_log(classifier(x, t)) / dx
-        """
-        assert y is not None
-        with torch.enable_grad():
-            x_in = x.detach().requires_grad_(True)
-            logits = classifier(x_in, t)
-            log_probs = F.log_softmax(logits, dim=-1)
-            selected = log_probs[range(len(logits)), y.view(-1)]
-            grad = torch.autograd.grad(selected.sum(), x_in)[0] * classifier_scale
-            return grad
-        
-    
-    
-    model = Unet(
-        dim = 64,
-        dim_mults = (1, 2, 4, 8)
-    )
-    image_size = 128
-    diffusion = GaussianDiffusion(
-        model,
-        image_size = image_size,
-        timesteps = 1000,   # number of steps
-    )
+                pbar.update(1)
 
-    classifier = Classifier(image_size=image_size, num_classes=1000, t_dim=1)
-    batch_size = 4
-    sampled_images = diffusion.sample(
-        batch_size = batch_size,
-        cond_fn=classifier_cond_fn, 
-        guidance_kwargs={
-            "classifier":classifier,
-            "y":torch.fill(torch.zeros(batch_size), 1).long(),
-            "classifier_scale":1,
-        }
-    )
-    sampled_images.shape # (4, 3, 128, 128)
+        accelerator.print('training complete')
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
         model_output = self.model(x_t, t)
         pred_noise, pred_x_start, weights = model_output.split(self.split_dims, dim = 1)
 
         # get loss for predicted noise and x_start
         # with the loss weight given at initialization
 
-        noise_loss = F.mse_loss(noise, pred_noise) * self.pred_noise_loss_weight
-        x_start_loss = F.mse_loss(x_start, pred_x_start) * self.pred_x_start_loss_weight
+        noise_loss = self.loss_fn(noise, pred_noise) * self.pred_noise_loss_weight
+        x_start_loss = self.loss_fn(x_start, pred_x_start) * self.pred_x_start_loss_weight
 
         # calculate x_start from predicted noise
         # then do a weighted sum of the x_start prediction, weights also predicted by the model (softmax normalized)
 
         x_start_from_pred_noise = self.predict_start_from_noise(x_t, t, pred_noise)
         x_start_from_pred_noise = x_start_from_pred_noise.clamp(-2., 2.)
         weighted_x_start = einsum('b j h w, b j c h w -> b c h w', weights.softmax(dim = 1), torch.stack((x_start_from_pred_noise, pred_x_start), dim = 1))
 
         # main loss to x_start with the weighted one
 
-        weighted_x_start_loss = F.mse_loss(x_start, weighted_x_start)
+        weighted_x_start_loss = self.loss_fn(x_start, weighted_x_start)
         return weighted_x_start_loss + x_start_loss + noise_loss
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.1
+Version: 1.6.2
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.1/setup.py` & `denoising-diffusion-pytorch-1.6.2/setup.py`

 * *Files identical despite different names*

