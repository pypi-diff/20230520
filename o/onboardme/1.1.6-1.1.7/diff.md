# Comparing `tmp/onboardme-1.1.6.tar.gz` & `tmp/onboardme-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.6.tar", max compression
+gzip compressed data, was "onboardme-1.1.7.tar", max compression
```

## Comparing `onboardme-1.1.6.tar` & `onboardme-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.6/LICENSE.txt
--rw-r--r--   0        0        0    12869 2023-05-20 13:06:42.792026 onboardme-1.1.6/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.6/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.6/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.6/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.6/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.6/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.6/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.6/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.6/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.6/onboardme/help_text.py
--rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.6/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.6/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.6/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.6/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.6/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.6/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.6/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-20 13:12:19.025256 onboardme-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    14250 1970-01-01 00:00:00.000000 onboardme-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.7/LICENSE.txt
+-rw-r--r--   0        0        0    14642 2023-05-20 15:55:20.596238 onboardme-1.1.7/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.7/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.7/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.7/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.7/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.7/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.7/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.7/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.7/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.7/onboardme/help_text.py
+-rw-r--r--   0        0        0     3111 2023-05-20 18:44:36.719734 onboardme-1.1.7/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.7/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.7/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.7/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.7/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.7/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.7/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-20 18:49:07.003887 onboardme-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    16023 1970-01-01 00:00:00.000000 onboardme-1.1.7/PKG-INFO
```

### Comparing `onboardme-1.1.6/LICENSE.txt` & `onboardme-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/README.md` & `onboardme-1.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 </h2>
 <p align="center">
   <a href="https://github.com/jessebot/onboardme/releases">
     <img src="https://img.shields.io/github/v/release/jessebot/onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </p>
 
-Get your daily driver just the way you like it, from dot files installation, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and upgrading your environment.
+Get your daily driver just the way you like it, from dot files management, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and maintaining your personal environments.
 
 ## Features
 
 ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 
 <details>
@@ -58,27 +58,25 @@
   <summary>Why no vim though?</summary>
   
   If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
 
 </details>
 
 ### Easy `yaml` config files
