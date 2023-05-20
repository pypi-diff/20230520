# Comparing `tmp/mlm8s-1.0.1.tar.gz` & `tmp/mlm8s-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlm8s-1.0.1.tar", max compression
+gzip compressed data, was "mlm8s-1.0.2.tar", max compression
```

## Comparing `mlm8s-1.0.1.tar` & `mlm8s-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-04-29 12:39:38.358629 mlm8s-1.0.1/LICENSE
--rw-r--r--   0        0        0     2301 2023-04-29 12:39:38.358629 mlm8s-1.0.1/README.md
--rw-r--r--   0        0        0      425 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/__init__.py
--rw-r--r--   0        0        0     1436 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/chaos.py
--rw-r--r--   0        0        0      609 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/connect.py
--rw-r--r--   0        0        0     2235 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/custom_metrices.py
--rw-r--r--   0        0        0     1626 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/generator.py
--rw-r--r--   0        0        0     1751 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/helpers.py
--rw-r--r--   0        0        0     2683 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/hypermodel.py
--rw-r--r--   0        0        0     4208 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/lattice.py
--rw-r--r--   0        0        0      808 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/numeric.py
--rw-r--r--   0        0        0     1001 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/overview - metrics
--rw-r--r--   0        0        0     2124 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/paths.py
--rw-r--r--   0        0        0      907 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/plot.py
--rw-r--r--   0        0        0     5936 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/polynom.py
--rw-r--r--   0        0        0     1004 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/rounding_loss.py
--rw-r--r--   0        0        0     3539 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/sparse.py
--rw-r--r--   0        0        0     6658 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/spiral.py
--rw-r--r--   0        0        0     5444 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/text.py
--rw-r--r--   0        0        0      872 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/training.py
--rw-r--r--   0        0        0      757 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/triangle.py
--rw-r--r--   0        0        0     5352 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/voltera.py
--rw-r--r--   0        0        0     1172 2023-04-29 12:39:38.358629 mlm8s-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 mlm8s-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-20 17:28:49.162431 mlm8s-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2373 2023-05-20 17:28:49.162431 mlm8s-1.0.2/README.md
+-rw-r--r--   0        0        0      425 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/__init__.py
+-rw-r--r--   0        0        0     1436 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/chaos.py
+-rw-r--r--   0        0        0      609 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/connect.py
+-rw-r--r--   0        0        0     2235 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/custom_metrices.py
+-rw-r--r--   0        0        0     1626 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/generator.py
+-rw-r--r--   0        0        0     1839 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/helpers.py
+-rw-r--r--   0        0        0     2683 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/hypermodel.py
+-rw-r--r--   0        0        0     4208 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/lattice.py
+-rw-r--r--   0        0        0      808 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/numeric.py
+-rw-r--r--   0        0        0     1001 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/overview - metrics
+-rw-r--r--   0        0        0     2124 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/paths.py
+-rw-r--r--   0        0        0      953 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/plot.py
+-rw-r--r--   0        0        0     5936 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/polynom.py
+-rw-r--r--   0        0        0     1004 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/rounding_loss.py
+-rw-r--r--   0        0        0     3539 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/sparse.py
+-rw-r--r--   0        0        0     6658 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/spiral.py
+-rw-r--r--   0        0        0     5444 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/text.py
+-rw-r--r--   0        0        0      872 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/training.py
+-rw-r--r--   0        0        0      757 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/triangle.py
+-rw-r--r--   0        0        0     5352 2023-05-20 17:28:49.162431 mlm8s-1.0.2/mlm8s/voltera.py
+-rw-r--r--   0        0        0     1172 2023-05-20 17:28:49.162431 mlm8s-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 mlm8s-1.0.2/PKG-INFO
```

### Comparing `mlm8s-1.0.1/LICENSE` & `mlm8s-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/README.md` & `mlm8s-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 Enables alternating results of tf.random* -calls, from within
 the generator of tf.data.Dataset.from_generator*.
 
 ```
 kwargs = dict()
 kwargs['paths'] = paths
+kwargs['label_dict'] = label_dict
 kwargs['seperators'] = ['/', '.']
 kwargs['indices'] = [-2, 0]
 
 ### Feature-Engineering with generator, that can use random variables!!
 def engineer_features(paths):
     # use data in path to engineer features
     features = tf.random.uniform(shape=[32, 256, 256, 4])
@@ -54,14 +55,15 @@
 
 ### Creating Features & Labels:
 def generate_from_paths(batch_size=1024, **kwargs):
     paths = kwargs['paths']
     seperators = kwargs['seperators']
     indices = kwargs['indices']
     engineer_features = kwargs['engineer_features']
+    label_dict = kwargs['label_dict']
     rdm_paths = paths.get_rdm(batch_size)
     features = engineer_features(rdm_paths)
     labels = paths2labels(rdm_paths, seperators, indices)
     labels = map_via_dict(labels, label_dict)
     return features, labels
 
 ### Creating tf.data.Dataset, that can generate an infinite number of random batches
```

