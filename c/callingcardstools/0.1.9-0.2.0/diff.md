# Comparing `tmp/callingcardstools-0.1.9.tar.gz` & `tmp/callingcardstools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.9.tar", max compression
+gzip compressed data, was "callingcardstools-0.2.0.tar", max compression
```

## Comparing `callingcardstools-0.1.9.tar` & `callingcardstools-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.9/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.9/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.9/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.9/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.9/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0    12786 2023-05-19 17:42:53.279362 callingcardstools-0.1.9/callingcardstools/Alignment/mammals/Qbed.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.9/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     4252 2023-05-19 18:02:51.599306 callingcardstools-0.1.9/callingcardstools/Alignment/mammals/combine_qc.py
--rw-r--r--   0        0        0     9963 2023-05-19 22:48:19.506163 callingcardstools-0.1.9/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.9/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.9/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.9/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.9/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.9/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.9/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.1.9/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
--rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.1.9/callingcardstools/BarcodeParser/mammals/__init__.py
--rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.1.9/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.9/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.9/callingcardstools/BarcodeParser/yeast/combine_qc.py
--rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.9/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.9/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.9/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.9/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.9/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.9/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.9/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.9/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.1.9/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.9/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.9/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.9/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.9/callingcardstools/__init__.py
--rw-r--r--   0        0        0     6389 2023-05-19 18:05:32.236311 callingcardstools-0.1.9/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.9/callingcardstools/utils.py
--rw-r--r--   0        0        0     1941 2023-05-19 22:48:48.530351 callingcardstools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 callingcardstools-0.1.9/setup.py
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 callingcardstools-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0    12786 2023-05-19 17:42:53.279362 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/Qbed.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     4252 2023-05-19 18:02:51.599306 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/combine_qc.py
+-rw-r--r--   0        0        0    10112 2023-05-19 23:12:04.741087 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.2.0/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/__init__.py
+-rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/combine_qc.py
+-rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.2.0/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.2.0/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.2.0/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.2.0/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.2.0/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     6389 2023-05-19 18:05:32.236311 callingcardstools-0.2.0/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/utils.py
+-rw-r--r--   0        0        0     1941 2023-05-19 23:13:40.505603 callingcardstools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 callingcardstools-0.2.0/setup.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 callingcardstools-0.2.0/PKG-INFO
```

### Comparing `callingcardstools-0.1.9/LICENSE` & `callingcardstools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/README.md` & `callingcardstools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/mammals/Qbed.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/Qbed.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/mammals/combine_qc.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/combine_qc.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,18 +138,20 @@
     at = AlignmentTagger(barcode_details_path,
                          genome_path)  # pylint:disable=C0103
     status_coder = create_status_coder(at.insert_seq, mapq_threshold)
 
     # start iterating over the bam_chunk
     logger.debug("iterating over bam chunk...")
     for read in bam_in.fetch(until_eof=True):
-        # only look at mapped primary alignments
-        if not read.is_secondary and \
-            not read.is_supplementary and \
-                not read.is_unmapped:
+        # write reads that are not primary, unique reads to the failing list
+        if read.is_secondary or read.is_supplementary or read.is_unmapped:
+            # parse the barcode, tag the read
+            tagged_read = at.tag_read(read)
+            output_dict['failing'].append(tagged_read['read'])
+        else:
             # parse the barcode, tag the read
             tagged_read = at.tag_read(read)
             # eval the read based on quality expectations, get the status
             status = status_coder(tagged_read)
             # add the data to the qbed and qc records
             output_dict['qbed'].update(tagged_read,
                                        status,
```

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.2.0/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.2.0/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.2.0/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py` & `callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/BarcodeParser/yeast/combine_qc.py` & `callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/combine_qc.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.2.0/callingcardstools/QC/StatusFlags.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.2.0/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.2.0/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.2.0/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.2.0/callingcardstools/Reads/split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.2.0/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.2.0/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.2.0/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.2.0/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.2.0/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.2.0/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.2.0/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/__main__.py` & `callingcardstools-0.2.0/callingcardstools/__main__.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/callingcardstools/utils.py` & `callingcardstools-0.2.0/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.9/pyproject.toml` & `callingcardstools-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.9"
+version = "0.2.0"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
```

### Comparing `callingcardstools-0.1.9/setup.py` & `callingcardstools-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'pysam>=0.19.1,<0.20.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.9/PKG-INFO` & `callingcardstools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.9
+Version: 0.2.0
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

