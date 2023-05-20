# Comparing `tmp/pytest-postgresql-4.1.1.tar.gz` & `tmp/pytest-postgresql-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-postgresql-4.1.1.tar", last modified: Fri Mar 11 20:57:26 2022, max compression
+gzip compressed data, was "pytest-postgresql-5.0.0.tar", last modified: Sat May 20 13:25:37 2023, max compression
```

## Comparing `pytest-postgresql-4.1.1.tar` & `pytest-postgresql-5.0.0.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:26.226791 pytest-postgresql-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8385 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35146 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7650 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    24675 2022-03-11 20:57:26.226791 pytest-postgresql-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14952 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-03-11 20:57:26.226791 pytest-postgresql-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:26.222791 pytest-postgresql-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:26.222791 pytest-postgresql-4.1.1/src/pytest_postgresql/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8078 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/executor_noop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:26.226791 pytest-postgresql-4.1.1/src/pytest_postgresql/factories/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/factories/noprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     6292 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     5903 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/janitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/retry.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-11 20:57:13.000000 pytest-postgresql-4.1.1/src/pytest_postgresql/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 20:57:26.226791 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24675 2022-03-11 20:57:25.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-03-11 20:57:26.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-11 20:57:25.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-11 20:57:26.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-11 20:57:25.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-03-11 20:57:26.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-11 20:57:26.000000 pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:37.211497 pytest-postgresql-5.0.0/pytest_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/executor_noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/pytest_postgresql/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/factories/noprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/janitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/pytest_postgresql/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 13:25:37.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:25:36.000000 pytest-postgresql-5.0.0/pytest_postgresql.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:37.215497 pytest-postgresql-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_janitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_noopexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_postgres_options_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_template_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-20 13:25:21.000000 pytest-postgresql-5.0.0/tests/test_version.py
```

### Comparing `pytest-postgresql-4.1.1/CONTRIBUTING.rst` & `pytest-postgresql-5.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-postgresql-4.1.1/COPYING` & `pytest-postgresql-5.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-postgresql-4.1.1/COPYING.lesser` & `pytest-postgresql-5.0.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-postgresql-4.1.1/README.rst` & `pytest-postgresql-5.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -202,20 +202,14 @@
      - -w
    * - Postgres exe extra arguments (passed via pg_ctl's -o argument)
      - postgres_options
      - --postgresql-postgres-options
      - postgresql_postgres_options
      - -
      -
-   * - Log filename's prefix
-     - logsprefix
-     - --postgresql-logsprefix
-     - postgresql_logsprefix
-     - -
-     -
    * - Location for unixsockets
      - unixsocket
      - --postgresql-unixsocketdir
      - postgresql_unixsocketdir
      - -
      - $TMPDIR
    * - Database name
@@ -474,7 +468,15 @@
 
 The way this will work is that the process fixture will populate template database,
 which in turn will be used automatically by client fixture to create a test database from scratch.
 Fast, clean and no dangling transactions, that could be accidentally rolled back.
 
 Same approach will work with noproces fixture, while connecting to already running postgresql instance whether
 it'll be on a docker machine or running remotely or locally.
+Release
+=======
+
+Install pipenv and --dev dependencies first, Then run:
+
+.. code-block::
+
+    pipenv run tbump [NEW_VERSION]
```

### Comparing `pytest-postgresql-4.1.1/setup.py` & `pytest-postgresql-5.0.0/pytest_postgresql/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2016-2020 by Clearcode <http://clearcode.cc>
+# Copyright (C) 2016 by Clearcode <http://clearcode.cc>
 # and associates (see AUTHORS).
 
 # This file is part of pytest-postgresql.
 
 # pytest-postgresql is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -12,11 +12,10 @@
 # pytest-postgresql is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-postgresql. If not, see <http://www.gnu.org/licenses/>.
-"""pytest-postgresql setup.py module."""
-from setuptools import setup
+"""Main module for pytest-postgresql."""
 
-setup()
+__version__ = "5.0.0"
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/__init__.py` & `pytest-postgresql-5.0.0/pytest_postgresql/factories/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# -*- coding: utf-8 -*-
-# Copyright (C) 2016 by Clearcode <http://clearcode.cc>
+# Copyright (C) 2013-2021 by Clearcode <http://clearcode.cc>
 # and associates (see AUTHORS).
 
 # This file is part of pytest-postgresql.
 
-# pytest-postgresql is free software: you can redistribute it and/or modify
+# pytest-dbfixtures is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
-# pytest-postgresql is distributed in the hope that it will be useful,
+# pytest-dbfixtures is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
-# along with pytest-postgresql. If not, see <http://www.gnu.org/licenses/>.
-"""Main module for pytest-postgresql."""
+# along with pytest-dbfixtures.  If not, see <http://www.gnu.org/licenses/>.
+"""Fixture factories for postgresql fixtures."""
 
-__version__ = "4.1.1"
+from pytest_postgresql.factories.client import postgresql
+from pytest_postgresql.factories.noprocess import postgresql_noproc
+from pytest_postgresql.factories.process import postgresql_proc
+
+__all__ = ("postgresql_proc", "postgresql_noproc", "postgresql")
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/executor.py` & `pytest-postgresql-5.0.0/pytest_postgresql/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,50 +20,47 @@
 import os.path
 import platform
 import re
 import shutil
 import subprocess
 import tempfile
 import time
-from typing import TypeVar, Optional, Any
+from typing import Any, Optional, TypeVar
 
-from pkg_resources import parse_version
 from mirakuru import TCPExecutor
 from mirakuru.exceptions import ProcessFinishedWithError
+from pkg_resources import parse_version
+
+from pytest_postgresql.exceptions import ExecutableMissingException, PostgreSQLUnsupported
 
 _LOCALE = "C.UTF-8"
 
 if platform.system() == "Darwin":
     _LOCALE = "en_US.UTF-8"
 
 
 T = TypeVar("T", bound="PostgreSQLExecutor")
 
 
-class PostgreSQLUnsupported(Exception):
-    """Exception raised when unsupported postgresql would be detected."""
-
-
 class PostgreSQLExecutor(TCPExecutor):
-    """
-    PostgreSQL executor running on pg_ctl.
+    """PostgreSQL executor running on pg_ctl.
 
     Based over an `pg_ctl program
     <http://www.postgresql.org/docs/current/static/app-pg-ctl.html>`_
     """
 
     BASE_PROC_START_COMMAND = (
         "{executable} start -D {datadir} "
         "-o \"-F -p {port} -c log_destination='stderr' "
         "-c logging_collector=off "
         "-c unix_socket_directories='{unixsocketdir}' {postgres_options}\" "
         "-l {logfile} {startparams}"
     )
 
-    VERSION_RE = re.compile(r".* (?P<version>\d+\.\d+)")
+    VERSION_RE = re.compile(r".* (?P<version>\d+(?:\.\d+)?)")
     MIN_SUPPORTED_VERSION = parse_version("10")
 
     def __init__(
         self,
         executable: str,
         host: str,
         port: int,
@@ -76,16 +73,15 @@
         timeout: Optional[int] = 60,
         sleep: float = 0.1,
         user: str = "postgres",
         password: str = "",
         options: str = "",
         postgres_options: str = "",
     ):
-        """
-        Initialize PostgreSQLExecutor executor.
+        """Initialize PostgreSQLExecutor executor.
 
         :param executable: pg_ctl location
         :param host: host under which process is accessible
         :param port: port under which process is accessible
         :param datadir: path to postgresql datadir
         :param unixsocketdir: path to socket directory
         :param logfile: path to logfile for postgresql
@@ -149,16 +145,15 @@
     def clean_directory(self) -> None:
         """Remove directory created for postgresql run."""
         if os.path.isdir(self.datadir):
             shutil.rmtree(self.datadir)
         self._directory_initialised = False
 
     def init_directory(self) -> None:
-        """
-        Initialize postgresql data directory.
+        """Initialize postgresql data directory.
 
         See `Initialize postgresql data directory
             <www.postgresql.org/docs/9.5/static/app-initdb.html>`_
         """
         # only make sure it's removed if it's handled by this exact process
         if self._directory_initialised:
             return
@@ -194,15 +189,22 @@
             if self.running():
                 break
             time.sleep(1)
 
     @property
     def version(self) -> Any:
         """Detect postgresql version."""
-        version_string = subprocess.check_output([self.executable, "--version"]).decode("utf-8")
+        try:
+            version_string = subprocess.check_output([self.executable, "--version"]).decode("utf-8")
+        except FileNotFoundError as ex:
+            raise ExecutableMissingException(
+                f"Could not found {self.executable}. Is PostgreSQL server installed? "
+                f"Alternatively pg_config installed might be from different "
+                f"version that postgresql-server."
+            ) from ex
         matches = self.VERSION_RE.search(version_string)
         assert matches is not None
         return parse_version(matches.groupdict()["version"])
 
     def running(self) -> bool:
         """Check if server is running."""
         if not os.path.exists(self.datadir):
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/executor_noop.py` & `pytest-postgresql-5.0.0/pytest_postgresql/executor_noop.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dbfixtures.  If not, see <http://www.gnu.org/licenses/>.
 """PostgreSQL Noop executor providing connection details for postgres client."""
-from typing import Union, Optional, Any
+from typing import Any, Optional, Union
 
+import psycopg
 from pkg_resources import parse_version
 
-from pytest_postgresql.compat import check_for_psycopg, psycopg
-
 
 class NoopExecutor:
-    """
-    Nooperator executor.
+    """Nooperator executor.
 
     This executor actually does nothing more than provide connection details
     for existing PostgreSQL server. I.E. one already started either on machine
     or with the use of containerisation like kubernetes or docker compose.
     """
 
     def __init__(
@@ -37,16 +35,15 @@
         host: str,
         port: Union[str, int],
         user: str,
         options: str,
         dbname: str,
         password: Optional[str] = None,
     ):
-        """
-        Initialize nooperator executor mock.
+        """Initialize nooperator executor mock.
 
         :param host: Postgresql hostname
         :param port: Postgresql port
         :param user: Postgresql username
         :param options: Additional connection options
         :param password: postgresql password
         :param dbname: postgresql database name
@@ -59,15 +56,14 @@
         self.dbname = dbname
         self._version: Any = None
 
     @property
     def version(self) -> Any:
         """Get postgresql's version."""
         if not self._version:
-            check_for_psycopg()
             # could be called before self.dbname will be created.
             # Use default postgres database
             with psycopg.connect(
                 dbname="postgres",
                 user=self.user,
                 host=self.host,
                 port=self.port,
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/factories/client.py` & `pytest-postgresql-5.0.0/pytest_postgresql/factories/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,52 +12,50 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dbfixtures.  If not, see <http://www.gnu.org/licenses/>.
 """Fixture factory for postgresql client."""
-from typing import List, Optional, Callable, Union, Iterator
+from typing import Callable, Iterator, List, Optional, Union
 
+import psycopg
 import pytest
+from psycopg import Connection
 from pytest import FixtureRequest
 
-from pytest_postgresql.compat import connection, check_for_psycopg, psycopg
 from pytest_postgresql.executor import PostgreSQLExecutor
 from pytest_postgresql.executor_noop import NoopExecutor
 from pytest_postgresql.janitor import DatabaseJanitor
 
 
 def postgresql(
     process_fixture_name: str,
     dbname: Optional[str] = None,
     load: Optional[List[Union[Callable, str]]] = None,
     isolation_level: "Optional[psycopg.IsolationLevel]" = None,
-) -> Callable[[FixtureRequest], Iterator[connection]]:
-    """
-    Return connection fixture factory for PostgreSQL.
+) -> Callable[[FixtureRequest], Iterator[Connection]]:
+    """Return connection fixture factory for PostgreSQL.
 
     :param process_fixture_name: name of the process fixture
     :param dbname: database name
     :param load: SQL, function or function import paths to automatically load
                  into our test database
     :param isolation_level: optional postgresql isolation level
                             defaults to server's default
     :returns: function which makes a connection to postgresql
     """
 
     @pytest.fixture
-    def postgresql_factory(request: FixtureRequest) -> Iterator[connection]:
-        """
-        Fixture factory for PostgreSQL.
+    def postgresql_factory(request: FixtureRequest) -> Iterator[Connection]:
+        """Fixture factory for PostgreSQL.
 
         :param request: fixture request object
         :returns: postgresql client
         """
-        check_for_psycopg()
         proc_fixture: Union[PostgreSQLExecutor, NoopExecutor] = request.getfixturevalue(
             process_fixture_name
         )
 
         pg_host = proc_fixture.host
         pg_port = proc_fixture.port
         pg_user = proc_fixture.user
@@ -65,15 +63,15 @@
         pg_options = proc_fixture.options
         pg_db = dbname or proc_fixture.dbname
         pg_load = load or []
 
         with DatabaseJanitor(
             pg_user, pg_host, pg_port, pg_db, proc_fixture.version, pg_password, isolation_level
         ) as janitor:
-            db_connection: connection = psycopg.connect(
+            db_connection: Connection = psycopg.connect(
                 dbname=pg_db,
                 user=pg_user,
                 password=pg_password,
                 host=pg_host,
                 port=pg_port,
                 options=pg_options,
             )
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/factories/noprocess.py` & `pytest-postgresql-5.0.0/pytest_postgresql/factories/noprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dbfixtures.  If not, see <http://www.gnu.org/licenses/>.
 """Fixture factory for existing postgresql server."""
 import os
-from typing import Union, Callable, List, Iterator, Optional
+from typing import Callable, Iterator, List, Optional, Union
 
 import pytest
 from pytest import FixtureRequest
 
 from pytest_postgresql.config import get_config
 from pytest_postgresql.executor_noop import NoopExecutor
 from pytest_postgresql.janitor import DatabaseJanitor
 
 
 def xdistify_dbname(dbname: str) -> str:
-    """Modified the database name depending on the presence and usage of xdist."""
+    """Modify the database name depending on the presence and usage of xdist."""
     xdist_worker = os.getenv("PYTEST_XDIST_WORKER")
     if xdist_worker:
         return f"{dbname}{xdist_worker}"
     return dbname
 
 
 def postgresql_noproc(
@@ -40,31 +40,29 @@
     port: Union[str, int, None] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     dbname: Optional[str] = None,
     options: str = "",
     load: Optional[List[Union[Callable, str]]] = None,
 ) -> Callable[[FixtureRequest], Iterator[NoopExecutor]]:
-    """
-    Postgresql noprocess factory.
+    """Postgresql noprocess factory.
 
     :param host: hostname
     :param port: exact port (e.g. '8000', 8000)
     :param user: postgresql username
     :param password: postgresql password
     :param dbname: postgresql database name
     :param options: Postgresql connection options
     :param load: List of functions used to initialize database's template.
     :returns: function which makes a postgresql process
     """
 
     @pytest.fixture(scope="session")
     def postgresql_noproc_fixture(request: FixtureRequest) -> Iterator[NoopExecutor]:
-        """
-        Noop Process fixture for PostgreSQL.
+        """Noop Process fixture for PostgreSQL.
 
         :param request: fixture request object
         :returns: tcp executor-like object
         """
         config = get_config(request)
         pg_host = host or config["host"]
         pg_port = port or config["port"] or 5432
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/factories/process.py` & `pytest-postgresql-5.0.0/pytest_postgresql/factories/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dbfixtures.  If not, see <http://www.gnu.org/licenses/>.
 """Fixture factory for postgresql process."""
 import os.path
 import platform
 import subprocess
-from typing import Union, Callable, List, Iterator, Optional, Tuple, Set
-from warnings import warn
+from typing import Callable, Iterator, List, Optional, Set, Tuple, Union
 
 import pytest
-from pytest import FixtureRequest, TempPathFactory
 from port_for import get_port
+from pytest import FixtureRequest, TempPathFactory
 
 from pytest_postgresql.config import get_config
+from pytest_postgresql.exceptions import ExecutableMissingException
 from pytest_postgresql.executor import PostgreSQLExecutor
 from pytest_postgresql.janitor import DatabaseJanitor
 
 
 def postgresql_proc(
     executable: Optional[str] = None,
     host: Optional[str] = None,
@@ -49,20 +49,18 @@
     ] = -1,
     user: Optional[str] = None,
     password: Optional[str] = None,
     dbname: Optional[str] = None,
     options: str = "",
     startparams: Optional[str] = None,
     unixsocketdir: Optional[str] = None,
-    logs_prefix: str = "",
     postgres_options: Optional[str] = None,
     load: Optional[List[Union[Callable, str]]] = None,
 ) -> Callable[[FixtureRequest, TempPathFactory], Iterator[PostgreSQLExecutor]]:
-    """
-    Postgresql process factory.
+    """Postgresql process factory.
 
     :param executable: path to postgresql_ctl
     :param host: hostname
     :param port:
         exact port (e.g. '8000', 8000)
         randomly selected port (None) - any random available port
         -1 - command line or pytest.ini configured port
@@ -71,60 +69,54 @@
         [(2000,3000), {4002,4003}] - random of given range and set
     :param user: postgresql username
     :param password: postgresql password
     :param dbname: postgresql database name
     :param options: Postgresql connection options
     :param startparams: postgresql starting parameters
     :param unixsocketdir: directory to create postgresql's unixsockets
-    :param logs_prefix: prefix for log filename
     :param postgres_options: Postgres executable options for use by pg_ctl
     :param load: List of functions used to initialize database's template.
     :returns: function which makes a postgresql process
     """
 
     @pytest.fixture(scope="session")
     def postgresql_proc_fixture(
         request: FixtureRequest, tmp_path_factory: TempPathFactory
     ) -> Iterator[PostgreSQLExecutor]:
-        """
-        Process fixture for PostgreSQL.
+        """Process fixture for PostgreSQL.
 
         :param request: fixture request object
         :param tmp_path_factory: temporary path object (fixture)
         :returns: tcp executor
         """
         config = get_config(request)
         postgresql_ctl = executable or config["exec"]
-        logfile_prefix = logs_prefix or config["logsprefix"]
         pg_dbname = dbname or config["dbname"]
         pg_load = load or config["load"]
 
         # check if that executable exists, as it's no on system PATH
         # only replace if executable isn't passed manually
         if not os.path.exists(postgresql_ctl) and executable is None:
-            pg_bindir = subprocess.check_output(
-                ["pg_config", "--bindir"], universal_newlines=True
-            ).strip()
+            try:
+                pg_bindir = subprocess.check_output(
+                    ["pg_config", "--bindir"], universal_newlines=True
+                ).strip()
+            except FileNotFoundError as ex:
+                raise ExecutableMissingException(
+                    "Could not found pg_config executable. Is it in systenm $PATH?"
+                ) from ex
             postgresql_ctl = os.path.join(pg_bindir, "pg_ctl")
 
         tmpdir = tmp_path_factory.mktemp(f"pytest-postgresql-{request.fixturename}")
 
-        if logfile_prefix:
-            warn(
-                f"logfile_prefix and logsprefix config option is deprecated, "
-                f"and will be dropped in future releases. All fixture related "
-                f"data resides within {tmpdir}",
-                DeprecationWarning,
-            )
-
         pg_port = get_port(port) or get_port(config["port"])
         assert pg_port is not None
         datadir = tmpdir / f"data-{pg_port}"
         datadir.mkdir()
-        logfile_path = tmpdir / f"{logfile_prefix}postgresql.{pg_port}.log"
+        logfile_path = tmpdir / f"postgresql.{pg_port}.log"
 
         if platform.system() == "FreeBSD":
             with (datadir / "pg_hba.conf").open(mode="a") as conf_file:
                 conf_file.write("host all all 0.0.0.0/0 trust\n")
 
         postgresql_executor = PostgreSQLExecutor(
             executable=postgresql_ctl,
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/janitor.py` & `pytest-postgresql-5.0.0/pytest_postgresql/janitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Database Janitor."""
 import re
 from contextlib import contextmanager
 from functools import partial
 from types import TracebackType
-from typing import TypeVar, Union, Optional, Type, Callable, Iterator
+from typing import Callable, Iterator, Optional, Type, TypeVar, Union
 
+import psycopg
 from pkg_resources import parse_version
+from psycopg import Connection, Cursor
 
-from pytest_postgresql.compat import psycopg, cursor, check_for_psycopg, connection
 from pytest_postgresql.retry import retry
 from pytest_postgresql.sql import loader
 
 Version = type(parse_version("1"))
 
 
 DatabaseJanitorType = TypeVar("DatabaseJanitorType", bound="DatabaseJanitor")
@@ -27,16 +28,15 @@
         port: Union[str, int],
         dbname: str,
         version: Union[str, float, Version],  # type: ignore[valid-type]
         password: Optional[str] = None,
         isolation_level: "Optional[psycopg.IsolationLevel]" = None,
         connection_timeout: int = 60,
     ) -> None:
-        """
-        Initialize janitor.
+        """Initialize janitor.
 
         :param user: postgresql username
         :param host: postgresql host
         :param port: postgresql port
         :param dbname: database name
         :param version: postgresql version number
         :param password: optional postgresql password
@@ -47,15 +47,14 @@
         """
         self.user = user
         self.password = password
         self.host = host
         self.port = port
         self.dbname = dbname
         self._connection_timeout = connection_timeout
-        check_for_psycopg()
         self.isolation_level = isolation_level
         if not isinstance(version, Version):
             self.version = parse_version(str(version))
         else:
             self.version = version
 
     def init(self) -> None:
@@ -88,29 +87,28 @@
         # terminate all connections first while not allowing new connections.
         with self.cursor() as cur:
             self._dont_datallowconn(cur, self.dbname)
             self._terminate_connection(cur, self.dbname)
             cur.execute(f'DROP DATABASE IF EXISTS "{self.dbname}";')
 
     @staticmethod
-    def _dont_datallowconn(cur: cursor, dbname: str) -> None:
+    def _dont_datallowconn(cur: Cursor, dbname: str) -> None:
         cur.execute(f'ALTER DATABASE "{dbname}" with allow_connections false;')
 
     @staticmethod
-    def _terminate_connection(cur: cursor, dbname: str) -> None:
+    def _terminate_connection(cur: Cursor, dbname: str) -> None:
         cur.execute(
             "SELECT pg_terminate_backend(pg_stat_activity.pid)"
             "FROM pg_stat_activity "
             "WHERE pg_stat_activity.datname = %s;",
             (dbname,),
         )
 
     def load(self, load: Union[Callable, str]) -> None:
-        """
-        Loads data into a database.
+        """Load data into a database.
 
         Either runs a passed loader if it's callback,
         or runs predefined loader if it's sql file.
         """
         if isinstance(load, str):
             if "/" in load:
                 _loader: Callable = partial(loader, load)
@@ -127,18 +125,18 @@
             port=self.port,
             user=self.user,
             dbname=self.dbname,
             password=self.password,
         )
 
     @contextmanager
-    def cursor(self) -> Iterator[cursor]:
+    def cursor(self) -> Iterator[Cursor]:
         """Return postgresql cursor."""
 
-        def connect() -> connection:
+        def connect() -> Connection:
             return psycopg.connect(
                 dbname="postgres",
                 user=self.user,
                 password=self.password,
                 host=self.host,
                 port=self.port,
             )
@@ -153,17 +151,19 @@
         try:
             yield cur
         finally:
             cur.close()
             conn.close()
 
     def __enter__(self: DatabaseJanitorType) -> DatabaseJanitorType:
+        """Initialize Database Janitor."""
         self.init()
         return self
 
     def __exit__(
         self: DatabaseJanitorType,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
+        """Exit from Database janitor context cleaning after itself."""
         self.drop()
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/plugin.py` & `pytest-postgresql-5.0.0/pytest_postgresql/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-postgresql.  If not, see <http://www.gnu.org/licenses/>.
 """Plugin module of pytest-postgresql."""
 from tempfile import gettempdir
 
-from pytest_postgresql import factories
 from _pytest.config.argparsing import Parser
 
+from pytest_postgresql import factories
 
 _help_executable = "Path to PostgreSQL executable"
 _help_host = "Host at which PostgreSQL will accept connections"
 _help_port = "Port at which PostgreSQL will accept connections"
 _help_user = "PostgreSQL username"
 _help_password = "PostgreSQL password"
 _help_options = "PostgreSQL connection options"
 _help_startparams = "Starting parameters for the PostgreSQL"
-_help_logsprefix = "Prefix for the log files"
 _help_unixsocketdir = "Location of the socket directory"
 _help_dbname = "Default database name"
 _help_load = "Dotted-style or entrypoint-style path to callable or path to SQL File"
 _help_postgres_options = "Postgres executable extra parameters. Passed via the -o option to pg_ctl"
 
 
 def pytest_addoption(parser: Parser) -> None:
@@ -54,16 +53,14 @@
 
     parser.addini(name="postgresql_password", help=_help_password, default=None)
 
     parser.addini(name="postgresql_options", help=_help_options, default="")
 
     parser.addini(name="postgresql_startparams", help=_help_startparams, default="-w")
 
-    parser.addini(name="postgresql_logsprefix", help=_help_logsprefix, default="")
-
     parser.addini(name="postgresql_unixsocketdir", help=_help_unixsocketdir, default=gettempdir())
 
     parser.addini(name="postgresql_dbname", help=_help_dbname, default="tests")
 
     parser.addini(name="postgresql_load", type="pathlist", help=_help_load, default=None)
     parser.addini(name="postgresql_postgres_options", help=_help_postgres_options, default="")
 
@@ -98,21 +95,14 @@
         "--postgresql-startparams",
         action="store",
         dest="postgresql_startparams",
         help=_help_startparams,
     )
 
     parser.addoption(
-        "--postgresql-logsprefix",
-        action="store",
-        dest="postgresql_logsprefix",
-        help=_help_logsprefix,
-    )
-
-    parser.addoption(
         "--postgresql-unixsocketdir",
         action="store",
         dest="postgresql_unixsocketdir",
         help=_help_unixsocketdir,
     )
 
     parser.addoption(
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql/retry.py` & `pytest-postgresql-5.0.0/pytest_postgresql/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""Small retry callable in case of specific error occurred"""
+"""Small retry callable in case of specific error occurred."""
 
 from datetime import datetime, timedelta
 from time import sleep
-from typing import Callable, TypeVar, Type
-
+from typing import Callable, Type, TypeVar
 
 T = TypeVar("T")
 
 
 def retry(
     func: Callable[[], T], timeout: int = 60, possible_exception: Type[Exception] = Exception
 ) -> T:
-    """
-    Attempt to retry the function for timeout time.
+    """Attempt to retry the function for timeout time.
 
     Most often used for connecting to postgresql database as,
     especially on macos on github-actions, first few tries fails
     with this message:
 
     ... ::
         FATAL:  the database system is starting up
```

### Comparing `pytest-postgresql-4.1.1/src/pytest_postgresql.egg-info/SOURCES.txt` & `pytest-postgresql-5.0.0/pytest_postgresql.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 CHANGES.rst
 CONTRIBUTING.rst
 COPYING
 COPYING.lesser
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
-src/pytest_postgresql/__init__.py
-src/pytest_postgresql/compat.py
-src/pytest_postgresql/config.py
-src/pytest_postgresql/executor.py
-src/pytest_postgresql/executor_noop.py
-src/pytest_postgresql/janitor.py
-src/pytest_postgresql/plugin.py
-src/pytest_postgresql/py.typed
-src/pytest_postgresql/retry.py
-src/pytest_postgresql/sql.py
-src/pytest_postgresql.egg-info/PKG-INFO
-src/pytest_postgresql.egg-info/SOURCES.txt
-src/pytest_postgresql.egg-info/dependency_links.txt
-src/pytest_postgresql.egg-info/entry_points.txt
-src/pytest_postgresql.egg-info/not-zip-safe
-src/pytest_postgresql.egg-info/requires.txt
-src/pytest_postgresql.egg-info/top_level.txt
-src/pytest_postgresql/factories/__init__.py
-src/pytest_postgresql/factories/client.py
-src/pytest_postgresql/factories/noprocess.py
-src/pytest_postgresql/factories/process.py
+pytest_postgresql/__init__.py
+pytest_postgresql/config.py
+pytest_postgresql/exceptions.py
+pytest_postgresql/executor.py
+pytest_postgresql/executor_noop.py
+pytest_postgresql/janitor.py
+pytest_postgresql/plugin.py
+pytest_postgresql/py.typed
+pytest_postgresql/retry.py
+pytest_postgresql/sql.py
+pytest_postgresql.egg-info/PKG-INFO
+pytest_postgresql.egg-info/SOURCES.txt
+pytest_postgresql.egg-info/dependency_links.txt
+pytest_postgresql.egg-info/entry_points.txt
+pytest_postgresql.egg-info/requires.txt
+pytest_postgresql.egg-info/top_level.txt
+pytest_postgresql.egg-info/zip-safe
+pytest_postgresql/factories/__init__.py
+pytest_postgresql/factories/client.py
+pytest_postgresql/factories/noprocess.py
+pytest_postgresql/factories/process.py
+tests/test_executor.py
+tests/test_janitor.py
+tests/test_noopexecutor.py
+tests/test_postgres_options_plugin.py
+tests/test_postgresql.py
+tests/test_template_database.py
+tests/test_version.py
```

