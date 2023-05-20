# Comparing `tmp/pytest-tally-1.0.0.tar.gz` & `tmp/pytest-tally-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-tally-1.0.0.tar", last modified: Thu Apr 13 11:46:13 2023, max compression
+gzip compressed data, was "pytest-tally-1.2.0.tar", last modified: Sat May 20 07:40:22 2023, max compression
```

## Comparing `pytest-tally-1.0.0.tar` & `pytest-tally-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.377107 pytest-tally-1.0.0/
--rw-r--r--   0 jwr003   (623385768) 542971493     1894 2023-03-06 00:13:44.000000 pytest-tally-1.0.0/.gitignore
--rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.0.0/LICENSE
--rw-r--r--   0 jwr003   (623385768) 542971493     2595 2023-04-13 11:46:13.376348 pytest-tally-1.0.0/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493     1677 2023-04-13 09:57:22.000000 pytest-tally-1.0.0/README.md
--rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.0.0/conftest.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.272178 pytest-tally-1.0.0/misc/
--rw-r--r--   0 jwr003   (623385768) 542971493      878 2023-04-12 17:40:39.000000 pytest-tally-1.0.0/misc/CHANGELOG.md
--rw-r--r--   0 jwr003   (623385768) 542971493     1458 2023-03-14 02:29:32.000000 pytest-tally-1.0.0/misc/RELEASE_INSTRUCTIONS
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.319160 pytest-tally-1.0.0/pytest_tally/
--rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.0.0/pytest_tally/__init__.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2785 2023-04-12 17:40:39.000000 pytest-tally-1.0.0/pytest_tally/classes.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.336144 pytest-tally-1.0.0/pytest_tally/clients/
--rw-r--r--   0 jwr003   (623385768) 542971493     5711 2023-04-13 09:49:11.000000 pytest-tally-1.0.0/pytest_tally/clients/rich_dashboard.py
--rw-r--r--   0 jwr003   (623385768) 542971493     6086 2023-04-13 09:49:11.000000 pytest-tally-1.0.0/pytest_tally/plugin.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.0.0/pytest_tally/pytest_reportlog.py
--rw-r--r--   0 jwr003   (623385768) 542971493     1338 2023-04-13 09:23:14.000000 pytest-tally-1.0.0/pytest_tally/utils.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.326518 pytest-tally-1.0.0/pytest_tally.egg-info/
--rw-r--r--   0 jwr003   (623385768) 542971493     2595 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493      603 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/SOURCES.txt
--rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/dependency_links.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      168 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/entry_points.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/requires.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-04-13 11:46:12.000000 pytest-tally-1.0.0/pytest_tally.egg-info/top_level.txt
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-13 11:46:13.375182 pytest-tally-1.0.0/requirements/
--rw-r--r--   0 jwr003   (623385768) 542971493       60 2023-03-06 05:54:30.000000 pytest-tally-1.0.0/requirements/requirements-dev.in
--rw-r--r--   0 jwr003   (623385768) 542971493     2113 2023-04-13 09:47:13.000000 pytest-tally-1.0.0/requirements/requirements-dev.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       56 2023-03-13 00:52:12.000000 pytest-tally-1.0.0/requirements/requirements.in
--rw-r--r--   0 jwr003   (623385768) 542971493      987 2023-04-13 09:47:07.000000 pytest-tally-1.0.0/requirements/requirements.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-04-13 11:46:13.377282 pytest-tally-1.0.0/setup.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493     1846 2023-03-13 04:48:28.000000 pytest-tally-1.0.0/setup.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.064190 pytest-tally-1.2.0/
+-rw-r--r--   0 jwr003   (623385768) 542971493      139 2023-04-15 00:11:14.000000 pytest-tally-1.2.0/.flake8
+-rw-r--r--   0 jwr003   (623385768) 542971493     1900 2023-04-19 18:50:46.000000 pytest-tally-1.2.0/.gitignore
+-rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-04-15 00:11:48.000000 pytest-tally-1.2.0/.isort.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493      419 2023-04-15 03:02:55.000000 pytest-tally-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.2.0/LICENSE
+-rw-r--r--   0 jwr003   (623385768) 542971493     4841 2023-05-20 07:40:22.063186 pytest-tally-1.2.0/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493     3924 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/README.md
+-rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.2.0/conftest.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.955987 pytest-tally-1.2.0/misc/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1346 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/misc/CHANGELOG.md
+-rw-r--r--   0 jwr003   (623385768) 542971493     1698 2023-04-14 05:16:42.000000 pytest-tally-1.2.0/misc/RELEASE_INSTRUCTIONS
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.961205 pytest-tally-1.2.0/pytest_tally/
+-rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.2.0/pytest_tally/__init__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     3466 2023-04-20 02:27:46.000000 pytest-tally-1.2.0/pytest_tally/classes.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.006699 pytest-tally-1.2.0/pytest_tally/clients/
+-rw-r--r--   0 jwr003   (623385768) 542971493     3200 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/app.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    11206 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/rich_dashboard.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.039559 pytest-tally-1.2.0/pytest_tally/clients/templates/
+-rw-r--r--   0 jwr003   (623385768) 542971493    11749 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/templates/index.html
+-rw-r--r--   0 jwr003   (623385768) 542971493     8250 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/plugin.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.2.0/pytest_tally/pytest_reportlog.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2687 2023-04-19 18:51:00.000000 pytest-tally-1.2.0/pytest_tally/utils.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.970415 pytest-tally-1.2.0/pytest_tally.egg-info/
+-rw-r--r--   0 jwr003   (623385768) 542971493     4841 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493      716 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/SOURCES.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/dependency_links.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      163 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/entry_points.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      130 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/requires.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/top_level.txt
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.061710 pytest-tally-1.2.0/requirements/
+-rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-15 00:12:58.000000 pytest-tally-1.2.0/requirements/requirements-dev.in
+-rw-r--r--   0 jwr003   (623385768) 542971493     2882 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements-dev.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       95 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements.in
+-rw-r--r--   0 jwr003   (623385768) 542971493      987 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-05-20 07:40:22.064406 pytest-tally-1.2.0/setup.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493     1920 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/setup.py
```

### Comparing `pytest-tally-1.0.0/.gitignore` & `pytest-tally-1.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -132,8 +132,8 @@
 settings.json
 launch.json
 
 # JetBrains
 .idea/
 
 # pytest-tally scratch file
