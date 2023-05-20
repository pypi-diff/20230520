# Comparing `tmp/onboardme-1.1.4.tar.gz` & `tmp/onboardme-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.4.tar", max compression
+gzip compressed data, was "onboardme-1.1.5.tar", max compression
```

## Comparing `onboardme-1.1.4.tar` & `onboardme-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0    12700 2023-05-20 11:41:08.375549 onboardme-1.1.4/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.4/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.4/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.4/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3085 2023-05-20 12:20:28.473119 onboardme-1.1.4/onboardme/console_logging.py
--rw-r--r--   0        0        0     1789 2023-05-20 12:19:03.694838 onboardme-1.1.4/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.4/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.4/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.4/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.4/onboardme/help_text.py
--rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.4/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.4/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.4/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.4/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.4/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.4/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.4/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-20 12:20:39.244511 onboardme-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    14081 1970-01-01 00:00:00.000000 onboardme-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0    12700 2023-05-20 11:41:08.375549 onboardme-1.1.5/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.5/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.5/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.5/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.5/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1789 2023-05-20 12:19:03.694838 onboardme-1.1.5/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.5/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.5/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.5/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.5/onboardme/help_text.py
+-rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.5/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.5/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.5/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.5/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.5/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.5/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.5/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-20 12:26:05.572037 onboardme-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    14081 1970-01-01 00:00:00.000000 onboardme-1.1.5/PKG-INFO
```

### Comparing `onboardme-1.1.4/LICENSE.txt` & `onboardme-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/README.md` & `onboardme-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/__init__.py` & `onboardme-1.1.5/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.5/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/console_logging.py` & `onboardme-1.1.5/onboardme/console_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,42 +11,48 @@
                                "header": "cornflower_blue"}))
 
 
 def print_manual_steps(OS):
     """
     Just prints out the final steps to be done manually, til we automate them
     """
+    rc_file = "~/.bashrc"
     # table to print the results of all the files
     table = Table(expand=True, box=None,
                   title=" ",
-                  row_styles=["", "dim"],
                   border_style="dim",
                   header_style="cornflower_blue",
                   title_style="light_steel_blue")
-    table.add_column("Don't forget these (currently) manual tasks",
+    table.add_column("[u]Don't forget these (currently) manual tasks[/u]",
                      justify="center")
 
     table.add_row(" ")
-    table.add_row("Import subscriptions into FreeTube")
+    table.add_row("📺 Import subscriptions into FreeTube")
+
+    table.add_row(" ")
     table.add_row("⌨️  Set CAPSLOCK to control")
 
     if "Darwin" in OS[0]:
+        table.add_row(" ")
         table.add_row("🐚 Set your default shell to BASH:")
-        table.add_row("  [green]sudo -i")
+        table.add_row("   [green]sudo -i")
         if "arm" in OS[1]:
-            table.add_row("  echo '/opt/homebrew/bin/bash' >> /etc/shells")
-            table.add_row("  exit")
-            table.add_row("  chsh -s /opt/homebrew/bin/bash $(whoami)")
+            shell = '/opt/homebrew/bin/bash'
         else:
-            table.add_row("  echo '/usr/local/bin/bash' >> /etc/shells")
-            table.add_row("  exit")
-            table.add_row("  chsh -s /usr/local/bin/bash $(whoami)")
+            shell = '/usr/local/bin/bash'
+
+        table.add_row(f"   [green]echo {shell} >> /etc/shells && exit")
+        table.add_row(f"   [green]chsh -s {shell} $(whoami)")
+        table.add_row(" ")
+        rc_file = "~/.bash_profile"
+
+    table.add_row(f"🦪 Load your BASH config: [green]source {rc_file}[/]")
+    table.add_row(" ")
 
-    table.add_row("Load your BASH config: [green]source .bashrc[/]")
-    table.add_row("Reboot, as [turquoise2]docker[/] demands it")
+    table.add_row("🐳 Reboot, as [turquoise2]docker[/] demands it")
     table.add_row(" ")
     table.add_row("If you need any help, check the docs:")
     table.add_row("[cyan][link=https://jessebot.github.io/onboardme]"
                   "jessebot.github.io/onboardme[/link]")
     table.add_row(" ")
 
     print_panel(table, '[green]♥ ˖⁺‧Success‧⁺˖ ♥')
```

### Comparing `onboardme-1.1.4/onboardme/constants.py` & `onboardme-1.1.5/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/dot_files.py` & `onboardme-1.1.5/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/env_config.py` & `onboardme-1.1.5/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/firewall.py` & `onboardme-1.1.5/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/help_text.py` & `onboardme-1.1.5/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/ide_setup.py` & `onboardme-1.1.5/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/misc.py` & `onboardme-1.1.5/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/pkg_management.py` & `onboardme-1.1.5/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/subproc.py` & `onboardme-1.1.5/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/onboardme/sudo_setup.py` & `onboardme-1.1.5/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.4/pyproject.toml` & `onboardme-1.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.4"
+version       = "1.1.5"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.4/PKG-INFO` & `onboardme-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.4
+Version: 1.1.5
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
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.4 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.5 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
```

