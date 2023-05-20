# Comparing `tmp/JaqalPaq-extras-1.1.1.tar.gz` & `tmp/JaqalPaq-extras-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/jaqalpaq-extras/dist/.tmp-3g6nn6ff/JaqalPaq-extras-1.1.1.tar", last modified: Wed Mar 29 16:23:50 2023, max compression
+gzip compressed data, was "/tmp/build-jaqal/jaqalpaq-extras/dist/.tmp-1x1tnq_t/JaqalPaq-extras-1.2.0a1.tar", last modified: Fri May 19 23:35:44 2023, max compression
```

## Comparing `JaqalPaq-extras-1.1.1.tar` & `JaqalPaq-extras-1.2.0a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       51 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      197 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4202 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3230 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/contrib/vim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/contrib/vim/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/contrib/vim/addons/ftdetect/
--rw-rw-r--   0 root         (0) root         (0)       64 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/contrib/vim/addons/ftdetect/jaqal.vim
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/contrib/vim/addons/syntax/
--rw-rw-r--   0 root         (0) root         (0)     4448 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/contrib/vim/addons/syntax/jaqal.vim
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/examples/Tutorials/
--rw-rw-r--   0 root         (0) root         (0)    30905 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/examples/Tutorials/Transpiler_Demo.ipynb
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     2670 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4202 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1973 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/scheduler/
--rw-rw-r--   0 root         (0) root         (0)      275 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/scheduler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8957 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/cirq/
--rw-rw-r--   0 root         (0) root         (0)      304 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/cirq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5032 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/cirq/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/projectq/
--rw-rw-r--   0 root         (0) root         (0)      302 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/projectq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8717 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/projectq/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/
--rw-rw-r--   0 root         (0) root         (0)      715 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15645 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/frontend.py
--rw-rw-r--   0 root         (0) root         (0)     8777 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/gates.py
--rw-rw-r--   0 root         (0) root         (0)     3558 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/
--rw-rw-r--   0 root         (0) root         (0)      402 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2850 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/frontend.py
--rw-rw-r--   0 root         (0) root         (0)     7648 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/ioncompiler.py
--rw-rw-r--   0 root         (0) root         (0)     1453 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/qscoutam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/
--rw-rw-r--   0 root         (0) root         (0)      437 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7785 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/backend.py
--rw-rw-r--   0 root         (0) root         (0)    13877 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/scheduler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/scheduler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8510 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/scheduler/test_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)      321 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/test_smoke.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/cirq/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/cirq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/cirq/test_cirq_transpiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/projectq/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/projectq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1326 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/projectq/test_projectq_transpiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      719 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_backend.py
--rw-rw-r--   0 root         (0) root         (0)     1248 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_gates.py
--rw-rw-r--   0 root         (0) root         (0)     1322 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2640 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_unroller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/quil/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/quil/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2749 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/quil/test_quil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:50.000000 JaqalPaq-extras-1.1.1/tests/transpilers/tket/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/tket/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      564 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_backend.py
--rw-rw-r--   0 root         (0) root         (0)      967 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_reverse_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2176 2023-03-29 15:58:25.000000 JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       51 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3230 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/ftdetect/
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/ftdetect/jaqal.vim
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/
+-rw-rw-r--   0 root         (0) root         (0)     4448 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/jaqal.vim
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/examples/Tutorials/
+-rw-rw-r--   0 root         (0) root         (0)    30905 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/examples/Tutorials/Transpiler_Demo.ipynb
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     2676 2023-05-19 23:35:44.000000 JaqalPaq-extras-1.2.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/
+-rw-rw-r--   0 root         (0) root         (0)      275 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8957 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/
+-rw-rw-r--   0 root         (0) root         (0)      304 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5032 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/
+-rw-rw-r--   0 root         (0) root         (0)      302 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8717 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/
+-rw-rw-r--   0 root         (0) root         (0)      715 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15645 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/frontend.py
+-rw-rw-r--   0 root         (0) root         (0)     8777 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/gates.py
+-rw-rw-r--   0 root         (0) root         (0)     3558 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/
+-rw-rw-r--   0 root         (0) root         (0)      402 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2850 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/frontend.py
+-rw-rw-r--   0 root         (0) root         (0)     7648 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py
+-rw-rw-r--   0 root         (0) root         (0)     1453 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/
+-rw-rw-r--   0 root         (0) root         (0)      437 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7744 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/backend.py
+-rw-rw-r--   0 root         (0) root         (0)    13877 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8510 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/test_scheduler.py
+-rw-rw-r--   0 root         (0) root         (0)      321 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1344 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/test_cirq_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1326 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/test_projectq_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      719 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_backend.py
+-rw-rw-r--   0 root         (0) root         (0)     1248 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_gates.py
+-rw-rw-r--   0 root         (0) root         (0)     1322 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_transpiler.py
+-rw-rw-r--   0 root         (0) root         (0)     2640 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_unroller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2749 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/test_quil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      564 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_backend.py
+-rw-rw-r--   0 root         (0) root         (0)      967 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py
+-rw-rw-r--   0 root         (0) root         (0)     2176 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_transpiler.py
```

### Comparing `JaqalPaq-extras-1.1.1/LICENSE` & `JaqalPaq-extras-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/PKG-INFO` & `JaqalPaq-extras-1.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaq-extras
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Python tools for Jaqal (extras)
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaq-extras-1.1.1/README.md` & `JaqalPaq-extras-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/contrib/vim/addons/syntax/jaqal.vim` & `JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/jaqal.vim`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/examples/Tutorials/Transpiler_Demo.ipynb` & `JaqalPaq-extras-1.2.0a1/examples/Tutorials/Transpiler_Demo.ipynb`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/setup.cfg` & `JaqalPaq-extras-1.2.0a1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = JaqalPaq-extras
 author = Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 author_email = qscout@sandia.gov
 description = Python tools for Jaqal (extras)
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.1.1
+version = 1.2.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,15 +18,15 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = JaqalPaq==1.1.1; QSCOUT-gatemodels>=1.1.1
+install_requires = JaqalPaq==1.2.0a1; QSCOUT-gatemodels>=1.2.0a1
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	jaqalpaq.scheduler
 	jaqalpaq.transpilers
