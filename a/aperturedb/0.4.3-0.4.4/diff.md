# Comparing `tmp/aperturedb-0.4.3.tar.gz` & `tmp/aperturedb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aperturedb-0.4.3.tar", last modified: Fri Mar 10 16:47:54 2023, max compression
+gzip compressed data, was "aperturedb-0.4.4.tar", last modified: Fri May 19 23:51:56 2023, max compression
```

## Comparing `aperturedb-0.4.3.tar` & `aperturedb-0.4.4.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 16:47:54.827500 aperturedb-0.4.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-10 16:41:20.000000 aperturedb-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1957 2023-03-10 16:47:54.827500 aperturedb-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1442 2023-03-10 16:41:20.000000 aperturedb-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 16:47:54.827500 aperturedb-0.4.3/aperturedb/
--rw-r--r--   0 root         (0) root         (0)     4412 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/BBoxDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/BlobDataCSV.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Blobs.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/BoundingBoxes.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/CSVParser.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ConnectionDataCSV.py
--rw-r--r--   0 root         (0) root         (0)    13623 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Connector.py
--rw-r--r--   0 root         (0) root         (0)     5224 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ConnectorRest.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Constraints.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/DaskManager.py
--rw-r--r--   0 root         (0) root         (0)     5219 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/DescriptorDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/DescriptorSetDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     9263 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Entities.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/EntityDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ImageDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     4834 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ImageDownloader.py
--rw-r--r--   0 root         (0) root         (0)    21476 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Images.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/KaggleData.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/NotebookHelpers.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Operations.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ParallelLoader.py
--rw-r--r--   0 root         (0) root         (0)    10598 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ParallelQuery.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Parallelizer.py
--rw-r--r--   0 root         (0) root         (0)     3869 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/PolygonDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Polygons.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/ProgressBar.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/PyTorchDataset.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/PytorchData.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Query.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/QueryGenerator.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/QueryTypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Sort.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Stats.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Subscriptable.py
--rw-r--r--   0 root         (0) root         (0)    21945 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Utils.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/VideoDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/VideoDownloader.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/Videos.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-03-10 16:41:20.000000 aperturedb-0.4.3/aperturedb/queryMessage_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 16:47:54.827500 aperturedb-0.4.3/aperturedb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1957 2023-03-10 16:47:54.000000 aperturedb-0.4.3/aperturedb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1515 2023-03-10 16:47:54.000000 aperturedb-0.4.3/aperturedb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 16:47:54.000000 aperturedb-0.4.3/aperturedb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-03-10 16:47:54.000000 aperturedb-0.4.3/aperturedb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-10 16:47:54.000000 aperturedb-0.4.3/aperturedb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 16:47:54.827500 aperturedb-0.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1377 2023-03-10 16:41:21.000000 aperturedb-0.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 16:47:54.827500 aperturedb-0.4.3/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/conftest.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/dbinfo.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/download_images.py
--rw-r--r--   0 root         (0) root         (0)     9832 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/generateInput.py
--rw-r--r--   0 root         (0) root         (0)     4832 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_Data.py
--rw-r--r--   0 root         (0) root         (0)     6309 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_Datawizard.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_ResponseHandler.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_Session.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_Stats.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_Utils.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-03-10 16:41:21.000000 aperturedb-0.4.3/test/test_torch_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-15 16:49:00.000000 aperturedb-0.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-05-19 23:51:56.817841 aperturedb-0.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-05-15 16:49:00.000000 aperturedb-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/aperturedb/
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BBoxDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BlobDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Blobs.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BoundingBoxes.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/CSVParser.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ConnectionDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)    13798 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Connector.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-05-19 19:28:21.000000 aperturedb-0.4.4/aperturedb/ConnectorRest.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Constraints.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DaskManager.py
+-rw-r--r--   0 root         (0) root         (0)     5329 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DescriptorDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DescriptorSetDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     9263 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Entities.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/EntityDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ImageDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     4834 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ImageDownloader.py
+-rw-r--r--   0 root         (0) root         (0)    21476 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Images.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/KaggleData.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/NotebookHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Operations.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ParallelLoader.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ParallelQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Parallelizer.py
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PolygonDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Polygons.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ProgressBar.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PyTorchDataset.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PytorchData.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Query.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/QueryGenerator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/QueryTypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Sort.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Stats.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Subscriptable.py
+-rw-r--r--   0 root         (0) root         (0)    18835 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Utils.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/VideoDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/VideoDownloader.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Videos.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-19 22:38:25.000000 aperturedb-0.4.4/aperturedb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/queryMessage_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/aperturedb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 23:51:56.817841 aperturedb-0.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 22:38:25.000000 aperturedb-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/dbinfo.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/download_images.py
+-rw-r--r--   0 root         (0) root         (0)    10159 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/generateInput.py
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Data.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Datawizard.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_ResponseHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Session.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Stats.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Success.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Utils.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_torch_connector.py
```

### Comparing `aperturedb-0.4.3/LICENSE` & `aperturedb-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/PKG-INFO` & `aperturedb-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.3
+Version: 0.4.4
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.3/README.md` & `aperturedb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/BBoxDataCSV.py` & `aperturedb-0.4.4/aperturedb/BBoxDataCSV.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,22 +56,29 @@
         dataset_id would be only inserted if it does not already exist in the database.
 
     """
 
     def __init__(self, filename, df=None, use_dask=False):
 
         super().__init__(filename, df=df, use_dask=use_dask)
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[5:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.constraints_keys = [x for x in self.header[5:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
 
-            self.img_key = self.header[0]
-            self.command = "AddBoundingBox"
+        self.props_keys = [x for x in self.header[5:]
+                           if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.constraints_keys = [x for x in self.header[5:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+
+        self.img_key = self.header[0]
+        self.command = "AddBoundingBox"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                "_BoundingBox": self.get_indexed_properties()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
 
         q = []
 
         img_id = self.df.loc[idx, self.img_key]
@@ -99,15 +106,15 @@
             "image_ref": img_ref,
             "rectangle": {
                 attr: val for attr, val in zip(rect_attrs, box_data)
             },
         }
         abb = self._basic_command(idx, custom_fields)
 
-        properties  = self.parse_properties(self.df, idx)
+        properties = self.parse_properties(idx)
         if properties:
             props = properties
             if "_label" in props:
                 abb[self.command]["label"] = props["_label"]
                 props.pop("_label")
             # Check if props is not empty after removing "_label"
             if props:
```

### Comparing `aperturedb-0.4.3/aperturedb/BlobDataCSV.py` & `aperturedb-0.4.4/aperturedb/BlobDataCSV.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,27 @@
         In the above example, the constraint_id ensures that a blob with the specified
         id would be only inserted if it does not already exist in the database.
     """
 
     def __init__(self, filename, df=None, use_dask=False):
 
         super().__init__(filename, df=df, use_dask=use_dask)
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[1:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX) and x != BLOB_PATH]
-            self.constraints_keys = [x for x in self.header[1:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.command = "AddBlob"
+
+        self.props_keys = [x for x in self.header[1:]
+                           if not x.startswith(CSVParser.CONSTRAINTS_PREFIX) and x != BLOB_PATH]
+        self.constraints_keys = [x for x in self.header[1:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.command = "AddBlob"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                "_Blob": self.get_indexed_properties()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
         filename = self.df.loc[idx, BLOB_PATH]
         blob_ok, blob = self.load_blob(filename)
         if not blob_ok:
             logger.error("Error loading blob: " + filename)
```

### Comparing `aperturedb-0.4.3/aperturedb/CSVParser.py` & `aperturedb-0.4.4/aperturedb/CSVParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import multiprocessing as mp
 
 
 logger = logging.getLogger(__name__)
 
 ENTITY_CLASS      = "EntityClass"
 CONSTRAINTS_PREFIX = "constraint_"
+DATE_PREFIX = "date:"
 PROPERTIES  = "properties"
 CONSTRAINTS = "constraints"
 
 # This number is based on the partitions one wants to use per core.
 PARTITIONS_PER_CORE = 10
 
 # Use 90% os the CPU cores by default.
@@ -45,61 +46,67 @@
             # It'll impact the number of partitions, and memory usage.
             # TODO: tune this for the best performance.
             cores_used = int(CORES_USED_FOR_PARALLELIZATION * mp.cpu_count())
             self.df = dataframe.read_csv(
                 self.filename,
                 blocksize = os.path.getsize(self.filename) // (cores_used * PARTITIONS_PER_CORE))
 
-        if len(self.df) == 0:
+        # len for dask dataframe needs a client.
+        if not use_dask and len(self.df) == 0:
             logger.error("Dataframe empty. Is the CSV file ok?")
 
         self.df = self.df.astype('object')
         self.header = list(self.df.columns.values)
         self.validate()
 
     def __len__(self):
-
         return len(self.df.index)
 
-    def parse_properties(self, df, idx):
+    def get_indexed_properties(self):
+        if self.constraints_keys:
+            return {self._parse_prop(k)[0] for k in self.constraints_keys}
+        return set()
+
+    def get_indices(self):
+        raise NotImplementedError
+
+    def _parse_prop(self, key, val=None):
+        if key.startswith(CONSTRAINTS_PREFIX):
+            key = key[len(CONSTRAINTS_PREFIX):]
+        if key.startswith(DATE_PREFIX):
+            key = key[len(DATE_PREFIX):]
+            val = {"_date": val}
+        return key, val
+
+    def parse_properties(self, idx):
 
         properties = {}
-        if len(self.props_keys) > 0:
+        if self.props_keys:
             for key in self.props_keys:
-                # Handle Date data type
-                if key.startswith("date:"):
-                    prop = key[len("date:"):]  # remove prefix
-                    properties[prop] = {"_date": self.df.loc[idx, key]}
-                else:
-                    value = self.df.loc[idx, key]
-                    if value == value:  # skips nan values
-                        properties[key] = value
+                prop, value = self._parse_prop(key, self.df.loc[idx, key])
+                if value == value:  # skips nan values
+                    properties[prop] = value
 
         return properties
 
-    def parse_constraints(self, df, idx):
+    def parse_constraints(self, idx):
 
         constraints = {}
-        if len(self.constraints_keys) > 0:
+        if self.constraints_keys:
             for key in self.constraints_keys:
-                if key.startswith("constraint_date:"):
-                    prop = key[len("constraint_date:"):]  # remove prefix
-                    constraints[prop] = [
-                        "==", {"_date": self.df.loc[idx, key]}]
-                else:
-                    prop = key[len(CONSTRAINTS_PREFIX):]  # remove "prefix
-                    constraints[prop] = ["==", self.df.loc[idx, key]]
+                prop, value = self._parse_prop(key, self.df.loc[idx, key])
+                constraints[prop] = ["==", value]
 
         return constraints
 
     def _basic_command(self, idx, custom_fields: dict = None):
         if custom_fields == None:
             custom_fields = {}
-        properties = self.parse_properties(self.df, idx)
-        constraints = self.parse_constraints(self.df, idx)
+        properties = self.parse_properties(idx)
+        constraints = self.parse_constraints(idx)
         query = {
             self.command: custom_fields
         }
         if properties:
             query[self.command][PROPERTIES] = properties
 
         if constraints:
```

### Comparing `aperturedb-0.4.3/aperturedb/ConnectionDataCSV.py` & `aperturedb-0.4.4/aperturedb/ConnectionDataCSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,34 @@
         In the above example, the constraint_id ensures that a connection with the specified
         id would be only inserted if it does not already exist in the database.
 
     """
 
     def __init__(self, filename, df=None, use_dask=False):
         super().__init__(filename, df=df, use_dask=use_dask)
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[3:]
-                                     if not x.startswith(CONSTRAINTS_PREFIX)]
-
-            self.constraints_keys = [x for x in self.header[3:]
-                                     if x.startswith(CONSTRAINTS_PREFIX)]
-
-            self.src_class   = self.header[1].split("@")[0]
-            self.src_key     = self.header[1].split("@")[1]
-            self.dst_class   = self.header[2].split("@")[0]
-            # Pandas appends a .n to the column name if there is a duplicate
-            self.dst_key     = self.header[2].split("@")[1].split(".")[0]
-            self.command     = "AddConnection"
+
+        self.props_keys       = [x for x in self.header[3:]
+                                 if not x.startswith(CONSTRAINTS_PREFIX)]
+
+        self.constraints_keys = [x for x in self.header[3:]
+                                 if x.startswith(CONSTRAINTS_PREFIX)]
+
+        self.src_class   = self.header[1].split("@")[0]
+        self.src_key     = self.header[1].split("@")[1]
+        self.dst_class   = self.header[2].split("@")[0]
+        # Pandas appends a .n to the column name if there is a duplicate
+        self.dst_key     = self.header[2].split("@")[1].split(".")[0]
+        self.command     = "AddConnection"
+
+    def get_indices(self):
+        return {
+            "connection": {
+                cls: self.get_indexed_properties() for cls in self.df[CONNECTION_CLASS].unique()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
         src_value = self.df.loc[idx, self.header[1]]
         dst_value = self.df.loc[idx, self.header[2]]
         connection_class = self.df.loc[idx, CONNECTION_CLASS]
         q = []
```

### Comparing `aperturedb-0.4.3/aperturedb/Connector.py` & `aperturedb-0.4.4/aperturedb/Connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,29 @@
         str (password): Password to specify while connecting to the db.
         str (token): Token to use while connecting to the database.
         bool (use_ssl): Use SSL to encrypt communication with the database.
     """
 
     def __init__(self, host="localhost", port=55555,
                  user="", password="", token="",
-                 use_ssl=True, shared_data=None):
+                 use_ssl=True, shared_data=None, authenticate=True):
 
         self.host = host
         self.port = port
         self.use_ssl = use_ssl
         self.connected = False
         self.last_response   = ''
         self.last_query_time = 0
 
         self._connect()
 
+        if authenticate:
+            self.authenticate(shared_data, user, password, token)
+
+    def authenticate(self, shared_data, user, password, token):
         if shared_data is None:
             self.shared_data = SimpleNamespace()
             self.shared_data.session = None
             self.shared_data.lock = Lock()
             try:
                 self._authenticate(user, password, token)
             except Exception as e:
```

### Comparing `aperturedb-0.4.3/aperturedb/ConnectorRest.py` & `aperturedb-0.4.4/aperturedb/ConnectorRest.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,22 +76,31 @@
         int (port): Port to connect to.
         str (user): Username to specify while establishing a connection.
         str (password): Password to specify while connecting to the db.
         str (token): Token to use while connecting to the database.
         bool (use_ssl): Use SSL to encrypt communication with the database.
     """
 
-    def __init__(self, host="localhost", port=80,
+    def __init__(self, host="localhost", port=None,
                  user="", password="", token="",
                  use_ssl=True, shared_data=None):
 
         self.host = host
-        self.port = port
+
+        if port is None:
+            self.port = 443 if use_ssl else 80
+        else:
+            self.port = port
+
         self.use_ssl = use_ssl
         self.connected = False
+        # Session is useful because it does not add "Connection: close header"
+        # Since we will be making same call to the same URL, making a session
+        # REF: https://requests.readthedocs.io/en/latest/user/advanced/
+        self.http_session = requests.Session()
 
         self.last_response   = ''
         self.last_query_time = 0
 
         self.url = ('https' if self.use_ssl else 'http') + \
             '://' + host + ':' + str(port) + '/api/'
 
@@ -104,14 +113,15 @@
             except Exception as e:
                 raise Exception("Authentication failed:", str(e))
         else:
             self.shared_data = shared_data
 
     def __del__(self):
         logger.info("Done with connector")
+        self.http_session.close()
 
     def _query(self, query, blob_array = []):
         response_blob_array = []
         # Check the query type
         if not isinstance(query, str):  # assumes json
             query_str = json.dumps(query)
         else:
@@ -131,18 +141,18 @@
         else:
             headers = None
         tries = 0
         response = SimpleNamespace()
         response.status_code = 0
         while tries < 3:
             tries += 1
-            response = requests.post(self.url,
-                                     headers = headers,
-                                     files   = files,
-                                     verify  = self.use_ssl)
+            response = self.http_session.post(self.url,
+                                              headers = headers,
+                                              files   = files,
+                                              verify  = self.use_ssl)
             if response.status_code == 200:
                 # Parse response:
                 json_response       = json.loads(response.text)
                 import base64
                 response_blob_array = [base64.b64decode(
                     b) for b in json_response['blobs']]
                 self.last_response  = json_response["json"]
```

### Comparing `aperturedb-0.4.3/aperturedb/Constraints.py` & `aperturedb-0.4.4/aperturedb/Constraints.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/DaskManager.py` & `aperturedb-0.4.4/aperturedb/DaskManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,30 @@
 
 logger = logging.getLogger(__name__)
 
 
 class DaskManager:
     def __init__(self, num_workers: int = -1):
         self.__num_workers = num_workers
+        # The -1 magic number is to use as many 90% of the cores (1 worker per core).
+        # This can be overridden by the user.
+        # Create a pool of workers.
+        # TODO: see if the same pool can be reused for multiple tasks.
+        workers = self.__num_workers if self.__num_workers != \
+            -1 else int(0.9 * mp.cpu_count())
+
+        self._cluster = LocalCluster(n_workers=workers)
+        self._cluster.shutdown_on_close = False
+        self._client = Client(self._cluster)
+        dask.config.set(scheduler="distributed")
+
+    def __del__(self):
+        logger.info(".......Shutting cluster.........")
+        self._client.close()
+        self._cluster.close()
 
     def run(self, db: Connector, generator, batchsize, stats):
         def process(df, host, port, use_ssl, session, connnector_type):
             metrics = Stats()
             # Dask reads data in partitions, and the first partition is of 2 rows, with all
             # values as 'foo'. This is for sampling the column names and types. Should not process
             # those rows.
@@ -43,33 +59,29 @@
                 slice = df[i:end]
                 data = generator.__class__(filename="", df=slice)
                 loader.ingest(generator=data, batchsize=len(
                     slice), numthreads=1, stats=False)
                 count += 1
                 metrics.times_arr.extend(loader.times_arr)
                 metrics.error_counter += loader.error_counter
+                metrics.objects_existed += loader.get_objects_existed()
+                metrics.suceeded_queries += loader.get_suceeded_queries()
+                metrics.suceeded_commands += loader.get_suceeded_commands()
 
             return metrics
 
-        # The -1 magic number is to use as many 90% of the cores (1 worker per core).
-        # This can be overridden by the user.
-        # Create a pool of workers.
-        # TODO: see if the same pool can be reused for multiple tasks.
-        workers = self.__num_workers if self.__num_workers != \
-            -1 else int(0.9 * mp.cpu_count())
-        with LocalCluster(n_workers=workers) as cluster, Client(cluster) as client:
-            dask.config.set(scheduler="distributed")
-            start_time = time.time()
-            # Passing DB as an argument to function is not supported by Dask,
-            # so we pass session and host/port instead.
-            computation = generator.df.map_partitions(
-                process,
-                db.host,
-                db.port,
-                db.use_ssl,
-                db.shared_data.session,
-                type(db))
-            computation = computation.persist()
-            if stats:
-                progress(computation)
-            results = computation.compute()
+        start_time = time.time()
+        # Passing DB as an argument to function is not supported by Dask,
+        # so we pass session and host/port instead.
+        computation = generator.df.map_partitions(
+            process,
+            db.host,
+            db.port,
+            db.use_ssl,
+            db.shared_data.session,
+            type(db))
+        computation = computation.persist()
+        if stats:
+            progress(computation)
+        results = computation.compute()
+
         return results, time.time() - start_time
```

### Comparing `aperturedb-0.4.3/aperturedb/DescriptorDataCSV.py` & `aperturedb-0.4.4/aperturedb/DescriptorDataCSV.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,20 +69,27 @@
     """
 
     def __init__(self, filename, df=None, use_dask=False):
 
         super().__init__(filename, df=df, use_dask=use_dask)
         self.npy_arrays = {}
         self.has_label = False
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[3:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.constraints_keys = [x for x in self.header[3:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.command = "AddDescriptor"
+
+        self.props_keys       = [x for x in self.header[3:]
+                                 if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.constraints_keys = [x for x in self.header[3:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.command = "AddDescriptor"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                "_Descriptor": self.get_indexed_properties()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
         filename = self.df.loc[idx, HEADER_PATH]
         index    = self.df.loc[idx, HEADER_INDEX]
         desc_set = self.df.loc[idx, HEADER_SET]
```

### Comparing `aperturedb-0.4.3/aperturedb/DescriptorSetDataCSV.py` & `aperturedb-0.4.4/aperturedb/DescriptorSetDataCSV.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,20 +44,27 @@
         When performing a search on this set, FaissIVFFlat engine would be used and the metric to compute
         the distance would be L2.
     """
 
     def __init__(self, filename, df=None, use_dask=False):
 
         super().__init__(filename, df=df, use_dask=use_dask)
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[4:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.constraints_keys = [x for x in self.header[4:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.command = "AddDescriptorSet"
+
+        self.props_keys = [x for x in self.header[4:]
+                           if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.constraints_keys = [x for x in self.header[4:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.command = "AddDescriptorSet"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                "_DescriptorSet": self.get_indexed_properties()
+            }
+        }
 
     def getitem(self, idx):
 
         # Metrics/Engine can be of the form:
         #       "IP", or
         #       ["IP" ...]
         idx = self.df.index.start + idx
```

### Comparing `aperturedb-0.4.3/aperturedb/Entities.py` & `aperturedb-0.4.4/aperturedb/Entities.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/EntityDataCSV.py` & `aperturedb-0.4.4/aperturedb/EntityDataCSV.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,20 +37,27 @@
         id would be only inserted if it does not already exist in the database.
 
 
     """
 
     def __init__(self, filename, df=None, use_dask=False):
         super().__init__(filename, df=df, use_dask=use_dask)
-        if not use_dask:
-            self.props_keys       = [x for x in self.header[1:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.constraints_keys = [x for x in self.header[1:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.command = "AddEntity"
+
+        self.props_keys = [x for x in self.header[1:]
+                           if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.constraints_keys = [x for x in self.header[1:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.command = "AddEntity"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                cls: self.get_indexed_properties() for cls in self.df[ENTITY_CLASS].unique()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
         eclass = self.df.loc[idx, ENTITY_CLASS]
         q = []
         ae = self._basic_command(idx,
                                  custom_fields = {
```

### Comparing `aperturedb-0.4.3/aperturedb/ImageDataCSV.py` & `aperturedb-0.4.4/aperturedb/ImageDataCSV.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,34 +72,41 @@
                         self.load_s3_url, self.load_gs_url]
         self.source_types = [HEADER_PATH,
                              HEADER_URL, HEADER_S3_URL, HEADER_GS_URL]
 
         super().__init__(filename, df=df, use_dask=use_dask)
 
         self.check_image = check_image
-        if not use_dask:
-            self.format_given     = IMG_FORMAT in self.header
-            self.props_keys       = [x for x in self.header[1:]
-                                     if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-            self.props_keys       = [
-                x for x in self.props_keys if x != IMG_FORMAT]
-            self.constraints_keys = [x for x in self.header[1:]
-                                     if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
-
-            self.source_type      = self.header[0]
-
-            if self.source_type not in self.source_types:
-                logger.error("Source not recognized: " + self.source_type)
-                raise Exception("Error loading image: " + filename)
-            self.source_loader    = {
-                st: sl for st, sl in zip(self.source_types, self.loaders)
-            }
 
-            self.n_download_retries = n_download_retries
-            self.command = "AddImage"
+        self.format_given     = IMG_FORMAT in self.header
+        self.props_keys       = [x for x in self.header[1:]
+                                 if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+        self.props_keys       = [
+            x for x in self.props_keys if x != IMG_FORMAT]
+        self.constraints_keys = [x for x in self.header[1:]
+                                 if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
+
+        self.source_type      = self.header[0]
+
+        if self.source_type not in self.source_types:
+            logger.error("Source not recognized: " + self.source_type)
+            raise Exception("Error loading image: " + filename)
+        self.source_loader    = {
+            st: sl for st, sl in zip(self.source_types, self.loaders)
+        }
+
+        self.n_download_retries = n_download_retries
+        self.command = "AddImage"
+
+    def get_indices(self):
+        return {
+            "entity": {
+                "_Image": self.get_indexed_properties()
+            }
+        }
 
     def getitem(self, idx):
         idx = self.df.index.start + idx
         image_path = self.df.loc[idx, self.source_type]
         img_ok, img = self.source_loader[self.source_type](image_path)
 
         if not img_ok:
```

### Comparing `aperturedb-0.4.3/aperturedb/ImageDownloader.py` & `aperturedb-0.4.4/aperturedb/ImageDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Images.py` & `aperturedb-0.4.4/aperturedb/Images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/KaggleData.py` & `aperturedb-0.4.4/aperturedb/KaggleData.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/NotebookHelpers.py` & `aperturedb-0.4.4/aperturedb/NotebookHelpers.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Operations.py` & `aperturedb-0.4.4/aperturedb/Operations.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/ParallelQuery.py` & `aperturedb-0.4.4/aperturedb/ParallelQuery.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from aperturedb.DaskManager import DaskManager
 
 
 logger = logging.getLogger(__name__)
 
 
-def execute_batch(q, blobs, db,
+def execute_batch(q, blobs, db, success_statuses: list[int] = [0],
                   response_handler: Callable = None, commands_per_query: int = 1, blobs_per_query: int = 0):
     """
     Execute a batch of queries, doing useful logging around it.
     Calls the response handler if provided.
     This should be used (without the parallel machinery) istead of db.query to keep the
     response handling consistent, better logging, etc.
 
@@ -65,53 +65,82 @@
                 except BaseException as e:
                     logger.exception(e)
                 blobs_returned += b_count
     else:
         # Transaction failed entirely.
         logger.error(f"Failed query = {q} with response = {r}")
         result = 1
-    if isinstance(r, dict) and db.last_response['status'] != 0:
-        logger.error(f"Failed query = {q} with response = {r}")
+
+    statuses = {}
+    if isinstance(r, dict):
+        statuses[r['status']] = [r]
+    elif isinstance(r, list):
+        # add each result to a list of the responses, keyed by the response
+        # code.
+        [statuses.setdefault(result[cmd]['status'], []).append(result)
+         for result in r for cmd in result]
+    else:
+        logger.error("Response in unexpected format")
         result = 1
-    if isinstance(r, list) and not all([v['status'] == 0 for i in r for k, v in i.items()]):
-        logger.warning(
-            f"Partial errors:\r\n{json.dumps(q)}\r\n{json.dumps(r)}")
-        result = 2
+
+    # last_query_ok means result status >= 0
+    if result != 1:
+        warn_list = []
+        for status, results in statuses.items():
+            if status not in success_statuses:
+                for wr in results:
+                    warn_list.append(wr)
+        if len(warn_list) != 0:
+            logger.warning(
+                f"Partial errors:\r\n{json.dumps(q)}\r\n{json.dumps(warn_list)}")
+            result = 2
 
     return result, r, b
 
 
 class ParallelQuery(Parallelizer.Parallelizer):
     """
     **Parallel and Batch Querier for ApertureDB**
     This class provides the abstraction for partitioning data into batches,
     so that they may be processed using different threads.
     """
 
+    # 0 is success, 2 is object exists
+    success_statuses = [0, 2]
+
+    @classmethod
+    def setSuccessStatus(cls, statuses: list[int]):
+        cls.success_statuses = statuses
+
+    @classmethod
+    def getSuccessStatus(cls):
+        return cls.success_statuses
+
     def __init__(self, db, dry_run=False):
 
         super().__init__()
 
         self.db = db.create_new_connection()
 
         self.dry_run = dry_run
 
         self.type = "query"
 
         self.responses = []
 
         self.commands_per_query = 1
         self.blobs_per_query = 0
+        self.daskManager = None
 
     def generate_batch(self, data):
         """
             Here we flatten the individual queries to run them as
             a single query in a batch
         """
-        q     = [cmd for query in data for cmd in query[0]]
+        q = [cmd for query in data for cmd in query[0]]
         blobs = [blob for query in data for blob in query[1]]
 
         return q, blobs
 
     def call_response_handler(self, q, blobs, r, b):
         try:
             self.generator.response_handler(q, blobs, r, b)
@@ -144,26 +173,31 @@
         query_time = 0
         worker_stats = {}
         if not self.dry_run:
             response_handler = None
             if hasattr(self.generator, "response_handler") and callable(self.generator.response_handler):
                 response_handler = self.generator.response_handler
             result, r, b = execute_batch(
-                q, blobs, db, response_handler, self.commands_per_query, self.blobs_per_query)
+                q, blobs, db, ParallelQuery.success_statuses, response_handler, self.commands_per_query, self.blobs_per_query)
             if result == 0:
                 query_time = db.get_last_query_time()
                 worker_stats["suceeded_commands"] = len(q)
                 worker_stats["suceeded_queries"] = len(data)
+                worker_stats["objects_existed"] = sum(
+                    [v['status'] == 2 for i in r for k, v in i.items()])
             elif result == 1:
                 self.error_counter += 1
                 worker_stats["suceeded_queries"] = 0
                 worker_stats["suceeded_commands"] = 0
+                worker_stats["objects_existed"] = 0
             elif result == 2:
                 worker_stats["suceeded_commands"] = sum(
                     [v['status'] == 0 for i in r for k, v in i.items()])
+                worker_stats["objects_existed"] = sum(
+                    [v['status'] == 2 for i in r for k, v in i.items()])
                 sq = 0
                 for i in range(0, len(r), self.commands_per_query):
                     if all([v['status'] == 0 for j in r[i:i + self.commands_per_query] for k, v in j.items()]):
                         sq += 1
                 worker_stats["suceeded_queries"] = sq
         else:
             query_time = 1
@@ -180,15 +214,15 @@
 
         if (end - start) % self.batchsize > 0:
             total_batches += 1
 
         for i in range(total_batches):
 
             batch_start = start + i * self.batchsize
-            batch_end   = min(batch_start + self.batchsize, end)
+            batch_end = min(batch_start + self.batchsize, end)
 
             try:
                 self.do_batch(db, generator[batch_start:batch_end])
             except Exception as e:
                 logger.exception(e)
                 self.error_counter += 1
 
@@ -202,24 +236,34 @@
         Args:
             generator (_type_): The class that generates the queries to be executed.
             batchsize (int, optional): Nummber of queries per transaction. Defaults to 1.
             numthreads (int, optional): Number of parallel workers. Defaults to 4.
             stats (bool, optional): Show statistics at end of ingestion. Defaults to False.
         """
 
-        if hasattr(generator, "use_dask") and generator.use_dask:
+        use_dask = hasattr(generator, "use_dask") and generator.use_dask
+        if use_dask:
             self._reset(batchsize=batchsize, numthreads=numthreads)
-            daskmanager = DaskManager(num_workers=numthreads)
+            self.daskmanager = DaskManager(num_workers=numthreads)
+
+        if hasattr(self, "query_setup"):
+            self.query_setup(generator)
 
-            results, self.total_actions_time = daskmanager.run(
+        if use_dask:
+            results, self.total_actions_time = self.daskmanager.run(
                 self.db, generator, batchsize, stats=stats)
+            self.actual_stats = []
             for result in results:
                 if result is not None:
                     self.times_arr.extend(result.times_arr)
                     self.error_counter += result.error_counter
+                    self.actual_stats.append(
+                        {"suceeded_queries": result.suceeded_queries,
+                         "suceeded_commands": result.suceeded_commands,
+                         "objects_existed": result.objects_existed})
             self.total_actions = len(generator.df)
 
             if stats:
                 self.print_stats()
         else:
             if len(generator) > 0:
                 if isinstance(generator[0], tuple) and isinstance(generator[0][0], list):
@@ -249,15 +293,15 @@
         print(f"Total queries executed: {total_queries_exec}")
 
         if total_queries_exec == 0:
             print("All queries failed!")
 
         else:
             mean = np.mean(times)
-            std  = np.std(times)
+            std = np.std(times)
             tp = 1 / mean * self.numthreads
 
             print(f"Avg Query time (s): {mean}")
             print(f"Query time std: {std}")
             print(f"Avg Query Throughput (q/s): {tp}")
 
             i_tp = self.total_actions / self.total_actions_time
```

### Comparing `aperturedb-0.4.3/aperturedb/Parallelizer.py` & `aperturedb-0.4.4/aperturedb/Parallelizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
                                 args=(i, generator, idx_start, idx_end))
             thread_arr.append(thread_add)
 
         a = [th.start() for th in thread_arr]
         a = [th.join() for th in thread_arr]
 
         # Update progress bar to completion
-        self.pb.update(1)
+        if self.stats:
+            self.pb.update(1)
 
         self.total_actions_time = time.time() - start_time
 
         if self.stats:
             self.print_stats()
 
     def print_stats(self):
```

### Comparing `aperturedb-0.4.3/aperturedb/PolygonDataCSV.py` & `aperturedb-0.4.4/aperturedb/PolygonDataCSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,21 @@
                 self.constraints_keys.append(key)
             else:
                 self.props_keys.append(key)
 
         self.img_key = self.header[0]
         self.command = "AddPolygon"
 
+    def get_indices(self):
+        return {
+            "entity": {
+                "_Polygon": self.get_indexed_properties()
+            }
+        }
+
     def getitem(self, idx):
         idx = self.df.index.start + idx
 
         q = []
 
         img_id = self.df.loc[idx, self.img_key]
```

### Comparing `aperturedb-0.4.3/aperturedb/Polygons.py` & `aperturedb-0.4.4/aperturedb/Polygons.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/ProgressBar.py` & `aperturedb-0.4.4/aperturedb/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/PyTorchDataset.py` & `aperturedb-0.4.4/aperturedb/PyTorchDataset.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/PytorchData.py` & `aperturedb-0.4.4/aperturedb/PytorchData.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Query.py` & `aperturedb-0.4.4/aperturedb/Query.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/QueryTypes.py` & `aperturedb-0.4.4/aperturedb/QueryTypes.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Subscriptable.py` & `aperturedb-0.4.4/aperturedb/Subscriptable.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Utils.py` & `aperturedb-0.4.4/aperturedb/Utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from calendar import c
 import logging
 import json
 
 from aperturedb.Connector import Connector
 from aperturedb import ProgressBar
+from aperturedb.ParallelQuery import execute_batch
 
 logger = logging.getLogger(__name__)
 
 DESCRIPTOR_CLASS = "_Descriptor"
 DESCRIPTOR_CONNECTION_CLASS = "_DescriptorSetToDescriptor"
 
 DEFAULT_METADATA_BATCH_SIZE = 100_000
@@ -30,24 +32,33 @@
         return self.status()
 
     def print(self, str):
 
         if self.verbose:
             print(str)
 
-    def status(self):
-
-        q = [{"GetStatus": {}}]
-
+    def execute(self, query, blobs=[], success_statuses=[0]):
         try:
-            res, blobs = self.connector.query(q)
+            rc, r, b = execute_batch(
+                query, blobs, self.connector, success_statuses=success_statuses)
         except BaseException as e:
             logger.error(self.connector.get_last_response_str())
             raise e
 
+        if rc != 0:
+            raise Exception("query failed with result {rc}")
+
+        return r, b
+
+    def status(self):
+
+        q = [{"GetStatus": {}}]
+
+        self.execute(q)
+
         return self.connector.get_last_response_str()
 
     def print_schema(self, refresh=False):
 
         if refresh:
             logger.warning("get_schema: refresh no longer needed.")
             logger.warning("get_schema: refresh will be deprecated.")
@@ -166,20 +177,16 @@
                 "index_type":    index_type,
                 "class":         class_name,
                 "property_key":  property_key,
             }
         }]
 
         try:
-            res, blobs = self.connector.query(q)
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
-                return False
+            self.execute(q, success_statuses=[0, 2])
         except:
-            logger.error(self.connector.get_last_response_str())
             return False
 
         return True
 
     def _remove_index(self, index_type, class_name, property_key):
 
         q = [{
@@ -187,20 +194,16 @@
                 "index_type":   index_type,
                 "class":        class_name,
                 "property_key": property_key,
             }
         }]
 
         try:
-            res, blobs = self.connector.query(q)
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
-                return False
+            self.execute(q)
         except:
-            logger.error(self.connector.get_last_response_str())
             return False
 
         return True
 
     def create_entity_index(self, class_name, property_key, property_type=None):
 
         if property_type is not None:
@@ -237,20 +240,16 @@
                 }
             }
         }]
 
         if constraints:
             q[0]["FindImage"]["constraints"] = constraints
 
-        try:
-            res, blobs = self.connector.query(q)
-            total_images = res[0]["FindImage"]["count"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total_images = res[0]["FindImage"]["count"]
 
         return total_images
 
     def get_uniqueids(self, object_type, constraints={}):
 
         q = [{
             "FindEntity": {
@@ -263,20 +262,16 @@
         }]
 
         if constraints:
             q[0]["FindEntity"]["constraints"] = constraints
 
         ids = []
 
-        try:
-            res, blobs = self.connector.query(q)
-            total_elements = res[0]["FindEntity"]["batch"]["total_elements"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total_elements = res[0]["FindEntity"]["batch"]["total_elements"]
 
         batch_size = DEFAULT_METADATA_BATCH_SIZE
         iterations = total_elements // batch_size
         reminder   = total_elements % batch_size
 
         if iterations == 0 and reminder > 0:
             iterations = 1
@@ -288,21 +283,17 @@
             batch = {
                 "batch_size": batch_size,
                 "batch_id": i
             }
 
             q[0]["FindEntity"]["batch"] = batch
 
-            try:
-                res, blobs = self.connector.query(q)
-                ids += [element["_uniqueid"]
-                        for element in res[0]["FindEntity"]["entities"]]
-            except BaseException as e:
-                logger.error(self.connector.get_last_response_str())
-                raise e
+            res, _ = self.execute(q)
+            ids += [element["_uniqueid"]
+                    for element in res[0]["FindEntity"]["entities"]]
 
             if self.verbose:
                 pb.update(i / iterations)
 
         if self.verbose:
             pb.update(1)  # For the end of line
 
@@ -324,20 +315,16 @@
                 }
             }
         }]
 
         if constraints:
             q[0]["FindBoundingBox"]["constraints"] = constraints
 
-        try:
-            res, blobs = self.connector.query(q)
-            total_connections = res[0]["FindBoundingBox"]["count"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total_connections = res[0]["FindBoundingBox"]["count"]
 
         return total_connections
 
     def count_entities(self, entity_class, constraints=None):
 
         q = [{
             "FindEntity": {
@@ -347,31 +334,16 @@
                 }
             }
         }]
 
         if constraints:
             q[0]["FindEntity"]["constraints"] = constraints
 
-        try:
-            res, blobs = self.connector.query(q)
-            fe = res[0]["FindEntity"]
-
-            if fe["status"] == 1:
-                # TODO: Here we return 0 entities because the query failed.
-                # This is because Find* Command will return status: 1
-                # and no count if no object is found.
-                # We should change the Find* Command to return status: 0
-                # and count: 0 if no object is found.
-                total_entities = 0
-            else:
-                total_entities = fe["count"]
-
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total_entities = res[0]["FindEntity"]["count"]
 
         return total_entities
 
     def count_connections(self, connections_class, constraints=None):
 
         q = [{
             "FindConnection": {
@@ -381,64 +353,49 @@
                 }
             }
         }]
 
         if constraints:
             q[0]["FindConnection"]["constraints"] = constraints
 
-        try:
-            res, blobs = self.connector.query(q)
-            total_connections = res[0]["FindConnection"]["count"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total_connections = res[0]["FindConnection"]["count"]
 
         return total_connections
 
     def add_descriptorset(self, name, dim, metric="L2", engine="FaissFlat"):
 
         query = [{
             "AddDescriptorSet": {
                 "name":       name,
                 "dimensions": dim,
                 "metric":     metric,
                 "engine":     engine
             }
         }]
 
-        response, arr = self.connector.query(query)
-
-        expected = [{
-            "AddDescriptorSet": {
-                "status": 0,
-            }
-        }]
-
-        if response != expected:
-            logger.error(self.connector.get_last_response_str())
+        try:
+            self.execute(query)
+        except:
             return False
 
         return True
 
     def count_descriptorsets(self):
 
         q = [{
             "FindDescriptorSet": {
                 "results": {
                     "count": True,
                 }
             }
         }]
 
-        try:
-            res, blobs = self.connector.query(q)
-            total_descriptor_sets = res[0]["FindDescriptorSet"]["count"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.query(q)
+        total_descriptor_sets = res[0]["FindDescriptorSet"]["count"]
 
         return total_descriptor_sets
 
     def get_descriptorset_list(self):
 
         q = [{
             "FindDescriptorSet": {
@@ -446,22 +403,18 @@
                     "list": ["_name"],
                 }
 
             }
         }]
 
         sets = []
-        try:
-            res, _ = self.connector.query(q)
-
+        res, _ = self.execute(q)
+        if res[0]["FindDescriptorSet"]["returned"] > 0:
             sets = [ent["_name"]
                     for ent in res[0]["FindDescriptorSet"]["entities"]]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
 
         return sets
 
     def remove_descriptorset(self, set_name):
 
         q = [{
             "FindDescriptorSet": {
@@ -472,20 +425,16 @@
         }, {
             "DeleteDescriptorSet": {
                 "ref": 1
             }
         }]
 
         try:
-            res, _ = self.connector.query(q)
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
-                return False
+            self.execute(q)
         except:
-            logger.error(self.connector.get_last_response_str())
             return False
 
         return True
 
     def _remove_objects(self, type, class_name, batch_size):
 
         if type == "entities":
@@ -515,18 +464,17 @@
                 }
             }, {
                 dele: {
                     "ref": 1
                 }
             }]
 
-            res, _ = self.connector.query(q)
-
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
+            try:
+                self.execute(q)
+            except:
                 return False
 
             self.print(
                 f"Delete transaction of {batch_size} elements took: {self.connector.get_last_query_time()}")
 
             count -= batch_size
 
@@ -545,21 +493,16 @@
 
         query = [{
             "DeleteEntity": {
                 "with_class": class_name
             }
         }]
 
-        r, _ = self.connector.query(query)
-
-        if not self.connector.last_query_ok():
-            logger.error(self.connector.get_last_response_str())
-            return False
-
         try:
+            r, _ = self.execute(query)
             count = r[0]["DeleteEntity"]["count"]
             self.print(f"Deleted {count} entities")
             self.print(
                 f"Delete transaction took: {self.connector.get_last_query_time()}")
         except:
             logger.error("Could not get count of deleted entities")
             return False
@@ -576,21 +519,16 @@
 
         query = [{
             "DeleteConnection": {
                 "with_class": class_name
             }
         }]
 
-        r, _ = self.connector.query(query)
-
-        if not self.connector.last_query_ok():
-            logger.error(self.connector.get_last_response_str())
-            return False
-
         try:
+            r, _ = self.execute(query)
             count = r[0]["DeleteConnection"]["count"]
             self.print(f"Deleted {count} connections")
             self.print(
                 f"Delete transaction took: {self.connector.get_last_query_time()}")
         except:
             logger.error("Could not get count of deleted connections")
             return False
@@ -666,23 +604,16 @@
                 },
                 "results": {
                     "count": True
                 }
             }
         }]
 
-        try:
-            res, _ = self.connector.query(q)
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
-            else:
-                total = res[1]["FindDescriptor"]["count"]
-        except BaseException as e:
-            logger.error(self.connector.get_last_response_str())
-            raise e
+        res, _ = self.execute(q)
+        total = res[1]["FindDescriptor"]["count"]
 
         return total
 
     def remove_all_objects(self):
 
         cmd = {"constraints": {"_uniqueid": ["!=", "0.0.0"]}}
 
@@ -699,36 +630,30 @@
             # We keep them here until ApertureDB fully implements this.
             [{"DeleteBoundingBox": cmd}],
             [{"DeletePolygon": cmd}],
             [{"DeleteFrame": cmd}],
         ]
 
         try:
-            for q in queries:
-                response, _ = self.connector.query(q)
-                if not self.connector.last_query_ok():
-                    logger.error(self.connector.get_last_response_str())
-                    return False
-
-            response, _ = self.connector.query(
-                [{"GetSchema": {"refresh": True}}])
-
-            if not self.connector.last_query_ok():
-                logger.error(self.connector.get_last_response_str())
+            try:
+                for q in queries:
+                    self.execute(q)
+                response, _ = self.execute(
+                    [{"GetSchema": {"refresh": True}}])
+            except:
                 return False
 
-            entities    = response[0]["GetSchema"]["entities"]
-            connections = response[0]["GetSchema"]["connections"]
+            schema = response[0]["GetSchema"]
 
-            if entities is not None:
+            if "entities" in schema and schema["entities"] is not None:
                 logger.error("Entities not removed completely")
                 logger.error(self.connector.get_last_response_str())
                 return False
 
-            if connections is not None:
+            if "connections" in schema and schema["connections"] is not None:
                 logger.error("Connections not removed completely")
                 logger.error(self.connector.get_last_response_str())
                 return False
 
         except BaseException as e:
             logger.error(self.connector.get_last_response_str())
             raise e
```

### Comparing `aperturedb-0.4.3/aperturedb/VideoDataCSV.py` & `aperturedb-0.4.4/aperturedb/VideoDataCSV.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 
         self.props_keys       = [x for x in self.header[1:]
                                  if not x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
         self.constraints_keys = [x for x in self.header[1:]
                                  if x.startswith(CSVParser.CONSTRAINTS_PREFIX)]
         self.command = "AddVideo"
 
+    def get_indices(self):
+        return {
+            "entity": {
+                "_Video": self.get_indexed_properties()
+            }
+        }
+
     def getitem(self, idx):
         filename   = self.df.loc[idx, HEADER_PATH]
         video_ok, video = self.load_video(filename)
 
         if not video_ok:
             logger.error("Error loading video: " + filename)
             raise Exception("Error loading video: " + filename)
```

### Comparing `aperturedb-0.4.3/aperturedb/VideoDownloader.py` & `aperturedb-0.4.4/aperturedb/VideoDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/Videos.py` & `aperturedb-0.4.4/aperturedb/Videos.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb/__init__.py` & `aperturedb-0.4.4/aperturedb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import os
 import json
 import requests
 
 logger = logging.getLogger(__name__)
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 # set log level
 logger.setLevel(logging.DEBUG)
 formatter    = logging.Formatter(
     "%(asctime)s : %(levelname)s : %(name)s : %(thread)d : %(lineno)d : %(message)s")
 
 log_file_level = logging.getLevelName(os.getenv("LOG_FILE_LEVEL", "WARN"))
```

### Comparing `aperturedb-0.4.3/aperturedb/queryMessage_pb2.py` & `aperturedb-0.4.4/aperturedb/queryMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/aperturedb.egg-info/PKG-INFO` & `aperturedb-0.4.4/aperturedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.3
+Version: 0.4.4
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.3/aperturedb.egg-info/SOURCES.txt` & `aperturedb-0.4.4/aperturedb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,11 @@
 test/download_images.py
 test/generateInput.py
 test/test_Data.py
 test/test_Datawizard.py
 test/test_ResponseHandler.py
 test/test_Session.py
 test/test_Stats.py
+test/test_Success.py
 test/test_Utils.py
 test/test_kaggle.py
 test/test_torch_connector.py
```

### Comparing `aperturedb-0.4.3/setup.py` & `aperturedb-0.4.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 OPENCV_VERSION = os.getenv("OPENCV_VERSION")
 
 install_requires = ['scikit-image', 'image', 'requests', 'boto3',
                     'numpy', 'matplotlib', 'pandas', 'kaggle', 'google-cloud-storage',
-                    'dask[complete]<=2023.1.0', 'ipywidgets', 'pydantic', 'devtools',
-                    # Pinning this to be able to install tensorflow.
-                    'protobuf<3.20.0',
+                    'dask[complete]', 'ipywidgets', 'pydantic', 'devtools',
+                    # Pin to the bridge version.
+                    # https://github.com/tensorflow/tensorflow/issues/60320
+                    'protobuf==3.20.3',
                     # Pinning this to be able to install google-cloud-bigquery
-                    'grpcio-status==1.48.2'
+                    'grpcio-status==1.48.2',
+                    # Pinning this to resolve test errors temporarily
+                    'ipywidgets==8.0.4'
                     ]
 if OPENCV_VERSION is None:
     install_requires.append('opencv-python')
 
 setuptools.setup(
     name="aperturedb",
-    version="0.4.3",
+    version="0.4.4",
     description="ApertureDB Client Module",
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aperture-data/aperturedb-python",
     license="Apache",
     packages=setuptools.find_packages(),
```

### Comparing `aperturedb-0.4.3/test/download_images.py` & `aperturedb-0.4.4/test/download_images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/test/generateInput.py` & `aperturedb-0.4.4/test/generateInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,24 @@
     df["dimensions"] = dims
     df["engine"]     = [random.sample(engines, 1)[0] for i in names]
     df["metric"]     = [random.sample(metrics, 1)[0] for i in names]
 
     df.to_csv("input/descriptorset.adb.csv", index=False)
 
 
+def generate_partial_load():
+
+    df = pd.read_csv("input/persons.adb.csv")
+    base = df.head(10)
+    base.to_csv("input/persons-exist-base.adb.csv", index=False)
+    # causes 3 overlaps
+    overlapped = df.head(12).tail(5)
+    overlapped.to_csv("input/persons-some-exist.adb.csv", index=False)
+
+
 def main(params):
 
     persons = generate_person_csv(params.multiplier)
     blobs   = generate_blobs_csv()
     images  = generate_images_csv(int(params.multiplier / 2))
     s3_imgs = generate_http_images_csv("input/sample_http_urls.csv")
     s3_imgs = generate_s3_images_csv("input/sample_s3_urls.csv")
@@ -312,14 +322,16 @@
 
     desc_name = ["setA", "setB", "setC", "setD", "setE", "setF"]
     desc_dims = [2048, 1025, 2048, 1025, 2048, 1025]    # yes, 1025
     generate_descriptorset(desc_name, desc_dims)
     for name, dims in zip(desc_name, desc_dims):
         generate_descriptors(images, name, dims)
 
+    generate_partial_load()
+
 
 def get_args():
     obj = argparse.ArgumentParser()
 
     # Run Config
     obj.add_argument('-multiplier', type=int, default=10)
```

### Comparing `aperturedb-0.4.3/test/test_Data.py` & `aperturedb-0.4.4/test/test_Data.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,62 +20,62 @@
         self.assertTrue(utils.remove_all_objects())
 
         results = [utils.create_entity_index(
             e, "id") for e in classes]
         self.assertTrue(all(results))
 
         # Insert Person Nodes
-        data = insert_data_from_csv("./input/persons.adb.csv")
+        data, _ = insert_data_from_csv("./input/persons.adb.csv")
         self.assertEqual(len(data), utils.count_entities("Person"))
 
         # Insert Images
-        data = insert_data_from_csv(in_csv_file = "./input/images.adb.csv")
+        data, _ = insert_data_from_csv(in_csv_file = "./input/images.adb.csv")
         self.assertEqual(len(data), utils.count_images())
 
         # Insert Connections
-        data = insert_data_from_csv(
+        data, _ = insert_data_from_csv(
             in_csv_file = "./input/connections-persons-images.adb.csv")
         self.assertEqual(
             len(data), utils.count_connections("has_image"))
 
         # Insert BBoxes
-        data = insert_data_from_csv(in_csv_file="./input/bboxes.adb.csv")
+        data, _ = insert_data_from_csv(in_csv_file="./input/bboxes.adb.csv")
         self.assertEqual(len(data), utils.count_bboxes())
 
     def test_LoaderDescriptorsImages(self, utils, insert_data_from_csv):
         self.assertTrue(utils.remove_all_objects())
 
         # Insert Images, images may be there already, and that case should
         # be handled correctly by contraints
-        data = insert_data_from_csv(in_csv_file = "./input/images.adb.csv")
+        data, _ = insert_data_from_csv(in_csv_file = "./input/images.adb.csv")
         self.assertEqual(len(data), utils.count_images())
 
         # Insert DescriptorsSet
-        data = insert_data_from_csv(
+        data, _ = insert_data_from_csv(
             in_csv_file = "./input/descriptorset.adb.csv")
         self.assertEqual(len(data), utils.count_entities("_DescriptorSet"))
 
         # Insert Descriptors
 
         sets = ["setA", "setB"]
 
         total_descriptors = 0
         for setname in sets:
-            data = insert_data_from_csv(
+            data, _ = insert_data_from_csv(
                 in_csv_file = "./input/" + setname + ".adb.csv")
 
             total_descriptors += len(data)
             self.assertEqual(total_descriptors,
                              utils.count_entities("_Descriptor"))
 
     def test_BlobLoader(self, db, utils, insert_data_from_csv):
         # Assert that we have a clean slate to begin with.
         self.assertTrue(utils.remove_all_objects())
 
-        data = insert_data_from_csv(in_csv_file = "./input/blobs.adb.csv")
+        data, _ = insert_data_from_csv(in_csv_file = "./input/blobs.adb.csv")
         self.assertEqual(len(data), utils.count_entities("_Blob"))
 
         query = [{
             "FindBlob": {
                 "blobs": True,
                 "results": {
                     "list": ["license"],
@@ -90,41 +90,43 @@
         arr = np.frombuffer(blob[0])
         self.assertEqual(arr[2], 3.3)
 
     def test_conditional_add(self, utils, insert_data_from_csv):
         logger.debug(f"Cleaning existing data")
         self.assertTrue(utils.remove_all_objects())
         # insert one of the images from image csv, for bboxes to refer to.
-        images = insert_data_from_csv(
+        images, _ = insert_data_from_csv(
             in_csv_file="./input/images.adb.csv", rec_count=1)
         self.assertEqual(len(images), 1)
 
         # Insert BBoxes with repeated entries.
         # There is just one unique entry in the input csv.
         logger.debug(f"Inserting bounding box data")
-        boxes = insert_data_from_csv(
+        boxes, _ = insert_data_from_csv(
             in_csv_file="./input/bboxes-constraints.adb.csv")
         self.assertEqual(3, len(boxes))
         self.assertEqual(1, utils.count_bboxes())
 
 
 class TestURILoader():
     def assertEqual(self, expected, actual):
         if expected != actual:
             raise AssertionError(
                 "Expected {}, got {}".format(expected, actual))
 
     def test_S3Loader(self, utils, insert_data_from_csv):
         self.assertEqual(utils.remove_all_objects(), True)
-        data = insert_data_from_csv(in_csv_file = "./input/s3_images.adb.csv")
+        data, _ = insert_data_from_csv(
+            in_csv_file = "./input/s3_images.adb.csv")
         self.assertEqual(len(data), utils.count_images())
 
     def test_HttpImageLoader(self, utils, insert_data_from_csv):
         self.assertEqual(utils.remove_all_objects(), True)
-        data = insert_data_from_csv(
+        data, _ = insert_data_from_csv(
             in_csv_file = "./input/http_images.adb.csv")
         self.assertEqual(len(data), utils.count_images())
 
     def test_GSImageLoader(self, utils, insert_data_from_csv):
         self.assertEqual(utils.remove_all_objects(), True)
-        data = insert_data_from_csv(in_csv_file = "./input/gs_images.adb.csv")
+        data, _ = insert_data_from_csv(
+            in_csv_file = "./input/gs_images.adb.csv")
         self.assertEqual(len(data), utils.count_images())
```

### Comparing `aperturedb-0.4.3/test/test_Datawizard.py` & `aperturedb-0.4.4/test/test_Datawizard.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from devtools import debug
 
 logger = logging.getLogger(__file__)
 
 
 class TestDataWizardEntities():
     def test_get_persons(self, insert_data_from_csv, db):
-        loaded = insert_data_from_csv(in_csv_file="./input/persons.adb.csv")
+        loaded, _ = insert_data_from_csv(in_csv_file="./input/persons.adb.csv")
         all_persons = Entities.retrieve(db,
                                         spec=Query.spec(with_class="Person"))
         assert len(all_persons) == len(loaded)
         too_young = all_persons.filter(lambda p: p["age"] < 18)
         too_old = all_persons.filter(lambda p: p["age"] > 60)
         working_people = all_persons - too_old - too_young
 
@@ -58,38 +58,41 @@
 
         assert len(persons) == len(retired_persons)
         assert all(p["risk_factor"] == (p["age"] - 60) // 10 for p in persons)
 
 
 class TestDataWizardImages():
     def test_get_images(self, insert_data_from_csv, db):
-        loaded = insert_data_from_csv("./input/images.adb.csv", rec_count=10)
+        loaded, _ = insert_data_from_csv(
+            "./input/images.adb.csv", rec_count=10)
         images = Images.retrieve(db, Query.spec(limit=10))
         assert isinstance(
             images, Images), f"{type(images)} is not an instance of Images"
         logger.info(f"\n{images.inspect()}")
         assert images != None
         assert len(images) <= 10
 
 
 class TestDataWizardBlobs():
     def test_get_blobs(self, insert_data_from_csv, db):
-        loaded = insert_data_from_csv("./input/blobs.adb.csv", rec_count=10)
+        loaded, _ = insert_data_from_csv("./input/blobs.adb.csv", rec_count=10)
         blobs = Blobs.retrieve(db, Query.spec(limit=10))
         assert isinstance(
             blobs, Blobs), f"blobs is not an instance of Blobs = {blobs}"
         logger.info(f"\n{blobs.inspect()}")
         assert blobs != None
         assert len(blobs) <= 10
 
 
 class TestDataWizardBoundingBoxes():
     def test_get_bounding_boxes(self, insert_data_from_csv, db):
-        loaded = insert_data_from_csv("./input/images.adb.csv", rec_count=10)
-        loaded = insert_data_from_csv("./input/bboxes.adb.csv", rec_count=10)
+        loaded, _ = insert_data_from_csv(
+            "./input/images.adb.csv", rec_count=10)
+        loaded, _ = insert_data_from_csv(
+            "./input/bboxes.adb.csv", rec_count=10)
         bboxes = BoundingBoxes.retrieve(db, Query.spec(limit=10))
         assert isinstance(
             bboxes, BoundingBoxes), f"bboxes is not an instance of BoundingBoxes = {bboxes}"
         logger.info(f"\n{bboxes.inspect()}")
         assert bboxes != None
         assert len(bboxes) <= 10
```

### Comparing `aperturedb-0.4.3/test/test_ResponseHandler.py` & `aperturedb-0.4.4/test/test_ResponseHandler.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/test/test_Session.py` & `aperturedb-0.4.4/test/test_Session.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/test/test_Stats.py` & `aperturedb-0.4.4/test/test_Stats.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/test/test_kaggle.py` & `aperturedb-0.4.4/test/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.3/test/test_torch_connector.py` & `aperturedb-0.4.4/test/test_torch_connector.py`

 * *Files identical despite different names*

