# Comparing `tmp/sarf-0.3.0.tar.gz` & `tmp/sarf-1.0.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarf-0.3.0.tar", last modified: Thu Sep  1 16:24:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

