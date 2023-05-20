# Comparing `tmp/types-setuptools-67.7.0.3.tar.gz` & `tmp/types-setuptools-67.8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-67.7.0.3.tar", last modified: Fri May 19 06:18:47 2023, max compression
+gzip compressed data, was "types-setuptools-67.8.0.0.tar", last modified: Sat May 20 09:12:52 2023, max compression
```

## Comparing `types-setuptools-67.7.0.3.tar` & `types-setuptools-67.8.0.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.270707 types-setuptools-67.7.0.3/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/pkg_resources-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/py312compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.001527 types-setuptools-67.8.0.0/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/pkg_resources-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.005527 types-setuptools-67.8.0.0/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.009527 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.009527 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/py312compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-67.7.0.3/CHANGELOG.md` & `types-setuptools-67.8.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+## 67.8.0.0 (2023-05-20)
+
+[stubsabot] Bump setuptools to 67.8.* (#10194)
+
+Release: https://pypi.org/pypi/setuptools/67.8.0
+Homepage: https://github.com/pypa/setuptools
+Changelog: https://setuptools.pypa.io/en/stable/history.html
+Diff: https://github.com/pypa/setuptools/compare/v67.7.2...v67.8.0
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 2 files included in typeshed's stubs have been modified or renamed: `setuptools/command/easy_install.py`, `setuptools/version.py`.
+ - Total lines of Python code added: 425.
+ - Total lines of Python code deleted: 215.
+
+---------
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 67.7.0.3 (2023-05-19)
 
 Don't ignore missing stubs in setuptools (#10058)
 
 ## 67.7.0.2 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
```

### Comparing `types-setuptools-67.7.0.3/PKG-INFO` & `types-setuptools-67.8.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.3
+Version: 67.8.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
+This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
```

### Comparing `types-setuptools-67.7.0.3/pkg_resources-stubs/__init__.pyi` & `types-setuptools-67.8.0.0/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setup.py` & `types-setuptools-67.8.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
+This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
 '''.lstrip()
 
 setup(name=name,
-      version="67.7.0.3",
+      version="67.8.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
```

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/__init__.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/archive_util.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/build_meta.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/build_py.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/develop.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/easy_install.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 def get_exe_prefixes(exe_filename): ...
 
 class PthDistributions(Environment):
     dirty: bool
     filename: Any
     sitedirs: Any
     basedir: Any
+    paths: list[str]
     def __init__(self, filename, sitedirs=()) -> None: ...
     def save(self) -> None: ...
     def add(self, dist) -> None: ...
     def remove(self, dist) -> None: ...
     def make_relative(self, path): ...
 
 class RewritePthDistributions(PthDistributions):
```

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/editable_wheel.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/sdist.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/setopt.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/test.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/config/expand.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/depends.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/discovery.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/dist.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/errors.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/extension.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/msvc.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/package_index.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/setuptools-stubs/sandbox.pyi` & `types-setuptools-67.8.0.0/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.3/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-67.8.0.0/types_setuptools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.3
+Version: 67.8.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
+This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
```

### Comparing `types-setuptools-67.7.0.3/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-67.8.0.0/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

