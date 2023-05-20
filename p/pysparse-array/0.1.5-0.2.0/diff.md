# Comparing `tmp/pysparse-array-0.1.5.tar.gz` & `tmp/pysparse-array-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-0.1.5.tar", last modified: Thu May 18 13:19:17 2023, max compression
+gzip compressed data, was "pysparse-array-0.2.0.tar", last modified: Sat May 20 06:56:43 2023, max compression
```

## Comparing `pysparse-array-0.1.5.tar` & `pysparse-array-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.676799 pysparse-array-0.1.5/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1680 2023-05-18 11:13:40.000000 pysparse-array-0.1.5/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.5/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.5/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5091 2023-05-18 13:19:17.638477 pysparse-array-0.1.5/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4386 2023-05-18 13:18:38.000000 pysparse-array-0.1.5/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-18 12:07:42.000000 pysparse-array-0.1.5/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.370822 pysparse-array-0.1.5/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5091 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-18 13:19:17.677325 pysparse-array-0.1.5/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-18 12:07:54.000000 pysparse-array-0.1.5/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.636387 pysparse-array-0.1.5/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.5/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     9489 2023-05-18 12:33:48.000000 pysparse-array-0.1.5/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     6829 2023-05-18 12:03:39.000000 pysparse-array-0.1.5/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 06:56:43.669297 pysparse-array-0.2.0/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2328 2023-05-20 06:55:00.000000 pysparse-array-0.2.0/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.2.0/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.2.0/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 06:56:43.650516 pysparse-array-0.2.0/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4669 2023-05-20 06:55:56.000000 pysparse-array-0.2.0/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      773 2023-05-20 06:55:06.000000 pysparse-array-0.2.0/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 06:56:43.581943 pysparse-array-0.2.0/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 06:56:43.000000 pysparse-array-0.2.0/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-20 06:56:43.000000 pysparse-array-0.2.0/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-20 06:56:43.000000 pysparse-array-0.2.0/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       41 2023-05-20 06:56:43.000000 pysparse-array-0.2.0/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-20 06:56:43.000000 pysparse-array-0.2.0/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-20 06:56:43.669550 pysparse-array-0.2.0/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-20 06:55:23.000000 pysparse-array-0.2.0/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 06:56:43.640770 pysparse-array-0.2.0/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.2.0/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     9878 2023-05-20 06:51:45.000000 pysparse-array-0.2.0/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7682 2023-05-19 16:45:55.000000 pysparse-array-0.2.0/sparse/core.py
```

### Comparing `pysparse-array-0.1.5/HISTORY.md` & `pysparse-array-0.2.0/HISTORY.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [0.2.0] - 2023-05-20
+
+### Added
+- Additional "coords_dictionary" file included, which replaces the previous find_indices function and introduces significant loading speed-up of 2-3x. This version is not backwards compatible with arrays encoded using v0.1.*
+
+### Fixed
+- N/A
+
+### Changed
+- README tidied up a little.
+- One of the core to_sparse functions are now jitted - this introduces a slight speed-up. Reading from slow I/O formats (.h5) still takes a long time to convert to sparse.
+- tqdm now replaced with an in-house progress bar to reduce dependencies
+
+### Removed
+- find_indices now replaced with a static coords_dictionary.pkl file.
+
 ## [0.1.5] - 2023-05-18
 
 ### Added
 - N/A
 
 ### Fixed
 - N/A
```

### Comparing `pysparse-array-0.1.5/LICENSE.txt` & `pysparse-array-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.5/PKG-INFO` & `pysparse-array-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.5
+Version: 0.2.0
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
@@ -21,99 +21,101 @@
 
 For machine-learning purposes, a NumPy array might be stored in one of two formats:
 1) As a binary (extremely large, very fast to access)
 2) As a compressed file format like HDF5 (much smaller, much slower to access)
 
 Both of the above can be accessed in a memory-mapped fashion (to avoid OOM errors), but both require concessions in the form of either size or speed.
 
-PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into two (smaller) arrays - a 1D array containing all non-zero values, and a 2D array containing the mapped coordinates for these values in the original 'dense' array.
+PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into four files:
+- a 1D array containing all non-zero values
+- a 2D array containing the mapped coordinates for these values in the original 'dense' array
+- a 1D array containing the shape of the original dense array
+- and a pickled dictionary mapping dense-to-sparse row coordinates, new to v1.
 
