# Comparing `tmp/onboardme-1.1.5.tar.gz` & `tmp/onboardme-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.5.tar", max compression
+gzip compressed data, was "onboardme-1.1.6.tar", max compression
```

## Comparing `onboardme-1.1.5.tar` & `onboardme-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.5/LICENSE.txt
--rw-r--r--   0        0        0    12700 2023-05-20 11:41:08.375549 onboardme-1.1.5/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.5/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.5/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.5/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.5/onboardme/console_logging.py
--rw-r--r--   0        0        0     1789 2023-05-20 12:19:03.694838 onboardme-1.1.5/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.5/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.5/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.5/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.5/onboardme/help_text.py
--rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.5/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.5/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.5/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.5/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.5/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.5/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.5/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-20 12:26:05.572037 onboardme-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    14081 1970-01-01 00:00:00.000000 onboardme-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.6/LICENSE.txt
+-rw-r--r--   0        0        0    12869 2023-05-20 13:06:42.792026 onboardme-1.1.6/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.6/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.6/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.6/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.6/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.6/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.6/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.6/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.6/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.6/onboardme/help_text.py
+-rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.6/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.6/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.6/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.6/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.6/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.6/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.6/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-20 13:12:19.025256 onboardme-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14250 1970-01-01 00:00:00.000000 onboardme-1.1.6/PKG-INFO
```

### Comparing `onboardme-1.1.5/LICENSE.txt` & `onboardme-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/README.md` & `onboardme-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -119,25 +119,37 @@
 #### Locally
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
+Linux: source your `.bashrc` like:
+```bash
+# for linux
+source ~/.bashrc
+```
+
+MacOS: source your `.bash_profile` like:
+```bash
+bash
+source ~/.bash_profile
+```
+
 Now you can run `onboardme` 🎉
 ```bash
 # this will display the help text for onboardme
 onboardme --help
 ```
 
 If you've already got brew and Python3.11 on your machine, you can just do:
 
 ```bash
 # should also work with pipx, if you'd like to use that instead
-pip install --user onboardme
+pip install --user --upgrade onboardme
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
 #### Docker
 
 To run the image locally with onboardme installed and already run using default settings:
```

#### html2text {}

