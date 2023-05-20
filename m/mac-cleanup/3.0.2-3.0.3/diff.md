# Comparing `tmp/mac_cleanup-3.0.2.tar.gz` & `tmp/mac_cleanup-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mac_cleanup-3.0.2.tar", max compression
+gzip compressed data, was "mac_cleanup-3.0.3.tar", max compression
```

## Comparing `mac_cleanup-3.0.2.tar` & `mac_cleanup-3.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-11 22:17:44.340035 mac_cleanup-3.0.2/LICENSE
--rw-r--r--   0        0        0     3795 2023-05-20 16:36:29.591790 mac_cleanup-3.0.2/README.md
--rw-r--r--   0        0        0      425 2023-05-11 22:17:44.340449 mac_cleanup-3.0.2/mac_cleanup/__init__.py
--rw-r--r--   0        0        0      181 2023-05-11 22:17:44.340660 mac_cleanup-3.0.2/mac_cleanup/__version__.py
--rw-r--r--   0        0        0     8289 2023-05-20 16:28:42.279287 mac_cleanup-3.0.2/mac_cleanup/config.py
--rw-r--r--   0        0        0      652 2023-05-20 16:28:42.280426 mac_cleanup-3.0.2/mac_cleanup/console.py
--rw-r--r--   0        0        0     7720 2023-05-20 16:28:42.286177 mac_cleanup-3.0.2/mac_cleanup/core.py
--rw-r--r--   0        0        0     4185 2023-05-20 16:29:57.350961 mac_cleanup-3.0.2/mac_cleanup/core_modules.py
--rw-r--r--   0        0        0    14634 2023-05-20 16:06:49.038722 mac_cleanup-3.0.2/mac_cleanup/default_modules.py
--rw-r--r--   0        0        0     3790 2023-05-20 16:28:42.307709 mac_cleanup-3.0.2/mac_cleanup/error_handling.py
--rw-r--r--   0        0        0     2918 2023-05-11 22:17:44.341805 mac_cleanup-3.0.2/mac_cleanup/main.py
--rw-r--r--   0        0        0     1181 2023-05-11 22:17:44.341922 mac_cleanup-3.0.2/mac_cleanup/parser.py
--rw-r--r--   0        0        0     3378 2023-05-20 16:28:42.315352 mac_cleanup-3.0.2/mac_cleanup/progress.py
--rwxr-xr-x   0        0        0     3176 2023-05-20 16:28:42.318896 mac_cleanup-3.0.2/mac_cleanup/utils.py
--rw-r--r--   0        0        0     2946 2023-05-20 16:36:29.591839 mac_cleanup-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 22:17:44.340035 mac_cleanup-3.0.3/LICENSE
+-rw-r--r--   0        0        0     3831 2023-05-20 17:39:59.781578 mac_cleanup-3.0.3/README.md
+-rw-r--r--   0        0        0      425 2023-05-11 22:17:44.340449 mac_cleanup-3.0.3/mac_cleanup/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-11 22:17:44.340660 mac_cleanup-3.0.3/mac_cleanup/__version__.py
+-rw-r--r--   0        0        0     8289 2023-05-20 17:35:49.810064 mac_cleanup-3.0.3/mac_cleanup/config.py
+-rw-r--r--   0        0        0      652 2023-05-20 17:35:49.810403 mac_cleanup-3.0.3/mac_cleanup/console.py
+-rw-r--r--   0        0        0     7720 2023-05-20 17:35:49.810702 mac_cleanup-3.0.3/mac_cleanup/core.py
+-rw-r--r--   0        0        0     4185 2023-05-20 17:35:49.811119 mac_cleanup-3.0.3/mac_cleanup/core_modules.py
+-rw-r--r--   0        0        0    14634 2023-05-20 17:36:58.239398 mac_cleanup-3.0.3/mac_cleanup/default_modules.py
+-rw-r--r--   0        0        0     3790 2023-05-20 17:35:49.811893 mac_cleanup-3.0.3/mac_cleanup/error_handling.py
+-rw-r--r--   0        0        0     2918 2023-05-11 22:17:44.341805 mac_cleanup-3.0.3/mac_cleanup/main.py
+-rw-r--r--   0        0        0     1181 2023-05-11 22:17:44.341922 mac_cleanup-3.0.3/mac_cleanup/parser.py
+-rw-r--r--   0        0        0     3378 2023-05-20 17:35:49.812177 mac_cleanup-3.0.3/mac_cleanup/progress.py
+-rwxr-xr-x   0        0        0     3176 2023-05-20 17:35:49.812475 mac_cleanup-3.0.3/mac_cleanup/utils.py
+-rw-r--r--   0        0        0     2946 2023-05-20 17:39:59.756956 mac_cleanup-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4971 1970-01-01 00:00:00.000000 mac_cleanup-3.0.3/PKG-INFO
```

### Comparing `mac_cleanup-3.0.2/LICENSE` & `mac_cleanup-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/README.md` & `mac_cleanup-3.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
   - `java_cache` - Removes **Java head dumps** from home directory
   - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm** etc
   - `kite` - Deletes **Kite** logs
   - `lunarclient` - Removes **Lunar Client** logs and cache
   - `microsoft_teams` - Remove **Microsoft Teams** logs and cache
   - `minecraft` - Remove **Minecraft** logs and cache
   - `npm` - Cleanup **npm** Cache