-- [XDG Base Directory Spec] use for [config files](#configuration)
-  - Uses `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/packages.yml`
+[XDG Base Directory Spec] use for [config files](#configuration)
 
 ### Docker image for an on-the-go dev workspace
 
 The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [docker](#docker) section for more info!
 
-### Other useful (but optional) configurations
+### Other optional configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
-- Install nerdfonts (defaults to Hack and Symbols Only)
-- Set capslock to control (🚧 in the works)
+- Install nerdfonts (defaults to mononoki and Symbols Only)
 
 ### Screenshots
 
 <details>
   <summary>Example of <code>onboardme --help</code></summary>
 
 <p align="center" width="100%">
@@ -108,79 +106,130 @@
 
 ### Python virtual env in powerline and cat
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
-## Quick Start
+# Quick Start
 
-### Installation
+### Prereq Installs
+You'll need `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
+
+<details>
+  <summary>Local prereq install script</summary>
 
-#### Locally
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
-Linux: source your `.bashrc` like:
+#### Linux
+Source your updated `.bashrc`:
+
 ```bash
 # for linux
 source ~/.bashrc
 ```
 
-MacOS: source your `.bash_profile` like:
+#### MacOS
+source your updated `.bash_profile`:
+
 ```bash
 bash
 source ~/.bash_profile
 ```
 
-Now you can run `onboardme` 🎉
+You will still have to set your default shell to BASH to if you want to take advantage of the default dot files for onboardme. You can do that like this:
+
 ```bash
-# this will display the help text for onboardme
-onboardme --help
+brew install bash
+sudo -i
+
+# if you're on an M1 or newer:
+echo "/opt/homebrew/bin/bash" >> /etc/shells && exit
+chsh -s /opt/homebrew/bin/bash $(whoami)
+
+# if you're on a mac earlier than the M1:
+echo "/usr/local/bin/bash" >> /etc/shells && exit
+chsh -s /usr/local/bin/bash $(whoami)
 ```
 
-If you've already got brew and Python3.11 on your machine, you can just do:
+After that, you can also set the shell directly in your terminal app via the settings.
 
-```bash
-# should also work with pipx, if you'd like to use that instead
-pip install --user --upgrade onboardme
-```
+</details>
 
-You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
-#### Docker
+<details>
+  <summary><code>jessebot/onboardme</code> docker image</summary>
 
 To run the image locally with onboardme installed and already run using default settings:
+
 ```bash
 # this image is built daily and has already run onboardme with the default settings
 docker run jessebot/onboardme:latest /bin/bash
 ```
 
 To run the image locally with onbaordme installed but _not_ run:
+
 ```bash
 # best if you have your own dot files, or need a smaller initial docker image to pull
 # no packages outside of the required pre-reqs for onboardme have been installed
 docker run jessebot/onboardme:no-install /bin/bash
 ```
 
+</details>
+
+## Install
+
+If you've already got brew and Python3.11 on your machine, you can just do:
+```bash
+# should also work with pipx, if you'd like to use that instead
+pip install --user --upgrade onboardme
+```
+
+## Running commands
+
+_Now_ you can run `onboardme` 🎉 
+```bash
+# this will display the help text for onboardme
+onboardme --help
+
+# Running this won't overwrite any existing dot files, but it may add new ones.
+onboardme
+```
+
+From here, if you want to *completely wipe your existing dot files* for a fresh start with with `onboardme`, you can run:
+```bash
+# WARNING: This will overwrite your local dotfiles, including your .bashrc and .bash_profile
+# can also be done with: onboardme -O
+onboardme --overwrite
+```
+
+You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
+
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
 
 ### Configuration
 onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
 
-Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples below:
+Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
+
+| Config File                               |        Description                                  |
+|:------------------------------------------|:----------------------------------------------------|
+| `$XDG_CONFIG_HOME/onboardme/config.yml`   | For step configuration to run either all steps, or just a subset. | 
+| `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
 
+Examples:
 <details>
 <summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
@@ -305,14 +354,15 @@
 
 Get started with virtual machines and QEMU with [scrap metal](https://github.com/cloudymax/Scrap-Metal).
 
 Get started with testing kubernetes locally, even on metal with [smol k8s lab](https://github.com/jessebot/smol_k8s_lab).
 
 <!-- link references -->
 [documentation]: https://jessebot.github.io/onboardme/onboardme "onboardme documentation"
+[docs]: https://jessebot.github.io/onboardme/onboardme "onboardme documentation"
 [default dot files]: https://github.com/jessebot/dot_files "default dot files for onboardme"
 [help text]: https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/help_text.svg "an svg of the command: onboardme --help"
 [Getting Started Docs]: https://jessebot.github.io/onboardme/onboardme/getting-started "getting started documentation"
 [default packages]: https://github.com/jessebot/dot_files/blob/main/.config/onboardme/packages.yml "default installed packages for onboardme"
 
 <!-- external link references -->
 [dot files]: https://en.wikipedia.org/wiki/Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry for dot file explanation"
```

#### html2text {}

```diff
@@ -1,106 +1,126 @@
   ***** [https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/
    misc/transparent.png] ð» onboardme [https://raw.githubusercontent.com/
          catppuccin/catppuccin/main/assets/misc/transparent.png] *****
               [https://img.shields.io/github/v/release/jessebot/
 onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white]
 GetÂ yourÂ dailyÂ driverÂ justÂ theÂ wayÂ youÂ likeÂ it,Â fromÂ dotÂ files
-installation,Â toÂ packageÂ installation, to other little features you didn't
+management,Â toÂ packageÂ installation, to other little features you didn't
 know you needed,Â `onboardme` intends to save
-youÂ timeÂ withÂ initializingÂ andÂ upgradingÂ yourÂ environment. ## Features
-### Keep your Dot Files Up To Date Across multiple systems `onboardme` can
-manage your [dot files] using a git by turning your home directory into a repo.
-We provide default dot files, so you don't have to manage them - The [default
-dot files] are open source, and the maintainers use these themselves - They
-cover a lot of common apps/tools you probably want anyway - They have
-consistent colorschemes accross different CLI/TUI programs ð - They set all
-the helpful BASH aliases you could need (zsh support coming soon)  ### Package
-management We install and upgrade libraries and apps using common package
-managers.  onboardme provides a currated list of default packages - checkout
-the [default packages] - supports `brew`, `apt`, `snap`, `flatpak`, and `pip`
-(and you can add your own ð) - group together packages for different kinds
-of environments - onboardme provides default package groups: - default (no
-desktop GUI apps installed by default, always installed) - macOS (default apps
-for _macOS only_ apps, always installed on macOS) - gui (default GUI apps for
-Linux desktops, optionally installed) - devops (devops related tooling,
-optionally installed)  ### NeoVim Plugin Installtion and Updates onboardme
-keeps your neovim plugins installed and up to date with [lazy.nvim] under the
-hood.  Why no vim though? If you haven't already made the switch from Vim to
-[NeoVim], you can try out NeoVim today with `onboardme` :D We used to support
-both neovim _and_ vim, but these days none of the primary developers of this
-repo use pure vim anymore, so we can't ensure it's up to standards. All of your
-knowledge from vim is still helpful in neovim though, and we highly recommend
-switching as neovim has a lot more features and a very active plugin community
-:) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/
-doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml` config files - [XDG Base
-Directory Spec] use for [config files](#configuration) - Uses
-`$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/
-packages.yml` ### Docker image for an on-the-go dev workspace The docker image
-is built daily or on push to main. The base image is `debian:bookworm`, but we
-will rollout support for Ubuntu down the line :) See the [docker](#docker)
-section for more info! ### Other useful (but optional) configurations - Enable
-touchID for sudo on macOS - Add your user to the docker group - Install
-nerdfonts (defaults to Hack and Symbols Only) - Set capslock to control (ð§
-in the works) ### Screenshots  Example of onboardme --help
+youÂ timeÂ withÂ initializingÂ andÂ maintainingÂ yourÂ personal environments.
+## Features ### Keep your Dot Files Up To Date Across multiple systems
+`onboardme` can manage your [dot files] using a git by turning your home
+directory into a repo.  We provide default dot files, so you don't have to
+manage them - The [default dot files] are open source, and the maintainers use
+these themselves - They cover a lot of common apps/tools you probably want
+anyway - They have consistent colorschemes accross different CLI/TUI programs
+ð - They set all the helpful BASH aliases you could need (zsh support coming
+soon)  ### Package management We install and upgrade libraries and apps using
+common package managers.  onboardme provides a currated list of default
+packages - checkout the [default packages] - supports `brew`, `apt`, `snap`,
+`flatpak`, and `pip` (and you can add your own ð) - group together packages
+for different kinds of environments - onboardme provides default package
+groups: - default (no desktop GUI apps installed by default, always installed)
+- macOS (default apps for _macOS only_ apps, always installed on macOS) - gui
+(default GUI apps for Linux desktops, optionally installed) - devops (devops
+related tooling, optionally installed)  ### NeoVim Plugin Installtion and
+Updates onboardme keeps your neovim plugins installed and up to date with
+[lazy.nvim] under the hood.  Why no vim though? If you haven't already made the
+switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :
+D We used to support both neovim _and_ vim, but these days none of the primary
+developers of this repo use pure vim anymore, so we can't ensure it's up to
+standards. All of your knowledge from vim is still helpful in neovim though,
+and we highly recommend switching as neovim has a lot more features and a very
+active plugin community :) NeoVim maintains a guide on how to switch from vim
+[here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml`
+config files [XDG Base Directory Spec] use for [config files](#configuration)
+### Docker image for an on-the-go dev workspace The docker image is built daily
+or on push to main. The base image is `debian:bookworm`, but we will rollout
+support for Ubuntu down the line :) See the [docker](#docker) section for more
+info! ### Other optional configurations - Enable touchID for sudo on macOS -
+Add your user to the docker group - Install nerdfonts (defaults to mononoki and
+Symbols Only) ### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- ## Quick Start ### Installation #### Locally The quickest way to get started
-on a fresh macOS or distro of Debian (including Ubuntu) is: ```bash # this will
-download setup.sh to your current directory and run it /bin/bash -c "$(curl -
-fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ```
-Linux: source your `.bashrc` like: ```bash # for linux source ~/.bashrc ```
-MacOS: source your `.bash_profile` like: ```bash bash source ~/.bash_profile
-``` Now you can run `onboardme` ð ```bash # this will display the help text
-for onboardme onboardme --help ``` If you've already got brew and Python3.11 on
+ # Quick Start ### Prereq Installs You'll need `brew`, `git`, and Python 3.11
+to get started. We have a setup script to install those and help you get your
+environment to the XDG spec under Locally or you can just use our docker image,
+[jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).  Local
+prereq install script The quickest way to get started on a fresh macOS or
+distro of Debian (including Ubuntu) is: ```bash # this will download setup.sh
+to your current directory and run it /bin/bash -c "$(curl -fsSL https://
+raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ``` #### Linux
+Source your updated `.bashrc`: ```bash # for linux source ~/.bashrc ``` ####
+MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
+``` You will still have to set your default shell to BASH to if you want to
+take advantage of the default dot files for onboardme. You can do that like
+this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
+opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
+(whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
+>> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
+you can also set the shell directly in your terminal app via the settings.
+jessebot/onboardme docker image To run the image locally with onboardme
+installed and already run using default settings: ```bash # this image is built
+daily and has already run onboardme with the default settings docker run
+jessebot/onboardme:latest /bin/bash ``` To run the image locally with onbaordme
+installed but _not_ run: ```bash # best if you have your own dot files, or need
+a smaller initial docker image to pull # no packages outside of the required
+pre-reqs for onboardme have been installed docker run jessebot/onboardme:no-
+install /bin/bash ```  ## Install If you've already got brew and Python3.11 on
 your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user --upgrade onboardme ``` You can
-read more in depth at the [Getting Started Docs] ð! There's also more [docs]
-on basically every program that onboardme touches. #### Docker To run the image
-locally with onboardme installed and already run using default settings:
-```bash # this image is built daily and has already run onboardme with the
-default settings docker run jessebot/onboardme:latest /bin/bash ``` To run the
-image locally with onbaordme installed but _not_ run: ```bash # best if you
-have your own dot files, or need a smaller initial docker image to pull # no
-packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
-on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
-onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
-also use config files. You have to create these files for the time being.
-Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
-defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
-path to a file you'd like to log to. Creates file if it doesn't exist file: ""
-# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
-refer to a specific function in the list of functions we run steps: # these are
-mac specific steps Darwin: # clones dot files into home dir/git fetches updates
-for dot files - dot_files # install packages - packages # adds nerdfonts -
-font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
-up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
-dot_files - packages - font_setup - neovim_setup # add your user to the docker
-group - group_setup dot_files: # personal git repo URL for your dot files,
-defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
-dot_files.git" # the branch to use for the git repo above, defaults to main
-git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
-delete local files in ~ that # conflict with the above defined git repo url and
-branch. You should run # `onboardme -s dot_files` to get the files that would
-be overwritten overwrite: false # basic package config package: # Remove any of
-the below pkg managers to only run the remaining pkg managers managers: # these
-are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
-steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
-packages groups to install groups: - default # uncomment these to add them as
-default installed package groups # - gui # - gaming # - devops ```  ## Under
-the Hood Made and tested for these operating systems: [![Tested on Ventura with
-an M1 and older generation](https://img.shields.io/badge/mac%20os-
-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
-wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
-badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+like to use that instead pip install --user --upgrade onboardme ``` ## Running
+commands _Now_ you can run `onboardme` ð ```bash # this will display the
+help text for onboardme onboardme --help # Running this won't overwrite any
+existing dot files, but it may add new ones. onboardme ``` From here, if you
+want to *completely wipe your existing dot files* for a fresh start with with
+`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
+dotfiles, including your .bashrc and .bash_profile # can also be done with:
+onboardme -O onboardme --overwrite ``` You can read more in depth at the
+[Getting Started Docs] ð! There's also more [docs] on basically every
+program that onboardme touches. ### Upgrades If you're on python 3.11, you
+should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
+Configuration onboardme has lots of CLI options, but you can also use config
+files. You have to create these files for the time being. Config files are in
+`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
+is not defined. | Config File | Description | |:-------------------------------
+-----------|:----------------------------------------------------| |
+`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
+all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
+For adding packages with different package managers | Examples:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura with an M1 and older
+generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
+A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
@@ -121,16 +141,17 @@
  JesseBot       Max!
  ## Shameless plugs for other projects Get running on a machine using a
 bootable USB stick with [pxeless](https://github.com/cloudymax/pxeless). Get
 started with virtual machines and QEMU with [scrap metal](https://github.com/
 cloudymax/Scrap-Metal). Get started with testing kubernetes locally, even on
 metal with [smol k8s lab](https://github.com/jessebot/smol_k8s_lab).
 [documentation]: https://jessebot.github.io/onboardme/onboardme "onboardme
-documentation" [default dot files]: https://github.com/jessebot/dot_files
-"default dot files for onboardme" [help text]: https://
+documentation" [docs]: https://jessebot.github.io/onboardme/onboardme
+"onboardme documentation" [default dot files]: https://github.com/jessebot/
+dot_files "default dot files for onboardme" [help text]: https://
 raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/
 help_text.svg "an svg of the command: onboardme --help" [Getting Started Docs]:
 https://jessebot.github.io/onboardme/onboardme/getting-started "getting started
 documentation" [default packages]: https://github.com/jessebot/dot_files/blob/
 main/.config/onboardme/packages.yml "default installed packages for onboardme"
 [dot files]: https://en.wikipedia.org/wiki/
 Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry
```

### Comparing `onboardme-1.1.6/onboardme/__init__.py` & `onboardme-1.1.7/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.7/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/console_logging.py` & `onboardme-1.1.7/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/constants.py` & `onboardme-1.1.7/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/dot_files.py` & `onboardme-1.1.7/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/env_config.py` & `onboardme-1.1.7/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/firewall.py` & `onboardme-1.1.7/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/help_text.py` & `onboardme-1.1.7/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/ide_setup.py` & `onboardme-1.1.7/onboardme/ide_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,10 +74,12 @@
     Installs all plugins and syncs them if needed.
     Runs this command that works via the cli:
         nvim --headless "+Lazy! sync" +qa
     """
     print_header('[green][i]NeoVim[/i][/green] plugins installation '
                  '[dim]and[/dim] upgrades via [green]lazy.nvim[/green]')
 
-    subproc(['nvim --headless "+Lazy! sync" +qa'])
+    # this didn't error:
+    # subproc(['nvim --headless "+Lazy! sync" +qa'])
+    subproc(['nvim --headless ":Lazy sync" +qa'])
 
     print_sub_header('NeoVim Plugins installed.')
```

### Comparing `onboardme-1.1.6/onboardme/misc.py` & `onboardme-1.1.7/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/pkg_management.py` & `onboardme-1.1.7/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/subproc.py` & `onboardme-1.1.7/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/onboardme/sudo_setup.py` & `onboardme-1.1.7/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.6/pyproject.toml` & `onboardme-1.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.6"
+version       = "1.1.7"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.6/PKG-INFO` & `onboardme-1.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.6
+Version: 1.1.7
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -43,15 +43,15 @@
 </h2>
 <p align="center">
   <a href="https://github.com/jessebot/onboardme/releases">
     <img src="https://img.shields.io/github/v/release/jessebot/onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white">
   </a>
 </p>
 
-Get your daily driver just the way you like it, from dot files installation, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and upgrading your environment.
+Get your daily driver just the way you like it, from dot files management, to package installation, to other little features you didn't know you needed, `onboardme` intends to save you time with initializing and maintaining your personal environments.
 
 ## Features
 
 ### Keep your Dot Files Up To Date Across multiple systems
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 
 <details>
@@ -88,27 +88,25 @@
   <summary>Why no vim though?</summary>
   
   If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
 
 </details>
 
 ### Easy `yaml` config files
-- [XDG Base Directory Spec] use for [config files](#configuration)
-  - Uses `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/packages.yml`
+[XDG Base Directory Spec] use for [config files](#configuration)
 
 ### Docker image for an on-the-go dev workspace
 
 The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [docker](#docker) section for more info!
 
-### Other useful (but optional) configurations
+### Other optional configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
-- Install nerdfonts (defaults to Hack and Symbols Only)
-- Set capslock to control (🚧 in the works)
+- Install nerdfonts (defaults to mononoki and Symbols Only)
 
 ### Screenshots
 
 <details>
   <summary>Example of <code>onboardme --help</code></summary>
 
 <p align="center" width="100%">
@@ -138,79 +136,130 @@
 
 ### Python virtual env in powerline and cat
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
-## Quick Start
+# Quick Start
 
-### Installation
+### Prereq Installs
+You'll need `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
+
+<details>
+  <summary>Local prereq install script</summary>
 
-#### Locally
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
-Linux: source your `.bashrc` like:
+#### Linux
+Source your updated `.bashrc`:
+
 ```bash
 # for linux
 source ~/.bashrc
 ```
 
-MacOS: source your `.bash_profile` like:
+#### MacOS
+source your updated `.bash_profile`:
+
 ```bash
 bash
 source ~/.bash_profile
 ```
 
-Now you can run `onboardme` 🎉
+You will still have to set your default shell to BASH to if you want to take advantage of the default dot files for onboardme. You can do that like this:
+
 ```bash
-# this will display the help text for onboardme
-onboardme --help
+brew install bash
+sudo -i
+
+# if you're on an M1 or newer:
+echo "/opt/homebrew/bin/bash" >> /etc/shells && exit
+chsh -s /opt/homebrew/bin/bash $(whoami)
+
+# if you're on a mac earlier than the M1:
+echo "/usr/local/bin/bash" >> /etc/shells && exit
+chsh -s /usr/local/bin/bash $(whoami)
 ```
 
-If you've already got brew and Python3.11 on your machine, you can just do:
+After that, you can also set the shell directly in your terminal app via the settings.
 
-```bash
-# should also work with pipx, if you'd like to use that instead
-pip install --user --upgrade onboardme
-```
+</details>
 
-You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
-#### Docker
+<details>
+  <summary><code>jessebot/onboardme</code> docker image</summary>
 
 To run the image locally with onboardme installed and already run using default settings:
+
 ```bash
 # this image is built daily and has already run onboardme with the default settings
 docker run jessebot/onboardme:latest /bin/bash
 ```
 
 To run the image locally with onbaordme installed but _not_ run:
+
 ```bash
 # best if you have your own dot files, or need a smaller initial docker image to pull
 # no packages outside of the required pre-reqs for onboardme have been installed
 docker run jessebot/onboardme:no-install /bin/bash
 ```
 
+</details>
+
+## Install
+
+If you've already got brew and Python3.11 on your machine, you can just do:
+```bash
+# should also work with pipx, if you'd like to use that instead
+pip install --user --upgrade onboardme
+```
+
+## Running commands
+
+_Now_ you can run `onboardme` 🎉 
+```bash
+# this will display the help text for onboardme
+onboardme --help
+
+# Running this won't overwrite any existing dot files, but it may add new ones.
+onboardme
+```
+
+From here, if you want to *completely wipe your existing dot files* for a fresh start with with `onboardme`, you can run:
+```bash
+# WARNING: This will overwrite your local dotfiles, including your .bashrc and .bash_profile
+# can also be done with: onboardme -O
+onboardme --overwrite
+```
+
+You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
+
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
 
 ### Configuration
 onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
 
-Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if defined). Examples below:
+Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
+
+| Config File                               |        Description                                  |
+|:------------------------------------------|:----------------------------------------------------|
+| `$XDG_CONFIG_HOME/onboardme/config.yml`   | For step configuration to run either all steps, or just a subset. | 
+| `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
 
+Examples:
 <details>
 <summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
@@ -335,14 +384,15 @@
 
 Get started with virtual machines and QEMU with [scrap metal](https://github.com/cloudymax/Scrap-Metal).
 
 Get started with testing kubernetes locally, even on metal with [smol k8s lab](https://github.com/jessebot/smol_k8s_lab).
 
 <!-- link references -->
 [documentation]: https://jessebot.github.io/onboardme/onboardme "onboardme documentation"
+[docs]: https://jessebot.github.io/onboardme/onboardme "onboardme documentation"
 [default dot files]: https://github.com/jessebot/dot_files "default dot files for onboardme"
 [help text]: https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/help_text.svg "an svg of the command: onboardme --help"
 [Getting Started Docs]: https://jessebot.github.io/onboardme/onboardme/getting-started "getting started documentation"
 [default packages]: https://github.com/jessebot/dot_files/blob/main/.config/onboardme/packages.yml "default installed packages for onboardme"
 
 <!-- external link references -->
 [dot files]: https://en.wikipedia.org/wiki/Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry for dot file explanation"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.6 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.7 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -19,107 +19,127 @@
 Description-Content-Type: text/markdown
   ***** [https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/
    misc/transparent.png] ð» onboardme [https://raw.githubusercontent.com/
          catppuccin/catppuccin/main/assets/misc/transparent.png] *****
               [https://img.shields.io/github/v/release/jessebot/
 onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white]
 GetÂ yourÂ dailyÂ driverÂ justÂ theÂ wayÂ youÂ likeÂ it,Â fromÂ dotÂ files
-installation,Â toÂ packageÂ installation, to other little features you didn't
+management,Â toÂ packageÂ installation, to other little features you didn't
 know you needed,Â `onboardme` intends to save
-youÂ timeÂ withÂ initializingÂ andÂ upgradingÂ yourÂ environment. ## Features
-### Keep your Dot Files Up To Date Across multiple systems `onboardme` can
-manage your [dot files] using a git by turning your home directory into a repo.
-We provide default dot files, so you don't have to manage them - The [default
-dot files] are open source, and the maintainers use these themselves - They
-cover a lot of common apps/tools you probably want anyway - They have
-consistent colorschemes accross different CLI/TUI programs ð - They set all
-the helpful BASH aliases you could need (zsh support coming soon)  ### Package
-management We install and upgrade libraries and apps using common package
-managers.  onboardme provides a currated list of default packages - checkout
-the [default packages] - supports `brew`, `apt`, `snap`, `flatpak`, and `pip`
-(and you can add your own ð) - group together packages for different kinds
-of environments - onboardme provides default package groups: - default (no
-desktop GUI apps installed by default, always installed) - macOS (default apps
-for _macOS only_ apps, always installed on macOS) - gui (default GUI apps for
-Linux desktops, optionally installed) - devops (devops related tooling,
-optionally installed)  ### NeoVim Plugin Installtion and Updates onboardme
-keeps your neovim plugins installed and up to date with [lazy.nvim] under the
-hood.  Why no vim though? If you haven't already made the switch from Vim to
-[NeoVim], you can try out NeoVim today with `onboardme` :D We used to support
-both neovim _and_ vim, but these days none of the primary developers of this
-repo use pure vim anymore, so we can't ensure it's up to standards. All of your
-knowledge from vim is still helpful in neovim though, and we highly recommend
-switching as neovim has a lot more features and a very active plugin community
-:) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/
-doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml` config files - [XDG Base
-Directory Spec] use for [config files](#configuration) - Uses
-`$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/
-packages.yml` ### Docker image for an on-the-go dev workspace The docker image
-is built daily or on push to main. The base image is `debian:bookworm`, but we
-will rollout support for Ubuntu down the line :) See the [docker](#docker)
-section for more info! ### Other useful (but optional) configurations - Enable
-touchID for sudo on macOS - Add your user to the docker group - Install
-nerdfonts (defaults to Hack and Symbols Only) - Set capslock to control (ð§
-in the works) ### Screenshots  Example of onboardme --help
+youÂ timeÂ withÂ initializingÂ andÂ maintainingÂ yourÂ personal environments.
+## Features ### Keep your Dot Files Up To Date Across multiple systems
+`onboardme` can manage your [dot files] using a git by turning your home
+directory into a repo.  We provide default dot files, so you don't have to
+manage them - The [default dot files] are open source, and the maintainers use
+these themselves - They cover a lot of common apps/tools you probably want
+anyway - They have consistent colorschemes accross different CLI/TUI programs
+ð - They set all the helpful BASH aliases you could need (zsh support coming
+soon)  ### Package management We install and upgrade libraries and apps using
+common package managers.  onboardme provides a currated list of default
+packages - checkout the [default packages] - supports `brew`, `apt`, `snap`,
+`flatpak`, and `pip` (and you can add your own ð) - group together packages
+for different kinds of environments - onboardme provides default package
+groups: - default (no desktop GUI apps installed by default, always installed)
+- macOS (default apps for _macOS only_ apps, always installed on macOS) - gui
+(default GUI apps for Linux desktops, optionally installed) - devops (devops
+related tooling, optionally installed)  ### NeoVim Plugin Installtion and
+Updates onboardme keeps your neovim plugins installed and up to date with
+[lazy.nvim] under the hood.  Why no vim though? If you haven't already made the
+switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :
+D We used to support both neovim _and_ vim, but these days none of the primary
+developers of this repo use pure vim anymore, so we can't ensure it's up to
+standards. All of your knowledge from vim is still helpful in neovim though,
+and we highly recommend switching as neovim has a lot more features and a very
+active plugin community :) NeoVim maintains a guide on how to switch from vim
+[here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml`
+config files [XDG Base Directory Spec] use for [config files](#configuration)
+### Docker image for an on-the-go dev workspace The docker image is built daily
+or on push to main. The base image is `debian:bookworm`, but we will rollout
+support for Ubuntu down the line :) See the [docker](#docker) section for more
+info! ### Other optional configurations - Enable touchID for sudo on macOS -
+Add your user to the docker group - Install nerdfonts (defaults to mononoki and
+Symbols Only) ### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- ## Quick Start ### Installation #### Locally The quickest way to get started
-on a fresh macOS or distro of Debian (including Ubuntu) is: ```bash # this will
-download setup.sh to your current directory and run it /bin/bash -c "$(curl -
-fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ```
-Linux: source your `.bashrc` like: ```bash # for linux source ~/.bashrc ```
-MacOS: source your `.bash_profile` like: ```bash bash source ~/.bash_profile
-``` Now you can run `onboardme` ð ```bash # this will display the help text
-for onboardme onboardme --help ``` If you've already got brew and Python3.11 on
+ # Quick Start ### Prereq Installs You'll need `brew`, `git`, and Python 3.11
+to get started. We have a setup script to install those and help you get your
+environment to the XDG spec under Locally or you can just use our docker image,
+[jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).  Local
+prereq install script The quickest way to get started on a fresh macOS or
+distro of Debian (including Ubuntu) is: ```bash # this will download setup.sh
+to your current directory and run it /bin/bash -c "$(curl -fsSL https://
+raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ``` #### Linux
+Source your updated `.bashrc`: ```bash # for linux source ~/.bashrc ``` ####
+MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
+``` You will still have to set your default shell to BASH to if you want to
+take advantage of the default dot files for onboardme. You can do that like
+this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
+opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
+(whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
+>> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
+you can also set the shell directly in your terminal app via the settings.
+jessebot/onboardme docker image To run the image locally with onboardme
+installed and already run using default settings: ```bash # this image is built
+daily and has already run onboardme with the default settings docker run
+jessebot/onboardme:latest /bin/bash ``` To run the image locally with onbaordme
+installed but _not_ run: ```bash # best if you have your own dot files, or need
+a smaller initial docker image to pull # no packages outside of the required
+pre-reqs for onboardme have been installed docker run jessebot/onboardme:no-
+install /bin/bash ```  ## Install If you've already got brew and Python3.11 on
 your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user --upgrade onboardme ``` You can
-read more in depth at the [Getting Started Docs] ð! There's also more [docs]
-on basically every program that onboardme touches. #### Docker To run the image
-locally with onboardme installed and already run using default settings:
-```bash # this image is built daily and has already run onboardme with the
-default settings docker run jessebot/onboardme:latest /bin/bash ``` To run the
-image locally with onbaordme installed but _not_ run: ```bash # best if you
-have your own dot files, or need a smaller initial docker image to pull # no
-packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
-on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
-onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
-also use config files. You have to create these files for the time being.
-Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
-defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
-path to a file you'd like to log to. Creates file if it doesn't exist file: ""
-# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
-refer to a specific function in the list of functions we run steps: # these are
-mac specific steps Darwin: # clones dot files into home dir/git fetches updates
-for dot files - dot_files # install packages - packages # adds nerdfonts -
-font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
-up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
-dot_files - packages - font_setup - neovim_setup # add your user to the docker
-group - group_setup dot_files: # personal git repo URL for your dot files,
-defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
-dot_files.git" # the branch to use for the git repo above, defaults to main
-git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
-delete local files in ~ that # conflict with the above defined git repo url and
-branch. You should run # `onboardme -s dot_files` to get the files that would
-be overwritten overwrite: false # basic package config package: # Remove any of
-the below pkg managers to only run the remaining pkg managers managers: # these
-are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
-steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
-packages groups to install groups: - default # uncomment these to add them as
-default installed package groups # - gui # - gaming # - devops ```  ## Under
-the Hood Made and tested for these operating systems: [![Tested on Ventura with
-an M1 and older generation](https://img.shields.io/badge/mac%20os-
-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
-wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
-badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+like to use that instead pip install --user --upgrade onboardme ``` ## Running
+commands _Now_ you can run `onboardme` ð ```bash # this will display the
+help text for onboardme onboardme --help # Running this won't overwrite any
+existing dot files, but it may add new ones. onboardme ``` From here, if you
+want to *completely wipe your existing dot files* for a fresh start with with
+`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
+dotfiles, including your .bashrc and .bash_profile # can also be done with:
+onboardme -O onboardme --overwrite ``` You can read more in depth at the
+[Getting Started Docs] ð! There's also more [docs] on basically every
+program that onboardme touches. ### Upgrades If you're on python 3.11, you
+should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
+Configuration onboardme has lots of CLI options, but you can also use config
+files. You have to create these files for the time being. Config files are in
+`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
+is not defined. | Config File | Description | |:-------------------------------
+-----------|:----------------------------------------------------| |
+`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
+all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
+For adding packages with different package managers | Examples:  ~/.config/
+onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
+Creates file if it doesn't exist file: "" # what level of logs to output
+(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
+in the list of functions we run steps: # these are mac specific steps Darwin: #
+clones dot files into home dir/git fetches updates for dot files - dot_files #
+install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
+install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
+# these are linux specific steps Linux: - dot_files - packages - font_setup -
+neovim_setup # add your user to the docker group - group_setup dot_files: #
+personal git repo URL for your dot files, defaults to jessebot/dot_files
+git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
+the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
+reset --hard`, which will overwite/delete local files in ~ that # conflict with
+the above defined git repo url and branch. You should run # `onboardme -
+s dot_files` to get the files that would be overwritten overwrite: false #
+basic package config package: # Remove any of the below pkg managers to only
+run the remaining pkg managers managers: # these are macOS specific steps
+Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
+pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
+install groups: - default # uncomment these to add them as default installed
+package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
+tested for these operating systems: [![Tested on Ventura with an M1 and older
+generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
+badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
+[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
+A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
@@ -140,16 +160,17 @@
  JesseBot       Max!
  ## Shameless plugs for other projects Get running on a machine using a
 bootable USB stick with [pxeless](https://github.com/cloudymax/pxeless). Get
 started with virtual machines and QEMU with [scrap metal](https://github.com/
 cloudymax/Scrap-Metal). Get started with testing kubernetes locally, even on
 metal with [smol k8s lab](https://github.com/jessebot/smol_k8s_lab).
 [documentation]: https://jessebot.github.io/onboardme/onboardme "onboardme
-documentation" [default dot files]: https://github.com/jessebot/dot_files
-"default dot files for onboardme" [help text]: https://
+documentation" [docs]: https://jessebot.github.io/onboardme/onboardme
+"onboardme documentation" [default dot files]: https://github.com/jessebot/
+dot_files "default dot files for onboardme" [help text]: https://
 raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/
 help_text.svg "an svg of the command: onboardme --help" [Getting Started Docs]:
 https://jessebot.github.io/onboardme/onboardme/getting-started "getting started
 documentation" [default packages]: https://github.com/jessebot/dot_files/blob/
 main/.config/onboardme/packages.yml "default installed packages for onboardme"
 [dot files]: https://en.wikipedia.org/wiki/
 Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry
```

