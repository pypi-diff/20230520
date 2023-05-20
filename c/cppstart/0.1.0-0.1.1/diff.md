# Comparing `tmp/cppstart-0.1.0.tar.gz` & `tmp/cppstart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppstart-0.1.0.tar", last modified: Thu May 18 18:59:18 2023, max compression
+gzip compressed data, was "cppstart-0.1.1.tar", last modified: Sat May 20 19:46:04 2023, max compression
```

## Comparing `cppstart-0.1.0.tar` & `cppstart-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.855672 cppstart-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.835672 cppstart-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.843672 cppstart-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-18 18:59:03.000000 cppstart-0.1.0/.github/workflows/build_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-18 18:59:03.000000 cppstart-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 18:59:03.000000 cppstart-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-18 18:59:03.000000 cppstart-0.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-18 18:59:03.000000 cppstart-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-18 18:59:18.855672 cppstart-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-18 18:59:03.000000 cppstart-0.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-18 18:59:03.000000 cppstart-0.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-18 18:59:03.000000 cppstart-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.843672 cppstart-0.1.0/e2e_test/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-18 18:59:03.000000 cppstart-0.1.0/e2e_test/cppstart-tests.bats
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.843672 cppstart-0.1.0/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 18:59:03.000000 cppstart-0.1.0/packaging/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-18 18:59:03.000000 cppstart-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:59:18.855672 cppstart-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.843672 cppstart-0.1.0/src/cppstart/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/build_system_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/ci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/cpp_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/dependency_management_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/file_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/license_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/source_control_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/source_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/build_system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/build.ps1
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/src/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/test/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/build_system/cmake/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/ci/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_debug.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_debug.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/deps_mgmt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart/templates/deps_mgmt/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/deps_mgmt/conan/conanfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/deps_mgmt/conan/init.ps1
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/deps_mgmt/conan/init.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.851673 cppstart-0.1.0/src/cppstart/templates/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/AGPL-3.0-or-later
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/Apache-2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/BSL-1.0
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/GPL-3.0-or-later
--rw-r--r--   0 runner    (1001) docker     (123)    42802 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/LGPL-3.0-or-later
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/MIT
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/MPL-2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/licenses/Unlicense
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.851673 cppstart-0.1.0/src/cppstart/templates/projects/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/projects/default/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.839672 cppstart-0.1.0/src/cppstart/templates/source_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.851673 cppstart-0.1.0/src/cppstart/templates/source_control/git/
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-18 18:59:03.000000 cppstart-0.1.0/src/cppstart/templates/source_control/git/template.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.847673 cppstart-0.1.0/src/cppstart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 18:59:18.000000 cppstart-0.1.0/src/cppstart.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:59:18.855672 cppstart-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_build_system_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_ci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_cpp_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_dependency_management_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_file_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_license_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_source_control_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-18 18:59:03.000000 cppstart-0.1.0/tests/test_source_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.452379 cppstart-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.440379 cppstart-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-20 19:45:53.000000 cppstart-0.1.1/.github/workflows/build_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-20 19:45:53.000000 cppstart-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-20 19:45:53.000000 cppstart-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-20 19:45:53.000000 cppstart-0.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 19:45:53.000000 cppstart-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-20 19:46:04.452379 cppstart-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-20 19:45:53.000000 cppstart-0.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-20 19:45:53.000000 cppstart-0.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-05-20 19:45:53.000000 cppstart-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/e2e_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-20 19:45:53.000000 cppstart-0.1.1/e2e_test/cppstart-tests.bats
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 19:45:53.000000 cppstart-0.1.1/packaging/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-20 19:45:53.000000 cppstart-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:46:04.452379 cppstart-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.440379 cppstart-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/build_system_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/ci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/cpp_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/dependency_management_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/file_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/license_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/source_control_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/source_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/build_system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/build.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/build_system/cmake/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/ci/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_debug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_debug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/deps_mgmt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/deps_mgmt/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/deps_mgmt/conan/conanfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/deps_mgmt/conan/init.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/deps_mgmt/conan/init.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/AGPL-3.0-or-later
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/Apache-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/BSL-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/GPL-3.0-or-later
+-rw-r--r--   0 runner    (1001) docker     (123)    42802 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/LGPL-3.0-or-later
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/MPL-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/licenses/Unlicense
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/projects/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/projects/default/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.444379 cppstart-0.1.1/src/cppstart/templates/source_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart/templates/source_control/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-20 19:45:53.000000 cppstart-0.1.1/src/cppstart/templates/source_control/git/template.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.448379 cppstart-0.1.1/src/cppstart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 19:46:04.000000 cppstart-0.1.1/src/cppstart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:46:04.452379 cppstart-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_build_system_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_ci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_cpp_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_dependency_management_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_file_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_license_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_source_control_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-20 19:45:53.000000 cppstart-0.1.1/tests/test_source_generator.py
```

### Comparing `cppstart-0.1.0/.github/workflows/build_and_test.yml` & `cppstart-0.1.1/.github/workflows/build_and_test.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/.github/workflows/release.yml` & `cppstart-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/.gitmodules` & `cppstart-0.1.1/.gitmodules`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/PKG-INFO` & `cppstart-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: cppstart
-Version: 0.1.0
-Summary: Simplify the correct initialisation of C++ projects
-Author-email: Kevin J Channon <kevinchannon+cppstart@gmail.com>
-License: MIT
-Keywords: C++,libraries
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # CPP Start
 `cppstart` is a simple command-line tool to initialise a reasonable C++ project.
 ## Motivation
 When you first start writing C++, you will likely be confronted with an instruction like this:
 1. Make a file that looks like this and save it to main.cpp:
     ```c++
    #include <iostream>
