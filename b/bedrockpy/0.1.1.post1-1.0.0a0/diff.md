# Comparing `tmp/bedrockpy-0.1.1.post1.tar.gz` & `tmp/bedrockpy-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrockpy-0.1.1.post1.tar", last modified: Mon Sep 19 17:16:02 2022, max compression
+gzip compressed data, was "bedrockpy-1.0.0a0.tar", max compression
```

## Comparing `bedrockpy-0.1.1.post1.tar` & `bedrockpy-1.0.0a0.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxrwx---   0 root         (0)     9997        0 2022-09-19 17:16:02.098336 bedrockpy-0.1.1.post1/
--rw-rw----   0 root         (0)     9997     1065 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/LICENSE.txt
--rw-rw----   0 root         (0)     9997     3804 2022-09-19 17:16:02.098336 bedrockpy-0.1.1.post1/PKG-INFO
--rw-rw----   0 root         (0)     9997     1316 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/README.rst
-drwxrwx---   0 root         (0)     9997        0 2022-09-19 17:16:02.090336 bedrockpy-0.1.1.post1/bedrock/
--rw-rw----   0 root         (0)     9997       27 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/__init__.py
--rw-rw----   0 root         (0)     9997      587 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/_cli.py
--rw-rw----   0 root         (0)     9997      298 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/command_parsers.py
--rw-rw----   0 root         (0)     9997     6739 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/commands.py
--rw-rw----   0 root         (0)     9997     3205 2022-09-19 15:51:08.000000 bedrockpy-0.1.1.post1/bedrock/context.py
--rw-rw----   0 root         (0)     9997      660 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/debug_interface.py
--rw-rw----   0 root         (0)     9997    17675 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/server.py
--rw-rw----   0 root         (0)     9997     1251 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/ui.py
--rw-rw----   0 root         (0)     9997     3029 2022-09-10 11:09:45.000000 bedrockpy-0.1.1.post1/bedrock/utils.py
-drwxrwx---   0 root         (0)     9997        0 2022-09-19 17:16:02.094336 bedrockpy-0.1.1.post1/bedrockpy.egg-info/
--rw-rw----   0 root         (0)     9997     3804 2022-09-19 17:16:02.000000 bedrockpy-0.1.1.post1/bedrockpy.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      379 2022-09-19 17:16:02.000000 bedrockpy-0.1.1.post1/bedrockpy.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2022-09-19 17:16:02.000000 bedrockpy-0.1.1.post1/bedrockpy.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997       67 2022-09-19 17:16:02.000000 bedrockpy-0.1.1.post1/bedrockpy.egg-info/requires.txt
--rw-rw----   0 root         (0)     9997        8 2022-09-19 17:16:02.000000 bedrockpy-0.1.1.post1/bedrockpy.egg-info/top_level.txt
--rw-rw----   0 root         (0)     9997     1502 2022-09-19 17:14:54.000000 bedrockpy-0.1.1.post1/pyproject.toml
--rw-rw----   0 root         (0)     9997       38 2022-09-19 17:16:02.098336 bedrockpy-0.1.1.post1/setup.cfg
+-rwxr-xr-x   0        0        0     1071 2023-05-07 13:53:01.935072 bedrockpy-1.0.0a0/LICENSE.md
+-rwxr-xr-x   0        0        0     1848 2023-05-16 14:59:55.736142 bedrockpy-1.0.0a0/README.md
+-rwxr-xr-x   0        0        0     1681 2023-05-16 15:19:04.060713 bedrockpy-1.0.0a0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-02 13:46:17.293794 bedrockpy-1.0.0a0/src/bedrock/__init__.py
+-rwxr-xr-x   0        0        0      780 2023-05-16 14:38:02.689959 bedrockpy-1.0.0a0/src/bedrock/_demo.py
+-rwxr-xr-x   0        0        0     2336 2023-05-03 15:02:01.889213 bedrockpy-1.0.0a0/src/bedrock/consts.py
+-rwxr-xr-x   0        0        0     9250 2023-05-06 12:00:20.149136 bedrockpy-1.0.0a0/src/bedrock/context.py
+-rwxr-xr-x   0        0        0      505 2023-05-01 19:42:23.485482 bedrockpy-1.0.0a0/src/bedrock/events.py
+-rwxr-xr-x   0        0        0     7516 2023-05-07 14:28:54.118786 bedrockpy-1.0.0a0/src/bedrock/ext/ui/__init__.py
+-rwxr-xr-x   0        0        0     6863 2023-05-07 15:18:48.325559 bedrockpy-1.0.0a0/src/bedrock/ext/ui/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2023-04-29 13:27:19.399359 bedrockpy-1.0.0a0/src/bedrock/py.typed
+-rwxr-xr-x   0        0        0      794 2023-05-01 20:12:55.354814 bedrockpy-1.0.0a0/src/bedrock/request.py
+-rwxr-xr-x   0        0        0     1881 2023-05-05 14:47:44.619100 bedrockpy-1.0.0a0/src/bedrock/response.py
+-rwxr-xr-x   0        0        0    12890 2023-05-07 13:11:27.237467 bedrockpy-1.0.0a0/src/bedrock/server.py
+-rwxr-xr-x   0        0        0     2214 2023-05-16 14:59:44.248930 bedrockpy-1.0.0a0/src/bedrock/utils.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 bedrockpy-1.0.0a0/PKG-INFO
```

### Comparing `bedrockpy-0.1.1.post1/LICENSE.txt` & `bedrockpy-1.0.0a0/LICENSE.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 phoenixR
+Copyright (c) 2023 Jonas da Silva
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

