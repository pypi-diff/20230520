# Comparing `tmp/mixdiff-1.1.2.tar.gz` & `tmp/mixdiff-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixdiff-1.1.2.tar", last modified: Sat Feb 18 13:21:27 2023, max compression
+gzip compressed data, was "mixdiff-1.1.3.tar", last modified: Sat May 20 18:43:36 2023, max compression
```

## Comparing `mixdiff-1.1.2.tar` & `mixdiff-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 13:21:27.030524 mixdiff-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-18 13:21:15.000000 mixdiff-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-02-18 13:21:27.030524 mixdiff-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-02-18 13:21:15.000000 mixdiff-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 13:21:27.026524 mixdiff-1.1.2/mixdiff/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-18 13:21:15.000000 mixdiff-1.1.2/mixdiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-02-18 13:21:15.000000 mixdiff-1.1.2/mixdiff/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-18 13:21:15.000000 mixdiff-1.1.2/mixdiff/extrasmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-02-18 13:21:15.000000 mixdiff-1.1.2/mixdiff/imgtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-02-18 13:21:15.000000 mixdiff-1.1.2/mixdiff/tiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 13:21:27.030524 mixdiff-1.1.2/mixdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-02-18 13:21:27.000000 mixdiff-1.1.2/mixdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-18 13:21:27.000000 mixdiff-1.1.2/mixdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 13:21:27.000000 mixdiff-1.1.2/mixdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-18 13:21:27.000000 mixdiff-1.1.2/mixdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-18 13:21:27.000000 mixdiff-1.1.2/mixdiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 13:21:27.030524 mixdiff-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-02-18 13:21:15.000000 mixdiff-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-20 18:43:25.000000 mixdiff-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-20 18:43:36.010338 mixdiff-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-20 18:43:25.000000 mixdiff-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/mixdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20181 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/extrasmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/imgtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/mixdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 18:43:36.000000 mixdiff-1.1.3/mixdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:43:36.010338 mixdiff-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-20 18:43:25.000000 mixdiff-1.1.3/setup.py
```

### Comparing `mixdiff-1.1.2/LICENSE` & `mixdiff-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.2/PKG-INFO` & `mixdiff-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixdiff
-Version: 1.1.2
+Version: 1.1.3
 Summary: Mixture of Diffusers for scene composition and high resolution image generation .
 Home-page: https://github.com/albarji/mixture-of-diffusers
 Author: Alvaro Barbero
 License: MIT
 Keywords: artificial-intelligence,deep-learning,diffusion-models
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -21,16 +21,20 @@
 
 # Mixture of Diffusers
 
 ![2022-10-12 15_35_27 305133_A charming house in the countryside, by jakub rozalski, sunset lighting, elegant, highly detailed, s_640x640_schelms_seed7178915308_gc8_steps50](https://user-images.githubusercontent.com/9654655/195362341-bc7766c2-f5c6-40f2-b457-59277aa11027.png)
 
 [![Unit tests](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml/badge.svg)](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml)
 
+[![huggingface space](https://camo.githubusercontent.com/00380c35e60d6b04be65d3d94a58332be5cc93779f630bcdfc18ab9a3a7d3388/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f25463025394625413425393725323048756767696e67253230466163652d5370616365732d626c7565)](https://huggingface.co/spaces/albarji/mixture-of-diffusers)
+
 This repository holds various scripts and tools implementing a method for integrating a mixture of different diffusion processes collaborating to generate a single image. Each diffuser focuses on a particular region on the image, taking into account boundary effects to promote a smooth blending.
 
+If you prefer a more user friendly graphical interface to use this algorithm, I recommend trying the [Tiled Diffusion & VAE](https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111) plugin developed by pkuliyi2015 for [AUTOMATIC1111's stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui).
+
 ## Motivation
 
 Current image generation methods, such as Stable Diffusion, struggle to position objects at specific locations. While the content of the generated image (somewhat) reflects the objects present in the prompt, it is difficult to frame the prompt in a way that creates an specific composition. For instance, take a prompt expressing a complex composition such as
 
 > A charming house in the countryside on the left,
 > in the center a dirt road in the countryside crossing pastures,
 > on the right an old and rusty giant robot lying on a dirt road,
```

### Comparing `mixdiff-1.1.2/README.md` & `mixdiff-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Mixture of Diffusers
 
 ![2022-10-12 15_35_27 305133_A charming house in the countryside, by jakub rozalski, sunset lighting, elegant, highly detailed, s_640x640_schelms_seed7178915308_gc8_steps50](https://user-images.githubusercontent.com/9654655/195362341-bc7766c2-f5c6-40f2-b457-59277aa11027.png)
 
 [![Unit tests](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml/badge.svg)](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml)
 
+[![huggingface space](https://camo.githubusercontent.com/00380c35e60d6b04be65d3d94a58332be5cc93779f630bcdfc18ab9a3a7d3388/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f25463025394625413425393725323048756767696e67253230466163652d5370616365732d626c7565)](https://huggingface.co/spaces/albarji/mixture-of-diffusers)
+
 This repository holds various scripts and tools implementing a method for integrating a mixture of different diffusion processes collaborating to generate a single image. Each diffuser focuses on a particular region on the image, taking into account boundary effects to promote a smooth blending.
 
+If you prefer a more user friendly graphical interface to use this algorithm, I recommend trying the [Tiled Diffusion & VAE](https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111) plugin developed by pkuliyi2015 for [AUTOMATIC1111's stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui).
+
 ## Motivation
 
 Current image generation methods, such as Stable Diffusion, struggle to position objects at specific locations. While the content of the generated image (somewhat) reflects the objects present in the prompt, it is difficult to frame the prompt in a way that creates an specific composition. For instance, take a prompt expressing a complex composition such as
 
 > A charming house in the countryside on the left,
 > in the center a dirt road in the countryside crossing pastures,
 > on the right an old and rusty giant robot lying on a dirt road,
```

### Comparing `mixdiff-1.1.2/mixdiff/canvas.py` & `mixdiff-1.1.3/mixdiff/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
         # Prepare text embeddings
         for region in text2image_regions:
             region.tokenize_prompt(self.tokenizer)
             region.encode_prompt(self.text_encoder, self.device)
 
         # Create original noisy latents using the timesteps
-        latents_shape = (batch_size, self.unet.in_channels, canvas_height // 8, canvas_width // 8)
+        latents_shape = (batch_size, self.unet.config.in_channels, canvas_height // 8, canvas_width // 8)
         generator = torch.Generator(self.device).manual_seed(seed)
         init_noise = torch.randn(latents_shape, generator=generator, device=self.device)
 
         # Reset latents in seed reroll regions, if requested
         for region in reroll_regions:
             if region.reroll_mode == RerollModes.RESET.value:
                 region_shape = (latents_shape[0], latents_shape[1], region.latent_row_end - region.latent_row_init, region.latent_col_end - region.latent_col_init)
@@ -334,15 +334,15 @@
             region.encoded_prompt = torch.cat([uncond_embeddings, region.encoded_prompt])
 
         # Prepare image latents
         for region in image2image_regions:
             region.encode_reference_image(self.vae, device=self.device, generator=generator)
 
         # Prepare mask of weights for each region
-        mask_builder = MaskWeightsBuilder(latent_space_dim=self.unet.in_channels, nbatch=batch_size)
+        mask_builder = MaskWeightsBuilder(latent_space_dim=self.unet.config.in_channels, nbatch=batch_size)
         mask_weights = [mask_builder.compute_mask_weights(region).to(self.device) for region in text2image_regions]
 
         # Diffusion timesteps
         for i, t in tqdm(enumerate(self.scheduler.timesteps)):
             # Diffuse each region            
             noise_preds_regions = []
```

### Comparing `mixdiff-1.1.2/mixdiff/extrasmixin.py` & `mixdiff-1.1.3/mixdiff/extrasmixin.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.2/mixdiff/imgtools.py` & `mixdiff-1.1.3/mixdiff/imgtools.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.2/mixdiff/tiling.py` & `mixdiff-1.1.3/mixdiff/tiling.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         if seed_reroll_regions is None:
             seed_reroll_regions = []
         batch_size = 1
 
         # create original noisy latents using the timesteps
         height = tile_height + (grid_rows - 1) * (tile_height - tile_row_overlap)
         width = tile_width + (grid_cols - 1) * (tile_width - tile_col_overlap)
-        latents_shape = (batch_size, self.unet.in_channels, height // 8, width // 8)
+        latents_shape = (batch_size, self.unet.config.in_channels, height // 8, width // 8)
         generator = torch.Generator("cuda").manual_seed(seed)
         latents = torch.randn(latents_shape, generator=generator, device=self.device)
 
         # overwrite latents for specific tiles if provided
         if seed_tiles is not None:
             for row in range(grid_rows):
                 for col in range(grid_cols):
@@ -200,18 +200,15 @@
                     px_row_init, px_row_end, px_col_init, px_col_end = _tile2latent_indices(row, col, tile_width, tile_height, tile_row_overlap, tile_col_overlap)
                     noise_pred[:, :, px_row_init:px_row_end, px_col_init:px_col_end] += noise_preds[row][col] * tile_weights
                     contributors[:, :, px_row_init:px_row_end, px_col_init:px_col_end] += tile_weights
             # Average overlapping areas with more than 1 contributor
             noise_pred /= contributors
 
             # compute the previous noisy sample x_t -> x_t-1
-            if isinstance(self.scheduler, LMSDiscreteScheduler):
-                latents = self.scheduler.step(noise_pred, i, latents, **extra_step_kwargs)["prev_sample"]
-            else:
-                latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs)["prev_sample"]
+            latents = self.scheduler.step(noise_pred, t, latents).prev_sample
 
         # scale and decode the image latents with vae
         image = self.decode_latents(latents, cpu_vae)
 
         return {"sample": image}
 
     def _gaussian_weights(self, tile_width, tile_height, nbatches):
@@ -225,15 +222,15 @@
         var = 0.01
         midpoint = (latent_width - 1) / 2  # -1 because index goes from 0 to latent_width - 1
         x_probs = [exp(-(x-midpoint)*(x-midpoint)/(latent_width*latent_width)/(2*var)) / sqrt(2*pi*var) for x in range(latent_width)]
         midpoint = latent_height / 2
         y_probs = [exp(-(y-midpoint)*(y-midpoint)/(latent_height*latent_height)/(2*var)) / sqrt(2*pi*var) for y in range(latent_height)]
         
         weights = np.outer(y_probs, x_probs)
-        return torch.tile(torch.tensor(weights, device=self.device), (nbatches, self.unet.in_channels, 1, 1))
+        return torch.tile(torch.tensor(weights, device=self.device), (nbatches, self.unet.config.in_channels, 1, 1))
 
 
 
 def _tile2pixel_indices(tile_row, tile_col, tile_width, tile_height, tile_row_overlap, tile_col_overlap):
     """Given a tile row and column numbers returns the range of pixels affected by that tiles in the overall image
     
     Returns a tuple with:
```

### Comparing `mixdiff-1.1.2/mixdiff.egg-info/PKG-INFO` & `mixdiff-1.1.3/mixdiff.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixdiff
-Version: 1.1.2
+Version: 1.1.3
 Summary: Mixture of Diffusers for scene composition and high resolution image generation .
 Home-page: https://github.com/albarji/mixture-of-diffusers
 Author: Alvaro Barbero
 License: MIT
 Keywords: artificial-intelligence,deep-learning,diffusion-models
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -21,16 +21,20 @@
 
 # Mixture of Diffusers
 
 ![2022-10-12 15_35_27 305133_A charming house in the countryside, by jakub rozalski, sunset lighting, elegant, highly detailed, s_640x640_schelms_seed7178915308_gc8_steps50](https://user-images.githubusercontent.com/9654655/195362341-bc7766c2-f5c6-40f2-b457-59277aa11027.png)
 
 [![Unit tests](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml/badge.svg)](https://github.com/albarji/mixture-of-diffusers/actions/workflows/python-tests.yml)
 
+[![huggingface space](https://camo.githubusercontent.com/00380c35e60d6b04be65d3d94a58332be5cc93779f630bcdfc18ab9a3a7d3388/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f25463025394625413425393725323048756767696e67253230466163652d5370616365732d626c7565)](https://huggingface.co/spaces/albarji/mixture-of-diffusers)
+
 This repository holds various scripts and tools implementing a method for integrating a mixture of different diffusion processes collaborating to generate a single image. Each diffuser focuses on a particular region on the image, taking into account boundary effects to promote a smooth blending.
 
+If you prefer a more user friendly graphical interface to use this algorithm, I recommend trying the [Tiled Diffusion & VAE](https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111) plugin developed by pkuliyi2015 for [AUTOMATIC1111's stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui).
+
 ## Motivation
 
 Current image generation methods, such as Stable Diffusion, struggle to position objects at specific locations. While the content of the generated image (somewhat) reflects the objects present in the prompt, it is difficult to frame the prompt in a way that creates an specific composition. For instance, take a prompt expressing a complex composition such as
 
 > A charming house in the countryside on the left,
 > in the center a dirt road in the countryside crossing pastures,
 > on the right an old and rusty giant robot lying on a dirt road,
```

### Comparing `mixdiff-1.1.2/setup.py` & `mixdiff-1.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     packages=['mixdiff'],
     install_requires=[
         'numpy>=1.19,<2',
         'torch>=1.9,<2',
         'torchvision>=0.10,<1',
         'tqdm>=4.62,<5',
         'scipy==1.10.*',
-        'diffusers[torch]==0.7.*',
+        'diffusers[torch]==0.16.*',
         'ftfy==6.1.*',
         'gitpython==3.1.*',
         'ligo-segments==1.4.*',
         'torchvision==0.14.*',
-        'transformers==4.21.*'
+        'transformers==4.29.*'
     ],
     author="Alvaro Barbero",
     url='https://github.com/albarji/mixture-of-diffusers',
     license='MIT',
     classifiers=[
         'Development Status :: 1 - Planning',
         'Environment :: GPU :: NVIDIA CUDA',
```