@@ -47,14 +36,15 @@
 ### (Meta) dependencies
 The project that you create with cppstart will have a bunch of things that it needs for smooth running. These include:
 * Git
 * Some kind of C++ compiler (MSVC++, GCC, Clang, whatever)
 * CMake
 * Conan
 * Clang-Format
+
 To initialise the project, then you'll need a connection to the internet too, since it will need to pull down Catch2 to use for unit testing your code.
 
 ## Creating a C++ project
 Say you want to create a new C++ application called "foo" in the current directory. Then just do:
 ```shell
 cppstart foo
 ```
@@ -92,28 +82,33 @@
 |-- SECURITY.md
 |-- build.ps1               <--\    These build files can be called from the command line to
 |-- build.sh*                   |-- build your code. There are shell and Powerhell versions
 |                           <--/    that do the same thing, for running on Windows or Linux
 |-- conanfile.txt           <--- This pulls in third-party dependencies via Conan. It's used
 |                                by the "init" scripts. You can add new dependencies to it, as
 |                                your project develops and you need more third-party libs 
-|-- /examples               <--- Help your users with some working examples of how your code works
+|-- /examples               <--- Help your users with some working examples of how your code
+|                                works. If you created an APP project, then this directory
+|                                won't be here. You will run your project via src/main.cpp
+|                                instead.
 |   |-- CMakeLists.txt
 |  `-- main.cpp
 |-- /include                <--- The header files go in here.
 |   `-- /foo
 |       `-- foo.hpp
 |-- init.ps1                <--\    These files are called when you first create the project, to
 |-- init.sh*                    |-- pull in the dependencies that the project requires to build.
 |                           <--/    There are shell and Powershell versions, for Linux and Windows
 |-- /src                    <--- Your project sources go in here
 |   |-- CMakeLists.txt
 |   |-- /foo
 |   |   `-- foo.cpp 
-|   `-- main.cpp
+|   `-- main.cpp            <--- This is the "main" file for your app. If you created a LIB
+|                                project, then this file won't be here. You'll run your library
+|                                code via the examples and the tests in that case.
 `-- /test                   <--- The unit tests for your project go in here. There is an initial
     |                            (failing) test to get you going :)
     |-- CMakeLists.txt
     `-- foo.test.cpp
 ```
 
 ## Initialise and build your project
@@ -160,15 +155,15 @@
 cd weebles
 git remote add origin git@github.com:aishaadeboye/weebles.git
 git push -u origin main
 ```
 The way Github workflows work means that you won't generate any CI run on this first push, but the next one (and all the other ones after that) will.  This means that it's a good idea to get on with fixing the failing test by replacing it with one for some new code that you're writing; otherwise you'll get a test run failure on Github. How embarrassing!
 
 ## Releasing your code
-There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on. Push that tag and then run a the "Release" action in the Gitub actions page for your project. This will produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
+There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on and push that tag. When Github sees that tag arrive in the repo, it will trigger the Release workflow and produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
 ```shell
 git tag v1.2.3
 git push --tags
 ```
 Then go trigger the "release" action on Github.
 
 ## All the options
