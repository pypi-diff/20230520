# Comparing `tmp/denoising-diffusion-pytorch-1.6.2.tar.gz` & `tmp/denoising-diffusion-pytorch-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.6.2.tar", last modified: Sat May 20 16:40:31 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.6.3.tar", last modified: Sat May 20 17:14:21 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.6.2.tar` & `denoising-diffusion-pytorch-1.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 16:40:31.000000 denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:40:31.605023 denoising-diffusion-pytorch-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 16:40:14.000000 denoising-diffusion-pytorch-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36211 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.6.2/LICENSE` & `denoising-diffusion-pytorch-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/PKG-INFO` & `denoising-diffusion-pytorch-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.2
+Version: 1.6.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.2/README.md` & `denoising-diffusion-pytorch-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     dim = 64,
     dim_mults = (1, 2, 4, 8)
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
-    timesteps = 1000,   # number of steps
-    loss_type = 'l1'    # L1 or L2
+    timesteps = 1000    # number of steps
 )
 
 training_images = torch.rand(8, 3, 128, 128) # images are normalized from 0 to 1
 loss = diffusion(training_images)
 loss.backward()
 # after a lot of training
 
@@ -61,16 +60,15 @@
     dim_mults = (1, 2, 4, 8)
 )
 
 diffusion = GaussianDiffusion(
     model,
     image_size = 128,
     timesteps = 1000,           # number of steps
-    sampling_timesteps = 250,   # number of sampling timesteps (using ddim for faster inference [see citation for ddim paper])
-    loss_type = 'l1'            # L1 or L2
+    sampling_timesteps = 250    # number of sampling timesteps (using ddim for faster inference [see citation for ddim paper])
 )
 
 trainer = Trainer(
     diffusion,
     'path/to/your/images',
     train_batch_size = 32,
     train_lr = 8e-5,
@@ -307,7 +305,22 @@
 ```bibtex
 @inproceedings{Hang2023EfficientDT,
     title   = {Efficient Diffusion Training via Min-SNR Weighting Strategy},
     author  = {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han Hu and Xin Geng and Baining Guo},
     year    = {2023}
 }
 ```
+
+```bibtex
+@misc{Guttenberg2023,
+    author  = {Nicholas Guttenberg},
+    url     = {https://www.crosslabs.org/blog/diffusion-with-offset-noise}
+}
+```
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
@@ -9,40 +9,39 @@
 Research Scientists / Engineers from ð¤_Huggingface Update: Turns out none of
 the technicalities really matters at all | "Cold_Diffusion"_paper | Muse [./
 images/sample.png][Image] [![PyPI version](https://badge.fury.io/py/denoising-
 diffusion-pytorch.svg)](https://badge.fury.io/py/denoising-diffusion-pytorch)
 ## Install ```bash $ pip install denoising_diffusion_pytorch ``` ## Usage
 ```python import torch from denoising_diffusion_pytorch import Unet,
 GaussianDiffusion model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) ) diffusion
-= GaussianDiffusion( model, image_size = 128, timesteps = 1000, # number of
-steps loss_type = 'l1' # L1 or L2 ) training_images = torch.rand(8, 3, 128,
-128) # images are normalized from 0 to 1 loss = diffusion(training_images)
-loss.backward() # after a lot of training sampled_images = diffusion.sample
-(batch_size = 4) sampled_images.shape # (4, 3, 128, 128) ``` Or, if you simply
-want to pass in a folder name and the desired image dimensions, you can use the
-`Trainer` class to easily train a model. ```python from
-denoising_diffusion_pytorch import Unet, GaussianDiffusion, Trainer model =
-Unet( dim = 64, dim_mults = (1, 2, 4, 8) ) diffusion = GaussianDiffusion
-( model, image_size = 128, timesteps = 1000, # number of steps
-sampling_timesteps = 250, # number of sampling timesteps (using ddim for faster
-inference [see citation for ddim paper]) loss_type = 'l1' # L1 or L2 ) trainer
-= Trainer( diffusion, 'path/to/your/images', train_batch_size = 32, train_lr =
-8e-5, train_num_steps = 700000, # total training steps
-gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
-# exponential moving average decay amp = True, # turn on mixed precision
-calculate_fid = True # whether to calculate fid during training ) trainer.train
-() ``` Samples and model checkpoints will be logged to `./results` periodically
-## Multi-GPU Training The `Trainer` class is now equipped with ð¤
-Accelerator. You can easily do multi-gpu training in two steps using their
-`accelerate` CLI At the project root directory, where the training script is,
-run ```python $ accelerate config ``` Then, in the same directory ```python $
-accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
-request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
-from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
-model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
+= GaussianDiffusion( model, image_size = 128, timesteps = 1000 # number of
+steps ) training_images = torch.rand(8, 3, 128, 128) # images are normalized
+from 0 to 1 loss = diffusion(training_images) loss.backward() # after a lot of
+training sampled_images = diffusion.sample(batch_size = 4) sampled_images.shape
+# (4, 3, 128, 128) ``` Or, if you simply want to pass in a folder name and the
+desired image dimensions, you can use the `Trainer` class to easily train a
+model. ```python from denoising_diffusion_pytorch import Unet,
+GaussianDiffusion, Trainer model = Unet( dim = 64, dim_mults = (1, 2, 4, 8) )
+diffusion = GaussianDiffusion( model, image_size = 128, timesteps = 1000, #
+number of steps sampling_timesteps = 250 # number of sampling timesteps (using
+ddim for faster inference [see citation for ddim paper]) ) trainer = Trainer
+( diffusion, 'path/to/your/images', train_batch_size = 32, train_lr = 8e-5,
+train_num_steps = 700000, # total training steps gradient_accumulate_every = 2,
+# gradient accumulation steps ema_decay = 0.995, # exponential moving average
+decay amp = True, # turn on mixed precision calculate_fid = True # whether to
+calculate fid during training ) trainer.train() ``` Samples and model
+checkpoints will be logged to `./results` periodically ## Multi-GPU Training
+The `Trainer` class is now equipped with ð¤_Accelerator. You can easily do
+multi-gpu training in two steps using their `accelerate` CLI At the project
+root directory, where the training script is, run ```python $ accelerate config
+``` Then, in the same directory ```python $ accelerate launch train.py ``` ##
+Miscellaneous ### 1D Sequence By popular request, a 1D Unet + Gaussian
+Diffusion implementation. ```python import torch from
+denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D model
+= Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
 GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000, objective =
 'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are normalized
 from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or using trainer
 trainer = Trainer1D( diffusion, dataset = training_seq, train_batch_size = 32,
 train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
@@ -104,8 +103,13 @@
 ```bibtex @misc{https://doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/
 ARXIV.2302.01327}, url = {https://arxiv.org/abs/2302.01327}, author = {Kumar,
 Manoj and Dehghani, Mostafa and Houlsby, Neil}, title = {Dual PatchNorm},
 publisher = {arXiv}, year = {2023}, copyright = {Creative Commons Attribution
 4.0 International} } ``` ```bibtex @inproceedings{Hang2023EfficientDT, title =
 {Efficient Diffusion Training via Min-SNR Weighting Strategy}, author =
 {Tiankai Hang and Shuyang Gu and Chen Li and Jianmin Bao and Dong Chen and Han
-Hu and Xin Geng and Baining Guo}, year = {2023} } ```
+Hu and Xin Geng and Baining Guo}, year = {2023} } ``` ```bibtex @misc
+{Guttenberg2023, author = {Nicholas Guttenberg}, url = {https://
+www.crosslabs.org/blog/diffusion-with-offset-noise} } ``` ```bibtex
+@inproceedings{Lin2023CommonDN, title = {Common Diffusion Noise Schedules and
+Sample Steps are Flawed}, author = {Shanchuan Lin and Bingchen Liu and Jiashi
+Li and Xiao Yang}, year = {2023} } ```
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 7% similar despite different names*

```diff
@@ -371,23 +371,32 @@
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     def forward_with_cond_scale(
         self,
         *args,
         cond_scale = 1.,
+        rescaled_phi = 0.,
         **kwargs
     ):
         logits = self.forward(*args, cond_drop_prob = 0., **kwargs)
 
         if cond_scale == 1:
             return logits
 
         null_logits = self.forward(*args, cond_drop_prob = 1., **kwargs)
-        return null_logits + (logits - null_logits) * cond_scale
+        scaled_logits = null_logits + (logits - null_logits) * cond_scale
+
+        if rescaled_phi == 0.:
+            return scaled_logits
+
+        std_fn = partial(torch.std, dim = tuple(range(1, scaled_logits.ndim)), keepdim = True)
+        rescaled_logits = scaled_logits * (std_fn(logits) / std_fn(scaled_logits))
+
+        return rescaled_logits * rescaled_phi + scaled_logits * (1. - rescaled_phi)
 
     def forward(
         self,
         x,
         time,
         classes,
         cond_drop_prob = None
@@ -479,18 +488,18 @@
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
-        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'cosine',
         ddim_sampling_eta = 1.,
+        offset_noise_strength = 0.,
         min_snr_loss_weight = False,
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
@@ -512,15 +521,14 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
-        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -552,14 +560,18 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
+        # offset noise strength - 0.1 was claimed ideal
+
+        self.offset_noise_strength = offset_noise_strength
+
         # loss weight
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
         maybe_clipped_snr = snr.clone()
         if min_snr_loss_weight:
             maybe_clipped_snr.clamp_(max = min_snr_gamma)
@@ -602,16 +614,16 @@
             extract(self.posterior_mean_coef1, t, x_t.shape) * x_start +
             extract(self.posterior_mean_coef2, t, x_t.shape) * x_t
         )
         posterior_variance = extract(self.posterior_variance, t, x_t.shape)
         posterior_log_variance_clipped = extract(self.posterior_log_variance_clipped, t, x_t.shape)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
-    def model_predictions(self, x, t, classes, cond_scale = 3., clip_x_start = False):
-        model_output = self.model.forward_with_cond_scale(x, t, classes, cond_scale = cond_scale)
+    def model_predictions(self, x, t, classes, cond_scale = 6., rescaled_phi = 0.7, clip_x_start = False):
+        model_output = self.model.forward_with_cond_scale(x, t, classes, cond_scale = cond_scale, rescaled_phi = rescaled_phi)
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, pred_noise)
             x_start = maybe_clip(x_start)
 
@@ -624,49 +636,49 @@
             v = model_output
             x_start = self.predict_start_from_v(x, t, v)
             x_start = maybe_clip(x_start)
             pred_noise = self.predict_noise_from_start(x, t, x_start)
 
         return ModelPrediction(pred_noise, x_start)
 
-    def p_mean_variance(self, x, t, classes, cond_scale, clip_denoised = True):
-        preds = self.model_predictions(x, t, classes, cond_scale)
+    def p_mean_variance(self, x, t, classes, cond_scale, rescaled_phi, clip_denoised = True):
+        preds = self.model_predictions(x, t, classes, cond_scale, rescaled_phi)
         x_start = preds.pred_x_start
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
 
     @torch.no_grad()
-    def p_sample(self, x, t: int, classes, cond_scale = 3., clip_denoised = True):
+    def p_sample(self, x, t: int, classes, cond_scale = 6., rescaled_phi = 0.7, clip_denoised = True):
         b, *_, device = *x.shape, x.device
         batched_times = torch.full((x.shape[0],), t, device = x.device, dtype = torch.long)
-        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, classes = classes, cond_scale = cond_scale, clip_denoised = clip_denoised)
+        model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, classes = classes, cond_scale = cond_scale, rescaled_phi = rescaled_phi, clip_denoised = clip_denoised)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
-    def p_sample_loop(self, classes, shape, cond_scale = 3.):
+    def p_sample_loop(self, classes, shape, cond_scale = 6., rescaled_phi = 0.7):
         batch, device = shape[0], self.betas.device
 
         img = torch.randn(shape, device=device)
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
-            img, x_start = self.p_sample(img, t, classes, cond_scale)
+            img, x_start = self.p_sample(img, t, classes, cond_scale, rescaled_phi)
 
         img = unnormalize_to_zero_to_one(img)
         return img
 
     @torch.no_grad()
-    def ddim_sample(self, classes, shape, cond_scale = 3., clip_denoised = True):
+    def ddim_sample(self, classes, shape, cond_scale = 6., rescaled_phi = 0.7, clip_denoised = True):
         batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps=sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
@@ -693,18 +705,18 @@
                   c * pred_noise + \
                   sigma * noise
 
         img = unnormalize_to_zero_to_one(img)
         return img
 
     @torch.no_grad()
-    def sample(self, classes, cond_scale = 3.):
+    def sample(self, classes, cond_scale = 6., rescaled_phi = 0.7):
         batch_size, image_size, channels = classes.shape[0], self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn(classes, (batch_size, channels, image_size, image_size), cond_scale)
+        return sample_fn(classes, (batch_size, channels, image_size, image_size), cond_scale, rescaled_phi)
 
     @torch.no_grad()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
@@ -717,28 +729,23 @@
             img = self.p_sample(img, torch.full((b,), i, device=device, dtype=torch.long))
 
         return img
 
     def q_sample(self, x_start, t, noise=None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
+        if self.offset_noise_strength > 0.:
+            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
+            noise += self.offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
+
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    @property
-    def loss_fn(self):
-        if self.loss_type == 'l1':
-            return F.l1_loss
-        elif self.loss_type == 'l2':
-            return F.mse_loss
-        else:
-            raise ValueError(f'invalid loss type {self.loss_type}')
-
     def p_losses(self, x_start, t, *, classes, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -753,15 +760,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = self.loss_fn(model_out, target, reduction = 'none')
+        loss = F.mse_loss(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
@@ -795,11 +802,11 @@
     loss = diffusion(training_images, classes = image_classes)
     loss.backward()
 
     # do above for many steps
 
     sampled_images = diffusion.sample(
         classes = image_classes,
-        cond_scale = 3.                # condition scaling, anything greater than 1 strengthens the classifier free guidance. reportedly 3-8 is good empirically
+        cond_scale = 6.                # condition scaling, anything greater than 1 strengthens the classifier free guidance. reportedly 3-8 is good empirically
     )
 
     sampled_images.shape # (8, 3, 128, 128)
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 class ContinuousTimeGaussianDiffusion(nn.Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         channels = 3,
-        loss_type = 'l1',
         noise_schedule = 'linear',
         num_sample_steps = 500,
         clip_sample_denoised = True,
         learned_schedule_net_hidden_dim = 1024,
         learned_noise_schedule_frac_gradient = 1.,   # between 0 and 1, determines what percentage of gradients go back, so one can update the learned noise schedule more slowly
         min_snr_loss_weight = False,
         min_snr_gamma = 5
@@ -134,16 +133,14 @@
         # image dimensions
 
         self.channels = channels
         self.image_size = image_size
 
         # continuous noise schedule related stuff
 
-        self.loss_type = loss_type
-
         if noise_schedule == 'linear':
             self.log_snr = beta_linear_log_snr
         elif noise_schedule == 'cosine':
             self.log_snr = alpha_cosine_log_snr
         elif noise_schedule == 'learned':
             log_snr_max, log_snr_min = [beta_linear_log_snr(torch.tensor([time])).item() for time in (0., 1.)]
 
@@ -166,23 +163,14 @@
         self.min_snr_loss_weight = min_snr_loss_weight
         self.min_snr_gamma = min_snr_gamma
 
     @property
     def device(self):
         return next(self.model.parameters()).device
 
-    @property
-    def loss_fn(self):
-        if self.loss_type == 'l1':
-            return F.l1_loss
-        elif self.loss_type == 'l2':
-            return F.mse_loss
-        else:
-            raise ValueError(f'invalid loss type {self.loss_type}')
-
     def p_mean_variance(self, x, time, time_next):
         # reviewer found an error in the equation in the paper (missing sigma)
         # following - https://openreview.net/forum?id=2LdBqxc1Yv&noteId=rIQgH0zKsRt
 
         log_snr = self.log_snr(time)
         log_snr_next = self.log_snr(time_next)
         c = -expm1(log_snr - log_snr_next)
@@ -262,15 +250,15 @@
 
     def p_losses(self, x_start, times, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         x, log_snr = self.q_sample(x_start = x_start, times = times, noise = noise)
         model_out = self.model(x, log_snr)
 
-        losses = self.loss_fn(model_out, noise, reduction = 'none')
+        losses = F.mse_loss(model_out, noise, reduction = 'none')
         losses = reduce(losses, 'b ... -> b', 'mean')
 
         if self.min_snr_loss_weight:
             snr = log_snr.exp()
             loss_weight = snr.clamp(min = self.min_snr_gamma) / snr
             losses = losses * loss_weight
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,20 +445,20 @@
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
-        loss_type = 'l1',
-        objective = 'pred_noise',
+        objective = 'pred_v',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
+        offset_noise_strength = 0.,  # https://www.crosslabs.org/blog/diffusion-with-offset-noise
         min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
         assert not model.random_or_learned_sinusoidal_cond
 
@@ -486,15 +486,14 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
-        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -526,14 +525,18 @@
 
         # below: log calculation clipped because the posterior variance is 0 at the beginning of the diffusion chain
 
         register_buffer('posterior_log_variance_clipped', torch.log(posterior_variance.clamp(min =1e-20)))
         register_buffer('posterior_mean_coef1', betas * torch.sqrt(alphas_cumprod_prev) / (1. - alphas_cumprod))
         register_buffer('posterior_mean_coef2', (1. - alphas_cumprod_prev) * torch.sqrt(alphas) / (1. - alphas_cumprod))
 
+        # offset noise strength - in blogpost, they claimed 0.1 was ideal
+
+        self.offset_noise_strength = offset_noise_strength
+
         # derive loss weight
         # snr - signal noise ratio
 
         snr = alphas_cumprod / (1 - alphas_cumprod)
 
         # https://arxiv.org/abs/2303.09556
 
@@ -549,14 +552,18 @@
             register_buffer('loss_weight', maybe_clipped_snr / (snr + 1))
 
         # auto-normalization of data [0, 1] -> [-1, 1] - can turn off by setting it to be False
 
         self.normalize = normalize_to_neg_one_to_one if auto_normalize else identity
         self.unnormalize = unnormalize_to_zero_to_one if auto_normalize else identity
 
+    @property
+    def device(self):
+        return self.betas.device
+
     def predict_start_from_noise(self, x_t, t, noise):
         return (
             extract(self.sqrt_recip_alphas_cumprod, t, x_t.shape) * x_t -
             extract(self.sqrt_recipm1_alphas_cumprod, t, x_t.shape) * noise
         )
 
     def predict_noise_from_start(self, x_t, t, x0):
@@ -619,24 +626,24 @@
             x_start.clamp_(-1., 1.)
 
         model_mean, posterior_variance, posterior_log_variance = self.q_posterior(x_start = x_start, x_t = x, t = t)
         return model_mean, posterior_variance, posterior_log_variance, x_start
 
     @torch.no_grad()
     def p_sample(self, x, t: int, x_self_cond = None):
-        b, *_, device = *x.shape, x.device
-        batched_times = torch.full((b,), t, device = x.device, dtype = torch.long)
+        b, *_, device = *x.shape, self.device
+        batched_times = torch.full((b,), t, device = device, dtype = torch.long)
         model_mean, _, model_log_variance, x_start = self.p_mean_variance(x = x, t = batched_times, x_self_cond = x_self_cond, clip_denoised = True)
         noise = torch.randn_like(x) if t > 0 else 0. # no noise if t == 0
         pred_img = model_mean + (0.5 * model_log_variance).exp() * noise
         return pred_img, x_start
 
     @torch.no_grad()
     def p_sample_loop(self, shape, return_all_timesteps = False):
-        batch, device = shape[0], self.betas.device
+        batch, device = shape[0], self.device
 
         img = torch.randn(shape, device = device)
         imgs = [img]
 
         x_start = None
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
@@ -647,15 +654,15 @@
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.no_grad()
     def ddim_sample(self, shape, return_all_timesteps = False):
-        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.betas.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
+        batch, device, total_timesteps, sampling_timesteps, eta, objective = shape[0], self.device, self.num_timesteps, self.sampling_timesteps, self.ddim_sampling_eta, self.objective
 
         times = torch.linspace(-1, total_timesteps - 1, steps = sampling_timesteps + 1)   # [-1, 0, 1, 2, ..., T-1] when sampling_timesteps == total_timesteps
         times = list(reversed(times.int().tolist()))
         time_pairs = list(zip(times[:-1], times[1:])) # [(T-1, T-2), (T-2, T-3), ..., (1, 0), (0, -1)]
 
         img = torch.randn(shape, device = device)
         imgs = [img]
@@ -713,31 +720,26 @@
 
         for i in tqdm(reversed(range(0, t)), desc = 'interpolation sample time step', total = t):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
-    def q_sample(self, x_start, t, noise=None):
+    def q_sample(self, x_start, t, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
+        if self.offset_noise_strength > 0.:
+            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
+            noise += self.offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
+
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    @property
-    def loss_fn(self):
-        if self.loss_type == 'l1':
-            return F.l1_loss
-        elif self.loss_type == 'l2':
-            return F.mse_loss
-        else:
-            raise ValueError(f'invalid loss type {self.loss_type}')
-
     def p_losses(self, x_start, t, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -762,15 +764,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = self.loss_fn(model_out, target, reduction = 'none')
+        loss = F.mse_loss(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,15 +413,14 @@
     def __init__(
         self,
         model,
         *,
         seq_length,
         timesteps = 1000,
         sampling_timesteps = None,
-        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'cosine',
         ddim_sampling_eta = 0.,
         auto_normalize = True
     ):
         super().__init__()
         self.model = model
@@ -443,15 +442,14 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
-        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -663,23 +661,14 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    @property
-    def loss_fn(self):
-        if self.loss_type == 'l1':
-            return F.l1_loss
-        elif self.loss_type == 'l2':
-            return F.mse_loss
-        else:
-            raise ValueError(f'invalid loss type {self.loss_type}')
-
     def p_losses(self, x_start, t, noise = None):
         b, c, n = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -704,15 +693,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = self.loss_fn(model_out, target, reduction = 'none')
+        loss = F.mse_loss(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, n, device, seq_length, = *img.shape, img.device, self.seq_length
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,14 @@
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
-        loss_type = 'l1',
         objective = 'pred_noise',
         beta_schedule = 'sigmoid',
         schedule_fn_kwargs = dict(),
         ddim_sampling_eta = 0.,
         auto_normalize = True,
         min_snr_loss_weight = False,
         min_snr_gamma = 5
@@ -482,15 +481,14 @@
 
         alphas = 1. - betas
         alphas_cumprod = torch.cumprod(alphas, dim=0)
         alphas_cumprod_prev = F.pad(alphas_cumprod[:-1], (1, 0), value = 1.)
 
         timesteps, = betas.shape
         self.num_timesteps = int(timesteps)
-        self.loss_type = loss_type
 
         # sampling related parameters
 
         self.sampling_timesteps = default(sampling_timesteps, timesteps) # default num sampling timesteps to number of timesteps at training
 
         assert self.sampling_timesteps <= timesteps
         self.is_ddim_sampling = self.sampling_timesteps < timesteps
@@ -733,23 +731,14 @@
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    @property
-    def loss_fn(self):
-        if self.loss_type == 'l1':
-            return F.l1_loss
-        elif self.loss_type == 'l2':
-            return F.mse_loss
-        else:
-            raise ValueError(f'invalid loss type {self.loss_type}')
-
     def p_losses(self, x_start, t, noise = None):
         b, c, h, w = x_start.shape
         noise = default(noise, lambda: torch.randn_like(x_start))
 
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
@@ -774,15 +763,15 @@
             target = x_start
         elif self.objective == 'pred_v':
             v = self.predict_v(x_start, t, noise)
             target = v
         else:
             raise ValueError(f'unknown objective {self.objective}')
 
-        loss = self.loss_fn(model_out, target, reduction = 'none')
+        loss = F.mse_loss(model_out, target, reduction = 'none')
         loss = reduce(loss, 'b ... -> b (...)', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
@@ -1024,16 +1013,15 @@
         dim = 64,
         dim_mults = (1, 2, 4, 8)
     )
     image_size = 128
     diffusion = GaussianDiffusion(
         model,
         image_size = image_size,
-        timesteps = 1000,   # number of steps
-        loss_type = 'l1'    # L1 or L2
+        timesteps = 1000   # number of steps
     )
 
     classifier = Classifier(image_size=image_size, num_classes=1000, t_dim=1)
     batch_size = 4
     sampled_images = diffusion.sample(
         batch_size = batch_size,
         cond_fn=classifier_cond_fn,
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,10 +146,10 @@
 
         vb_losses = torch.where(t == 0, decoder_nll, kl)
 
         # simple loss - predicting noise, x0, or x_prev
 
         pred_noise, _ = model_output.chunk(2, dim = 1)
 
-        simple_losses = self.loss_fn(pred_noise, noise)
+        simple_losses = F.mse_loss(pred_noise, noise)
 
         return simple_losses + vb_losses.mean() * self.vb_loss_weight
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
         model_output = self.model(x_t, t)
         pred_noise, pred_x_start, weights = model_output.split(self.split_dims, dim = 1)
 
         # get loss for predicted noise and x_start
         # with the loss weight given at initialization
 
-        noise_loss = self.loss_fn(noise, pred_noise) * self.pred_noise_loss_weight
-        x_start_loss = self.loss_fn(x_start, pred_x_start) * self.pred_x_start_loss_weight
+        noise_loss = F.mse_loss(noise, pred_noise) * self.pred_noise_loss_weight
+        x_start_loss = F.mse_loss(x_start, pred_x_start) * self.pred_x_start_loss_weight
 
         # calculate x_start from predicted noise
         # then do a weighted sum of the x_start prediction, weights also predicted by the model (softmax normalized)
 
         x_start_from_pred_noise = self.predict_start_from_noise(x_t, t, pred_noise)
         x_start_from_pred_noise = x_start_from_pred_noise.clamp(-2., 2.)
         weighted_x_start = einsum('b j h w, b j c h w -> b c h w', weights.softmax(dim = 1), torch.stack((x_start_from_pred_noise, pred_x_start), dim = 1))
 
         # main loss to x_start with the weighted one
 
-        weighted_x_start_loss = self.loss_fn(x_start, weighted_x_start)
+        weighted_x_start_loss = F.mse_loss(x_start, weighted_x_start)
         return weighted_x_start_loss + x_start_loss + noise_loss
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.2
+Version: 1.6.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.2/setup.py` & `denoising-diffusion-pytorch-1.6.3/setup.py`

 * *Files identical despite different names*