```

### Comparing `JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/PKG-INFO` & `JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaq-extras
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Python tools for Jaqal (extras)
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaq-extras-1.1.1/src/JaqalPaq_extras.egg-info/SOURCES.txt` & `JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/scheduler/scheduler.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/cirq/frontend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/frontend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/projectq/frontend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/frontend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/__init__.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/frontend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/frontend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/gates.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/gates.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/qiskit/instance.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/instance.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/frontend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/frontend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/ioncompiler.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/quil/qscoutam.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/backend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     GateSetPredicate,
     NoMidMeasurePredicate,
 )
 
 from jaqalpaq.error import JaqalError
 from jaqalpaq.emulator import UnitarySerializedEmulator, run_jaqal_circuit
 from jaqalpaq.emulator.backend import AbstractBackend
-from jaqalpaq.core.result import ExecutionResult, ProbabilisticSubcircuit
+from jaqalpaq.run.result import ExecutionResult
 from .frontend import _TKET_NAMES, jaqal_circuit_from_tket_circuit
 
 extension_version = "1.0"
 
 
 class JaqalBackend(Backend):
     """
@@ -189,15 +189,15 @@
             Qubit(bit)
             for bit in range(len(result.readouts[0].subcircuit.measured_qubits))
         ]
         if n_shots == 1:
             shots = OutcomeArray.from_readouts(
                 [[int(bit) for shot in result.readouts for bit in shot.as_str]]
             )
-        elif isinstance(result.subcircuits[0], ProbabilisticSubcircuit):
+        elif result.subcircuits[0]._subcircuit.simulated:
             rng = default_rng()
 
             def _generate_outcome(probs):
                 return rng.choice(list(probs.keys()), p=list(probs.values()))
 
             shots = OutcomeArray.from_readouts(
                 [
```

### Comparing `JaqalPaq-extras-1.1.1/src/jaqalpaq/transpilers/tket/frontend.py` & `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/frontend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/scheduler/test_scheduler.py` & `JaqalPaq-extras-1.2.0a1/tests/scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/cirq/test_cirq_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/test_cirq_transpiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/projectq/test_projectq_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/test_projectq_transpiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_backend.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_backend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_gates.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_gates.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_transpiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/qiskit/test_qiskit_unroller.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_unroller.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/quil/test_quil.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/test_quil.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_backend.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_backend.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_reverse_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.1.1/tests/transpilers/tket/test_tket_transpiler.py` & `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_transpiler.py`

 * *Files identical despite different names*