-data.json
+tally-data.json
```

### Comparing `pytest-tally-1.0.0/LICENSE` & `pytest-tally-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.0.0/misc/CHANGELOG.md` & `pytest-tally-1.2.0/misc/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.2.0 - 2023-05-20
+- Added web app support via Flask
+- Fixed broekn'ds Rich app
+
+## [1.1.1] 2023-04-14
+- Implemented file-lock on shared JSON file to fix client stuttering issue.
+- Added support for CLI option '-l' (lines -separators).
+- Added threading to support new client runtime-keypress ("q" for Quit).
+
+## [1.1.0] 2023-04-10
+- New Rich client option "-f" for fixed-width output.
+- Argprse for Rich client.
+- User can now specify name/location of JSON file.
+
 ## [1.0.0] 2023-03-12
 - Complete rewrite of outcome processing logic to definitively determine the outcome of a test.
 - Added support for CLI option '-n' (do not delete existing data file).
 - Added support for CLI option '-r' (max num rows to display on terminal).
 
 ## [0.1.2] 2023-03-07
 - Added spinner to last test in dashboard table.
```

### Comparing `pytest-tally-1.0.0/pytest_tally/classes.py` & `pytest-tally-1.2.0/pytest_tally/classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,68 @@
-from dataclasses import dataclass
-
 from _pytest.config import Config
 from count_timer import CountTimer
 
 
 class TallyCountTimer(CountTimer):
     """
-    Overriding CountTimer to add a to_json method. For tis module all we care
-    about is duration, and if the counter is running or not.
+    Overriding CountTimer to add a to_json method. For this module all
+    we care about is duration, and if the counter is running or not.
     """
 
     def __init__(self, duration=0):
         super().__init__(duration)
 
     def to_json(self):
         return {
             "elapsed": self.elapsed,
             "running": self.running,
+            "finished": self.elapsed > 0 and not self.running,
         }
 
 
 class TallySession:
     """
     Class to hold pertinent info for the entire Pytest test session.
     A test session is made up of one or more tests.
     """
 
     def __init__(
         self,
         config: Config,
+        session_started: bool = False,
         session_finished: bool = False,
+        num_tests_to_run: int = 0,
+        num_tests_have_run: int = 0,
         session_duration: float = 0.0,
+        lastline: str = "",
+        lastline_ansi: str = "",
         timer: TallyCountTimer = TallyCountTimer(),
         tally_tests: dict = {},
     ) -> None:
+        self.session_started = session_started
         self.session_finished = session_finished
         self.session_duration = session_duration
+        self.num_tests_to_run = num_tests_to_run
+        self.num_tests_have_run = num_tests_have_run
         self.timer = timer
+        self.lastline = lastline
+        self.lastline_ansi = lastline_ansi
         self.tally_tests = tally_tests
         self.config = config
 
     def to_json(self):
         return {
+            "session_started": self.session_started,
             "session_finished": self.session_finished,
             "session_duration": self.session_duration,
+            "num_tests_to_run": self.num_tests_to_run,
+            "num_tests_have_run": self.num_tests_have_run,
             "timer": self.timer.to_json(),
+            "lastline": self.lastline,
+            "lastline_ansi": self.lastline_ansi,
             "tally_tests": {k: v.to_json() for k, v in self.tally_tests.items()},
         }
 
 
 class TallyTest:
     """
     Class to hold pertinent info for each Pytest test executed.
```

### Comparing `pytest-tally-1.0.0/pytest_tally/plugin.py` & `pytest-tally-1.2.0/pytest_tally/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,239 @@
-import json
 import logging
 import os
+import re
 from pathlib import Path
 
 import pytest
 from _pytest.config import Config, ExitCode
 from _pytest.main import Session
 from _pytest.nodes import Item
 from _pytest.reports import TestReport
 from _pytest.runner import CallInfo
+from _pytest.stash import Stash, StashKey
+from _pytest.terminal import TerminalReporter
+from strip_ansi import strip_ansi
 
 from pytest_tally.classes import TallyReport, TallySession, TallyTest
+from pytest_tally.utils import LocakbleJsonFileUtils
 
-DEFAULT_FILE = Path(os.getcwd()) / "data.json"
+DEFAULT_FILE = Path(os.getcwd()) / "tally-data.json"
+FLUSH_TIME = 0.05
 
-global_config = None
+pytest_tally_enabled = StashKey[bool]()
+pytest_tally_json_file = StashKey[Path]()
+pytest_tally_session = StashKey[TallySession]()
 
 logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(name)s - %(message)s")
+stream_handler = logging.StreamHandler()
+stream_handler.setLevel(logging.DEBUG)
+stream_handler.setFormatter(formatter)
+logger.addHandler(stream_handler)
 
 
 def check_tally_enabled(config: Config) -> bool:
-    return bool(config.option.tally) if hasattr(config.option, "tally") else False
-
-
-def get_data_file() -> Path:
-    global global_config
-    return (
-        Path(global_config.option.tally_file)
-        if hasattr(global_config.option, "tally_file")
-        else DEFAULT_FILE
+    stash: Stash = config.stash
+    stash["pytest_tally_enabled"] = (
+        bool(config.option.tally) if hasattr(config.option, "tally") else False
     )
+    return stash["pytest_tally_enabled"]
 
 
 def pytest_addoption(parser) -> None:
     group = parser.getgroup("tally")
     group.addoption(
         "--tally",
         action="store_true",
         help=(
             "Enable the pytest-tally plugin. Writes live summary results data to a JSON"
-            " file for comsumption by a dashboard client."
+            " file for consumption by a dashboard client."
         ),
     ),
     group.addoption(
         "--tally-file",
         action="store",
         default=DEFAULT_FILE,
         help=(
             "Specify the file path to write the pytest-tally data to. Defaults to"
-            " data.json in the current working directory."
+            " tally-data.json in the current working directory."
         ),
     )
 
 
 def pytest_cmdline_main(config: Config) -> None:
-    if not check_tally_enabled(config):
-        return
+    # Define stash values here since this is one of the first pytest hooks to run in a sssion
+    stash: Stash = config.stash
+    stash["pytest_tally_enabled"] = (
+        bool(config.option.tally) if hasattr(config.option, "tally") else False
+    )
+    if not stash["pytest_tally_enabled"]:
+        return
+    stash["pytest_tally_json_file"] = (
+        Path(config.option.tally_file)
+        if hasattr(config.option, "tally_file")
+        else DEFAULT_FILE
+    )
 
-    global global_config
-    global_config = config
+    pytest_tally_session = stash.get("pytest_tally_session", None)
+    if not pytest_tally_session:
+        stash["pytest_tally_session"] = TallySession(config=config)
 
-    if not hasattr(global_config, "_tally_session"):
-        global_config._tally_session = TallySession(
-            config=config,
-        )
 
-
-def write_to_file(session: Session, filename: Path) -> None:
-    global global_config
-    global_config = session.config
-
-    session_data = global_config._tally_session.to_json()
-    os.makedirs(filename.parent, exist_ok=True)
-    with open(filename, "w", encoding="utf-8") as file:
-        json.dump(session_data, file)
+def write_json_to_file(config: Config) -> None:
+    stash: Stash = config.stash
+    file_path = stash.get("pytest_tally_json_file", DEFAULT_FILE)
+    os.makedirs(file_path.parent, exist_ok=True)
+    session_data = stash["pytest_tally_session"].to_json()
+    lock_utils = LocakbleJsonFileUtils(file_path=file_path)
+    lock_utils.overwrite_json(session_data)
 
 
 def pytest_sessionstart(session: Session) -> None:
     if not check_tally_enabled(session.config):
         return
 
-    global global_config
-    global_config = session.config
-
-    global_config._tally_session.timer.start()
-    global_config._tally_session.session_duration = (
-        global_config._tally_session.timer.elapsed
-    )
-    write_to_file(session, get_data_file())
+    pytest_tally_session = session.config.stash["pytest_tally_session"]
+    pytest_tally_session.timer.start()
+    pytest_tally_session.session_started = True
+    pytest_tally_session.session_duration = pytest_tally_session.timer.elapsed
+    write_json_to_file(session.config)
 
 
 def pytest_collection_finish(session: Session) -> None:
     if not check_tally_enabled(session.config):
         return
 
-    global_config._tally_session.session_duration = (
-        global_config._tally_session.timer.elapsed
-    )
-    write_to_file(session, get_data_file())
+    pytest_tally_session = session.config.stash["pytest_tally_session"]
+    pytest_tally_session.num_tests_to_run = len(session.items)
+    pytest_tally_session.session_duration = pytest_tally_session.timer.elapsed
+    write_json_to_file(session.config)
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_setup(item: Item):
-    yield
-
     if not check_tally_enabled(item.session.config):
+        yield
         return
 
-    global global_config
-    global_config = item.session.config
-
     tally_test = TallyTest(node_id=item.nodeid)
     tally_test.timer.reset()
     tally_test.timer.start()
-    global_config._tally_session.tally_tests[item.nodeid] = tally_test
-
+    pytest_tally_session = item.session.config.stash["pytest_tally_session"]
+    pytest_tally_session.tally_tests[item.nodeid] = tally_test
 
-@pytest.hookimpl(hookwrapper=True)
-def pytest_runtest_logreport(report: TestReport) -> None:
+    if pytest_tally_session.num_tests_have_run == 0:
+        write_json_to_file(item.session.config)
+    pytest_tally_session.num_tests_have_run += 1
     yield
 
-    if not global_config:
-        return
 
-    if report.when in ("setup", "teardown") and report.outcome == "failed":
-        outcome = "error"
-    elif hasattr(report, "wasxfail"):
-        if report.outcome in ("passed", "failed"):
-            outcome = "xpassed"
-        elif report.outcome == "skipped":
-            outcome = "xfailed"
-    else:
-        outcome = report.outcome
-
-    tally_report = TallyReport(
-        node_id=report.nodeid,
-        when=report.when,
-        outcome=report.outcome,
-    )
-    try:
-        tally_test = global_config._tally_session.tally_tests[tally_report.node_id]
-        tally_test.reports[tally_report.when] = tally_report
-    except KeyError:
-        logger.warning(f"Could not find tally test for node ID {tally_report.node_id}")
-        return
-
-    if tally_test.test_outcome:
-        tally_test.timer.pause()
-        tally_test.test_duration = tally_test.timer.elapsed
-        return
-
-    if tally_report.when == "setup" and outcome in ["error", "skipped"]:
-        tally_test.timer.pause()
-        tally_test.test_duration = tally_test.timer.elapsed
-        tally_test.test_outcome = outcome.capitalize()
-        return
-
-    if tally_report.when == "call":
-        tally_test.test_outcome = outcome.capitalize()
-        return
-
-
-@pytest.hookimpl(trylast=True)
+@pytest.hookimpl(trylast=True)  # do not remove!
 def pytest_configure(config: Config) -> None:
     if not check_tally_enabled(config):
+        # yield
         return
 
-    global global_config
-    global_config = config
+    assert config.pluginmanager.hasplugin("terminal")
 
-    if not hasattr(config, "_tally_session"):
-        global_config._tally_session = TallySession(
-            config=config,
-        )
+    stash = config.stash
+    pytest_tally_session = stash.get("pytest_tally_session", None)
+    if not pytest_tally_session:
+        stash["pytest_tally_session"] = TallySession(config=config)
+
+    # This code exists solely to extract the single 'lastline' of the session for
+    # display in the dashboard. It is a hacky way to do it, but it works.
+    tr = config.pluginmanager.getplugin("terminalreporter")
+    if tr is not None:
+        oldwrite = tr._tw.write
+
+        def tee_write(s, **kwargs):
+            lastline_matcher = re.compile(r"^==.*in\s\d+.\d+s.*=+")
+            oldwrite(s, **kwargs)
+            match = re.search(lastline_matcher, s)
+            if match:
+                pytest_tally_session.lastline_ansi = match.string.replace(
+                    "=", ""
+                ).strip()
+                pytest_tally_session.lastline = (
+                    strip_ansi(match.string).replace("=", "").strip()
+                )
+                write_json_to_file(config)
+
+        tr._tw.write = tee_write
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item: Item, call: CallInfo) -> None:
     if not check_tally_enabled(item.session.config):
         yield
+        return  # do we need both yield and return?
 
     else:
-        global global_config
-        global_config = item.session.config
+        session_config = item.session.config
+        pytest_tally_session = session_config.stash["pytest_tally_session"]
 
         r = yield
         report = r.get_result()
         if report.when == "teardown":
             try:
-                global_config._tally_session.tally_tests[item.nodeid].timer.pause()
+                pytest_tally_session.tally_tests[item.nodeid].timer.pause()
             except KeyError:
                 logger.warning(f"Could not find tally test for node ID {item.nodeid}")
                 return
-        global_config._tally_session.session_duration = (
-            global_config._tally_session.timer.elapsed
+            pytest_tally_session.session_duration = pytest_tally_session.timer.elapsed
+            write_json_to_file(item.session.config)
+
+        if report.when in ("setup", "teardown") and report.outcome == "failed":
+            outcome = "error"
+        elif hasattr(report, "wasxfail"):
+            if report.outcome in ("passed", "failed"):
+                outcome = "xpassed"
+            elif report.outcome == "skipped":
+                outcome = "xfailed"
+        else:
+            outcome = report.outcome
+
+        tally_report = TallyReport(
+            node_id=report.nodeid,
+            when=report.when,
+            outcome=report.outcome,
         )
-        write_to_file(item.session, get_data_file())
+
+        try:
+            tally_test = pytest_tally_session.tally_tests[tally_report.node_id]
+            tally_test.reports[tally_report.when] = tally_report
+        except KeyError:
+            logger.warning(
+                f"Could not find tally test for node ID {tally_report.node_id}"
+            )
+            return
+
+        if tally_test.test_outcome:
+            tally_test.timer.pause()
+            tally_test.test_duration = tally_test.timer.elapsed
+            return
+
+        if tally_report.when == "setup" and outcome in ["error", "skipped"]:
+            tally_test.timer.pause()
+            tally_test.test_duration = tally_test.timer.elapsed
+            tally_test.test_outcome = outcome.capitalize()
+            return
+
+        if tally_report.when == "call":
+            tally_test.test_outcome = outcome.capitalize()
+            return
 
 
-@pytest.hookimpl(
-    tryfirst=True
-)  # run our hookimpl before pytest-html does its own postprocessing
 def pytest_sessionfinish(session: Session, exitstatus: ExitCode) -> None:
+    # This called after whole test run finished, right before returning the exit status to the system.
     if not check_tally_enabled(session.config):
         return
 
-    global global_config
-    global_config = session.config
-
-    global_config._tally_session.timer.pause()
-    global_config._tally_session.session_duration = (
-        global_config._tally_session.timer.elapsed
-    )
-    global_config._tally_session.session_finished = True
+    session_config = session.config
+    pytest_tally_session = session_config.stash["pytest_tally_session"]
 
-    write_to_file(session, get_data_file())
+    pytest_tally_session.timer.pause()
+    pytest_tally_session.session_duration = pytest_tally_session.timer.elapsed
+    pytest_tally_session.session_finished = True
+    write_json_to_file(session.config)
```

### Comparing `pytest-tally-1.0.0/pytest_tally/pytest_reportlog.py` & `pytest-tally-1.2.0/pytest_tally/pytest_reportlog.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.0.0/pytest_tally.egg-info/SOURCES.txt` & `pytest-tally-1.2.0/pytest_tally.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+.flake8
 .gitignore
+.isort.cfg
+.pre-commit-config.yaml
 LICENSE
 README.md
 conftest.py
 setup.py
 misc/CHANGELOG.md
 misc/RELEASE_INSTRUCTIONS
 pytest_tally/__init__.py
@@ -12,12 +15,14 @@
 pytest_tally/utils.py
 pytest_tally.egg-info/PKG-INFO
 pytest_tally.egg-info/SOURCES.txt
 pytest_tally.egg-info/dependency_links.txt
 pytest_tally.egg-info/entry_points.txt
 pytest_tally.egg-info/requires.txt
 pytest_tally.egg-info/top_level.txt
+pytest_tally/clients/app.py
 pytest_tally/clients/rich_dashboard.py
+pytest_tally/clients/templates/index.html
 requirements/requirements-dev.in
 requirements/requirements-dev.txt
 requirements/requirements.in
 requirements/requirements.txt
```

### Comparing `pytest-tally-1.0.0/setup.py` & `pytest-tally-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,49 +10,54 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-tally",
-    version="1.0.0",
+    version="1.2.0",
     author="Jeff Wright",
     author_email="jeff.washcloth@gmail.com",
     license="MIT",
     url="https://github.com/jeffwright13/pytest-tally",
-    description="A Pytest plugin to generate realtime summary stats, and display them in-console using a text-based dashboard.",
+    description=(
+        "A Pytest plugin to generate realtime summary stats, and display them"
+        " in-console using a text-based dashboard."
+    ),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     py_modules=["pytest_tally"],
     python_requires=">=3.8",
     install_requires=[
         "blessed==1.20.0",
         "count-timer==0.3.8",
+        "flask==2.3.2",
         "pytest>=6.2.5",
         "quantiphy==2.19",
         "rich==13.3.2",
         "single-source==0.3.0",
+        "strip-ansi==0.1.1",
     ],
     setup_requires=["setuptools_scm"],
     include_package_data=True,
     classifiers=[
         "Framework :: Pytest",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],
     keywords="pytest pytest-plugin testing tui rich blessed",
     entry_points={
         "pytest11": ["pytest_tally = pytest_tally.plugin"],
         "console_scripts": [
-            "tally = pytest_tally.clients.rich_dashboard:main",
             "tally-rich = pytest_tally.clients.rich_dashboard:main",
+            "tally-flask = pytest_tally.clients.app:main",
         ],
     },
 )
```

