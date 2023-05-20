# Comparing `tmp/mcdreforged-2.8.4.tar.gz` & `tmp/mcdreforged-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcdreforged-2.8.4.tar", last modified: Sun May  7 13:59:31 2023, max compression
+gzip compressed data, was "mcdreforged-2.9.0.tar", last modified: Sat May 20 17:16:47 2023, max compression
```

## Comparing `mcdreforged-2.8.4.tar` & `mcdreforged-2.9.0.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged/api/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/all/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/new_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/spam_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/event/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/rcon/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/rcon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/rtext/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/rtext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/utils/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cli_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_gendefault.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/command_builder_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/command_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/command_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/core_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/plugin_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/console_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/task_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/thread_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/update_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8295 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/abstract_server_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/handler/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/abstract_minecraft_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/basic_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/beta18_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit14_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bungeecord_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/cat_server_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/forge_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/vanilla_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/velocity_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/waterfall_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/server_handler_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/info_reactor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/abstract_info_reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/general_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/player_reactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/server_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/info_reactor_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/server_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24141 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/permission/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/permission_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/permission_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/check_update_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/python_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/dependency_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/operation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24770 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    42338 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/server_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/directory_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/multi_file_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/packed_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/permanent_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/regular_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/solo_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/preference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/preference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/preference/preference_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/default_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/default_permission.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/resources/lang/
--rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/lang/en_us.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/lang/zh_cn.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/translation_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/translation_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/mcdreforged/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/class_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/future.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/lazy_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/misc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/resources_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/thread_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/translation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/tree_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/yaml_data_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.606075 mcdreforged-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-20 17:16:47.606075 mcdreforged-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.586074 mcdreforged-2.9.0/mcdreforged/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/decorator/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/decorator/new_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/decorator/spam_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/rcon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/rtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/rtext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/api/utils/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cli_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cmd_gendefault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cmd_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/cli/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/command/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/command_builder_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged/command/builder/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/nodes/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/nodes/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/builder/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/command_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/command/command_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/constants/core_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/constants/plugin_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/console_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/thread_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/update_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/executor/watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8295 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/abstract_server_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/handler/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/abstract_minecraft_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/basic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/beta18_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/bukkit14_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/bukkit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/bungeecord_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/cat_server_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/forge_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/vanilla_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/velocity_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/impl/waterfall_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/handler/server_handler_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/info_reactor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/abstract_info_reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/info_reactor/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/impl/general_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/impl/player_reactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2027 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/impl/server_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/info_reactor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/info_reactor/server_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/mcdr_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25095 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/mcdr_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/mcdr_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.594075 mcdreforged-2.9.0/mcdreforged/minecraft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/minecraft/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rcon/rcon_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rcon/rcon_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/minecraft/rtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rtext/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/minecraft/rtext/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/permission/permission_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/permission/permission_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/plugin/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.598075 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/check_update_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/server_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/builtin/python_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/plugin/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/meta/dependency_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/meta/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/meta/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/operation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/plugin_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/plugin_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24770 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/plugin_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43216 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/server_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/plugin/type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/directory_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/multi_file_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/packed_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/permanent_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/regular_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/plugin/type/solo_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/preference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/preference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/preference/preference_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/resources/default_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/resources/default_permission.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/resources/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/resources/lang/en_us.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/resources/lang/zh_cn.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.602075 mcdreforged-2.9.0/mcdreforged/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/translation/translation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/translation/translation_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.606075 mcdreforged-2.9.0/mcdreforged/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/class_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/lazy_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/misc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/resources_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/thread_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/translation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/tree_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/mcdreforged/utils/yaml_data_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:47.590074 mcdreforged-2.9.0/mcdreforged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-20 17:16:47.000000 mcdreforged-2.9.0/mcdreforged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-20 17:16:47.000000 mcdreforged-2.9.0/mcdreforged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:16:47.000000 mcdreforged-2.9.0/mcdreforged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 17:16:47.000000 mcdreforged-2.9.0/mcdreforged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 17:16:47.000000 mcdreforged-2.9.0/mcdreforged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:16:47.606075 mcdreforged-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-20 17:16:41.000000 mcdreforged-2.9.0/setup.py
```

### Comparing `mcdreforged-2.8.4/LICENSE` & `mcdreforged-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/PKG-INFO` & `mcdreforged-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdreforged
-Version: 2.8.4
+Version: 2.9.0
 Summary: A rewritten version of MCDaemon, a python script to control your Minecraft server
 Home-page: https://github.com/Fallen-Breath/MCDReforged
 Author: Fallen_Breath
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `mcdreforged-2.8.4/README.md` & `mcdreforged-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/all/__init__.py` & `mcdreforged-2.9.0/mcdreforged/api/all/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/command/__init__.py` & `mcdreforged-2.9.0/mcdreforged/api/command/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/decorator/event_listener.py` & `mcdreforged-2.9.0/mcdreforged/api/decorator/event_listener.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/decorator/new_thread.py` & `mcdreforged-2.9.0/mcdreforged/api/decorator/new_thread.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/decorator/spam_proof.py` & `mcdreforged-2.9.0/mcdreforged/api/decorator/spam_proof.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/api/types/__init__.py` & `mcdreforged-2.9.0/mcdreforged/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/cli/cli_entry.py` & `mcdreforged-2.9.0/mcdreforged/cli/cli_entry.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/cli/cmd_pack.py` & `mcdreforged-2.9.0/mcdreforged/cli/cmd_pack.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/cli/cmd_run.py` & `mcdreforged-2.9.0/mcdreforged/cli/cmd_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 	try:
 		mcdreforged_server = MCDReforgedServer()
 	except Exception as e:
 		print('Fail to initialize {}: ({}) {}'.format(core_constant.NAME_SHORT, type(e), e), file=sys.stderr)
 		raise
 
 	if mcdreforged_server.is_initialized():
-		mcdreforged_server.start()
+		mcdreforged_server.run_mcdr()
 	else:
 		# If it's not initialized, config file or permission file is missing
 		# Just don't do anything to let the user check the files
 		pass
```

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/command_builder_util.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/command_builder_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/common.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/common.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/exception.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/exception.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/nodes/arguments.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/nodes/arguments.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/nodes/basic.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/nodes/basic.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/builder/tools.py` & `mcdreforged-2.9.0/mcdreforged/command/builder/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,26 +266,30 @@
 		self.clean_cache()
 		return definition
 
 	# --------------
 	#    Outputs
 	# --------------
 
-	def build(self) -> List[AbstractNode]:
+	def build(self, *, use_cache: bool = True) -> List[AbstractNode]:
 		"""
 		Build the command trees
 
 		Nodes with same name will be reused. e.g. if you define 3 commands with path ``"!!foo"``, ``"!!foo bar"`` and "``!!foo baz"``,
 		the root ``"!!foo"`` node will be reused, and there will be only 1 ``"!!foo"`` node eventually
 
+		:keyword use_cache: If set to false, do not use cache and always build new command trees
 		:return: A list of the built command tree root nodes. The result is cached until you instruct the builder again.
 			You can use :meth:`clean_cache` to explicitly clean the build cache
 		:raise SimpleCommandBuilder.Error: if there are undefined argument nodes
+
+		.. versionadded:: v2.9.0
+			Added ``use_cache`` keyword argument
 		"""
-		if self.__build_cache is None:
+		if not use_cache or self.__build_cache is None:
 			root = Literal('#TEMP')
 			for command, callback in self.__commands.items():
 				node = root
 				for segment in command.split(' '):
 					if len(segment) > 0:
 						node = self.__locate_or_create_child(node, segment)
 				node.runs(callback)
```

### Comparing `mcdreforged-2.8.4/mcdreforged/command/command_manager.py` & `mcdreforged-2.9.0/mcdreforged/command/command_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/command/command_source.py` & `mcdreforged-2.9.0/mcdreforged/command/command_source.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/constants/core_constant.py` & `mcdreforged-2.9.0/mcdreforged/constants/core_constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 NAME_SHORT = 'MCDR'
 NAME = 'MCDReforged'
 PACKAGE_NAME = 'mcdreforged'
 
 # MCDR Version Storage
 # Related: docs/source/conf.py
