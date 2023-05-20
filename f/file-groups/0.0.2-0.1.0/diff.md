# Comparing `tmp/file_groups-0.0.2.tar.gz` & `tmp/file_groups-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_groups-0.0.2.tar", last modified: Wed Feb  8 16:59:06 2023, max compression
+gzip compressed data, was "file_groups-0.1.0.tar", last modified: Sat May 20 20:15:56 2023, max compression
```

## Comparing `file_groups-0.0.2.tar` & `file_groups-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-02-08 16:59:06.422021 file_groups-0.0.2/
--rw-r--r--   0 lhn       (1000) lhn       (1000)     1465 2020-10-04 14:24:36.000000 file_groups-0.0.2/LICENSE.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)     1370 2023-02-08 16:59:06.422021 file_groups-0.0.2/PKG-INFO
--rw-r--r--   0 lhn       (1000) lhn       (1000)      602 2023-02-08 16:52:08.000000 file_groups-0.0.2/README.rst
-drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-02-08 16:59:06.421021 file_groups-0.0.2/file_groups.egg-info/
--rw-r--r--   0 lhn       (1000) lhn       (1000)     1370 2023-02-08 16:59:05.000000 file_groups-0.0.2/file_groups.egg-info/PKG-INFO
--rw-r--r--   0 lhn       (1000) lhn       (1000)      460 2023-02-08 16:59:06.000000 file_groups-0.0.2/file_groups.egg-info/SOURCES.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)        1 2023-02-08 16:59:06.000000 file_groups-0.0.2/file_groups.egg-info/dependency_links.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)        1 2023-02-04 11:02:42.000000 file_groups-0.0.2/file_groups.egg-info/not-zip-safe
--rw-r--r--   0 lhn       (1000) lhn       (1000)       15 2023-02-08 16:59:06.000000 file_groups-0.0.2/file_groups.egg-info/requires.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)       12 2023-02-08 16:59:06.000000 file_groups-0.0.2/file_groups.egg-info/top_level.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)        5 2023-02-08 16:59:05.000000 file_groups-0.0.2/file_groups.egg-info/version.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)        5 2023-02-08 16:59:05.000000 file_groups-0.0.2/file_groups.egg-info/version_full.txt
--rw-r--r--   0 lhn       (1000) lhn       (1000)       38 2023-02-08 16:59:06.422021 file_groups-0.0.2/setup.cfg
--rw-r--r--   0 lhn       (1000) lhn       (1000)     1818 2023-02-04 14:44:05.000000 file_groups-0.0.2/setup.py
-drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-02-08 16:59:06.422021 file_groups-0.0.2/src/
--rw-r--r--   0 lhn       (1000) lhn       (1000)        0 2020-10-04 14:24:36.000000 file_groups-0.0.2/src/__init__.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)      434 2023-02-04 23:03:47.000000 file_groups-0.0.2/src/compare_files.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)    10110 2023-02-05 13:28:10.000000 file_groups-0.0.2/src/config_files.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)    11018 2023-02-05 13:28:10.000000 file_groups-0.0.2/src/file_groups.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)     9585 2023-02-04 23:48:46.000000 file_groups-0.0.2/src/file_handler.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)     2152 2023-02-04 23:04:36.000000 file_groups-0.0.2/src/file_handler_compare.py
--rw-r--r--   0 lhn       (1000) lhn       (1000)        0 2020-10-04 14:24:36.000000 file_groups-0.0.2/src/py.typed
--rw-r--r--   0 lhn       (1000) lhn       (1000)      107 2023-02-05 13:28:10.000000 file_groups-0.0.2/src/types.py
+drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-05-20 20:15:56.574116 file_groups-0.1.0/
+-rw-r--r--   0 lhn       (1000) lhn       (1000)     1465 2020-10-04 14:24:36.000000 file_groups-0.1.0/LICENSE.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)     1370 2023-05-20 20:15:56.574116 file_groups-0.1.0/PKG-INFO
+-rw-r--r--   0 lhn       (1000) lhn       (1000)      602 2023-02-08 16:52:08.000000 file_groups-0.1.0/README.rst
+drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-05-20 20:15:56.572116 file_groups-0.1.0/file_groups.egg-info/
+-rw-r--r--   0 lhn       (1000) lhn       (1000)     1370 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/PKG-INFO
+-rw-r--r--   0 lhn       (1000) lhn       (1000)      460 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        1 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        1 2023-02-04 11:02:42.000000 file_groups-0.1.0/file_groups.egg-info/not-zip-safe
+-rw-r--r--   0 lhn       (1000) lhn       (1000)       15 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/requires.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)       12 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/top_level.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        5 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/version.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        5 2023-05-20 20:15:56.000000 file_groups-0.1.0/file_groups.egg-info/version_full.txt
+-rw-r--r--   0 lhn       (1000) lhn       (1000)       38 2023-05-20 20:15:56.574116 file_groups-0.1.0/setup.cfg
+-rw-r--r--   0 lhn       (1000) lhn       (1000)     1818 2023-02-04 14:44:05.000000 file_groups-0.1.0/setup.py
+drwxr-xr-x   0 lhn       (1000) lhn       (1000)        0 2023-05-20 20:15:56.574116 file_groups-0.1.0/src/
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        0 2023-03-05 21:46:55.000000 file_groups-0.1.0/src/__init__.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)      434 2023-02-04 23:03:47.000000 file_groups-0.1.0/src/compare_files.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)    10043 2023-03-07 22:45:46.000000 file_groups-0.1.0/src/config_files.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)    11460 2023-03-07 22:45:46.000000 file_groups-0.1.0/src/file_groups.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)    10124 2023-05-20 18:46:06.000000 file_groups-0.1.0/src/file_handler.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)     2161 2023-03-05 21:54:51.000000 file_groups-0.1.0/src/file_handler_compare.py
+-rw-r--r--   0 lhn       (1000) lhn       (1000)        0 2020-10-04 14:24:36.000000 file_groups-0.1.0/src/py.typed
+-rw-r--r--   0 lhn       (1000) lhn       (1000)      107 2023-02-05 13:28:10.000000 file_groups-0.1.0/src/types.py
```

### Comparing `file_groups-0.0.2/LICENSE.txt` & `file_groups-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_groups-0.0.2/PKG-INFO` & `file_groups-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_groups
-Version: 0.0.2
+Version: 0.1.0
 Summary: Group files into 'protect' and 'work_on' and provide operations for safe delete/move and symlink handling.
 Home-page: https://github.com/lhupfeldt/file_groups
 Author: Lars Hupfeldt Nielsen
 Author-email: lhn@hupfeldtit.dk
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `file_groups-0.0.2/README.rst` & `file_groups-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `file_groups-0.0.2/file_groups.egg-info/PKG-INFO` & `file_groups-0.1.0/file_groups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-groups
-Version: 0.0.2
+Version: 0.1.0
 Summary: Group files into 'protect' and 'work_on' and provide operations for safe delete/move and symlink handling.
 Home-page: https://github.com/lhupfeldt/file_groups
 Author: Lars Hupfeldt Nielsen
 Author-email: lhn@hupfeldtit.dk
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `file_groups-0.0.2/setup.py` & `file_groups-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `file_groups-0.0.2/src/config_files.py` & `file_groups-0.1.0/src/config_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import ast
 import os
 import re
 from pathlib import Path
 import itertools
 from pprint import pformat
