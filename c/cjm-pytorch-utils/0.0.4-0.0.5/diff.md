# Comparing `tmp/cjm-pytorch-utils-0.0.4.tar.gz` & `tmp/cjm-pytorch-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-pytorch-utils-0.0.4.tar", last modified: Thu Mar  2 00:29:43 2023, max compression
+gzip compressed data, was "cjm-pytorch-utils-0.0.5.tar", last modified: Sat May 20 18:51:57 2023, max compression
```

## Comparing `cjm-pytorch-utils-0.0.4.tar` & `cjm-pytorch-utils-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-03-02 00:29:43.524902 cjm-pytorch-utils-0.0.4/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-01-24 01:41:24.000000 cjm-pytorch-utils-0.0.4/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2022-09-05 16:31:43.000000 cjm-pytorch-utils-0.0.4/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3744 2023-03-02 00:29:43.524712 cjm-pytorch-utils-0.0.4/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2938 2023-03-02 00:23:21.000000 cjm-pytorch-utils-0.0.4/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-03-02 00:29:43.521848 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-03-02 00:23:16.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2029 2023-03-02 00:23:16.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3848 2023-03-02 00:23:16.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/core.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1628 2023-01-24 01:48:53.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/pytorch_utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-03-02 00:29:43.524326 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3744 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      459 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-01-24 01:52:44.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-03-02 00:29:43.000000 cjm-pytorch-utils-0.0.4/cjm_pytorch_utils.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      982 2023-03-02 00:10:54.000000 cjm-pytorch-utils-0.0.4/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-03-02 00:29:43.524956 cjm-pytorch-utils-0.0.4/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2541 2022-09-05 16:31:43.000000 cjm-pytorch-utils-0.0.4/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-05-20 18:51:57.682662 cjm-pytorch-utils-0.0.5/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-01-24 01:41:24.000000 cjm-pytorch-utils-0.0.5/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2022-09-05 16:31:43.000000 cjm-pytorch-utils-0.0.5/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3569 2023-05-20 18:51:57.682448 cjm-pytorch-utils-0.0.5/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2763 2023-05-20 18:47:46.000000 cjm-pytorch-utils-0.0.5/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-05-20 18:51:57.679900 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-05-20 18:47:41.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2157 2023-05-20 18:47:41.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     4736 2023-05-20 18:47:41.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/core.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1628 2023-01-24 01:48:53.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/pytorch_utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-05-20 18:51:57.682102 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3569 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      459 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-01-24 01:52:44.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-05-20 18:51:57.000000 cjm-pytorch-utils-0.0.5/cjm_pytorch_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      982 2023-05-20 18:51:54.000000 cjm-pytorch-utils-0.0.5/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-05-20 18:51:57.682728 cjm-pytorch-utils-0.0.5/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2541 2022-09-05 16:31:43.000000 cjm-pytorch-utils-0.0.5/setup.py
```

### Comparing `cjm-pytorch-utils-0.0.4/LICENSE` & `cjm-pytorch-utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/_modidx.py` & `cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   'syms': { 'cjm_pytorch_utils.core': { 'cjm_pytorch_utils.core.denorm_img_tensor': ( 'core.html#denorm_img_tensor',
                                                                                       'cjm_pytorch_utils/core.py'),
                                         'cjm_pytorch_utils.core.get_torch_device': ( 'core.html#get_torch_device',
                                                                                      'cjm_pytorch_utils/core.py'),
                                         'cjm_pytorch_utils.core.iterate_modules': ( 'core.html#iterate_modules',
                                                                                     'cjm_pytorch_utils/core.py'),
                                         'cjm_pytorch_utils.core.pil_to_tensor': ('core.html#pil_to_tensor', 'cjm_pytorch_utils/core.py'),
+                                        'cjm_pytorch_utils.core.set_seed': ('core.html#set_seed', 'cjm_pytorch_utils/core.py'),
                                         'cjm_pytorch_utils.core.tensor_stats_df': ( 'core.html#tensor_stats_df',
                                                                                     'cjm_pytorch_utils/core.py'),
                                         'cjm_pytorch_utils.core.tensor_to_pil': ('core.html#tensor_to_pil', 'cjm_pytorch_utils/core.py')},
             'cjm_pytorch_utils.pytorch_utils': { 'cjm_pytorch_utils.pytorch_utils.pil_to_tensor': ( 'core.html#pil_to_tensor',
                                                                                                     'cjm_pytorch_utils/pytorch_utils.py'),
                                                  'cjm_pytorch_utils.pytorch_utils.tensor_to_pil': ( 'core.html#tensor_to_pil',
                                                                                                     'cjm_pytorch_utils/pytorch_utils.py')}}}
```

### Comparing `cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/core.py` & `cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['pil_to_tensor', 'tensor_to_pil', 'iterate_modules', 'tensor_stats_df', 'get_torch_device', 'denorm_img_tensor']
+__all__ = ['set_seed', 'pil_to_tensor', 'tensor_to_pil', 'iterate_modules', 'tensor_stats_df', 'get_torch_device',
+           'denorm_img_tensor']
 
 # %% ../nbs/00_core.ipynb 3
 # Import necessary modules from the standard library
 from pathlib import Path  # For working with file paths
 import logging  # For logging messages
 import hashlib