@@ -213,8 +208,8 @@
   -o OUTPUT_DIRECTORY, --output-directory OUTPUT_DIRECTORY
                         output directory
   -s SOURCE_CONTROL, --source-control SOURCE_CONTROL
                         the type of source control that the project will use. Valid options are:
                           - git
 
 ```
-You can see these options by doing `cppstart -h`.
+You can see these options by doing `cppstart -h`.
```

### Comparing `cppstart-0.1.0/Pipfile.lock` & `cppstart-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/README.md` & `cppstart-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: cppstart
+Version: 0.1.1
+Summary: Simplify the correct initialisation of C++ projects
+Author-email: Kevin J Channon <kevinchannon+cppstart@gmail.com>
+License: MIT
+Project-URL: Documentation, https://github.com/kevinchannon/cppstart
+Project-URL: Source, https://github.com/kevinchannon/cppstart
+Keywords: C++,libraries
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # CPP Start
 `cppstart` is a simple command-line tool to initialise a reasonable C++ project.
 ## Motivation
 When you first start writing C++, you will likely be confronted with an instruction like this:
 1. Make a file that looks like this and save it to main.cpp:
     ```c++
    #include <iostream>
@@ -36,14 +49,15 @@
 ### (Meta) dependencies
 The project that you create with cppstart will have a bunch of things that it needs for smooth running. These include:
 * Git
 * Some kind of C++ compiler (MSVC++, GCC, Clang, whatever)
 * CMake
 * Conan
 * Clang-Format
+
 To initialise the project, then you'll need a connection to the internet too, since it will need to pull down Catch2 to use for unit testing your code.
 
 ## Creating a C++ project
 Say you want to create a new C++ application called "foo" in the current directory. Then just do:
 ```shell
 cppstart foo
 ```
@@ -81,28 +95,33 @@
 |-- SECURITY.md
 |-- build.ps1               <--\    These build files can be called from the command line to
 |-- build.sh*                   |-- build your code. There are shell and Powerhell versions
 |                           <--/    that do the same thing, for running on Windows or Linux
 |-- conanfile.txt           <--- This pulls in third-party dependencies via Conan. It's used
 |                                by the "init" scripts. You can add new dependencies to it, as
 |                                your project develops and you need more third-party libs 
-|-- /examples               <--- Help your users with some working examples of how your code works
+|-- /examples               <--- Help your users with some working examples of how your code
+|                                works. If you created an APP project, then this directory
+|                                won't be here. You will run your project via src/main.cpp
+|                                instead.
 |   |-- CMakeLists.txt
 |  `-- main.cpp
 |-- /include                <--- The header files go in here.
 |   `-- /foo
 |       `-- foo.hpp
 |-- init.ps1                <--\    These files are called when you first create the project, to
 |-- init.sh*                    |-- pull in the dependencies that the project requires to build.
 |                           <--/    There are shell and Powershell versions, for Linux and Windows
 |-- /src                    <--- Your project sources go in here
 |   |-- CMakeLists.txt
 |   |-- /foo
 |   |   `-- foo.cpp 
-|   `-- main.cpp
+|   `-- main.cpp            <--- This is the "main" file for your app. If you created a LIB
+|                                project, then this file won't be here. You'll run your library
+|                                code via the examples and the tests in that case.
 `-- /test                   <--- The unit tests for your project go in here. There is an initial
     |                            (failing) test to get you going :)
     |-- CMakeLists.txt
     `-- foo.test.cpp
 ```
 
 ## Initialise and build your project
@@ -149,15 +168,15 @@
 cd weebles
 git remote add origin git@github.com:aishaadeboye/weebles.git
 git push -u origin main
 ```
 The way Github workflows work means that you won't generate any CI run on this first push, but the next one (and all the other ones after that) will.  This means that it's a good idea to get on with fixing the failing test by replacing it with one for some new code that you're writing; otherwise you'll get a test run failure on Github. How embarrassing!
 
 ## Releasing your code
-There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on. Push that tag and then run a the "Release" action in the Gitub actions page for your project. This will produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
+There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on and push that tag. When Github sees that tag arrive in the repo, it will trigger the Release workflow and produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
 ```shell
 git tag v1.2.3
 git push --tags
 ```
 Then go trigger the "release" action on Github.
 
 ## All the options
@@ -202,8 +221,8 @@
   -o OUTPUT_DIRECTORY, --output-directory OUTPUT_DIRECTORY
                         output directory
   -s SOURCE_CONTROL, --source-control SOURCE_CONTROL
                         the type of source control that the project will use. Valid options are:
                           - git
 
 ```