-VERSION = '2.8.4'       # semver (1.2.3-alpha.4)
-VERSION_PYPI = '2.8.4'  # pythonic ver (1.2.3a4)
+VERSION = '2.9.0'       # semver (1.2.3-alpha.4)
+VERSION_PYPI = '2.9.0'  # pythonic ver (1.2.3a4)
 
 GITHUB_URL = 'https://github.com/Fallen-Breath/MCDReforged'
 GITHUB_API_LATEST = 'https://api.github.com/repos/Fallen-Breath/MCDReforged/releases/latest'
 DOCUMENTATION_URL = 'https://mcdreforged.readthedocs.io/'
 
 PACKAGE_PATH = os.path.realpath(os.path.join(os.path.dirname(__file__), '..'))
 LOGGING_FILE = os.path.join('logs', '{}.log'.format(NAME_SHORT))
```

### Comparing `mcdreforged-2.8.4/mcdreforged/constants/plugin_constant.py` & `mcdreforged-2.9.0/mcdreforged/constants/plugin_constant.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/executor/console_handler.py` & `mcdreforged-2.9.0/mcdreforged/executor/console_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/executor/task_executor.py` & `mcdreforged-2.9.0/mcdreforged/executor/task_executor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/executor/thread_executor.py` & `mcdreforged-2.9.0/mcdreforged/executor/thread_executor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/executor/update_helper.py` & `mcdreforged-2.9.0/mcdreforged/executor/update_helper.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/executor/watchdog.py` & `mcdreforged-2.9.0/mcdreforged/executor/watchdog.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,21 @@
 		self.pause()
 		try:
 			yield
 		finally:
 			self.resume()
 
 	def check_task_executor_state(self):
-		task_executor = self.mcdr_server.task_executor
 		no_respond_threshold = self.mcdr_server.config['watchdog_threshold']  # in seconds
 		if not isinstance(no_respond_threshold, (int, float)):
 			no_respond_threshold = self.DEFAULT_NO_RESPOND_THRESHOLD
 		if no_respond_threshold <= 0:
 			return
+
+		task_executor = self.mcdr_server.task_executor
 		if task_executor.get_this_tick_time() > no_respond_threshold and self.__monitoring:
 			plugin = self.mcdr_server.plugin_manager.get_current_running_plugin(thread=task_executor.get_thread())
 			self.mcdr_server.logger.warning(self.mcdr_server.tr('watchdog.task_executor_no_response.line1', no_respond_threshold))
 			self.mcdr_server.logger.warning(self.mcdr_server.tr('watchdog.task_executor_no_response.line2', plugin))
 			self.mcdr_server.logger.warning(self.mcdr_server.tr('watchdog.task_executor_no_response.line3'))
 
 			task_executor.soft_stop()  # Soft-stop it, in case it turns alive somehow
```

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/abstract_server_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/abstract_server_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/__init__.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/abstract_minecraft_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/abstract_minecraft_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/basic_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/basic_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/beta18_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/beta18_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit14_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/bukkit14_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/bukkit_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/bungeecord_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/bungeecord_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/cat_server_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/cat_server_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/forge_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/forge_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/velocity_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/velocity_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/impl/waterfall_handler.py` & `mcdreforged-2.9.0/mcdreforged/handler/impl/waterfall_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/handler/server_handler_manager.py` & `mcdreforged-2.9.0/mcdreforged/handler/server_handler_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/abstract_info_reactor.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/abstract_info_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/general_reactor.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/impl/general_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/player_reactor.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/impl/player_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/server_reactor.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/impl/server_reactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 	def react(self, info: Info):
 		if info.source == InfoSource.SERVER:
 			handler = self.mcdr_server.server_handler_manager.get_current_handler()
 
 			if handler.test_server_startup_done(info):
 				self.mcdr_server.logger.debug('Server startup detected', option=DebugOption.REACTOR)
-				self.mcdr_server.with_flag(MCDReforgedFlag.SERVER_STARTUP)
+				self.mcdr_server.add_flag(MCDReforgedFlag.SERVER_STARTUP)
 				self.mcdr_server.plugin_manager.dispatch_event(MCDRPluginEvents.SERVER_STARTUP, ())
 
 			version = handler.parse_server_version(info)
 			if version is not None:
 				self.mcdr_server.logger.debug('Server version detected: {}'.format(version), option=DebugOption.REACTOR)
 				self.server_info.version = version
 
 			ip_and_port = handler.parse_server_address(info)
 			if ip_and_port is not None:
 				self.mcdr_server.logger.debug('Server ip detected: {}:{}'.format(*ip_and_port), option=DebugOption.REACTOR)
 				self.server_info.ip, self.server_info.port = ip_and_port
 
 			if handler.test_rcon_started(info):
 				self.mcdr_server.logger.debug('Server rcon started detected', option=DebugOption.REACTOR)
-				self.mcdr_server.with_flag(MCDReforgedFlag.SERVER_RCON_READY)
+				self.mcdr_server.add_flag(MCDReforgedFlag.SERVER_RCON_READY)
 				self.mcdr_server.connect_rcon()
 
 			if handler.test_server_stopping(info):  # notes that it might happen more than once in the server lifecycle
 				self.mcdr_server.logger.debug('Server stopping detected', option=DebugOption.REACTOR)
 				self.mcdr_server.rcon_manager.disconnect()
```

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/info.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/info.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/info_reactor_manager.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/info_reactor_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/info_reactor/server_information.py` & `mcdreforged-2.9.0/mcdreforged/info_reactor/server_information.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/mcdr_config.py` & `mcdreforged-2.9.0/mcdreforged/mcdr_config.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/mcdr_server.py` & `mcdreforged-2.9.0/mcdreforged/mcdr_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import locale
 import os
 import sys
 import time
 import traceback
 from pathlib import Path
-from subprocess import Popen, PIPE, STDOUT
-from threading import Lock
+from subprocess import Popen, PIPE, STDOUT, TimeoutExpired
+from threading import Lock, Condition
 from typing import Optional, Callable, Any, List
 
 import pkg_resources
 import psutil
 from ruamel.yaml import YAMLError
 
 from mcdreforged.command.command_manager import CommandManager
@@ -28,28 +28,29 @@
 from mcdreforged.permission.permission_manager import PermissionManager
 from mcdreforged.plugin.plugin_event import MCDRPluginEvents
 from mcdreforged.plugin.plugin_manager import PluginManager
 from mcdreforged.plugin.server_interface import ServerInterface
 from mcdreforged.preference.preference_manager import PreferenceManager
 from mcdreforged.translation.translation_manager import TranslationManager
 from mcdreforged.utils import file_util
-from mcdreforged.utils.exception import IllegalCallError, ServerStopped, ServerStartError, IllegalStateError, DecodeError
+from mcdreforged.utils.exception import ServerStartError, IllegalStateError, DecodeError
 from mcdreforged.utils.logger import DebugOption, MCDReforgedLogger, MCColorFormatControl
 from mcdreforged.utils.types import MessageText
 
 
 class MCDReforgedServer:
 	process: Optional[Popen]
 
 	def __init__(self, *, generate_default_only: bool = False, initialize_environment: bool = False):
 		"""
 		:param generate_default_only: If set to true, MCDR will only generate the default configuration and permission files
 		"""
 		self.mcdr_state = MCDReforgedState.INITIALIZING
 		self.server_state = ServerState.STOPPED
+		self.server_state_cv = Condition()
 		self.server_information = ServerInformation()
 		self.process: Optional[Popen] = None
 		self.flags = MCDReforgedFlag.NONE
 		self.starting_server_lock = Lock()  # to prevent multiple start_server() call
 		self.stop_lock = Lock()  # to prevent multiple stop() call
 		self.config_change_lock = Lock()
 
@@ -170,15 +171,15 @@
 			self.logger.warning('In a production environment, you should install {} from PyPI, NOT from source codes'.format(mcdr_pkg))
 			self.logger.warning('See document ({}) for more information'.format(core_constant.DOCUMENTATION_URL))
 			self.logger.warning('MCDR will launch after 20 seconds...')
 			time.sleep(20)
 
 	def __on_file_missing(self):
 		self.logger.info('Looks like MCDR is not initialized at current directory {}'.format(os.getcwd()))
-		self.logger.info('Use "python -m {} init" to initialize MCDR first'.format(core_constant.PACKAGE_NAME))
+		self.logger.info('Use "{} -m {} init" to initialize MCDR first'.format(sys.argv[0], core_constant.PACKAGE_NAME))
 
 	# --------------------------
 	#         Translate
 	# --------------------------
 
 	def get_language(self) -> str:
 		return self.translation_manager.language
