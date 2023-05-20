# Comparing `tmp/pyllamacpp-2.2.0.tar.gz` & `tmp/pyllamacpp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.2.0.tar", last modified: Fri May 19 00:24:58 2023, max compression
+gzip compressed data, was "pyllamacpp-2.3.0.tar", last modified: Sat May 20 01:09:11 2023, max compression
```

## Comparing `pyllamacpp-2.2.0.tar` & `pyllamacpp-2.3.0.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/benchmark/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/quantize-stats/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/save-load-state/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/save-load-state/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/pocs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/pocs/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/pocs/vdot/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/pocs/vdot/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/scripts/build-info.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.377225 pyllamacpp-2.2.0/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43662 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/baby-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/baby-llama/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/benchmark/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/quantize-stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/examples/save-load-state/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/examples/save-load-state/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/pocs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/pocs/vdot/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/pocs/vdot/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/scripts/build-info.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-20 01:09:00.000000 pyllamacpp-2.3.0/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.224013 pyllamacpp-2.3.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.232014 pyllamacpp-2.3.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.228013 pyllamacpp-2.3.0/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:09:10.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 01:09:11.000000 pyllamacpp-2.3.0/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:09:11.236014 pyllamacpp-2.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43672 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-20 01:08:58.000000 pyllamacpp-2.3.0/src/main.h
```

### Comparing `pyllamacpp-2.2.0/CMakeLists.txt` & `pyllamacpp-2.3.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/LICENSE` & `pyllamacpp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/PKG-INFO` & `pyllamacpp-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
```

### Comparing `pyllamacpp-2.2.0/README.md` & `pyllamacpp-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.3.0/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.3.0/llama.cpp/examples/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,8 +32,9 @@
     add_subdirectory(main)
     add_subdirectory(quantize)
     add_subdirectory(quantize-stats)
     add_subdirectory(perplexity)
     add_subdirectory(embedding)
     add_subdirectory(save-load-state)
     add_subdirectory(benchmark)
+    add_subdirectory(baby-llama)
 endif()
```

### Comparing `pyllamacpp-2.2.0/llama.cpp/scripts/build-info.cmake` & `pyllamacpp-2.3.0/llama.cpp/scripts/build-info.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/llama.cpp/tests/CMakeLists.txt` & `pyllamacpp-2.3.0/llama.cpp/tests/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,7 +6,9 @@
 endfunction()
 
 # llama_add_test(test-double-float.c) # SLOW
 llama_add_test(test-quantize-fns.cpp)
 llama_add_test(test-quantize-perf.cpp)
 llama_add_test(test-sampling.cpp)
 llama_add_test(test-tokenizer-0.cpp ${CMAKE_CURRENT_SOURCE_DIR}/../models/ggml-vocab.bin)
+# llama_add_test(test-grad0.c) # SLOW
+# llama_add_test(test-opt.c) # SLOW
```

### Comparing `pyllamacpp-2.2.0/pybind11/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/LICENSE` & `pyllamacpp-2.3.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/options.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.3.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.3.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.3.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.3.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.3.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/check-style.sh` & `pyllamacpp-2.3.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.3.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/libsize.py` & `pyllamacpp-2.3.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/make_changelog.py` & `pyllamacpp-2.3.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.3.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.3.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.3.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.3.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.3.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.3.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pyllamacpp/_logger.py` & `pyllamacpp-2.3.0/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pyllamacpp/cli.py` & `pyllamacpp-2.3.0/pyllamacpp/cli.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pyllamacpp/model.py` & `pyllamacpp-2.3.0/pyllamacpp/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,29 +40,29 @@
                  model_path: str,
                  prompt_context: str = '',
                  prompt_prefix: str = '',
                  prompt_suffix: str = '',
                  log_level: int = logging.ERROR,
                  n_ctx: int = 512,
                  seed: int = 0,
-                 n_parts: int = -1,
+                 n_gpu_layers: int = 0,
                  f16_kv: bool = False,
                  logits_all: bool = False,
                  vocab_only: bool = False,
                  use_mlock: bool = False,
                  embedding: bool = False):
         """
         :param model_path: the path to the ggml model
         :param prompt_context: the global context of the interaction
         :param prompt_prefix: the prompt prefix
         :param prompt_suffix: the prompt suffix
         :param log_level: logging level, set to INFO by default
         :param n_ctx: LLaMA context
         :param seed: random seed
-        :param n_parts: LLaMA n_parts
+        :param n_gpu_layers: number of layers to store in VRAM
         :param f16_kv: use fp16 for KV cache
         :param logits_all: the llama_eval() call computes all logits, not just the last one
         :param vocab_only: only load the vocabulary, no weights
         :param use_mlock: force system to keep model in RAM
         :param embedding: embedding mode only
         """
 
@@ -73,15 +73,15 @@
         if not Path(model_path).is_file():
             raise Exception(f"File {model_path} not found!")
 
         self.llama_params = pp.llama_context_default_params()
         # update llama_params
         self.llama_params.n_ctx = n_ctx
         self.llama_params.seed = seed