-These mapped arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
+These arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
 
 # Example Code
 
 PySparse only provides you with two functions - one to encode an array, and one to load the encoded arrays.
 
 **Encoding an Array**
 
 ```
-from sparse import to_sparse, load_sparse
-import os
+> from sparse import to_sparse, load_sparse
+> import os
 
-print(to_sparse.__doc__)
+> print(to_sparse.__doc__)
 
     Convert and write a dense array to a sparse array
     :param array: numpy array to be converted
     :param savepath: filepath to write sparse array to
     :param chunksize: number of memmap rows to process at a time if array is np.memmap - if None, will convert the whole array in memory
     :param verbose: whether to print progress statements
     :return: None
 
-array = np.random.default_rng().integers(low=0, high=5, size=(10000))
-
-to_sparse(array=array,
-	  savepath='/.',
-	  chunksize=None,
-	  verbose=True)
+> array = np.random.default_rng().integers(low=0, high=5, size=(10000))
+> to_sparse(array=array,
+	        savepath='/.',
+	        chunksize=None,
+	        verbose=True)
 
 ==================================================
 Identifying sparse shape...
 ==================================================
 ==================================================
 Writing sparse arrays...
 ==================================================
 
-print(os.listdirs(savepath))
+> print(os.listdirs(savepath))
 
-['dense_shape.npy', 'sparse_data.npy', 'sparse_coords.npy']
+['dense_shape.npy', 'sparse_coords_dict.pkl', 'sparse_coords.npy', 'sparse_data.npy']
 
 ```
 **Decoding an Array**
 ```
-print(load_sparse.__doc__)
+> print(load_sparse.__doc__)
 
     Load a (memory-mapped) sparse array from disk
     :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
     :param coords_path: (optional) path to sparse coordinates array
+    :param coords_dict_path: (optional) path to dictionary mapping sparse to dense row coordinates
     :param shape: (optional) shape of the dense array, as either tuple or path to numpy array containing shape
     :return: SparseArray object
 
-
-encoded_array = load_sparse(data_path='./')
-
-print(encoded_array[100:110])
+> encoded_array = load_sparse(data_path='./')
+> print(encoded_array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(array[100:110])
+> print(array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(np.array_equal(array, encoded_array[:]))
+> print(np.array_equal(array, encoded_array[:]))
 
 True
 ```
 # Benchmarks
 
 Sample data is a sparse array of size (1102729, 288, 63).
 
 **Relative Sizes**
 - .npy binary = 80GB
 - HDF5 with maximal gzip compression = 1.79GB
-- SparseArray directory = 11.76GB
+- SparseArray directory = 11.77GB
 
 **Loading first 10,000 rows**
 - .npy binary (memory-mapped) = 39.3 µs (757 ns with cache)
 - HDF5 = 957 ms (898 ms with cache)
-- SparseArray = 626 ms (387 ms with cache)
+- SparseArray = 445 ms (402 ms with cache)
 
 **Loading random 10,000 rows**
 - .npy binary (memory-mapped) = 4.24 seconds (88 ms with cache)
 - HDF5 = 32 seconds (31 seconds with cache)
-- SparseArray = 6.52 seconds (374 ms with cache)
+- SparseArray = 2.28 seconds (320 ms with cache)
 
 Of course, there are so many caveats to this (sparsity of data, shape of data, computational power available, etc), so you'll just have to try it yourself to see whether it works for you.
 
 ## Important Considerations
 - SparseArray is NOT a child class of NumPy, and you can't perform functions directly on it. All operations must be done following an index call.
 - SparseArray is NOT a stable package. It is cobbled together using a mix of other packages, and you should always keep a copy of your data in a gold-standard format (e.g., HDF5). You should also perform basic sanity-checks of your own to ensure the encoded array does match the original as expected.
 - At present, SparseArray is read-only and does NOT support in-place modifying of the data. If you wish to change the data, you will need to change the gold-standard and re-encode your data from scratch.
```

### Comparing `pysparse-array-0.1.5/README.md` & `pysparse-array-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,99 +4,101 @@
 
 For machine-learning purposes, a NumPy array might be stored in one of two formats:
 1) As a binary (extremely large, very fast to access)
 2) As a compressed file format like HDF5 (much smaller, much slower to access)
 
 Both of the above can be accessed in a memory-mapped fashion (to avoid OOM errors), but both require concessions in the form of either size or speed.
 
-PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into two (smaller) arrays - a 1D array containing all non-zero values, and a 2D array containing the mapped coordinates for these values in the original 'dense' array.
+PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into four files:
+- a 1D array containing all non-zero values
+- a 2D array containing the mapped coordinates for these values in the original 'dense' array
+- a 1D array containing the shape of the original dense array
+- and a pickled dictionary mapping dense-to-sparse row coordinates, new to v1.
 