### Comparing `mlm8s-1.0.1/mlm8s/chaos.py` & `mlm8s-1.0.2/mlm8s/chaos.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/connect.py` & `mlm8s-1.0.2/mlm8s/connect.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/custom_metrices.py` & `mlm8s-1.0.2/mlm8s/custom_metrices.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/generator.py` & `mlm8s-1.0.2/mlm8s/generator.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/helpers.py` & `mlm8s-1.0.2/mlm8s/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,21 @@
 import numpy as np
 import tensorflow as tf
 
-@tf.function
 def standardize(x):
     x = (x-np.mean(x))/np.std(x)
     return x
 
-@tf.function
 def normalize(x):
     x = (x-np.min(x))/(np.max(x)-np.min(x))
     return x
 
-@tf.function
 def stretch(x, s):
     return x*[s, 1/s]
 
-@tf.function
-def rotate_deg(x, alpha_deg=45.):
-    alpha = -alpha_deg/90.*tf.asin(1.)
-    cos = tf.math.cos(alpha)
-    sin = tf.math.sin(alpha)
-    rot_matrix = [[cos, -sin], [sin, cos]]
-    rotated_x = tf.linalg.matmul(x, rot_matrix)
-    return rotated_x
-
-@tf.function
 def flatten(x):
     hm_ins = x.shape[0]
     x = np.reshape(x, [hm_ins, -1])
     return x
 
 def correlate(inputs, outputs, input_lag):
     lag = input_lag
@@ -38,31 +25,45 @@
 
 def group_unique(array, axis=0):
     a = array
     a = a[a[:, axis].argsort()]
     groups = np.split(a, np.unique(a[:, axis], return_index=True)[1][1:])
     return groups
 
+@tf.function
+def rotate_deg(x, alpha_deg=45.):
+    alpha = -alpha_deg/90.*tf.asin(1.)
+    cos = tf.math.cos(alpha)
+    sin = tf.math.sin(alpha)
+    rot_matrix = [[cos, -sin], [sin, cos]]
+    rotated_x = tf.linalg.matmul(x, rot_matrix)
+    return rotated_x
+
+def group_unique(array, axis=0):
+    a = array
+    a = a[a[:, axis].argsort()]
+    groups = np.split(a, np.unique(a[:, axis], return_index=True)[1][1:])
+    return groups
+
 
 @tf.function
 def span_polar_basis(x, y):
-    print("Traced")
     phi = tf.math.atan2(y, x)
     e_r = tf.stack([
                     tf.math.cos(phi),
                     tf.math.sin(phi)
                    ])
     e_phi = tf.stack([
                       tf.math.sin(phi) * -1,
                       tf.math.cos(phi)
                      ])
 
     e_r = tf.cast(e_r, dtype=tf.float32)
     e_phi = tf.cast(e_phi, dtype=tf.float32)
     return e_r, e_phi
 
-@tf.function
+
 def create_meshgrid(shape = tf.constant([10, 10, 10]), indexing = 'ij'):
     ranges = tf.map_fn(tf.range, shape, fn_output_signature = tf.RaggedTensorSpec(shape=[None],dtype=tf.int32))
     grid = tf.meshgrid(*ranges, indexing = indexing)
     grid = tf.stack(grid, axis=-1)
     return grid
