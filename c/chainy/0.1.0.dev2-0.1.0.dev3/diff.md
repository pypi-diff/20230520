# Comparing `tmp/chainy-0.1.0.dev2.tar.gz` & `tmp/chainy-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainy-0.1.0.dev2.tar", last modified: Fri May 19 23:20:18 2023, max compression
+gzip compressed data, was "chainy-0.1.0.dev3.tar", last modified: Fri May 19 23:23:07 2023, max compression
```

## Comparing `chainy-0.1.0.dev2.tar` & `chainy-0.1.0.dev3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:20:18.576743 chainy-0.1.0.dev2/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      511 2023-05-19 23:20:18.576511 chainy-0.1.0.dev2/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1779 2023-05-19 23:19:27.000000 chainy-0.1.0.dev2/README.md
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-19 23:20:18.576814 chainy-0.1.0.dev2/setup.cfg
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      837 2023-05-19 23:19:59.000000 chainy-0.1.0.dev2/setup.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:20:18.570843 chainy-0.1.0.dev2/src/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:20:18.571844 chainy-0.1.0.dev2/src/chainy/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 22:02:43.000000 chainy-0.1.0.dev2/src/chainy/__init__.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      543 2023-05-19 22:30:45.000000 chainy-0.1.0.dev2/src/chainy/config.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      376 2023-05-19 22:30:45.000000 chainy-0.1.0.dev2/src/chainy/llm.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     3089 2023-05-19 22:30:45.000000 chainy-0.1.0.dev2/src/chainy/model.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:20:18.576207 chainy-0.1.0.dev2/src/chainy.egg-info/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      511 2023-05-19 23:20:18.000000 chainy-0.1.0.dev2/src/chainy.egg-info/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      269 2023-05-19 23:20:18.000000 chainy-0.1.0.dev2/src/chainy.egg-info/SOURCES.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-19 23:20:18.000000 chainy-0.1.0.dev2/src/chainy.egg-info/dependency_links.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       12 2023-05-19 23:20:18.000000 chainy-0.1.0.dev2/src/chainy.egg-info/requires.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        7 2023-05-19 23:20:18.000000 chainy-0.1.0.dev2/src/chainy.egg-info/top_level.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.427887 chainy-0.1.0.dev3/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 chainy-0.1.0.dev3/LICENSE
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2413 2023-05-19 23:23:07.427677 chainy-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1826 2023-05-19 23:22:27.000000 chainy-0.1.0.dev3/README.md
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-19 23:23:07.427952 chainy-0.1.0.dev3/setup.cfg
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      934 2023-05-19 23:23:03.000000 chainy-0.1.0.dev3/setup.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.425075 chainy-0.1.0.dev3/src/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.426267 chainy-0.1.0.dev3/src/chainy/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 22:02:43.000000 chainy-0.1.0.dev3/src/chainy/__init__.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      543 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/config.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      376 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/llm.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     3089 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/model.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.427370 chainy-0.1.0.dev3/src/chainy.egg-info/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2413 2023-05-19 23:23:06.000000 chainy-0.1.0.dev3/src/chainy.egg-info/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      277 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       12 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/requires.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        7 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/top_level.txt
```

### Comparing `chainy-0.1.0.dev2/README.md` & `chainy-0.1.0.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 |----- tmpl02.md
 |--- chains/
 |----- example-1.yml
 |--- entrypoint.py
 ```
 
 ## Testing
+
 Tests are located in the `tests/` directory. To run them, use your preferred test runner.
 
 ## Contributing
+
 We welcome contributions! Please open an issue or submit a pull request if you have something to add.
 
 ## License
-MIT
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `chainy-0.1.0.dev2/src/chainy/config.py` & `chainy-0.1.0.dev3/src/chainy/config.py`

 * *Files identical despite different names*

### Comparing `chainy-0.1.0.dev2/src/chainy/model.py` & `chainy-0.1.0.dev3/src/chainy/model.py`

 * *Files identical despite different names*