-These mapped arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
+These arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
 
 # Example Code
 
 PySparse only provides you with two functions - one to encode an array, and one to load the encoded arrays.
 
 **Encoding an Array**
 
 ```
-from sparse import to_sparse, load_sparse
-import os
+> from sparse import to_sparse, load_sparse
+> import os
 
-print(to_sparse.__doc__)
+> print(to_sparse.__doc__)
 
     Convert and write a dense array to a sparse array
     :param array: numpy array to be converted
     :param savepath: filepath to write sparse array to
     :param chunksize: number of memmap rows to process at a time if array is np.memmap - if None, will convert the whole array in memory
     :param verbose: whether to print progress statements
     :return: None
 
-array = np.random.default_rng().integers(low=0, high=5, size=(10000))
-
-to_sparse(array=array,
-	  savepath='/.',
-	  chunksize=None,
-	  verbose=True)
+> array = np.random.default_rng().integers(low=0, high=5, size=(10000))
+> to_sparse(array=array,
+	        savepath='/.',
+	        chunksize=None,
+	        verbose=True)
 
 ==================================================
 Identifying sparse shape...
 ==================================================
 ==================================================
 Writing sparse arrays...
 ==================================================
 
-print(os.listdirs(savepath))
+> print(os.listdirs(savepath))
 
-['dense_shape.npy', 'sparse_data.npy', 'sparse_coords.npy']
+['dense_shape.npy', 'sparse_coords_dict.pkl', 'sparse_coords.npy', 'sparse_data.npy']
 
 ```
 **Decoding an Array**
 ```
-print(load_sparse.__doc__)
+> print(load_sparse.__doc__)
 
     Load a (memory-mapped) sparse array from disk
     :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
     :param coords_path: (optional) path to sparse coordinates array
+    :param coords_dict_path: (optional) path to dictionary mapping sparse to dense row coordinates
     :param shape: (optional) shape of the dense array, as either tuple or path to numpy array containing shape
     :return: SparseArray object
 
-
-encoded_array = load_sparse(data_path='./')
-
-print(encoded_array[100:110])
+> encoded_array = load_sparse(data_path='./')
+> print(encoded_array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(array[100:110])
+> print(array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(np.array_equal(array, encoded_array[:]))
+> print(np.array_equal(array, encoded_array[:]))
 
 True
 ```
 # Benchmarks
 
 Sample data is a sparse array of size (1102729, 288, 63).
 
 **Relative Sizes**
 - .npy binary = 80GB
 - HDF5 with maximal gzip compression = 1.79GB
-- SparseArray directory = 11.76GB
+- SparseArray directory = 11.77GB
 
 **Loading first 10,000 rows**
 - .npy binary (memory-mapped) = 39.3 µs (757 ns with cache)
 - HDF5 = 957 ms (898 ms with cache)
-- SparseArray = 626 ms (387 ms with cache)
+- SparseArray = 445 ms (402 ms with cache)
 
 **Loading random 10,000 rows**
 - .npy binary (memory-mapped) = 4.24 seconds (88 ms with cache)
 - HDF5 = 32 seconds (31 seconds with cache)
-- SparseArray = 6.52 seconds (374 ms with cache)
+- SparseArray = 2.28 seconds (320 ms with cache)
 
 Of course, there are so many caveats to this (sparsity of data, shape of data, computational power available, etc), so you'll just have to try it yourself to see whether it works for you.
 
 ## Important Considerations
 - SparseArray is NOT a child class of NumPy, and you can't perform functions directly on it. All operations must be done following an index call.
 - SparseArray is NOT a stable package. It is cobbled together using a mix of other packages, and you should always keep a copy of your data in a gold-standard format (e.g., HDF5). You should also perform basic sanity-checks of your own to ensure the encoded array does match the original as expected.
 - At present, SparseArray is read-only and does NOT support in-place modifying of the data. If you wish to change the data, you will need to change the gold-standard and re-encode your data from scratch.
```

### Comparing `pysparse-array-0.1.5/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-0.2.0/pysparse_array.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.5
+Version: 0.2.0
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
@@ -21,99 +21,101 @@
 
 For machine-learning purposes, a NumPy array might be stored in one of two formats:
 1) As a binary (extremely large, very fast to access)
 2) As a compressed file format like HDF5 (much smaller, much slower to access)
 
 Both of the above can be accessed in a memory-mapped fashion (to avoid OOM errors), but both require concessions in the form of either size or speed.
 
-PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into two (smaller) arrays - a 1D array containing all non-zero values, and a 2D array containing the mapped coordinates for these values in the original 'dense' array.
+PySparse tries to find a middle ground. The package takes a given NumPy array, and encodes it into four files:
+- a 1D array containing all non-zero values
+- a 2D array containing the mapped coordinates for these values in the original 'dense' array
+- a 1D array containing the shape of the original dense array
+- and a pickled dictionary mapping dense-to-sparse row coordinates, new to v1.
 
-These mapped arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
+These arrays can then be re-loaded into a SparseArray class, from which indexing can be performed as if you were operating on the original dense array. PySparse will decode the desired indices on-the-fly using memory-mapping of the encoded coordinates, and provide the desired subarray in-memory.
 
 # Example Code
 
 PySparse only provides you with two functions - one to encode an array, and one to load the encoded arrays.
 
 **Encoding an Array**
 
 ```
-from sparse import to_sparse, load_sparse
-import os
+> from sparse import to_sparse, load_sparse
+> import os
 
-print(to_sparse.__doc__)
+> print(to_sparse.__doc__)
 
     Convert and write a dense array to a sparse array
     :param array: numpy array to be converted
     :param savepath: filepath to write sparse array to
     :param chunksize: number of memmap rows to process at a time if array is np.memmap - if None, will convert the whole array in memory
     :param verbose: whether to print progress statements
     :return: None
 
-array = np.random.default_rng().integers(low=0, high=5, size=(10000))
-
-to_sparse(array=array,
-	  savepath='/.',
-	  chunksize=None,
-	  verbose=True)
+> array = np.random.default_rng().integers(low=0, high=5, size=(10000))
+> to_sparse(array=array,
+	        savepath='/.',
+	        chunksize=None,
+	        verbose=True)
 
 ==================================================
 Identifying sparse shape...
 ==================================================
 ==================================================
 Writing sparse arrays...
 ==================================================
 
-print(os.listdirs(savepath))
+> print(os.listdirs(savepath))
 
-['dense_shape.npy', 'sparse_data.npy', 'sparse_coords.npy']
+['dense_shape.npy', 'sparse_coords_dict.pkl', 'sparse_coords.npy', 'sparse_data.npy']
 
 ```
 **Decoding an Array**
 ```
-print(load_sparse.__doc__)
+> print(load_sparse.__doc__)
 
     Load a (memory-mapped) sparse array from disk
     :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
     :param coords_path: (optional) path to sparse coordinates array
+    :param coords_dict_path: (optional) path to dictionary mapping sparse to dense row coordinates
     :param shape: (optional) shape of the dense array, as either tuple or path to numpy array containing shape
     :return: SparseArray object
 
-
-encoded_array = load_sparse(data_path='./')
-
-print(encoded_array[100:110])
+> encoded_array = load_sparse(data_path='./')
+> print(encoded_array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(array[100:110])
+> print(array[100:110])
 
 array([3, 0, 4, 4, 2, 2, 3, 4, 0, 0])
 
-print(np.array_equal(array, encoded_array[:]))
+> print(np.array_equal(array, encoded_array[:]))
 
 True
 ```
 # Benchmarks
 
 Sample data is a sparse array of size (1102729, 288, 63).
 
 **Relative Sizes**
 - .npy binary = 80GB
 - HDF5 with maximal gzip compression = 1.79GB
-- SparseArray directory = 11.76GB
+- SparseArray directory = 11.77GB
 
 **Loading first 10,000 rows**
 - .npy binary (memory-mapped) = 39.3 µs (757 ns with cache)
 - HDF5 = 957 ms (898 ms with cache)
-- SparseArray = 626 ms (387 ms with cache)
+- SparseArray = 445 ms (402 ms with cache)
 
 **Loading random 10,000 rows**
 - .npy binary (memory-mapped) = 4.24 seconds (88 ms with cache)
 - HDF5 = 32 seconds (31 seconds with cache)
-- SparseArray = 6.52 seconds (374 ms with cache)
+- SparseArray = 2.28 seconds (320 ms with cache)
 
 Of course, there are so many caveats to this (sparsity of data, shape of data, computational power available, etc), so you'll just have to try it yourself to see whether it works for you.
 
 ## Important Considerations
 - SparseArray is NOT a child class of NumPy, and you can't perform functions directly on it. All operations must be done following an index call.
 - SparseArray is NOT a stable package. It is cobbled together using a mix of other packages, and you should always keep a copy of your data in a gold-standard format (e.g., HDF5). You should also perform basic sanity-checks of your own to ensure the encoded array does match the original as expected.
 - At present, SparseArray is read-only and does NOT support in-place modifying of the data. If you wish to change the data, you will need to change the gold-standard and re-encode your data from scratch.