@@ -285,15 +286,15 @@
 
 	def is_mcdr_about_to_exit(self):
 		return self.mcdr_in_state({MCDReforgedState.PRE_STOPPED, MCDReforgedState.STOPPED})
 
 	def should_exit_after_stop(self):
 		return MCDReforgedFlag.EXIT_AFTER_STOP in self.flags
 
-	def with_flag(self, flag: MCDReforgedFlag):
+	def add_flag(self, flag: MCDReforgedFlag):
 		self.flags |= flag
 		self.logger.debug('Added MCDReforgedFlag {}'.format(flag), option=DebugOption.MCDR)
 
 	def remove_flag(self, flag: MCDReforgedFlag):
 		self.flags &= ~flag
 		self.logger.debug('Removed MCDReforgedFlag {}'.format(flag), option=DebugOption.MCDR)
 
@@ -307,14 +308,16 @@
 
 	def is_initialized(self):
 		return self.mcdr_in_state(MCDReforgedState.INITIALIZED)
 
 	def set_server_state(self, state):
 		self.server_state = state
 		self.logger.debug('Server state has set to "{}"'.format(state), option=DebugOption.MCDR)
+		with self.server_state_cv:
+			self.server_state_cv.notify_all()
 
 	def set_mcdr_state(self, state):
 		self.mcdr_state = state
 		self.logger.debug('MCDR state has set to "{}"'.format(state), option=DebugOption.MCDR)
 
 	def should_keep_looping(self):
 		"""
@@ -370,35 +373,41 @@
 	def __kill_server(self):
 		"""
 		Kill the server process group
 		"""
 		if self.process and self.process.poll() is None:
 			self.logger.info(self.tr('mcdr_server.kill_server.killing'))
 			try:
-				for child in psutil.Process(self.process.pid).children(recursive=True):
-					child.kill()
-					self.logger.info(self.tr('mcdr_server.kill_server.process_killed', child.pid))
+				root = psutil.Process(self.process.pid)
+				processes = [root]
+				processes.extend(root.children(recursive=True))
+				for proc in reversed(processes):  # child first, parent last
+					try:
+						proc_pid, proc_name = proc.pid, proc.name()  # in case we cannot get them after the process dies
+						proc.kill()
+						self.logger.info(self.tr('mcdr_server.kill_server.process_killed', proc_name, proc_pid))
+					except psutil.NoSuchProcess:
+						pass
 			except psutil.NoSuchProcess:
 				pass
-			self.process.kill()
-			self.logger.info(self.tr('mcdr_server.kill_server.process_killed', self.process.pid))
+			self.process.poll()
 		else:
-			raise IllegalCallError("Server process has already been terminated")
+			self.logger.warning('Try to kill the server when the server process has already been terminated')
 
 	def interrupt(self) -> bool:
 		"""
 		Interrupt MCDR
 		The first call will softly stop the server and the later calls will kill the server
 		Return if it's the first try
 		"""
 		first_interrupt = not self.is_interrupt()
-		self.logger.info('Interrupting, first strike = {}'.format(first_interrupt))
+		self.logger.info(self.tr('mcdr_server.interrupt.{}'.format('soft' if first_interrupt else 'hard')))
 		if self.is_server_running():
 			self.stop(forced=not first_interrupt)
-		self.with_flag(MCDReforgedFlag.INTERRUPT)
+		self.add_flag(MCDReforgedFlag.INTERRUPT)
 		return first_interrupt
 
 	def stop(self, forced: bool = False) -> bool:
 		"""
 		Stop the server
 
 		:param forced: an optional bool. If it's False (default) MCDR will stop the server by sending the STOP_COMMAND from the
@@ -412,27 +421,24 @@
 			if not forced:
 				try:
 					self.send(self.server_handler_manager.get_current_handler().get_stop_command())
 				except Exception:
 					self.logger.error(self.tr('mcdr_server.stop.stop_fail'))
 					forced = True
 			if forced:
-				try:
-					self.__kill_server()
-				except IllegalCallError:
-					pass
+				self.__kill_server()
 			return True
 
 	# --------------------------
 	#      Server Logics
 	# --------------------------
 
 	def __on_server_start(self):
 		self.set_server_state(ServerState.RUNNING)
-		self.with_flag(MCDReforgedFlag.EXIT_AFTER_STOP)  # Set after server state is set to RUNNING, or MCDR might have a chance to exit if the server is started by other thread
+		self.add_flag(MCDReforgedFlag.EXIT_AFTER_STOP)  # Set after server state is set to RUNNING, or MCDR might have a chance to exit if the server is started by other thread
 		self.logger.info(self.tr('mcdr_server.start_server.pid_info', self.process.pid))
 		self.reactor_manager.on_server_start()
 		self.plugin_manager.dispatch_event(MCDRPluginEvents.SERVER_START, ())
 
 	def __on_server_stop(self):
 		return_code = self.process.poll()
 		self.logger.info(self.tr('mcdr_server.on_server_stop.show_return_code', return_code))
@@ -475,32 +481,34 @@
 		if self.is_server_running():
 			self.process.stdin.write(encoded_text)
 			self.process.stdin.flush()
 		else:
 			self.logger.warning(self.tr('mcdr_server.send.send_when_stopped'))
 			self.logger.warning(self.tr('mcdr_server.send.send_when_stopped.text', text if len(text) <= 32 else text[:32] + '...'))
 
-	def __receive(self):
+	def __receive(self) -> Optional[str]:
 		"""
 		Try to receive a str from server's stdout. This will block the current thread
-		If server has stopped it will wait up to 10s for the server process to exit, then raise a ServerStopped exception
 
-		:rtype: str
-		:raise: ServerStopped
+		If server has stopped it will wait up to 60s for the server process to exit, then return None
 		"""
 		try:
 			text: bytes = next(iter(self.process.stdout))
 		except StopIteration:  # server process has stopped
-			for i in range(core_constant.WAIT_TIME_AFTER_SERVER_STDOUT_END_SEC * 10):
-				if self.process.poll() is not None:
-					break
-				time.sleep(0.1)
-				if i % 10 == 0:
+			for i in range(core_constant.WAIT_TIME_AFTER_SERVER_STDOUT_END_SEC):
+				try:
+					self.process.wait(1)
+				except TimeoutExpired:
 					self.logger.info(self.tr('mcdr_server.receive.wait_stop'))
-			raise ServerStopped()
+				else:
+					break
+			else:
+				self.logger.warning('The server is still not stopped after {}s after its stdout was closed, killing'.format(core_constant.WAIT_TIME_AFTER_SERVER_STDOUT_END_SEC))
+				self.__kill_server()
+			return None
 		else:
 			try:
 				decoded_text: str = text.decode(self.decoding_method)
 			except Exception as e:
 				self.logger.error(self.tr('mcdr_server.receive.decode_fail', text, e))
 				raise DecodeError(e)
 			return decoded_text.rstrip('\n\r').lstrip('\n\r')
@@ -510,17 +518,19 @@
 		ticking MCDR:
 		try to receive a new line from server's stdout and parse / display / process the text
 		"""
 		try:
 			text = self.__receive()
 		except DecodeError:
 			return
-		except ServerStopped:
+
+		if text is None:  # server stops
 			self.__on_server_stop()
 			return
+
 		try:
 			text = self.server_handler_manager.get_current_handler().pre_parse_server_stdout(text)
 		except Exception:
 			self.logger.warning(self.tr('mcdr_server.tick.pre_parse_fail'))
 
 		parsed_result: Info
 		try:
@@ -536,14 +546,15 @@
 				self.logger.debug('Parsed text from server stdout:', no_check=True)
 				for line in parsed_result.debug_format_text().splitlines():
 					self.logger.debug('    {}'.format(line), no_check=True)
 		self.server_handler_manager.detect_text(text)
 		self.reactor_manager.put_info(parsed_result)
 
 	def __on_mcdr_start(self):
+		self.__register_signal_handler()
 		self.watch_dog.start()
 		self.task_executor.start()
 		self.preference_manager.load_preferences()
 		self.plugin_manager.register_permanent_plugins()
 		self.task_executor.execute_on_thread(self.load_plugins, block=True)
 		self.plugin_manager.dispatch_event(MCDRPluginEvents.MCDR_START, ())
 		if not self.config['disable_console_thread']:
@@ -552,14 +563,27 @@
 			self.logger.info(self.tr('mcdr_server.on_mcdr_start.console_disabled'))
 		if not self.start_server():
 			raise ServerStartError()
 		self.update_helper.start()
 		self.server_handler_manager.start_handler_detection()
 		self.set_mcdr_state(MCDReforgedState.RUNNING)
 
+	def __register_signal_handler(self):
+		def callback(sig: int, frame):
+			try:
+				signal_name = signal.Signals(sig).name
+			except ValueError:
+				signal_name = 'unknown'
+			self.logger.warning('Received signal {} ({}), interrupting MCDR'.format(signal_name, sig))
+			self.interrupt()
+
+		import signal
+		signal.signal(signal.SIGINT, callback)   # ctrl + c
+		signal.signal(signal.SIGTERM, callback)  # graceful termination
+
 	def __on_mcdr_stop(self):
 		try:
 			self.set_mcdr_state(MCDReforgedState.PRE_STOPPED)
 
 			self.logger.info(self.tr('mcdr_server.on_mcdr_stop.info'))
 
 			self.plugin_manager.dispatch_event(MCDRPluginEvents.PLUGIN_UNLOADED, ())
@@ -572,15 +596,15 @@
 		except KeyboardInterrupt:  # I don't know why there sometimes will be a KeyboardInterrupt if MCDR is stopped by ctrl-c
 			pass
 		except Exception:
 			self.logger.exception(self.tr('mcdr_server.on_mcdr_stop.stop_error'))
 		finally:
 			self.set_mcdr_state(MCDReforgedState.STOPPED)
 
-	def start(self):
+	def run_mcdr(self):
 		"""
 		The entry method to start MCDR
 		Try to start the server. if succeeded the console thread will start and MCDR will start ticking
 
 		:raise: IllegalStateError if MCDR is in wrong state
 		:raise: ServerStartError if the server is already running or start_server has been called by other
 		"""
@@ -598,15 +622,16 @@
 		"""
 		self.__on_mcdr_start()
 		while self.should_keep_looping():
 			try:
 				if self.is_server_running():
 					self.__tick()
 				else:
-					time.sleep(0.01)
+					with self.server_state_cv:
+						self.server_state_cv.wait(0.01)
 			except KeyboardInterrupt:
 				self.interrupt()
 			except Exception:
 				if self.is_interrupt():
 					break
 				else:
 					self.logger.critical(self.tr('mcdr_server.run.error'), exc_info=True)
```

### Comparing `mcdreforged-2.8.4/mcdreforged/mcdr_state.py` & `mcdreforged-2.9.0/mcdreforged/mcdr_state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum, unique, Flag, auto
 from typing import Iterable
 
 
 @unique
 class MCDReforgedFlag(Flag):
-	NONE = auto()
+	NONE = auto()               # placeholder
 	INTERRUPT = auto()			# ctrl-c flag
 	SERVER_STARTUP = auto()		# set to True after server startup
 	SERVER_RCON_READY = auto() 	# set to True after server started its rcon. used to start the rcon server
 	EXIT_AFTER_STOP = auto()	# if MCDR exit after server stop. can be modified by plugins
 
 
 class EnumStateBase(Enum):
@@ -30,11 +30,7 @@
 
 
 @unique
 class ServerState(EnumStateBase):
 	STOPPED		= 'server_state.stopped'		# Server is stopped
 	STOPPING	= 'server_state.stopping'		# Server is being stopped by MCDR
 	RUNNING		= 'server_state.running'		# Server is running
-	# PRE_STOPPED	= 'server_state.pre_stopped' 	# Server is stopped, and it's going to dispatch_event SERVER_STOP
-
-	def is_server_stopped(self):
-		return self.in_state({self.STOPPED})
```

### Comparing `mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_connection.py` & `mcdreforged-2.9.0/mcdreforged/minecraft/rcon/rcon_connection.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_manager.py` & `mcdreforged-2.9.0/mcdreforged/minecraft/rcon/rcon_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/minecraft/rtext/style.py` & `mcdreforged-2.9.0/mcdreforged/minecraft/rtext/style.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 	def name(self) -> str:
 		"""
 		Its value in Minecraft text component
 		"""
 		raise NotImplementedError()
 
 
-class RItemLegacy(RItem, ABC):
+class RItemClassic(RItem, ABC):
 	"""
 	A type of :class:`RItem` that can be represented with a classic "§"-prefixed formatting code,
-	or a "\033[31m" styled console ANSI escape code
+	or a "\\\\033[31m" styled console ANSI escape code
 	"""
 	def __init__(self, name: str, mc_code: str, console_code: str):
 		self.__name: str = name
 		assert len(mc_code) == 2 and mc_code[0] == '§'
 		self.__mc_code: str = mc_code
 		self.__console_code: str = console_code
 
@@ -96,32 +96,32 @@
 	pass
 
 
 class RColor(RItem, ABC, metaclass=__RColorMeta):
 	"""
 	Minecraft text colors
 	"""
-	black:        'RColor'
-	dark_blue:    'RColor'
-	dark_green:   'RColor'
-	dark_aqua:    'RColor'
-	dark_red:     'RColor'
-	dark_purple:  'RColor'
-	gold:         'RColor'
-	gray:         'RColor'
-	dark_gray:    'RColor'
-	blue:         'RColor'
-	green:        'RColor'
-	aqua:         'RColor'
-	red:          'RColor'
-	light_purple: 'RColor'
-	yellow:       'RColor'
-	white:        'RColor'
+	black:        'RColorClassic'
+	dark_blue:    'RColorClassic'
+	dark_green:   'RColorClassic'
+	dark_aqua:    'RColorClassic'
+	dark_red:     'RColorClassic'
+	dark_purple:  'RColorClassic'
+	gold:         'RColorClassic'
+	gray:         'RColorClassic'
+	dark_gray:    'RColorClassic'
+	blue:         'RColorClassic'
+	green:        'RColorClassic'
+	aqua:         'RColorClassic'
+	red:          'RColorClassic'
+	light_purple: 'RColorClassic'
+	yellow:       'RColorClassic'
+	white:        'RColorClassic'
 
-	reset:        'RColor'
+	reset:        'RColorClassic'
 
 	def __init__(self, rgb_code: int):
 		class_util.check_type(rgb_code, int)
 		self._rgb_code: int = rgb_code  # e.g. 0xRRGGBB
 
 	@classmethod
 	def from_mc_value(cls, value: str) -> 'RColor':
@@ -158,15 +158,15 @@
 	def b(self) -> int:
 		"""
 		The blue portion of the color in [0, 255]
 		"""
 		return (self._rgb_code >> 0) & 0xFF
 
 
-def __register_legacy_rcolor():
+def __register_classic_rcolor():
 	def register(name: str, rgb_hex: int, mc_code: str, console_code: str):
 		RColor.register_item(name, RColorClassic(name, rgb_hex, mc_code, console_code))
 
 	register('black',        0x000000, '§0', Fore.BLACK)
 	register('dark_blue',    0x0000AA, '§1', Fore.BLUE)
 	register('dark_green',   0x00AA00, '§2', Fore.GREEN)
 	register('dark_aqua',    0x00AAAA, '§3', Fore.CYAN)
@@ -183,25 +183,25 @@
 	register('yellow',       0xFFFF55, '§e', Fore.LIGHTYELLOW_EX)
 	register('white',        0xFFFFFF, '§f', Fore.WHITE)
 
 	# default text color is white, so use 0xFFFFFF
 	register('reset',        0xFFFFFF, '§r', Style.RESET_ALL)
 
 
-class RColorClassic(RItemLegacy, RColor):
+class RColorClassic(RItemClassic, RColor):
 	"""
 	Classic Minecraft text color defined with color name
 
 	.. attention::
 
 		Do not construct the class yourself. Use class fields in :class:`RColor` if you want to use classic colors
 	"""
 	def __init__(self, name: str, rgb_code: int, mc_code: str, console_code: str):
 		super().__init__(name, mc_code, console_code)
-		super(RItemLegacy, self).__init__(rgb_code)
+		super(RItemClassic, self).__init__(rgb_code)
 		self.__rgb_cache: Optional['RColorRGB'] = None
 
 	def to_rgb(self) -> 'RColorRGB':
 		"""
 		Converts to the corresponding :class:`RColorRGB` object with the exact same color
 		"""
 		if self.__rgb_cache is None:  # concurrency invocation is fine
@@ -282,15 +282,15 @@
 	# Interface implementation
 
 	@property
 	def name(self) -> str:
 		return '#{:06X}'.format(self._rgb_code)
 
 
-__register_legacy_rcolor()
+__register_classic_rcolor()
 
 
 # ------------------------------------------------
 #                   Text Style
 # ------------------------------------------------
 
 