```

### Comparing `mlm8s-1.0.1/mlm8s/hypermodel.py` & `mlm8s-1.0.2/mlm8s/hypermodel.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/lattice.py` & `mlm8s-1.0.2/mlm8s/lattice.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/numeric.py` & `mlm8s-1.0.2/mlm8s/numeric.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/overview - metrics` & `mlm8s-1.0.2/mlm8s/overview - metrics`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/paths.py` & `mlm8s-1.0.2/mlm8s/paths.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/plot.py` & `mlm8s-1.0.2/mlm8s/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import numpy as np
 from matplotlib import pyplot as plt
 import IPython.display as ipd
 import librosa
 
-def print_plot_play(path2file, sr=None):
+def print_plot_play(signal, sr=None):
     """ 
         - Prints & Plots information about an audio singal,
         - Creates player
-        
     """
-    signal, sr = librosa.load(path2file, sr=sr)
-    text = 'audiofile: ' + np.char.split(path2file, sep ='/').item(-1)[-1]
-    print('%s Fs = %d, x.shape = %s, x.dtype = %s' % (text, sr, signal.shape, signal.dtype))
+    if type(signal) == str:
+      path2file = signal
+      signal, sr = librosa.load(path2file, sr=sr)
+      text = 'audiofile: ' + np.char.split(path2file, sep ='/').item(-1)[-1]
+      print('%s Fs = %d, x.shape = %s, x.dtype = %s' % (text, sr, signal.shape, signal.dtype))
     
     fig, axs = plt.subplots(nrows=3, ncols=1, figsize=(12, 7))
-
     axs[0].plot(signal, color='gray')
     axs[0].set_xlabel('Time (samples)')
     axs[0].set_ylabel('Amplitude')
     axs[1].phase_spectrum(signal, Fs=sr, color='grey')
     axs[2].magnitude_spectrum(signal, Fs=sr, scale='dB', color='grey')
     fig.tight_layout()
     plt.show()
```

### Comparing `mlm8s-1.0.1/mlm8s/polynom.py` & `mlm8s-1.0.2/mlm8s/polynom.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/rounding_loss.py` & `mlm8s-1.0.2/mlm8s/rounding_loss.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/sparse.py` & `mlm8s-1.0.2/mlm8s/sparse.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/spiral.py` & `mlm8s-1.0.2/mlm8s/spiral.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/text.py` & `mlm8s-1.0.2/mlm8s/text.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/training.py` & `mlm8s-1.0.2/mlm8s/training.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/triangle.py` & `mlm8s-1.0.2/mlm8s/triangle.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/mlm8s/voltera.py` & `mlm8s-1.0.2/mlm8s/voltera.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.1/pyproject.toml` & `mlm8s-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlm8s"
 #version = "0.0.2.8"
-version = "1.0.1"
+version = "1.0.2"
 description = "utils & misc 4 mlm8s"
 license = "GPL-3.0-only"
 authors = ["2mrwolke"]
 readme = "README.md"
 packages = [{include = "mlm8s"}]
 homepage = "https://mlm8s.org/"
```

### Comparing `mlm8s-1.0.1/PKG-INFO` & `mlm8s-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlm8s
-Version: 1.0.1
+Version: 1.0.2
 Summary: utils & misc 4 mlm8s
 Home-page: https://mlm8s.org/
 License: GPL-3.0-only
 Author: 2mrwolke
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -55,14 +55,15 @@
 
 Enables alternating results of tf.random* -calls, from within
 the generator of tf.data.Dataset.from_generator*.
 
 ```
 kwargs = dict()
 kwargs['paths'] = paths
+kwargs['label_dict'] = label_dict
 kwargs['seperators'] = ['/', '.']
 kwargs['indices'] = [-2, 0]
 
 ### Feature-Engineering with generator, that can use random variables!!
 def engineer_features(paths):
     # use data in path to engineer features
     features = tf.random.uniform(shape=[32, 256, 256, 4])
@@ -72,14 +73,15 @@
 
 ### Creating Features & Labels:
 def generate_from_paths(batch_size=1024, **kwargs):
     paths = kwargs['paths']
     seperators = kwargs['seperators']
     indices = kwargs['indices']
     engineer_features = kwargs['engineer_features']
+    label_dict = kwargs['label_dict']
     rdm_paths = paths.get_rdm(batch_size)
     features = engineer_features(rdm_paths)
     labels = paths2labels(rdm_paths, seperators, indices)
     labels = map_via_dict(labels, label_dict)
     return features, labels
 
 ### Creating tf.data.Dataset, that can generate an infinite number of random batches
```