```

### Comparing `pysparse-array-0.1.5/setup.py` & `pysparse-array-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='0.1.5',
+    version='0.2.0',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-0.1.5/sparse/array_api.py` & `pysparse-array-0.2.0/sparse/array_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import numpy as np
 from numba import njit, types, prange, typed
-from numpy import ndarray
-
-from .core import find_indices
+import pickle
 import os
+from numpy import ndarray
 
 
-def load_sparse(data_path: str, coords_path=None, shape=None):
+def load_sparse(data_path: str, coords_path=None, coords_dict_path = None, shape=None):
     """
     Load a (memory-mapped) sparse array from disk
     :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
     :param coords_path: (optional) path to sparse coordinates array
+    :param coords_dict_path: (optional) path to dictionary mapping sparse to dense row coordinates
     :param shape: (optional) shape of the dense array, as either tuple or path to numpy array containing shape
     :return: SparseArray object
     """
     if os.path.isdir(data_path):
         coords_path = os.path.join(data_path, 'sparse_coords.npy')
+        coords_dict_path = os.path.join(data_path, 'sparse_coords_dict.pkl')
         shape = os.path.join(data_path, 'dense_shape.npy')
         data_path = os.path.join(data_path, 'sparse_data.npy')
 
-    return SparseArray(data_path, coords_path, shape, mode='r')
+    return SparseArray(data_path, coords_path, coords_dict_path, shape, mode='r')
 
 
 class SparseArray:
-    def __init__(self, data_path: str, coords_path: str, shape: str or tuple, mode='r'):
+    def __init__(self, data_path: str, coords_path: str, coords_dict_path, shape: str or tuple, mode='r'):
         self.data = np.load(data_path, mmap_mode=mode)
         self.data_dtype = self.data.dtype
 
         self.coords = np.load(coords_path, mmap_mode=mode)
         self.coords_shape = self.coords.shape
+        with open(coords_dict_path, 'rb') as f:
+            self.coords_dict = typed.Dict.empty(key_type=types.int64, value_type=types.UniTuple(types.int64, count=2))
+            coords_dict = pickle.load(f)
+            for key, value in coords_dict.items():
+                self.coords_dict[key] = value
 
         if shape is tuple:
             self.dense_shape = shape
         else:
             self.dense_shape = tuple(np.load(shape))
 
     def __getitem__(self, items):
@@ -114,18 +120,18 @@
         """
 
         # Specify the search function based on the type of index given
         search_function = {int: self.__find_rows_int,
                            np.ndarray: self.__find_rows_ndarray}
 
         # Find the target coordinates for the given row indices
-        find_coords, coords_present = search_function[type(row_idx)](self.coords, row_idx,
-                                                                     maxlen=self.coords_shape[0])
+        find_coords, coords_present = search_function[type(row_idx)](self.coords_dict, row_idx)
 
-        find_coords = np.concatenate([np.arange(start, end+1) for start, end in find_coords if start != -1])
+        find_coords = np.concatenate(find_coords)
+        find_coords = find_coords[find_coords >= 0]
 
         # Assuming the row indices have non-zero data...
         if coords_present:
             # Locate the coordinates of the non-zero data in the original dense array
             target_coords = self.coords[find_coords]
 
             # Some slightly complex indexing to identify the non-zero cells of the (indexed) target array
@@ -147,53 +153,57 @@
             # If the row indices have no non-zero data, return an array of zeros
             target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
                 (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
 
         return target_data
 
     @staticmethod
-    @njit(types.Tuple((types.int64[:], types.boolean))(types.Array(types.int32, 2, 'C', readonly=True), types.int64,
-                                                       types.int64))
-    def __find_rows_int(coords: np.ndarray, row_idx: int, maxlen: int) -> tuple[ndarray, bool]:
+    @njit(types.Tuple((types.List(types.Array(types.int64, 1, 'C')),
+                       types.boolean))(types.DictType(types.int64, types.UniTuple(types.int64, count=2)),
+                                       types.int64))
+    def __find_rows_int(coords_dict, row_idx: int) -> tuple[list[ndarray], bool]:
         """
-        Efficiently search the coordinates to find the indices that match the given row index
-        :param coords: numpy 2D array of coordinates
+        Efficiently search the coordinates to find the indices that match the given row indices
+        :param coords_dict: dictionary mapping each dense row index to the first/last indices of the coordinates
         :param row_idx: target row index (integer)