-        self.llama_params.n_parts = n_parts
+        self.llama_params.n_gpu_layers = n_gpu_layers
         self.llama_params.f16_kv = f16_kv
         self.llama_params.logits_all = logits_all
         self.llama_params.vocab_only = vocab_only
         self.llama_params.use_mlock = use_mlock
         self.llama_params.embedding = embedding
 
         self._ctx = pp.llama_init_from_file(model_path, self.llama_params)
@@ -214,24 +214,38 @@
             self._last_n_tokens.append(tok)
 
         n_remain = 0
         if antiprompt is not None:
             sequence_queue = []
             stop_word = antiprompt.strip()
 
+        n_ctx = pp.llama_n_ctx(self._ctx)
+
         while infinite_generation or predicted_token != pp.llama_token_eos():
             if len(predicted_tokens) > 0:
-                if (pp.llama_eval(self._ctx,
-                                  predicted_tokens,
-                                  len(predicted_tokens),
-                                  self._n_past,
-                                  n_threads)):
-                    raise Exception("failed to eval the model!")
-                self._n_past += len(predicted_tokens)
-                predicted_tokens.clear()
+                # infinite text generation via context swapping
+                if (self._n_past + len(predicted_tokens)) > n_ctx:
+                    n_left = self._n_past - self.gpt_params.n_keep
+                    self._n_past = max(1, self.gpt_params.n_keep)
+                    predicted_tokens[:0] = self._last_n_tokens[n_ctx - n_left // 2 - len(predicted_tokens):len(self._last_n_tokens) - len(predicted_tokens)]
+
+                for i in range(0, len(predicted_tokens), self.gpt_params.n_batch):
+                    n_eval = len(predicted_tokens) - i
+                    if n_eval > self.gpt_params.n_batch:
+                        n_eval = self.gpt_params.n_batch
+
+                    if (pp.llama_eval(self._ctx,
+                                      predicted_tokens[i:],
+                                      n_eval,
+                                      self._n_past,
+                                      n_threads)):
+                        raise Exception("Model eval failed!")
+                self._n_past += n_eval
+
+            predicted_tokens.clear()
 
             # sampling
             predicted_token = pp.sample_next_token(self._ctx, self.gpt_params, self._last_n_tokens)
 
             predicted_tokens.append(predicted_token)
             # tokens come as raw undecoded bytes,
             # and we decode them, replacing those that can't be decoded.
```

### Comparing `pyllamacpp-2.2.0/pyllamacpp/utils.py` & `pyllamacpp-2.3.0/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pyllamacpp/webui.py` & `pyllamacpp-2.3.0/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.3.0/pyllamacpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
```

### Comparing `pyllamacpp-2.2.0/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.3.0/pyllamacpp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ./pyllamacpp/cli.py
 ./pyllamacpp/constants.py
 ./pyllamacpp/model.py
 ./pyllamacpp/utils.py
 ./pyllamacpp/webui.py
 llama.cpp/CMakeLists.txt
 llama.cpp/examples/CMakeLists.txt
+llama.cpp/examples/baby-llama/CMakeLists.txt
 llama.cpp/examples/benchmark/CMakeLists.txt
 llama.cpp/examples/embedding/CMakeLists.txt
 llama.cpp/examples/main/CMakeLists.txt
 llama.cpp/examples/perplexity/CMakeLists.txt
 llama.cpp/examples/quantize/CMakeLists.txt
 llama.cpp/examples/quantize-stats/CMakeLists.txt
 llama.cpp/examples/save-load-state/CMakeLists.txt
```

### Comparing `pyllamacpp-2.2.0/pyproject.toml` & `pyllamacpp-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/setup.py` & `pyllamacpp-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.2.0",
+    version="2.3.0",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.2.0/src/llama.cpp_LICENSE` & `pyllamacpp-2.3.0/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.2.0/src/main.cpp` & `pyllamacpp-2.3.0/src/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -912,15 +912,15 @@
 //            llama_token_data *tokens_ptr = static_cast<llama_token_data *>(buf.ptr);
 //            self.data = tokens_ptr;
         });
 
     py::class_<llama_context_params>(m,"llama_context_params")
         .def(py::init<>())
         .def_readwrite("n_ctx", &llama_context_params::n_ctx)
-        .def_readwrite("n_parts", &llama_context_params::n_parts)
+        .def_readwrite("n_gpu_layers", &llama_context_params::n_gpu_layers)
         .def_readwrite("seed", &llama_context_params::seed)
         .def_readwrite("f16_kv", &llama_context_params::f16_kv)
         .def_readwrite("logits_all", &llama_context_params::logits_all)
         .def_readwrite("vocab_only", &llama_context_params::vocab_only)
         .def_readwrite("use_mlock", &llama_context_params::use_mlock)
         .def_readwrite("embedding", &llama_context_params::embedding)
         .def_property("progress_callback", [](llama_context_params &self) {},
```

### Comparing `pyllamacpp-2.2.0/src/main.h` & `pyllamacpp-2.3.0/src/main.h`

 * *Files identical despite different names*

