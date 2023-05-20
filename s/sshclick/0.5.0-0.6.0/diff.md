# Comparing `tmp/sshclick-0.5.0.tar.gz` & `tmp/sshclick-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshclick-0.5.0.tar", max compression
+gzip compressed data, was "sshclick-0.6.0.tar", max compression
```

## Comparing `sshclick-0.5.0.tar` & `sshclick-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1068 2023-04-17 16:09:18.391084 sshclick-0.5.0/LICENSE
--rw-r--r--   0        0        0    14399 2023-04-17 16:08:59.411089 sshclick-0.5.0/README.md
--rw-r--r--   0        0        0     1037 2023-04-17 13:22:02.913713 sshclick-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-10 13:49:51.835727 sshclick-0.5.0/sshclick/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/__init__.py
--rw-r--r--   0        0        0      455 2023-04-17 12:52:26.614177 sshclick-0.5.0/sshclick/cmds/cmd_config.py
--rw-r--r--   0        0        0      646 2022-08-10 20:50:38.844620 sshclick-0.5.0/sshclick/cmds/cmd_group.py
--rw-r--r--   0        0        0      732 2023-04-14 15:17:18.853394 sshclick-0.5.0/sshclick/cmds/cmd_host.py
--rw-r--r--   0        0        0        0 2023-04-17 12:48:49.004234 sshclick-0.5.0/sshclick/cmds/config/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-17 12:59:37.314064 sshclick-0.5.0/sshclick/cmds/config/config_del.py
--rw-r--r--   0        0        0     1354 2023-04-17 12:59:34.824065 sshclick-0.5.0/sshclick/cmds/config/config_set.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/group/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-14 13:48:55.874783 sshclick-0.5.0/sshclick/cmds/group/group_create.py
--rw-r--r--   0        0        0     2217 2023-04-14 13:45:08.024842 sshclick-0.5.0/sshclick/cmds/group/group_delete.py
--rw-r--r--   0        0        0     1068 2022-09-11 17:04:13.785725 sshclick-0.5.0/sshclick/cmds/group/group_list.py
--rw-r--r--   0        0        0     1196 2023-04-14 14:12:19.544415 sshclick-0.5.0/sshclick/cmds/group/group_rename.py
--rw-r--r--   0        0        0     2421 2023-04-14 13:49:04.844781 sshclick-0.5.0/sshclick/cmds/group/group_set.py
--rw-r--r--   0        0        0     2387 2023-04-17 09:36:07.926863 sshclick-0.5.0/sshclick/cmds/group/group_show.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/host/__init__.py
--rw-r--r--   0        0        0     3970 2023-04-14 14:07:21.804493 sshclick-0.5.0/sshclick/cmds/host/host_create.py
--rw-r--r--   0        0        0     2458 2023-04-14 14:08:54.144468 sshclick-0.5.0/sshclick/cmds/host/host_delete.py
--rw-r--r--   0        0        0     1715 2023-04-17 09:39:36.716809 sshclick-0.5.0/sshclick/cmds/host/host_install_key.py
--rw-r--r--   0        0        0     4494 2023-04-17 10:02:52.786444 sshclick-0.5.0/sshclick/cmds/host/host_list.py
--rw-r--r--   0        0        0     1162 2023-04-14 14:12:44.404409 sshclick-0.5.0/sshclick/cmds/host/host_rename.py
--rw-r--r--   0        0        0     6579 2023-04-14 14:19:27.594303 sshclick-0.5.0/sshclick/cmds/host/host_set.py
--rw-r--r--   0        0        0     3005 2023-04-17 12:43:47.674312 sshclick-0.5.0/sshclick/cmds/host/host_show.py
--rw-r--r--   0        0        0     1581 2023-04-14 13:45:33.234835 sshclick-0.5.0/sshclick/cmds/host/host_test.py
--rw-r--r--   0        0        0      107 2023-04-17 12:21:37.064660 sshclick-0.5.0/sshclick/globals.py
--rw-r--r--   0        0        0     1891 2023-04-17 13:24:55.183668 sshclick-0.5.0/sshclick/main.py
--rw-r--r--   0        0        0      411 2023-04-17 12:19:51.954689 sshclick-0.5.0/sshclick/sshc/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/__init__.py
--rw-r--r--   0        0        0     2312 2022-09-11 16:36:02.105733 sshclick-0.5.0/sshclick/sshc/host_styles/card.py
--rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/json.py
--rw-r--r--   0        0        0     2484 2023-04-17 09:57:40.316526 sshclick-0.5.0/sshclick/sshc/host_styles/panels.py
--rw-r--r--   0        0        0     2262 2022-09-11 16:56:01.465727 sshclick-0.5.0/sshclick/sshc/host_styles/simple.py
--rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/table.py
--rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/table2.py
--rw-r--r--   0        0        0    16226 2023-04-17 12:19:45.224691 sshclick-0.5.0/sshclick/sshc/ssh_config.py
--rw-r--r--   0        0        0      434 2023-04-17 08:39:08.357758 sshclick-0.5.0/sshclick/sshc/ssh_group.py
--rw-r--r--   0        0        0     1447 2023-04-17 12:19:06.094701 sshclick-0.5.0/sshclick/sshc/ssh_host.py
--rw-r--r--   0        0        0     4555 2023-04-17 12:20:45.644673 sshclick-0.5.0/sshclick/sshc/ssh_parameters.py
--rw-r--r--   0        0        0     4082 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/sshextras.py
--rw-r--r--   0        0        0     4842 2023-04-17 12:22:18.274649 sshclick-0.5.0/sshclick/sshc/sshutils.py
--rw-r--r--   0        0        0    15497 1970-01-01 00:00:00.000000 sshclick-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-17 16:09:18.391084 sshclick-0.6.0/LICENSE
+-rw-r--r--   0        0        0    17480 2023-05-20 18:57:10.639154 sshclick-0.6.0/README.md
+-rw-r--r--   0        0        0     1065 2023-05-20 16:44:37.720951 sshclick-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-10 13:49:51.835727 sshclick-0.6.0/sshclick/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-17 12:52:26.614177 sshclick-0.6.0/sshclick/cmds/cmd_config.py
+-rw-r--r--   0        0        0      646 2022-08-10 20:50:38.844620 sshclick-0.6.0/sshclick/cmds/cmd_group.py
+-rw-r--r--   0        0        0      732 2023-04-14 15:17:18.853394 sshclick-0.6.0/sshclick/cmds/cmd_host.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:48:49.004234 sshclick-0.6.0/sshclick/cmds/config/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-17 12:59:37.314064 sshclick-0.6.0/sshclick/cmds/config/config_del.py
+-rw-r--r--   0        0        0     1354 2023-04-17 12:59:34.824065 sshclick-0.6.0/sshclick/cmds/config/config_set.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/group/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-14 13:48:55.874783 sshclick-0.6.0/sshclick/cmds/group/group_create.py
+-rw-r--r--   0        0        0     2217 2023-04-14 13:45:08.024842 sshclick-0.6.0/sshclick/cmds/group/group_delete.py
+-rw-r--r--   0        0        0     1068 2022-09-11 17:04:13.785725 sshclick-0.6.0/sshclick/cmds/group/group_list.py
+-rw-r--r--   0        0        0     1196 2023-04-14 14:12:19.544415 sshclick-0.6.0/sshclick/cmds/group/group_rename.py
+-rw-r--r--   0        0        0     2421 2023-04-14 13:49:04.844781 sshclick-0.6.0/sshclick/cmds/group/group_set.py
+-rw-r--r--   0        0        0     2387 2023-04-17 09:36:07.926863 sshclick-0.6.0/sshclick/cmds/group/group_show.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/cmds/host/__init__.py
+-rw-r--r--   0        0        0     3970 2023-05-20 19:07:30.759013 sshclick-0.6.0/sshclick/cmds/host/host_create.py
+-rw-r--r--   0        0        0     2458 2023-04-14 14:08:54.144468 sshclick-0.6.0/sshclick/cmds/host/host_delete.py
+-rw-r--r--   0        0        0     1715 2023-04-17 09:39:36.716809 sshclick-0.6.0/sshclick/cmds/host/host_install_key.py
+-rw-r--r--   0        0        0     4494 2023-04-30 10:40:52.857020 sshclick-0.6.0/sshclick/cmds/host/host_list.py
+-rw-r--r--   0        0        0     1162 2023-04-14 14:12:44.404409 sshclick-0.6.0/sshclick/cmds/host/host_rename.py
+-rw-r--r--   0        0        0     6579 2023-04-14 14:19:27.594303 sshclick-0.6.0/sshclick/cmds/host/host_set.py
+-rw-r--r--   0        0        0     2997 2023-04-26 13:53:34.694329 sshclick-0.6.0/sshclick/cmds/host/host_show.py
+-rw-r--r--   0        0        0     2699 2023-05-20 16:34:15.411092 sshclick-0.6.0/sshclick/cmds/host/host_test.py
+-rw-r--r--   0        0        0      107 2023-04-17 12:21:37.064660 sshclick-0.6.0/sshclick/globals.py
+-rw-r--r--   0        0        0     2535 2023-05-20 18:56:47.529159 sshclick-0.6.0/sshclick/main.py
+-rw-r--r--   0        0        0     7832 2023-05-20 18:54:22.169193 sshclick-0.6.0/sshclick/main_tui.py
+-rw-r--r--   0        0        0      411 2023-04-26 14:19:59.943911 sshclick-0.6.0/sshclick/sshc/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/__init__.py
+-rw-r--r--   0        0        0     2312 2022-09-11 16:36:02.105733 sshclick-0.6.0/sshclick/sshc/host_styles/card.py
+-rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/json.py
+-rw-r--r--   0        0        0     2484 2023-04-17 09:57:40.316526 sshclick-0.6.0/sshclick/sshc/host_styles/panels.py
+-rw-r--r--   0        0        0     2262 2022-09-11 16:56:01.465727 sshclick-0.6.0/sshclick/sshc/host_styles/simple.py
+-rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/table.py
+-rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.6.0/sshclick/sshc/host_styles/table2.py
+-rw-r--r--   0        0        0    16709 2023-05-20 19:15:16.358913 sshclick-0.6.0/sshclick/sshc/ssh_config.py
+-rw-r--r--   0        0        0     4516 2023-04-26 17:00:52.291382 sshclick-0.6.0/sshclick/sshc/ssh_graph.py
+-rw-r--r--   0        0        0      434 2023-04-17 08:39:08.357758 sshclick-0.6.0/sshclick/sshc/ssh_group.py
+-rw-r--r--   0        0        0     2627 2023-05-01 10:12:53.391675 sshclick-0.6.0/sshclick/sshc/ssh_host.py
+-rw-r--r--   0        0        0     4555 2023-04-17 12:20:45.644673 sshclick-0.6.0/sshclick/sshc/ssh_parameters.py
+-rw-r--r--   0        0        0     4842 2023-04-17 12:22:18.274649 sshclick-0.6.0/sshclick/sshc/sshutils.py
+-rw-r--r--   0        0        0       17 2023-05-20 16:19:03.191299 sshclick-0.6.0/sshclick/version.py
+-rw-r--r--   0        0        0    18324 1970-01-01 00:00:00.000000 sshclick-0.6.0/PKG-INFO
```

### Comparing `sshclick-0.5.0/LICENSE` & `sshclick-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/README.md` & `sshclick-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,52 +11,54 @@
   - [Upgrade procedure](https://github.com/karlot/sshclick#upgrade-procedure)
   - [Uninstall procedure](https://github.com/karlot/sshclick#uninstall-procedure)
 - [SSH Config structure](https://github.com/karlot/sshclick#ssh-config-structure-and-important-note-about-comments)
   - [Comment blocks and metadata](https://github.com/karlot/sshclick#comment-blocks-and-metadata-in-ssh-config)
 - [Example usage and features](https://github.com/karlot/sshclick#example-usage-and-features)
   - [Group commands and options](https://github.com/karlot/sshclick#group-commands-and-options)
   - [Host commands and options](https://github.com/karlot/sshclick#host-commands-and-options)
+  - [Config commands and options](https://github.com/karlot/sshclick#config-commands-and-sshclick-configuration-options)
   - [Output styling and user ENV variables](https://github.com/karlot/sshclick#output-styling-and-user-env-variables)
-- [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)
+<!-- - [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)
   - [sshc group operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-group-operations)
-  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations)
+  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations) -->
 - [Author](https://github.com/karlot/sshclick#author)
 - [License](https://github.com/karlot/sshclick#license)
 
 
 ## Intro
 Terminal based assisted management of your SSH config files.  
 Built out of boredom with managing messy and huge ssh_config files.  
 
-EARLY VERSION, backup your SSH config files before using!  
-SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config!  
+Backup your SSH config files before using!  
+SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config in any way!  
 
 **Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**
 
+**NEW!** *Now comes with additional TUI that can be accessed via `sshc tui` or `ssht`.*  
+
+![splash_gif](tapes/sshc_tui_example.svg)
+
+
 ## Why?
 
-What am I trying to solve with this tool?
 * I need something that works fast and great in terminal, and does not require complex setup.
-* Managing some other configuration files that renders to SSH config is extra step that I don't like.
-* SSH config is already feature-full with all options SSH client support, why inventing extra layer?
 * SSH config is the only config I need to backup.
+* SSH config is very feature-full with all options SSH client support, why inventing extra layer?
 * I need quick way to search, group and visualize all hosts inside SSH configuration (especially since it can grow huge)
 
 
 ## What does it do?
 
 SSHClick (sshc) is just a tool designed to work with existing SSH configuration files on your Linux/Windows/WSL terminal environment.  
-It basically parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.
-Trough additional "magic" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.
+It parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.
+Trough additional "metadata" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.
 
 
 ### Installation procedure
 
-Should be straight forward...  
-
 1. **Check preconditions:**
     - Currently only tested on Linux (Debian 10,11, Ubuntu 20.04,22.04), but should work on other systems as well
     - Minimum python3.7 (tested up to 3.11 beta) & pip installed
         - it is preferable to not use system python version, to install "custom" user python on linux, you can try using pyenv (https://github.com/pyenv/pyenv
     - git installed
 
 2. **Install package:**
@@ -159,27 +161,27 @@
 SSHClick is deploying `sshc` cli tool that allows interacting with your SSH Config file and perform various organization,listing, displaying and modification of SSH Group/Host configuration parameters.  
 `sshc` comes with pre-built lots of help options so each level of commands provide `--help` options to provide you info what commands and options are available at which command level.  
 
 For example to check version, type: `sshc --version`  
 _Sample output:_
 ```console
 $ sshc --version
-SSHClick (sshc) - Version: 0.5.0
+SSHClick (sshc) - Version: 0.6.0
 ```
 
 If you run `sshc` command alone, or adding `-h` or `--help` option, it will show help what else must be added to the command...  
 _Example:_
 ```console
 $ sshc --help
 Usage: sshc [OPTIONS] COMMAND [ARGS]...
 
-  SSHClick - SSH Config manager. version 0.5.0
+  SSHClick - SSH Config manager. version 0.6.0
 
-  NOTE: As this is early alpha, backup your SSH config files before this
-  software, as you might accidentally lose some configuration
+  NOTE: As this will change your SSH config files, make backups before using
+  this software, as you might accidentally lose some configuration.
 
 Options:
   --sshconfig TEXT  Config file (default: ~/.ssh/config)
   --stdout          Send changed SSH config to STDOUT instead to original
                     file, can be enabled with setting ENV variable (export
                     SSHC_STDOUT=1)
   --version         Show the version and exit.
@@ -187,21 +189,21 @@
 
 Commands:
   config  Modify SSHClick configuration trough SSH Config
   group   Command group for managing groups
   groups  Lists all groups
   host    Command group for managing hosts
   hosts   List configured hosts
+  tui     TUI Interface (experimental)
 ```
 
-
 ### `group` commands and options
 
 To manage "groups" type `sshc group --help` to see options.  
-_example:_
+_Example:_
 ```console
 $ sshc group --help
 Usage: sshc group [OPTIONS] COMMAND [ARGS]...
 
   Command group for managing groups
 
 Options:
@@ -215,15 +217,15 @@
   set     Change group parameters
   show    Shows group details
 ```
 
 ### `host` commands and options
 
 To manage "groups" type `sshc host --help` to see options.  
-_example:_
+_Example:_
 ```console
 $ sshc host --help
 Usage: sshc host [OPTIONS] COMMAND [ARGS]...
 
   Command group for managing hosts
 
 Options:
@@ -236,29 +238,83 @@
   list     List configured hosts
   rename   Rename existing host
   set      Set/Change host configuration
   show     Show current host configuration
   test     Test SSH host connection  (experimental)
 ```
 
+### `config` commands and SSHClick configuration options
+
+SSHClick does not to have its own configuration files, so most of configuration that it tries to understand, come from commands arguments/options, environment variables, and SSH Config file itself.
+
+Sometimes when you want to persist some config options, not to repeat it via command, you can use ENV variables, that can be set trough user shell profile.
+
+Now there is also option to store such config in SSH Config file itself (as metadata comment), so it can be portable and backed up together with SSH Config file.
+
+Command `config` takes `set` or `del` commands that add or remove specific configuration.
+
+_Example:_
+```console
+$ sshc config --help
+Usage: sshc config [OPTIONS] COMMAND [ARGS]...
+
+  Modify SSHClick configuration trough SSH Config
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  del  Delete config option
+  set  Set config option
+```
+
+
+_Example: "Set host output style to 'card'"_
+```console
+$ sshc config set --help
+Usage: sshc config set [OPTIONS]
+
+  Set config option
+
+Options:
+  --host-style TEXT  Set how to display hosts in 'show' command.
+                     Available:(panels,card,simple,table,table2,json)
+                     (default: panels)
+  -h, --help         Show this message and exit.
+
+$ sshc config set --host-style card
+```
+
+This will now store config in "currently used" SSH config file as following:
+```
+#<<<<< SSH Config file managed by sshclick >>>>>
+#@config: host-style=card
+```
+
+To delete this config, either remove the line from file manually, or use `sshc` command:
+```console
+$ sshc config del --host-style
+```
+
 ### Output styling and user ENV variables
 
 `sshc host show` can display host output is several formats, you can specify it with `sshc host show <host> --style <style>`  
 Available styles are:
 
 | Style              | Description                                       |
 |--------------------|---------------------------------------------------|
 | `panels` (default) | Display data in several panels                    |
 | `card`             | Add data to single "card"                         |
 | `simple`           | Simple output with minimal decorations            |
 | `table`            | Flat table with 3 columns                         |
 | `table2`           | Nested table with separated host SSH params       |
-| `json`             | JSON output, useful for binding with other tools |
+| `json`             | JSON output, useful for binding with other tools  |
 
-If you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.
+If you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.  
+Alternatively, you can use SSHClick internal "config" mechanism to store some config data into your SSH Config file (as commented metadata) so it can be backed up with your SSH config. To do so, you can use following command as example: `sshc config set --host-style table`.
 
 In case user do not line "fancy" colors in output, you can set ENV variable to disable all color outputs with `export NO_COLOR=1`. If you want it permanently you can add it to startup "rc" files as well.
 
 
 > NOTE! When sending output into non-terminal such as to file, SSHClick will recognize that and will remove all ANSI Escape characters (colors and stuff...) so that output is captured in clear way.
 
 
@@ -349,10 +405,28 @@
 Karlo Tisaj  
 email: karlot@gmail.com  
 github: https://github.com/karlot
 
 
 ## License
 
-[MIT License](LICENSE)
+MIT License
 
+Copyright (c) 2023 Karlo Tisaj
 
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sshclick-0.5.0/pyproject.toml` & `sshclick-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !!! Remember to update version here and in the code !!! 
 # (ಠ_ಠ)  -- I wish poetry could just read version from the package
 
 [tool.poetry]
 name = "sshclick"
 homepage = "https://github.com/karlot/sshclick"
-version = "0.5.0"
+version = "0.6.0"
 description = "SSH Config manager"
 authors = ["Karlo Tisaj <karlot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -21,22 +21,23 @@
     "License :: OSI Approved :: MIT License",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1"
-prettytable = "^3.7"
 rich = "^13.3"
+textual = "^0.26"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 
 
 [tool.poetry.scripts]
 sshc = "sshclick.main:cli"
+ssht = "sshclick.main_tui:tui"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sshclick-0.5.0/sshclick/cmds/cmd_group.py` & `sshclick-0.6.0/sshclick/cmds/cmd_group.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/cmd_host.py` & `sshclick-0.6.0/sshclick/cmds/cmd_host.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/config/config_del.py` & `sshclick-0.6.0/sshclick/cmds/config/config_del.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/config/config_set.py` & `sshclick-0.6.0/sshclick/cmds/config/config_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_create.py` & `sshclick-0.6.0/sshclick/cmds/group/group_create.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_delete.py` & `sshclick-0.6.0/sshclick/cmds/group/group_delete.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_list.py` & `sshclick-0.6.0/sshclick/cmds/group/group_list.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_rename.py` & `sshclick-0.6.0/sshclick/cmds/group/group_rename.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_set.py` & `sshclick-0.6.0/sshclick/cmds/group/group_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/group/group_show.py` & `sshclick-0.6.0/sshclick/cmds/group/group_show.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_create.py` & `sshclick-0.6.0/sshclick/cmds/host/host_create.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_delete.py` & `sshclick-0.6.0/sshclick/cmds/host/host_delete.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_install_key.py` & `sshclick-0.6.0/sshclick/cmds/host/host_install_key.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_list.py` & `sshclick-0.6.0/sshclick/cmds/host/host_list.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_rename.py` & `sshclick-0.6.0/sshclick/cmds/host/host_rename.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_set.py` & `sshclick-0.6.0/sshclick/cmds/host/host_set.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/cmds/host/host_show.py` & `sshclick-0.6.0/sshclick/cmds/host/host_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     traced_hosts = trace_jumphosts(name, config, ctx, style)
 
     # Normal show, no linked graphs needed
     console.print(traced_hosts[0])
 
     #TODO: Make better graph output
     if graph:
-        console.print("\n", generate_graph(traced_hosts), "\n")
+        console.print(generate_graph(traced_hosts), "")
```

### Comparing `sshclick-0.5.0/sshclick/main.py` & `sshclick-0.6.0/sshclick/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,60 @@
-__version__ = "0.5.0"
-
+from .version import VERSION
 import click
 import os.path
 from .sshc import SSH_Config
 
 # Setup click to use both short and long help option
 USER_SSH_CONFIG   = "~/.ssh/config"
 CONTEXT_SETTINGS  = dict(help_option_names=['-h', '--help'])
-DEFAULT_USER_CONF = os.path.expanduser(USER_SSH_CONFIG)
 
 #------------------------------------------------------------------------------
 # COMMAND: sshc
 #------------------------------------------------------------------------------
 MAIN_HELP = f"""
-SSHClick - SSH Config manager. version {__version__}
+SSHClick - SSH Config manager. version {VERSION}
 
-NOTE: As this is early alpha, backup your SSH config files before
-this software, as you might accidentally lose some configuration
+NOTE: As this will change your SSH config files, make backups before
+using this software, as you might accidentally lose some configuration.
 """
 
 # Parameters help:
 SSHCONFIG_HELP = f"Config file (default: {USER_SSH_CONFIG})"
 STDOUT_HELP    =  "Send changed SSH config to STDOUT instead to original file, can be enabled with setting ENV variable (export SSHC_STDOUT=1)"
 #------------------------------------------------------------------------------
 
+# In cases we want to have some execution without any sub-commands, instead of displaying help
+# we can add "invoke_without_command=True" in a group decorator, to make function runnable directly
 @click.group(context_settings=CONTEXT_SETTINGS, help=MAIN_HELP)
-@click.option("--sshconfig", default=DEFAULT_USER_CONF, envvar="SSHC_SSHCONFIG", help=SSHCONFIG_HELP)
-@click.option("--stdout",    is_flag=True,              envvar="SSHC_STDOUT",    help=STDOUT_HELP)
-@click.version_option(__version__, message="SSHClick (sshc) - Version: %(version)s")
+@click.option("--sshconfig", default=USER_SSH_CONFIG, envvar="SSHC_SSHCONFIG", help=SSHCONFIG_HELP)
+@click.option("--stdout",    is_flag=True,            envvar="SSHC_STDOUT",    help=STDOUT_HELP)
+@click.version_option(VERSION, message="SSHClick (sshc) - Version: %(version)s")
 @click.pass_context
 def cli(ctx: click.core.Context, sshconfig: str, stdout: bool):
-    ctx.obj = SSH_Config(file=sshconfig, stdout=stdout).read().parse()
+    ctx.obj = SSH_Config(file=os.path.expanduser(sshconfig), stdout=stdout).read().parse()
+
 
+# Add experimental TUI
+from .main_tui import SSHTui
+TUI_SHORT_HELP = "TUI Interface (experimental)"
+TUI_HELP       = "Experimental TUI interface for interacting with SSH Configuration"
+@click.command(name="tui", short_help=TUI_SHORT_HELP, help=TUI_HELP)
+@click.pass_context
+def tui_cmd(ctx: click.core.Context):
+    SSHTui(ctx.obj).run()
 
+
+# Link all commands to root command
+#------------------------------------------------------------------------------
 # Top commands
 from .cmds import cmd_group, cmd_host, cmd_config
 cli.add_command(cmd_host.ssh_host)
 cli.add_command(cmd_group.ssh_group)
 cli.add_command(cmd_config.ssh_config)
+cli.add_command(tui_cmd)
 
 # Top level aliases (groups --> group list, hosts --> host list, etc..)
 from .cmds.cmd_group import group_list
 cli.add_command(group_list.cmd, "groups")
 
 from .cmds.cmd_host import host_list
 cli.add_command(host_list.cmd, "hosts")
```

### Comparing `sshclick-0.5.0/sshclick/sshc/host_styles/card.py` & `sshclick-0.6.0/sshclick/sshc/host_styles/card.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/host_styles/panels.py` & `sshclick-0.6.0/sshclick/sshc/host_styles/panels.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/host_styles/simple.py` & `sshclick-0.6.0/sshclick/sshc/host_styles/simple.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/host_styles/table.py` & `sshclick-0.6.0/sshclick/sshc/host_styles/table.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/host_styles/table2.py` & `sshclick-0.6.0/sshclick/sshc/host_styles/table2.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/ssh_config.py` & `sshclick-0.6.0/sshclick/sshc/ssh_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,22 @@
         self.opts: dict = {}
 
         # parsing "cache" info
         self.current_grindex: int = 0
         self.current_group: str = self.DEFAULT_GROUP_NAME
         self.current_host: Optional[SSH_Host] = None
         self.current_host_info: list = []
+        self.current_host_pass: str = ""
 
 
     def read(self):
         """
         Read content of SSH config file
         """
-        with open(self.ssh_config_file) as fh:
+        with open(self.ssh_config_file, "r") as fh:
             self.ssh_config_lines = fh.readlines()
         return self
 
 
     def _config_flush_host(self) -> None:
         """
         Internal function used to flush host configuration while parsing config file
@@ -113,14 +114,19 @@
                     continue
 
                 elif metadata == "host":
                     logging.debug(f"META: Host comment found '{value}' Caching for next host definition...'")
                     self.current_host_info.append(value)
                     continue
 
+                elif metadata == "password":
+                    logging.debug(f"META: Host password found '{value}' Caching for next host definition...'")
+                    self.current_host_pass = value
+                    continue
+
                 else:
                     logging.warning(f"META: Unhandled metadata '{metadata}' on SSH-config line number: {config_line_index}")
                     continue
 
             # Here we expect only normal ssh config lines "Host" is usually the keyword that begins definition
             # if we find any other keyword before first host keyword is defined, configuration is wrong probably
             match = re.search(r"^(\w+)\s+(.+)$", line)
@@ -134,18 +140,19 @@
             # --- Found "host" keyword, that defines new block, usually followed with name
             if keyword == "host":
                 self._config_flush_host()
 
                 host_type = "pattern" if "*" in value else "normal"
                 logging.debug(f"Host '{value}' is '{host_type}' type!")
 
-                self.current_host = SSH_Host(name=value, group=self.current_group, type=host_type, info=self.current_host_info)
+                self.current_host = SSH_Host(name=value, password=self.current_host_pass, group=self.current_group, type=host_type, info=self.current_host_info)
 
                 # Reset global host info cache when we find new host (from this line, any host comments will apply to next host)
                 self.current_host_info = []
+                self.current_host_pass = ""
                 continue
             else:
                 # any other normal line we just use as it is, wrong or not... :)
                 # Currently there is no support for keyword validation
                 if not self.current_host:
                     logging.warning(f"Config info without Host definition on SSH-config line number {config_line_index}")
                     exit(1)
@@ -192,14 +199,18 @@
         # First we lines before we flush them into file
         lines: List[str] = ["#<<<<< SSH Config file managed by sshclick >>>>>\n"]
 
         # Dump any saved configuration
         for option in self.opts:
             lines.append(f"#{SSHCONFIG_META_PREFIX}config{SSHCONFIG_META_SEPARATOR}{option}={self.opts[option]}\n")
 
+        # Add separation from header/config and rest of ssh-config
+        lines.append("\n")
+
+        # Render all groups
         for group in self.groups:
             # Ship default group as it does not have to be specified
             render_header = False if group.name == self.DEFAULT_GROUP_NAME else True
             
             if render_header:
                 # Add extra blank line when outputting new group header
                 lines.append("\n")
```

### Comparing `sshclick-0.5.0/sshclick/sshc/ssh_host.py` & `sshclick-0.6.0/sshclick/sshc/ssh_host.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,66 @@
-from ..globals import DEFAULT_HOST_STYLE
-from typing import List
+from typing import List, Tuple, Dict
 from dataclasses import dataclass, field
 import importlib
+import socket
+
+from ..globals import DEFAULT_HOST_STYLE
 
 from rich.console import Console
 console = Console()
 
 DEBUG_STYLES = False
 
 @dataclass
 class SSH_Host:
     """ Class for SSH host config structure """
     name: str
     group: str
+    password: str = ""
     type: str = "normal"
-    info: List[str] = field(default_factory=list)
+    info: list = field(default_factory=list)
     params: dict = field(default_factory=dict)
 
     inherited_params: list = field(default_factory=list)
     print_style: str = DEFAULT_HOST_STYLE
 
 
+    def get_all_params(self) -> Dict[str, str]:
+        """
+        Method combines configured host parameters with all
+        host inherited parameters, and returns them as dictionary
+        """
+        return {
+            **self.params,
+            **{ k: v for d in self.inherited_params for k, v in d[1].items()}
+        }
+    
+
+    def get_target(self) -> str:
+        """
+        Method returns whatever host has defined as target for connection.
+        If name is just alias, and host has defined "hostname" then hostname will be returned
+        When there is no hostname, only host name is returned
+        """
+        return self.name if not "hostname" in self.params else self.params["hostname"]
+
+
+    def resolve_target(self) -> Tuple[str, bool]:
+        """
+        Method returns tuple of resolved IP address for this host, and error as bool value,
+        that is set to true if host cannot be resolved
+        """
+        target = self.get_target()
+        try:
+            target_ip = socket.gethostbyname(target)
+            return (target_ip, False)
+        except socket.error:
+            return ("", True)
+
+
     # Method for interaction with printing the object via Rich library
     # Each supported style should be located in defined folder (by default under "host_styles")
     # Each module must have "render" function, and return "rich renderable" object
     def __rich__(self):
         try:
             # If current host "print_style" is set to "panels", we will try
             # to import module from "./host_styles/panels.py"
```

### Comparing `sshclick-0.5.0/sshclick/sshc/ssh_parameters.py` & `sshclick-0.6.0/sshclick/sshc/ssh_parameters.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/sshclick/sshc/sshutils.py` & `sshclick-0.6.0/sshclick/sshc/sshutils.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.5.0/PKG-INFO` & `sshclick-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshclick
-Version: 0.5.0
+Version: 0.6.0
 Summary: SSH Config manager
 Home-page: https://github.com/karlot/sshclick
 License: MIT
 Author: Karlo Tisaj
 Author-email: karlot@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,22 +13,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: prettytable (>=3.7,<4.0)
 Requires-Dist: rich (>=13.3,<14.0)
+Requires-Dist: textual (>=0.26,<0.27)
 Description-Content-Type: text/markdown
 
 # SSH Click Config manager (sshclick)
 
 ![splash_gif](tapes/splash.gif)
 
 ## Links
@@ -40,52 +35,54 @@
   - [Upgrade procedure](https://github.com/karlot/sshclick#upgrade-procedure)
   - [Uninstall procedure](https://github.com/karlot/sshclick#uninstall-procedure)
 - [SSH Config structure](https://github.com/karlot/sshclick#ssh-config-structure-and-important-note-about-comments)
   - [Comment blocks and metadata](https://github.com/karlot/sshclick#comment-blocks-and-metadata-in-ssh-config)
 - [Example usage and features](https://github.com/karlot/sshclick#example-usage-and-features)
   - [Group commands and options](https://github.com/karlot/sshclick#group-commands-and-options)
   - [Host commands and options](https://github.com/karlot/sshclick#host-commands-and-options)
+  - [Config commands and options](https://github.com/karlot/sshclick#config-commands-and-sshclick-configuration-options)
   - [Output styling and user ENV variables](https://github.com/karlot/sshclick#output-styling-and-user-env-variables)
-- [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)
+<!-- - [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)
   - [sshc group operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-group-operations)
-  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations)
+  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations) -->
 - [Author](https://github.com/karlot/sshclick#author)
 - [License](https://github.com/karlot/sshclick#license)
 
 
 ## Intro
 Terminal based assisted management of your SSH config files.  
 Built out of boredom with managing messy and huge ssh_config files.  
 
-EARLY VERSION, backup your SSH config files before using!  
-SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config!  
+Backup your SSH config files before using!  
+SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config in any way!  
 
 **Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**
 
+**NEW!** *Now comes with additional TUI that can be accessed via `sshc tui` or `ssht`.*  
+
+![splash_gif](tapes/sshc_tui_example.svg)
+
+
 ## Why?
 
-What am I trying to solve with this tool?
 * I need something that works fast and great in terminal, and does not require complex setup.
-* Managing some other configuration files that renders to SSH config is extra step that I don't like.
-* SSH config is already feature-full with all options SSH client support, why inventing extra layer?
 * SSH config is the only config I need to backup.
+* SSH config is very feature-full with all options SSH client support, why inventing extra layer?
 * I need quick way to search, group and visualize all hosts inside SSH configuration (especially since it can grow huge)
 
 
 ## What does it do?
 
 SSHClick (sshc) is just a tool designed to work with existing SSH configuration files on your Linux/Windows/WSL terminal environment.  
-It basically parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.
-Trough additional "magic" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.
+It parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.
+Trough additional "metadata" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.
 
 
 ### Installation procedure
 
-Should be straight forward...  
-
 1. **Check preconditions:**
     - Currently only tested on Linux (Debian 10,11, Ubuntu 20.04,22.04), but should work on other systems as well
     - Minimum python3.7 (tested up to 3.11 beta) & pip installed
         - it is preferable to not use system python version, to install "custom" user python on linux, you can try using pyenv (https://github.com/pyenv/pyenv
     - git installed
 
 2. **Install package:**
@@ -188,27 +185,27 @@
 SSHClick is deploying `sshc` cli tool that allows interacting with your SSH Config file and perform various organization,listing, displaying and modification of SSH Group/Host configuration parameters.  
 `sshc` comes with pre-built lots of help options so each level of commands provide `--help` options to provide you info what commands and options are available at which command level.  
 
 For example to check version, type: `sshc --version`  
 _Sample output:_
 ```console
 $ sshc --version
-SSHClick (sshc) - Version: 0.5.0
+SSHClick (sshc) - Version: 0.6.0
 ```
 
 If you run `sshc` command alone, or adding `-h` or `--help` option, it will show help what else must be added to the command...  
 _Example:_
 ```console
 $ sshc --help
 Usage: sshc [OPTIONS] COMMAND [ARGS]...
 
-  SSHClick - SSH Config manager. version 0.5.0
+  SSHClick - SSH Config manager. version 0.6.0
 
-  NOTE: As this is early alpha, backup your SSH config files before this
-  software, as you might accidentally lose some configuration
+  NOTE: As this will change your SSH config files, make backups before using
+  this software, as you might accidentally lose some configuration.
 
 Options:
   --sshconfig TEXT  Config file (default: ~/.ssh/config)
   --stdout          Send changed SSH config to STDOUT instead to original
                     file, can be enabled with setting ENV variable (export
                     SSHC_STDOUT=1)
   --version         Show the version and exit.
@@ -216,21 +213,21 @@
 
 Commands:
   config  Modify SSHClick configuration trough SSH Config
   group   Command group for managing groups
   groups  Lists all groups
   host    Command group for managing hosts
   hosts   List configured hosts
+  tui     TUI Interface (experimental)
 ```
 
-
 ### `group` commands and options
 
 To manage "groups" type `sshc group --help` to see options.  
-_example:_
+_Example:_
 ```console
 $ sshc group --help
 Usage: sshc group [OPTIONS] COMMAND [ARGS]...
 
   Command group for managing groups
 
 Options:
@@ -244,15 +241,15 @@
   set     Change group parameters
   show    Shows group details
 ```
 
 ### `host` commands and options
 
 To manage "groups" type `sshc host --help` to see options.  
-_example:_
+_Example:_
 ```console
 $ sshc host --help
 Usage: sshc host [OPTIONS] COMMAND [ARGS]...
 
   Command group for managing hosts
 
 Options:
@@ -265,29 +262,83 @@
   list     List configured hosts
   rename   Rename existing host
   set      Set/Change host configuration
   show     Show current host configuration
   test     Test SSH host connection  (experimental)
 ```
 
+### `config` commands and SSHClick configuration options
+
+SSHClick does not to have its own configuration files, so most of configuration that it tries to understand, come from commands arguments/options, environment variables, and SSH Config file itself.
+
+Sometimes when you want to persist some config options, not to repeat it via command, you can use ENV variables, that can be set trough user shell profile.
+
+Now there is also option to store such config in SSH Config file itself (as metadata comment), so it can be portable and backed up together with SSH Config file.
+
+Command `config` takes `set` or `del` commands that add or remove specific configuration.
+
+_Example:_
+```console
+$ sshc config --help
+Usage: sshc config [OPTIONS] COMMAND [ARGS]...
+
+  Modify SSHClick configuration trough SSH Config
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  del  Delete config option
+  set  Set config option
+```
+
+
+_Example: "Set host output style to 'card'"_
+```console
+$ sshc config set --help
+Usage: sshc config set [OPTIONS]
+
+  Set config option
+
+Options:
+  --host-style TEXT  Set how to display hosts in 'show' command.
+                     Available:(panels,card,simple,table,table2,json)
+                     (default: panels)
+  -h, --help         Show this message and exit.
+
+$ sshc config set --host-style card
+```
+
+This will now store config in "currently used" SSH config file as following:
+```
+#<<<<< SSH Config file managed by sshclick >>>>>
+#@config: host-style=card
+```
+
+To delete this config, either remove the line from file manually, or use `sshc` command:
+```console
+$ sshc config del --host-style
+```
+
 ### Output styling and user ENV variables
 
 `sshc host show` can display host output is several formats, you can specify it with `sshc host show <host> --style <style>`  
 Available styles are:
 
 | Style              | Description                                       |
 |--------------------|---------------------------------------------------|
 | `panels` (default) | Display data in several panels                    |
 | `card`             | Add data to single "card"                         |
 | `simple`           | Simple output with minimal decorations            |
 | `table`            | Flat table with 3 columns                         |
 | `table2`           | Nested table with separated host SSH params       |
-| `json`             | JSON output, useful for binding with other tools |
+| `json`             | JSON output, useful for binding with other tools  |
 
-If you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.
+If you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.  
+Alternatively, you can use SSHClick internal "config" mechanism to store some config data into your SSH Config file (as commented metadata) so it can be backed up with your SSH config. To do so, you can use following command as example: `sshc config set --host-style table`.
 
 In case user do not line "fancy" colors in output, you can set ENV variable to disable all color outputs with `export NO_COLOR=1`. If you want it permanently you can add it to startup "rc" files as well.
 
 
 > NOTE! When sending output into non-terminal such as to file, SSHClick will recognize that and will remove all ANSI Escape characters (colors and stuff...) so that output is captured in clear way.
 
 
@@ -378,11 +429,29 @@
 Karlo Tisaj  
 email: karlot@gmail.com  
 github: https://github.com/karlot
 
 
 ## License
 
-[MIT License](LICENSE)
+MIT License
 
+Copyright (c) 2023 Karlo Tisaj
 
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