-        :param maxlen: maximum length of the coordinates array
-        :return: numpy array of coordinates that match the given row index
+        :return: numpy array of coordinates that match the given row indices
         """
 
-        # Start with an efficient binary tree search algorithm for identifying the start and end indices
-        start_point, end_point = find_indices(coords, row_idx, 0, maxlen - 1)
+        start, end = coords_dict[row_idx]
+        find_coords = [np.arange(start, end+1)] if start >= 0 else [np.array([-1])]
+        coords_present = True if start >= 0 else False
 
-        coords_present = True if start_point >= 0 else False
-
-        return np.array([i for i in range(start_point, end_point + 1)]), coords_present
+        return find_coords, coords_present
 
+    """
+        @njit(types.Tuple((types.List(types.Array(types.int64, 1, 'C')), types.boolean))(types.DictType(types.int64, types.UniTuple(types.int64, count=2)),
+                                                                                         types.Array(types.int64, 1, 'A')),
+              parallel=True)
+    """
     @staticmethod
-    @njit(types.Tuple((types.ListType(types.UniTuple(types.int64, 2)), types.boolean))(types.Array(types.int32, 2, 'C', readonly=True),
-                                                                                       types.Array(types.int64, 1, 'A'), types.int64),
-          parallel=True)
-    def __find_rows_ndarray(coords: np.ndarray, row_idx: np.ndarray, maxlen: int) -> (np.ndarray, bool):
+    def __find_rows_ndarray(coords_dict, row_idx: np.ndarray) -> tuple[list[ndarray], bool]:
         """
         Efficiently search the coordinates to find the indices that match the given row indices
-        :param coords: numpy 2D array of coordinates
+        :param coords_dict: dictionary mapping each dense row index to the first/last indices of the coordinates
         :param row_idx: target row indices (numpy array)
-        :param maxlen: maximum length of the coordinates array
         :return: numpy array of coordinates that match the given row indices
         """
 
-        find_coords = typed.List([(-1, -1) for _ in range(len(row_idx))])
+        find_coords = [np.array([-1]) for _ in range(len(row_idx))]
+        coords_present = False
 
         for row in prange(len(row_idx)):
-            # Start with an efficient binary tree search algorithm for identifying the start and end indices
-            start_point, end_point = find_indices(coords, row_idx[row], 0, maxlen - 1)
-            find_coords[row] = (start_point, end_point)
+            start, end = coords_dict[row_idx[row]]
+            find_coords[row] = np.arange(start, end+1) if start >= 0 else np.array([-1])
+
+            coords_present += True if start >= 0 else False
+
+        coords_present = bool(coords_present)
 
-        return find_coords, True
+        return find_coords, coords_present
 
     def __get_item(self, items) -> np.ndarray:
         """
         Get the values of the dense array at the given indices
         :param items: tuple of indices
         :return: dense numpy array values at the given indices
         """
```

### Comparing `pysparse-array-0.1.5/sparse/core.py` & `pysparse-array-0.2.0/sparse/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing import Iterable
+
 import numpy as np
+from numpy import ndarray
 from numpy.lib.format import open_memmap
-from tqdm import tqdm
 import os
-from numba import njit, types, prange
-
+from numba import njit, prange
+import pickle
 
 """
 ============================================================
 Sparse array conversion functions
 ============================================================
 """
 
@@ -15,56 +17,100 @@
 def announce_progress(message: str) -> None:
     """
     Print a message to the console
     :param message: message to print
     :return: None
     """
 
-    print('\n' + '='*50 + '\n' + message + '\n' + '='*50)
+    print('\n' + '=' * 30 + '\n' + message + '\n' + '=' * 30)
     return
 
 
-def __calc_sparse_shape(array: np.ndarray, chunksize: int, verbose: bool) -> tuple:
+def progress_bar(iteration, total_iterations):
+    """
+    Print a progress bar to the console
+    :param iteration: current iteration
+    :param total_iterations: total number of iterations
+    :return: None
+    """
+    bar_length = 30
+
+    percent = iteration / total_iterations
+    percent_complete = int(percent * 100)
+
+    progress = int(percent * bar_length)
+    progress = '[' + '#' * progress + ' ' * (bar_length - progress) + ']'
+
+    print(f'\r{progress} {percent_complete}% complete', end='', flush=True)
+    return
+
+
+def __calc_sparse_shape(array: np.ndarray, chunksize: int, verbose: bool) -> int:
     """
     Calculate the shape of the (pending) sparse array
     :param array: dense numpy array
     :param chunksize: chunksize to use for calculation - if None, will use the whole array
     :param verbose: whether to print progress statements
     :return: tuple of shape
     """
 
     data_shape = 0
     shape = array.shape
-    announce_progress('Identifying sparse shape...') if verbose else None
 
     if (chunksize is None) or (type(array) is np.ndarray):
         data_shape = np.count_nonzero(array)
 
     else:
-        for i in tqdm(range(0, shape[0], chunksize)) if verbose else range(0, shape[0], chunksize):
+        for i in range(0, shape[0], chunksize):
+            progress_bar(i, shape[0]) if verbose else None
             data_shape += np.count_nonzero(array[i:i + chunksize])
 
-    return (data_shape,)
+    return data_shape
 
 
-def __convert_to_sparse_data(array_chunk: np.ndarray, iteration: int) -> (np.ndarray, np.ndarray):
+@njit
+def __convert_to_sparse_data(sparse_coords, sparse_values, iteration: int, chunksize, sparse_coords_idx_baseline) -> (np.ndarray, np.ndarray):
     """
     Convert a chunk of a dense array to sparse data