+  - `pnpm` - Cleanup **pnpm** Cache
   - `pod` - Cleanup **CocoaPods** Cache Files
   - `poetry` - Clears **Poetry** cache
   - `pyenv` - Cleanup **Pyenv-VirtualEnv** Cache
   - `steam` - Remove **Steam** logs and cache
   - `system_caches` - Clear **System cache**
   - `system_log` - Clear **System Log** Files
   - `trash` - Empty the **Trash** on All Mounted Volumes and the Main HDD
@@ -102,15 +103,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.2
+    3.0.3
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

### Comparing `mac_cleanup-3.0.2/mac_cleanup/config.py` & `mac_cleanup-3.0.3/mac_cleanup/config.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/console.py` & `mac_cleanup-3.0.3/mac_cleanup/console.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/core.py` & `mac_cleanup-3.0.3/mac_cleanup/core.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/core_modules.py` & `mac_cleanup-3.0.3/mac_cleanup/core_modules.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/default_modules.py` & `mac_cleanup-3.0.3/mac_cleanup/default_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
     if cmd("type 'npm'"):
         with clc as unit:
             unit.message("Cleaning up npm cache")
             unit.add(Command("npm cache clean --force"))
             unit.add(Path("~/.npm/*").dry_run_only())
 
 
-def pnpn():
+def pnpm():
     from mac_cleanup.utils import cmd
 
     if cmd("type 'pnpm'"):
         with clc as unit:
             unit.message("Cleaning up pnpm Cache...")
             unit.add(Command("pnpm store prune &>/dev/null"))
             unit.add(Path("~/.pnpm-store/*").dry_run_only())
```

### Comparing `mac_cleanup-3.0.2/mac_cleanup/error_handling.py` & `mac_cleanup-3.0.3/mac_cleanup/error_handling.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/main.py` & `mac_cleanup-3.0.3/mac_cleanup/main.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/parser.py` & `mac_cleanup-3.0.3/mac_cleanup/parser.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/progress.py` & `mac_cleanup-3.0.3/mac_cleanup/progress.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/mac_cleanup/utils.py` & `mac_cleanup-3.0.3/mac_cleanup/utils.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.2/pyproject.toml` & `mac_cleanup-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mac_cleanup"
-version = "3.0.2"
+version = "3.0.3"
 description = "Python cleanup script for macOS"
 license = "Apache-2.0"
 authors = [ "Drugsosos" ]
 readme = "README.md"
 homepage = "https://github.com/mac-cleanup/mac-cleanup-py"
 repository = "https://github.com/mac-cleanup/mac-cleanup-py"
 keywords = [
```

### Comparing `mac_cleanup-3.0.2/PKG-INFO` & `mac_cleanup-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mac-cleanup
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python cleanup script for macOS
 Home-page: https://github.com/mac-cleanup/mac-cleanup-py
 License: Apache-2.0
 Keywords: macos,script,cleanup,cleaner
 Author: Drugsosos
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
@@ -73,14 +73,15 @@
   - `java_cache` - Removes **Java head dumps** from home directory
   - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm** etc
   - `kite` - Deletes **Kite** logs
   - `lunarclient` - Removes **Lunar Client** logs and cache
   - `microsoft_teams` - Remove **Microsoft Teams** logs and cache
   - `minecraft` - Remove **Minecraft** logs and cache
   - `npm` - Cleanup **npm** Cache
+  - `pnpm` - Cleanup **pnpm** Cache
   - `pod` - Cleanup **CocoaPods** Cache Files
   - `poetry` - Clears **Poetry** cache
   - `pyenv` - Cleanup **Pyenv-VirtualEnv** Cache
   - `steam` - Remove **Steam** logs and cache
   - `system_caches` - Clear **System cache**
   - `system_log` - Clear **System Log** Files
   - `trash` - Empty the **Trash** on All Mounted Volumes and the Main HDD
@@ -129,15 +130,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.2
+    3.0.3
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