@@ -298,34 +298,36 @@
 	pass
 
 
 class RStyle(RItem, ABC, metaclass=__RStyleMeta):
 	"""
 	Minecraft text styles
 	"""
-	bold:          'RStyle'
-	italic:        'RStyle'
-	underlined:    'RStyle'
-	strikethrough: 'RStyle'
-	obfuscated:    'RStyle'
+	bold:          'RStyleClassic'
+	italic:        'RStyleClassic'
+	underlined:    'RStyleClassic'
+	strikethrough: 'RStyleClassic'
+	obfuscated:    'RStyleClassic'
 
 
 def __register_rstyle():
 	def register(name: str, mc_code: str, console_code: str):
-		RStyle.register_item(name, _RStyleImpl(name, mc_code, console_code))
+		RStyle.register_item(name, RStyleClassic(name, mc_code, console_code))
 
 	register('bold',          '§l', Style.BRIGHT)
 	register('italic',        '§o', '')
 	register('underlined',    '§n', '')
 	register('strikethrough', '§m', '')
 	register('obfuscated',    '§k', '')
 
 
-class _RStyleImpl(RItemLegacy, RStyle):
-	pass
+class RStyleClassic(RItemClassic, RStyle):
+	"""
+	Classic Minecraft text style with corresponding "§"-prefixed formatting code
+	"""
 
 
 __register_rstyle()
 
 
 # ------------------------------------------------
 #                  Text Special
```

### Comparing `mcdreforged-2.8.4/mcdreforged/minecraft/rtext/text.py` & `mcdreforged-2.9.0/mcdreforged/minecraft/rtext/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from abc import ABC
 from typing import Iterable, List, Union, Optional, Any, Tuple, Set, NamedTuple
 
 from colorama import Style
 from typing_extensions import Self
 
-from mcdreforged.minecraft.rtext.style import RStyle, RColor, RAction, RColorClassic, RColorRGB, RItemLegacy
+from mcdreforged.minecraft.rtext.style import RStyle, RColor, RAction, RColorClassic, RColorRGB, RItemClassic
 
 
 class RTextBase(ABC):
 	"""
 	An abstract base class of Minecraft text component
 	"""
 	def to_json_object(self) -> Union[dict, list]:
@@ -338,15 +338,15 @@
 		if isinstance(self.__color, RColorClassic):
 			color = self.__color.console_code
 		elif isinstance(self.__color, RColorRGB):
 			color = self.__color.to_classic().console_code
 		else:
 			color = ''
 		for style in self.__styles:
-			if isinstance(style, RItemLegacy):
+			if isinstance(style, RItemClassic):
 				color += style.console_code
 		return color + self.to_plain_text() + Style.RESET_ALL
 
 	def _copy_from(self, text: 'RText'):
 		self.__text = text.__text
 		self.__color = text.__color
 		self.__styles = text.__styles.copy()
```

### Comparing `mcdreforged-2.8.4/mcdreforged/permission/permission_level.py` & `mcdreforged-2.9.0/mcdreforged/permission/permission_level.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/permission/permission_manager.py` & `mcdreforged-2.9.0/mcdreforged/permission/permission_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 			if meta.description is not None:
 				source.reply(meta.get_description_rtext())
 
 	def __execute_and_report_plugin_manipulate(
 			self, source: CommandSource, operation_name: str, func: Callable[[], Future[PluginOperationResult]],
 			plugin_alias: str, result_type_to_check_success: PluginResultType
 	):
-		ret = self.function_call(source, func, operation_name, log_success=False, msg_args=(plugin_alias,))
+		ret = self.function_call(source, func, operation_name, reply_success=False, msg_args=(plugin_alias,))
 		if ret.no_error:
 			def report(result: PluginOperationResult):
 				if result.get_if_success(result_type_to_check_success):
 					source.reply(self.tr('mcdr_command.{}.success'.format(operation_name), plugin_alias))
 				else:
 					source.reply(self.tr('mcdr_command.{}.fail'.format(operation_name), plugin_alias))
 
@@ -183,9 +183,9 @@
 	def load_plugin(self, source: CommandSource, file_name: str):
 		self.__not_loaded_plugin_file_manipulate(source, file_name, self.plugin_manager.load_plugin, 'load_plugin', self.server_interface.get_unloaded_plugin_list())
 
 	def enable_plugin(self, source: CommandSource, file_name: str):
 		self.__not_loaded_plugin_file_manipulate(source, file_name, self.plugin_manager.enable_plugin, 'enable_plugin', self.server_interface.get_disabled_plugin_list())
 
 	def reload_all_plugin(self, source: CommandSource):
-		ret = self.function_call(source, self.mcdr_server.plugin_manager.refresh_all_plugins, 'reload_all_plugin', log_success=False)
+		ret = self.function_call(source, self.mcdr_server.plugin_manager.refresh_all_plugins, 'reload_all_plugin', reply_success=False)
 		self._print_plugin_operation_result_if_no_error(source, ret)
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 			then(Literal({'plugin', 'plg'}).runs(self.refresh_changed_plugins)).
 			then(Literal({'config', 'cfg'}).runs(self.reload_config)).
 			then(Literal({'permission', 'perm'}).runs(self.reload_permission)).
 			then(Literal('all').runs(self.reload_all))
 		)
 
 	def refresh_changed_plugins(self, source: CommandSource):
-		ret = self.function_call(source, self.mcdr_server.plugin_manager.refresh_changed_plugins, 'refresh_changed_plugins', log_success=False)
+		ret = self.function_call(source, self.mcdr_server.plugin_manager.refresh_changed_plugins, 'refresh_changed_plugins', reply_success=False)
 		self._print_plugin_operation_result_if_no_error(source, ret)
 
 	def reload_config(self, source: CommandSource):
 		self.function_call(source, self.mcdr_server.load_config, 'reload_config')
 
 	def reload_permission(self, source: CommandSource):
 		self.function_call(source, self.mcdr_server.permission_manager.load_permission_file, 'reload_permission')
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 				tree_printer.print_tree(
 					psutil.Process(process.pid),
 					lambda proc: proc.children(),
 					lambda proc: '{}: {}'.format(proc.name(), proc.pid),
 					lambda line: source.reply('  ' + line)
 				)
 			except psutil.NoSuchProcess:
-				self.mcdr_server.logger.exception('Fail to fetch process tree from pid {}', process.pid)
+				self.mcdr_server.logger.exception('Fail to fetch process tree from pid {}'.format(process.pid))
 
 		source.reply(self.tr('mcdr_command.print_mcdr_status.extra.queue', self.mcdr_server.task_executor.task_queue.qsize(), core_constant.MAX_TASK_QUEUE_SIZE))
 
 		source.reply(self.tr('mcdr_command.print_mcdr_status.extra.thread', threading.active_count()))
 		thread_pool_counts = 0
 		for thread in threading.enumerate():
 			name = thread.name
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,18 +80,21 @@
 
 	def _print_plugin_operation_result_if_no_error(self, source: CommandSource, ret: FunctionCallResult[Future[PluginOperationResult]]):
 		if ret.no_error:
 			def reply(result: PluginOperationResult):
 				source.reply(result.to_rtext(self.mcdr_server, show_path=source.has_permission(PermissionLevel.PHYSICAL_SERVER_CONTROL_LEVEL)))
 			ret.return_value.add_done_callback(reply)
 
-	def function_call(self, source: CommandSource, func: Callable[[], T], name: str, log_success=True, log_fail=True, msg_args=()) -> FunctionCallResult[T]:
+	def function_call(
+			self, source: CommandSource, func: Callable[[], T], name: str, *,
+			reply_success: bool = True, reply_fail: bool = True, msg_args: tuple = ()
+	) -> FunctionCallResult[T]:
 		try:
 			ret = FunctionCallResult(func(), True)
-			if log_success:
+			if reply_success:
 				source.reply(self.tr('mcdr_command.{}.success'.format(name), *msg_args))
 			return ret
 		except Exception:
-			if log_fail:
+			if reply_fail:
 				source.reply(self.tr('mcdr_command.{}.fail'.format(name), *msg_args))
 			self.mcdr_server.logger.error(traceback.format_exc())
 			return FunctionCallResult(None, False)
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,42 +10,44 @@
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.check_update_command import CheckUpdateCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.debug_command import DebugCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.help_command import HelpCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.permission_command import PermissionCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.plugin_command import PluginCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.preference_command import PreferenceCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.reload_command import ReloadCommand
+from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.server_command import ServerCommand
 from mcdreforged.plugin.builtin.mcdreforged_plugin.commands.status_command import StatusCommand
 from mcdreforged.plugin.meta.metadata import Metadata
 from mcdreforged.plugin.type.permanent_plugin import PermanentPlugin
 from mcdreforged.translation.translation_text import RTextMCDRTranslation
 
 METADATA = {
 	'id': core_constant.PACKAGE_NAME,
 	'version': core_constant.VERSION,
 	'name': core_constant.NAME,
 	'description': 'The core of {}'.format(core_constant.NAME),
 	'author': [
 		'Fallen_Breath'
 	],
-	'link': 'https://github.com/Fallen-Breath/MCDReforged'
+	'link': core_constant.GITHUB_URL
 }
 
 
 class MCDReforgedPlugin(PermanentPlugin):
 	def __init__(self, plugin_manager):
 		super().__init__(plugin_manager)
 		self._set_metadata(Metadata(METADATA, plugin=self))
 		self.command_check_update = CheckUpdateCommand(self)
 		self.command_debug = DebugCommand(self)
 		self.command_help = HelpCommand(self)
 		self.command_permission = PermissionCommand(self)
 		self.command_plugin = PluginCommand(self)
 		self.command_preference = PreferenceCommand(self)
 		self.command_reload = ReloadCommand(self)
+		self.command_server = ServerCommand(self)
 		self.command_status = StatusCommand(self)
 
 	def tr(self, key: str, *args, **kwargs) -> RTextMCDRTranslation:
 		return self.server_interface.rtr(key, *args, **kwargs)
 
 	def load(self):
 		self.plugin_registry.clear()
@@ -76,14 +78,15 @@
 			on_child_error(UnknownArgument, self.on_mcdr_command_unknown_argument).
 			then(self.command_check_update.get_command_node()).
 			then(self.command_debug.get_command_node()).
 			then(self.command_permission.get_command_node()).
 			then(self.command_plugin.get_command_node()).
 			then(self.command_preference.get_command_node()).
 			then(self.command_reload.get_command_node()).
+			then(self.command_server.get_command_node()).
 			then(self.command_status.get_command_node())
 		)
 		self.register_command(self.command_help.get_command_node())
 
 	# --------------------
 	#    Command Stuffs
 	# --------------------
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/builtin/python_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/builtin/python_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/meta/dependency_walker.py` & `mcdreforged-2.9.0/mcdreforged/plugin/meta/dependency_walker.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/meta/metadata.py` & `mcdreforged-2.9.0/mcdreforged/plugin/meta/metadata.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/meta/version.py` & `mcdreforged-2.9.0/mcdreforged/plugin/meta/version.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/operation_result.py` & `mcdreforged-2.9.0/mcdreforged/plugin/operation_result.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/plugin_event.py` & `mcdreforged-2.9.0/mcdreforged/plugin/plugin_event.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/plugin_factory.py` & `mcdreforged-2.9.0/mcdreforged/plugin/plugin_factory.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/plugin_manager.py` & `mcdreforged-2.9.0/mcdreforged/plugin/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/plugin_registry.py` & `mcdreforged-2.9.0/mcdreforged/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/plugin_thread.py` & `mcdreforged-2.9.0/mcdreforged/plugin/plugin_thread.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/server_interface.py` & `mcdreforged-2.9.0/mcdreforged/plugin/server_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import functools
 import json
 import logging
 import os
-import time
 from typing import Callable, TYPE_CHECKING, Tuple, Any, Union, Optional, List, IO, Dict, Type, TypeVar
 
 import psutil
 
 from mcdreforged.command.builder.nodes.basic import Literal
 from mcdreforged.command.command_source import CommandSource, PluginCommandSource, PlayerCommandSource, ConsoleCommandSource
 from mcdreforged.constants import plugin_constant
@@ -150,94 +149,124 @@
 
 	def start(self) -> bool:
 		"""
 		Start the server. Return if the action succeed.
 
 		If the server is running or being starting by other plugin it will return ``False``
 
-		:return: If the action succeed
+		:return: If the operation succeed.
+			The operation fails if the server is already started, or cannot start due to invalid command or current MCDR state
 		"""
 		return self._mcdr_server.start_server()
 
-	def stop(self) -> None:
+	def stop(self) -> bool:
 		"""
 		Soft shutting down the server by sending the correct stop command to the server
 
 		This option will not stop MCDR. MCDR will keep running unless :meth:`exit` is invoked
+
+		:return: If the operation succeed.
+			The operation fails if the server is already stopped
 		"""
 		self._mcdr_server.remove_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
-		self._mcdr_server.stop(forced=False)
+		return self._mcdr_server.stop(forced=False)
 
-	def kill(self) -> None:
+	def kill(self) -> bool:
 		"""
 		Kill the entire server process group. A hard shutting down
 
 		MCDR will keep running unless :meth:`exit` is invoked
+
+		:return: If the operation succeed.
+			The operation fails if the server is already stopped
 		"""
-		self._mcdr_server.stop(forced=True)
+		return self._mcdr_server.stop(forced=True)
+
+	def wait_until_stop(self) -> None:
+		"""
+		Wait until the server is stopped
+
+		.. note:: The current thread will be blocked
+		"""
+		cv = self._mcdr_server.server_state_cv
+		with cv:
+			while self.is_server_running():
+				cv.wait(0.1)
 
 	def wait_for_start(self) -> None:
 		"""
-		Wait until the server is able to start. In other words, wait until the server is stopped
+		Wait until the server is able to start
+
+		Actually it's an alias of :meth:`wait_until_stop`
 		"""
-		while self.is_server_running():
-			time.sleep(0.01)
+		self.wait_until_stop()
 
-	def restart(self) -> None:
+	def restart(self) -> bool:
 		"""
 		Restart the server
 
 		It will first :meth:`soft stop <stop>` the server
 		and then :meth:`wait <wait_for_start>` until the server is stopped,
-		finally :meth:start <start>` the server up
+		finally :meth:`start <start>` the server up
+
+		:return: If the operation succeed.
+			The operation fails if the server is already stopped
 		"""
-		if self.is_server_running():
-			self.stop()
-			self.wait_for_start()
-			self.start()
+		if not self.stop():
+			return False
+		self.wait_for_start()
+		return self.start()
 
-	def stop_exit(self) -> None:
+	def stop_exit(self) -> bool:
 		"""
 		:meth:`soft stop <stop>` the server and exit MCDR
+
+		:return: If the operation succeed.
+			The operation fails if the server is already stopped
 		"""
-		self._mcdr_server.stop(forced=False)
+		ok = self._mcdr_server.stop(forced=False)
+		if ok:
+			self._mcdr_server.add_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
+		return ok
 
-	def exit(self) -> None:
+	def exit(self) -> bool:
 		"""
 		Exit MCDR when the server is stopped
 
 		Basically it's the same to invoking :meth:`set_exit_after_stop_flag` with parameter ``True``,
 		but with an extra server not running check
 
 		Example usage::
 
 			server.stop()  # Stop the server
 			# do something A
 			server.wait_for_start()  # Make sure the server is fully stopped. It's necessary to run it in your custom thread
 			# do something B
 			server.exit()  # Exit MCDR
 
-		:raise IllegalCallError: If the server is not stopped
+		:return: If the operation succeed.
+			The operation fails if the server is still running
 		"""
 		if self._mcdr_server.is_server_running():
-			raise IllegalCallError('Cannot exit MCDR when the server is running')
-		self._mcdr_server.with_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
+			return False
+		self._mcdr_server.add_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
+		return True
 
 	def set_exit_after_stop_flag(self, flag_value: bool) -> None:
 		"""
 		Set the flag that indicating if MCDR should exit when the server has stopped
 
 		If set to ``True``, after the server stops MCDR will exit, otherwise (set to ``False``) MCDR will just keep running
 
 		The flag value will be set to ``True`` everytime when the server starts
 
 		The flag value is displayed in line 5 in command ``!!MCDR status``
 		"""
 		if flag_value:
-			self._mcdr_server.with_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
+			self._mcdr_server.add_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
 		else:
 			self._mcdr_server.remove_flag(MCDReforgedFlag.EXIT_AFTER_STOP)
 
 	def is_server_running(self) -> bool:
 		"""
 		Return if the server is running
 		"""
