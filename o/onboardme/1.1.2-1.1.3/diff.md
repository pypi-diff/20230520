# Comparing `tmp/onboardme-1.1.2.tar.gz` & `tmp/onboardme-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.2.tar", max compression
+gzip compressed data, was "onboardme-1.1.3.tar", max compression
```

## Comparing `onboardme-1.1.2.tar` & `onboardme-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0    12541 2023-05-19 13:59:36.158335 onboardme-1.1.2/README.md
--rwxr-xr-x   0        0        0     6784 2023-05-19 18:04:58.873390 onboardme-1.1.2/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.2/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.2/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.1.2/onboardme/console_logging.py
--rw-r--r--   0        0        0     1691 2023-05-19 11:53:30.594074 onboardme-1.1.2/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.2/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.2/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.2/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-19 17:53:54.217096 onboardme-1.1.2/onboardme/help_text.py
--rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.2/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.2/onboardme/misc.py
--rwxr-xr-x   0        0        0     8794 2023-05-19 17:49:38.672937 onboardme-1.1.2/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.2/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.2/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.2/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.2/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-19 18:05:11.059986 onboardme-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    13922 1970-01-01 00:00:00.000000 onboardme-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0    12541 2023-05-19 13:59:36.158335 onboardme-1.1.3/README.md
+-rwxr-xr-x   0        0        0     6784 2023-05-19 18:04:58.873390 onboardme-1.1.3/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.3/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.3/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.1.3/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1691 2023-05-19 11:53:30.594074 onboardme-1.1.3/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.3/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.3/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.3/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-19 17:53:54.217096 onboardme-1.1.3/onboardme/help_text.py
+-rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.3/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.3/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.3/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.3/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.3/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.3/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.3/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-20 10:54:11.892565 onboardme-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    13922 1970-01-01 00:00:00.000000 onboardme-1.1.3/PKG-INFO
```

### Comparing `onboardme-1.1.2/LICENSE.txt` & `onboardme-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/README.md` & `onboardme-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/__init__.py` & `onboardme-1.1.3/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.3/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/console_logging.py` & `onboardme-1.1.3/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/constants.py` & `onboardme-1.1.3/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/dot_files.py` & `onboardme-1.1.3/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/env_config.py` & `onboardme-1.1.3/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/firewall.py` & `onboardme-1.1.3/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/help_text.py` & `onboardme-1.1.3/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/ide_setup.py` & `onboardme-1.1.3/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/misc.py` & `onboardme-1.1.3/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/pkg_management.py` & `onboardme-1.1.3/onboardme/pkg_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,19 @@
     returns True
     """
     run_gaming_setup = False
     if 'gaming' in pkg_groups:
         run_gaming_setup = True
 
     pre_cmds = ['setup', 'update', 'upgrade']
+
     if no_upgrade:
         pre_cmds.pop(2)
 
-    for pre_cmd in ['setup', 'update', 'upgrade']:
+    for pre_cmd in pre_cmds:
         if pre_cmd in cmd_list:
             if pre_cmd == 'update' and 'apt' in pre_cmd:
                 if run_gaming_setup:
                     log.debug("Run gaming commands to update /etc/apt/sources")
                     cmds = ["sudo dpkg --add-architecture i386",
                             f"sudo {PWD}/scripts/update_apt_sources.sh"]
                     subproc(cmds, spinner=False)
```

### Comparing `onboardme-1.1.2/onboardme/subproc.py` & `onboardme-1.1.3/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/onboardme/sudo_setup.py` & `onboardme-1.1.3/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.2/pyproject.toml` & `onboardme-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.2"
+version       = "1.1.3"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.2/PKG-INFO` & `onboardme-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.2
+Version: 1.1.3
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.2 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.3 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
```

