# Comparing `tmp/dan-build-0.2.2.tar.gz` & `tmp/dan-build-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.2.tar", last modified: Fri May 19 06:38:37 2023, max compression
+gzip compressed data, was "dan-build-0.2.3.tar", last modified: Sat May 20 13:57:28 2023, max compression
```

## Comparing `dan-build-0.2.2.tar` & `dan-build-0.2.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.503644 dan-build-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 06:38:28.000000 dan-build-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 06:38:37.499644 dan-build-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 06:38:28.000000 dan-build-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.487644 dan-build-0.2.2/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cmake/configure_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.495644 dan-build-0.2.2/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.495644 dan-build-0.2.2/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-19 06:38:28.000000 dan-build-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:38:37.503644 dan-build-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_smc_catch2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 13:57:20.000000 dan-build-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-20 13:57:28.105941 dan-build-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-20 13:57:20.000000 dan-build-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.093941 dan-build-0.2.3/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 13:57:20.000000 dan-build-0.2.3/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cmake/configure_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.097941 dan-build-0.2.3/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.101941 dan-build-0.2.3/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 13:57:20.000000 dan-build-0.2.3/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 13:57:28.000000 dan-build-0.2.3/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-20 13:57:20.000000 dan-build-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:57:28.105941 dan-build-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:57:28.105941 dan-build-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-20 13:57:20.000000 dan-build-0.2.3/tests/test_cxx_smc_catch2.py
```

### Comparing `dan-build-0.2.2/LICENSE` & `dan-build-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/PKG-INFO` & `dan-build-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.2/README.md` & `dan-build-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/completion/bash/dan-io.sh` & `dan-build-0.2.3/completion/bash/dan-io.sh`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,17 @@
             COMPREPLY=()
             compopt -o dirnames
         elif [[ $type == 'file' ]]; then
             COMPREPLY=()
             compopt -o default
         elif [[ $type == 'plain' ]]; then
             COMPREPLY+=($value)
+        elif [[ $type == 'nospace' ]]; then
+            COMPREPLY+=($value)
+            compopt -o nospace
         fi
     done
 
     return 0
 }
 
 _dan_io_completion_setup() {
```

### Comparing `dan-build-0.2.2/completion/bash/dan.sh` & `dan-build-0.2.3/completion/bash/dan.sh`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,17 @@
             COMPREPLY=()
             compopt -o dirnames
         elif [[ $type == 'file' ]]; then
             COMPREPLY=()
             compopt -o default
         elif [[ $type == 'plain' ]]; then
             COMPREPLY+=($value)
+        elif [[ $type == 'nospace' ]]; then
+            COMPREPLY+=($value)
+            compopt -o nospace
         fi
     done
 
     return 0
 }
 
 _dan_completion_setup() {
```

### Comparing `dan-build-0.2.2/completion/zsh/dan-io.sh` & `dan-build-0.2.3/completion/zsh/dan-io.sh`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     local -a completions_with_descriptions
     local -a response
     (( ! $+commands[dan-io] )) && return 1
 
     response=("${(@f)$(env COMP_WORDS="${words[*]}" COMP_CWORD=$((CURRENT-1)) _DAN_IO_COMPLETE=zsh_complete 'dan-io')}")
 
     for type key descr in ${response}; do
-        if [[ "$type" == "plain" ]]; then
+        if [[ "$type" =~ ^(plain|nospace)$ ]]; then
             if [[ "$descr" == "_" ]]; then
                 completions+=("$key")
             else
                 completions_with_descriptions+=("$key":"$descr")
             fi
         elif [[ "$type" == "dir" ]]; then
             _path_files -/
@@ -23,13 +23,17 @@
     done
 
     if [ -n "$completions_with_descriptions" ]; then
         _describe -V unsorted completions_with_descriptions -U
     fi
 
     if [ -n "$completions" ]; then
-        compadd -U -V unsorted -a completions
+        if [[ "$type" == "nospace" ]]; then
+            compadd -U -S '' -V unsorted -a completions
+        else
+            compadd -U -V unsorted -a completions
+        fi
     fi
 }
 
 compdef _dan_io_completion dan-io;
```

### Comparing `dan-build-0.2.2/completion/zsh/dan.sh` & `dan-build-0.2.3/completion/zsh/dan.sh`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     local -a completions_with_descriptions
     local -a response
     (( ! $+commands[dan] )) && return 1
 
     response=("${(@f)$(env COMP_WORDS="${words[*]}" COMP_CWORD=$((CURRENT-1)) _DAN_COMPLETE=zsh_complete dan)}")
 
     for type key descr in ${response}; do
-        if [[ "$type" == "plain" ]]; then
+        if [[ "$type" =~ ^(plain|nospace)$ ]]; then
             if [[ "$descr" == "_" ]]; then
                 completions+=("$key")
             else
                 completions_with_descriptions+=("$key":"$descr")
             fi
         elif [[ "$type" == "dir" ]]; then
             _path_files -/
@@ -23,13 +23,17 @@
     done
 
     if [ -n "$completions_with_descriptions" ]; then
         _describe -V unsorted completions_with_descriptions -U
     fi
 
     if [ -n "$completions" ]; then
-        compadd -U -V unsorted -a completions
+        if [[ "$type" == "nospace" ]]; then
+            compadd -U -S '' -V unsorted -a completions
+        else
+            compadd -U -V unsorted -a completions
+        fi
     fi
 }
 
 compdef _dan_completion dan;