@@ -309,15 +338,17 @@
 
 			:meth:`execute_command` if you want to execute command in MCDR's command system
 
 		:param text: The content of the command you want to send
 		:param encoding: The encoding method for the text.
 			Leave it empty to use the encoding method from the configuration of MCDR
 		"""
-		self.logger.debug('Sending command "{}"'.format(text), option=DebugOption.PLUGIN)
+		logger = self.logger
+		if isinstance(logger, MCDReforgedLogger):  # make type checker happy
+			logger.debug('Sending command "{}"'.format(text), option=DebugOption.PLUGIN)
 		self._mcdr_server.send(text, encoding=encoding)
 
 	@property
 	def __server_handler(self) -> 'AbstractServerHandler':
 		return self._mcdr_server.server_handler_manager.get_current_handler()
 
 	def tell(self, player: str, text: MessageText, *, encoding: Optional[str] = None) -> None:
@@ -490,15 +521,15 @@
 		"""
 		future: Future[PluginOperationResult] = handler(self._mcdr_server.plugin_manager)(plugin_file_path)
 		if future.is_finished():
 			return future.get().get_if_success(PluginResultType.LOAD)  # the operations are always loading a plugin
 		else:
 			return False  # TODO handle unknown result caused by chained sync plugin operation
 
-	def __existed_regular_plugin_manipulate(self, plugin_id: str, handler: Callable[['PluginManager'], Callable[['RegularPlugin'], Any]],result_type: PluginResultType) -> Optional[bool]:
+	def __existed_regular_plugin_manipulate(self, plugin_id: str, handler: Callable[['PluginManager'], Callable[['RegularPlugin'], Any]], result_type: PluginResultType) -> Optional[bool]:
 		"""
 		Manipulate a loaded regular plugin from a given plugin id
 		:param plugin_id: The plugin id of the plugin you want to manipulate
 		:param handler: What callable you want to use with Plugin Manager to the plugin id,
 		the returned callable accepts the plugin instance
 		:param result_type: The type of the result. It's used to determine how to get the single operation result from the plugin operation result.
 		It's used to determine if the operation succeeded
```

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/directory_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/directory_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/multi_file_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/multi_file_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/packed_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/packed_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/permanent_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/permanent_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/regular_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/regular_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/plugin/type/solo_plugin.py` & `mcdreforged-2.9.0/mcdreforged/plugin/type/solo_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/preference/preference_manager.py` & `mcdreforged-2.9.0/mcdreforged/preference/preference_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/resources/default_config.yml` & `mcdreforged-2.9.0/mcdreforged/resources/default_config.yml`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/resources/lang/en_us.yml` & `mcdreforged-2.9.0/mcdreforged/resources/lang/en_us.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,18 @@
     start_fail: Fail to start the server
     pid_info: Server is running at PID {0}
   stop:
     stop_when_stopped: Server cannot stop when terminated
     stop_fail: Error stopping server, force the server to stop now
   kill_server:
     killing: Killing server process group
-    process_killed: Process {0} killed
+    process_killed: Process {0} (pid {1}) killed
   interrupt:
-    hint: Interrupting, first strike = {0}
+    soft: Interrupting MCDR, first strike. Interrupt again to kill the servers
+    hard: Interrupting MCDR and killing the servers
   send:
     send_when_stopped:
       .: Server has been terminated, cannot send command to its stdin
       text: 'Command being sent: {0}'
   receive:
     wait_stop: Waiting for server process to stop
     decode_fail: 'Fail to decode text {0}: {1}'
@@ -118,14 +119,15 @@
     .: |
       §7!!MCDR§r: Show this message
       §7!!MCDR checkupdate§r: Check update from Github
       §7!!MCDR permission§r: Show permission command help message
       §7!!MCDR plugin§r: Show plugin command help message
       §7!!MCDR preference§r: Show preference command help message
       §7!!MCDR reload§r: Show reload command help message
+      §7!!MCDR server§r: Show server command help message
       §7!!MCDR status§r: Show MCDR status
     reload: |
       §7!!MCDR reload plugin§r: Load / Reload / Unloaded §lchanged§r plugins
       §7!!MCDR reload config§r: Reload config file
       §7!!MCDR reload permission§r: Reload permission file
       §7!!MCDR reload all§r: Reload everything above
     permission: |
@@ -144,14 +146,21 @@
       §7!!MCDR plugin disable §6<plugin_id>§r: Disable a plugin with id §6<plugin_id>§r
       §7!!MCDR plugin reloadall§r: Load / Reload / Unloaded §lall§r not disabled plugins
     preference: |
       §7!!MCDR preference list§r: Display the preference list
       §7!!MCDR preference §e<pref_name>§r: Display the details of preference §e<pref_name>§r
       §7!!MCDR preference §e<pref_name>§r set §6<value>§r: Set the value of preference §e<pref_name>§r to §6<value>§r
       §7!!MCDR preference §e<pref_name>§r reset: Reset preference §e<pref_name>§r to the default value
+    server: |
+      §7!!MCDR server start§r: Start the server
+      §7!!MCDR server stop§r: Stop the server, but keep MCDR running
+      §7!!MCDR server stop_exit§r: Stop the server and exit MCDR
+      §7!!MCDR server exit§r: Exit MCDR. The server should already be stopped
+      §7!!MCDR server restart§r: Restart the server
+      §7!!MCDR server kill§r: Kill the server, and all of its child processes
     debug: |
       §7!!MCDR debug thread_dump §6[#all|<thread_name>]§r: Dump stack trace information of given threads
       §7!!MCDR debug translation get §6<translation_key>§r: Get the translation dict for given translation key
       §7!!MCDR debug translation dump §6<json_path>§r: Dump all translations starting with given path, e.g. "mcdr_server.on_server_stop"
       §7!!MCDR debug command_dump all§r: Dump all command trees
       §7!!MCDR debug command_dump plugin §6<plugin_id>§r: Dump all command trees registered by given plugin
       §7!!MCDR debug command_dump node §6<literal_name>§r: Dump all command trees with root with given name
@@ -244,14 +253,29 @@
       suggestions: 'Suggestions: {0}'
       current: Current value
       default: Default value
       set_suggestion_hint: Click to set the value of preference {0} to {1}
     set:
       done: Set preference {0} to {1}
     unknown_language: Unknown language {0}
+  server:
+    start.success: Starting the server
+    start.failed: Failed to start the server
+    stop.success: Stopping the server
+    stop.failed: Failed to stop the server
+    stop_exit.success: Stopping the server and exiting MCDR
+    stop_exit.failed: Failed to start the server and exit MCDR
+    exit.success: Exiting MCDR
+    exit.failed: Failed to exit MCDR. Make sure the server has already stopped
+    restart.success: Restarting the server, do not spam
+    restart.failed: Failed to restart the server
+    restart.spam: The server is already restarting
+    kill.success: Killed the server process group
+    kill.failed: Failed to kill the server
+    see_console: Check the console for more information
 python_plugin:
   info: '{0} is running on {1} environment'
 
 # ======================== plugin peripherals ========================
 
 plugin_operation_result:
   info_loaded_succeeded: 'Loaded: §7{0}§r plugins'
```

### Comparing `mcdreforged-2.8.4/mcdreforged/resources/lang/zh_cn.yml` & `mcdreforged-2.9.0/mcdreforged/resources/lang/zh_cn.yml`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,19 @@
     starting: 正在启动服务端，启动参数为 "{0}"
     start_fail: 服务端启动失败
     pid_info: 服务端正在以 PID {0} 运行中
   stop:
     stop_when_stopped: 服务端不能在关闭时再次关闭
     stop_fail: 服务端关闭出错，强制关闭
   kill_server:
-    killing: 正在终止服务端进程组
-    process_killed: 进程 {0} 已终止
+    killing: 正在杀死服务端进程组
+    process_killed: 进程 {0} (pid {1}) 已杀死
   interrupt:
-    hint: 中断 MCDR 中，首次操作 = {0}
+    soft: 正在终止 MCDR。再次执行以强制杀死服务端
+    hard: 正在终止 MCDR 并杀死服务端
   send:
     send_when_stopped:
       .: 服务端已关闭，不能向其标准输入流输入指令
       text: '被输入的指令: {0}'
   receive:
     wait_stop: 等待服务端进程停止
     decode_fail: '解析文本 {0} 出错: {1}'
@@ -118,14 +119,15 @@
     .: |
       §7!!MCDR§r: 显示这条消息
       §7!!MCDR checkupdate§r: 从 Github 检测更新
       §7!!MCDR permission§r: 显示权限相关的帮助信息
       §7!!MCDR plugin§r: 显示插件相关的帮助信息
       §7!!MCDR preference§r: 显示偏好相关的帮助信息
       §7!!MCDR reload§r: 显示重载相关的帮助信息
+      §7!!MCDR server§r: 显示控制服务端相关的帮助信息
       §7!!MCDR status§r: 显示 MCDR 状态
     reload: |
       §7!!MCDR reload plugin§r: 加载 / 重载 / 卸载§l有修改的§r插件
       §7!!MCDR reload config§r: 重载配置文件
       §7!!MCDR reload permission§r: 重载权限文件
       §7!!MCDR reload all§r: 重载上述所有
     permission: |
@@ -144,14 +146,21 @@
       §7!!MCDR plugin disable §6<plugin_id>§r: 禁用 id 为 §6<plugin_id>§r 的插件
       §7!!MCDR plugin reloadall§r: 加载 / 重载 / 卸载§l所有§r插件
     preference: |
       §7!!MCDR preference list§r: 显示偏好列表
       §7!!MCDR preference §e<pref_name>§r: 显示偏好 §e<pref_name>§r 的详情
       §7!!MCDR preference §e<pref_name>§r set §6<value>§r: 设定偏好 §e<pref_name>§r 的值为 §6<value>§r
       §7!!MCDR preference §e<pref_name>§r reset: 将偏好 §e<pref_name>§r 重置为默认值
+    server: |
+      §7!!MCDR server start§r: 启动服务端
+      §7!!MCDR server stop§r: 关闭服务端，且 MCDR 会继续运行
+      §7!!MCDR server stop_exit§r: 关闭服务端并退出 MCDR
+      §7!!MCDR server exit§r: 退出 MCDR。服务端应已关闭
+      §7!!MCDR server restart§r: 重启服务端
+      §7!!MCDR server kill§r: 杀死服务端，以及其所有子进程
     debug: |
       §7!!MCDR debug thread_dump §6[#all|<thread_name>]§r: 导出所有指定线程的堆栈追踪信息
       §7!!MCDR debug translation get §6<translation_key>§r: 导出给定翻译键的翻译信息
       §7!!MCDR debug translation dump §6<json_path>§r: 导出以给定路径为前缀的所有翻译键，例如 "mcdr_server.on_server_stop"
       §7!!MCDR debug command_dump all§r: 导出所有指令树
       §7!!MCDR debug command_dump plugin §6<plugin_id>§r: 导出给定插件注册的所有指令树
       §7!!MCDR debug command_dump node §6<literal_name>§r: 导出树根为给定名字所有指令树
@@ -246,14 +255,29 @@
       suggestions: '建议选项: {0}'
       current: 当前值
       default: 默认值
       set_suggestion_hint: 点击以将偏好 {0} 的值设置为 {1}
     set:
       done: 已将偏好 "{0}" 设置为 "{1}"
     unknown_language: 未知的语言 {0}
+  server:
+    start.success: 正在启动服务端
+    start.failed: 启动服务端失败
+    stop.success: 正在关闭服务端
+    stop.failed: 关闭服务端失败
+    stop_exit.success: 正在关闭服务端并退出MCDR
+    stop_exit.failed: 启动服务端并退出MCDR失败
+    exit.success: 正在退出MCDR
+    exit.failed: 退出MCDR失败，请确保服务端已关闭
+    restart.success: 正在重启服务端
+    restart.failed: 重启服务端失败
+    restart.spam: 服务端已在重启中，勿重复操作
+    kill.success: 已杀死服务端进程组
+    kill.failed: 杀死服务端失败
+    see_console: 见控制台以了解详情信息
 python_plugin:
   info: '{0}正于{1}环境中运行'
 
 # ======================== plugin peripherals ========================
 
 plugin_operation_result:
   info_loaded_succeeded: '共加载: §7{0}§r 个插件'
```

### Comparing `mcdreforged-2.8.4/mcdreforged/translation/translation_manager.py` & `mcdreforged-2.9.0/mcdreforged/translation/translation_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/translation/translation_text.py` & `mcdreforged-2.9.0/mcdreforged/translation/translation_text.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/class_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/class_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/file_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/future.py` & `mcdreforged-2.9.0/mcdreforged/utils/future.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/logger.py` & `mcdreforged-2.9.0/mcdreforged/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from enum import Enum, unique, auto
 from threading import RLock, local
 from typing import Dict, Optional, List, Set
 
 from colorlog import ColoredFormatter
 
 from mcdreforged.constants import core_constant
-from mcdreforged.minecraft.rtext.style import RColor, RStyle, RItemLegacy
+from mcdreforged.minecraft.rtext.style import RColor, RStyle, RItemClassic
 from mcdreforged.utils import string_util, file_util
 
 
 @unique
 class DebugOption(Enum):
 	# remember to sync with the debug field in the default config file
 	ALL = auto()
@@ -57,15 +57,15 @@
 			try:
 				inst.stream = stream
 			finally:
 				inst.release()
 
 
 class MCColorFormatControl:
-	MC_CODE_ITEMS: List[RItemLegacy] = list(filter(lambda item: isinstance(item, RItemLegacy), list(RColor) + list(RStyle)))
+	MC_CODE_ITEMS: List[RItemClassic] = list(filter(lambda item: isinstance(item, RItemClassic), list(RColor) + list(RStyle)))
 
 	# global flag
 	console_color_disabled = False
 
 	__TLS = local()
 
 	@classmethod
```

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/misc_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/misc_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/resources_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/resources_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/serializer.py` & `mcdreforged-2.9.0/mcdreforged/utils/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,27 +390,47 @@
 				value = copy.copy(getattr(cls, attr_name))
 			if value is not _NONE:
 				setattr(self, attr_name, value)
 
 	def __init_from(self, data: dict):
 		self.__set_attributes(lambda attr_name: data.get(attr_name, _NONE), copy_default=True)
 
+	def merge_from(self, other: Self):
+		"""
+		Merge attributes from another instance into the current one
+
+		.. note::
+
+			It won't create copies of the attribute values being merged
+
+			If you want the merged values to be independent, you can make a :meth:`deep copy <copy>`
+			of the other object first, and then merge from the copy
+
+		:param other: The other object to merge attributes from
+
+		.. versionadded:: v2.9.0
+		"""
+		self.__set_attributes(lambda attr_name: getattr(other, attr_name, _NONE), copy_default=False)
+
 	def copy(self, *, deep: bool = True) -> Self:
 		"""
 		Make a copy of the object. Only fields declared in the class annotation will be copied
 
 		By default, a deep copy will be made
 