+import random
 
 # Disable logging warnings
 logging.disable(logging.WARNING)
 
 import numpy as np  # For working with arrays
 
 from PIL import Image  # For working with images
 
 import torch  # PyTorch module for deep learning
 from torchvision import transforms  # PyTorch module for image transformations
 
 # %% ../nbs/00_core.ipynb 5
+def set_seed(seed: int, # The seed value to be set for all random number generators.
+             deterministic: bool = False # If True, uses deterministic algorithms in PyTorch where possible for reproducibility, at the cost of performance.
+            ) -> None:
+    """
+    Sets the seed for generating random numbers in PyTorch, NumPy, and Python's random module.
+
+    This function is used for reproducibility in stochastic operations, e.g. shuffling in data loaders,
+    random initializations in neural networks, etc.
+
+    Note: The deterministic flag does not guarantee complete reproducibility. Operations which rely on CUDA might
+    still produce non-deterministic results.
+    """
+    torch.manual_seed(seed)
+    np.random.seed(seed)
+    random.seed(seed)
+    torch.use_deterministic_algorithms(deterministic)
+
+# %% ../nbs/00_core.ipynb 8
 def pil_to_tensor(img:Image, # The input PIL image.
                   mean=[0.485, 0.456, 0.406], # The mean values for normalization.
                   std=[0.229, 0.224, 0.225] # The standard deviation values for normalization.
                  ):
     """
     Converts a PIL image to a normalized and batched PyTorch tensor.
     
     Returns:
         The normalized and batched tensor.
     """
     
     return transforms.Normalize(mean, std)(transforms.ToTensor()(img))[None]
 
-# %% ../nbs/00_core.ipynb 13
+# %% ../nbs/00_core.ipynb 16
 def tensor_to_pil(tensor: torch.Tensor # The tensor to be converted
                  ):
     """
     Convert a tensor to a PIL image.
     
     Returns:
     img (PIL.Image): The PIL image
@@ -45,40 +65,40 @@
     
     # Remove the first dimension if the tensor has 4 dimensions
     if len(tensor.shape) == 4: tensor.squeeze_(0)
         
     # Use the ToPILImage() function from the transforms module to convert the tensor to a PIL image
     return transforms.ToPILImage()(tensor)
 
-# %% ../nbs/00_core.ipynb 17
+# %% ../nbs/00_core.ipynb 20
 def iterate_modules(module: torch.nn.Module): # A PyTorch module that contains child modules to be iterated over.
     """
     A generator function that yields the children and grandchildren of a PyTorch module.    
     """
     
     for child in module.children():
         yield child
         yield from iterate_modules(child)
 
-# %% ../nbs/00_core.ipynb 20
+# %% ../nbs/00_core.ipynb 23
 import pandas as pd
 
-# %% ../nbs/00_core.ipynb 21
+# %% ../nbs/00_core.ipynb 24
 def tensor_stats_df(tensor, # Input tensor for which statistics are to be calculated.
                     attrs = ["mean", "std", "min", "max"], # List of statistics to be calculated.
                     shape=True): # If True, include shape of the tensor in the output.
     """
     Calculate and return statistics of a given tensor as a pandas DataFrame.
     """
     
     attr_dict = {attr: getattr(tensor, attr)().item() for attr in attrs}
     if shape: attr_dict["shape"] = tensor.shape
     return pd.DataFrame.from_dict(attr_dict, orient='index')
 
-# %% ../nbs/00_core.ipynb 24
+# %% ../nbs/00_core.ipynb 27
 def get_torch_device():
     """
     This function returns the device to be used for PyTorch computations.
     
     Returns:
     str: "mps" if Metal Performance Shaders (MPS) for MacOS is available, 
          "cuda" if CUDA is available, 
@@ -89,15 +109,15 @@
         if torch.backends.mps.is_available()
         else "cuda"
         if torch.cuda.is_available()
         else "cpu"
     )
     return device
 
-# %% ../nbs/00_core.ipynb 27
+# %% ../nbs/00_core.ipynb 30
 def denorm_img_tensor(img_tensor:torch.Tensor, # The tensor representing the normalized image.
                       mean:list, # The mean values used for normalization.
                       std:list): # The standard deviation values used for normalization.
     """
     Denormalize an image tensor.
     
     Returns:
```

### Comparing `cjm-pytorch-utils-0.0.4/cjm_pytorch_utils/pytorch_utils.py` & `cjm-pytorch-utils-0.0.5/cjm_pytorch_utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `cjm-pytorch-utils-0.0.4/settings.ini` & `cjm-pytorch-utils-0.0.5/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-pytorch-utils
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_pytorch_utils
 nbs_path = nbs
```

### Comparing `cjm-pytorch-utils-0.0.4/setup.py` & `cjm-pytorch-utils-0.0.5/setup.py`

 * *Files identical despite different names*

