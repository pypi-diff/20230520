# Comparing `tmp/gfs_dynamical_core-0.1.1.tar.gz` & `tmp/gfs_dynamical_core-0.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfs_dynamical_core-0.1.1.tar", last modified: Sat May 20 07:34:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