-		:keyword deep: If this operation make a deep copy
+		:keyword deep: If this operation make a deep copy. True: deep copy, False: shallow copy
 
 		.. versionadded:: v2.8.0
+
+		.. versionadded:: v2.9.0
+			Added ``deep`` keyword argument
 		"""
 		def value_provider(attr_name: str):
 			value = getattr(self, attr_name, _NONE)
-			if value is not _NONE:
+			if deep and value is not _NONE:
 				if isinstance(value, Serializable):
 					value = value.copy()
 				else:
 					value = deserialize(serialize(value), type(value))
 			return value
 
 		other = self.get_default()
```

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/string_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/thread_local_storage.py` & `mcdreforged-2.9.0/mcdreforged/utils/thread_local_storage.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/translation_util.py` & `mcdreforged-2.9.0/mcdreforged/utils/translation_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/tree_printer.py` & `mcdreforged-2.9.0/mcdreforged/utils/tree_printer.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged/utils/yaml_data_storage.py` & `mcdreforged-2.9.0/mcdreforged/utils/yaml_data_storage.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.4/mcdreforged.egg-info/PKG-INFO` & `mcdreforged-2.9.0/mcdreforged.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdreforged
-Version: 2.8.4
+Version: 2.9.0
 Summary: A rewritten version of MCDaemon, a python script to control your Minecraft server
 Home-page: https://github.com/Fallen-Breath/MCDReforged
 Author: Fallen_Breath
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `mcdreforged-2.8.4/mcdreforged.egg-info/SOURCES.txt` & `mcdreforged-2.9.0/mcdreforged.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/check_update_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py
+mcdreforged/plugin/builtin/mcdreforged_plugin/commands/server_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py
 mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py
 mcdreforged/plugin/meta/__init__.py
 mcdreforged/plugin/meta/dependency_walker.py
 mcdreforged/plugin/meta/metadata.py
 mcdreforged/plugin/meta/version.py
 mcdreforged/plugin/type/__init__.py
```

### Comparing `mcdreforged-2.8.4/setup.py` & `mcdreforged-2.9.0/setup.py`

 * *Files identical despite different names*