```

### Comparing `dan-build-0.2.2/dan/cli/io.py` & `dan-build-0.2.3/dan/cli/io.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cli/main.py` & `dan-build-0.2.3/dan/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import sys
+import logging
+import asyncio
 
 from dan.core.find import find_file
 from dan.core.pathlib import Path
 from dan.cli import click
 
-import logging
-import asyncio
 from dan.core.cache import Cache
 from dan.cxx.targets import Executable
+from dan.core.settings import Settings
 
 
 from dan.make import ConfigCache, InstallMode, Make
 from dan.cli.vscode import Code
 
 
 _minimal_options = [
@@ -94,15 +95,15 @@
 
 
 @cli.command()
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--toolchain', '-t', help='The toolchain to use',
               type=_toolchain_choice)
-@click.option('--setting', '-s', 'settings', help='Set or change a setting', multiple=True)
+@click.option('--setting', '-s', 'settings', help='Set or change a setting', multiple=True, type=click.SettingsParamType(Settings))
 @click.option('--option', '-o', 'options', help='Set or change an option', multiple=True)
 @click.option('--build-path', '-B', help='Path where dan has been initialized.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='build')
 @click.option('--source-path', '-S', help='Path where source is located.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='.')
 async def configure(verbose: bool, toolchain: str, settings: tuple[str], options: tuple[str], build_path: Path, source_path: Path):
     """Configure dan project"""
```

### Comparing `dan-build-0.2.2/dan/cli/vscode.py` & `dan-build-0.2.3/dan/cli/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cmake/configure_file.py` & `dan-build-0.2.3/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/conan/requirements.py` & `dan-build-0.2.3/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/aiofiles.py` & `dan-build-0.2.3/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/asyncio.py` & `dan-build-0.2.3/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/cache.py` & `dan-build-0.2.3/dan/core/cache.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/find.py` & `dan-build-0.2.3/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/functools.py` & `dan-build-0.2.3/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/generator.py` & `dan-build-0.2.3/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/include.py` & `dan-build-0.2.3/dan/core/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     source_path = Path(module.__file__).parent
     if parent is None and context.current is not None:
         parent = context.current
 
     if build_path is None:
         assert parent is not None
         build_path = build_path or parent.build_path / name
-    build_path.mkdir(parents=True, exist_ok=True)
 
     module.__class__ = MakeFile
     context.current = module
     module._setup(
         name,
         source_path,
         build_path,
```

### Comparing `dan-build-0.2.2/dan/core/makefile.py` & `dan-build-0.2.3/dan/core/makefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,7 +151,14 @@
     @property
     def default(self):
         return [target for target in self.targets if target.default == True]
 
     @property
     def all_default(self):
         return [target for target in self.all_targets if target.default == True]
+    
+    @cached_property
+    def root(self):
+        m = self
+        while m.parent is not None:
+            m = m.parent
+        return m
```

### Comparing `dan-build-0.2.2/dan/core/osinfo.py` & `dan-build-0.2.3/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/pathlib.py` & `dan-build-0.2.3/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/pm.py` & `dan-build-0.2.3/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/register.py` & `dan-build-0.2.3/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/requirements.py` & `dan-build-0.2.3/dan/core/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/runners.py` & `dan-build-0.2.3/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/settings.py` & `dan-build-0.2.3/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/target.py` & `dan-build-0.2.3/dan/core/target.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/test.py` & `dan-build-0.2.3/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/utils.py` & `dan-build-0.2.3/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/version.py` & `dan-build-0.2.3/dan/core/version.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/core/win.py` & `dan-build-0.2.3/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/__init__.py` & `dan-build-0.2.3/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/compile_commands.py` & `dan-build-0.2.3/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/detect.py` & `dan-build-0.2.3/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.3/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/support/qt.py` & `dan-build-0.2.3/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/targets.py` & `dan-build-0.2.3/dan/cxx/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     async def __build__(self):
         self.info(f'generating {self.output}...')
         commands = await self.toolchain.compile(self.source, self.output, self.private_cxx_flags)
         self.cache['compile_args'] = [str(a) for a in commands[0]]
         self.info(f'scanning dependencies of {self.source}')
         deps = await self.toolchain.scan_dependencies(self.source, self.private_cxx_flags, self.build_path)
         deps = [d for d in deps
-                if self.source_path in Path(d).parents
+                if self.makefile.root.source_path in Path(d).parents
                 or self.build_path in Path(d).parents]
         self.cache['deps'] = deps
 
 
 class OptionSet:
     def __init__(self, parent: 'CXXTarget',
                  name: str,
```

### Comparing `dan-build-0.2.2/dan/cxx/toolchain.py` & `dan-build-0.2.3/dan/cxx/toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/cxx/unix_toolchain.py` & `dan-build-0.2.3/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/io/package.py` & `dan-build-0.2.3/dan/io/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,24 +52,32 @@
                 for version in avail_versions:
                     if self.spec.is_compatible(version):
                         self.debug(f'using version {version} to match {self.spec}')
                         self.version = version
                         break
 
         packages_path = get_packages_path()
+        
         from dan.cxx import target_toolchain as toolchain
         self._build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / self.package / str(self.version)
         self.install_settings = InstallSettings(self.build_path)
-
+        
+        # update package build-path
         makefile = self.package_makefile
-        for target in makefile.all_installed:
-            target.package_name = f'{self.package}:{target.name}'
+        makefile.build_path = self.build_path / 'build'
+
+        # set package version
+        if self.version:
+            makefile.options.get('version').value = str(self.version)
 
-        self.output = Path(self.install_settings.libraries_prefix) / 'pkgconfig' / f'{target.package_name}.pc'
-        sources.output = 'src' # TODO source_prefix in install settings
+        # set our output to the last installed package
+        # TODO handle multiple outputs, then set our outputs to all installed packages
+        pkg_name = makefile.all_installed[-1].name     
+        self.output = Path(self.install_settings.libraries_prefix) / 'pkgconfig' / f'{pkg_name}.pc'
+        sources.output = self.build_path / 'src' # TODO source_prefix in install settings
 
         return await super().__initialize__()
     
     @property
     def build_path(self) -> Path:
         return self._build_path
     
@@ -79,18 +87,14 @@
             self.debug(f'{ident} already built by {self._all_builds[ident].fullname}')
             await self._all_builds[ident].build()
             return
 
         self._all_builds[ident] = self
 
         makefile = self.package_makefile
-        makefile.build_path = self.build_path / 'build'
-
-        if self.version:
-            makefile.options.get('version').value = str(self.version)
 
         async with asyncio.TaskGroup(f'installing {self.package}\'s targets') as group:
             for target in makefile.all_installed:
                 group.create_task(target.install(self.install_settings, InstallMode.dev))
 
         makefile.cache.ignore()
         del makefile
```

### Comparing `dan-build-0.2.2/dan/io/repositories.py` & `dan-build-0.2.3/dan/io/repositories.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,31 @@
 from dan.core.runners import async_run
 from dan.core import aiofiles
 from dan.core.cache import Cache
 
 from dataclasses_json import dataclass_json
 from dataclasses import dataclass, field
 
+import typing as t
+
 
 @dataclass
 class RepositoryConfig:
     name: str
     url: str
     branch: str = 'main'
 
+@dataclass
+class GitHubConfig:
+    api_token: str = None
 
 @dataclass_json
 @dataclass
 class RepositoriesSettings:
+    github: GitHubConfig = field(default_factory=lambda: GitHubConfig())
     repositories: list[RepositoryConfig] = field(default_factory=lambda: [
         RepositoryConfig('dan.io', 'https://github.com/Garcia6l20/dan.io.git'),
     ])
 
     def get(self, name):
         for config in self.repositories:
             if config.name == name:
```

### Comparing `dan-build-0.2.2/dan/jinja.py` & `dan-build-0.2.3/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/logging.py` & `dan-build-0.2.3/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/make.py` & `dan-build-0.2.3/dan/make.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/pkgconfig/package.py` & `dan-build-0.2.3/dan/pkgconfig/package.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/src/git.py` & `dan-build-0.2.3/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/dan/src/github.py` & `dan-build-0.2.3/dan/src/github.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,16 +42,26 @@
                 raise RuntimeError(f'cannot resolve url of {self.name}')
             self.cache['url'] = self._url
 
     @asyncio.cached
     async def available_versions(self) -> dict[Version, dict]:
         self.info('fetching github releases')
 
+
+        api_token = None
+
+        from dan.io.repositories import _get_settings
+        settings = _get_settings()
+        if settings.github.api_token is not None:
+            api_token = settings.github.api_token
+
         url = f'https://api.github.com/repos/{self.user}/{self.project}/releases'
         async with aiohttp.ClientSession() as session:
+            if api_token is not None:
+                session.headers['Authorization'] = f'Bearer {api_token}'
             async with session.get(url) as resp:
                 data = await resp.read()
                 if resp.status != 200:
                     raise RuntimeError(f'unable to fetch {url}: {data.decode()}')
                 releases = json.loads(data)
                 return {Version(release['tag_name']): release for release in releases}
```

### Comparing `dan-build-0.2.2/dan/src/tar.py` & `dan-build-0.2.3/dan/src/tar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from click import Path
 import tqdm
-from dan.core import aiofiles
+from dan.core import aiofiles, asyncio
 from dan.core.target import Target
 import aiohttp
 import tarfile
 import zipfile
 
 
 async def fetch_file(url, dest: Path):
@@ -42,8 +42,10 @@
             with zipfile.ZipFile(self.build_path / archive_name) as f:
                 root = os.path.commonprefix(f.namelist())
                 f.extractall(self.output.parent)
         else:
             with tarfile.open(self.build_path / archive_name) as f:
                 root = os.path.commonprefix(f.getnames())
                 f.extractall(self.output.parent)
-        os.rename(self.output.parent / root, self.output)
+        async with asyncio.TaskGroup() as g:
+            g.create_task(aiofiles.os.rename(self.output.parent / root, self.output))
+            g.create_task(aiofiles.os.remove(self.build_path / archive_name))
```

### Comparing `dan-build-0.2.2/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.3/dan_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.2/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.3/dan_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/pyproject.toml` & `dan-build-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/tests/test_cxx_libraries.py` & `dan-build-0.2.3/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/tests/test_cxx_simple.py` & `dan-build-0.2.3/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.2/tests/test_cxx_smc_catch2.py` & `dan-build-0.2.3/tests/test_cxx_smc_catch2.py`

 * *Files identical despite different names*

