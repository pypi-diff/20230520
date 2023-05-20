# Comparing `tmp/cellmaps_ppi_embedding-0.1.0a2.tar.gz` & `tmp/cellmaps_ppi_embedding-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a2.tar", last modified: Mon May 15 16:49:13 2023, max compression
+gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a3.tar", last modified: Sat May 20 00:06:46 2023, max compression
```

## Comparing `cellmaps_ppi_embedding-0.1.0a2.tar` & `cellmaps_ppi_embedding-0.1.0a3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:49:13.488277 cellmaps_ppi_embedding-0.1.0a2/
--rw-r--r--   0 churas     (504) staff       (20)      192 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a2/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a2/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-15 16:49:13.488454 cellmaps_ppi_embedding-0.1.0a2/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3743 2023-05-15 16:46:17.000000 cellmaps_ppi_embedding-0.1.0a2/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:49:13.475387 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      296 2023-05-15 16:48:35.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     5227 2023-05-12 20:39:39.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    10725 2023-05-12 21:31:58.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:49:13.477515 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      981 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-15 16:49:13.000000 cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:49:13.486369 cellmaps_ppi_embedding-0.1.0a2/docs/
--rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/docs/authors.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a2/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      972 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a2/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-15 16:49:13.489013 cellmaps_ppi_embedding-0.1.0a2/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1860 2023-05-15 16:48:06.000000 cellmaps_ppi_embedding-0.1.0a2/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-15 16:49:13.487952 cellmaps_ppi_embedding-0.1.0a2/tests/
--rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/tests/test_cellmaps_network_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     2804 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/tests/test_cellmapsnetworkembeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a2/tests/test_integration_cellmaps_network_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.011741 cellmaps_ppi_embedding-0.1.0a3/
+-rw-r--r--   0 churas     (504) staff       (20)      192 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-20 00:06:46.011869 cellmaps_ppi_embedding-0.1.0a3/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3743 2023-05-15 16:46:17.000000 cellmaps_ppi_embedding-0.1.0a3/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.005870 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      296 2023-05-19 23:36:32.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     4915 2023-05-20 00:05:39.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    10725 2023-05-20 00:04:55.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.007478 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      981 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-20 00:06:45.000000 cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.010694 cellmaps_ppi_embedding-0.1.0a3/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/Makefile
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/authors.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a3/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      972 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a3/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-20 00:06:46.012305 cellmaps_ppi_embedding-0.1.0a3/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1860 2023-05-15 16:48:06.000000 cellmaps_ppi_embedding-0.1.0a3/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:06:46.011561 cellmaps_ppi_embedding-0.1.0a3/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmaps_network_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     2804 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmapsnetworkembeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a3/tests/test_integration_cellmaps_network_embedding.py
```

### Comparing `cellmaps_ppi_embedding-0.1.0a2/CONTRIBUTING.rst` & `cellmaps_ppi_embedding-0.1.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/LICENSE` & `cellmaps_ppi_embedding-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_ppi_embedding
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate embeddings from networks for CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
 Author: Mayank Jain
 Author-email: maj014@ucsd.edu
 License: MIT license
 Description: ==========================
         cellmaps_ppi_embedding
```

### Comparing `cellmaps_ppi_embedding-0.1.0a2/README.rst` & `cellmaps_ppi_embedding-0.1.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,35 @@
 
 import argparse
 import sys
 import logging
 import logging.config
 import networkx as nx
 from cellmaps_utils import logutils
+from cellmaps_utils import constants
 import cellmaps_ppi_embedding
 from cellmaps_ppi_embedding.runner import Node2VecEmbeddingGenerator
 from cellmaps_ppi_embedding.runner import CellMapsPPIEmbedder
 
 logger = logging.getLogger(__name__)
 
 
-LOG_FORMAT = "%(asctime)-15s %(levelname)s %(relativeCreated)dms " \
-             "%(filename)s::%(funcName)s():%(lineno)d %(message)s"
-
-
-class Formatter(argparse.ArgumentDefaultsHelpFormatter,
-                argparse.RawDescriptionHelpFormatter):
-    """
-    Combine two Formatters to get help and default values
-    displayed when showing help
-
-    """
-    pass
-
-
 def _parse_arguments(desc, args):
     """
     Parses command line arguments
 
     :param desc: description to display on command line
     :type desc: str
     :param args: command line arguments usually :py:func:`sys.argv[1:]`
     :type args: list
     :return: arguments parsed by :py:mod:`argparse`
     :rtype: :py:class:`argparse.Namespace`
     """
     parser = argparse.ArgumentParser(description=desc,
-                                     formatter_class=Formatter)
+                                     formatter_class=constants.ArgParseFormatter)
     parser.add_argument('outdir', help='Output directory')
     parser.add_argument('--inputdir', required=True,
                         help='Directory where apms_edgelist.tsv file resides')
     parser.add_argument('--dimensions', type=int, default=1024,
                         help='Size of embedding to generate')
     parser.add_argument('--walk_length', type=int, default=80,
                         help='Walk Length')
```

### Comparing `cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding/runner.py` & `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-ppi-embedding
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate embeddings from networks for CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
 Author: Mayank Jain
 Author-email: maj014@ucsd.edu
 License: MIT license
 Description: ==========================
         cellmaps_ppi_embedding
```

### Comparing `cellmaps_ppi_embedding-0.1.0a2/cellmaps_ppi_embedding.egg-info/SOURCES.txt` & `cellmaps_ppi_embedding-0.1.0a3/cellmaps_ppi_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/Makefile` & `cellmaps_ppi_embedding-0.1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/conf.py` & `cellmaps_ppi_embedding-0.1.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/index.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/installation.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/make.bat` & `cellmaps_ppi_embedding-0.1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/newrelease.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/pypircfile.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/usage.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/docs/versioningscheme.rst` & `cellmaps_ppi_embedding-0.1.0a3/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/setup.py` & `cellmaps_ppi_embedding-0.1.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/tests/test_cellmaps_network_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmaps_network_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/tests/test_cellmapsnetworkembeddingrunner.py` & `cellmaps_ppi_embedding-0.1.0a3/tests/test_cellmapsnetworkembeddingrunner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a2/tests/test_integration_cellmaps_network_embedding.py` & `cellmaps_ppi_embedding-0.1.0a3/tests/test_integration_cellmaps_network_embedding.py`

 * *Files identical despite different names*

