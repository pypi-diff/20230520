# Comparing `tmp/vtclear-0.9.tar.gz` & `tmp/vtclear-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vtclear-0.9.tar", last modified: Wed Mar  6 21:18:25 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