-    :param array_chunk: chunk of dense array
-    :param iteration: chunk index
+    :param sparse_coords: sparse coordinates
+    :param sparse_values: sparse values
+    :param iteration: iteration number
+    :param prev_sparse_coords_max: maximum idx of the previous sparse coordinates
     :return: tuple of sparse coordinates and sparse values
     """
-
-    sparse_coords = np.nonzero(array_chunk)
-    sparse_values = array_chunk[sparse_coords]
     sparse_coords = list(sparse_coords)
     sparse_coords[0] += iteration
-    sparse_coords = np.stack(sparse_coords, axis=1)
+    sparse_coords_arr = np.empty((len(sparse_coords), sparse_coords[0].shape[0]), dtype=np.int64)
+    for row in range(len(sparse_coords)):
+        sparse_coords_arr[row] = sparse_coords[row]
+    sparse_coords = sparse_coords_arr.T
+    sparse_coords_dict = __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize,
+                                                           sparse_coords_idx_baseline)
+
+    return sparse_coords, sparse_values, sparse_coords_dict
+
 
-    return sparse_coords, sparse_values
+@njit(parallel=True)
+def __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize, sparse_coords_idx_baseline):
+    """
+    Convert a chunk of a dense array to sparse data
+    :param sparse_coords: sparse coordinates
+    :return: dictionary mapping dense rows to sparse coordinates
+    """
+    min_value = sparse_coords[:, 0].min()
+    max_value = sparse_coords[:, 0].max()
+    sparse_coords_dict = {i: (-1, -1) for i in range(iteration, iteration + chunksize)}
+
+    for dense_row in prange(min_value, max_value + 1):
+        sparse_to_dense_coords = np.where(sparse_coords[:, 0] == dense_row)[0]
+        if np.any(sparse_to_dense_coords):
+            sparse_coords_dict[dense_row] = (sparse_to_dense_coords.min() + sparse_coords_idx_baseline,
+                                             sparse_to_dense_coords.max() + sparse_coords_idx_baseline)
+
+    return sparse_coords_dict
 
 
 def __write_sparse_arrays(array: np.ndarray or np.memmap, path: 'str', chunksize: int, verbose: bool) -> None:
     """
     Simultaneously convert and write a dense array to sparse arrays
     :param array: dense numpy array to be converted
     :param path: path to write sparse arrays to