```diff
@@ -48,57 +48,59 @@
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
  ## Quick Start ### Installation #### Locally The quickest way to get started
 on a fresh macOS or distro of Debian (including Ubuntu) is: ```bash # this will
 download setup.sh to your current directory and run it /bin/bash -c "$(curl -
 fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ```
-Now you can run `onboardme` ð ```bash # this will display the help text for
-onboardme onboardme --help ``` If you've already got brew and Python3.11 on
+Linux: source your `.bashrc` like: ```bash # for linux source ~/.bashrc ```
+MacOS: source your `.bash_profile` like: ```bash bash source ~/.bash_profile
+``` Now you can run `onboardme` ð ```bash # this will display the help text
+for onboardme onboardme --help ``` If you've already got brew and Python3.11 on
 your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user onboardme ``` You can read more in
-depth at the [Getting Started Docs] ð! There's also more [docs] on basically
-every program that onboardme touches. #### Docker To run the image locally with
-onboardme installed and already run using default settings: ```bash # this
-image is built daily and has already run onboardme with the default settings
-docker run jessebot/onboardme:latest /bin/bash ``` To run the image locally
-with onbaordme installed but _not_ run: ```bash # best if you have your own dot
-files, or need a smaller initial docker image to pull # no packages outside of
-the required pre-reqs for onboardme have been installed docker run jessebot/
-onboardme:no-install /bin/bash ``` ### Upgrades If you're on python 3.11, you
-should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
-Configuration onboardme has lots of CLI options, but you can also use config
-files. You have to create these files for the time being. Config files are in
-`~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples
-below:  ~/.config/onboardme/config.yml ```yaml log: # Full path to a file you'd
-like to log to. Creates file if it doesn't exist file: "" # what level of logs
-to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific
-function in the list of functions we run steps: # these are mac specific steps
-Darwin: # clones dot files into home dir/git fetches updates for dot files -
-dot_files # install packages - packages # adds nerdfonts - font_setup # runs :
-Lazy sync to install all your plugins - neovim_setup # sets up touchID for sudo
-- sudo_setup # these are linux specific steps Linux: - dot_files - packages -
-font_setup - neovim_setup # add your user to the docker group - group_setup
-dot_files: # personal git repo URL for your dot files, defaults to jessebot/
-dot_files git_url: "https://github.com/jessebot/dot_files.git" # the branch to
-use for the git repo above, defaults to main git_branch: "main" # !CAREFUL:
-runs a `git reset --hard`, which will overwite/delete local files in ~ that #
-conflict with the above defined git repo url and branch. You should run #
-`onboardme -s dot_files` to get the files that would be overwritten overwrite:
-false # basic package config package: # Remove any of the below pkg managers to
-only run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+like to use that instead pip install --user --upgrade onboardme ``` You can
+read more in depth at the [Getting Started Docs] ð! There's also more [docs]
+on basically every program that onboardme touches. #### Docker To run the image
+locally with onboardme installed and already run using default settings:
+```bash # this image is built daily and has already run onboardme with the
+default settings docker run jessebot/onboardme:latest /bin/bash ``` To run the
+image locally with onbaordme installed but _not_ run: ```bash # best if you
+have your own dot files, or need a smaller initial docker image to pull # no
+packages outside of the required pre-reqs for onboardme have been installed
+docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
+on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
+onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
+also use config files. You have to create these files for the time being.
+Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
+defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
+path to a file you'd like to log to. Creates file if it doesn't exist file: ""
+# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
+refer to a specific function in the list of functions we run steps: # these are
+mac specific steps Darwin: # clones dot files into home dir/git fetches updates
+for dot files - dot_files # install packages - packages # adds nerdfonts -
+font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
+up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
+dot_files - packages - font_setup - neovim_setup # add your user to the docker
+group - group_setup dot_files: # personal git repo URL for your dot files,
+defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
+dot_files.git" # the branch to use for the git repo above, defaults to main
+git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
+delete local files in ~ that # conflict with the above defined git repo url and
+branch. You should run # `onboardme -s dot_files` to get the files that would
+be overwritten overwrite: false # basic package config package: # Remove any of
+the below pkg managers to only run the remaining pkg managers managers: # these
+are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
+steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
+packages groups to install groups: - default # uncomment these to add them as
+default installed package groups # - gui # - gaming # - devops ```  ## Under
+the Hood Made and tested for these operating systems: [![Tested on Ventura with
+an M1 and older generation](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

### Comparing `onboardme-1.1.5/onboardme/__init__.py` & `onboardme-1.1.6/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.6/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/console_logging.py` & `onboardme-1.1.6/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/constants.py` & `onboardme-1.1.6/onboardme/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,28 +36,28 @@
 # package manager config is different per OS
 PKG_MNGRS = ['brew','pip3.11']
 if OS[0] == 'Linux':
     PKG_MNGRS.extend(['apt','snap','flatpak'])
 
 
 default_dotfiles = ("https://raw.githubusercontent.com/jessebot/dot_files/"
-                    "main/.config/onboardme/config.yml")
+                    "main/.config/onboardme/")
 
 
 def load_cfg(config_file='config.yml') -> dict:
     """
     load yaml config files for onboardme
     """
     config_dir = path.join(xdg_config_home(), 'onboardme')
     config_full_path = path.join(config_dir, config_file)
 
     # create default pathing and config file if it doesn't exist
     if not path.exists(config_full_path):
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         # downloads a default config file from default dot files
-        wget.download(default_dotfiles, config_full_path)
+        wget.download(default_dotfiles + config_file, config_full_path)
 
     with open(config_full_path, 'r') as yaml_file:
         return yaml.safe_load(yaml_file)
 
 
 USR_CONFIG_FILE = load_cfg()
```

### Comparing `onboardme-1.1.5/onboardme/dot_files.py` & `onboardme-1.1.6/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/env_config.py` & `onboardme-1.1.6/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/firewall.py` & `onboardme-1.1.6/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/help_text.py` & `onboardme-1.1.6/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/ide_setup.py` & `onboardme-1.1.6/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/misc.py` & `onboardme-1.1.6/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/pkg_management.py` & `onboardme-1.1.6/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/subproc.py` & `onboardme-1.1.6/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/onboardme/sudo_setup.py` & `onboardme-1.1.6/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.5/pyproject.toml` & `onboardme-1.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.5"
+version       = "1.1.6"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.5/PKG-INFO` & `onboardme-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.5
+Version: 1.1.6
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -149,25 +149,37 @@
 #### Locally
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
+Linux: source your `.bashrc` like:
+```bash
+# for linux
+source ~/.bashrc
+```
+
+MacOS: source your `.bash_profile` like:
+```bash
+bash
+source ~/.bash_profile
+```
+
 Now you can run `onboardme` 🎉
 ```bash
 # this will display the help text for onboardme
 onboardme --help
 ```
 
 If you've already got brew and Python3.11 on your machine, you can just do:
 
 ```bash
 # should also work with pipx, if you'd like to use that instead
-pip install --user onboardme
+pip install --user --upgrade onboardme
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
 #### Docker
 
 To run the image locally with onboardme installed and already run using default settings:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.5 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.6 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -67,57 +67,59 @@
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
  ## Quick Start ### Installation #### Locally The quickest way to get started
 on a fresh macOS or distro of Debian (including Ubuntu) is: ```bash # this will
 download setup.sh to your current directory and run it /bin/bash -c "$(curl -
 fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ```
-Now you can run `onboardme` ð ```bash # this will display the help text for
-onboardme onboardme --help ``` If you've already got brew and Python3.11 on
+Linux: source your `.bashrc` like: ```bash # for linux source ~/.bashrc ```
+MacOS: source your `.bash_profile` like: ```bash bash source ~/.bash_profile
+``` Now you can run `onboardme` ð ```bash # this will display the help text
+for onboardme onboardme --help ``` If you've already got brew and Python3.11 on
 your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user onboardme ``` You can read more in
-depth at the [Getting Started Docs] ð! There's also more [docs] on basically
-every program that onboardme touches. #### Docker To run the image locally with
-onboardme installed and already run using default settings: ```bash # this
-image is built daily and has already run onboardme with the default settings
-docker run jessebot/onboardme:latest /bin/bash ``` To run the image locally
-with onbaordme installed but _not_ run: ```bash # best if you have your own dot
-files, or need a smaller initial docker image to pull # no packages outside of
-the required pre-reqs for onboardme have been installed docker run jessebot/
-onboardme:no-install /bin/bash ``` ### Upgrades If you're on python 3.11, you
-should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
-Configuration onboardme has lots of CLI options, but you can also use config
-files. You have to create these files for the time being. Config files are in
-`~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples
-below:  ~/.config/onboardme/config.yml ```yaml log: # Full path to a file you'd
-like to log to. Creates file if it doesn't exist file: "" # what level of logs
-to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific
-function in the list of functions we run steps: # these are mac specific steps
-Darwin: # clones dot files into home dir/git fetches updates for dot files -
-dot_files # install packages - packages # adds nerdfonts - font_setup # runs :
-Lazy sync to install all your plugins - neovim_setup # sets up touchID for sudo
-- sudo_setup # these are linux specific steps Linux: - dot_files - packages -
-font_setup - neovim_setup # add your user to the docker group - group_setup
-dot_files: # personal git repo URL for your dot files, defaults to jessebot/
-dot_files git_url: "https://github.com/jessebot/dot_files.git" # the branch to
-use for the git repo above, defaults to main git_branch: "main" # !CAREFUL:
-runs a `git reset --hard`, which will overwite/delete local files in ~ that #
-conflict with the above defined git repo url and branch. You should run #
-`onboardme -s dot_files` to get the files that would be overwritten overwrite:
-false # basic package config package: # Remove any of the below pkg managers to
-only run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+like to use that instead pip install --user --upgrade onboardme ``` You can
+read more in depth at the [Getting Started Docs] ð! There's also more [docs]
+on basically every program that onboardme touches. #### Docker To run the image
+locally with onboardme installed and already run using default settings:
+```bash # this image is built daily and has already run onboardme with the
+default settings docker run jessebot/onboardme:latest /bin/bash ``` To run the
+image locally with onbaordme installed but _not_ run: ```bash # best if you
+have your own dot files, or need a smaller initial docker image to pull # no
+packages outside of the required pre-reqs for onboardme have been installed
+docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
+on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
+onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
+also use config files. You have to create these files for the time being.
+Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
+defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
+path to a file you'd like to log to. Creates file if it doesn't exist file: ""
+# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
+refer to a specific function in the list of functions we run steps: # these are
+mac specific steps Darwin: # clones dot files into home dir/git fetches updates
+for dot files - dot_files # install packages - packages # adds nerdfonts -
+font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
+up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
+dot_files - packages - font_setup - neovim_setup # add your user to the docker
+group - group_setup dot_files: # personal git repo URL for your dot files,
+defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
+dot_files.git" # the branch to use for the git repo above, defaults to main
+git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
+delete local files in ~ that # conflict with the above defined git repo url and
+branch. You should run # `onboardme -s dot_files` to get the files that would
+be overwritten overwrite: false # basic package config package: # Remove any of
+the below pkg managers to only run the remaining pkg managers managers: # these
+are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
+steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
+packages groups to install groups: - default # uncomment these to add them as
+default installed package groups # - gui # - gaming # - devops ```  ## Under
+the Hood Made and tested for these operating systems: [![Tested on Ventura with
+an M1 and older generation](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

