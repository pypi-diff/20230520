# Comparing `tmp/atramentarium-0.3.tar.gz` & `tmp/atramentarium-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atramentarium-0.3.tar", last modified: Wed Apr 24 21:30:52 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