-You can see these options by doing `cppstart -h`.
+You can see these options by doing `cppstart -h`.
```

### Comparing `cppstart-0.1.0/e2e_test/cppstart-tests.bats` & `cppstart-0.1.1/e2e_test/cppstart-tests.bats`

 * *Files 24% similar despite different names*

```diff
@@ -6,23 +6,39 @@
     load 'test_helper/bats-file/load'
     DIR="$( cd "$( dirname "$BATS_TEST_FILENAME" )" >/dev/null 2>&1 && pwd )"
     PATH="$DIR/../src:$PATH"
 }
 
 teardown_file() {
     rm -rf foo
+    rm -rf bar
 }
 
-@test "creates a directory for the new project" {
+@test "creates a directory for a new application project" {
   cppstart foo -c "some user"
   assert_exist foo
 }
 
-@test "new project dependencies can be resolved out of the box" {
+@test "new app project dependencies can be resolved out of the box" {
   cd foo
   ./init.sh
 }
 
-@test "new project can be built out of the box" {
+@test "new app project can be built out of the box" {
   cd foo
   ./build.sh
+}
+
+@test "creates a directory for a new library project" {
+  cppstart --lib bar -c "User 2"
+  assert_exist bar
+}
+
+@test "new lib project dependencies can be resolved out of the box" {
+  cd bar
+  ./init.sh
+}
+
+@test "new lib project can be built out of the box" {
+  cd bar
+  ./build.sh
 }
```

### Comparing `cppstart-0.1.0/src/cppstart/build_system_generator.py` & `cppstart-0.1.1/src/cppstart/dependency_management_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from pathlib import Path
-
-from file_access import FileReader
-from file_info import FileInfo
-from generator import Generator
-
-
-class BuildSystemGenerator(Generator):
-    def run(self) -> set[FileInfo]:
-        files = super().run()
-
-        for p in [Path("build.sh"), Path("build.ps1")]:
-            build_script = next((f for f in files if f.path == p), None)
-            if build_script is not None:
-                build_script.permissions = 0o755
-
-        return files
-
-
-def make_build_system_generator(build_sys_name: str, proj_name: str, template_root_dir: Path):
-    return BuildSystemGenerator({"proj_name": proj_name}, FileReader(template_root_dir / build_sys_name))
+from pathlib import Path
+
+from file_access import FileReader
+from file_info import FileInfo
+from generator import Generator
+
+
+class DepsManagementGenerator(Generator):
+    def run(self) -> set[FileInfo]:
+        files = super().run()
+
+        for p in [Path("init.sh"), Path("init.ps1")]:
+            build_script = next((f for f in files if f.path == p), None)
+            if build_script is not None:
+                build_script.permissions = 0o755
+
+        return files
+
+
+def make_dependency_namagement_generator(dep_mgr_name: str, build_sys_name: str, template_root_dir: Path):
+    return DepsManagementGenerator({"build_sys_name": build_sys_name}, FileReader(template_root_dir / dep_mgr_name))
```

### Comparing `cppstart-0.1.0/src/cppstart/config.py` & `cppstart-0.1.1/src/cppstart/config.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/cpp_start.py` & `cppstart-0.1.1/src/cppstart/cpp_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 def make_cppstart(args, config: Config) -> CppStart:
     return CppStart(make_source_generator(args.project_type, args.proj_name,
                                           get_source_code_preamble(spdx_id=get_license(args).spdx_id,
                                                                    year=str(datetime.now().year),
                                                                    copyright_name=get_copyright_name(args, config))),
-                    make_build_system_generator(args.build_system, args.proj_name, BUILD_SYSTEM_TEMPLATES_DIR),
+                    make_build_system_generator(args.build_system, args.proj_name, args.project_type, BUILD_SYSTEM_TEMPLATES_DIR),
                     make_dependency_namagement_generator(args.dependency_management, args.build_system, DEPENDENCY_MANAGER_TEMPLATES_DIR),
                     make_source_control_generator(args.source_control, SOURCE_CONTROL_TEMPLATES_DIR),
                     make_ci_generator(args.ci, args.proj_name, CI_TEMPLATES_DIR))
 
 
 def get_license(args) -> License:
     return LicenseGenerator(licences=get_license_paths(LICENSE_TEMPLATES_DIR), default="MIT",
```

### Comparing `cppstart-0.1.0/src/cppstart/file_access.py` & `cppstart-0.1.1/src/cppstart/file_access.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/generator.py` & `cppstart-0.1.1/src/cppstart/generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/license_generator.py` & `cppstart-0.1.1/src/cppstart/license_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/main.py` & `cppstart-0.1.1/src/cppstart/main.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/source_control_generator.py` & `cppstart-0.1.1/src/cppstart/source_control_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/source_generator.py` & `cppstart-0.1.1/src/cppstart/source_generator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         else:
             self._include = self._INCLUDE
             self._examples_main = self._EXAMPLES_MAIN.format(self._proj_name)
             self._test_src = self._TEST_SRC.format(self._proj_name)
 
     def run(self) -> set[FileInfo]:
         return {FileInfo(Path("include") / self._proj_name / f"{self._proj_name}.hpp", self._include),
-                FileInfo(Path("examples") / "main.cpp", self._examples_main),
                 FileInfo(Path("test") / f"{self._proj_name}.tests.cpp", self._test_src)}
 
 
 class AppSourceGenerator(__SourceGeneratorBase):
     def __init__(self, project_name: str, license_text=None):
         super().__init__(project_name, license_text)
 
@@ -87,14 +86,15 @@
             self._proj_src = self._LICENSED_SOURCE.format(self._license_text, proj_src)
         else:
             self._proj_src = proj_src
 
     def run(self) -> set[FileInfo]:
         base_content = super().run()
         return {*base_content,
+                FileInfo(Path("examples") / "main.cpp", self._examples_main),
                 FileInfo(Path("src") / self._proj_name / f"{self._proj_name}.cpp", self._proj_src)}
 
 
 def make_source_generator(project_type: ProjectType, project_name: str, license_text=None):
     if ProjectType.APP == project_type:
         return AppSourceGenerator(project_name, license_text)
     if ProjectType.LIB == project_type:
```

### Comparing `cppstart-0.1.0/src/cppstart/templates/build_system/cmake/CMakeLists.txt` & `cppstart-0.1.1/src/cppstart/templates/build_system/cmake/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 if (MASTER_PROJECT)
   # The GCC in MinGW requires this, for some reason.
   if(WIN32 AND CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
     set(CMAKE_CXX_STANDARD_LIBRARIES "-static-libgcc -static-libstdc++ -lwsock32 -lws2_32 ${CMAKE_CXX_STANDARD_LIBRARIES}")
     set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -Wl,-Bstatic,--whole-archive -lwinpthread -Wl,--no-whole-archive")
   endif()
 
-  add_subdirectory ("test")
-  add_subdirectory("examples")
+  add_subdirectory(test)
+  add_subdirectory(examples)
 
   set(package_files proj_name/  CMakeLists.txt)
   add_custom_command(OUTPUT ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}.${PROJECT_VERSION}.zip
     COMMAND ${CMAKE_COMMAND} -E tar c ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}.${PROJECT_VERSION}.zip --format=zip -- ${package_files}
     WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
     DEPENDS ${package_files})
   add_custom_target(${PROJECT_NAME}_package DEPENDS ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}.${PROJECT_VERSION}.zip)
```

### Comparing `cppstart-0.1.0/src/cppstart/templates/build_system/cmake/examples/CMakeLists.txt` & `cppstart-0.1.1/src/cppstart/templates/build_system/cmake/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/build_system/cmake/test/CMakeLists.txt` & `cppstart-0.1.1/src/cppstart/templates/build_system/cmake/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_debug.yml` & `cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_debug.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_release.yml` & `cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_ubuntu_gcc12_x64_release.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_debug.yml` & `cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_debug.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_release.yml` & `cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/build_and_test_windows_msvc_x64_release.yml`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/ci/github/.github/workflows/release.yml` & `cppstart-0.1.1/src/cppstart/templates/ci/github/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 name: Release
 permissions:
   contents: write
 
 on:
-    workflow_dispatch:
-        inputs:
-            version:
-                description: Version to release
-                default: v1.0.0
-                required: true
+  push:
+    tags:
+      - 'v*.*.*'
 
 jobs:
   release:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Create version number
         run: |
           mkdir -p build/package
-          echo ${{ github.event.inputs.version }} | sed 's/^v//' > build/package/version.txt
+          echo "${GITHUB_REF#refs/*/}" | sed 's/v//' > build/package/version.txt
 
       - name: Configure CMake
         run: cmake -B build/package -DPROJECT_VERSION:STRING=$(cat build/package/version.txt)
 
       - name: Package source code
         run: cmake --build build/package --target proj_name_package
 
@@ -33,9 +30,9 @@
 
       - name: Add packaged source code to release
         uses: svenstaro/upload-release-action@v2
         with:
           repo_token: ${{ secrets.GITHUB_TOKEN }}
           file_glob: true
           file: build/package/proj_name*
-          tag: ${{ github.event.inputs.version }}
+          tag: ${{ github.ref }}
           overwrite: true
```

### Comparing `cppstart-0.1.0/src/cppstart/templates/deps_mgmt/conan/init.sh` & `cppstart-0.1.1/src/cppstart/templates/deps_mgmt/conan/init.sh`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/AGPL-3.0-or-later` & `cppstart-0.1.1/src/cppstart/templates/licenses/AGPL-3.0-or-later`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/Apache-2.0` & `cppstart-0.1.1/src/cppstart/templates/licenses/Apache-2.0`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/BSL-1.0` & `cppstart-0.1.1/src/cppstart/templates/licenses/BSL-1.0`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/GPL-3.0-or-later` & `cppstart-0.1.1/src/cppstart/templates/licenses/GPL-3.0-or-later`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/LGPL-3.0-or-later` & `cppstart-0.1.1/src/cppstart/templates/licenses/LGPL-3.0-or-later`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/MIT` & `cppstart-0.1.1/src/cppstart/templates/licenses/MIT`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/MPL-2.0` & `cppstart-0.1.1/src/cppstart/templates/licenses/MPL-2.0`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/licenses/Unlicense` & `cppstart-0.1.1/src/cppstart/templates/licenses/Unlicense`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/projects/default/CODE_OF_CONDUCT.md` & `cppstart-0.1.1/src/cppstart/templates/projects/default/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/projects/default/README.md` & `cppstart-0.1.1/src/cppstart/templates/projects/default/README.md`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart/templates/source_control/git/template.gitignore` & `cppstart-0.1.1/src/cppstart/templates/source_control/git/template.gitignore`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/src/cppstart.egg-info/PKG-INFO` & `cppstart-0.1.1/src/cppstart.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: cppstart
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplify the correct initialisation of C++ projects
 Author-email: Kevin J Channon <kevinchannon+cppstart@gmail.com>
 License: MIT
+Project-URL: Documentation, https://github.com/kevinchannon/cppstart
+Project-URL: Source, https://github.com/kevinchannon/cppstart
 Keywords: C++,libraries
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # CPP Start
 `cppstart` is a simple command-line tool to initialise a reasonable C++ project.
@@ -47,14 +49,15 @@
 ### (Meta) dependencies
 The project that you create with cppstart will have a bunch of things that it needs for smooth running. These include:
 * Git
 * Some kind of C++ compiler (MSVC++, GCC, Clang, whatever)
 * CMake
 * Conan
 * Clang-Format
+
 To initialise the project, then you'll need a connection to the internet too, since it will need to pull down Catch2 to use for unit testing your code.
 
 ## Creating a C++ project
 Say you want to create a new C++ application called "foo" in the current directory. Then just do:
 ```shell
 cppstart foo
 ```
@@ -92,28 +95,33 @@
 |-- SECURITY.md
 |-- build.ps1               <--\    These build files can be called from the command line to
 |-- build.sh*                   |-- build your code. There are shell and Powerhell versions
 |                           <--/    that do the same thing, for running on Windows or Linux
 |-- conanfile.txt           <--- This pulls in third-party dependencies via Conan. It's used
 |                                by the "init" scripts. You can add new dependencies to it, as
 |                                your project develops and you need more third-party libs 
-|-- /examples               <--- Help your users with some working examples of how your code works
+|-- /examples               <--- Help your users with some working examples of how your code
+|                                works. If you created an APP project, then this directory
+|                                won't be here. You will run your project via src/main.cpp
+|                                instead.
 |   |-- CMakeLists.txt
 |  `-- main.cpp
 |-- /include                <--- The header files go in here.
 |   `-- /foo
 |       `-- foo.hpp
 |-- init.ps1                <--\    These files are called when you first create the project, to
 |-- init.sh*                    |-- pull in the dependencies that the project requires to build.
 |                           <--/    There are shell and Powershell versions, for Linux and Windows
 |-- /src                    <--- Your project sources go in here
 |   |-- CMakeLists.txt
 |   |-- /foo
 |   |   `-- foo.cpp 
-|   `-- main.cpp
+|   `-- main.cpp            <--- This is the "main" file for your app. If you created a LIB
+|                                project, then this file won't be here. You'll run your library
+|                                code via the examples and the tests in that case.
 `-- /test                   <--- The unit tests for your project go in here. There is an initial
     |                            (failing) test to get you going :)
     |-- CMakeLists.txt
     `-- foo.test.cpp
 ```
 
 ## Initialise and build your project
@@ -160,15 +168,15 @@
 cd weebles
 git remote add origin git@github.com:aishaadeboye/weebles.git
 git push -u origin main
 ```
 The way Github workflows work means that you won't generate any CI run on this first push, but the next one (and all the other ones after that) will.  This means that it's a good idea to get on with fixing the failing test by replacing it with one for some new code that you're writing; otherwise you'll get a test run failure on Github. How embarrassing!
 
 ## Releasing your code
-There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on. Push that tag and then run a the "Release" action in the Gitub actions page for your project. This will produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
+There's a good chance that you're embarking on your project because you think other people might find its features useful in some way.  In that case, you'll probably want to create releases to distribute to other people. To do this, you should tag your repo with a tag like `v1.2.3`, or whatever release number you're on and push that tag. When Github sees that tag arrive in the repo, it will trigger the Release workflow and produce things like a zip file of the code and things. There's a VERY high chance that you'll need to tweak things to get them the way you want them for your project, but the basics are kind of there to get you going (which is the point of this project :) ).  So, to create and push a tag, go for something like this:
 ```shell
 git tag v1.2.3
 git push --tags
 ```
 Then go trigger the "release" action on Github.
 
 ## All the options
```

### Comparing `cppstart-0.1.0/src/cppstart.egg-info/SOURCES.txt` & `cppstart-0.1.1/src/cppstart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_ci_generator.py` & `cppstart-0.1.1/tests/test_ci_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_config.py` & `cppstart-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_cpp_start.py` & `cppstart-0.1.1/tests/test_cpp_start.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,29 +95,26 @@
         self.assertTrue(isinstance(app._source_generator, LibSourceGenerator))
 
     def test_factory_creates_app_source_builder_when_args_has_is_app(self):
         args = get_command_line_parser([]).parse_args(["foo", "--app", "-c", "bar"])
         app = make_cppstart(args, self._empty_config)
         self.assertTrue(isinstance(app._source_generator, AppSourceGenerator))
 
-    def test_factory_write_the_expected_source_files(self):
+    def test_factory_write_the_expected_app_source_files(self):
         src_preamble = get_source_code_preamble("MIT", "2023", "Some Name")
         writer = FileReadWriter(Path("foo"))
         writer.write = MagicMock()
 
         args = get_command_line_parser([]).parse_args(["foo", "-c", "Some Name"])
         app = make_cppstart(args, self._empty_config)
         app.run(writer)
 
         write_calls = [
             call({FileInfo(Path("include/foo/foo.hpp"), f"{src_preamble}\n\n#include <cstdint>\n"),
                   FileInfo(Path(
-                      "examples/main.cpp"),
-                      f"{src_preamble}\n\n#include <foo/foo.hpp>\n\nauto main() -> int {{\n    return 0;\n}}\n"),
-                  FileInfo(Path(
                       "test/foo.tests.cpp"), f"{src_preamble}\n"
                                              f"\n"
                                              f"#include <foo/foo.hpp>\n"
                                              f"\n"
                                              f"#include <catch2/catch_test_macros.hpp>\n"
                                              f"\n"
                                              f"TEST_CASE(\"foo tests\") {{\n"
@@ -130,14 +127,46 @@
                       f"{src_preamble}\n\n#include <foo/foo.hpp>\n\nauto main() -> int {{\n    return 0;\n}}\n")
                   }
                  )
         ]
 
         writer.write.assert_has_calls(write_calls)
 
+    def test_factory_write_the_expected_lib_source_files(self):
+        src_preamble = get_source_code_preamble("MIT", "2023", "Some Name")
+        writer = FileReadWriter(Path("foo"))
+        writer.write = MagicMock()
+
+        args = get_command_line_parser([]).parse_args(["foo", "--lib", "-c", "Some Name"])
+        app = make_cppstart(args, self._empty_config)
+        app.run(writer)
+
+        write_calls = [
+            call({FileInfo(Path("include/foo/foo.hpp"), f"{src_preamble}\n\n#include <cstdint>\n"),
+                  FileInfo(Path(
+                      "examples/main.cpp"),
+                      f"{src_preamble}\n\n#include <foo/foo.hpp>\n\nauto main() -> int {{\n    return 0;\n}}\n"),
+                  FileInfo(Path(
+                      "test/foo.tests.cpp"), f"{src_preamble}\n"
+                                             f"\n"
+                                             f"#include <foo/foo.hpp>\n"
+                                             f"\n"
+                                             f"#include <catch2/catch_test_macros.hpp>\n"
+                                             f"\n"
+                                             f"TEST_CASE(\"foo tests\") {{\n"
+                                             f"    SECTION(\"delete this require and add your own tests!\")\n"
+                                             f"        REQUIRE(false);\n"
+                                             f"}}\n"),
+                  FileInfo(Path("src/foo/foo.cpp"), f"{src_preamble}\n\n#include <foo/foo.hpp>\n")
+                  }
+                 )
+        ]
+
+        writer.write.assert_has_calls(write_calls)
+
     def test_writes_files(self):
         src_gen = AppSourceGenerator("foo")
         src_gen.run = MagicMock(return_value={FileInfo(Path("Some/Path"), "some content")})
         writer = FileReadWriter(Path("foo"))
         writer.write = MagicMock()
 
         build_sys_template_reader = FileReader(Path("build_sys_template/dir"))
```

### Comparing `cppstart-0.1.0/tests/test_dependency_management_generator.py` & `cppstart-0.1.1/tests/test_dependency_management_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_file_access.py` & `cppstart-0.1.1/tests/test_file_access.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_generator.py` & `cppstart-0.1.1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_license_generator.py` & `cppstart-0.1.1/tests/test_license_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_project_type.py` & `cppstart-0.1.1/tests/test_project_type.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_source_control_generator.py` & `cppstart-0.1.1/tests/test_source_control_generator.py`

 * *Files identical despite different names*

### Comparing `cppstart-0.1.0/tests/test_source_generator.py` & `cppstart-0.1.1/tests/test_source_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     def test_adds_include_file(self, builder):
         files = builder.run()
 
         expected = next((f for f in files if f.path == Path("include/foo/foo.hpp")), None)
         self.assertIsNotNone(expected)
         self.assertEqual(expected.content, "#include <cstdint>\n")
 
-    @parameterized.expand([
-        AppSourceGenerator("foo"),
-        LibSourceGenerator("foo")
-    ])
-    def test_adds_example_files(self, builder):
-        files = builder.run()
+    def test_lib_adds_example_files(self):
+        files = LibSourceGenerator("foo").run()
 
         expected = next((f for f in files if f.path == Path("examples/main.cpp")), None)
         self.assertIsNotNone(expected)
         self.assertEqual(expected.content,
                          "#include <foo/foo.hpp>\n\nauto main() -> int {\n    return 0;\n}\n")
 
+    def test_app_doesnt_add_example_files(self):
+        files = AppSourceGenerator("foo").run()
+
+        expected = next((f for f in files if f.path == Path("examples/main.cpp")), None)
+        self.assertIsNone(expected)
+
     @parameterized.expand([
         AppSourceGenerator("foo"),
         LibSourceGenerator("foo")
     ])
     def test_adds_source_files(self, builder):
         files = builder.run()
 
@@ -51,14 +53,20 @@
 
     def test_lib_source_builder_does_not_add_main(self):
         files = LibSourceGenerator("foo").run()
 
         expected = next((f for f in files if f.path == Path("src/main.cpp")), None)
         self.assertIsNone(expected)
 
+    def test_app_source_builder_does_not_add_examples(self):
+        files = AppSourceGenerator("foo").run()
+
+        expected = next((f for f in files if f.path == Path("examples/main.cpp")), None)
+        self.assertIsNone(expected)
+
     def test_source_builder_factory_returns_an_app_builder(self):
         builder = make_source_generator(ProjectType.APP, "foo")
         self.assertIsInstance(builder, AppSourceGenerator)
 
     def test_source_builder_factory_returns_a_lib_builder(self):
         builder = make_source_generator(ProjectType.LIB, "foo")
         self.assertIsInstance(builder, LibSourceGenerator)
```