+import logging
 from typing import Mapping, Tuple, Sequence, cast
 
 from appdirs import AppDirs # type: ignore
 
 from .types import FsPath
 
 
+_LOG = logging.getLogger(__name__)
+
+
 class ConfigException(Exception):
     """Invalid configuration"""
 
 
 class ConfigFiles():
     r"""Handle config files.
 
@@ -68,15 +72,14 @@
     Note that for security ast.literal_eval is used to interpret the config, so no code is allowed.
 
     Arguments:
         protect: An optional sequence of regexes to be added to protect[recursive] for all directories.
         ignore_config_dirs_config_files: Ignore config files in standard config directories.
         ignore_per_directory_config_files: Ignore config files in collected directories.
         remember_configs: Store loaded and merged configs in `dir_configs` member variable.
-        debug: Be extremely verbose.
 
     Members:
        global_config: dict
        remember_configs: Whether per directory resolved/merged configs are stored in `dir_configs`.
        dir_configs: dict[str: dict] Mapping from dir name to directory specific config dict. Only if remember_configs is True.
     """
 
@@ -84,18 +87,17 @@
     _fg_key = "file_groups"
     _protect_key = "protect"
     _valid_dir_protect_scopes = ("local", "recursive")
     _valid_config_dir_protect_scopes = ("local", "recursive", "global")
 
     def __init__(
             self, protect: Sequence[re.Pattern] = (),
-            ignore_config_dirs_config_files=False, ignore_per_directory_config_files=False, remember_configs=False, debug=False):
+            ignore_config_dirs_config_files=False, ignore_per_directory_config_files=False, remember_configs=False):
         super().__init__()
         self.remember_configs = remember_configs
