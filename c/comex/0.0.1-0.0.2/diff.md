# Comparing `tmp/comex-0.0.1.tar.gz` & `tmp/comex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.1.tar", last modified: Sat May 20 03:17:31 2023, max compression
+gzip compressed data, was "comex-0.0.2.tar", last modified: Sat May 20 03:22:50 2023, max compression
```

## Comparing `comex-0.0.1.tar` & `comex-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:17:31.120000 comex-0.0.1/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.1/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     7791 2023-05-20 03:17:31.130000 comex-0.0.1/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7174 2023-05-20 03:17:16.000000 comex-0.0.1/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-20 03:17:31.130000 comex-0.0.1/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.1/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:17:31.120000 comex-0.0.1/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:17:31.120000 comex-0.0.1/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     7791 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:17:31.000000 comex-0.0.1/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:22:50.150000 comex-0.0.2/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.2/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     7884 2023-05-20 03:22:50.160000 comex-0.0.2/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7267 2023-05-20 03:21:28.000000 comex-0.0.2/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-20 03:22:50.160000 comex-0.0.2/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.2/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:22:50.150000 comex-0.0.2/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-20 03:22:50.150000 comex-0.0.2/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     7884 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)      236 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-20 03:22:50.000000 comex-0.0.2/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.1/LICENSE` & `comex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.1/PKG-INFO` & `comex-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -86,15 +86,15 @@
 codeviews: refers to the configuration passed for each codeview
 ````
 
 ### Output Example:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
-<img src="sample.png" >
+<img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
 1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
 2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
 3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
@@ -131,15 +131,15 @@
 Then run the following commands:
 
 ```bash
 rm -rf build dist
 python setup.py sdist bdist_wheel
 ```
 
-Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
+Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation) (`pip install twine` if not installed):
 
 ```bash
 twine upload dist/*
 ```
 
 
 ### About the IBM OSCP Project
```

### Comparing `comex-0.0.1/README.md` & `comex-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 codeviews: refers to the configuration passed for each codeview
 ````
 
 ### Output Example:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
-<img src="sample.png" >
+<img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
 1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
 2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
 3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
@@ -114,15 +114,15 @@
 Then run the following commands:
 
 ```bash
 rm -rf build dist
 python setup.py sdist bdist_wheel
 ```
 
-Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
+Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation) (`pip install twine` if not installed):
 
 ```bash
 twine upload dist/*
 ```
 
 
 ### About the IBM OSCP Project
```

### Comparing `comex-0.0.1/setup.cfg` & `comex-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.1
+version = 0.0.2
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.0.1/src/comex.egg-info/PKG-INFO` & `comex-0.0.2/src/comex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -86,15 +86,15 @@
 codeviews: refers to the configuration passed for each codeview
 ````
 
 ### Output Example:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
-<img src="sample.png" >
+<img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
 
 
 ### Code Organization
 The code is structured in the following way:
 1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
 2. The [codeviews](src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
 3. The [cli.py](src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
@@ -131,15 +131,15 @@
 Then run the following commands:
 
 ```bash
 rm -rf build dist
 python setup.py sdist bdist_wheel
 ```
 
-Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):
+Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation) (`pip install twine` if not installed):
 
 ```bash
 twine upload dist/*
 ```
 
 
 ### About the IBM OSCP Project
```