@@ -72,47 +118,65 @@
     :param verbose: whether to print progress statements
     :return:
     """
 
     # Identify the relevant shapes of the dense and sparse arrays
     dense_shape = array.shape
     dense_dtype = array.dtype
+    announce_progress('Identifying sparse shape...') if verbose else None
     nonzero_shape = __calc_sparse_shape(array, chunksize, verbose)
 
     # Create the sparse array binaries (memory-mapped)
     memmap_sparse_data = open_memmap(os.path.join(path, 'sparse_data.npy'),
                                      dtype=dense_dtype,
                                      mode='w+',
-                                     shape=nonzero_shape)
+                                     shape=(nonzero_shape,))
 
     memmap_sparse_coords = open_memmap(os.path.join(path, 'sparse_coords.npy'),
                                        dtype=np.int32,
                                        mode='w+',
-                                       shape=(nonzero_shape[0], len(dense_shape)))
+                                       shape=(nonzero_shape, len(dense_shape)))
 
     np.save(os.path.join(path, 'dense_shape.npy'), dense_shape)
 
     # Convert the dense array to sparse arrays
     announce_progress('Writing sparse arrays...') if verbose else None
     sparse_index = 0
 
     if (chunksize is None) or (type(array) is np.ndarray):
-        sparse_coords, sparse_values = __convert_to_sparse_data(array, 0)
+        # Use of the bool dtype accelerates this step
+        sparse_coords = array.astype(bool).nonzero()
+        sparse_values = array[sparse_coords]
+        sparse_coords, sparse_values, sparse_coords_dict = __convert_to_sparse_data(sparse_coords, sparse_values, 0, 0)
 
         memmap_sparse_coords[:] = sparse_coords
         memmap_sparse_data[:] = sparse_values
 
     else:
-        for chunk_idx in tqdm(range(0, dense_shape[0], chunksize)) if verbose else range(0, dense_shape[0], chunksize):
-            sparse_coords, sparse_values = __convert_to_sparse_data(array[chunk_idx:chunk_idx + chunksize], chunk_idx)
+        sparse_coords_dict = {}
+        sparse_coords_idx_baseline = 0
+        for chunk_idx in range(0, dense_shape[0], chunksize):
+            progress_bar(chunk_idx, dense_shape[0]) if verbose else None
+            array_chunk = array[chunk_idx:chunk_idx + chunksize]
+            # Use of the bool dtype accelerates this step
+            sparse_coords = array_chunk.astype(bool).nonzero()
+            sparse_values = array_chunk[sparse_coords]
+            sparse_coords, sparse_values, sparse_coords_dict_temp = __convert_to_sparse_data(sparse_coords, sparse_values,
+                                                                                             chunk_idx, chunksize,
+                                                                                             sparse_coords_idx_baseline)
 
             memmap_sparse_coords[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_coords
             memmap_sparse_data[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_values
+            sparse_coords_dict.update(sparse_coords_dict_temp)
 
             sparse_index += sparse_coords.shape[0]
+            sparse_coords_idx_baseline = sparse_coords_dict[min(chunk_idx + chunksize - 1, dense_shape[0]-1)][1] + 1
+
+    with open(os.path.join(path, 'sparse_coords_dict.pkl'), 'wb') as f:
+        pickle.dump(sparse_coords_dict, f)
 
     return
 
 
 def to_sparse(array: np.ndarray or np.memmap, savepath: 'str', chunksize=1000, verbose=True) -> None:
     """
     Convert and write a dense array to a sparse array
@@ -123,73 +187,7 @@
     :return: None
     """
     if not os.path.isdir(savepath):
         os.makedirs(savepath)
 
     __write_sparse_arrays(array, savepath, chunksize, verbose)
     return
-
-
-@njit(types.UniTuple(types.int64, 2)(types.Array(types.int32, 2, 'C', readonly=True), types.int64, types.int64,
-                                     types.int64), cache=True)
-def find_indices(coords, row_idx, start, end):
-    """
-    Find the start and end indices of a particular row coordinate in a sparse coordinates array
-    :param coords: array of sparse coordinates
-    :param row_idx: row index to find
-    :param start: start index of the array to search from
-    :param end: end index of the array to search to
-    :return:
-    """
-    if start > end:
-        # Target number not found in the array
-        return -1, -1
-
-    mid = (start + end) // 2
-
-    if coords[mid, 0] < row_idx:
-        # Target number is in the right half of the array
-        return find_indices(coords, row_idx, mid + 1, end)
-    elif coords[mid, 0] > row_idx:
-        # Target number is in the left half of the array
-        return find_indices(coords, row_idx, start, mid - 1)
-    else:
-        # Found the target number, now find the start and end indices
-        start_index = end_index = mid
-
-        # Find the start index
-        step = 1
-        while start_index > start and coords[start_index - step, 0] == row_idx:
-            start_index -= step
-            step *= 2
-
-        # Refine the start index using binary search
-        left = start_index - step
-        right = start_index
-        while left < right:
-            mid = (left + right) // 2
-            if coords[mid, 0] == row_idx:
-                start_index = mid
-                right = mid
-            else:
-                left = mid + 1
-
-        # Find the end index
-        step = 1
-        while end_index < end and coords[end_index + step, 0] == row_idx:
-            end_index += step
-            step *= 2
-
-        # Refine the end index using binary search
-        left = end_index
-        right = end_index + step
-        while left < right:
-            mid = (left + right) // 2
-            if coords[mid, 0] == row_idx:
-                end_index = mid
-                left = mid + 1
-            else:
-                right = mid
-
-        return start_index, end_index
-
-
```