-        self.debug = debug
 
         self.per_dir_configs: dict[str, dict] = {}  # key is abs_dir_path, value is config dict
         self.global_config = {
             "file_groups": {
                 "protect": {
                     "local": set(),
                     "recursive": set(protect),
@@ -104,69 +106,64 @@
         }
 
         self.ignore_per_directory_config_files = ignore_per_directory_config_files
 
         if not ignore_config_dirs_config_files:
             app_dirs = AppDirs("file_groups", "Hupfeldt_IT")
             config_dirs = app_dirs.site_config_dir.split(':') + [app_dirs.user_config_dir]
-            self.trace("config_dirs:", config_dirs)
+            _LOG.debug("config_dirs: %s", config_dirs)
             gfpt = self.global_config["file_groups"]["protect"]
             for conf_dir in config_dirs:
                 conf_dir = Path(conf_dir)
                 if not conf_dir.exists():
                     continue
 
                 new_config, _ = self._read_and_validate_config_file(conf_dir, self.global_config, self._valid_config_dir_protect_scopes, False)
                 if self.remember_configs:
                     self.per_dir_configs[str(conf_dir)] = new_config
 
                 fpt = new_config["file_groups"]["protect"]
                 cast(set, gfpt["recursive"]).update(fpt.get("global", ()))
-                self.trace(f"Merged global config:\n{pformat(new_config)}")
+                _LOG.debug("Merged global config:\n %s", pformat(new_config))
 
                 try:
                     del fpt['global']
                 except KeyError:
                     pass
 
         # self.default_config_file_example = self.default_config_file.with_suffix('.example.py')
 
-    def trace(self, *args, **kwargs):
-        """call `print` if debug is true"""
-        if self.debug:
-            print(*args, **kwargs)
-
     def _get_single_conf_file(self, conf_dir: Path, ignore_config_files: bool) -> Tuple[dict|None, Path|None]:
         """Return the config file content and path if any config file is found in conf_dir. Error if two are found."""
-        self.trace(f"Checking for config file in directory: {conf_dir}")
+        _LOG.debug("Checking for config file in directory: %s", conf_dir)
 
         num_files = 0
         for cfn in self._conf_file_names:
             tmp_conf_file = conf_dir/cfn
             if tmp_conf_file.exists():
                 conf_file = tmp_conf_file
                 num_files += 1
 
         if num_files == 1:
             if ignore_config_files:
-                self.trace(f"Ignoring config file: {conf_file}")
+                _LOG.debug("Ignoring config file: %s", conf_file)
                 return None, None
 
-            self.trace(f"Read config file: {conf_file}")
+            _LOG.debug("Read config file: %s", conf_file)
             with open(conf_file, encoding="utf-8") as fh:
                 new_config = ast.literal_eval(fh.read())
-            self.trace(pformat(new_config))
+            _LOG.debug("%s", pformat(new_config))
             return new_config, conf_file
 
         if num_files == 0:
-            self.trace(f"No config file in directory {conf_dir}")
+            _LOG.debug("No config file in directory %s", conf_dir)
             return None, None
 
         msg = f"More than one config file in dir '{conf_dir}': {self._conf_file_names}."
-        self.trace(msg)
+        _LOG.debug("%s", msg)
         raise ConfigException(msg)
 
     def _read_and_validate_config_file(
             self, conf_dir: Path, parent_conf: dict, valid_protect_scopes: Tuple[str, ...], ignore_config_files: bool
     ) -> Tuple[dict, Path|None]:
         """Read config file, validate keys and compile regexes and merge with parent.
 
@@ -194,25 +191,28 @@
             protect_conf = new_config[self._fg_key][self._protect_key]
         except KeyError as ex:
             raise ConfigException(f"Config file '{conf_file}' is missing mandatory configuration '{self._fg_key}[{self._protect_key}]'.") from ex
 
         for key, val in protect_conf.items():
             if key not in valid_protect_scopes:
                 msg = f"The only keys allowed in '{self._fg_key}[{self._protect_key}]' section in the config file '{conf_file}' are: {valid_protect_scopes}. Got: '{key}'."
-                self.trace(msg)
+                _LOG.debug("%s", msg)
                 raise ConfigException(msg)
 
             protect_conf[key] = set(re.compile(pattern) for pattern in val)
             if key == "recursive":
                 protect_conf[key].update(parent_conf[self._fg_key][self._protect_key][key])
 
         for key in self._valid_dir_protect_scopes:  # Do NOT use the 'valid_protect_scopes' argument here
             protect_conf.setdefault(key, set())
 
-        self.trace(f"Merged directory config:\n{pformat(new_config)}")
+        lvl = logging.DEBUG
+        if _LOG.isEnabledFor(lvl):
+            _LOG.log(lvl, "Merged directory config:\n%s", pformat(new_config))
+
         return new_config, conf_file
 
     def dir_config(self, conf_dir: Path, parent_conf: dict) -> Tuple[dict, Path|None]:
         """Read and merge config file from directory 'conf_dir' with 'parent_conf'.
 
         If directory has no parent in the file_groups included dirs, then self.global_config must be supplied as parent_conf.
         """
```

### Comparing `file_groups-0.0.2/src/file_groups.py` & `file_groups-0.1.0/src/file_groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 from os import DirEntry
 from pathlib import Path
 import re
 from collections import defaultdict
 from dataclasses import dataclass
 from itertools import chain
 from enum import Enum
+import logging
 from typing import Sequence
 
 from .config_files import ConfigFiles
 
 
+_LOG = logging.getLogger(__name__)
+
+
 class GroupType(Enum):
     MUST_PROTECT = 0
     MAY_WORK_ON = 1
 
 
 @dataclass
 class _Group():
@@ -28,46 +32,44 @@
     symlinks: dict[str, DirEntry]
     symlinks_by_abs_points_to: dict[str, list[DirEntry]]
 
     # For stats only
     num_directories: int = 0
     num_directory_symlinks: int = 0
 
-    def add_entry_match(self, entry, *, debug):
+    def add_entry_match(self, entry):
         """Abstract, but abstract and dataclass does not work with mypy. https://github.com/python/mypy/issues/500"""
 
 @dataclass
 class _IncludeMatchGroup(_Group):
     include: re.Pattern|None = None
 
-    def add_entry_match(self, entry, *, debug):
+    def add_entry_match(self, entry):
         if not self.include:
             self.files[entry.path] = entry
             return
 
         match = self.include.match(entry.name)
-        if debug:
-            print(f' - include {self.include} match {match}')
+        _LOG.debug(" - include %s, match %s", self.include, match)
 
         if match:
             self.files[entry.path] = entry
 
 
 @dataclass
 class _ExcludeMatchGroup(_Group):
     exclude: re.Pattern|None = None
 
-    def add_entry_match(self, entry, *, debug):
+    def add_entry_match(self, entry):
         if not self.exclude:
             self.files[entry.path] = entry
             return
 
         match = self.exclude.match(entry.name)
-        if debug:
-            print(f' - exclude {self.exclude} match {match}')
+        _LOG.debug(" - exclude %s, match %s", self.exclude, match)
 
         if not match:
             self.files[entry.path] = entry
 
 
 class FileGroups():
     """Create six different groups of regular files and symlinks by collecting files under specified directories.
@@ -81,55 +83,51 @@
         protect_dirs_seq: Directories in which (regular) files may not be deleted/modified.
             Directory may be a subdirectory of (or the same, for convenient globbing) as a work_dirs_seq directory.
 
         work_dirs_seq: Directories in which to potentially delete/rename/modify files.
             Directory may be a subdirectory of (or the same, for convenient globbing) as a protect_dirs_seq directory.
 
         protect_exclude: Exclude files matching regex in the protected files (does not apply to symlinks). Default: Include ALL.
+            Note: Since these files are excluded from protection, it means they er NOT protected!
         work_include: Only include files matching regex in the may_work_on files (does not apply to symlinks). Default: Include ALL.
 
         ignore_config_dirs_config_files: Ignore config files in standard config directories.
         ignore_per_directory_config_files: Ignore config files in collected directories.
-
-        debug: Be extremely verbose.
     """
 
     def __init__(
             self,
             protect_dirs_seq: Sequence[Path], work_dirs_seq: Sequence[Path],
             *,
             protect: Sequence[re.Pattern] = (),
             protect_exclude: re.Pattern|None = None, work_include: re.Pattern|None = None,
             ignore_config_dirs_config_files=False, ignore_per_directory_config_files=False,
-            remember_configs=True,
-            debug=False):
+            remember_configs=True):
         super().__init__()
-        self.debug = debug
 
         self.config_files = ConfigFiles(
             protect=protect,
             ignore_config_dirs_config_files=ignore_config_dirs_config_files,
             ignore_per_directory_config_files=ignore_per_directory_config_files,
-            remember_configs=remember_configs,
-            debug=debug)
+            remember_configs=remember_configs)
 
         # Turn all paths into absolute paths with symlinks resolved, keep referrence to original argument for messages
         protect_dirs: dict[str, Path] = {os.path.abspath(os.path.realpath(kp)): kp for kp in protect_dirs_seq}
 
         work_dirs: dict[str, Path] = {}
         for input_work_dir in work_dirs_seq:
             real_dp = os.path.abspath(os.path.realpath(input_work_dir))
             if real_dp in protect_dirs:
                 specified_protect_dir = protect_dirs[real_dp]
 
                 if input_work_dir == specified_protect_dir:
-                    print(f"Ignoring 'work' dir '{input_work_dir}' which is also a 'protect' dir.")
+                    _LOG.info("Ignoring 'work' dir '%s' which is also a 'protect' dir.", input_work_dir)
                     continue
 
-                print(f"Ignoring 'work' dir '{real_dp}' (from argument '{input_work_dir}') which is also a 'protect' dir (from argument '{specified_protect_dir}').")
+                _LOG.info("Ignoring 'work' dir '%s' (from argument '%s') which is also a 'protect' dir (from argument '%s').", real_dp, input_work_dir, specified_protect_dir)
                 continue
 
             work_dirs[real_dp] = input_work_dir
 
         self.must_protect = _ExcludeMatchGroup(GroupType.MUST_PROTECT, protect_dirs, {}, {}, defaultdict(list), exclude=protect_exclude)
         self.may_work_on = _IncludeMatchGroup(GroupType.MAY_WORK_ON, work_dirs, {}, {}, defaultdict(list), include=work_include)
 
@@ -172,66 +170,62 @@
             top/d1/d1/f2.jpg
             top/d1/d1/f2.JPG
             top/d2/d1/f1.jpg
 
         This is called from __init__(), so there would normally be no need to call this explicitly.
         """
 
-        def trace(*args, **kwargs):
-            if self.debug:
-                print(*args, **kwargs)
-
         checked_dirs: set[str] = set()
 
         def find_group(abs_dir_path: str, group: _Group, other_group: _Group, parent_conf: dict):
             """Find all files belonging to 'group'"""
-            trace(f'find {group.typ.name}:', abs_dir_path)
+            _LOG.debug("find %s: %s", group.typ.name, abs_dir_path)
             if abs_dir_path in checked_dirs:
-                trace('directory already checked')
+                _LOG.debug("directory already checked")
                 return
 
             group.num_directories += 1
             dir_config, config_file = self.config_files.dir_config(Path(abs_dir_path), parent_conf)
 
             for entry in os.scandir(abs_dir_path):
                 if entry.is_dir(follow_symlinks=False):
                     if entry.path in other_group.dirs:
-                        trace(f"find {group.typ.name} - '{entry.path}' is in '{other_group.typ.name}' dir list and not in '{group.typ.name}' dir list")
+                        _LOG.debug("find %s - '%s' is in '%s' dir list and not in '%s' dir list", group.typ.name, entry.path, other_group.typ.name, group.typ.name)
                         find_group(entry.path, other_group, group, dir_config)
                         continue
 
                     find_group(entry.path, group, other_group, dir_config)
                     continue
 
                 if config_file and entry.name == config_file.name:
                     continue
 
                 current_group = group
                 if group.typ is GroupType.MAY_WORK_ON:
                     # We need to check for match against configured protect patterns, if match, then the file must got to protect group instead
                     pattern = self.config_files.is_protected(entry, dir_config)
                     if pattern:
-                        trace(f"find {group.typ.name} - '{entry.path}' is protected by regex {pattern}, assigning to group {other_group.typ.name} instead.")
+                        _LOG.debug("find %s - '%s' is protected by regex %s, assigning to group %s instead.", group.typ.name, entry.path, pattern, other_group.typ.name)
                         current_group = other_group
 
                 if entry.is_symlink():
                     points_to = os.readlink(entry)
                     abs_points_to = os.path.normpath(os.path.join(abs_dir_path, points_to))
 
                     if entry.is_dir(follow_symlinks=True):
-                        trace(f"find {current_group.typ.name} - '{entry.path}' -> '{points_to}' is a symlink to a directory - ignoring")
+                        _LOG.debug("find %s - '%s' -> '%s' is a symlink to a directory - ignoring", current_group.typ.name, entry.path, points_to)
                         current_group.num_directory_symlinks += 1
                         continue
 
                     current_group.symlinks[entry.path] = entry
                     current_group.symlinks_by_abs_points_to[abs_points_to].append(entry)
                     continue
 
-                trace(f'find {current_group.typ.name} - entry name: {entry.name}')
-                current_group.add_entry_match(entry, debug=self.debug)
+                _LOG.debug("find %s - entry name: %s", current_group.typ.name, entry.name)
+                current_group.add_entry_match(entry)
 
             checked_dirs.add(abs_dir_path)
 
         for any_dir in sorted(chain(self.must_protect.dirs, self.may_work_on.dirs), key=lambda dd: len(Path(dd).parts)):
             parent_dir = Path(any_dir)
             while len(parent_dir.parts) > 1:
                 parent_conf = self.config_files.per_dir_configs.get(any_dir)
@@ -244,53 +238,63 @@
 
             if any_dir in self.must_protect.dirs:
                 find_group(any_dir, self.must_protect, self.may_work_on, parent_conf)
             else:
                 find_group(any_dir, self.may_work_on, self.must_protect, parent_conf)
 
     def dump(self):
-        """Print collected files. This may be A LOT of output for large directories."""
+        """Log collected files. This may be A LOT of output for large directories."""
 
-        print()
+        log = _LOG.getChild("dump")
+        lvl = logging.DEBUG
+        if not log.isEnabledFor(lvl):
+            return
+
+        log.log(lvl, "")
 
-        print('must protect:')
+        log.log(lvl, "must protect:")
         for path in self.must_protect.files:
-            print(path)
-        print()
+            log.log(lvl, "%s", path)
+        log.log(lvl, "")
 
-        print('must protect symlinks:')
+        log.log(lvl, "must protect symlinks:")
         for path in self.must_protect.symlinks:
-            print(path, '->', os.readlink(path))
-        print()
+            log.log(lvl, "%s -> %s", path, os.readlink(path))
+        log.log(lvl, "")
 
-        print('must protect symlinks by absolute points to:')
+        log.log(lvl, "must protect symlinks by absolute points to:")
         for abs_points_to, lnks in self.must_protect.symlinks_by_abs_points_to.items():
-            print(lnks, '->', abs_points_to)
-        print()
+            log.log(lvl, "%s -> %s", lnks, abs_points_to)
+        log.log(lvl, "")
 
-        print('may work on:')
+        log.log(lvl, "may work on:")
         for path in self.may_work_on.files:
-            print(path)
-        print()
+            log.log(lvl, "%s", path)
+        log.log(lvl, "")
 
-        print('may work on symlinks:')
+        log.log(lvl, "may work on symlinks:")
         for path in self.may_work_on.symlinks:
-            print(path, '->', os.readlink(path))
-        print()
+            log.log(lvl, "%s -> %s", path, os.readlink(path))
+        log.log(lvl, "")
 
-        print('may work on symlinks by absolute points to:')
+        log.log(lvl, "may work on symlinks by absolute points to:")
         for abs_points_to, lnks in self.may_work_on.symlinks_by_abs_points_to.items():
-            print(lnks, '->', abs_points_to)
-        print()
+            log.log(lvl, "%s -> %s", lnks, abs_points_to)
+        log.log(lvl, "")
 
-        print()
+        log.log(lvl, "")
 
     def stats(self):
-        print('collected protect_directories:', self.must_protect.num_directories)
-        print('collected protect_directory_symlinks:', self.must_protect.num_directory_symlinks)
-        print('collected work_on_directories:', self.may_work_on.num_directories)
-        print('collected work_on_directory_symlinks:', self.may_work_on.num_directory_symlinks)
-
-        print('collected must_protect_files:', len(self.must_protect.files))
-        print('collected must_protect_symlinks:', len(self.must_protect.symlinks))
-        print('collected may_work_on_files:', len(self.may_work_on.files))
-        print('collected may_work_on_symlinks:', len(self.may_work_on.symlinks))
+        log = _LOG.getChild("stats")
+        lvl = logging.INFO
+        if not log.isEnabledFor(lvl):
+            return
+
+        log.log(lvl, "collected protect_directories: %s", self.must_protect.num_directories)
+        log.log(lvl, "collected protect_directory_symlinks: %s", self.must_protect.num_directory_symlinks)
+        log.log(lvl, "collected work_on_directories: %s", self.may_work_on.num_directories)
+        log.log(lvl, "collected work_on_directory_symlinks: %s", self.may_work_on.num_directory_symlinks)
+
+        log.log(lvl, "collected must_protect_files: %s", len(self.must_protect.files))
+        log.log(lvl, "collected must_protect_symlinks: %s", len(self.must_protect.symlinks))
+        log.log(lvl, "collected may_work_on_files: %s", len(self.may_work_on.files))
+        log.log(lvl, "collected may_work_on_symlinks: %s", len(self.may_work_on.symlinks))
```

### Comparing `file_groups-0.0.2/src/file_handler.py` & `file_groups-0.1.0/src/file_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 import shutil
 import re
 from contextlib import contextmanager
+import logging
 from typing import Sequence
 
 from .file_groups import FileGroups
 
 
+_LOG = logging.getLogger(__name__)
+
+
 class FileHandler(FileGroups):
     """Protected files and symlinks safe operations on files in FileGroups.
 
     Check that files being deleted/renamed/moved are not in the protect files set and that files in protect files are not overwritten.
     Re-link symlinks pointing to a file being moved.
     Re-link symlinks when a file being deleted has a corresponding file.
 
     Arguments:
-        protect_dirs_seq, work_dirs_seq, protect_exclude, work_include, debug: See `FileGroups` class.
+        protect_dirs_seq, work_dirs_seq, protect_exclude, work_include: See `FileGroups` class.
         dry_run: Don't actually do anything.
         protected_regexes: Protect files matching this from being deleted or moved.
         delete_symlinks_instead_of_relinking: Normal operation is to re-link to a 'corresponding' or renamed file when renaming or deleting a file.
            If delete_symlinks_instead_of_relinking is true, then symlinks in work_on dirs pointing to renamed/deletes files will be deleted even if
            they could have logically been made to point to a file in a protect dir.
-        debug: Be very verbose.
     """
 
     def __init__(
             self,
             protect_dirs_seq: Sequence[Path], work_dirs_seq: Sequence[Path],
             *,
             dry_run: bool,
             protected_regexes: Sequence[re.Pattern],
             protect_exclude: re.Pattern|None = None, work_include: re.Pattern|None = None,
-            delete_symlinks_instead_of_relinking=False,
-            debug=False):
+            delete_symlinks_instead_of_relinking=False):
         super().__init__(
             protect=protected_regexes,
             protect_dirs_seq=protect_dirs_seq, work_dirs_seq=work_dirs_seq,
-            protect_exclude=protect_exclude, work_include=work_include,
-            debug=debug)
+            protect_exclude=protect_exclude, work_include=work_include)
 
         self.dry_run = dry_run
         self.delete_symlinks_instead_of_relinking = delete_symlinks_instead_of_relinking
 
         # Holds paths of deleted symlinks
         self.deleted_symlinks: set[str] = set()
 
@@ -66,154 +67,163 @@
         self.moved_from = {}
 
         self.num_deleted = 0
         self.num_renamed = 0
         self.num_moved = 0
         self.num_relinked = 0
 
-    def trace(self, *args, **kwargs):
-        if self.debug:
-            print(*args, **kwargs)
-
     def _no_symlink_check_registered_delete(self, delete_path: str):
         """Does a registered delete without checking for symlinks, so that we can use this in the symlink handling."""
         assert isinstance(delete_path, str)
         assert os.path.isabs(delete_path), f"Expected absolute path, got '{delete_path}'"
         assert delete_path not in self.must_protect.files, f"Oops, trying to delete protected file '{delete_path}'."
         assert delete_path not in self.must_protect.symlinks, f"Oops, trying to delete protected symlink '{delete_path}'."
 
-        print("    deleting:", delete_path)
+        _LOG.info("    deleting: %s", delete_path)
         if not self.dry_run:
             os.unlink(delete_path)
         self.num_deleted += 1
 
         if delete_path in self.may_work_on.symlinks:
             self.deleted_symlinks.add(delete_path)
 
     def _handle_single_symlink_chain(self, symlnk_path: str, keep_path):
         """TODO doc - Symlink will only be deleted if it is in self.may_work_on.files."""
 
         assert os.path.isabs(symlnk_path), f"Expected an absolute path, got '{symlnk_path}'"
 
         if symlnk_path in self.deleted_symlinks:
-            self.trace(f"{symlnk_path} previously deleted.")
+            _LOG.debug("%s previously deleted.", symlnk_path)
             return
 
         points_to = os.readlink(symlnk_path)
         abs_points_to = os.path.normpath(os.path.join(os.path.dirname(symlnk_path), points_to))
 
         # Check whether symlink points outside our work files
         if abs_points_to not in self.may_work_on.files and abs_points_to not in self.may_work_on.symlinks:
-            print(f"Keeping symlink pointing outside delete-dirs: '{symlnk_path}' -> '{points_to}' ({abs_points_to})")
+            _LOG.info("Keeping symlink pointing outside delete-dirs: '%s' -> '%s' (%s)", symlnk_path, points_to, abs_points_to)
             return
 
-        print(f"Symlinked: '{symlnk_path}' -> '{points_to}' ({abs_points_to})")
+        _LOG.info("Symlinked: '%s' -> '%s' (%s)", symlnk_path, points_to, abs_points_to)
 
         if self.delete_symlinks_instead_of_relinking or not keep_path:
             # Find symlinks to the symlink which we will delete, and delete those as well
             symlnk_to_symlinks = self.may_work_on.symlinks_by_abs_points_to.get(symlnk_path, [])
             for symlnk_to_symlink in symlnk_to_symlinks:
                 abs_points_to_symlnk = os.path.normpath(os.path.join(os.path.dirname(symlnk_to_symlink), symlnk_to_symlink))
-                print(f"Symlink to symlink: '{symlnk_to_symlink}' ({abs_points_to_symlnk}).")
+                _LOG.info("Symlink to symlink: '%s' (%s).", symlnk_to_symlink, abs_points_to_symlnk)
                 self._handle_single_symlink_chain(abs_points_to_symlnk, keep_path)
 
         if self.delete_symlinks_instead_of_relinking and (symlnk_path in self.may_work_on.files or symlnk_path in self.may_work_on.symlinks):
             self._no_symlink_check_registered_delete(symlnk_path)
             return
 
         if not keep_path:
             if symlnk_path in self.may_work_on.files or symlnk_path in self.may_work_on.symlinks:
                 self._no_symlink_check_registered_delete(symlnk_path)
             else:
                 # TODO, verify message
-                print(f"Created broken symlink '{symlnk_path}' -> '{points_to}'")
+                _LOG.info("Created broken symlink '%s' -> '%s'", symlnk_path, points_to)
             return
 
         abs_keep_path = Path(keep_path).absolute()
         abs_keep_dir = os.path.dirname(abs_keep_path)
         abs_symlnk_dir = os.path.dirname(symlnk_path)
         if abs_keep_dir == abs_symlnk_dir:
             keep_path = os.path.basename(keep_path)
         else:
             try:
                 keep_path = abs_keep_path.relative_to(abs_symlnk_dir)
             except ValueError:
                 keep_path = abs_keep_path
 
-        print(f"Changing symlink: '{symlnk_path}' -> '{keep_path}' (was -> {points_to})")
+        _LOG.info("Changing symlink: '%s' -> '%s' (was -> %s)", symlnk_path, keep_path, points_to)
         if not self.dry_run:
             os.unlink(symlnk_path)
             os.symlink(keep_path, symlnk_path)
 
         self.num_relinked += 1
 
     def _fix_symlinks_to_deleted_or_moved_files(self, from_path: str, to_path):
         """Any symlinks pointing to 'from_path' will be change to point to 'to_path'"""
-        self.trace(f"_fix_symlinks_to_deleted_or_moved_files(self, {from_path}, {to_path})")
+        _LOG.debug("_fix_symlinks_to_deleted_or_moved_files(self, %s, %s)", from_path, to_path)
 
         for symlnk in self.must_protect.symlinks_by_abs_points_to.get(from_path, ()):
-            self.trace(f"_fix_symlinks_to_deleted_or_moved_files, must protect symlink: '{symlnk}'.")
+            _LOG.debug("_fix_symlinks_to_deleted_or_moved_files, must protect symlink: '%s'.", symlnk)
             self._handle_single_symlink_chain(os.fspath(symlnk), to_path)
 
         for symlnk in self.may_work_on.symlinks_by_abs_points_to.get(from_path, ()):
-            self.trace(f"_fix_symlinks_to_deleted_or_moved_files, may_work_on symlink: '{symlnk}'.")
+            _LOG.debug("_fix_symlinks_to_deleted_or_moved_files, may_work_on symlink: '%s'.", symlnk)
             self._handle_single_symlink_chain(os.fspath(symlnk), to_path)
 
-    def registered_delete(self, delete_path: str, corresponding_keep_path):
+    def registered_delete(self, delete_path: str, corresponding_keep_path) -> Path|None:
+        """Return `corresponding_keep_path` as absolute Path"""
         self._no_symlink_check_registered_delete(delete_path)
         self._fix_symlinks_to_deleted_or_moved_files(delete_path, corresponding_keep_path)
+        return Path(corresponding_keep_path).absolute() if corresponding_keep_path else None
 
-    def _registered_move_or_rename(self, from_path: str, to_path, *, is_move):
+    def _registered_move_or_rename(self, from_path: str, to_path, *, is_move) -> Path:
+        """Return `to_path` as absolute Path"""
         assert isinstance(from_path, str)
         assert os.path.isabs(from_path), f"Expected absolute path, got '{from_path}'"
         assert from_path not in self.must_protect.files, f"Oops, trying to move/rename protected file '{from_path}'."
         assert from_path not in self.must_protect.symlinks, f"Oops, trying to move/rename protected symlink '{from_path}'."
-        abs_tp = str(Path(to_path).absolute())
+        res = Path(to_path).absolute()
+        abs_tp = str(res)
         assert abs_tp not in self.must_protect.files, f"Oops, trying to overwrite protected file '{Path(to_path).absolute()}' with '{from_path}'."
         assert abs_tp not in self.must_protect.symlinks, f"Oops, trying to overwrite protected symlink '{to_path}' with '{from_path}'."
 
         if self.dry_run:
             self.moved_from[abs_tp] = from_path
 
         if is_move:
-            print("    moving:", from_path, 'to', os.fspath(to_path))
+            _LOG.info("    moving: %s to %s", from_path, os.fspath(to_path))
             if not self.dry_run:
                 shutil.move(from_path, to_path)
 
             self.num_moved += 1
         else:
-            print("    renaming:", from_path, 'to', os.fspath(to_path))
+            _LOG.info("    renaming: %s to %s", from_path, os.fspath(to_path))
             if not self.dry_run:
                 os.rename(from_path, to_path)
 
             self.num_renamed += 1
 
         self._fix_symlinks_to_deleted_or_moved_files(from_path, to_path)
+        return res
 
-    def registered_move(self, from_path: str, to_path):
-        self._registered_move_or_rename(from_path, to_path, is_move=True)
-
-    def registered_rename(self, from_path: str, to_path):
-        self._registered_move_or_rename(from_path, to_path, is_move=False)
+    def registered_move(self, from_path: str, to_path) -> Path:
+        """Return `to_path` as absolute Path"""
+        return self._registered_move_or_rename(from_path, to_path, is_move=True)
+
+    def registered_rename(self, from_path: str, to_path) -> Path:
+        """Return `to_path` as absolute Path"""
+        return self._registered_move_or_rename(from_path, to_path, is_move=False)
 
     @contextmanager
     def stats(self):
+        log = _LOG.getChild("stats")
+        lvl = logging.INFO
+        if not log.isEnabledFor(lvl):
+            yield
+            return
+
         prefix = ''
 
-        print()
+        log.log(lvl, "")
         if self.dry_run:
-            print("*** DRY RUN ***")
+            log.log(lvl, "*** DRY RUN ***")
             prefix = 'would have '
 
         super().stats()
-        print()
-        print(f'{prefix}deleted:', self.num_deleted)
-        print(f'{prefix}renamed:', self.num_renamed)
-        print(f'{prefix}moved:', self.num_moved)
-        print(f'{prefix}relinked:', self.num_relinked)
+        log.log(lvl, "")
+        log.log(lvl, "%sdeleted: %s", prefix, self.num_deleted)
+        log.log(lvl, "%srenamed: %s", prefix, self.num_renamed)
+        log.log(lvl, "%smoved: %s", prefix, self.num_moved)
+        log.log(lvl, "%srelinked: %s", prefix, self.num_relinked)
 
         try:
             yield
 
         finally:
             if self.dry_run:
-                print("*** DRY RUN ***")
+                log.log(lvl, "*** DRY RUN ***")
```

### Comparing `file_groups-0.0.2/src/file_handler_compare.py` & `file_groups-0.1.0/src/file_handler_compare.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 import re
+import logging
 from typing import Sequence
 
 from .compare_files import CompareFiles
 from .types import FsPath
 from .file_handler import FileHandler
 
 
+_LOG = logging.getLogger(__name__)
+
+
 class FileHandlerCompare(FileHandler):
     """Extend `FileHandler` with a compare method
 
     Arguments:
-        protect_dirs_seq, work_dirs_seq, protect_exclude, work_include, debug: See `FileGroups` class.
+        protect_dirs_seq, work_dirs_seq, protect_exclude, work_include: See `FileGroups` class.
         dry_run, protected_regexes, delete_symlinks_instead_of_relinking: See `FileHandler` class.
         fcmp: Object providing compare function.
     """
 
     def __init__(
             self,
             protect_dirs_seq: Sequence[Path], work_dirs_seq: Sequence[Path], fcmp: CompareFiles,
             *,
             dry_run: bool,
             protected_regexes: Sequence[re.Pattern],
             protect_exclude: re.Pattern|None = None, work_include: re.Pattern|None = None,
-            delete_symlinks_instead_of_relinking=False,
-            debug=False):
+            delete_symlinks_instead_of_relinking=False):
         super().__init__(
             protect_dirs_seq=protect_dirs_seq,
             work_dirs_seq=work_dirs_seq,
             dry_run=dry_run,
             protected_regexes=protected_regexes,
             protect_exclude=protect_exclude,
             work_include=work_include,
-            delete_symlinks_instead_of_relinking=delete_symlinks_instead_of_relinking,
-            debug=debug)
+            delete_symlinks_instead_of_relinking=delete_symlinks_instead_of_relinking)
 
         self._fcmp = fcmp
 
     def compare(self, fsp1: FsPath, fsp2: FsPath) -> bool:
         """Extends CompareFiles.compare with logic to handle 'renamed/moved' files during dry_run."""
 
         if not self.dry_run:
             if self._fcmp.compare(fsp1, fsp2):
-                print(f"Duplicates: '{fsp1}' '{fsp2}'")
+                _LOG.info("Duplicates: '%s' '%s'", fsp1, fsp2)
                 return True
 
             return False
 
         fsp1_abs = str(Path(fsp1).absolute())
         existing_fsp1 = Path(self.moved_from.get(os.fspath(fsp1_abs), fsp1))
         fsp2_abs = str(Path(fsp2).absolute())
         existing_fsp2 = Path(self.moved_from.get(os.fspath(fsp2_abs), fsp2))
         if self._fcmp.compare(existing_fsp1, existing_fsp2):
-            print(f"Duplicates: '{fsp1}' '{fsp2}'")
+            _LOG.info("Duplicates: '%s' '%s'", fsp1, fsp2)
             return True
 
         return False
```

