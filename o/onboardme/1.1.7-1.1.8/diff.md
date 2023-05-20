# Comparing `tmp/onboardme-1.1.7.tar.gz` & `tmp/onboardme-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.7.tar", max compression
+gzip compressed data, was "onboardme-1.1.8.tar", max compression
```

## Comparing `onboardme-1.1.7.tar` & `onboardme-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.7/LICENSE.txt
--rw-r--r--   0        0        0    14642 2023-05-20 15:55:20.596238 onboardme-1.1.7/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.7/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.7/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.7/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.7/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.7/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.7/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.7/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.7/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.7/onboardme/help_text.py
--rw-r--r--   0        0        0     3111 2023-05-20 18:44:36.719734 onboardme-1.1.7/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.7/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.7/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.7/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.7/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.7/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.7/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-20 18:49:07.003887 onboardme-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    16023 1970-01-01 00:00:00.000000 onboardme-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.8/LICENSE.txt
+-rw-r--r--   0        0        0    14730 2023-05-20 19:55:38.998380 onboardme-1.1.8/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.8/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.8/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.8/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.8/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.8/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.8/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.8/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.8/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.8/onboardme/help_text.py
+-rw-r--r--   0        0        0     3081 2023-05-20 20:09:43.362905 onboardme-1.1.8/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.8/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.8/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.8/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.8/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.8/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.8/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-20 20:05:50.789968 onboardme-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    16111 1970-01-01 00:00:00.000000 onboardme-1.1.8/PKG-INFO
```

### Comparing `onboardme-1.1.7/LICENSE.txt` & `onboardme-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/README.md` & `onboardme-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -294,16 +294,16 @@
 ```
 
 </details>
 
 ## Under the Hood
 Made and tested for these operating systems:
 
-[![Tested on Ventura with an M1 and older generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
-[![Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
+[![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
+[![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
 [![Tested only on ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
 
 And optomized for the following programs:
 
 [![made-with-neovim](https://img.shields.io/badge/NeoVim-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
 [![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 [![made-with-bash](https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
```

#### html2text {}

```diff
@@ -108,19 +108,20 @@
 s dot_files` to get the files that would be overwritten overwrite: false #
 basic package config package: # Remove any of the below pkg managers to only
 run the remaining pkg managers managers: # these are macOS specific steps
 Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
 pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
 install groups: - default # uncomment these to add them as default installed
 package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
+Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
+(https://img.shields.io/badge/mac%20os-000000?style=for-the-
 badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

### Comparing `onboardme-1.1.7/onboardme/__init__.py` & `onboardme-1.1.8/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.8/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/console_logging.py` & `onboardme-1.1.8/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/constants.py` & `onboardme-1.1.8/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/dot_files.py` & `onboardme-1.1.8/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/env_config.py` & `onboardme-1.1.8/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/firewall.py` & `onboardme-1.1.8/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/help_text.py` & `onboardme-1.1.8/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/ide_setup.py` & `onboardme-1.1.8/onboardme/ide_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,12 +74,11 @@
     Installs all plugins and syncs them if needed.
     Runs this command that works via the cli:
         nvim --headless "+Lazy! sync" +qa
     """
     print_header('[green][i]NeoVim[/i][/green] plugins installation '
                  '[dim]and[/dim] upgrades via [green]lazy.nvim[/green]')
 
-    # this didn't error:
-    # subproc(['nvim --headless "+Lazy! sync" +qa'])
-    subproc(['nvim --headless ":Lazy sync" +qa'])
+    subproc(['nvim --headless ":Lazy sync" +qa',
+             'nvim --headless ":TSUpdate" +qa'])
 
     print_sub_header('NeoVim Plugins installed.')
```

### Comparing `onboardme-1.1.7/onboardme/misc.py` & `onboardme-1.1.8/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/pkg_management.py` & `onboardme-1.1.8/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/subproc.py` & `onboardme-1.1.8/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/onboardme/sudo_setup.py` & `onboardme-1.1.8/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.7/pyproject.toml` & `onboardme-1.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.7"
+version       = "1.1.8"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.7/PKG-INFO` & `onboardme-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.7
+Version: 1.1.8
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -324,16 +324,16 @@
 ```
 
 </details>
 
 ## Under the Hood
 Made and tested for these operating systems:
 
-[![Tested on Ventura with an M1 and older generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
-[![Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
+[![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
+[![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
 [![Tested only on ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
 
 And optomized for the following programs:
 
 [![made-with-neovim](https://img.shields.io/badge/NeoVim-0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
 [![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 [![made-with-bash](https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.7 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.8 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -127,19 +127,20 @@
 s dot_files` to get the files that would be overwritten overwrite: false #
 basic package config package: # Remove any of the below pkg managers to only
 run the remaining pkg managers managers: # these are macOS specific steps
 Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
 pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
 install groups: - default # uncomment these to add them as default installed
 package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
+Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
+(https://img.shields.io/badge/mac%20os-000000?style=for-the-
 badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

