# Comparing `tmp/lenskit-build-helpers-0.2.0.tar.gz` & `tmp/lenskit_build_helpers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenskit-build-helpers-0.2.0.tar", last modified: Mon Apr 10 20:52:02 2023, max compression
+gzip compressed data, was "lenskit_build_helpers-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lenskit-build-helpers-0.2.0.tar` & `lenskit_build_helpers-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      228 2022-07-16 00:06:38.137880 lenskit-build-helpers-0.2.0/.editorconfig
--rw-r--r--   0        0        0      121 2022-07-16 00:06:38.138887 lenskit-build-helpers-0.2.0/.gitignore
--rw-r--r--   0        0        0     2858 2022-12-07 00:26:56.364440 lenskit-build-helpers-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1083 2022-07-21 03:02:08.855947 lenskit-build-helpers-0.2.0/README.md
--rw-r--r--   0        0        0      255 2022-12-07 00:26:56.405575 lenskit-build-helpers-0.2.0/boot-env.yml
--rw-r--r--   0        0        0   156523 2022-12-07 00:29:13.161444 lenskit-build-helpers-0.2.0/conda-lock.yml
--rw-r--r--   0        0        0      363 2023-04-10 20:51:40.606368 lenskit-build-helpers-0.2.0/lkbuild/__init__.py
--rw-r--r--   0        0        0      125 2022-07-16 00:06:38.139756 lenskit-build-helpers-0.2.0/lkbuild/__main__.py
--rw-r--r--   0        0        0      165 2022-12-07 00:26:56.425263 lenskit-build-helpers-0.2.0/lkbuild/data/__init__.py
--rw-r--r--   0        0        0     8364 2022-12-07 00:26:56.426184 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/README.txt
--rw-r--r--   0        0        0   174246 2022-12-07 00:26:56.433179 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/links.csv
--rw-r--r--   0        0        0   449264 2022-12-07 00:26:56.439178 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/movies.csv
--rw-r--r--   0        0        0  2338261 2022-12-07 00:26:56.460260 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/ratings.csv
--rw-r--r--   0        0        0    40605 2022-12-07 00:26:56.465184 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/tags.csv
--rw-r--r--   0        0        0      958 2022-12-08 23:27:24.561754 lenskit-build-helpers-0.2.0/lkbuild/datasets.py
--rw-r--r--   0        0        0      541 2022-07-16 00:06:38.140253 lenskit-build-helpers-0.2.0/lkbuild/env.py
--rw-r--r--   0        0        0       82 2022-07-16 00:06:38.140612 lenskit-build-helpers-0.2.0/lkbuild/specs/mkl-spec.yml
--rw-r--r--   0        0        0       84 2022-07-16 00:06:38.144272 lenskit-build-helpers-0.2.0/lkbuild/specs/openblas-spec.yml
--rw-r--r--   0        0        0       77 2022-07-16 00:06:38.142000 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.10-spec.yml
--rw-r--r--   0        0        0       77 2023-04-06 20:53:12.695024 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.11-spec.yml
--rw-r--r--   0        0        0       75 2022-07-16 00:06:38.143743 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.7-spec.yml
--rw-r--r--   0        0        0       75 2022-07-16 00:06:38.144272 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.8-spec.yml
--rw-r--r--   0        0        0       75 2022-07-16 00:06:38.140612 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.9-spec.yml
--rw-r--r--   0        0        0     4028 2022-12-07 00:42:45.886534 lenskit-build-helpers-0.2.0/lkbuild/tasks.py
--rw-r--r--   0        0        0      224 2022-02-19 17:32:27.353316 lenskit-build-helpers-0.2.0/lock-for-ci.sh
--rw-r--r--   0        0        0      453 2022-07-21 03:02:08.918887 lenskit-build-helpers-0.2.0/meta.yaml
--rw-r--r--   0        0        0      705 2022-12-07 00:32:24.589580 lenskit-build-helpers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      567 2022-12-07 00:26:56.486378 lenskit-build-helpers-0.2.0/tasks.py
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 lenskit-build-helpers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2023-05-20 19:39:45.877730 lenskit_build_helpers-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      121 2023-05-20 19:39:45.877800 lenskit_build_helpers-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2858 2023-05-20 19:39:45.877930 lenskit_build_helpers-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1083 2023-05-20 19:39:45.878014 lenskit_build_helpers-0.3.0/README.md
+-rw-r--r--   0        0        0      255 2023-05-20 19:40:57.296296 lenskit_build_helpers-0.3.0/boot-env.yml
+-rw-r--r--   0        0        0   151486 2023-05-20 19:39:45.879881 lenskit_build_helpers-0.3.0/conda-lock.yml
+-rw-r--r--   0        0        0      363 2023-05-20 19:41:19.893823 lenskit_build_helpers-0.3.0/lkbuild/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-20 19:39:45.880086 lenskit_build_helpers-0.3.0/lkbuild/__main__.py
+-rw-r--r--   0        0        0      165 2023-05-20 19:39:45.880195 lenskit_build_helpers-0.3.0/lkbuild/data/__init__.py
+-rw-r--r--   0        0        0     8364 2023-05-20 19:39:45.880302 lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/README.txt
+-rw-r--r--   0        0        0   174246 2023-05-20 19:39:45.881210 lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/links.csv
+-rw-r--r--   0        0        0   449264 2023-05-20 19:39:45.883242 lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/movies.csv
+-rw-r--r--   0        0        0  2338261 2023-05-20 19:39:45.891734 lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/ratings.csv
+-rw-r--r--   0        0        0    40605 2023-05-20 19:39:45.892114 lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/tags.csv
+-rw-r--r--   0        0        0      958 2023-05-20 19:39:45.892215 lenskit_build_helpers-0.3.0/lkbuild/datasets.py
+-rw-r--r--   0        0        0      541 2023-05-20 19:39:45.892284 lenskit_build_helpers-0.3.0/lkbuild/env.py
+-rw-r--r--   0        0        0       82 2023-05-20 19:39:45.892383 lenskit_build_helpers-0.3.0/lkbuild/specs/mkl-spec.yml
+-rw-r--r--   0        0        0       84 2023-05-20 19:39:45.892443 lenskit_build_helpers-0.3.0/lkbuild/specs/openblas-spec.yml
+-rw-r--r--   0        0        0       77 2023-05-20 19:39:45.892500 lenskit_build_helpers-0.3.0/lkbuild/specs/python-3.10-spec.yml
+-rw-r--r--   0        0        0       77 2023-05-20 19:39:45.892555 lenskit_build_helpers-0.3.0/lkbuild/specs/python-3.11-spec.yml
+-rw-r--r--   0        0        0       75 2023-05-20 19:39:45.892623 lenskit_build_helpers-0.3.0/lkbuild/specs/python-3.7-spec.yml
+-rw-r--r--   0        0        0       75 2023-05-20 19:39:45.892687 lenskit_build_helpers-0.3.0/lkbuild/specs/python-3.8-spec.yml
+-rw-r--r--   0        0        0       75 2023-05-20 19:39:45.892742 lenskit_build_helpers-0.3.0/lkbuild/specs/python-3.9-spec.yml
+-rw-r--r--   0        0        0     4028 2023-05-20 19:39:45.892822 lenskit_build_helpers-0.3.0/lkbuild/tasks.py
+-rwxr-xr-x   0        0        0      224 2023-05-20 19:39:45.892890 lenskit_build_helpers-0.3.0/lock-for-ci.sh
+-rw-r--r--   0        0        0      444 2023-05-20 19:40:27.071801 lenskit_build_helpers-0.3.0/meta.yaml
+-rw-r--r--   0        0        0      705 2023-05-20 19:42:33.320198 lenskit_build_helpers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      567 2023-05-20 19:39:45.893073 lenskit_build_helpers-0.3.0/tasks.py
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 lenskit_build_helpers-0.3.0/PKG-INFO
```

### Comparing `lenskit-build-helpers-0.2.0/LICENSE.md` & `lenskit_build_helpers-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/README.md` & `lenskit_build_helpers-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/conda-lock.yml` & `lenskit_build_helpers-0.3.0/conda-lock.yml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,5037 +1,5037 @@
-# This lock file was generated by conda-lock (https://github.com/conda-incubator/conda-lock). DO NOT EDIT!
-#
-# A "lock file" contains a concrete list of package versions (with checksums) to be installed. Unlike
-# e.g. `conda env create`, the resulting environment will not change as new package versions become
-# available, unless you explicitly update the lock file.
-#
-# Install this environment as "YOURENV" with:
-#     conda-lock install -n YOURENV --file conda-lock.yml
-# To update a single package to the latest version compatible with the version constraints in the source:
-#     conda-lock lock --lockfile conda-lock.yml --update PACKAGE
-# To re-solve the entire environment, e.g. after changing a version constraint in the source file:
-#     conda-lock -f pyproject.toml -f C:\Users\michael\Documents\LensKit\lkbuild\pyproject.toml --lockfile conda-lock.yml
-metadata:
-  channels:
-  - url: conda-forge
-    used_env_vars: []
-  content_hash:
-    linux-64: 66b8d24fe36a198717ddca7d1fc328fc453a37f8878c80fb73db22b4baa3f8bc
-    osx-64: f5833e90d66407c42f4f0830ed8287aca17995fb4ca49e1fa2825e96ddf2692a
-    win-64: def7cf82c8e903a65f0ad53079339ea52c054c43f2164fabfa828188aa5e623a
-  platforms:
-  - linux-64
-  - osx-64
-  - win-64
-  sources:
-  - pyproject.toml
-  - C:\Users\michael\Documents\LensKit\lkbuild\pyproject.toml
-package:
-- category: main
-  dependencies: {}
-  hash:
-    md5: d7c89558ba9fa0495403155b64376d81
-    sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
-  manager: conda
-  name: _libgcc_mutex
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
-  version: '0.1'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 41e4e87062433e283696cf384f952ef6
-    sha256: 058355034667e77d15389700f6b2364cc74efce0af63a418eacc1ce252458942
-  manager: conda
-  name: ca-certificates
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.9.24-ha878542_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies: {}
-  hash:
-    md5: 737be0d34c22d24432049ab7a3214de4
-    sha256: 3e7f203e33ea497b6e468279cc5fdef7d556473c25e7466b35fd672940392469
-  manager: conda
-  name: ld_impl_linux-64
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.39-hcc3a1bd_1.conda
-  version: '2.39'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 1030b1f38c129f2634eae026f704fe60
-    sha256: 0289e6a7b9a5249161a3967909e12dcfb4ab4475cdede984635d3fb65c606f08
-  manager: conda
-  name: libstdcxx-ng
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2
-  version: 12.2.0
-- category: main
-  dependencies: {}
-  hash:
-    md5: 878f923dd6acc8aeb47a75da6c4098be
-    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
-  manager: conda
-  name: pybind11-abi
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
-  version: '4'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 4eb33d14d794b0f4be116443ffed3853
-    sha256: bcb15db27eb6fbc0fe15d23aa60dcfa58ef451d92771441068d4a911aea7bb9f
-  manager: conda
-  name: python_abi
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-3_cp310.conda
-  version: '3.10'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
-    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
-  manager: conda
-  name: tzdata
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
-  version: 2022g
-- category: main
-  dependencies:
-    _libgcc_mutex: 0.1 conda_forge
-  hash:
-    md5: cedcee7c064c01c403f962c9e8d3c373
-    sha256: 81a76d20cfdee9fe0728b93ef057ba93494fd1450d42bc3717af4e468235661e
-  manager: conda
-  name: libgomp
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2
-  version: 12.2.0
-- category: main
-  dependencies:
-    _libgcc_mutex: 0.1 conda_forge
-    libgomp: '>=7.5.0'
-  hash:
-    md5: 73aaf86a425cc6e73fcf236a5a46396d
-    sha256: fbe2c5e56a653bebb982eda4876a9178aedfc2b545f25d0ce9c4c0b508253d22
-  manager: conda
-  name: _openmp_mutex
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
-  version: '4.5'
-- category: main
-  dependencies:
-    _libgcc_mutex: 0.1 conda_forge
-    _openmp_mutex: '>=4.5'
-  hash:
-    md5: e4c94f80aef025c17ab0828cd85ef535
-    sha256: f3899c26824cee023f1e360bd0859b0e149e2b3e8b1668bc6dd04bfc70dcd659
-  manager: conda
-  name: libgcc-ng
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2
-  version: 12.2.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.3.0'
-  hash:
-    md5: a1fd65c7ccbf10880423d82bca54eb54
-    sha256: cb521319804640ff2ad6a9f118d972ed76d86bea44e5626c09a13d38f562e1fa
-  manager: conda
-  name: bzip2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-  hash:
-    md5: f26ef8098fab1f719c91eb760d63381a
-    sha256: ee735e60d2cf68e5635df17847e97b505a752985d10581d2438203e7c0f44c15
-  manager: conda
-  name: c-ares
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2
-  version: 1.18.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-  hash:
-    md5: c4fbad8d4bddeb3c085f18cbf97fbfad
-    sha256: b44db0b92ae926b3fbbcd57c179fceb64fa11a9f9d09082e03be58b74dcad832
-  manager: conda
-  name: expat
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-h27087fc_0.tar.bz2
-  version: 2.5.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-  hash:
-    md5: b57864c85261a0fbc7132d2cc17478c7
-    sha256: bd48506faffa86e07f7b40d54f2d7e13b0fc956eda9760236750f5ea20db7129
-  manager: conda
-  name: fmt
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/fmt-9.1.0-h924138e_0.tar.bz2
-  version: 9.1.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-  hash:
-    md5: 14947d8770185e5153fdd04d4673ed37
-    sha256: 4fcfedc44e4c9a053f0416f9fc6ab6ed50644fca3a761126dbd00d09db1f546a
-  manager: conda
-  name: gettext
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2
-  version: 0.21.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=10.3.0'
-    libstdcxx-ng: '>=10.3.0'
-  hash:
-    md5: 87473a15119779e021c314249d4b4aed
-    sha256: 1d7950f3be4637ab915d886304e57731d39a41ab705ffc95c4681655c459374a
-  manager: conda
-  name: icu
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/icu-70.1-h27087fc_0.tar.bz2
-  version: '70.1'
-- category: main
-  dependencies:
-    libgcc-ng: '>=10.3.0'
-  hash:
-    md5: 30186d27e2c9fa62b45fb1476b7200e3
-    sha256: 150c05a6e538610ca7c43beb3a40d65c90537497a4f6a5f4d15ec0451b6f5ebb
-  manager: conda
-  name: keyutils
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
-  version: 1.6.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=7.5.0'
-  hash:
-    md5: 6f8720dff19e17ce5d48cfe7f3d2f0a3
-    sha256: 8c9635aa0ea28922877dc96358f9547f6a55fc7e2eb75a556b05f1725496baf9
-  manager: conda
-  name: libev
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2
-  version: '4.33'
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-  hash:
-    md5: d645c6d2ac96843a2bfaccd2d62b3ac3
-    sha256: ab6e9856c21709b7b517e940ae7028ae0737546122f83c2aa5d692860c3b149e
-  manager: conda
-  name: libffi
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
-  version: 3.4.2
-- category: main
-  dependencies:
-    libgcc-ng: '>=10.3.0'
-  hash:
-    md5: b62b52da46c39ee2bc3c162ac7f1804d
-    sha256: 6a81ebac9f1aacdf2b4f945c87ad62b972f0f69c8e0981d68e111739e6720fd7
-  manager: conda
-  name: libiconv
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2
-  version: '1.17'
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-  hash:
-    md5: 39b1328babf85c7c3a61636d9cd50206
-    sha256: 32f4fb94d99946b0dabfbbfd442b25852baf909637f2eed1ffe3baea15d02aad
-  manager: conda
-  name: libnsl
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2
-  version: 2.0.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.3.0'
-  hash:
-    md5: 772d69f030955d9646d3d0eaf21d859d
-    sha256: 54f118845498353c936826f8da79b5377d23032bcac8c4a02de2019e26c3f6b3
-  manager: conda
-  name: libuuid
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2
-  version: 2.32.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-  hash:
-    md5: f3f9de449d32ca9b9c66a22863c96f41
-    sha256: 22f3663bcf294d349327e60e464a51cd59664a71b8ed70c28a9f512d10bc77dd
-  manager: conda
-  name: libzlib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2
-  version: 1.2.13
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.3.0'
-    libstdcxx-ng: '>=9.3.0'
-  hash:
-    md5: fbe97e8fa6f275d7c76a09e795adc3e6
-    sha256: 56313fe4e602319682d4ea05c0ed3c5c45fc79884a5896f2cb7436b15d6987f9
-  manager: conda
-  name: lz4-c
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.3-h9c3ff4c_1.tar.bz2
-  version: 1.9.3
-- category: main
-  dependencies:
-    libgcc-ng: '>=7.5.0'
-  hash:
-    md5: bb14fcb13341b81d5eb386423b9d2bac
-    sha256: 25d16e6aaa3d0b450e61d0c4fadd7c9fd17f16e2fef09b34507209342d63c9f6
-  manager: conda
-  name: lzo
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/lzo-2.10-h516909a_1000.tar.bz2
-  version: '2.10'
-- category: main
-  dependencies:
-    libgcc-ng: '>=10.3.0'
-  hash:
-    md5: 4acfc691e64342b9dae57cf2adc63238
-    sha256: b801e8cf4b2c9a30bce5616746c6c2a4e36427f045b46d9fc08a4ed40a9f7065
-  manager: conda
-  name: ncurses
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2
-  version: '6.3'
-- category: main
-  dependencies:
-    ca-certificates: ''
-    libgcc-ng: '>=12'
-  hash:
-    md5: 7adaac6ff98219bcb99b45e408b80f4e
-    sha256: d9143f6d10e7edaa8cbb03e510d60c54463f4538c01f30b0abff51def582d94e
-  manager: conda
-  name: openssl
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.0.7-h0b41bf4_1.conda
-  version: 3.0.7
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.3.0'
-    libstdcxx-ng: '>=9.3.0'
-  hash:
-    md5: c05d1820a6d34ff07aaaab7a9b7eddaa
-    sha256: 8f35c244b1631a4f31fb1d66ab6e1d9bfac0ca9b679deced1112c7225b3ad138
-  manager: conda
-  name: pcre
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/pcre-8.45-h9c3ff4c_0.tar.bz2
-  version: '8.45'
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-  hash:
-    md5: 1e16d4142b016b6a5ebdeb3d6d33aaf4
-    sha256: f46a85d6df26dce9ec2c63c90662dd02bdc446cece65afd37b1ee9e31525a206
-  manager: conda
-  name: reproc
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/reproc-14.2.3-h7f98852_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-  hash:
-    md5: 2161070d867d1b1204ea749c8eec4ef0
-    sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
-  manager: conda
-  name: xz
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
-  version: 5.2.6
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-  hash:
-    md5: 4cb3ad778ec2d5a7acbdf254eb1c42ae
-    sha256: a4e34c710eeb26945bdbdaba82d3d74f60a78f54a874ec10d373811a5d217535
-  manager: conda
-  name: yaml
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
-  version: 0.2.5
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-  hash:
-    md5: 0449d47d8457feaa3720d4779616dde2
-    sha256: fcdffce895f84a49221720b811a6bb14ae79f7ac14f7930f3768bbb7b2470444
-  manager: conda
-  name: yaml-cpp
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/yaml-cpp-0.7.0-h27087fc_2.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=7.5.0'
-    ncurses: '>=6.2,<7.0.0a0'
-  hash:
-    md5: 4d331e44109e3f0e19b4cb8f9b82f3e1
-    sha256: a57d37c236d8f7c886e01656f4949d9dcca131d2a0728609c6f7fa338b65f1cf
-  manager: conda
-  name: libedit
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2
-  version: 3.1.20191231
-- category: main
-  dependencies:
-    c-ares: '>=1.18.1,<2.0a0'
-    libev: '>=4.33,<4.34.0a0'
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    openssl: '>=3.0.5,<4.0a0'
-  hash:
-    md5: 2b7dbfa6988a41f9d23ba6d4f0e1d74e
-    sha256: 66988eb178d6ffbad3de5e391dad49aaa298e1309ac197ab40996eac740fbfff
-  manager: conda
-  name: libnghttp2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.47.0-hff17c54_1.tar.bz2
-  version: 1.47.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=10.3.0'
-    libstdcxx-ng: '>=10.3.0'
-    libzlib: '>=1.2.11,<1.3.0a0'
-  hash:
-    md5: 461963bb499e58bae159a898600f8792
-    sha256: 2c03438609126505d7167eb8f9eec84a6de5e5f098495de052550cb371b18407
-  manager: conda
-  name: libsolv
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libsolv-0.7.22-h6239696_0.tar.bz2
-  version: 0.7.22
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libzlib: '>=1.2.13,<1.3.0a0'
-  hash:
-    md5: 2e5f9a37d487e1019fd4d8113adb2f9f
-    sha256: 6008a0b914bd1a3510a3dba38eada93aa0349ebca3a21e5fa276833c8205bf49
-  manager: conda
-  name: libsqlite
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.40.0-h753d276_0.tar.bz2
-  version: 3.40.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    openssl: '>=3.0.5,<4.0a0'
-  hash:
-    md5: d85acad4b47dff4e3def14a769a97906
-    sha256: 9a9a01f35d2d50326eb8ca7c0a92d0c45b2d0f77d9ea117680c70094ff480c0c
-  manager: conda
-  name: libssh2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-hf14f497_3.tar.bz2
-  version: 1.10.0
-- category: main
-  dependencies:
-    icu: '>=70.1,<71.0a0'
-    libgcc-ng: '>=12'
-    libiconv: '>=1.17,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    xz: '>=5.2.6,<6.0a0'
-  hash:
-    md5: 3b933ea47ef8f330c4c068af25fcd6a8
-    sha256: b30713fb4477ff4f722280d956593e7e7a2cb705b7444dcc278de447432b43b1
-  manager: conda
-  name: libxml2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.10.3-h7463322_0.tar.bz2
-  version: 2.10.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libgcc-ng: '>=12'
-    libzlib: '>=1.2.12,<1.3.0a0'
-  hash:
-    md5: 69e2c796349cd9b273890bee0febfe1b
-    sha256: 7a29ec847556eed4faa1646010baae371ced69059a4ade43851367a076d6108a
-  manager: conda
-  name: pcre2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2
-  version: '10.40'
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    ncurses: '>=6.3,<7.0a0'
-  hash:
-    md5: db2ebbe2943aae81ed051a6a9af8e0fa
-    sha256: f5f383193bdbe01c41cb0d6f99fec68e820875e842e6e8b392dbe1a9b6c43ed8
-  manager: conda
-  name: readline
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2
-  version: 8.1.2
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-    libstdcxx-ng: '>=9.4.0'
-    reproc: 14.2.3 h7f98852_0
-  hash:
-    md5: 1fc15d3b393b62192d3eeade92b61610
-    sha256: 03d7dcc19ac0a16f32b77368c22e24cf370d2ea5681e28c5687d9e4bd25ab2db
-  manager: conda
-  name: reproc-cpp
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/reproc-cpp-14.2.3-h9c3ff4c_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies:
-    libgcc-ng: '>=9.4.0'
-    libzlib: '>=1.2.11,<1.3.0a0'
-  hash:
-    md5: 5b8c42eb62e9fc961af70bdd6a26e168
-    sha256: 032fd769aad9d4cad40ba261ab222675acb7ec951a8832455fce18ef33fa8df0
-  manager: conda
-  name: tk
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2
-  version: 8.6.12
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libzlib: 1.2.12 h166bdaf_2
-  hash:
-    md5: 4533821485cde83ab12ff3d8bda83768
-    sha256: 084342e7f0d2feeca6eb0f194f0a82ac75217730745e6c9033016ed015283bcc
-  manager: conda
-  name: zlib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/zlib-1.2.12-h166bdaf_2.tar.bz2
-  version: 1.2.12
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-    libzlib: '>=1.2.12,<1.3.0a0'
-  hash:
-    md5: adcf0be7897e73e312bd24353b613f74
-    sha256: c42d9ec413edd7e984b6cac676997105d0f106556a0f045961153b049b95b87c
-  manager: conda
-  name: zstd
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h6239696_4.tar.bz2
-  version: 1.5.2
-- category: main
-  dependencies:
-    keyutils: '>=1.6.1,<2.0a0'
-    libedit: '>=3.1.20191231,<4.0a0'
-    libgcc-ng: '>=10.3.0'
-    libstdcxx-ng: '>=10.3.0'
-    openssl: '>=3.0.0,<4.0a0'
-  hash:
-    md5: d25e05e7ee0e302b52d24491db4891eb
-    sha256: 9faad78e078a3e671f3572a01163acc1b2a47539559c746ea3ffd17c754ea578
-  manager: conda
-  name: krb5
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.3-h08a2579_0.tar.bz2
-  version: 1.19.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libgcc-ng: '>=12'
-    libxml2: '>=2.9.14,<2.11.0a0'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    lz4-c: '>=1.9.3,<1.10.0a0'
-    lzo: '>=2.10,<3.0a0'
-    openssl: '>=3.0.3,<4.0a0'
-    xz: '>=5.2.5,<5.3.0a0'
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: c0c3973a9f2df3e1a408e3205d86a88d
-    sha256: b67ff7262422ef04bfa1056c5ef10eba4d64773f40bb34314e0d492f58e726e7
-  manager: conda
-  name: libarchive
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarchive-3.5.2-hada088e_3.tar.bz2
-  version: 3.5.2
-- category: main
-  dependencies:
-    gettext: '>=0.21.1,<1.0a0'
-    libffi: '>=3.4,<4.0a0'
-    libgcc-ng: '>=12'
-    libiconv: '>=1.17,<2.0a0'
-    libstdcxx-ng: '>=12'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    pcre2: '>=10.40,<10.41.0a0'
-  hash:
-    md5: ed5349aa96776e00b34eccecf4a948fe
-    sha256: 3cbad3d63cff2dd9ac1dc9cce54fd3d657f3aff53df41bfe5bae9d760562a5af
-  manager: conda
-  name: libglib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.74.1-h606061b_1.tar.bz2
-  version: 2.74.1
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    ld_impl_linux-64: '>=2.36.1'
-    libffi: '>=3.4,<4.0a0'
-    libgcc-ng: '>=12'
-    libnsl: '>=2.0.0,<2.1.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
-    libuuid: '>=2.32.1,<3.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-    readline: '>=8.1.2,<9.0a0'
-    tk: '>=8.6.12,<8.7.0a0'
-    tzdata: ''
-    xz: '>=5.2.6,<6.0a0'
-  hash:
-    md5: be2a6d78752c2ab85f360ce37d2c64e2
-    sha256: 79cc250d8f85da29c7a06116a51db4c9efbd46f62f21daef6cf10e8bccdc0523
-  manager: conda
-  name: python
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.8-h4a9ceb5_0_cpython.conda
-  version: 3.10.8
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    readline: '>=8.1.2,<9.0a0'
-    zlib: '>=1.2.12,<1.3.0a0'
-  hash:
-    md5: 2cf5cb4cd116a78e639977eb61ad9987
-    sha256: 5878c9d99a731991eea6e9dea4baf09248a3caf4fa032acb41f2283965719138
-  manager: conda
-  name: sqlite
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/sqlite-3.39.2-h4ff8645_0.tar.bz2
-  version: 3.39.2
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 5f095bc6454094e96f146491fd03633b
-    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
-  manager: conda
-  name: appdirs
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
-  version: 1.4.4
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 5dfee17f24e2dfd18d7392b48c9351e2
-    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
-  manager: conda
-  name: cachy
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
-  version: 0.3.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: f66309b099374af91369e67e84af397d
-    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
-  manager: conda
-  name: certifi
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: c1d5b294fbf9a795dec349a6f4d8be8e
-    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
-  manager: conda
-  name: charset-normalizer
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    __unix: ''
-    python: '>=3.8'
-  hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
-  manager: conda
-  name: click
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: c267da48ce208905d7d976d49dfd9433
-    sha256: fcab1a16af5daf3a1ea9b0a7ed15615f0d5fff05ff4925ed570988868bb29e38
-  manager: conda
-  name: colorama
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2
-  version: 0.4.5
-- category: main
-  dependencies:
-    python: '>=3.6,<4.0'
-  hash:
-    md5: b8477552274c1cfdb533e954c76523f1
-    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
-  manager: conda
-  name: crashtest
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.1
-- category: main
-  dependencies:
-    expat: '>=2.4.2,<3.0a0'
-    libgcc-ng: '>=9.4.0'
-    libglib: '>=2.70.2,<3.0a0'
-  hash:
-    md5: ecfff944ba3960ecb334b9a2663d708d
-    sha256: 8f5f995699a2d9dbdd62c61385bfeeb57c82a681a7c8c5313c395aa0ccab68a5
-  manager: conda
-  name: dbus
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2
-  version: 1.13.6
-- category: main
-  dependencies:
-    python: 2.7|>=3.6
-  hash:
-    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
-    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
-  manager: conda
-  name: distlib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.6
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 21b8fa2179290505e607f5ccd65b01b0
-    sha256: f3a564449daedafe5931ab4efe7bc4f240182f2b760e7877f15b2898b7f1c988
-  manager: conda
-  name: docutils
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py310hff52083_1.tar.bz2
-  version: '0.19'
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
-    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
-  manager: conda
-  name: filelock
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
-  version: 3.8.2
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 6d5e56de2e65da7aa35fd10131226efa
-    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
-  manager: conda
-  name: flit-core
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 34272b248891bddccc64479f9a7fffed
-    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
-  manager: conda
-  name: idna
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
-  version: '3.4'
-- category: main
-  dependencies:
-    python: 2.7|>=3.4
-  hash:
-    md5: 25045ddd7fe83ddf71c181d6212e9913
-    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
-  manager: conda
-  name: invoke
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.7.3
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 9800ad1699b42612478755a2d26c722d
-    sha256: 16639759b811866d63315fe1391f6fb45f5478b823972f4d3d9f0392b7dd80b8
-  manager: conda
-  name: jeepney
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 0.8.0
-- category: main
-  dependencies:
-    krb5: '>=1.19.3,<1.20.0a0'
-    libgcc-ng: '>=12'
-    libnghttp2: '>=1.47.0,<2.0a0'
-    libssh2: '>=1.10.0,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-  hash:
-    md5: fdca8cd67ec2676f90a70ac73a32538b
-    sha256: 485249c8cf7c2bd67d8308f7d1fccbe64e54334ad6cc73168d665eed824ca3bc
-  manager: conda
-  name: libcurl
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.86.0-h2283fc2_1.tar.bz2
-  version: 7.86.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: c104d98e09c47519950cffb8dd5b4f10
-    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
-  manager: conda
-  name: lockfile
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
-  version: 0.12.2
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 2d7028ea2a77f909931e1a173d952261
-    sha256: 05a217ff2eea3fb0bada54f4c7c8efe5eb35e1ad7d142d662b364c686ff80da6
-  manager: conda
-  name: markupsafe
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py310h5764c6d_2.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 9b6ad26944f19f599800b068e0582227
-    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
-  manager: conda
-  name: more-itertools
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 9.0.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    libstdcxx-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 1fa34c9e9be72b7e4c3c9b95017463a3
-    sha256: 7878b37c7a97c14d01745f72b33921fbdb46617932bed8c791803129f9fae8a9
-  manager: conda
-  name: msgpack-python
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.4-py310hbf28c38_1.tar.bz2
-  version: 1.0.4
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: a4eea5bff523f26442405bc5d1f52adb
-    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
-  manager: conda
-  name: pastel
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.2.1
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
-    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
-  manager: conda
-  name: pkginfo
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
-  version: 1.9.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2fb3f88922e7aec26ba652fcdfe13950
-    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
-  manager: conda
-  name: platformdirs
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
-  version: 2.5.2
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 4c75b7766a1a1dd09d504c63cb5276e2
-    sha256: c8953a9542a1df749037721722ae25316d416812f74728d85a7bd07e9a94268b
-  manager: conda
-  name: poetry-core
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/poetry-core-1.0.8-py310hff52083_1.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 359eeb6536da0e687af562ed265ec263
-    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
-  manager: conda
-  name: ptyprocess
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 0e565d732f6660374b45d76761c09b06
-    sha256: 9bf587a2a0f0f73b71740b079507ec99282b73c596ec73cc602d7ccf73350709
-  manager: conda
-  name: pycosat
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pycosat-0.6.4-py310h5764c6d_1.tar.bz2
-  version: 0.6.4
-- category: main
-  dependencies:
-    python: 2.7.*|>=3.4
-  hash:
-    md5: 076becd9e05608f8dc72757d5f3a91ff
-    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
-  manager: conda
-  name: pycparser
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
-  version: '2.21'
-- category: main
-  dependencies:
-    python: '>=3.3'
-  hash:
-    md5: edf8651c4379d9d1495ad6229622d150
-    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
-  manager: conda
-  name: pylev
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: e8fbc1b54b25f4b08281467bc13b70cc
-    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
-  manager: conda
-  name: pyparsing
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
-  version: 3.0.9
-- category: main
-  dependencies:
-    __unix: ''
-    python: '>=3.8'
-  hash:
-    md5: 2a7de29fb590ca14b5243c4c812c8025
-    sha256: a42f826e958a8d22e65b3394f437af7332610e43ee313393d1cf143f0a2d274b
-  manager: conda
-  name: pysocks
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
-  version: 1.7.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: 9e68d2ff6d98737c855b65f48dd3c597
-    sha256: 602d68ee4544274b12fb6d13b8d5fc61d0ebbee190292c21d8be10a4e68185bd
-  manager: conda
-  name: pyyaml
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2
-  version: '6.0'
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 2dabb2fa2603a52d072ea6a50c539205
-    sha256: 6de36a7b9d56dda401ef3545f979a23d2225a150519bcc44bd39b2b995bbe3d0
-  manager: conda
-  name: ruamel.yaml.clib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h5764c6d_0.tar.bz2
-  version: 0.2.7
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: f588192bd22fb64650ccb5781cd83fb0
-    sha256: 4a17acbb2fae7b567b9f7527eb50833c266df00de7fee41f18bb2006dfab8939
-  manager: conda
-  name: ruamel_yaml
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel_yaml-0.15.80-py310h5764c6d_1008.tar.bz2
-  version: 0.15.80
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
-    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
-  manager: conda
-  name: setuptools
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
-  version: 65.5.1
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 437655338696f9d0dfdb0a024e66b255
-    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
-  manager: conda
-  name: shellingham
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: e5f25f8dbc060e9a8d912e432202afc2
-    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
-  manager: conda
-  name: six
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
-  version: 1.16.0
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: f832c45a477c78bebd107098db465095
-    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
-  manager: conda
-  name: toml
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
-  version: 0.10.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 5844808ffab9ebdb694585b50ba02a96
-    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
-  manager: conda
-  name: tomli
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.0.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 73506d1ab4202481841c68c169b7ef6c
-    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
-  manager: conda
-  name: tomli-w
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.0.0
-- category: main
-  dependencies:
-    python: '>=3.5'
-  hash:
-    md5: 92facfec94bc02d6ccf42e7173831a36
-    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
-  manager: conda
-  name: toolz
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
-  version: 0.12.0
-- category: main
-  dependencies:
-    python: '>=3'
-  hash:
-    md5: e6573ac68718f17b9d4f5c8eda3190f2
-    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
-  manager: conda
-  name: typing
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.10.0.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2d93b130d148d7fc77e583677792fc6a
-    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
-  manager: conda
-  name: typing_extensions
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 3563be4c5611a44210d9ba0c16113136
-    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
-  manager: conda
-  name: webencodings
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
-  version: 0.5.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: c829cfb8cb826acb9de0ac1a2df0a940
-    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
-  manager: conda
-  name: wheel
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
-  version: 0.38.4
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 09b5b885341697137879a4f039a9e5a1
-    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
-  manager: conda
-  name: zipp
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
-  version: 3.11.0
-- category: main
-  dependencies:
-    libffi: '>=3.4,<4.0a0'
-    libgcc-ng: '>=12'
-    pycparser: ''
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 6bb8063dd08f9724c18744b0e040cfe2
-    sha256: 97c8d32460e294486e44c9b92e8bb2bf5680bd58c10f5f5a172e47017309d442
-  manager: conda
-  name: cffi
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_2.tar.bz2
-  version: 1.15.1
-- category: main
-  dependencies:
-    click: ''
-    python: '>=3.6'
-  hash:
-    md5: 72a46ffc25701c173932fd55cf0965d3
-    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
-  manager: conda
-  name: click-default-group
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.2
-- category: main
-  dependencies:
-    crashtest: '>=0.3.0,<0.4.0'
-    pastel: '>=0.2.0,<0.3.0'
-    pylev: '>=1.3,<2.0'
-    python: ''
-  hash:
-    md5: 159273f717a11e53b2656f8b6521a5e2
-    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
-  manager: conda
-  name: clikit
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
-  version: 0.6.2
-- category: main
-  dependencies:
-    python: ''
-    six: '>=1.9'
-    webencodings: ''
-  hash:
-    md5: b2355343d6315c892543200231d7154a
-    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
-  manager: conda
-  name: html5lib
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
-  version: '1.1'
-- category: main
-  dependencies:
-    python: '>=3.8'
-    zipp: '>=0.5'
-  hash:
-    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
-    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
-  manager: conda
-  name: importlib-metadata
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    more-itertools: ''
-    python: '>=3.7'
-  hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
-  manager: conda
-  name: jaraco.classes
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
-  version: 3.2.3
-- category: main
-  dependencies:
-    markupsafe: '>=2.0'
-    python: '>=3.7'
-  hash:
-    md5: c8490ed5c70966d232fdd389d0dbed37
-    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
-  manager: conda
-  name: jinja2
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
-  version: 3.1.2
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libarchive: '>=3.5.2,<3.6.0a0'
-    libcurl: '>=7.86.0,<8.0a0'
-    libgcc-ng: '>=12'
-    libiconv: '>=1.17,<2.0a0'
-    libsolv: '>=0.7.22,<0.8.0a0'
-    libstdcxx-ng: '>=12'
-    openssl: '>=3.0.7,<4.0a0'
-    reproc-cpp: '>=14.2,<15.0a0'
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: 9d38a1b35b7de29dfc4d64daeb1e27fc
-    sha256: 0422a1e4a5f0e12230d2108c42242f49bbcb4f5da296bb6054000f3d051b5231
-  manager: conda
-  name: libmamba
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.1.0-h70b1f8a_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    pyparsing: '>=2.0.2,!=3.0.5'
-    python: '>=3.6'
-  hash:
-    md5: 71f1ab2de48613876becddd496371c85
-    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
-  manager: conda
-  name: packaging
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
-  version: '21.3'
-- category: main
-  dependencies:
-    ptyprocess: '>=0.5'
-    python: ''
-  hash:
-    md5: 5909e7b978141dd80d28dbf9de627827
-    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
-  manager: conda
-  name: pexpect
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
-  version: 4.8.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    setuptools: ''
-    wheel: ''
-  hash:
-    md5: da66f2851b9836d3a7c5190082a45f7d
-    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
-  manager: conda
-  name: pip
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 22.3.1
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ruamel.yaml.clib: '>=0.1.2'
-    setuptools: ''
-  hash:
-    md5: 93643151fba5c31c676effdd7661f075
-    sha256: d78bd1f789a1a79be1f76a8025476e1fcf72fe9becdaf23ec9e1c4bbc67eebf8
-  manager: conda
-  name: ruamel.yaml
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.21-py310h5764c6d_2.tar.bz2
-  version: 0.17.21
-- category: main
-  dependencies:
-    python: '>=3.6'
-    typing: '>=3.6,<4.0'
-  hash:
-    md5: 471bf9e605820b59988e830382b8d654
-    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
-  manager: conda
-  name: tomlkit
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
-  version: 0.11.6
-- category: main
-  dependencies:
-    colorama: ''
-    python: '>=2.7'
-  hash:
-    md5: 6642233f341e1900d0c8e6eddb979c14
-    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
-  manager: conda
-  name: tqdm
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
-  version: 4.64.0
-- category: main
-  dependencies:
-    typing_extensions: 4.4.0 pyha770c72_0
-  hash:
-    md5: be969210b61b897775a0de63cd9e9026
-    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
-  manager: conda
-  name: typing-extensions
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    distlib: '>=0.3.6,<1'
-    filelock: '>=3.4.1,<4'
-    platformdirs: '>=2.4,<3'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: c6fc5e3f0a463ddb59cfda9a1582cfa0
-    sha256: b43ae0b1fe2c77c05b39de70c28a419078d67731d12a52aa3b3440a12398446c
-  manager: conda
-  name: virtualenv
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.17.0-py310hff52083_0.conda
-  version: 20.17.0
-- category: main
-  dependencies:
-    cffi: '>=1.0.0'
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 87669c3468dff637bbd0363bc0f895cf
-    sha256: a37f9a00170f48e71b67bb4547e8bf352dcee4e4a79a55f087b512022cc64a0d
-  manager: conda
-  name: brotlipy
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1005.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    clikit: '>=0.6.0,<0.7.0'
-    python: '>=3.6'
-  hash:
-    md5: 4c82b11a3d06031bd58e7d869f53d965
-    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
-  manager: conda
-  name: cleo
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
-  version: 0.8.1
-- category: main
-  dependencies:
-    cffi: '>=1.12'
-    libgcc-ng: '>=12'
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: f999dcc21fe27ad97a8afcfa590daa14
-    sha256: 64a31aa5153e977e58256b098044b61ef903885b5b8f7ed807d066d1ceed2244
-  manager: conda
-  name: cryptography
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.4-py310h600f1e7_0.conda
-  version: 38.0.4
-- category: main
-  dependencies:
-    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
-  hash:
-    md5: 3dc2248927de739b4d2e2da9a9972bfe
-    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
-  manager: conda
-  name: importlib_metadata
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libgcc-ng: '>=12'
-    libmamba: 1.1.0 h70b1f8a_2
-    libstdcxx-ng: '>=12'
-    openssl: '>=3.0.7,<4.0a0'
-    pybind11-abi: '4'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: 1bc930a417259d6a0668931cdd9aa805
-    sha256: 7d8b967de764a98526c08e9aa718d650f6e7d5a5ba57181f6b4d6c1af5f0d5b0
-  manager: conda
-  name: libmambapy
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.1.0-py310h69aa5bf_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    typing-extensions: '>=4.1.0'
-  hash:
-    md5: d666328dd06e3be9c1e541c5f499f895
-    sha256: c4a0c7ae066f43ef764f95578e16fad41b5cf577cf3777e5a657ff08334d9b97
-  manager: conda
-  name: pydantic
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.2-py310h5764c6d_1.tar.bz2
-  version: 1.10.2
-- category: main
-  dependencies:
-    cffi: '>=1.11'
-    libgcc-ng: '>=12'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: 2cce1a48e6687f64d371d2e7fc9c7fbf
-    sha256: 97f69cae6513a1c64ce2ec87380f9a177e386af398300921a869c07e826b4949
-  manager: conda
-  name: zstandard
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py310hdeb6495_1.conda
-  version: 0.19.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    zstandard: '>=0.15'
-  hash:
-    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
-    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
-  manager: conda
-  name: conda-package-streaming
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
-  version: 0.7.0
-- category: main
-  dependencies:
-    cryptography: '>=38.0.0,<39'
-    python: '>=3.6'
-  hash:
-    md5: fbfa0a180d48c800f922a10a114a8632
-    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
-  manager: conda
-  name: pyopenssl
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
-  version: 22.1.0
-- category: main
-  dependencies:
-    cryptography: ''
-    dbus: ''
-    jeepney: '>=0.6'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: e135d0e3bbb226e8d53d31b4e4f6d93c
-    sha256: 25d2a00bf24a3cab81eba8f77eba8f70a7b3995041fc227f535c0f174536670f
-  manager: conda
-  name: secretstorage
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py310hff52083_1.tar.bz2
-  version: 3.3.3
-- category: main
-  dependencies:
-    conda-package-streaming: '>=0.7.0'
-    python: '>=3.7'
-  hash:
-    md5: 44800e9bd13143292097c65e57323038
-    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
-  manager: conda
-  name: conda-package-handling
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
-  version: 2.0.2
-- category: main
-  dependencies:
-    importlib_metadata: '>=4.11.4'
-    jaraco.classes: ''
-    jeepney: '>=0.4.2'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    secretstorage: '>=3.2'
-  hash:
-    md5: 1cc09aec47df38e68442c113f675c8e2
-    sha256: d6052c86a5aa3190bb3ee9ba49230c5a9083c588715a696693378228fadc135d
-  manager: conda
-  name: keyring
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/keyring-23.11.0-py310hff52083_0.tar.bz2
-  version: 23.11.0
-- category: main
-  dependencies:
-    brotlipy: '>=0.6.0'
-    certifi: ''
-    cryptography: '>=1.3.4'
-    idna: '>=2.0.0'
-    pyopenssl: '>=0.14'
-    pysocks: '>=1.5.6,<2.0,!=1.5.7'
-    python: <4.0
-  hash:
-    md5: 3078ef2359efd6ecadbc7e085c5e0592
-    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
-  manager: conda
-  name: urllib3
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
-  version: 1.26.13
-- category: main
-  dependencies:
-    certifi: '>=2017.4.17'
-    charset-normalizer: '>=2,<3'
-    idna: '>=2.5,<4'
-    python: '>=3.7,<4.0'
-    urllib3: '>=1.21.1,<1.27'
-  hash:
-    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
-    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
-  manager: conda
-  name: requests
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
-  version: 2.28.1
-- category: main
-  dependencies:
-    filelock: '>=3.8.0'
-    msgpack-python: '>=0.5.2'
-    python: '>=3.6'
-    requests: ''
-  hash:
-    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
-    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
-  manager: conda
-  name: cachecontrol
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
-  version: 0.12.12
-- category: main
-  dependencies:
-    conda-package-handling: '>=1.3.0'
-    pycosat: '>=0.6.3'
-    pyopenssl: '>=16.2.0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.20.1,<3'
-    ruamel_yaml: '>=0.11.14,<0.17'
-    setuptools: '>=31.0.1'
-    toolz: '>=0.8.1'
-  hash:
-    md5: 8d78ef95742dcd284e6a5ee99bb0659b
-    sha256: 9be2c55658fdfc9837c5d4f9bf2cc384ebbc8dd2bb8dbdb1300721a8abc93c95
-  manager: conda
-  name: conda
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/conda-22.9.0-py310hff52083_2.tar.bz2
-  version: 22.9.0
-- category: main
-  dependencies:
-    appdirs: ''
-    click: '>=5.1'
-    filelock: ''
-    python: '>=3.7'
-    requests: '>=2'
-  hash:
-    md5: c99ae3abf501990769047b4b40a98f17
-    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
-  manager: conda
-  name: ensureconda
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.3
-- category: main
-  dependencies:
-    docutils: ''
-    flit-core: 3.8.0 pyhd8ed1ab_0
-    pip: ''
-    python: '>=3.6'
-    requests: ''
-    tomli-w: ''
-  hash:
-    md5: d37c34176396c5402cf80c32e67731b7
-    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
-  manager: conda
-  name: flit
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: ''
-    requests: '>=2.0.1,<=3.0.0'
-  hash:
-    md5: 402668adee8fcba9a9c265cdc2a88f5a
-    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
-  manager: conda
-  name: requests-toolbelt
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
-  version: 0.9.1
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9'
-    cachy: '>=0.3.0'
-    click: '>=8.0'
-    click-default-group: ''
-    clikit: '>=0.6.2'
-    crashtest: '>=0.3.0'
-    ensureconda: '>=1.3'
-    filelock: '>=3.8.0'
-    html5lib: '>=1.0'
-    importlib-metadata: '>=1.7.0'
-    jinja2: ''
-    keyring: '>=21.2.0'
-    packaging: '>=20.4'
-    pkginfo: '>=1.4'
-    pydantic: '>=1.8.1'
-    python: '>=3.6'
-    pyyaml: '>=5.1'
-    requests: '>=2.18'
-    ruamel.yaml: ''
-    tomli: ''
-    tomlkit: '>=0.7.0'
-    toolz: <1.0.0,>=0.12.0
-    typing-extensions: ''
-    virtualenv: '>=20.0.26'
-  hash:
-    md5: 7b1dde4760c5c554523fead6c2771af2
-    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
-  manager: conda
-  name: conda-lock
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.1
-- category: main
-  dependencies:
-    conda: '>=4.8,<23.4'
-    libmambapy: 1.1.0 py310h69aa5bf_2
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 263d921fcebace4d7bd7ad2ac0b6ae3f
-    sha256: 7f142cc44354354baf12ccfba5ce39e2a0f4fde4bfb567ed42a4ca0f9b43589b
-  manager: conda
-  name: mamba
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/mamba-1.1.0-py310h51d5547_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9,<0.13.0'
-    cachy: '>=0.3.0,<0.4.0'
-    cleo: '>=0.8.1,<0.9.0'
-    clikit: '>=0.6.2,<0.7.0'
-    crashtest: '>=0.3.0,<0.4.0'
-    html5lib: '>=1.0,<2.0'
-    keyring: '>=21.2.0'
-    lockfile: '>=0.9'
-    packaging: '>=20.4,<21.0'
-    pexpect: '>=4.7.0,<5.0.0'
-    pkginfo: '>=1.4,<2.0'
-    poetry-core: '>=1.0.7,<1.1.0'
-    ptyprocess: '>=0.5'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.18,<3.0'
-    requests-toolbelt: '>=0.9.1,<0.10.0'
-    shellingham: '>=1.1,<2.0'
-    tomlkit: '>=0.7.0,<1.0.0'
-    virtualenv: '>=20.0.26,<21.0.0'
-  hash:
-    md5: 774207808696c8728977983b930f1cb5
-    sha256: ebeeffa1afaece3c6defc74dcb566a430a3b2d12c574000483bdb5a268b14f57
-  manager: conda
-  name: poetry
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/poetry-1.1.14-py310hff52083_0.tar.bz2
-  version: 1.1.14
-- category: main
-  dependencies: {}
-  hash:
-    md5: 37edc4e6304ca87316e160f5ca0bd1b5
-    sha256: 60ba4c64f5d0afca0d283c7addba577d3e2efc0db86002808dadb0498661b2f2
-  manager: conda
-  name: bzip2
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies: {}
-  hash:
-    md5: 00b3e98a61e6430808fe7a2534681f28
-    sha256: 1cb663c9916aab52a90a80505fec8c1a89fab21f58f3c5a949a2f286e92cb16c
-  manager: conda
-  name: c-ares
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.18.1-h0d85af4_0.tar.bz2
-  version: 1.18.1
-- category: main
-  dependencies: {}
-  hash:
-    md5: 67b268c32433047914482def1ce215c2
-    sha256: e1c929207f8a8e03fa86150c3b446f3511f35b2146d3031de305088c3b148c58
-  manager: conda
-  name: ca-certificates
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.9.24-h033912b_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies: {}
-  hash:
-    md5: 208a6a874b073277374de48a782f6b10
-    sha256: ebb75dd9f854b1f184a98d0b9128a3faed6cd2f05f83677e1f399c253580afe7
-  manager: conda
-  name: libcxx
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hccf4f1f_0.tar.bz2
-  version: 14.0.6
-- category: main
-  dependencies: {}
-  hash:
-    md5: 79dc2be110b2a3d1e97ec21f691c50ad
-    sha256: c4154d424431898d84d6afb8b32e3ba749fe5d270d322bb0af74571a3cb09c6b
-  manager: conda
-  name: libev
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2
-  version: '4.33'
-- category: main
-  dependencies: {}
-  hash:
-    md5: ccb34fb14960ad8b125962d3d79b31a9
-    sha256: 7a2d27a936ceee6942ea4d397f9c7d136f12549d86f7617e8b6bad51e01a941f
-  manager: conda
-  name: libffi
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
-  version: 3.4.2
-- category: main
-  dependencies: {}
-  hash:
-    md5: 691d103d11180486154af49c037b7ed9
-    sha256: 4a3294037d595754f7da7c11a41f3922f995aaa333f3cb66f02d8afa032a7bc2
-  manager: conda
-  name: libiconv
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2
-  version: '1.17'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 35eb3fce8d51ed3c1fd4122bad48250b
-    sha256: 0d954350222cc12666a1f4852dbc9bcf4904d8e467d29505f2b04ded6518f890
-  manager: conda
-  name: libzlib
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2
-  version: 1.2.13
-- category: main
-  dependencies: {}
-  hash:
-    md5: 0b6bca372a95d6c602c7a922e928ce79
-    sha256: c8a9401eff2efbbcc6da03d0066ee85d72402f7658c240e7968c64052a0d0493
-  manager: conda
-  name: lzo
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/lzo-2.10-haf1e3a3_1000.tar.bz2
-  version: '2.10'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 76217ebfbb163ff2770a261f955a5861
-    sha256: 9794a23d03586c99cac49d4ae3d5337faaa6bfc256b31d2662ff4ad5972be143
-  manager: conda
-  name: ncurses
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2
-  version: '6.3'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 878f923dd6acc8aeb47a75da6c4098be
-    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
-  manager: conda
-  name: pybind11-abi
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
-  version: '4'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 42da9b0138e911cd5b2f75b0278e26dc
-    sha256: 0a66852c47be6b28b70bde29891a71d047730c723355d44b0da48db79fb99eb1
-  manager: conda
-  name: python_abi
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-3_cp310.conda
-  version: '3.10'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 6f87f4707e4daf5823ce56dce5d9fbea
-    sha256: 7181e7eab6f959640e41c285d57670885c1db7f7a897b43c7d7fb47987222d32
-  manager: conda
-  name: reproc
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/reproc-14.2.3-h0d85af4_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies: {}
-  hash:
-    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
-    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
-  manager: conda
-  name: tzdata
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
-  version: 2022g
-- category: main
-  dependencies: {}
-  hash:
-    md5: a72f9d4ea13d55d745ff1ed594747f10
-    sha256: eb09823f34cc2dd663c0ec4ab13f246f45dcd52e5b8c47b9864361de5204a1c8
-  manager: conda
-  name: xz
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
-  version: 5.2.6
-- category: main
-  dependencies: {}
-  hash:
-    md5: d7e08fcf8259d742156188e8762b4d20
-    sha256: 5301417e2c8dea45b401ffee8df3957d2447d4ce80c83c5ff151fc6bfe1c4148
-  manager: conda
-  name: yaml
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
-  version: 0.2.5
-- category: main
-  dependencies:
-    libcxx: '>=14.0.4'
-  hash:
-    md5: 310d897883dbdd88555d6321a4c2e6e8
-    sha256: 4891b66c94df8a346010caefb5d92df5e367be87ef0dea35a15d988f39a82719
-  manager: conda
-  name: fmt
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/fmt-9.1.0-hb8565cd_0.tar.bz2
-  version: 9.1.0
-- category: main
-  dependencies:
-    libcxx: '>=12.0.1'
-  hash:
-    md5: 376635049e9b9b0bb875efd39dcd7b3b
-    sha256: 0807aa3fd93804ab239808d149e7f210a83e1c61bc59bb84818f4ef9f6036d86
-  manager: conda
-  name: icu
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2
-  version: '70.1'
-- category: main
-  dependencies:
-    ncurses: '>=6.2,<7.0.0a0'
-  hash:
-    md5: 6016a8a1d0e63cac3de2c352cd40208b
-    sha256: dbd3c3f2eca1d21c52e4c03b21930bbce414c4592f8ce805801575b9e9256095
-  manager: conda
-  name: libedit
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
-  version: 3.1.20191231
-- category: main
-  dependencies:
-    libcxx: '>=12.0.1'
-    libzlib: '>=1.2.11,<1.3.0a0'
-  hash:
-    md5: 068ed0617893ecbccbf65a32ea1e8056
-    sha256: 7c04b4a878ccc596b9ec71e2418c49e713e5c32748437134ec72dca51820374c
-  manager: conda
-  name: libsolv
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libsolv-0.7.22-hd9580d2_0.tar.bz2
-  version: 0.7.22
-- category: main
-  dependencies:
-    libzlib: '>=1.2.13,<1.3.0a0'
-  hash:
-    md5: ceb13b6726534b96e3b4e3dda91e9050
-    sha256: ae19f866188cc0c514fed754468460ae9e8dd763ebbd7b7afc4e818d71844297
-  manager: conda
-  name: libsqlite
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.40.0-ha978bb4_0.tar.bz2
-  version: 3.40.0
-- category: main
-  dependencies:
-    libcxx: '>=11.1.0'
-  hash:
-    md5: 05c08241b66631c00ca4f9e0b75320bc
-    sha256: 627c435c511e789ed04e0e2077fdfc645117474c4d1c4a7c0d31241936632cd4
-  manager: conda
-  name: lz4-c
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.3-he49afe7_1.tar.bz2
-  version: 1.9.3
-- category: main
-  dependencies:
-    ca-certificates: ''
-  hash:
-    md5: 7a3fb6d40e0aa5dbb5b4ef54462f00a8
-    sha256: 3eb19686ae870daae035582cb93253a6435f71baf537addced41be449b4daf67
-  manager: conda
-  name: openssl
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.0.7-hfd90126_1.conda
-  version: 3.0.7
-- category: main
-  dependencies:
-    ncurses: '>=6.3,<7.0a0'
-  hash:
-    md5: 89fa404901fa8fb7d4f4e07083b8d635
-    sha256: c65dc1200a252832db49bdd6836c512a0eaafe97aa914b9f8358b15eebb1d94b
-  manager: conda
-  name: readline
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/readline-8.1.2-h3899abd_0.tar.bz2
-  version: 8.1.2
-- category: main
-  dependencies:
-    libcxx: '>=11.1.0'
-    reproc: 14.2.3 h0d85af4_0
-  hash:
-    md5: 7dafcfaa471cd16cbd73832cefc39770
-    sha256: e7f7ca953a0888b37cee9197ed844d67af02036c87402174935107827779bbf4
-  manager: conda
-  name: reproc-cpp
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/reproc-cpp-14.2.3-he49afe7_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies:
-    libzlib: '>=1.2.11,<1.3.0a0'
-  hash:
-    md5: 8e9480d9c47061db2ed1b4ecce519a7f
-    sha256: 331aa1137a264fd9cc905f04f09a161c801fe504b93da08b4e6697bd7c9ae6a6
-  manager: conda
-  name: tk
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2
-  version: 8.6.12
-- category: main
-  dependencies:
-    libcxx: '>=14.0.4'
-  hash:
-    md5: 06c92b93b45ed2c842eb0893c5d2552a
-    sha256: 9d1c5df1d4503d1451b5fe46a7502eb8ee98aa603f3f092f7fcf3e0d43d2a8f3
-  manager: conda
-  name: yaml-cpp
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/yaml-cpp-0.7.0-hf0c8a7f_2.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    libzlib: 1.2.12 hfe4f2af_2
-  hash:
-    md5: fe7ebd3b35b8f26f6a7d0af481a21721
-    sha256: 8f455dcebeae224fdb422ba8f90d33e61298dc088139227e25eb4ee20a3ea35f
-  manager: conda
-  name: zlib
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/zlib-1.2.12-hfe4f2af_2.tar.bz2
-  version: 1.2.12
-- category: main
-  dependencies:
-    libcxx: '>=13.0.1'
-    libzlib: '>=1.2.12,<1.3.0a0'
-  hash:
-    md5: 0b446e84f3ccf085e590dc1f73eebe3f
-    sha256: acf19719a0a4b7534532166f84346709fdb8ccf960bc6c19ac3b437177e95dde
-  manager: conda
-  name: zstd
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hfa58983_4.tar.bz2
-  version: 1.5.2
-- category: main
-  dependencies:
-    libcxx: '>=12.0.1'
-    libedit: '>=3.1.20191231,<4.0a0'
-    openssl: '>=3.0.0,<4.0a0'
-  hash:
-    md5: 8acf20165e07870bc65510a363ff45bb
-    sha256: 7f4de03413501f22f287a9fad86710de0f47b459ecf08026257e9a49d7c93428
-  manager: conda
-  name: krb5
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.19.3-hb98e516_0.tar.bz2
-  version: 1.19.3
-- category: main
-  dependencies:
-    c-ares: '>=1.18.1,<2.0a0'
-    libcxx: '>=13.0.1'
-    libev: '>=4.33,<4.34.0a0'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    openssl: '>=3.0.5,<4.0a0'
-  hash:
-    md5: 19d5ae4be3e4b3cfa5696f3667e8c631
-    sha256: 9e14d62e4462e6be28bcaa266f69e96ead43f4d7ef566e9cd460dbc9ae999daf
-  manager: conda
-  name: libnghttp2
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.47.0-h5aae05b_1.tar.bz2
-  version: 1.47.0
-- category: main
-  dependencies:
-    libzlib: '>=1.2.12,<1.3.0a0'
-    openssl: '>=3.0.5,<4.0a0'
-  hash:
-    md5: 5a28624eeb7812b585b9e2d75f846ba2
-    sha256: 3261dc7fa9cb928e8a0da4857b89bdd3e965766a6cd5b6456d4407cba6b25402
-  manager: conda
-  name: libssh2
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.10.0-h47af595_3.tar.bz2
-  version: 1.10.0
-- category: main
-  dependencies:
-    icu: '>=70.1,<71.0a0'
-    libiconv: '>=1.17,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    xz: '>=5.2.6,<6.0a0'
-  hash:
-    md5: 13ba8bf8f44cdac2e5401dac20a36040
-    sha256: 464b3e2350c25615bbea89ab512f8f5fcd88a9e2f6cf9dfe7b72aa9bc56efcda
-  manager: conda
-  name: libxml2
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.10.3-hb9e07b5_0.tar.bz2
-  version: 2.10.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-    readline: '>=8.1.2,<9.0a0'
-    tk: '>=8.6.12,<8.7.0a0'
-    tzdata: ''
-    xz: '>=5.2.6,<6.0a0'
-  hash:
-    md5: 4b6976686db5f16650df28332d84ce9e
-    sha256: b001073de81761dc30848a55e92fd2eb4cb9fc60c2809afa0987c2a7d7f621f9
-  manager: conda
-  name: python
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.8-he7542f4_0_cpython.conda
-  version: 3.10.8
-- category: main
-  dependencies:
-    libzlib: '>=1.2.12,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    readline: '>=8.1.2,<9.0a0'
-    zlib: '>=1.2.12,<1.3.0a0'
-  hash:
-    md5: eea4504fd46050a22d482addde6ae7c7
-    sha256: 437de0e2658840c53ce8f6a4cb748aca49205fefe0b61164151372be2cfbef40
-  manager: conda
-  name: sqlite
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/sqlite-3.39.2-hd9f0692_0.tar.bz2
-  version: 3.39.2
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 5f095bc6454094e96f146491fd03633b
-    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
-  manager: conda
-  name: appdirs
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
-  version: 1.4.4
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 5dfee17f24e2dfd18d7392b48c9351e2
-    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
-  manager: conda
-  name: cachy
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
-  version: 0.3.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: f66309b099374af91369e67e84af397d
-    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
-  manager: conda
-  name: certifi
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: c1d5b294fbf9a795dec349a6f4d8be8e
-    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
-  manager: conda
-  name: charset-normalizer
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    __unix: ''
-    python: '>=3.8'
-  hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
-  manager: conda
-  name: click
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: c267da48ce208905d7d976d49dfd9433
-    sha256: fcab1a16af5daf3a1ea9b0a7ed15615f0d5fff05ff4925ed570988868bb29e38
-  manager: conda
-  name: colorama
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2
-  version: 0.4.5
-- category: main
-  dependencies:
-    python: '>=3.6,<4.0'
-  hash:
-    md5: b8477552274c1cfdb533e954c76523f1
-    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
-  manager: conda
-  name: crashtest
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.1
-- category: main
-  dependencies:
-    python: 2.7|>=3.6
-  hash:
-    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
-    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
-  manager: conda
-  name: distlib
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.6
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 932d057a35046e6eb92561c723d4ebe6
-    sha256: 72c1aa5ae0133081037e7c7115633ad7308e85aa871347f70ebf677e12f41ce6
-  manager: conda
-  name: docutils
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py310h2ec42d9_1.tar.bz2
-  version: '0.19'
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
-    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
-  manager: conda
-  name: filelock
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
-  version: 3.8.2
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 6d5e56de2e65da7aa35fd10131226efa
-    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
-  manager: conda
-  name: flit-core
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 34272b248891bddccc64479f9a7fffed
-    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
-  manager: conda
-  name: idna
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
-  version: '3.4'
-- category: main
-  dependencies:
-    python: 2.7|>=3.4
-  hash:
-    md5: 25045ddd7fe83ddf71c181d6212e9913
-    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
-  manager: conda
-  name: invoke
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.7.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libiconv: '>=1.16,<2.0.0a0'
-    libxml2: '>=2.9.14,<2.11.0a0'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    lz4-c: '>=1.9.3,<1.10.0a0'
-    lzo: '>=2.10,<3.0a0'
-    openssl: '>=3.0.3,<4.0a0'
-    xz: '>=5.2.5,<5.3.0a0'
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: 57f1c0e98ad3d4836d66d457f3690dc9
-    sha256: 0eed997df470af8f268d69428dacc51a26d1ecafea1de446c406f4d5f8ae5469
-  manager: conda
-  name: libarchive
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarchive-3.5.2-hbf7dfe4_3.tar.bz2
-  version: 3.5.2
-- category: main
-  dependencies:
-    krb5: '>=1.19.3,<1.20.0a0'
-    libnghttp2: '>=1.47.0,<2.0a0'
-    libssh2: '>=1.10.0,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-  hash:
-    md5: af83102fc53762fb78e27657b540756f
-    sha256: f76129b5fbb7d08a1457ce36eb16b32da470ccd5ad8e498265c97750ccddd921
-  manager: conda
-  name: libcurl
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libcurl-7.86.0-h581aaea_1.tar.bz2
-  version: 7.86.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: c104d98e09c47519950cffb8dd5b4f10
-    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
-  manager: conda
-  name: lockfile
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
-  version: 0.12.2
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 232c20719e4290fa284ae1e9a4661dfa
-    sha256: 45aa996770bb49fdd6bc68e24b301932c2bb592522e3798f0c80e0206c352b8b
-  manager: conda
-  name: markupsafe
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py310h90acd4f_2.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 9b6ad26944f19f599800b068e0582227
-    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
-  manager: conda
-  name: more-itertools
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 9.0.0
-- category: main
-  dependencies:
-    libcxx: '>=14.0.4'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 164e856479d735e96fcbd547afa70251
-    sha256: c8311366a2858a24b3ac65fa1c6f8ca63f83528bbb2f6825cdf56d30047d022b
-  manager: conda
-  name: msgpack-python
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.4-py310ha23aa8a_1.tar.bz2
-  version: 1.0.4
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: a4eea5bff523f26442405bc5d1f52adb
-    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
-  manager: conda
-  name: pastel
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.2.1
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
-    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
-  manager: conda
-  name: pkginfo
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
-  version: 1.9.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2fb3f88922e7aec26ba652fcdfe13950
-    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
-  manager: conda
-  name: platformdirs
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
-  version: 2.5.2
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: f8d8f3b9a093c53d03ca1ca52fab989c
-    sha256: 864e4ae20da2fb810a9ecb948396b49705a35f5b36f909a3e2b10abdfe4b0dca
-  manager: conda
-  name: poetry-core
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/poetry-core-1.0.8-py310h2ec42d9_1.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 359eeb6536da0e687af562ed265ec263
-    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
-  manager: conda
-  name: ptyprocess
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 95c032c354c500001a935aac4c059376
-    sha256: 28012e6ae66102b9b4f69316d026985373b2c33161304bc6841c1d9c3f9ec34e
-  manager: conda
-  name: pycosat
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pycosat-0.6.4-py310h90acd4f_1.tar.bz2
-  version: 0.6.4
-- category: main
-  dependencies:
-    python: 2.7.*|>=3.4
-  hash:
-    md5: 076becd9e05608f8dc72757d5f3a91ff
-    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
-  manager: conda
-  name: pycparser
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
-  version: '2.21'
-- category: main
-  dependencies:
-    python: '>=3.3'
-  hash:
-    md5: edf8651c4379d9d1495ad6229622d150
-    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
-  manager: conda
-  name: pylev
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: e8fbc1b54b25f4b08281467bc13b70cc
-    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
-  manager: conda
-  name: pyparsing
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
-  version: 3.0.9
-- category: main
-  dependencies:
-    __unix: ''
-    python: '>=3.8'
-  hash:
-    md5: 2a7de29fb590ca14b5243c4c812c8025
-    sha256: a42f826e958a8d22e65b3394f437af7332610e43ee313393d1cf143f0a2d274b
-  manager: conda
-  name: pysocks
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
-  version: 1.7.1
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: e0ba2009f52ccda088c63dedf0d1c5ec
-    sha256: ab7b2b8fef9adc4211834054d004f3e286161bb3e1dcb17d4b974fae4f87b31b
-  manager: conda
-  name: pyyaml
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h90acd4f_5.tar.bz2
-  version: '6.0'
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: a47602a6c5a1fc89a64b91bb44036537
-    sha256: 9231096ef851e63705df491ffa2d0571d68757630c52513b5dd655474d37741f
-  manager: conda
-  name: ruamel.yaml.clib
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py310h90acd4f_0.tar.bz2
-  version: 0.2.7
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: 936cc17fa13ae01bcbd1daaf4e31fc72
-    sha256: 6212a6298cda55296a32724ed1065cb6b9ba55c2df7fecf650be4a4ac373f5d7
-  manager: conda
-  name: ruamel_yaml
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel_yaml-0.15.80-py310h90acd4f_1008.tar.bz2
-  version: 0.15.80
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
-    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
-  manager: conda
-  name: setuptools
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
-  version: 65.5.1
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 437655338696f9d0dfdb0a024e66b255
-    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
-  manager: conda
-  name: shellingham
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: e5f25f8dbc060e9a8d912e432202afc2
-    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
-  manager: conda
-  name: six
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
-  version: 1.16.0
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: f832c45a477c78bebd107098db465095
-    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
-  manager: conda
-  name: toml
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
-  version: 0.10.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 5844808ffab9ebdb694585b50ba02a96
-    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
-  manager: conda
-  name: tomli
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.0.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 73506d1ab4202481841c68c169b7ef6c
-    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
-  manager: conda
-  name: tomli-w
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.0.0
-- category: main
-  dependencies:
-    python: '>=3.5'
-  hash:
-    md5: 92facfec94bc02d6ccf42e7173831a36
-    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
-  manager: conda
-  name: toolz
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
-  version: 0.12.0
-- category: main
-  dependencies:
-    python: '>=3'
-  hash:
-    md5: e6573ac68718f17b9d4f5c8eda3190f2
-    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
-  manager: conda
-  name: typing
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.10.0.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2d93b130d148d7fc77e583677792fc6a
-    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
-  manager: conda
-  name: typing_extensions
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 3563be4c5611a44210d9ba0c16113136
-    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
-  manager: conda
-  name: webencodings
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
-  version: 0.5.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: c829cfb8cb826acb9de0ac1a2df0a940
-    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
-  manager: conda
-  name: wheel
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
-  version: 0.38.4
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 09b5b885341697137879a4f039a9e5a1
-    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
-  manager: conda
-  name: zipp
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
-  version: 3.11.0
-- category: main
-  dependencies:
-    libffi: '>=3.4,<4.0a0'
-    pycparser: ''
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: dacdbcd6bcec3dc5b34f1f6a06915b66
-    sha256: b548a2f5ba121a698010a9c4b05009f5e701d5d16da0b24fbad9691f8d84b17e
-  manager: conda
-  name: cffi
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_2.tar.bz2
-  version: 1.15.1
-- category: main
-  dependencies:
-    click: ''
-    python: '>=3.6'
-  hash:
-    md5: 72a46ffc25701c173932fd55cf0965d3
-    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
-  manager: conda
-  name: click-default-group
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.2
-- category: main
-  dependencies:
-    crashtest: '>=0.3.0,<0.4.0'
-    pastel: '>=0.2.0,<0.3.0'
-    pylev: '>=1.3,<2.0'
-    python: ''
-  hash:
-    md5: 159273f717a11e53b2656f8b6521a5e2
-    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
-  manager: conda
-  name: clikit
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
-  version: 0.6.2
-- category: main
-  dependencies:
-    python: ''
-    six: '>=1.9'
-    webencodings: ''
-  hash:
-    md5: b2355343d6315c892543200231d7154a
-    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
-  manager: conda
-  name: html5lib
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
-  version: '1.1'
-- category: main
-  dependencies:
-    python: '>=3.8'
-    zipp: '>=0.5'
-  hash:
-    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
-    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
-  manager: conda
-  name: importlib-metadata
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    more-itertools: ''
-    python: '>=3.7'
-  hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
-  manager: conda
-  name: jaraco.classes
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
-  version: 3.2.3
-- category: main
-  dependencies:
-    markupsafe: '>=2.0'
-    python: '>=3.7'
-  hash:
-    md5: c8490ed5c70966d232fdd389d0dbed37
-    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
-  manager: conda
-  name: jinja2
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
-  version: 3.1.2
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libarchive: '>=3.5.2,<3.6.0a0'
-    libcurl: '>=7.86.0,<8.0a0'
-    libcxx: '>=14.0.6'
-    libiconv: '>=1.17,<2.0a0'
-    libsolv: '>=0.7.22,<0.8.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-    reproc-cpp: '>=14.2,<15.0a0'
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: b2f3194abef248954cbd738d602fc6a5
-    sha256: 3af6ff8646629c59b2777a39f25abd05010ca9c4111079cd92d48a94597a51bb
-  manager: conda
-  name: libmamba
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.1.0-h8b63968_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    pyparsing: '>=2.0.2,!=3.0.5'
-    python: '>=3.6'
-  hash:
-    md5: 71f1ab2de48613876becddd496371c85
-    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
-  manager: conda
-  name: packaging
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
-  version: '21.3'
-- category: main
-  dependencies:
-    ptyprocess: '>=0.5'
-    python: ''
-  hash:
-    md5: 5909e7b978141dd80d28dbf9de627827
-    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
-  manager: conda
-  name: pexpect
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
-  version: 4.8.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    setuptools: ''
-    wheel: ''
-  hash:
-    md5: da66f2851b9836d3a7c5190082a45f7d
-    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
-  manager: conda
-  name: pip
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 22.3.1
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ruamel.yaml.clib: '>=0.1.2'
-    setuptools: ''
-  hash:
-    md5: b7921dd86e7931ff90727c3545f9a976
-    sha256: 520193524d3c12723d0d675e4fa059ec078e103a88cd3069692c32ff9f57cfda
-  manager: conda
-  name: ruamel.yaml
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.21-py310h90acd4f_2.tar.bz2
-  version: 0.17.21
-- category: main
-  dependencies:
-    python: '>=3.6'
-    typing: '>=3.6,<4.0'
-  hash:
-    md5: 471bf9e605820b59988e830382b8d654
-    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
-  manager: conda
-  name: tomlkit
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
-  version: 0.11.6
-- category: main
-  dependencies:
-    colorama: ''
-    python: '>=2.7'
-  hash:
-    md5: 6642233f341e1900d0c8e6eddb979c14
-    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
-  manager: conda
-  name: tqdm
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
-  version: 4.64.0
-- category: main
-  dependencies:
-    typing_extensions: 4.4.0 pyha770c72_0
-  hash:
-    md5: be969210b61b897775a0de63cd9e9026
-    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
-  manager: conda
-  name: typing-extensions
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    distlib: '>=0.3.6,<1'
-    filelock: '>=3.4.1,<4'
-    platformdirs: '>=2.4,<3'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: a8c9ed46d17f8a92a457e5d0433e8468
-    sha256: 6afe16afef89bf2d51d9ed4588cfb2eb6205dc44d04b46b30d2c70203bfa741d
-  manager: conda
-  name: virtualenv
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.17.0-py310h2ec42d9_0.conda
-  version: 20.17.0
-- category: main
-  dependencies:
-    cffi: '>=1.0.0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 63accc45f2b9ae1dad4db9cdfaa903b4
-    sha256: de6e5b17631ef35c6acaeec0ba0143d0e77e0970704f0a3e947a5d59364f3c4a
-  manager: conda
-  name: brotlipy
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    clikit: '>=0.6.0,<0.7.0'
-    python: '>=3.6'
-  hash:
-    md5: 4c82b11a3d06031bd58e7d869f53d965
-    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
-  manager: conda
-  name: cleo
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
-  version: 0.8.1
-- category: main
-  dependencies:
-    cffi: '>=1.12'
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 7f0791ebd6b9c996fbd16ed1368b7eee
-    sha256: 16cfba388e76b1b22b31a0f9ec864f5d4e19902f72eb65b29e2eebb2a1bdc9db
-  manager: conda
-  name: cryptography
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-38.0.4-py310hdd0c95c_0.conda
-  version: 38.0.4
-- category: main
-  dependencies:
-    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
-  hash:
-    md5: 3dc2248927de739b4d2e2da9a9972bfe
-    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
-  manager: conda
-  name: importlib_metadata
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libcxx: '>=14.0.6'
-    libmamba: 1.1.0 h8b63968_2
-    openssl: '>=3.0.7,<4.0a0'
-    pybind11-abi: '4'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: 2b0e4f8eecc71ac0e8e01a01040cb871
-    sha256: a6cf61d04fac8a57490662cc65b686206f9d66954a1d5cdf1ea7db70aa57a9e3
-  manager: conda
-  name: libmambapy
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.1.0-py310hb15139c_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    typing-extensions: '>=4.1.0'
-  hash:
-    md5: 140aaad46ef1de7f9ca167dfebf40aad
-    sha256: fb689bccf7ce9b1643ec59003fc51f4dca3fe719a86782fce72a1b6bd549ecd5
-  manager: conda
-  name: pydantic
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.2-py310h90acd4f_1.tar.bz2
-  version: 1.10.2
-- category: main
-  dependencies:
-    cffi: '>=1.11'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: 6daa5261761ae2a155f21f5a6c162b27
-    sha256: f43d356b78cde97a2a4b0798d5e3256315e6323343ef0d5e69578ce685237838
-  manager: conda
-  name: zstandard
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py310h3cf44b0_1.conda
-  version: 0.19.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    zstandard: '>=0.15'
-  hash:
-    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
-    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
-  manager: conda
-  name: conda-package-streaming
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
-  version: 0.7.0
-- category: main
-  dependencies:
-    importlib_metadata: '>=4.11.4'
-    jaraco.classes: ''
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 2ea3fb1aedecb07304bbc73c8ce3f0ea
-    sha256: fb1229a850420b5f6fd5855b54cfbc837100c0f5c862bc288bb302f0455af035
-  manager: conda
-  name: keyring
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/keyring-23.11.0-py310h2ec42d9_0.tar.bz2
-  version: 23.11.0
-- category: main
-  dependencies:
-    cryptography: '>=38.0.0,<39'
-    python: '>=3.6'
-  hash:
-    md5: fbfa0a180d48c800f922a10a114a8632
-    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
-  manager: conda
-  name: pyopenssl
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
-  version: 22.1.0
-- category: main
-  dependencies:
-    conda-package-streaming: '>=0.7.0'
-    python: '>=3.7'
-  hash:
-    md5: 44800e9bd13143292097c65e57323038
-    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
-  manager: conda
-  name: conda-package-handling
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
-  version: 2.0.2
-- category: main
-  dependencies:
-    brotlipy: '>=0.6.0'
-    certifi: ''
-    cryptography: '>=1.3.4'
-    idna: '>=2.0.0'
-    pyopenssl: '>=0.14'
-    pysocks: '>=1.5.6,<2.0,!=1.5.7'
-    python: <4.0
-  hash:
-    md5: 3078ef2359efd6ecadbc7e085c5e0592
-    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
-  manager: conda
-  name: urllib3
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
-  version: 1.26.13
-- category: main
-  dependencies:
-    certifi: '>=2017.4.17'
-    charset-normalizer: '>=2,<3'
-    idna: '>=2.5,<4'
-    python: '>=3.7,<4.0'
-    urllib3: '>=1.21.1,<1.27'
-  hash:
-    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
-    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
-  manager: conda
-  name: requests
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
-  version: 2.28.1
-- category: main
-  dependencies:
-    filelock: '>=3.8.0'
-    msgpack-python: '>=0.5.2'
-    python: '>=3.6'
-    requests: ''
-  hash:
-    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
-    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
-  manager: conda
-  name: cachecontrol
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
-  version: 0.12.12
-- category: main
-  dependencies:
-    conda-package-handling: '>=1.3.0'
-    pycosat: '>=0.6.3'
-    pyopenssl: '>=16.2.0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.20.1,<3'
-    ruamel_yaml: '>=0.11.14,<0.17'
-    setuptools: '>=31.0.1'
-    toolz: '>=0.8.1'
-  hash:
-    md5: 2cf59c02b1e43a37232da097fe9024db
-    sha256: a55ab27dc68ffc0d421750cd840fddeb44a27270530496dfa316bc4cbbf5d50d
-  manager: conda
-  name: conda
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/conda-22.9.0-py310h2ec42d9_2.tar.bz2
-  version: 22.9.0
-- category: main
-  dependencies:
-    appdirs: ''
-    click: '>=5.1'
-    filelock: ''
-    python: '>=3.7'
-    requests: '>=2'
-  hash:
-    md5: c99ae3abf501990769047b4b40a98f17
-    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
-  manager: conda
-  name: ensureconda
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.3
-- category: main
-  dependencies:
-    docutils: ''
-    flit-core: 3.8.0 pyhd8ed1ab_0
-    pip: ''
-    python: '>=3.6'
-    requests: ''
-    tomli-w: ''
-  hash:
-    md5: d37c34176396c5402cf80c32e67731b7
-    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
-  manager: conda
-  name: flit
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: ''
-    requests: '>=2.0.1,<=3.0.0'
-  hash:
-    md5: 402668adee8fcba9a9c265cdc2a88f5a
-    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
-  manager: conda
-  name: requests-toolbelt
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
-  version: 0.9.1
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9'
-    cachy: '>=0.3.0'
-    click: '>=8.0'
-    click-default-group: ''
-    clikit: '>=0.6.2'
-    crashtest: '>=0.3.0'
-    ensureconda: '>=1.3'
-    filelock: '>=3.8.0'
-    html5lib: '>=1.0'
-    importlib-metadata: '>=1.7.0'
-    jinja2: ''
-    keyring: '>=21.2.0'
-    packaging: '>=20.4'
-    pkginfo: '>=1.4'
-    pydantic: '>=1.8.1'
-    python: '>=3.6'
-    pyyaml: '>=5.1'
-    requests: '>=2.18'
-    ruamel.yaml: ''
-    tomli: ''
-    tomlkit: '>=0.7.0'
-    toolz: <1.0.0,>=0.12.0
-    typing-extensions: ''
-    virtualenv: '>=20.0.26'
-  hash:
-    md5: 7b1dde4760c5c554523fead6c2771af2
-    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
-  manager: conda
-  name: conda-lock
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.1
-- category: main
-  dependencies:
-    conda: '>=4.8,<23.4'
-    libmambapy: 1.1.0 py310hb15139c_2
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 2bf0001c9bb77ded523219dd77549db1
-    sha256: 8bc81d851ab65e517a4a1d28be3c31993cd21e9a75ee49fce76872967b9a5965
-  manager: conda
-  name: mamba
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/mamba-1.1.0-py310h6bde348_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9,<0.13.0'
-    cachy: '>=0.3.0,<0.4.0'
-    cleo: '>=0.8.1,<0.9.0'
-    clikit: '>=0.6.2,<0.7.0'
-    crashtest: '>=0.3.0,<0.4.0'
-    html5lib: '>=1.0,<2.0'
-    keyring: '>=21.2.0'
-    lockfile: '>=0.9'
-    packaging: '>=20.4,<21.0'
-    pexpect: '>=4.7.0,<5.0.0'
-    pkginfo: '>=1.4,<2.0'
-    poetry-core: '>=1.0.7,<1.1.0'
-    ptyprocess: '>=0.5'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.18,<3.0'
-    requests-toolbelt: '>=0.9.1,<0.10.0'
-    shellingham: '>=1.1,<2.0'
-    tomlkit: '>=0.7.0,<1.0.0'
-    virtualenv: '>=20.0.26,<21.0.0'
-  hash:
-    md5: 7bc43495d162b6be9590ffe65422963f
-    sha256: 90fc5ab9dbbed1c1739d1fa5b1d26f4f6a87c1f56dee7178a18885433bde6f49
-  manager: conda
-  name: poetry
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/poetry-1.1.14-py310h2ec42d9_0.tar.bz2
-  version: 1.1.14
-- category: main
-  dependencies: {}
-  hash:
-    md5: 5fba0abc60bf327a4bc4188cd64678be
-    sha256: 564f7c91d51b8b7b7111fd207bcbefe5c4f6c2075e41dc1b44725d974325ed90
-  manager: conda
-  name: ca-certificates
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.9.24-h5b45459_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies: {}
-  hash:
-    md5: 878f923dd6acc8aeb47a75da6c4098be
-    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
-  manager: conda
-  name: pybind11-abi
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
-  version: '4'
-- category: main
-  dependencies: {}
-  hash:
-    md5: f4cfd883c0d91bb17164d8e34f4900d5
-    sha256: 8212c6f1a68d5a494bcde5cd64196626024059dcbe8995469c8a5ed32694efa0
-  manager: conda
-  name: python_abi
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-3_cp310.conda
-  version: '3.10'
-- category: main
-  dependencies: {}
-  hash:
-    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
-    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
-  manager: conda
-  name: tzdata
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
-  version: 2022g
-- category: main
-  dependencies: {}
-  hash:
-    md5: 72608f6cd3e5898229c3ea16deb1ac43
-    sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
-  manager: conda
-  name: ucrt
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
-  version: 10.0.22621.0
-- category: main
-  dependencies:
-    ucrt: '>=10.0.20348.0'
-  hash:
-    md5: c98b6e39006315599b793592bcc3c978
-    sha256: 6b6feb349d3414655c2f9c549092689e5f99b487ff7ed9c1f1fda69a5dd4a624
-  manager: conda
-  name: vs2015_runtime
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.32.31332-h1d6e394_9.tar.bz2
-  version: 14.32.31332
-- category: main
-  dependencies:
-    vs2015_runtime: '>=14.32.31332'
-  hash:
-    md5: ba28983ef4f6d430827d0e7c5cdd7b48
-    sha256: 1ca9e60e4e977be81dbee0ed236c6fb0a459c32957d2c2dc45a114d83f4c70d6
-  manager: conda
-  name: vc
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h3d8a991_9.tar.bz2
-  version: '14.3'
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: 7c03c66026944073040cb19a4f3ec3c9
-    sha256: 5389dad4e73e4865bb485f460fc60b120bae74404003d457ecb1a62eb7abf0c1
-  manager: conda
-  name: bzip2
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies:
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30037'
-  hash:
-    md5: 31a20cf261b2bd0a76d670db1b3e6fa1
-    sha256: b4882f05294a46949cf4d15e4b2c50f29257b0d042d7d8184e4722b392d71193
-  manager: conda
-  name: fmt
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/fmt-9.1.0-h181d51b_0.tar.bz2
-  version: 9.1.0
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: 2c96d1b6915b408893f9472569dee135
-    sha256: 1951ab740f80660e9bc07d2ed3aefb874d78c107264fd810f24a1a6211d4b1a5
-  manager: conda
-  name: libffi
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
-  version: 3.4.2
-- category: main
-  dependencies:
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: 050119977a86e4856f0416e2edcf81bb
-    sha256: 657c2a992c896475021a25faebd9ccfaa149c5d70c7dc824d4069784b686cea1
-  manager: conda
-  name: libiconv
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2
-  version: '1.17'
-- category: main
-  dependencies:
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 5e5a97795de72f8cc3baf3d9ea6327a2
-    sha256: 4e50b3d90a351c9d47d239d3f90fce4870df2526e4f7fef35203ab3276a6dfc9
-  manager: conda
-  name: libsqlite
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.40.0-hcfcfb64_0.tar.bz2
-  version: 3.40.0
-- category: main
-  dependencies:
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 0cc5c5cc64ee1637f37f8540a175854c
-    sha256: 184da12b4296088a47086f4e69e65eb5f8537a824ee3131d8076775e1d1ea767
-  manager: conda
-  name: libzlib
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2
-  version: 1.2.13
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: d12763533276560a931c1bd3df1adf63
-    sha256: 1d4b25978dc5f158d235908f1fd541116e9db3f31229bda665c4d3ff6b3979f8
-  manager: conda
-  name: lz4-c
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.3-h8ffe710_1.tar.bz2
-  version: 1.9.3
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: d5cf4b7eaa52316f135eed9e8548ad57
-    sha256: ff064e34d3cad829f1e31f2d26125b61d20ba8d3771f8f5337069027b8e3fab4
-  manager: conda
-  name: lzo
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/lzo-2.10-he774522_1000.tar.bz2
-  version: '2.10'
-- category: main
-  dependencies:
-    ca-certificates: ''
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: e48b661f57b25ddf34996fa8b685182d
-    sha256: 3f26c38e6167d7351de5bdcf13d1456891c242711e689999c25e50e5898bb660
-  manager: conda
-  name: openssl
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.0.7-hcfcfb64_1.conda
-  version: 3.0.7
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: 843a3cd031e593c24b542206c3444a2b
-    sha256: 3aec1eebaa039abb4c5accd9df021193859a7b8855555d2bd0465972f55fdc45
-  manager: conda
-  name: reproc
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/reproc-14.2.3-h8ffe710_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies:
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: 902c57a6f2f2e0b837a004004cd2ca57
-    sha256: ff4522ccfed5453dd773a935cf034b307872eba6814aa2798bef1cd4cc5e67df
-  manager: conda
-  name: sqlite
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/sqlite-3.39.2-h8ffe710_0.tar.bz2
-  version: 3.39.2
-- category: main
-  dependencies:
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: c69a5047cc9291ae40afd4a1ad6f0c0f
-    sha256: 087795090a99a1d397ef1ed80b4a01fabfb0122efb141562c168e3c0a76edba6
-  manager: conda
-  name: tk
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2
-  version: 8.6.12
-- category: main
-  dependencies:
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: 515d77642eaa3639413c6b1bc3f94219
-    sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
-  manager: conda
-  name: xz
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
-  version: 5.2.6
-- category: main
-  dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: adbfb9f45d1004a26763652246a33764
-    sha256: 4e2246383003acbad9682c7c63178e2e715ad0eb84f03a8df1fbfba455dfedc5
-  manager: conda
-  name: yaml
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
-  version: 0.2.5
-- category: main
-  dependencies:
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 27c8a78ba0cd18268cfc7b04c5512162
-    sha256: b26b8ea17d1f8146c66c1b7b6acec3c759c2207a2e691e69a2a7cccdd2e1acae
-  manager: conda
-  name: yaml-cpp
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/yaml-cpp-0.7.0-h63175ca_2.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    openssl: '>=3.0.0,<4.0a0'
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: 729fcb13bda4bbd2dbc0c979dd16e677
-    sha256: 46ce0b65faad064a5be2fdc577b5ba8efac135adf2d410b67142fa922cfd6b71
-  manager: conda
-  name: krb5
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/krb5-1.19.3-hc8ab02b_0.tar.bz2
-  version: 1.19.3
-- category: main
-  dependencies:
-    libzlib: '>=1.2.11,<1.3.0a0'
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: f782e1756fd2c9b62931e95363e0205a
-    sha256: 975ecb6ce123df414075dc5018034ccc7dbf12a28f2e86b3ddf4639ff862aa82
-  manager: conda
-  name: libsolv
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libsolv-0.7.22-h7755175_0.tar.bz2
-  version: 0.7.22
-- category: main
-  dependencies:
-    libzlib: '>=1.2.12,<1.3.0a0'
-    openssl: '>=3.0.5,<4.0a0'
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: c2b344e960a173c777bb3ed172c38cd8
-    sha256: 93cc00b7ec3766d4313ff0795997a10745ce68f708811b2213a3655ca2c639b6
-  manager: conda
-  name: libssh2
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libssh2-1.10.0-h9a1e1f7_3.tar.bz2
-  version: 1.10.0
-- category: main
-  dependencies:
-    libiconv: '>=1.17,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 6dcf17bf780618ddb559d992ea3b6961
-    sha256: bba812f5c8c4b47c2b97aa8e66fa43f11a4be37d2d383d766890b30b2f28cdde
-  manager: conda
-  name: libxml2
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.10.3-hc3477c8_0.tar.bz2
-  version: 2.10.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.40.0,<4.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-    tk: '>=8.6.12,<8.7.0a0'
-    tzdata: ''
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-    xz: '>=5.2.6,<6.0a0'
-  hash:
-    md5: 6a74ef0e5662397929214f2fb04c7d19
-    sha256: 7c05da8180e62ebdf6e5af72fd1605df79395b11b0d0653788b828f6e1a6649e
-  manager: conda
-  name: python
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.10.8-h4de0772_0_cpython.conda
-  version: 3.10.8
-- category: main
-  dependencies:
-    reproc: 14.2.3 h8ffe710_0
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: 534e8626893c41ed3b08bbba07396ca3
-    sha256: 94bd2036942929d6a128fe49e8af34d572a9ce06946d5b8b387fab6d42201c26
-  manager: conda
-  name: reproc-cpp
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/reproc-cpp-14.2.3-h0e60522_0.tar.bz2
-  version: 14.2.3
-- category: main
-  dependencies:
-    libzlib: 1.2.12 h8ffe710_2
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: d6f4eeb62da2ad90c31082cc7178776a
-    sha256: a1a4c6997ba96debd345d5d3fdf6109340ce4bf08c25d86e3db33b08e371937d
-  manager: conda
-  name: zlib
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/zlib-1.2.12-h8ffe710_2.tar.bz2
-  version: 1.2.12
-- category: main
-  dependencies:
-    libzlib: '>=1.2.12,<1.3.0a0'
-    ucrt: ''
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-  hash:
-    md5: 13acb3626fcc8c0577249f3a7b6129f4
-    sha256: 109f83494b8bc82d1c41eea92a3cf8303a151674b623df08cc85ca54061cb008
-  manager: conda
-  name: zstd
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h7755175_4.tar.bz2
-  version: 1.5.2
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 5f095bc6454094e96f146491fd03633b
-    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
-  manager: conda
-  name: appdirs
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
-  version: 1.4.4
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 5dfee17f24e2dfd18d7392b48c9351e2
-    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
-  manager: conda
-  name: cachy
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
-  version: 0.3.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: f66309b099374af91369e67e84af397d
-    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
-  manager: conda
-  name: certifi
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
-  version: 2022.9.24
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: c1d5b294fbf9a795dec349a6f4d8be8e
-    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
-  manager: conda
-  name: charset-normalizer
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 3faab06a954c2a04039983f2c4a50d99
-    sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
-  manager: conda
-  name: colorama
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
-  version: 0.4.6
-- category: main
-  dependencies:
-    python: '>=3.6,<4.0'
-  hash:
-    md5: b8477552274c1cfdb533e954c76523f1
-    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
-  manager: conda
-  name: crashtest
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.1
-- category: main
-  dependencies:
-    python: 2.7|>=3.6
-  hash:
-    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
-    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
-  manager: conda
-  name: distlib
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
-  version: 0.3.6
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 88111d95b12d83681d0ecdbbc24eee8e
-    sha256: 6b40f145b1fdf6b45016d29f193a8ca72a9359ea44cc19624901248f7a9b5ba7
-  manager: conda
-  name: docutils
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py310h5588dad_1.tar.bz2
-  version: '0.19'
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
-    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
-  manager: conda
-  name: filelock
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
-  version: 3.8.2
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 6d5e56de2e65da7aa35fd10131226efa
-    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
-  manager: conda
-  name: flit-core
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 34272b248891bddccc64479f9a7fffed
-    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
-  manager: conda
-  name: idna
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
-  version: '3.4'
-- category: main
-  dependencies:
-    python: 2.7|>=3.4
-  hash:
-    md5: 25045ddd7fe83ddf71c181d6212e9913
-    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
-  manager: conda
-  name: invoke
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.7.3
-- category: main
-  dependencies:
-    bzip2: '>=1.0.8,<2.0a0'
-    libxml2: '>=2.9.14,<2.11.0a0'
-    libzlib: '>=1.2.12,<1.3.0a0'
-    lz4-c: '>=1.9.3,<1.10.0a0'
-    lzo: '>=2.10,<3.0a0'
-    openssl: '>=3.0.3,<4.0a0'
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
-    xz: '>=5.2.5,<5.3.0a0'
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: 96f14843ac68b6d49d376b2c76018c1a
-    sha256: 10f045b5c74aed06ef090fb898f67ad0d8fc597fd2ff7563c55089a0b1edf054
-  manager: conda
-  name: libarchive
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libarchive-3.5.2-habf0b7a_3.tar.bz2
-  version: 3.5.2
-- category: main
-  dependencies:
-    krb5: '>=1.19.3,<1.20.0a0'
-    libssh2: '>=1.10.0,<2.0a0'
-    libzlib: '>=1.2.13,<1.3.0a0'
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: d5fc1cba559c9889332ffb2a39001704
-    sha256: 3c2edc12356b57aeb0d9ba11f273196b99862680bc7cec58f8b69f25cf4ab1b1
-  manager: conda
-  name: libcurl
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libcurl-7.86.0-heaf79c2_1.tar.bz2
-  version: 7.86.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: c104d98e09c47519950cffb8dd5b4f10
-    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
-  manager: conda
-  name: lockfile
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
-  version: 0.12.2
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 24e57be449c71b8edc52cc6a48ff846d
-    sha256: 76576c5fd2a6ad1e987b3df4bba55dab05c0f4f35e4f54c6ddbb9559aaf01537
-  manager: conda
-  name: markupsafe
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py310h8d17308_2.tar.bz2
-  version: 2.1.1
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 15cfc917187d7c173647dd65d340259b
-    sha256: 606f9ed8839ba6ba1926ecf1a99cde0e8f02f47cb8d657a390ae13872e019efa
-  manager: conda
-  name: menuinst
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/menuinst-1.4.19-py310h5588dad_1.tar.bz2
-  version: 1.4.19
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 9b6ad26944f19f599800b068e0582227
-    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
-  manager: conda
-  name: more-itertools
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 9.0.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 037a60d74aadd3a2f10e1e9580a42a9b
-    sha256: 9f44cff2cd152db18ef4b8101b6fdb72a8616c80bace71dfff8f248dc0dafe05
-  manager: conda
-  name: msgpack-python
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.4-py310h232114e_1.tar.bz2
-  version: 1.0.4
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: a4eea5bff523f26442405bc5d1f52adb
-    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
-  manager: conda
-  name: pastel
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
-  version: 0.2.1
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
-    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
-  manager: conda
-  name: pkginfo
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
-  version: 1.9.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2fb3f88922e7aec26ba652fcdfe13950
-    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
-  manager: conda
-  name: platformdirs
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
-  version: 2.5.2
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: a15f6e219a4f2b73bccf2210e0f63364
-    sha256: 03951bb41e1e4daa128d2a3fda23643d20174eddf5af6c9badaa317b21ea2583
-  manager: conda
-  name: poetry-core
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/poetry-core-1.0.8-py310h5588dad_1.tar.bz2
-  version: 1.0.8
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 359eeb6536da0e687af562ed265ec263
-    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
-  manager: conda
-  name: ptyprocess
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 3324f50e5d46a04309d8f8f956c17244
-    sha256: 2e74d789ff6846181bd7e32260b9c0d57b91d4fcc0311274fca4279f8a35b048
-  manager: conda
-  name: pycosat
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pycosat-0.6.4-py310h8d17308_1.tar.bz2
-  version: 0.6.4
-- category: main
-  dependencies:
-    python: 2.7.*|>=3.4
-  hash:
-    md5: 076becd9e05608f8dc72757d5f3a91ff
-    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
-  manager: conda
-  name: pycparser
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
-  version: '2.21'
-- category: main
-  dependencies:
-    python: '>=3.3'
-  hash:
-    md5: edf8651c4379d9d1495ad6229622d150
-    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
-  manager: conda
-  name: pylev
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: '>=3.6'
-  hash:
-    md5: e8fbc1b54b25f4b08281467bc13b70cc
-    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
-  manager: conda
-  name: pyparsing
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
-  version: 3.0.9
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
-  hash:
-    md5: e034f495e69b266fc082c92f75398f22
-    sha256: 309c5992598de0424daab9bf20c6eb9909b1eed85bac4608b98a568ac0f41759
-  manager: conda
-  name: pywin32
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/pywin32-303-py310he2412df_0.tar.bz2
-  version: '303'
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 8fa9c1b03d838a262be611ca23003ebd
-    sha256: 7c5ad91c9b454b115d931e8bc5024221cf94b0232871ea89a3c1048f27f7c8a3
-  manager: conda
-  name: pywin32-ctypes
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.0-py310h5588dad_1006.tar.bz2
-  version: 0.2.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: d0daf3eed98dd2bf4337ed08d8011eb8
-    sha256: 7d948a99bf7af50c9823a248267fce75ac555e4f357de166f65a75fab8549f3c
-  manager: conda
-  name: pyyaml
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310h8d17308_5.tar.bz2
-  version: '6.0'
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: b3ef8910b2d18259dbddaee0eb19ef9b
-    sha256: 31968149fcfcd4094936dd8e97ec46491c5bae47a2ccdb68f137d366cf423056
-  manager: conda
-  name: ruamel.yaml.clib
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py310h8d17308_0.tar.bz2
-  version: 0.2.7
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-    yaml: '>=0.2.5,<0.3.0a0'
-  hash:
-    md5: e4537a0116ce275dc510d04d68477060
-    sha256: 997d10b4eaecce80bc95ee5419135548e8e9484221d670d5a9c59f4ad89f5fed
-  manager: conda
-  name: ruamel_yaml
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ruamel_yaml-0.15.80-py310h8d17308_1008.tar.bz2
-  version: 0.15.80
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
-    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
-  manager: conda
-  name: setuptools
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
-  version: 65.5.1
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 437655338696f9d0dfdb0a024e66b255
-    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
-  manager: conda
-  name: shellingham
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
-  version: 1.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: e5f25f8dbc060e9a8d912e432202afc2
-    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
-  manager: conda
-  name: six
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
-  version: 1.16.0
-- category: main
-  dependencies:
-    python: '>=2.7'
-  hash:
-    md5: f832c45a477c78bebd107098db465095
-    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
-  manager: conda
-  name: toml
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
-  version: 0.10.2
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 5844808ffab9ebdb694585b50ba02a96
-    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
-  manager: conda
-  name: tomli
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-  version: 2.0.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 73506d1ab4202481841c68c169b7ef6c
-    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
-  manager: conda
-  name: tomli-w
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 1.0.0
-- category: main
-  dependencies:
-    python: '>=3.5'
-  hash:
-    md5: 92facfec94bc02d6ccf42e7173831a36
-    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
-  manager: conda
-  name: toolz
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
-  version: 0.12.0
-- category: main
-  dependencies:
-    python: '>=3'
-  hash:
-    md5: e6573ac68718f17b9d4f5c8eda3190f2
-    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
-  manager: conda
-  name: typing
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.10.0.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 2d93b130d148d7fc77e583677792fc6a
-    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
-  manager: conda
-  name: typing_extensions
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    python: ''
-  hash:
-    md5: 3563be4c5611a44210d9ba0c16113136
-    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
-  manager: conda
-  name: webencodings
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
-  version: 0.5.1
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: c829cfb8cb826acb9de0ac1a2df0a940
-    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
-  manager: conda
-  name: wheel
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
-  version: 0.38.4
-- category: main
-  dependencies:
-    __win: ''
-    python: '>=3.6'
-  hash:
-    md5: 30878ecc4bd36e8deeea1e3c151b2e0b
-    sha256: a11ae693a0645bf6c7b8a47bac030be9c0967d0b1924537b9ff7458e832c0511
-  manager: conda
-  name: win_inet_pton
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2
-  version: 1.1.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-  hash:
-    md5: 09b5b885341697137879a4f039a9e5a1
-    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
-  manager: conda
-  name: zipp
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
-  version: 3.11.0
-- category: main
-  dependencies:
-    pycparser: ''
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: ec6be66017eb91c9077abe15dcb19e75
-    sha256: bccfec5fbcaa255d0aa471933d1aaaf76f4a4070783e4e2b45b41c73df101af7
-  manager: conda
-  name: cffi
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_2.tar.bz2
-  version: 1.15.1
-- category: main
-  dependencies:
-    __win: ''
-    colorama: ''
-    python: '>=3.8'
-  hash:
-    md5: 6b58680207b526c42dcff68b543803dd
-    sha256: 84e80a33e9a8e5398d3e97209366b57f635462a5b894f8076ec8c95e56672c44
-  manager: conda
-  name: click
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
-- category: main
-  dependencies:
-    crashtest: '>=0.3.0,<0.4.0'
-    pastel: '>=0.2.0,<0.3.0'
-    pylev: '>=1.3,<2.0'
-    python: ''
-  hash:
-    md5: 159273f717a11e53b2656f8b6521a5e2
-    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
-  manager: conda
-  name: clikit
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
-  version: 0.6.2
-- category: main
-  dependencies:
-    python: ''
-    six: '>=1.9'
-    webencodings: ''
-  hash:
-    md5: b2355343d6315c892543200231d7154a
-    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
-  manager: conda
-  name: html5lib
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
-  version: '1.1'
-- category: main
-  dependencies:
-    python: '>=3.8'
-    zipp: '>=0.5'
-  hash:
-    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
-    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
-  manager: conda
-  name: importlib-metadata
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    more-itertools: ''
-    python: '>=3.7'
-  hash:
-    md5: 31e4a1506968d017229bdb64695013a1
-    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
-  manager: conda
-  name: jaraco.classes
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
-  version: 3.2.3
-- category: main
-  dependencies:
-    markupsafe: '>=2.0'
-    python: '>=3.7'
-  hash:
-    md5: c8490ed5c70966d232fdd389d0dbed37
-    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
-  manager: conda
-  name: jinja2
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
-  version: 3.1.2
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libarchive: '>=3.5.2,<3.6.0a0'
-    libcurl: '>=7.86.0,<8.0a0'
-    libsolv: '>=0.7.22,<0.8.0a0'
-    openssl: '>=3.0.7,<4.0a0'
-    reproc-cpp: '>=14.2,<15.0a0'
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: 672850850275c7f10001328b65ae297b
-    sha256: 379851f5d60f74e9f89aa6b571c3568e8d1ba860a9eb27ead9d0b7b776de4645
-  manager: conda
-  name: libmamba
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libmamba-1.1.0-hd18bbca_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    pyparsing: '>=2.0.2,!=3.0.5'
-    python: '>=3.6'
-  hash:
-    md5: 71f1ab2de48613876becddd496371c85
-    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
-  manager: conda
-  name: packaging
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
-  version: '21.3'
-- category: main
-  dependencies:
-    ptyprocess: '>=0.5'
-    python: ''
-  hash:
-    md5: 5909e7b978141dd80d28dbf9de627827
-    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
-  manager: conda
-  name: pexpect
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
-  version: 4.8.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    setuptools: ''
-    wheel: ''
-  hash:
-    md5: da66f2851b9836d3a7c5190082a45f7d
-    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
-  manager: conda
-  name: pip
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
-  version: 22.3.1
-- category: main
-  dependencies:
-    __win: ''
-    python: '>=3.8'
-    win_inet_pton: ''
-  hash:
-    md5: 56cd9fe388baac0e90c7149cfac95b60
-    sha256: b3a612bc887f3dd0fb7c4199ad8e342bd148cf69a9b74fd9468a18cf2bef07b7
-  manager: conda
-  name: pysocks
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
-  version: 1.7.1
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ruamel.yaml.clib: '>=0.1.2'
-    setuptools: ''
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 266f81ef89f0cfef72a628e236147f7f
-    sha256: 02480785e2b4fe91b6678d32f3aebbc23749622563f017feac0a83bfed0f3d8f
-  manager: conda
-  name: ruamel.yaml
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.21-py310h8d17308_2.tar.bz2
-  version: 0.17.21
-- category: main
-  dependencies:
-    python: '>=3.6'
-    typing: '>=3.6,<4.0'
-  hash:
-    md5: 471bf9e605820b59988e830382b8d654
-    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
-  manager: conda
-  name: tomlkit
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
-  version: 0.11.6
-- category: main
-  dependencies:
-    colorama: ''
-    python: '>=2.7'
-  hash:
-    md5: 6642233f341e1900d0c8e6eddb979c14
-    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
-  manager: conda
-  name: tqdm
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
-  version: 4.64.0
-- category: main
-  dependencies:
-    typing_extensions: 4.4.0 pyha770c72_0
-  hash:
-    md5: be969210b61b897775a0de63cd9e9026
-    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
-  manager: conda
-  name: typing-extensions
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
-  version: 4.4.0
-- category: main
-  dependencies:
-    distlib: '>=0.3.6,<1'
-    filelock: '>=3.4.1,<4'
-    platformdirs: '>=2.4,<3'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: 6a22296594d9b77bcf1f962bed2f6a61
-    sha256: c07d8ac0c29e28d47c08d42834ed5d8a804fbc01e2886d9603be430c3bfd1702
-  manager: conda
-  name: virtualenv
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.17.0-py310h5588dad_0.conda
-  version: 20.17.0
-- category: main
-  dependencies:
-    cffi: '>=1.0.0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 6cb010e0fa21d7b606a13038a89ccbc2
-    sha256: 2631b26d291196d76694bf7d71ea77ba2abcfc46278c3a54730a2d5683ca6c2b
-  manager: conda
-  name: brotlipy
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310h8d17308_1005.tar.bz2
-  version: 0.7.0
-- category: main
-  dependencies:
-    clikit: '>=0.6.0,<0.7.0'
-    python: '>=3.6'
-  hash:
-    md5: 4c82b11a3d06031bd58e7d869f53d965
-    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
-  manager: conda
-  name: cleo
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
-  version: 0.8.1
-- category: main
-  dependencies:
-    click: ''
-    python: '>=3.6'
-  hash:
-    md5: 72a46ffc25701c173932fd55cf0965d3
-    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
-  manager: conda
-  name: click-default-group
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.2
-- category: main
-  dependencies:
-    cffi: '>=1.12'
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 0e8b49bc425a99afa3c8d48776c6e6ed
-    sha256: 22930c11e3c44785cfc83f739bea5250bee34a078ee90f8840378a100d624aa4
-  manager: conda
-  name: cryptography
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-38.0.4-py310h6e82f81_0.conda
-  version: 38.0.4
-- category: main
-  dependencies:
-    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
-  hash:
-    md5: 3dc2248927de739b4d2e2da9a9972bfe
-    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
-  manager: conda
-  name: importlib_metadata
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
-  version: 5.1.0
-- category: main
-  dependencies:
-    fmt: '>=9.1.0,<10.0a0'
-    libmamba: 1.1.0 hd18bbca_2
-    openssl: '>=3.0.7,<4.0a0'
-    pybind11-abi: '4'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-    yaml-cpp: '>=0.7.0,<0.8.0a0'
-  hash:
-    md5: d9976c2eb8ad85ed4a160da739242fba
-    sha256: 28082342d92ee056be62c11f2a0b31a6a1daf9ef06cef2d363fca5f68fadb21f
-  manager: conda
-  name: libmambapy
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.1.0-py310h3fe4c2e_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    typing-extensions: '>=4.1.0'
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-  hash:
-    md5: 675afeba3c75ece50ef5b1f22350a710
-    sha256: 393dc63fa4c61153e1685c05a2f9bd91562e66f131858d7e6d1a49c4538b6a00
-  manager: conda
-  name: pydantic
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-1.10.2-py310h8d17308_1.tar.bz2
-  version: 1.10.2
-- category: main
-  dependencies:
-    cffi: '>=1.11'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    ucrt: '>=10.0.20348.0'
-    vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
-    zstd: '>=1.5.2,<1.6.0a0'
-  hash:
-    md5: 9ef29771ac801a8a1e132f2f67ccf5cc
-    sha256: 189ed4c35ef53c01c909aa9afa8ef654f9a9cee8725aa05f38fa138d57702cfa
-  manager: conda
-  name: zstandard
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py310h0009e47_1.conda
-  version: 0.19.0
-- category: main
-  dependencies:
-    python: '>=3.7'
-    zstandard: '>=0.15'
-  hash:
-    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
-    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
-  manager: conda
-  name: conda-package-streaming
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
-  version: 0.7.0
-- category: main
-  dependencies:
-    importlib_metadata: '>=4.11.4'
-    jaraco.classes: ''
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    pywin32-ctypes: ''
-  hash:
-    md5: 9adbff9beec7edbee5e02836f7c0ad43
-    sha256: c0cee60a41b09bf39d648b1af75b0ec9b57252bd7be1812f786bb68168f58f23
-  manager: conda
-  name: keyring
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/keyring-23.11.0-py310h5588dad_0.tar.bz2
-  version: 23.11.0
-- category: main
-  dependencies:
-    cryptography: '>=38.0.0,<39'
-    python: '>=3.6'
-  hash:
-    md5: fbfa0a180d48c800f922a10a114a8632
-    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
-  manager: conda
-  name: pyopenssl
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
-  version: 22.1.0
-- category: main
-  dependencies:
-    conda-package-streaming: '>=0.7.0'
-    python: '>=3.7'
-  hash:
-    md5: 44800e9bd13143292097c65e57323038
-    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
-  manager: conda
-  name: conda-package-handling
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
-  version: 2.0.2
-- category: main
-  dependencies:
-    brotlipy: '>=0.6.0'
-    certifi: ''
-    cryptography: '>=1.3.4'
-    idna: '>=2.0.0'
-    pyopenssl: '>=0.14'
-    pysocks: '>=1.5.6,<2.0,!=1.5.7'
-    python: <4.0
-  hash:
-    md5: 3078ef2359efd6ecadbc7e085c5e0592
-    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
-  manager: conda
-  name: urllib3
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
-  version: 1.26.13
-- category: main
-  dependencies:
-    certifi: '>=2017.4.17'
-    charset-normalizer: '>=2,<3'
-    idna: '>=2.5,<4'
-    python: '>=3.7,<4.0'
-    urllib3: '>=1.21.1,<1.27'
-  hash:
-    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
-    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
-  manager: conda
-  name: requests
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
-  version: 2.28.1
-- category: main
-  dependencies:
-    filelock: '>=3.8.0'
-    msgpack-python: '>=0.5.2'
-    python: '>=3.6'
-    requests: ''
-  hash:
-    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
-    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
-  manager: conda
-  name: cachecontrol
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
-  version: 0.12.12
-- category: main
-  dependencies:
-    conda-package-handling: '>=1.3.0'
-    menuinst: '>=1.4.11,<2'
-    pycosat: '>=0.6.3'
-    pyopenssl: '>=16.2.0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.20.1,<3'
-    ruamel_yaml: '>=0.11.14,<0.17'
-    setuptools: '>=31.0.1'
-    toolz: '>=0.8.1'
-  hash:
-    md5: c69ac3dd1ebd4a6898f2b08f2639c1cc
-    sha256: bd7abec2f08e6e42e7dfe6446d8520401db98d1a1bcdc95b3f388dd6738e2885
-  manager: conda
-  name: conda
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/conda-22.9.0-py310h5588dad_2.tar.bz2
-  version: 22.9.0
-- category: main
-  dependencies:
-    appdirs: ''
-    click: '>=5.1'
-    filelock: ''
-    python: '>=3.7'
-    requests: '>=2'
-  hash:
-    md5: c99ae3abf501990769047b4b40a98f17
-    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
-  manager: conda
-  name: ensureconda
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
-  version: 1.4.3
-- category: main
-  dependencies:
-    docutils: ''
-    flit-core: 3.8.0 pyhd8ed1ab_0
-    pip: ''
-    python: '>=3.6'
-    requests: ''
-    tomli-w: ''
-  hash:
-    md5: d37c34176396c5402cf80c32e67731b7
-    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
-  manager: conda
-  name: flit
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
-  version: 3.8.0
-- category: main
-  dependencies:
-    python: ''
-    requests: '>=2.0.1,<=3.0.0'
-  hash:
-    md5: 402668adee8fcba9a9c265cdc2a88f5a
-    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
-  manager: conda
-  name: requests-toolbelt
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
-  version: 0.9.1
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9'
-    cachy: '>=0.3.0'
-    click: '>=8.0'
-    click-default-group: ''
-    clikit: '>=0.6.2'
-    crashtest: '>=0.3.0'
-    ensureconda: '>=1.3'
-    filelock: '>=3.8.0'
-    html5lib: '>=1.0'
-    importlib-metadata: '>=1.7.0'
-    jinja2: ''
-    keyring: '>=21.2.0'
-    packaging: '>=20.4'
-    pkginfo: '>=1.4'
-    pydantic: '>=1.8.1'
-    python: '>=3.6'
-    pyyaml: '>=5.1'
-    requests: '>=2.18'
-    ruamel.yaml: ''
-    tomli: ''
-    tomlkit: '>=0.7.0'
-    toolz: <1.0.0,>=0.12.0
-    typing-extensions: ''
-    virtualenv: '>=20.0.26'
-  hash:
-    md5: 7b1dde4760c5c554523fead6c2771af2
-    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
-  manager: conda
-  name: conda-lock
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
-  version: 1.2.1
-- category: main
-  dependencies:
-    conda: '>=4.8,<23.4'
-    libmambapy: 1.1.0 py310h3fe4c2e_2
-    openssl: '>=3.0.7,<4.0a0'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-  hash:
-    md5: a61405ee533eff515ef5848ea77efac5
-    sha256: d14f3a2de4510ae24ac61084a83c325abf15b98a91e6e43e786579b6a1a82ef0
-  manager: conda
-  name: mamba
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/mamba-1.1.0-py310hd9d798f_2.conda
-  version: 1.1.0
-- category: main
-  dependencies:
-    cachecontrol: '>=0.12.9,<0.13.0'
-    cachy: '>=0.3.0,<0.4.0'
-    cleo: '>=0.8.1,<0.9.0'
-    clikit: '>=0.6.2,<0.7.0'
-    crashtest: '>=0.3.0,<0.4.0'
-    html5lib: '>=1.0,<2.0'
-    keyring: '>=21.2.0'
-    lockfile: '>=0.9'
-    packaging: '>=20.4,<21.0'
-    pexpect: '>=4.7.0,<5.0.0'
-    pkginfo: '>=1.4,<2.0'
-    poetry-core: '>=1.0.7,<1.1.0'
-    ptyprocess: '>=0.5'
-    python: '>=3.10,<3.11.0a0'
-    python_abi: 3.10.* *_cp310
-    requests: '>=2.18,<3.0'
-    requests-toolbelt: '>=0.9.1,<0.10.0'
-    shellingham: '>=1.1,<2.0'
-    tomlkit: '>=0.7.0,<1.0.0'
-    virtualenv: '>=20.0.26,<21.0.0'
-  hash:
-    md5: 0e9febdede429556c039b685d779fdc1
-    sha256: 31d83812fd55331e82ef4655fc72ddfe000fa9a03de5fb374a54a5c4a560d7f7
-  manager: conda
-  name: poetry
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/poetry-1.1.14-py310h5588dad_0.tar.bz2
-  version: 1.1.14
-version: 1
+# This lock file was generated by conda-lock (https://github.com/conda-incubator/conda-lock). DO NOT EDIT!
+#
+# A "lock file" contains a concrete list of package versions (with checksums) to be installed. Unlike
+# e.g. `conda env create`, the resulting environment will not change as new package versions become
+# available, unless you explicitly update the lock file.
+#
+# Install this environment as "YOURENV" with:
+#     conda-lock install -n YOURENV --file conda-lock.yml
+# To update a single package to the latest version compatible with the version constraints in the source:
+#     conda-lock lock --lockfile conda-lock.yml --update PACKAGE
+# To re-solve the entire environment, e.g. after changing a version constraint in the source file:
+#     conda-lock -f pyproject.toml -f C:\Users\michael\Documents\LensKit\lkbuild\pyproject.toml --lockfile conda-lock.yml
+metadata:
+  channels:
+  - url: conda-forge
+    used_env_vars: []
+  content_hash:
+    linux-64: 66b8d24fe36a198717ddca7d1fc328fc453a37f8878c80fb73db22b4baa3f8bc
+    osx-64: f5833e90d66407c42f4f0830ed8287aca17995fb4ca49e1fa2825e96ddf2692a
+    win-64: def7cf82c8e903a65f0ad53079339ea52c054c43f2164fabfa828188aa5e623a
+  platforms:
+  - linux-64
+  - osx-64
+  - win-64
+  sources:
+  - pyproject.toml
+  - C:\Users\michael\Documents\LensKit\lkbuild\pyproject.toml
+package:
+- category: main
+  dependencies: {}
+  hash:
+    md5: d7c89558ba9fa0495403155b64376d81
+    sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
+  manager: conda
+  name: _libgcc_mutex
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+  version: '0.1'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 41e4e87062433e283696cf384f952ef6
+    sha256: 058355034667e77d15389700f6b2364cc74efce0af63a418eacc1ce252458942
+  manager: conda
+  name: ca-certificates
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.9.24-ha878542_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies: {}
+  hash:
+    md5: 737be0d34c22d24432049ab7a3214de4
+    sha256: 3e7f203e33ea497b6e468279cc5fdef7d556473c25e7466b35fd672940392469
+  manager: conda
+  name: ld_impl_linux-64
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.39-hcc3a1bd_1.conda
+  version: '2.39'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 1030b1f38c129f2634eae026f704fe60
+    sha256: 0289e6a7b9a5249161a3967909e12dcfb4ab4475cdede984635d3fb65c606f08
+  manager: conda
+  name: libstdcxx-ng
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2
+  version: 12.2.0
+- category: main
+  dependencies: {}
+  hash:
+    md5: 878f923dd6acc8aeb47a75da6c4098be
+    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
+  manager: conda
+  name: pybind11-abi
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
+  version: '4'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 4eb33d14d794b0f4be116443ffed3853
+    sha256: bcb15db27eb6fbc0fe15d23aa60dcfa58ef451d92771441068d4a911aea7bb9f
+  manager: conda
+  name: python_abi
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-3_cp310.conda
+  version: '3.10'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
+    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
+  manager: conda
+  name: tzdata
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
+  version: 2022g
+- category: main
+  dependencies:
+    _libgcc_mutex: 0.1 conda_forge
+  hash:
+    md5: cedcee7c064c01c403f962c9e8d3c373
+    sha256: 81a76d20cfdee9fe0728b93ef057ba93494fd1450d42bc3717af4e468235661e
+  manager: conda
+  name: libgomp
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2
+  version: 12.2.0
+- category: main
+  dependencies:
+    _libgcc_mutex: 0.1 conda_forge
+    libgomp: '>=7.5.0'
+  hash:
+    md5: 73aaf86a425cc6e73fcf236a5a46396d
+    sha256: fbe2c5e56a653bebb982eda4876a9178aedfc2b545f25d0ce9c4c0b508253d22
+  manager: conda
+  name: _openmp_mutex
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+  version: '4.5'
+- category: main
+  dependencies:
+    _libgcc_mutex: 0.1 conda_forge
+    _openmp_mutex: '>=4.5'
+  hash:
+    md5: e4c94f80aef025c17ab0828cd85ef535
+    sha256: f3899c26824cee023f1e360bd0859b0e149e2b3e8b1668bc6dd04bfc70dcd659
+  manager: conda
+  name: libgcc-ng
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2
+  version: 12.2.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.3.0'
+  hash:
+    md5: a1fd65c7ccbf10880423d82bca54eb54
+    sha256: cb521319804640ff2ad6a9f118d972ed76d86bea44e5626c09a13d38f562e1fa
+  manager: conda
+  name: bzip2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+  hash:
+    md5: f26ef8098fab1f719c91eb760d63381a
+    sha256: ee735e60d2cf68e5635df17847e97b505a752985d10581d2438203e7c0f44c15
+  manager: conda
+  name: c-ares
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2
+  version: 1.18.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+  hash:
+    md5: c4fbad8d4bddeb3c085f18cbf97fbfad
+    sha256: b44db0b92ae926b3fbbcd57c179fceb64fa11a9f9d09082e03be58b74dcad832
+  manager: conda
+  name: expat
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-h27087fc_0.tar.bz2
+  version: 2.5.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+  hash:
+    md5: b57864c85261a0fbc7132d2cc17478c7
+    sha256: bd48506faffa86e07f7b40d54f2d7e13b0fc956eda9760236750f5ea20db7129
+  manager: conda
+  name: fmt
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/fmt-9.1.0-h924138e_0.tar.bz2
+  version: 9.1.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+  hash:
+    md5: 14947d8770185e5153fdd04d4673ed37
+    sha256: 4fcfedc44e4c9a053f0416f9fc6ab6ed50644fca3a761126dbd00d09db1f546a
+  manager: conda
+  name: gettext
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2
+  version: 0.21.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=10.3.0'
+    libstdcxx-ng: '>=10.3.0'
+  hash:
+    md5: 87473a15119779e021c314249d4b4aed
+    sha256: 1d7950f3be4637ab915d886304e57731d39a41ab705ffc95c4681655c459374a
+  manager: conda
+  name: icu
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/icu-70.1-h27087fc_0.tar.bz2
+  version: '70.1'
+- category: main
+  dependencies:
+    libgcc-ng: '>=10.3.0'
+  hash:
+    md5: 30186d27e2c9fa62b45fb1476b7200e3
+    sha256: 150c05a6e538610ca7c43beb3a40d65c90537497a4f6a5f4d15ec0451b6f5ebb
+  manager: conda
+  name: keyutils
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
+  version: 1.6.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=7.5.0'
+  hash:
+    md5: 6f8720dff19e17ce5d48cfe7f3d2f0a3
+    sha256: 8c9635aa0ea28922877dc96358f9547f6a55fc7e2eb75a556b05f1725496baf9
+  manager: conda
+  name: libev
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2
+  version: '4.33'
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+  hash:
+    md5: d645c6d2ac96843a2bfaccd2d62b3ac3
+    sha256: ab6e9856c21709b7b517e940ae7028ae0737546122f83c2aa5d692860c3b149e
+  manager: conda
+  name: libffi
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+  version: 3.4.2
+- category: main
+  dependencies:
+    libgcc-ng: '>=10.3.0'
+  hash:
+    md5: b62b52da46c39ee2bc3c162ac7f1804d
+    sha256: 6a81ebac9f1aacdf2b4f945c87ad62b972f0f69c8e0981d68e111739e6720fd7
+  manager: conda
+  name: libiconv
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2
+  version: '1.17'
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+  hash:
+    md5: 39b1328babf85c7c3a61636d9cd50206
+    sha256: 32f4fb94d99946b0dabfbbfd442b25852baf909637f2eed1ffe3baea15d02aad
+  manager: conda
+  name: libnsl
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2
+  version: 2.0.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.3.0'
+  hash:
+    md5: 772d69f030955d9646d3d0eaf21d859d
+    sha256: 54f118845498353c936826f8da79b5377d23032bcac8c4a02de2019e26c3f6b3
+  manager: conda
+  name: libuuid
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2
+  version: 2.32.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+  hash:
+    md5: f3f9de449d32ca9b9c66a22863c96f41
+    sha256: 22f3663bcf294d349327e60e464a51cd59664a71b8ed70c28a9f512d10bc77dd
+  manager: conda
+  name: libzlib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2
+  version: 1.2.13
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.3.0'
+    libstdcxx-ng: '>=9.3.0'
+  hash:
+    md5: fbe97e8fa6f275d7c76a09e795adc3e6
+    sha256: 56313fe4e602319682d4ea05c0ed3c5c45fc79884a5896f2cb7436b15d6987f9
+  manager: conda
+  name: lz4-c
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.3-h9c3ff4c_1.tar.bz2
+  version: 1.9.3
+- category: main
+  dependencies:
+    libgcc-ng: '>=7.5.0'
+  hash:
+    md5: bb14fcb13341b81d5eb386423b9d2bac
+    sha256: 25d16e6aaa3d0b450e61d0c4fadd7c9fd17f16e2fef09b34507209342d63c9f6
+  manager: conda
+  name: lzo
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/lzo-2.10-h516909a_1000.tar.bz2
+  version: '2.10'
+- category: main
+  dependencies:
+    libgcc-ng: '>=10.3.0'
+  hash:
+    md5: 4acfc691e64342b9dae57cf2adc63238
+    sha256: b801e8cf4b2c9a30bce5616746c6c2a4e36427f045b46d9fc08a4ed40a9f7065
+  manager: conda
+  name: ncurses
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2
+  version: '6.3'
+- category: main
+  dependencies:
+    ca-certificates: ''
+    libgcc-ng: '>=12'
+  hash:
+    md5: 7adaac6ff98219bcb99b45e408b80f4e
+    sha256: d9143f6d10e7edaa8cbb03e510d60c54463f4538c01f30b0abff51def582d94e
+  manager: conda
+  name: openssl
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.0.7-h0b41bf4_1.conda
+  version: 3.0.7
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.3.0'
+    libstdcxx-ng: '>=9.3.0'
+  hash:
+    md5: c05d1820a6d34ff07aaaab7a9b7eddaa
+    sha256: 8f35c244b1631a4f31fb1d66ab6e1d9bfac0ca9b679deced1112c7225b3ad138
+  manager: conda
+  name: pcre
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/pcre-8.45-h9c3ff4c_0.tar.bz2
+  version: '8.45'
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+  hash:
+    md5: 1e16d4142b016b6a5ebdeb3d6d33aaf4
+    sha256: f46a85d6df26dce9ec2c63c90662dd02bdc446cece65afd37b1ee9e31525a206
+  manager: conda
+  name: reproc
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/reproc-14.2.3-h7f98852_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+  hash:
+    md5: 2161070d867d1b1204ea749c8eec4ef0
+    sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
+  manager: conda
+  name: xz
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+  version: 5.2.6
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+  hash:
+    md5: 4cb3ad778ec2d5a7acbdf254eb1c42ae
+    sha256: a4e34c710eeb26945bdbdaba82d3d74f60a78f54a874ec10d373811a5d217535
+  manager: conda
+  name: yaml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
+  version: 0.2.5
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+  hash:
+    md5: 0449d47d8457feaa3720d4779616dde2
+    sha256: fcdffce895f84a49221720b811a6bb14ae79f7ac14f7930f3768bbb7b2470444
+  manager: conda
+  name: yaml-cpp
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/yaml-cpp-0.7.0-h27087fc_2.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=7.5.0'
+    ncurses: '>=6.2,<7.0.0a0'
+  hash:
+    md5: 4d331e44109e3f0e19b4cb8f9b82f3e1
+    sha256: a57d37c236d8f7c886e01656f4949d9dcca131d2a0728609c6f7fa338b65f1cf
+  manager: conda
+  name: libedit
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2
+  version: 3.1.20191231
+- category: main
+  dependencies:
+    c-ares: '>=1.18.1,<2.0a0'
+    libev: '>=4.33,<4.34.0a0'
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    openssl: '>=3.0.5,<4.0a0'
+  hash:
+    md5: 2b7dbfa6988a41f9d23ba6d4f0e1d74e
+    sha256: 66988eb178d6ffbad3de5e391dad49aaa298e1309ac197ab40996eac740fbfff
+  manager: conda
+  name: libnghttp2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.47.0-hff17c54_1.tar.bz2
+  version: 1.47.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=10.3.0'
+    libstdcxx-ng: '>=10.3.0'
+    libzlib: '>=1.2.11,<1.3.0a0'
+  hash:
+    md5: 461963bb499e58bae159a898600f8792
+    sha256: 2c03438609126505d7167eb8f9eec84a6de5e5f098495de052550cb371b18407
+  manager: conda
+  name: libsolv
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsolv-0.7.22-h6239696_0.tar.bz2
+  version: 0.7.22
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libzlib: '>=1.2.13,<1.3.0a0'
+  hash:
+    md5: 2e5f9a37d487e1019fd4d8113adb2f9f
+    sha256: 6008a0b914bd1a3510a3dba38eada93aa0349ebca3a21e5fa276833c8205bf49
+  manager: conda
+  name: libsqlite
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.40.0-h753d276_0.tar.bz2
+  version: 3.40.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    openssl: '>=3.0.5,<4.0a0'
+  hash:
+    md5: d85acad4b47dff4e3def14a769a97906
+    sha256: 9a9a01f35d2d50326eb8ca7c0a92d0c45b2d0f77d9ea117680c70094ff480c0c
+  manager: conda
+  name: libssh2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-hf14f497_3.tar.bz2
+  version: 1.10.0
+- category: main
+  dependencies:
+    icu: '>=70.1,<71.0a0'
+    libgcc-ng: '>=12'
+    libiconv: '>=1.17,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    xz: '>=5.2.6,<6.0a0'
+  hash:
+    md5: 3b933ea47ef8f330c4c068af25fcd6a8
+    sha256: b30713fb4477ff4f722280d956593e7e7a2cb705b7444dcc278de447432b43b1
+  manager: conda
+  name: libxml2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.10.3-h7463322_0.tar.bz2
+  version: 2.10.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libgcc-ng: '>=12'
+    libzlib: '>=1.2.12,<1.3.0a0'
+  hash:
+    md5: 69e2c796349cd9b273890bee0febfe1b
+    sha256: 7a29ec847556eed4faa1646010baae371ced69059a4ade43851367a076d6108a
+  manager: conda
+  name: pcre2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2
+  version: '10.40'
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    ncurses: '>=6.3,<7.0a0'
+  hash:
+    md5: db2ebbe2943aae81ed051a6a9af8e0fa
+    sha256: f5f383193bdbe01c41cb0d6f99fec68e820875e842e6e8b392dbe1a9b6c43ed8
+  manager: conda
+  name: readline
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2
+  version: 8.1.2
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+    libstdcxx-ng: '>=9.4.0'
+    reproc: 14.2.3 h7f98852_0
+  hash:
+    md5: 1fc15d3b393b62192d3eeade92b61610
+    sha256: 03d7dcc19ac0a16f32b77368c22e24cf370d2ea5681e28c5687d9e4bd25ab2db
+  manager: conda
+  name: reproc-cpp
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/reproc-cpp-14.2.3-h9c3ff4c_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies:
+    libgcc-ng: '>=9.4.0'
+    libzlib: '>=1.2.11,<1.3.0a0'
+  hash:
+    md5: 5b8c42eb62e9fc961af70bdd6a26e168
+    sha256: 032fd769aad9d4cad40ba261ab222675acb7ec951a8832455fce18ef33fa8df0
+  manager: conda
+  name: tk
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2
+  version: 8.6.12
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libzlib: 1.2.12 h166bdaf_2
+  hash:
+    md5: 4533821485cde83ab12ff3d8bda83768
+    sha256: 084342e7f0d2feeca6eb0f194f0a82ac75217730745e6c9033016ed015283bcc
+  manager: conda
+  name: zlib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/zlib-1.2.12-h166bdaf_2.tar.bz2
+  version: 1.2.12
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+    libzlib: '>=1.2.12,<1.3.0a0'
+  hash:
+    md5: adcf0be7897e73e312bd24353b613f74
+    sha256: c42d9ec413edd7e984b6cac676997105d0f106556a0f045961153b049b95b87c
+  manager: conda
+  name: zstd
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h6239696_4.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
+    keyutils: '>=1.6.1,<2.0a0'
+    libedit: '>=3.1.20191231,<4.0a0'
+    libgcc-ng: '>=10.3.0'
+    libstdcxx-ng: '>=10.3.0'
+    openssl: '>=3.0.0,<4.0a0'
+  hash:
+    md5: d25e05e7ee0e302b52d24491db4891eb
+    sha256: 9faad78e078a3e671f3572a01163acc1b2a47539559c746ea3ffd17c754ea578
+  manager: conda
+  name: krb5
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.3-h08a2579_0.tar.bz2
+  version: 1.19.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libgcc-ng: '>=12'
+    libxml2: '>=2.9.14,<2.11.0a0'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    lz4-c: '>=1.9.3,<1.10.0a0'
+    lzo: '>=2.10,<3.0a0'
+    openssl: '>=3.0.3,<4.0a0'
+    xz: '>=5.2.5,<5.3.0a0'
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: c0c3973a9f2df3e1a408e3205d86a88d
+    sha256: b67ff7262422ef04bfa1056c5ef10eba4d64773f40bb34314e0d492f58e726e7
+  manager: conda
+  name: libarchive
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarchive-3.5.2-hada088e_3.tar.bz2
+  version: 3.5.2
+- category: main
+  dependencies:
+    gettext: '>=0.21.1,<1.0a0'
+    libffi: '>=3.4,<4.0a0'
+    libgcc-ng: '>=12'
+    libiconv: '>=1.17,<2.0a0'
+    libstdcxx-ng: '>=12'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    pcre2: '>=10.40,<10.41.0a0'
+  hash:
+    md5: ed5349aa96776e00b34eccecf4a948fe
+    sha256: 3cbad3d63cff2dd9ac1dc9cce54fd3d657f3aff53df41bfe5bae9d760562a5af
+  manager: conda
+  name: libglib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.74.1-h606061b_1.tar.bz2
+  version: 2.74.1
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    ld_impl_linux-64: '>=2.36.1'
+    libffi: '>=3.4,<4.0a0'
+    libgcc-ng: '>=12'
+    libnsl: '>=2.0.0,<2.1.0a0'
+    libsqlite: '>=3.40.0,<4.0a0'
+    libuuid: '>=2.32.1,<3.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    ncurses: '>=6.3,<7.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+    readline: '>=8.1.2,<9.0a0'
+    tk: '>=8.6.12,<8.7.0a0'
+    tzdata: ''
+    xz: '>=5.2.6,<6.0a0'
+  hash:
+    md5: be2a6d78752c2ab85f360ce37d2c64e2
+    sha256: 79cc250d8f85da29c7a06116a51db4c9efbd46f62f21daef6cf10e8bccdc0523
+  manager: conda
+  name: python
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.8-h4a9ceb5_0_cpython.conda
+  version: 3.10.8
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    ncurses: '>=6.3,<7.0a0'
+    readline: '>=8.1.2,<9.0a0'
+    zlib: '>=1.2.12,<1.3.0a0'
+  hash:
+    md5: 2cf5cb4cd116a78e639977eb61ad9987
+    sha256: 5878c9d99a731991eea6e9dea4baf09248a3caf4fa032acb41f2283965719138
+  manager: conda
+  name: sqlite
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/sqlite-3.39.2-h4ff8645_0.tar.bz2
+  version: 3.39.2
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 5dfee17f24e2dfd18d7392b48c9351e2
+    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
+  manager: conda
+  name: cachy
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
+  version: 0.3.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: f66309b099374af91369e67e84af397d
+    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
+  manager: conda
+  name: certifi
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c1d5b294fbf9a795dec349a6f4d8be8e
+    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
+  manager: conda
+  name: charset-normalizer
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    __unix: ''
+    python: '>=3.8'
+  hash:
+    md5: 20e4087407c7cb04a40817114b333dbf
+    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+  manager: conda
+  name: click
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  version: 8.1.3
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c267da48ce208905d7d976d49dfd9433
+    sha256: fcab1a16af5daf3a1ea9b0a7ed15615f0d5fff05ff4925ed570988868bb29e38
+  manager: conda
+  name: colorama
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.5
+- category: main
+  dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: b8477552274c1cfdb533e954c76523f1
+    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.1
+- category: main
+  dependencies:
+    expat: '>=2.4.2,<3.0a0'
+    libgcc-ng: '>=9.4.0'
+    libglib: '>=2.70.2,<3.0a0'
+  hash:
+    md5: ecfff944ba3960ecb334b9a2663d708d
+    sha256: 8f5f995699a2d9dbdd62c61385bfeeb57c82a681a7c8c5313c395aa0ccab68a5
+  manager: conda
+  name: dbus
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2
+  version: 1.13.6
+- category: main
+  dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
+    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
+  manager: conda
+  name: distlib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.6
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 21b8fa2179290505e607f5ccd65b01b0
+    sha256: f3a564449daedafe5931ab4efe7bc4f240182f2b760e7877f15b2898b7f1c988
+  manager: conda
+  name: docutils
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py310hff52083_1.tar.bz2
+  version: '0.19'
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
+    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
+  manager: conda
+  name: filelock
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
+  version: 3.8.2
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 6d5e56de2e65da7aa35fd10131226efa
+    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
+  manager: conda
+  name: flit-core
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 34272b248891bddccc64479f9a7fffed
+    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
+  manager: conda
+  name: idna
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
+  version: '3.4'
+- category: main
+  dependencies:
+    python: 2.7|>=3.4
+  hash:
+    md5: 25045ddd7fe83ddf71c181d6212e9913
+    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
+  manager: conda
+  name: invoke
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.7.3
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 9800ad1699b42612478755a2d26c722d
+    sha256: 16639759b811866d63315fe1391f6fb45f5478b823972f4d3d9f0392b7dd80b8
+  manager: conda
+  name: jeepney
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.8.0
+- category: main
+  dependencies:
+    krb5: '>=1.19.3,<1.20.0a0'
+    libgcc-ng: '>=12'
+    libnghttp2: '>=1.47.0,<2.0a0'
+    libssh2: '>=1.10.0,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+  hash:
+    md5: fdca8cd67ec2676f90a70ac73a32538b
+    sha256: 485249c8cf7c2bd67d8308f7d1fccbe64e54334ad6cc73168d665eed824ca3bc
+  manager: conda
+  name: libcurl
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.86.0-h2283fc2_1.tar.bz2
+  version: 7.86.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 2d7028ea2a77f909931e1a173d952261
+    sha256: 05a217ff2eea3fb0bada54f4c7c8efe5eb35e1ad7d142d662b364c686ff80da6
+  manager: conda
+  name: markupsafe
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py310h5764c6d_2.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 9b6ad26944f19f599800b068e0582227
+    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 9.0.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 1fa34c9e9be72b7e4c3c9b95017463a3
+    sha256: 7878b37c7a97c14d01745f72b33921fbdb46617932bed8c791803129f9fae8a9
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.4-py310hbf28c38_1.tar.bz2
+  version: 1.0.4
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: a4eea5bff523f26442405bc5d1f52adb
+    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
+  manager: conda
+  name: pastel
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.2.1
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
+    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
+  version: 1.9.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2fb3f88922e7aec26ba652fcdfe13950
+    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
+  manager: conda
+  name: platformdirs
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
+  version: 2.5.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 4c75b7766a1a1dd09d504c63cb5276e2
+    sha256: c8953a9542a1df749037721722ae25316d416812f74728d85a7bd07e9a94268b
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/poetry-core-1.0.8-py310hff52083_1.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 359eeb6536da0e687af562ed265ec263
+    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
+  manager: conda
+  name: ptyprocess
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 0e565d732f6660374b45d76761c09b06
+    sha256: 9bf587a2a0f0f73b71740b079507ec99282b73c596ec73cc602d7ccf73350709
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pycosat-0.6.4-py310h5764c6d_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
+    python: 2.7.*|>=3.4
+  hash:
+    md5: 076becd9e05608f8dc72757d5f3a91ff
+    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
+  manager: conda
+  name: pycparser
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
+  version: '2.21'
+- category: main
+  dependencies:
+    python: '>=3.3'
+  hash:
+    md5: edf8651c4379d9d1495ad6229622d150
+    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
+  manager: conda
+  name: pylev
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
+  manager: conda
+  name: pyparsing
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
+- category: main
+  dependencies:
+    __unix: ''
+    python: '>=3.8'
+  hash:
+    md5: 2a7de29fb590ca14b5243c4c812c8025
+    sha256: a42f826e958a8d22e65b3394f437af7332610e43ee313393d1cf143f0a2d274b
+  manager: conda
+  name: pysocks
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
+  version: 1.7.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: 9e68d2ff6d98737c855b65f48dd3c597
+    sha256: 602d68ee4544274b12fb6d13b8d5fc61d0ebbee190292c21d8be10a4e68185bd
+  manager: conda
+  name: pyyaml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2
+  version: '6.0'
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 2dabb2fa2603a52d072ea6a50c539205
+    sha256: 6de36a7b9d56dda401ef3545f979a23d2225a150519bcc44bd39b2b995bbe3d0
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h5764c6d_0.tar.bz2
+  version: 0.2.7
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: f588192bd22fb64650ccb5781cd83fb0
+    sha256: 4a17acbb2fae7b567b9f7527eb50833c266df00de7fee41f18bb2006dfab8939
+  manager: conda
+  name: ruamel_yaml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel_yaml-0.15.80-py310h5764c6d_1008.tar.bz2
+  version: 0.15.80
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
+    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
+  manager: conda
+  name: setuptools
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 65.5.1
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 437655338696f9d0dfdb0a024e66b255
+    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: e5f25f8dbc060e9a8d912e432202afc2
+    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
+  manager: conda
+  name: six
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+  version: 1.16.0
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: f832c45a477c78bebd107098db465095
+    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
+  manager: conda
+  name: toml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+  version: 0.10.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 5844808ffab9ebdb694585b50ba02a96
+    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
+  manager: conda
+  name: tomli
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.0.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 73506d1ab4202481841c68c169b7ef6c
+    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
+  manager: conda
+  name: tomli-w
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2d93b130d148d7fc77e583677792fc6a
+    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
+  manager: conda
+  name: typing_extensions
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 3563be4c5611a44210d9ba0c16113136
+    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
+  manager: conda
+  name: webencodings
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
+  version: 0.5.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: c829cfb8cb826acb9de0ac1a2df0a940
+    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
+  manager: conda
+  name: wheel
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
+  version: 0.38.4
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 09b5b885341697137879a4f039a9e5a1
+    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
+  manager: conda
+  name: zipp
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
+  version: 3.11.0
+- category: main
+  dependencies:
+    libffi: '>=3.4,<4.0a0'
+    libgcc-ng: '>=12'
+    pycparser: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 6bb8063dd08f9724c18744b0e040cfe2
+    sha256: 97c8d32460e294486e44c9b92e8bb2bf5680bd58c10f5f5a172e47017309d442
+  manager: conda
+  name: cffi
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_2.tar.bz2
+  version: 1.15.1
+- category: main
+  dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
+    crashtest: '>=0.3.0,<0.4.0'
+    pastel: '>=0.2.0,<0.3.0'
+    pylev: '>=1.3,<2.0'
+    python: ''
+  hash:
+    md5: 159273f717a11e53b2656f8b6521a5e2
+    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
+  manager: conda
+  name: clikit
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
+  version: 0.6.2
+- category: main
+  dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
+    python: '>=3.8'
+    zipp: '>=0.5'
+  hash:
+    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
+    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
+  manager: conda
+  name: importlib-metadata
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: 31e4a1506968d017229bdb64695013a1
+    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 3.2.3
+- category: main
+  dependencies:
+    markupsafe: '>=2.0'
+    python: '>=3.7'
+  hash:
+    md5: c8490ed5c70966d232fdd389d0dbed37
+    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
+  manager: conda
+  name: jinja2
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
+  version: 3.1.2
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libarchive: '>=3.5.2,<3.6.0a0'
+    libcurl: '>=7.86.0,<8.0a0'
+    libgcc-ng: '>=12'
+    libiconv: '>=1.17,<2.0a0'
+    libsolv: '>=0.7.22,<0.8.0a0'
+    libstdcxx-ng: '>=12'
+    openssl: '>=3.0.7,<4.0a0'
+    reproc-cpp: '>=14.2,<15.0a0'
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: 9d38a1b35b7de29dfc4d64daeb1e27fc
+    sha256: 0422a1e4a5f0e12230d2108c42242f49bbcb4f5da296bb6054000f3d051b5231
+  manager: conda
+  name: libmamba
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.1.0-h70b1f8a_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    pyparsing: '>=2.0.2,!=3.0.5'
+    python: '>=3.6'
+  hash:
+    md5: 71f1ab2de48613876becddd496371c85
+    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
+  manager: conda
+  name: packaging
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
+  version: '21.3'
+- category: main
+  dependencies:
+    ptyprocess: '>=0.5'
+    python: ''
+  hash:
+    md5: 5909e7b978141dd80d28dbf9de627827
+    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
+  manager: conda
+  name: pexpect
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
+  version: 4.8.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    setuptools: ''
+    wheel: ''
+  hash:
+    md5: da66f2851b9836d3a7c5190082a45f7d
+    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
+  manager: conda
+  name: pip
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 22.3.1
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+  hash:
+    md5: 93643151fba5c31c676effdd7661f075
+    sha256: d78bd1f789a1a79be1f76a8025476e1fcf72fe9becdaf23ec9e1c4bbc67eebf8
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.21-py310h5764c6d_2.tar.bz2
+  version: 0.17.21
+- category: main
+  dependencies:
+    python: '>=3.6'
+    typing: '>=3.6,<4.0'
+  hash:
+    md5: 471bf9e605820b59988e830382b8d654
+    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
+  version: 0.11.6
+- category: main
+  dependencies:
+    colorama: ''
+    python: '>=2.7'
+  hash:
+    md5: 6642233f341e1900d0c8e6eddb979c14
+    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
+  manager: conda
+  name: tqdm
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
+  version: 4.64.0
+- category: main
+  dependencies:
+    typing_extensions: 4.4.0 pyha770c72_0
+  hash:
+    md5: be969210b61b897775a0de63cd9e9026
+    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
+  manager: conda
+  name: typing-extensions
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    distlib: '>=0.3.6,<1'
+    filelock: '>=3.4.1,<4'
+    platformdirs: '>=2.4,<3'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: c6fc5e3f0a463ddb59cfda9a1582cfa0
+    sha256: b43ae0b1fe2c77c05b39de70c28a419078d67731d12a52aa3b3440a12398446c
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.17.0-py310hff52083_0.conda
+  version: 20.17.0
+- category: main
+  dependencies:
+    cffi: '>=1.0.0'
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 87669c3468dff637bbd0363bc0f895cf
+    sha256: a37f9a00170f48e71b67bb4547e8bf352dcee4e4a79a55f087b512022cc64a0d
+  manager: conda
+  name: brotlipy
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1005.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    clikit: '>=0.6.0,<0.7.0'
+    python: '>=3.6'
+  hash:
+    md5: 4c82b11a3d06031bd58e7d869f53d965
+    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
+  manager: conda
+  name: cleo
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
+  version: 0.8.1
+- category: main
+  dependencies:
+    cffi: '>=1.12'
+    libgcc-ng: '>=12'
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: f999dcc21fe27ad97a8afcfa590daa14
+    sha256: 64a31aa5153e977e58256b098044b61ef903885b5b8f7ed807d066d1ceed2244
+  manager: conda
+  name: cryptography
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.4-py310h600f1e7_0.conda
+  version: 38.0.4
+- category: main
+  dependencies:
+    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
+  hash:
+    md5: 3dc2248927de739b4d2e2da9a9972bfe
+    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
+  manager: conda
+  name: importlib_metadata
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libgcc-ng: '>=12'
+    libmamba: 1.1.0 h70b1f8a_2
+    libstdcxx-ng: '>=12'
+    openssl: '>=3.0.7,<4.0a0'
+    pybind11-abi: '4'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: 1bc930a417259d6a0668931cdd9aa805
+    sha256: 7d8b967de764a98526c08e9aa718d650f6e7d5a5ba57181f6b4d6c1af5f0d5b0
+  manager: conda
+  name: libmambapy
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.1.0-py310h69aa5bf_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.1.0'
+  hash:
+    md5: d666328dd06e3be9c1e541c5f499f895
+    sha256: c4a0c7ae066f43ef764f95578e16fad41b5cf577cf3777e5a657ff08334d9b97
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.2-py310h5764c6d_1.tar.bz2
+  version: 1.10.2
+- category: main
+  dependencies:
+    cffi: '>=1.11'
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 2cce1a48e6687f64d371d2e7fc9c7fbf
+    sha256: 97f69cae6513a1c64ce2ec87380f9a177e386af398300921a869c07e826b4949
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py310hdeb6495_1.conda
+  version: 0.19.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
+    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
+  version: 0.7.0
+- category: main
+  dependencies:
+    cryptography: '>=38.0.0,<39'
+    python: '>=3.6'
+  hash:
+    md5: fbfa0a180d48c800f922a10a114a8632
+    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
+  manager: conda
+  name: pyopenssl
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
+  version: 22.1.0
+- category: main
+  dependencies:
+    cryptography: ''
+    dbus: ''
+    jeepney: '>=0.6'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: e135d0e3bbb226e8d53d31b4e4f6d93c
+    sha256: 25d2a00bf24a3cab81eba8f77eba8f70a7b3995041fc227f535c0f174536670f
+  manager: conda
+  name: secretstorage
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py310hff52083_1.tar.bz2
+  version: 3.3.3
+- category: main
+  dependencies:
+    conda-package-streaming: '>=0.7.0'
+    python: '>=3.7'
+  hash:
+    md5: 44800e9bd13143292097c65e57323038
+    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
+  version: 2.0.2
+- category: main
+  dependencies:
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    jeepney: '>=0.4.2'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    secretstorage: '>=3.2'
+  hash:
+    md5: 1cc09aec47df38e68442c113f675c8e2
+    sha256: d6052c86a5aa3190bb3ee9ba49230c5a9083c588715a696693378228fadc135d
+  manager: conda
+  name: keyring
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/keyring-23.11.0-py310hff52083_0.tar.bz2
+  version: 23.11.0
+- category: main
+  dependencies:
+    brotlipy: '>=0.6.0'
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: <4.0
+  hash:
+    md5: 3078ef2359efd6ecadbc7e085c5e0592
+    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
+  manager: conda
+  name: urllib3
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
+  version: 1.26.13
+- category: main
+  dependencies:
+    certifi: '>=2017.4.17'
+    charset-normalizer: '>=2,<3'
+    idna: '>=2.5,<4'
+    python: '>=3.7,<4.0'
+    urllib3: '>=1.21.1,<1.27'
+  hash:
+    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
+    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
+  manager: conda
+  name: requests
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
+  version: 2.28.1
+- category: main
+  dependencies:
+    filelock: '>=3.8.0'
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: ''
+  hash:
+    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
+    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
+  version: 0.12.12
+- category: main
+  dependencies:
+    conda-package-handling: '>=1.3.0'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.20.1,<3'
+    ruamel_yaml: '>=0.11.14,<0.17'
+    setuptools: '>=31.0.1'
+    toolz: '>=0.8.1'
+  hash:
+    md5: 8d78ef95742dcd284e6a5ee99bb0659b
+    sha256: 9be2c55658fdfc9837c5d4f9bf2cc384ebbc8dd2bb8dbdb1300721a8abc93c95
+  manager: conda
+  name: conda
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/conda-22.9.0-py310hff52083_2.tar.bz2
+  version: 22.9.0
+- category: main
+  dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
+    docutils: ''
+    flit-core: 3.8.0 pyhd8ed1ab_0
+    pip: ''
+    python: '>=3.6'
+    requests: ''
+    tomli-w: ''
+  hash:
+    md5: d37c34176396c5402cf80c32e67731b7
+    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
+  manager: conda
+  name: flit
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: ''
+    requests: '>=2.0.1,<=3.0.0'
+  hash:
+    md5: 402668adee8fcba9a9c265cdc2a88f5a
+    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
+  version: 0.9.1
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9'
+    cachy: '>=0.3.0'
+    click: '>=8.0'
+    click-default-group: ''
+    clikit: '>=0.6.2'
+    crashtest: '>=0.3.0'
+    ensureconda: '>=1.3'
+    filelock: '>=3.8.0'
+    html5lib: '>=1.0'
+    importlib-metadata: '>=1.7.0'
+    jinja2: ''
+    keyring: '>=21.2.0'
+    packaging: '>=20.4'
+    pkginfo: '>=1.4'
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2.18'
+    ruamel.yaml: ''
+    tomli: ''
+    tomlkit: '>=0.7.0'
+    toolz: <1.0.0,>=0.12.0
+    typing-extensions: ''
+    virtualenv: '>=20.0.26'
+  hash:
+    md5: 7b1dde4760c5c554523fead6c2771af2
+    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.1
+- category: main
+  dependencies:
+    conda: '>=4.8,<23.4'
+    libmambapy: 1.1.0 py310h69aa5bf_2
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 263d921fcebace4d7bd7ad2ac0b6ae3f
+    sha256: 7f142cc44354354baf12ccfba5ce39e2a0f4fde4bfb567ed42a4ca0f9b43589b
+  manager: conda
+  name: mamba
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/mamba-1.1.0-py310h51d5547_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9,<0.13.0'
+    cachy: '>=0.3.0,<0.4.0'
+    cleo: '>=0.8.1,<0.9.0'
+    clikit: '>=0.6.2,<0.7.0'
+    crashtest: '>=0.3.0,<0.4.0'
+    html5lib: '>=1.0,<2.0'
+    keyring: '>=21.2.0'
+    lockfile: '>=0.9'
+    packaging: '>=20.4,<21.0'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.4,<2.0'
+    poetry-core: '>=1.0.7,<1.1.0'
+    ptyprocess: '>=0.5'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<0.10.0'
+    shellingham: '>=1.1,<2.0'
+    tomlkit: '>=0.7.0,<1.0.0'
+    virtualenv: '>=20.0.26,<21.0.0'
+  hash:
+    md5: 774207808696c8728977983b930f1cb5
+    sha256: ebeeffa1afaece3c6defc74dcb566a430a3b2d12c574000483bdb5a268b14f57
+  manager: conda
+  name: poetry
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/linux-64/poetry-1.1.14-py310hff52083_0.tar.bz2
+  version: 1.1.14
+- category: main
+  dependencies: {}
+  hash:
+    md5: 37edc4e6304ca87316e160f5ca0bd1b5
+    sha256: 60ba4c64f5d0afca0d283c7addba577d3e2efc0db86002808dadb0498661b2f2
+  manager: conda
+  name: bzip2
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies: {}
+  hash:
+    md5: 00b3e98a61e6430808fe7a2534681f28
+    sha256: 1cb663c9916aab52a90a80505fec8c1a89fab21f58f3c5a949a2f286e92cb16c
+  manager: conda
+  name: c-ares
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.18.1-h0d85af4_0.tar.bz2
+  version: 1.18.1
+- category: main
+  dependencies: {}
+  hash:
+    md5: 67b268c32433047914482def1ce215c2
+    sha256: e1c929207f8a8e03fa86150c3b446f3511f35b2146d3031de305088c3b148c58
+  manager: conda
+  name: ca-certificates
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.9.24-h033912b_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies: {}
+  hash:
+    md5: 208a6a874b073277374de48a782f6b10
+    sha256: ebb75dd9f854b1f184a98d0b9128a3faed6cd2f05f83677e1f399c253580afe7
+  manager: conda
+  name: libcxx
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hccf4f1f_0.tar.bz2
+  version: 14.0.6
+- category: main
+  dependencies: {}
+  hash:
+    md5: 79dc2be110b2a3d1e97ec21f691c50ad
+    sha256: c4154d424431898d84d6afb8b32e3ba749fe5d270d322bb0af74571a3cb09c6b
+  manager: conda
+  name: libev
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2
+  version: '4.33'
+- category: main
+  dependencies: {}
+  hash:
+    md5: ccb34fb14960ad8b125962d3d79b31a9
+    sha256: 7a2d27a936ceee6942ea4d397f9c7d136f12549d86f7617e8b6bad51e01a941f
+  manager: conda
+  name: libffi
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+  version: 3.4.2
+- category: main
+  dependencies: {}
+  hash:
+    md5: 691d103d11180486154af49c037b7ed9
+    sha256: 4a3294037d595754f7da7c11a41f3922f995aaa333f3cb66f02d8afa032a7bc2
+  manager: conda
+  name: libiconv
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2
+  version: '1.17'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 35eb3fce8d51ed3c1fd4122bad48250b
+    sha256: 0d954350222cc12666a1f4852dbc9bcf4904d8e467d29505f2b04ded6518f890
+  manager: conda
+  name: libzlib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2
+  version: 1.2.13
+- category: main
+  dependencies: {}
+  hash:
+    md5: 0b6bca372a95d6c602c7a922e928ce79
+    sha256: c8a9401eff2efbbcc6da03d0066ee85d72402f7658c240e7968c64052a0d0493
+  manager: conda
+  name: lzo
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/lzo-2.10-haf1e3a3_1000.tar.bz2
+  version: '2.10'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 76217ebfbb163ff2770a261f955a5861
+    sha256: 9794a23d03586c99cac49d4ae3d5337faaa6bfc256b31d2662ff4ad5972be143
+  manager: conda
+  name: ncurses
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2
+  version: '6.3'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 878f923dd6acc8aeb47a75da6c4098be
+    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
+  manager: conda
+  name: pybind11-abi
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
+  version: '4'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 42da9b0138e911cd5b2f75b0278e26dc
+    sha256: 0a66852c47be6b28b70bde29891a71d047730c723355d44b0da48db79fb99eb1
+  manager: conda
+  name: python_abi
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-3_cp310.conda
+  version: '3.10'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 6f87f4707e4daf5823ce56dce5d9fbea
+    sha256: 7181e7eab6f959640e41c285d57670885c1db7f7a897b43c7d7fb47987222d32
+  manager: conda
+  name: reproc
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/reproc-14.2.3-h0d85af4_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies: {}
+  hash:
+    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
+    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
+  manager: conda
+  name: tzdata
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
+  version: 2022g
+- category: main
+  dependencies: {}
+  hash:
+    md5: a72f9d4ea13d55d745ff1ed594747f10
+    sha256: eb09823f34cc2dd663c0ec4ab13f246f45dcd52e5b8c47b9864361de5204a1c8
+  manager: conda
+  name: xz
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+  version: 5.2.6
+- category: main
+  dependencies: {}
+  hash:
+    md5: d7e08fcf8259d742156188e8762b4d20
+    sha256: 5301417e2c8dea45b401ffee8df3957d2447d4ce80c83c5ff151fc6bfe1c4148
+  manager: conda
+  name: yaml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
+  version: 0.2.5
+- category: main
+  dependencies:
+    libcxx: '>=14.0.4'
+  hash:
+    md5: 310d897883dbdd88555d6321a4c2e6e8
+    sha256: 4891b66c94df8a346010caefb5d92df5e367be87ef0dea35a15d988f39a82719
+  manager: conda
+  name: fmt
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/fmt-9.1.0-hb8565cd_0.tar.bz2
+  version: 9.1.0
+- category: main
+  dependencies:
+    libcxx: '>=12.0.1'
+  hash:
+    md5: 376635049e9b9b0bb875efd39dcd7b3b
+    sha256: 0807aa3fd93804ab239808d149e7f210a83e1c61bc59bb84818f4ef9f6036d86
+  manager: conda
+  name: icu
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2
+  version: '70.1'
+- category: main
+  dependencies:
+    ncurses: '>=6.2,<7.0.0a0'
+  hash:
+    md5: 6016a8a1d0e63cac3de2c352cd40208b
+    sha256: dbd3c3f2eca1d21c52e4c03b21930bbce414c4592f8ce805801575b9e9256095
+  manager: conda
+  name: libedit
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
+  version: 3.1.20191231
+- category: main
+  dependencies:
+    libcxx: '>=12.0.1'
+    libzlib: '>=1.2.11,<1.3.0a0'
+  hash:
+    md5: 068ed0617893ecbccbf65a32ea1e8056
+    sha256: 7c04b4a878ccc596b9ec71e2418c49e713e5c32748437134ec72dca51820374c
+  manager: conda
+  name: libsolv
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libsolv-0.7.22-hd9580d2_0.tar.bz2
+  version: 0.7.22
+- category: main
+  dependencies:
+    libzlib: '>=1.2.13,<1.3.0a0'
+  hash:
+    md5: ceb13b6726534b96e3b4e3dda91e9050
+    sha256: ae19f866188cc0c514fed754468460ae9e8dd763ebbd7b7afc4e818d71844297
+  manager: conda
+  name: libsqlite
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.40.0-ha978bb4_0.tar.bz2
+  version: 3.40.0
+- category: main
+  dependencies:
+    libcxx: '>=11.1.0'
+  hash:
+    md5: 05c08241b66631c00ca4f9e0b75320bc
+    sha256: 627c435c511e789ed04e0e2077fdfc645117474c4d1c4a7c0d31241936632cd4
+  manager: conda
+  name: lz4-c
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.3-he49afe7_1.tar.bz2
+  version: 1.9.3
+- category: main
+  dependencies:
+    ca-certificates: ''
+  hash:
+    md5: 7a3fb6d40e0aa5dbb5b4ef54462f00a8
+    sha256: 3eb19686ae870daae035582cb93253a6435f71baf537addced41be449b4daf67
+  manager: conda
+  name: openssl
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.0.7-hfd90126_1.conda
+  version: 3.0.7
+- category: main
+  dependencies:
+    ncurses: '>=6.3,<7.0a0'
+  hash:
+    md5: 89fa404901fa8fb7d4f4e07083b8d635
+    sha256: c65dc1200a252832db49bdd6836c512a0eaafe97aa914b9f8358b15eebb1d94b
+  manager: conda
+  name: readline
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/readline-8.1.2-h3899abd_0.tar.bz2
+  version: 8.1.2
+- category: main
+  dependencies:
+    libcxx: '>=11.1.0'
+    reproc: 14.2.3 h0d85af4_0
+  hash:
+    md5: 7dafcfaa471cd16cbd73832cefc39770
+    sha256: e7f7ca953a0888b37cee9197ed844d67af02036c87402174935107827779bbf4
+  manager: conda
+  name: reproc-cpp
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/reproc-cpp-14.2.3-he49afe7_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies:
+    libzlib: '>=1.2.11,<1.3.0a0'
+  hash:
+    md5: 8e9480d9c47061db2ed1b4ecce519a7f
+    sha256: 331aa1137a264fd9cc905f04f09a161c801fe504b93da08b4e6697bd7c9ae6a6
+  manager: conda
+  name: tk
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2
+  version: 8.6.12
+- category: main
+  dependencies:
+    libcxx: '>=14.0.4'
+  hash:
+    md5: 06c92b93b45ed2c842eb0893c5d2552a
+    sha256: 9d1c5df1d4503d1451b5fe46a7502eb8ee98aa603f3f092f7fcf3e0d43d2a8f3
+  manager: conda
+  name: yaml-cpp
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/yaml-cpp-0.7.0-hf0c8a7f_2.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    libzlib: 1.2.12 hfe4f2af_2
+  hash:
+    md5: fe7ebd3b35b8f26f6a7d0af481a21721
+    sha256: 8f455dcebeae224fdb422ba8f90d33e61298dc088139227e25eb4ee20a3ea35f
+  manager: conda
+  name: zlib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/zlib-1.2.12-hfe4f2af_2.tar.bz2
+  version: 1.2.12
+- category: main
+  dependencies:
+    libcxx: '>=13.0.1'
+    libzlib: '>=1.2.12,<1.3.0a0'
+  hash:
+    md5: 0b446e84f3ccf085e590dc1f73eebe3f
+    sha256: acf19719a0a4b7534532166f84346709fdb8ccf960bc6c19ac3b437177e95dde
+  manager: conda
+  name: zstd
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hfa58983_4.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
+    libcxx: '>=12.0.1'
+    libedit: '>=3.1.20191231,<4.0a0'
+    openssl: '>=3.0.0,<4.0a0'
+  hash:
+    md5: 8acf20165e07870bc65510a363ff45bb
+    sha256: 7f4de03413501f22f287a9fad86710de0f47b459ecf08026257e9a49d7c93428
+  manager: conda
+  name: krb5
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.19.3-hb98e516_0.tar.bz2
+  version: 1.19.3
+- category: main
+  dependencies:
+    c-ares: '>=1.18.1,<2.0a0'
+    libcxx: '>=13.0.1'
+    libev: '>=4.33,<4.34.0a0'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    openssl: '>=3.0.5,<4.0a0'
+  hash:
+    md5: 19d5ae4be3e4b3cfa5696f3667e8c631
+    sha256: 9e14d62e4462e6be28bcaa266f69e96ead43f4d7ef566e9cd460dbc9ae999daf
+  manager: conda
+  name: libnghttp2
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.47.0-h5aae05b_1.tar.bz2
+  version: 1.47.0
+- category: main
+  dependencies:
+    libzlib: '>=1.2.12,<1.3.0a0'
+    openssl: '>=3.0.5,<4.0a0'
+  hash:
+    md5: 5a28624eeb7812b585b9e2d75f846ba2
+    sha256: 3261dc7fa9cb928e8a0da4857b89bdd3e965766a6cd5b6456d4407cba6b25402
+  manager: conda
+  name: libssh2
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.10.0-h47af595_3.tar.bz2
+  version: 1.10.0
+- category: main
+  dependencies:
+    icu: '>=70.1,<71.0a0'
+    libiconv: '>=1.17,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    xz: '>=5.2.6,<6.0a0'
+  hash:
+    md5: 13ba8bf8f44cdac2e5401dac20a36040
+    sha256: 464b3e2350c25615bbea89ab512f8f5fcd88a9e2f6cf9dfe7b72aa9bc56efcda
+  manager: conda
+  name: libxml2
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.10.3-hb9e07b5_0.tar.bz2
+  version: 2.10.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libffi: '>=3.4,<4.0a0'
+    libsqlite: '>=3.40.0,<4.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    ncurses: '>=6.3,<7.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+    readline: '>=8.1.2,<9.0a0'
+    tk: '>=8.6.12,<8.7.0a0'
+    tzdata: ''
+    xz: '>=5.2.6,<6.0a0'
+  hash:
+    md5: 4b6976686db5f16650df28332d84ce9e
+    sha256: b001073de81761dc30848a55e92fd2eb4cb9fc60c2809afa0987c2a7d7f621f9
+  manager: conda
+  name: python
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.8-he7542f4_0_cpython.conda
+  version: 3.10.8
+- category: main
+  dependencies:
+    libzlib: '>=1.2.12,<1.3.0a0'
+    ncurses: '>=6.3,<7.0a0'
+    readline: '>=8.1.2,<9.0a0'
+    zlib: '>=1.2.12,<1.3.0a0'
+  hash:
+    md5: eea4504fd46050a22d482addde6ae7c7
+    sha256: 437de0e2658840c53ce8f6a4cb748aca49205fefe0b61164151372be2cfbef40
+  manager: conda
+  name: sqlite
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/sqlite-3.39.2-hd9f0692_0.tar.bz2
+  version: 3.39.2
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 5dfee17f24e2dfd18d7392b48c9351e2
+    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
+  manager: conda
+  name: cachy
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
+  version: 0.3.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: f66309b099374af91369e67e84af397d
+    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
+  manager: conda
+  name: certifi
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c1d5b294fbf9a795dec349a6f4d8be8e
+    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
+  manager: conda
+  name: charset-normalizer
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    __unix: ''
+    python: '>=3.8'
+  hash:
+    md5: 20e4087407c7cb04a40817114b333dbf
+    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+  manager: conda
+  name: click
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
+  version: 8.1.3
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c267da48ce208905d7d976d49dfd9433
+    sha256: fcab1a16af5daf3a1ea9b0a7ed15615f0d5fff05ff4925ed570988868bb29e38
+  manager: conda
+  name: colorama
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.5
+- category: main
+  dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: b8477552274c1cfdb533e954c76523f1
+    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.1
+- category: main
+  dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
+    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
+  manager: conda
+  name: distlib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.6
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 932d057a35046e6eb92561c723d4ebe6
+    sha256: 72c1aa5ae0133081037e7c7115633ad7308e85aa871347f70ebf677e12f41ce6
+  manager: conda
+  name: docutils
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py310h2ec42d9_1.tar.bz2
+  version: '0.19'
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
+    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
+  manager: conda
+  name: filelock
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
+  version: 3.8.2
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 6d5e56de2e65da7aa35fd10131226efa
+    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
+  manager: conda
+  name: flit-core
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 34272b248891bddccc64479f9a7fffed
+    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
+  manager: conda
+  name: idna
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
+  version: '3.4'
+- category: main
+  dependencies:
+    python: 2.7|>=3.4
+  hash:
+    md5: 25045ddd7fe83ddf71c181d6212e9913
+    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
+  manager: conda
+  name: invoke
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.7.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libiconv: '>=1.16,<2.0.0a0'
+    libxml2: '>=2.9.14,<2.11.0a0'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    lz4-c: '>=1.9.3,<1.10.0a0'
+    lzo: '>=2.10,<3.0a0'
+    openssl: '>=3.0.3,<4.0a0'
+    xz: '>=5.2.5,<5.3.0a0'
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 57f1c0e98ad3d4836d66d457f3690dc9
+    sha256: 0eed997df470af8f268d69428dacc51a26d1ecafea1de446c406f4d5f8ae5469
+  manager: conda
+  name: libarchive
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarchive-3.5.2-hbf7dfe4_3.tar.bz2
+  version: 3.5.2
+- category: main
+  dependencies:
+    krb5: '>=1.19.3,<1.20.0a0'
+    libnghttp2: '>=1.47.0,<2.0a0'
+    libssh2: '>=1.10.0,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+  hash:
+    md5: af83102fc53762fb78e27657b540756f
+    sha256: f76129b5fbb7d08a1457ce36eb16b32da470ccd5ad8e498265c97750ccddd921
+  manager: conda
+  name: libcurl
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libcurl-7.86.0-h581aaea_1.tar.bz2
+  version: 7.86.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 232c20719e4290fa284ae1e9a4661dfa
+    sha256: 45aa996770bb49fdd6bc68e24b301932c2bb592522e3798f0c80e0206c352b8b
+  manager: conda
+  name: markupsafe
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py310h90acd4f_2.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 9b6ad26944f19f599800b068e0582227
+    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 9.0.0
+- category: main
+  dependencies:
+    libcxx: '>=14.0.4'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 164e856479d735e96fcbd547afa70251
+    sha256: c8311366a2858a24b3ac65fa1c6f8ca63f83528bbb2f6825cdf56d30047d022b
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.4-py310ha23aa8a_1.tar.bz2
+  version: 1.0.4
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: a4eea5bff523f26442405bc5d1f52adb
+    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
+  manager: conda
+  name: pastel
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.2.1
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
+    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
+  version: 1.9.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2fb3f88922e7aec26ba652fcdfe13950
+    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
+  manager: conda
+  name: platformdirs
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
+  version: 2.5.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: f8d8f3b9a093c53d03ca1ca52fab989c
+    sha256: 864e4ae20da2fb810a9ecb948396b49705a35f5b36f909a3e2b10abdfe4b0dca
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/poetry-core-1.0.8-py310h2ec42d9_1.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 359eeb6536da0e687af562ed265ec263
+    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
+  manager: conda
+  name: ptyprocess
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 95c032c354c500001a935aac4c059376
+    sha256: 28012e6ae66102b9b4f69316d026985373b2c33161304bc6841c1d9c3f9ec34e
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pycosat-0.6.4-py310h90acd4f_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
+    python: 2.7.*|>=3.4
+  hash:
+    md5: 076becd9e05608f8dc72757d5f3a91ff
+    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
+  manager: conda
+  name: pycparser
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
+  version: '2.21'
+- category: main
+  dependencies:
+    python: '>=3.3'
+  hash:
+    md5: edf8651c4379d9d1495ad6229622d150
+    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
+  manager: conda
+  name: pylev
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
+  manager: conda
+  name: pyparsing
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
+- category: main
+  dependencies:
+    __unix: ''
+    python: '>=3.8'
+  hash:
+    md5: 2a7de29fb590ca14b5243c4c812c8025
+    sha256: a42f826e958a8d22e65b3394f437af7332610e43ee313393d1cf143f0a2d274b
+  manager: conda
+  name: pysocks
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
+  version: 1.7.1
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: e0ba2009f52ccda088c63dedf0d1c5ec
+    sha256: ab7b2b8fef9adc4211834054d004f3e286161bb3e1dcb17d4b974fae4f87b31b
+  manager: conda
+  name: pyyaml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h90acd4f_5.tar.bz2
+  version: '6.0'
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: a47602a6c5a1fc89a64b91bb44036537
+    sha256: 9231096ef851e63705df491ffa2d0571d68757630c52513b5dd655474d37741f
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py310h90acd4f_0.tar.bz2
+  version: 0.2.7
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: 936cc17fa13ae01bcbd1daaf4e31fc72
+    sha256: 6212a6298cda55296a32724ed1065cb6b9ba55c2df7fecf650be4a4ac373f5d7
+  manager: conda
+  name: ruamel_yaml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel_yaml-0.15.80-py310h90acd4f_1008.tar.bz2
+  version: 0.15.80
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
+    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
+  manager: conda
+  name: setuptools
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 65.5.1
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 437655338696f9d0dfdb0a024e66b255
+    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: e5f25f8dbc060e9a8d912e432202afc2
+    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
+  manager: conda
+  name: six
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+  version: 1.16.0
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: f832c45a477c78bebd107098db465095
+    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
+  manager: conda
+  name: toml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+  version: 0.10.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 5844808ffab9ebdb694585b50ba02a96
+    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
+  manager: conda
+  name: tomli
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.0.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 73506d1ab4202481841c68c169b7ef6c
+    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
+  manager: conda
+  name: tomli-w
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2d93b130d148d7fc77e583677792fc6a
+    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
+  manager: conda
+  name: typing_extensions
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 3563be4c5611a44210d9ba0c16113136
+    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
+  manager: conda
+  name: webencodings
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
+  version: 0.5.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: c829cfb8cb826acb9de0ac1a2df0a940
+    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
+  manager: conda
+  name: wheel
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
+  version: 0.38.4
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 09b5b885341697137879a4f039a9e5a1
+    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
+  manager: conda
+  name: zipp
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
+  version: 3.11.0
+- category: main
+  dependencies:
+    libffi: '>=3.4,<4.0a0'
+    pycparser: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: dacdbcd6bcec3dc5b34f1f6a06915b66
+    sha256: b548a2f5ba121a698010a9c4b05009f5e701d5d16da0b24fbad9691f8d84b17e
+  manager: conda
+  name: cffi
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_2.tar.bz2
+  version: 1.15.1
+- category: main
+  dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
+    crashtest: '>=0.3.0,<0.4.0'
+    pastel: '>=0.2.0,<0.3.0'
+    pylev: '>=1.3,<2.0'
+    python: ''
+  hash:
+    md5: 159273f717a11e53b2656f8b6521a5e2
+    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
+  manager: conda
+  name: clikit
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
+  version: 0.6.2
+- category: main
+  dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
+    python: '>=3.8'
+    zipp: '>=0.5'
+  hash:
+    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
+    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
+  manager: conda
+  name: importlib-metadata
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: 31e4a1506968d017229bdb64695013a1
+    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 3.2.3
+- category: main
+  dependencies:
+    markupsafe: '>=2.0'
+    python: '>=3.7'
+  hash:
+    md5: c8490ed5c70966d232fdd389d0dbed37
+    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
+  manager: conda
+  name: jinja2
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
+  version: 3.1.2
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libarchive: '>=3.5.2,<3.6.0a0'
+    libcurl: '>=7.86.0,<8.0a0'
+    libcxx: '>=14.0.6'
+    libiconv: '>=1.17,<2.0a0'
+    libsolv: '>=0.7.22,<0.8.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+    reproc-cpp: '>=14.2,<15.0a0'
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: b2f3194abef248954cbd738d602fc6a5
+    sha256: 3af6ff8646629c59b2777a39f25abd05010ca9c4111079cd92d48a94597a51bb
+  manager: conda
+  name: libmamba
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.1.0-h8b63968_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    pyparsing: '>=2.0.2,!=3.0.5'
+    python: '>=3.6'
+  hash:
+    md5: 71f1ab2de48613876becddd496371c85
+    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
+  manager: conda
+  name: packaging
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
+  version: '21.3'
+- category: main
+  dependencies:
+    ptyprocess: '>=0.5'
+    python: ''
+  hash:
+    md5: 5909e7b978141dd80d28dbf9de627827
+    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
+  manager: conda
+  name: pexpect
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
+  version: 4.8.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    setuptools: ''
+    wheel: ''
+  hash:
+    md5: da66f2851b9836d3a7c5190082a45f7d
+    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
+  manager: conda
+  name: pip
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 22.3.1
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+  hash:
+    md5: b7921dd86e7931ff90727c3545f9a976
+    sha256: 520193524d3c12723d0d675e4fa059ec078e103a88cd3069692c32ff9f57cfda
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.21-py310h90acd4f_2.tar.bz2
+  version: 0.17.21
+- category: main
+  dependencies:
+    python: '>=3.6'
+    typing: '>=3.6,<4.0'
+  hash:
+    md5: 471bf9e605820b59988e830382b8d654
+    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
+  version: 0.11.6
+- category: main
+  dependencies:
+    colorama: ''
+    python: '>=2.7'
+  hash:
+    md5: 6642233f341e1900d0c8e6eddb979c14
+    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
+  manager: conda
+  name: tqdm
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
+  version: 4.64.0
+- category: main
+  dependencies:
+    typing_extensions: 4.4.0 pyha770c72_0
+  hash:
+    md5: be969210b61b897775a0de63cd9e9026
+    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
+  manager: conda
+  name: typing-extensions
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    distlib: '>=0.3.6,<1'
+    filelock: '>=3.4.1,<4'
+    platformdirs: '>=2.4,<3'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: a8c9ed46d17f8a92a457e5d0433e8468
+    sha256: 6afe16afef89bf2d51d9ed4588cfb2eb6205dc44d04b46b30d2c70203bfa741d
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.17.0-py310h2ec42d9_0.conda
+  version: 20.17.0
+- category: main
+  dependencies:
+    cffi: '>=1.0.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 63accc45f2b9ae1dad4db9cdfaa903b4
+    sha256: de6e5b17631ef35c6acaeec0ba0143d0e77e0970704f0a3e947a5d59364f3c4a
+  manager: conda
+  name: brotlipy
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    clikit: '>=0.6.0,<0.7.0'
+    python: '>=3.6'
+  hash:
+    md5: 4c82b11a3d06031bd58e7d869f53d965
+    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
+  manager: conda
+  name: cleo
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
+  version: 0.8.1
+- category: main
+  dependencies:
+    cffi: '>=1.12'
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 7f0791ebd6b9c996fbd16ed1368b7eee
+    sha256: 16cfba388e76b1b22b31a0f9ec864f5d4e19902f72eb65b29e2eebb2a1bdc9db
+  manager: conda
+  name: cryptography
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-38.0.4-py310hdd0c95c_0.conda
+  version: 38.0.4
+- category: main
+  dependencies:
+    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
+  hash:
+    md5: 3dc2248927de739b4d2e2da9a9972bfe
+    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
+  manager: conda
+  name: importlib_metadata
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libcxx: '>=14.0.6'
+    libmamba: 1.1.0 h8b63968_2
+    openssl: '>=3.0.7,<4.0a0'
+    pybind11-abi: '4'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: 2b0e4f8eecc71ac0e8e01a01040cb871
+    sha256: a6cf61d04fac8a57490662cc65b686206f9d66954a1d5cdf1ea7db70aa57a9e3
+  manager: conda
+  name: libmambapy
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.1.0-py310hb15139c_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.1.0'
+  hash:
+    md5: 140aaad46ef1de7f9ca167dfebf40aad
+    sha256: fb689bccf7ce9b1643ec59003fc51f4dca3fe719a86782fce72a1b6bd549ecd5
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.2-py310h90acd4f_1.tar.bz2
+  version: 1.10.2
+- category: main
+  dependencies:
+    cffi: '>=1.11'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 6daa5261761ae2a155f21f5a6c162b27
+    sha256: f43d356b78cde97a2a4b0798d5e3256315e6323343ef0d5e69578ce685237838
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py310h3cf44b0_1.conda
+  version: 0.19.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
+    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
+  version: 0.7.0
+- category: main
+  dependencies:
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 2ea3fb1aedecb07304bbc73c8ce3f0ea
+    sha256: fb1229a850420b5f6fd5855b54cfbc837100c0f5c862bc288bb302f0455af035
+  manager: conda
+  name: keyring
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/keyring-23.11.0-py310h2ec42d9_0.tar.bz2
+  version: 23.11.0
+- category: main
+  dependencies:
+    cryptography: '>=38.0.0,<39'
+    python: '>=3.6'
+  hash:
+    md5: fbfa0a180d48c800f922a10a114a8632
+    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
+  manager: conda
+  name: pyopenssl
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
+  version: 22.1.0
+- category: main
+  dependencies:
+    conda-package-streaming: '>=0.7.0'
+    python: '>=3.7'
+  hash:
+    md5: 44800e9bd13143292097c65e57323038
+    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
+  version: 2.0.2
+- category: main
+  dependencies:
+    brotlipy: '>=0.6.0'
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: <4.0
+  hash:
+    md5: 3078ef2359efd6ecadbc7e085c5e0592
+    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
+  manager: conda
+  name: urllib3
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
+  version: 1.26.13
+- category: main
+  dependencies:
+    certifi: '>=2017.4.17'
+    charset-normalizer: '>=2,<3'
+    idna: '>=2.5,<4'
+    python: '>=3.7,<4.0'
+    urllib3: '>=1.21.1,<1.27'
+  hash:
+    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
+    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
+  manager: conda
+  name: requests
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
+  version: 2.28.1
+- category: main
+  dependencies:
+    filelock: '>=3.8.0'
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: ''
+  hash:
+    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
+    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
+  version: 0.12.12
+- category: main
+  dependencies:
+    conda-package-handling: '>=1.3.0'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.20.1,<3'
+    ruamel_yaml: '>=0.11.14,<0.17'
+    setuptools: '>=31.0.1'
+    toolz: '>=0.8.1'
+  hash:
+    md5: 2cf59c02b1e43a37232da097fe9024db
+    sha256: a55ab27dc68ffc0d421750cd840fddeb44a27270530496dfa316bc4cbbf5d50d
+  manager: conda
+  name: conda
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/conda-22.9.0-py310h2ec42d9_2.tar.bz2
+  version: 22.9.0
+- category: main
+  dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
+    docutils: ''
+    flit-core: 3.8.0 pyhd8ed1ab_0
+    pip: ''
+    python: '>=3.6'
+    requests: ''
+    tomli-w: ''
+  hash:
+    md5: d37c34176396c5402cf80c32e67731b7
+    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
+  manager: conda
+  name: flit
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: ''
+    requests: '>=2.0.1,<=3.0.0'
+  hash:
+    md5: 402668adee8fcba9a9c265cdc2a88f5a
+    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
+  version: 0.9.1
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9'
+    cachy: '>=0.3.0'
+    click: '>=8.0'
+    click-default-group: ''
+    clikit: '>=0.6.2'
+    crashtest: '>=0.3.0'
+    ensureconda: '>=1.3'
+    filelock: '>=3.8.0'
+    html5lib: '>=1.0'
+    importlib-metadata: '>=1.7.0'
+    jinja2: ''
+    keyring: '>=21.2.0'
+    packaging: '>=20.4'
+    pkginfo: '>=1.4'
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2.18'
+    ruamel.yaml: ''
+    tomli: ''
+    tomlkit: '>=0.7.0'
+    toolz: <1.0.0,>=0.12.0
+    typing-extensions: ''
+    virtualenv: '>=20.0.26'
+  hash:
+    md5: 7b1dde4760c5c554523fead6c2771af2
+    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.1
+- category: main
+  dependencies:
+    conda: '>=4.8,<23.4'
+    libmambapy: 1.1.0 py310hb15139c_2
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 2bf0001c9bb77ded523219dd77549db1
+    sha256: 8bc81d851ab65e517a4a1d28be3c31993cd21e9a75ee49fce76872967b9a5965
+  manager: conda
+  name: mamba
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/mamba-1.1.0-py310h6bde348_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9,<0.13.0'
+    cachy: '>=0.3.0,<0.4.0'
+    cleo: '>=0.8.1,<0.9.0'
+    clikit: '>=0.6.2,<0.7.0'
+    crashtest: '>=0.3.0,<0.4.0'
+    html5lib: '>=1.0,<2.0'
+    keyring: '>=21.2.0'
+    lockfile: '>=0.9'
+    packaging: '>=20.4,<21.0'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.4,<2.0'
+    poetry-core: '>=1.0.7,<1.1.0'
+    ptyprocess: '>=0.5'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<0.10.0'
+    shellingham: '>=1.1,<2.0'
+    tomlkit: '>=0.7.0,<1.0.0'
+    virtualenv: '>=20.0.26,<21.0.0'
+  hash:
+    md5: 7bc43495d162b6be9590ffe65422963f
+    sha256: 90fc5ab9dbbed1c1739d1fa5b1d26f4f6a87c1f56dee7178a18885433bde6f49
+  manager: conda
+  name: poetry
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/osx-64/poetry-1.1.14-py310h2ec42d9_0.tar.bz2
+  version: 1.1.14
+- category: main
+  dependencies: {}
+  hash:
+    md5: 5fba0abc60bf327a4bc4188cd64678be
+    sha256: 564f7c91d51b8b7b7111fd207bcbefe5c4f6c2075e41dc1b44725d974325ed90
+  manager: conda
+  name: ca-certificates
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.9.24-h5b45459_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies: {}
+  hash:
+    md5: 878f923dd6acc8aeb47a75da6c4098be
+    sha256: d4fb485b79b11042a16dc6abfb0c44c4f557707c2653ac47c81e5d32b24a3bb0
+  manager: conda
+  name: pybind11-abi
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2
+  version: '4'
+- category: main
+  dependencies: {}
+  hash:
+    md5: f4cfd883c0d91bb17164d8e34f4900d5
+    sha256: 8212c6f1a68d5a494bcde5cd64196626024059dcbe8995469c8a5ed32694efa0
+  manager: conda
+  name: python_abi
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-3_cp310.conda
+  version: '3.10'
+- category: main
+  dependencies: {}
+  hash:
+    md5: 51fc4fcfb19f5d95ffc8c339db5068e8
+    sha256: 0bfae0b9962bc0dbf79048f9175b913ed4f53c4310d06708dc7acbb290ad82f6
+  manager: conda
+  name: tzdata
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2022g-h191b570_0.conda
+  version: 2022g
+- category: main
+  dependencies: {}
+  hash:
+    md5: 72608f6cd3e5898229c3ea16deb1ac43
+    sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
+  manager: conda
+  name: ucrt
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+  version: 10.0.22621.0
+- category: main
+  dependencies:
+    ucrt: '>=10.0.20348.0'
+  hash:
+    md5: c98b6e39006315599b793592bcc3c978
+    sha256: 6b6feb349d3414655c2f9c549092689e5f99b487ff7ed9c1f1fda69a5dd4a624
+  manager: conda
+  name: vs2015_runtime
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.32.31332-h1d6e394_9.tar.bz2
+  version: 14.32.31332
+- category: main
+  dependencies:
+    vs2015_runtime: '>=14.32.31332'
+  hash:
+    md5: ba28983ef4f6d430827d0e7c5cdd7b48
+    sha256: 1ca9e60e4e977be81dbee0ed236c6fb0a459c32957d2c2dc45a114d83f4c70d6
+  manager: conda
+  name: vc
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h3d8a991_9.tar.bz2
+  version: '14.3'
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: 7c03c66026944073040cb19a4f3ec3c9
+    sha256: 5389dad4e73e4865bb485f460fc60b120bae74404003d457ecb1a62eb7abf0c1
+  manager: conda
+  name: bzip2
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies:
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30037'
+  hash:
+    md5: 31a20cf261b2bd0a76d670db1b3e6fa1
+    sha256: b4882f05294a46949cf4d15e4b2c50f29257b0d042d7d8184e4722b392d71193
+  manager: conda
+  name: fmt
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/fmt-9.1.0-h181d51b_0.tar.bz2
+  version: 9.1.0
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: 2c96d1b6915b408893f9472569dee135
+    sha256: 1951ab740f80660e9bc07d2ed3aefb874d78c107264fd810f24a1a6211d4b1a5
+  manager: conda
+  name: libffi
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+  version: 3.4.2
+- category: main
+  dependencies:
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: 050119977a86e4856f0416e2edcf81bb
+    sha256: 657c2a992c896475021a25faebd9ccfaa149c5d70c7dc824d4069784b686cea1
+  manager: conda
+  name: libiconv
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2
+  version: '1.17'
+- category: main
+  dependencies:
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 5e5a97795de72f8cc3baf3d9ea6327a2
+    sha256: 4e50b3d90a351c9d47d239d3f90fce4870df2526e4f7fef35203ab3276a6dfc9
+  manager: conda
+  name: libsqlite
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.40.0-hcfcfb64_0.tar.bz2
+  version: 3.40.0
+- category: main
+  dependencies:
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 0cc5c5cc64ee1637f37f8540a175854c
+    sha256: 184da12b4296088a47086f4e69e65eb5f8537a824ee3131d8076775e1d1ea767
+  manager: conda
+  name: libzlib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2
+  version: 1.2.13
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: d12763533276560a931c1bd3df1adf63
+    sha256: 1d4b25978dc5f158d235908f1fd541116e9db3f31229bda665c4d3ff6b3979f8
+  manager: conda
+  name: lz4-c
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.3-h8ffe710_1.tar.bz2
+  version: 1.9.3
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: d5cf4b7eaa52316f135eed9e8548ad57
+    sha256: ff064e34d3cad829f1e31f2d26125b61d20ba8d3771f8f5337069027b8e3fab4
+  manager: conda
+  name: lzo
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/lzo-2.10-he774522_1000.tar.bz2
+  version: '2.10'
+- category: main
+  dependencies:
+    ca-certificates: ''
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: e48b661f57b25ddf34996fa8b685182d
+    sha256: 3f26c38e6167d7351de5bdcf13d1456891c242711e689999c25e50e5898bb660
+  manager: conda
+  name: openssl
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.0.7-hcfcfb64_1.conda
+  version: 3.0.7
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: 843a3cd031e593c24b542206c3444a2b
+    sha256: 3aec1eebaa039abb4c5accd9df021193859a7b8855555d2bd0465972f55fdc45
+  manager: conda
+  name: reproc
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/reproc-14.2.3-h8ffe710_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies:
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: 902c57a6f2f2e0b837a004004cd2ca57
+    sha256: ff4522ccfed5453dd773a935cf034b307872eba6814aa2798bef1cd4cc5e67df
+  manager: conda
+  name: sqlite
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/sqlite-3.39.2-h8ffe710_0.tar.bz2
+  version: 3.39.2
+- category: main
+  dependencies:
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: c69a5047cc9291ae40afd4a1ad6f0c0f
+    sha256: 087795090a99a1d397ef1ed80b4a01fabfb0122efb141562c168e3c0a76edba6
+  manager: conda
+  name: tk
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2
+  version: 8.6.12
+- category: main
+  dependencies:
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: 515d77642eaa3639413c6b1bc3f94219
+    sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
+  manager: conda
+  name: xz
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+  version: 5.2.6
+- category: main
+  dependencies:
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: adbfb9f45d1004a26763652246a33764
+    sha256: 4e2246383003acbad9682c7c63178e2e715ad0eb84f03a8df1fbfba455dfedc5
+  manager: conda
+  name: yaml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
+  version: 0.2.5
+- category: main
+  dependencies:
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 27c8a78ba0cd18268cfc7b04c5512162
+    sha256: b26b8ea17d1f8146c66c1b7b6acec3c759c2207a2e691e69a2a7cccdd2e1acae
+  manager: conda
+  name: yaml-cpp
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/yaml-cpp-0.7.0-h63175ca_2.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    openssl: '>=3.0.0,<4.0a0'
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: 729fcb13bda4bbd2dbc0c979dd16e677
+    sha256: 46ce0b65faad064a5be2fdc577b5ba8efac135adf2d410b67142fa922cfd6b71
+  manager: conda
+  name: krb5
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/krb5-1.19.3-hc8ab02b_0.tar.bz2
+  version: 1.19.3
+- category: main
+  dependencies:
+    libzlib: '>=1.2.11,<1.3.0a0'
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: f782e1756fd2c9b62931e95363e0205a
+    sha256: 975ecb6ce123df414075dc5018034ccc7dbf12a28f2e86b3ddf4639ff862aa82
+  manager: conda
+  name: libsolv
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libsolv-0.7.22-h7755175_0.tar.bz2
+  version: 0.7.22
+- category: main
+  dependencies:
+    libzlib: '>=1.2.12,<1.3.0a0'
+    openssl: '>=3.0.5,<4.0a0'
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: c2b344e960a173c777bb3ed172c38cd8
+    sha256: 93cc00b7ec3766d4313ff0795997a10745ce68f708811b2213a3655ca2c639b6
+  manager: conda
+  name: libssh2
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libssh2-1.10.0-h9a1e1f7_3.tar.bz2
+  version: 1.10.0
+- category: main
+  dependencies:
+    libiconv: '>=1.17,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 6dcf17bf780618ddb559d992ea3b6961
+    sha256: bba812f5c8c4b47c2b97aa8e66fa43f11a4be37d2d383d766890b30b2f28cdde
+  manager: conda
+  name: libxml2
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.10.3-hc3477c8_0.tar.bz2
+  version: 2.10.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libffi: '>=3.4,<4.0a0'
+    libsqlite: '>=3.40.0,<4.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+    tk: '>=8.6.12,<8.7.0a0'
+    tzdata: ''
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+    xz: '>=5.2.6,<6.0a0'
+  hash:
+    md5: 6a74ef0e5662397929214f2fb04c7d19
+    sha256: 7c05da8180e62ebdf6e5af72fd1605df79395b11b0d0653788b828f6e1a6649e
+  manager: conda
+  name: python
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.10.8-h4de0772_0_cpython.conda
+  version: 3.10.8
+- category: main
+  dependencies:
+    reproc: 14.2.3 h8ffe710_0
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: 534e8626893c41ed3b08bbba07396ca3
+    sha256: 94bd2036942929d6a128fe49e8af34d572a9ce06946d5b8b387fab6d42201c26
+  manager: conda
+  name: reproc-cpp
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/reproc-cpp-14.2.3-h0e60522_0.tar.bz2
+  version: 14.2.3
+- category: main
+  dependencies:
+    libzlib: 1.2.12 h8ffe710_2
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: d6f4eeb62da2ad90c31082cc7178776a
+    sha256: a1a4c6997ba96debd345d5d3fdf6109340ce4bf08c25d86e3db33b08e371937d
+  manager: conda
+  name: zlib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/zlib-1.2.12-h8ffe710_2.tar.bz2
+  version: 1.2.12
+- category: main
+  dependencies:
+    libzlib: '>=1.2.12,<1.3.0a0'
+    ucrt: ''
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+  hash:
+    md5: 13acb3626fcc8c0577249f3a7b6129f4
+    sha256: 109f83494b8bc82d1c41eea92a3cf8303a151674b623df08cc85ca54061cb008
+  manager: conda
+  name: zstd
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h7755175_4.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 5dfee17f24e2dfd18d7392b48c9351e2
+    sha256: 9b193a4e483c4d0004bc5b88fac7a02516b6311137ab61b8db85aa9741422e35
+  manager: conda
+  name: cachy
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2
+  version: 0.3.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: f66309b099374af91369e67e84af397d
+    sha256: 52e7459b3c457e888e2b6a4e6d13ab7f8675999bc12d20a83e34f12591a8771a
+  manager: conda
+  name: certifi
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2
+  version: 2022.9.24
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c1d5b294fbf9a795dec349a6f4d8be8e
+    sha256: 9e6170fa7b65b5546377eddb602d5ff871110f84bebf101b7b8177ff64aab1cb
+  manager: conda
+  name: charset-normalizer
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 3faab06a954c2a04039983f2c4a50d99
+    sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
+  manager: conda
+  name: colorama
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.6
+- category: main
+  dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: b8477552274c1cfdb533e954c76523f1
+    sha256: af1db267e03c649aefcc1571ddce4eac361a0e5232d1bdd05fd93fadbfdd2da6
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.1
+- category: main
+  dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: b65b4d50dbd2d50fa0aeac367ec9eed7
+    sha256: 06eb7167d4d760b3b437a491e32ab5b3f89e2a18f023c117fe213b038d88538a
+  manager: conda
+  name: distlib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2
+  version: 0.3.6
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 88111d95b12d83681d0ecdbbc24eee8e
+    sha256: 6b40f145b1fdf6b45016d29f193a8ca72a9359ea44cc19624901248f7a9b5ba7
+  manager: conda
+  name: docutils
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py310h5588dad_1.tar.bz2
+  version: '0.19'
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0f09c2bc17ddd8732be8e5b99297c7ce
+    sha256: 29cb48ad4a0e2633968c1c4d7cab8aabcce8f435cf3bf11b2d2599e3e978c531
+  manager: conda
+  name: filelock
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.2-pyhd8ed1ab_0.conda
+  version: 3.8.2
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 6d5e56de2e65da7aa35fd10131226efa
+    sha256: 251e79241eadab363eeaaf20f118423571e1a90ef351ae78e1c4574c53c8526c
+  manager: conda
+  name: flit-core
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 34272b248891bddccc64479f9a7fffed
+    sha256: 9887c35c374ec1847f167292d3fde023cb4c994a4ceeec283072b95440131f09
+  manager: conda
+  name: idna
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2
+  version: '3.4'
+- category: main
+  dependencies:
+    python: 2.7|>=3.4
+  hash:
+    md5: 25045ddd7fe83ddf71c181d6212e9913
+    sha256: 32421934e708a48d38927eb690dcf7c26856b437b43ca3b7182bb089edaa68af
+  manager: conda
+  name: invoke
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/invoke-1.7.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.7.3
+- category: main
+  dependencies:
+    bzip2: '>=1.0.8,<2.0a0'
+    libxml2: '>=2.9.14,<2.11.0a0'
+    libzlib: '>=1.2.12,<1.3.0a0'
+    lz4-c: '>=1.9.3,<1.10.0a0'
+    lzo: '>=2.10,<3.0a0'
+    openssl: '>=3.0.3,<4.0a0'
+    vc: '>=14.1,<15'
+    vs2015_runtime: '>=14.16.27033'
+    xz: '>=5.2.5,<5.3.0a0'
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 96f14843ac68b6d49d376b2c76018c1a
+    sha256: 10f045b5c74aed06ef090fb898f67ad0d8fc597fd2ff7563c55089a0b1edf054
+  manager: conda
+  name: libarchive
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libarchive-3.5.2-habf0b7a_3.tar.bz2
+  version: 3.5.2
+- category: main
+  dependencies:
+    krb5: '>=1.19.3,<1.20.0a0'
+    libssh2: '>=1.10.0,<2.0a0'
+    libzlib: '>=1.2.13,<1.3.0a0'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: d5fc1cba559c9889332ffb2a39001704
+    sha256: 3c2edc12356b57aeb0d9ba11f273196b99862680bc7cec58f8b69f25cf4ab1b1
+  manager: conda
+  name: libcurl
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libcurl-7.86.0-heaf79c2_1.tar.bz2
+  version: 7.86.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 24e57be449c71b8edc52cc6a48ff846d
+    sha256: 76576c5fd2a6ad1e987b3df4bba55dab05c0f4f35e4f54c6ddbb9559aaf01537
+  manager: conda
+  name: markupsafe
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py310h8d17308_2.tar.bz2
+  version: 2.1.1
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 15cfc917187d7c173647dd65d340259b
+    sha256: 606f9ed8839ba6ba1926ecf1a99cde0e8f02f47cb8d657a390ae13872e019efa
+  manager: conda
+  name: menuinst
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/menuinst-1.4.19-py310h5588dad_1.tar.bz2
+  version: 1.4.19
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 9b6ad26944f19f599800b068e0582227
+    sha256: 9b13d47aab2ee2708157bf90244915652b9d2ceaee9952694cfd5caff3559fbc
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 9.0.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 037a60d74aadd3a2f10e1e9580a42a9b
+    sha256: 9f44cff2cd152db18ef4b8101b6fdb72a8616c80bace71dfff8f248dc0dafe05
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.4-py310h232114e_1.tar.bz2
+  version: 1.0.4
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: a4eea5bff523f26442405bc5d1f52adb
+    sha256: 9153f0f38c76a09da7688a61fdbf8f3d7504e2326bef53e4ec20d994311b15bd
+  manager: conda
+  name: pastel
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.2.1
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 8fb2779f1ab2ce91e893f31a36fbcbfa
+    sha256: 2327e1afee1ccd981a4ff1c3eae0d1a649590e3445ad47db0127d87f0d2861f1
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.2-pyhd8ed1ab_0.conda
+  version: 1.9.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2fb3f88922e7aec26ba652fcdfe13950
+    sha256: a46843e317318405a8c66b640e7ad0c95d2f536918faa4f36cdfcda852000bcd
+  manager: conda
+  name: platformdirs
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2
+  version: 2.5.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: a15f6e219a4f2b73bccf2210e0f63364
+    sha256: 03951bb41e1e4daa128d2a3fda23643d20174eddf5af6c9badaa317b21ea2583
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/poetry-core-1.0.8-py310h5588dad_1.tar.bz2
+  version: 1.0.8
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 359eeb6536da0e687af562ed265ec263
+    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
+  manager: conda
+  name: ptyprocess
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 3324f50e5d46a04309d8f8f956c17244
+    sha256: 2e74d789ff6846181bd7e32260b9c0d57b91d4fcc0311274fca4279f8a35b048
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pycosat-0.6.4-py310h8d17308_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
+    python: 2.7.*|>=3.4
+  hash:
+    md5: 076becd9e05608f8dc72757d5f3a91ff
+    sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
+  manager: conda
+  name: pycparser
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2
+  version: '2.21'
+- category: main
+  dependencies:
+    python: '>=3.3'
+  hash:
+    md5: edf8651c4379d9d1495ad6229622d150
+    sha256: 50bd91767686bfe769e50a5a1b883e238d944a6163fea43e7c0beaac54ca674f
+  manager: conda
+  name: pylev
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
+  manager: conda
+  name: pyparsing
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    vc: '>=14.1,<15.0a0'
+    vs2015_runtime: '>=14.16.27012'
+  hash:
+    md5: e034f495e69b266fc082c92f75398f22
+    sha256: 309c5992598de0424daab9bf20c6eb9909b1eed85bac4608b98a568ac0f41759
+  manager: conda
+  name: pywin32
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/pywin32-303-py310he2412df_0.tar.bz2
+  version: '303'
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 8fa9c1b03d838a262be611ca23003ebd
+    sha256: 7c5ad91c9b454b115d931e8bc5024221cf94b0232871ea89a3c1048f27f7c8a3
+  manager: conda
+  name: pywin32-ctypes
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.0-py310h5588dad_1006.tar.bz2
+  version: 0.2.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: d0daf3eed98dd2bf4337ed08d8011eb8
+    sha256: 7d948a99bf7af50c9823a248267fce75ac555e4f357de166f65a75fab8549f3c
+  manager: conda
+  name: pyyaml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310h8d17308_5.tar.bz2
+  version: '6.0'
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: b3ef8910b2d18259dbddaee0eb19ef9b
+    sha256: 31968149fcfcd4094936dd8e97ec46491c5bae47a2ccdb68f137d366cf423056
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py310h8d17308_0.tar.bz2
+  version: 0.2.7
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+    yaml: '>=0.2.5,<0.3.0a0'
+  hash:
+    md5: e4537a0116ce275dc510d04d68477060
+    sha256: 997d10b4eaecce80bc95ee5419135548e8e9484221d670d5a9c59f4ad89f5fed
+  manager: conda
+  name: ruamel_yaml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel_yaml-0.15.80-py310h8d17308_1008.tar.bz2
+  version: 0.15.80
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: cfb8dc4d9d285ca5fb1177b9dd450e33
+    sha256: 55521371cfbd1bc046c362a108f9b8e294c35604896757659c6fb6765b6955c2
+  manager: conda
+  name: setuptools
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 65.5.1
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 437655338696f9d0dfdb0a024e66b255
+    sha256: 7d79f4500b4267414a2bd6a08e74aedc1629feb890efec71b0480501d37f148a
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2
+  version: 1.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: e5f25f8dbc060e9a8d912e432202afc2
+    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
+  manager: conda
+  name: six
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+  version: 1.16.0
+- category: main
+  dependencies:
+    python: '>=2.7'
+  hash:
+    md5: f832c45a477c78bebd107098db465095
+    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
+  manager: conda
+  name: toml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+  version: 0.10.2
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 5844808ffab9ebdb694585b50ba02a96
+    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
+  manager: conda
+  name: tomli
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+  version: 2.0.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 73506d1ab4202481841c68c169b7ef6c
+    sha256: efb5f78a224c4bb14aab04690c9912256ea12c3a8b8413e60167573ce1282b02
+  manager: conda
+  name: tomli-w
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 2d93b130d148d7fc77e583677792fc6a
+    sha256: 70c57b5ac94cd32e78f1a2fa2c38572bfac85b901a6a99aa254a9e8e126c132d
+  manager: conda
+  name: typing_extensions
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    python: ''
+  hash:
+    md5: 3563be4c5611a44210d9ba0c16113136
+    sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
+  manager: conda
+  name: webencodings
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
+  version: 0.5.1
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: c829cfb8cb826acb9de0ac1a2df0a940
+    sha256: bd4f11ff075ff251ade9f57686f31473e25be46ab282d9603f551401250f9f44
+  manager: conda
+  name: wheel
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2
+  version: 0.38.4
+- category: main
+  dependencies:
+    __win: ''
+    python: '>=3.6'
+  hash:
+    md5: 30878ecc4bd36e8deeea1e3c151b2e0b
+    sha256: a11ae693a0645bf6c7b8a47bac030be9c0967d0b1924537b9ff7458e832c0511
+  manager: conda
+  name: win_inet_pton
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2
+  version: 1.1.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 09b5b885341697137879a4f039a9e5a1
+    sha256: d98e41fe62edde9d979d79114f8cffa992ca86f4e7428c75e3c8b8fd6ab040a3
+  manager: conda
+  name: zipp
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.11.0-pyhd8ed1ab_0.conda
+  version: 3.11.0
+- category: main
+  dependencies:
+    pycparser: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: ec6be66017eb91c9077abe15dcb19e75
+    sha256: bccfec5fbcaa255d0aa471933d1aaaf76f4a4070783e4e2b45b41c73df101af7
+  manager: conda
+  name: cffi
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_2.tar.bz2
+  version: 1.15.1
+- category: main
+  dependencies:
+    __win: ''
+    colorama: ''
+    python: '>=3.8'
+  hash:
+    md5: 6b58680207b526c42dcff68b543803dd
+    sha256: 84e80a33e9a8e5398d3e97209366b57f635462a5b894f8076ec8c95e56672c44
+  manager: conda
+  name: click
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2
+  version: 8.1.3
+- category: main
+  dependencies:
+    crashtest: '>=0.3.0,<0.4.0'
+    pastel: '>=0.2.0,<0.3.0'
+    pylev: '>=1.3,<2.0'
+    python: ''
+  hash:
+    md5: 159273f717a11e53b2656f8b6521a5e2
+    sha256: 59b5c9ea3415e45e1beb1c191e3a0bf0dcca92c200a184704ea55002d1ef535c
+  manager: conda
+  name: clikit
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyh9f0ad1d_0.tar.bz2
+  version: 0.6.2
+- category: main
+  dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
+    python: '>=3.8'
+    zipp: '>=0.5'
+  hash:
+    md5: 46a62e35b9ae515cf0e49afc7fe0e7ef
+    sha256: 6e5e45c3cc3ba9fc854cd80960d775ff6c042e1f0b1351ca2e294b1b9d987d8c
+  manager: conda
+  name: importlib-metadata
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.1.0-pyha770c72_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: 31e4a1506968d017229bdb64695013a1
+    sha256: 6a81b67a1de8f761f66a4540bbd07cc27f9fbf2c7d67aa3732ebef379cf62874
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 3.2.3
+- category: main
+  dependencies:
+    markupsafe: '>=2.0'
+    python: '>=3.7'
+  hash:
+    md5: c8490ed5c70966d232fdd389d0dbed37
+    sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
+  manager: conda
+  name: jinja2
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
+  version: 3.1.2
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libarchive: '>=3.5.2,<3.6.0a0'
+    libcurl: '>=7.86.0,<8.0a0'
+    libsolv: '>=0.7.22,<0.8.0a0'
+    openssl: '>=3.0.7,<4.0a0'
+    reproc-cpp: '>=14.2,<15.0a0'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: 672850850275c7f10001328b65ae297b
+    sha256: 379851f5d60f74e9f89aa6b571c3568e8d1ba860a9eb27ead9d0b7b776de4645
+  manager: conda
+  name: libmamba
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libmamba-1.1.0-hd18bbca_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    pyparsing: '>=2.0.2,!=3.0.5'
+    python: '>=3.6'
+  hash:
+    md5: 71f1ab2de48613876becddd496371c85
+    sha256: 8322a9e93e2e09fbf2103f0d37c9287b7b97387125abadd6db26686084893540
+  manager: conda
+  name: packaging
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2
+  version: '21.3'
+- category: main
+  dependencies:
+    ptyprocess: '>=0.5'
+    python: ''
+  hash:
+    md5: 5909e7b978141dd80d28dbf9de627827
+    sha256: 04eef875d461732ef22cd19bf2c989c40e73b5da625bf6a6b82ddae200e90e56
+  manager: conda
+  name: pexpect
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2
+  version: 4.8.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    setuptools: ''
+    wheel: ''
+  hash:
+    md5: da66f2851b9836d3a7c5190082a45f7d
+    sha256: 7a86b2427abbf5cf695da192ba1c03130115f157297e7bfde65f0a18a345a7bc
+  manager: conda
+  name: pip
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2
+  version: 22.3.1
+- category: main
+  dependencies:
+    __win: ''
+    python: '>=3.8'
+    win_inet_pton: ''
+  hash:
+    md5: 56cd9fe388baac0e90c7149cfac95b60
+    sha256: b3a612bc887f3dd0fb7c4199ad8e342bd148cf69a9b74fd9468a18cf2bef07b7
+  manager: conda
+  name: pysocks
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
+  version: 1.7.1
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 266f81ef89f0cfef72a628e236147f7f
+    sha256: 02480785e2b4fe91b6678d32f3aebbc23749622563f017feac0a83bfed0f3d8f
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.21-py310h8d17308_2.tar.bz2
+  version: 0.17.21
+- category: main
+  dependencies:
+    python: '>=3.6'
+    typing: '>=3.6,<4.0'
+  hash:
+    md5: 471bf9e605820b59988e830382b8d654
+    sha256: e8b3bc2203266636740ce10536ef951c52b53b43bfed3b938117547efc47e374
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.6-pyha770c72_0.tar.bz2
+  version: 0.11.6
+- category: main
+  dependencies:
+    colorama: ''
+    python: '>=2.7'
+  hash:
+    md5: 6642233f341e1900d0c8e6eddb979c14
+    sha256: 4a07828941e4bf8c8167c278e1999990b984055e49c794a81d9e76073191aaed
+  manager: conda
+  name: tqdm
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/tqdm-4.64.0-pyhd8ed1ab_0.tar.bz2
+  version: 4.64.0
+- category: main
+  dependencies:
+    typing_extensions: 4.4.0 pyha770c72_0
+  hash:
+    md5: be969210b61b897775a0de63cd9e9026
+    sha256: 6f129b1bc18d111dcf3abaec6fcf6cbee00f1b77bb42d0f0bc8d85f8faa65cf0
+  manager: conda
+  name: typing-extensions
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2
+  version: 4.4.0
+- category: main
+  dependencies:
+    distlib: '>=0.3.6,<1'
+    filelock: '>=3.4.1,<4'
+    platformdirs: '>=2.4,<3'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 6a22296594d9b77bcf1f962bed2f6a61
+    sha256: c07d8ac0c29e28d47c08d42834ed5d8a804fbc01e2886d9603be430c3bfd1702
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.17.0-py310h5588dad_0.conda
+  version: 20.17.0
+- category: main
+  dependencies:
+    cffi: '>=1.0.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 6cb010e0fa21d7b606a13038a89ccbc2
+    sha256: 2631b26d291196d76694bf7d71ea77ba2abcfc46278c3a54730a2d5683ca6c2b
+  manager: conda
+  name: brotlipy
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310h8d17308_1005.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
+    clikit: '>=0.6.0,<0.7.0'
+    python: '>=3.6'
+  hash:
+    md5: 4c82b11a3d06031bd58e7d869f53d965
+    sha256: a3a5beaf5b4a5ba671580164e6b1da77837f9d69414b095bd3231e84a85f505c
+  manager: conda
+  name: cleo
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/cleo-0.8.1-pyhd8ed1ab_2.tar.bz2
+  version: 0.8.1
+- category: main
+  dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
+    cffi: '>=1.12'
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 0e8b49bc425a99afa3c8d48776c6e6ed
+    sha256: 22930c11e3c44785cfc83f739bea5250bee34a078ee90f8840378a100d624aa4
+  manager: conda
+  name: cryptography
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-38.0.4-py310h6e82f81_0.conda
+  version: 38.0.4
+- category: main
+  dependencies:
+    importlib-metadata: '>=5.1.0,<5.1.1.0a0'
+  hash:
+    md5: 3dc2248927de739b4d2e2da9a9972bfe
+    sha256: 6f643ecc303fba87b1de661d63460624434fe98fd124f1f1306b7b27d4c8b050
+  manager: conda
+  name: importlib_metadata
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-5.1.0-hd8ed1ab_0.conda
+  version: 5.1.0
+- category: main
+  dependencies:
+    fmt: '>=9.1.0,<10.0a0'
+    libmamba: 1.1.0 hd18bbca_2
+    openssl: '>=3.0.7,<4.0a0'
+    pybind11-abi: '4'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+    yaml-cpp: '>=0.7.0,<0.8.0a0'
+  hash:
+    md5: d9976c2eb8ad85ed4a160da739242fba
+    sha256: 28082342d92ee056be62c11f2a0b31a6a1daf9ef06cef2d363fca5f68fadb21f
+  manager: conda
+  name: libmambapy
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.1.0-py310h3fe4c2e_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.1.0'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 675afeba3c75ece50ef5b1f22350a710
+    sha256: 393dc63fa4c61153e1685c05a2f9bd91562e66f131858d7e6d1a49c4538b6a00
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-1.10.2-py310h8d17308_1.tar.bz2
+  version: 1.10.2
+- category: main
+  dependencies:
+    cffi: '>=1.11'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 9ef29771ac801a8a1e132f2f67ccf5cc
+    sha256: 189ed4c35ef53c01c909aa9afa8ef654f9a9cee8725aa05f38fa138d57702cfa
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py310h0009e47_1.conda
+  version: 0.19.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 1a2fa9e53cfbc2e4d9ab21990805a436
+    sha256: 48cde99cc0abe5e50fb00713710851db9f76812a644892a9a2b5cbf9fe9707f5
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.7.0-pyhd8ed1ab_1.conda
+  version: 0.7.0
+- category: main
+  dependencies:
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    pywin32-ctypes: ''
+  hash:
+    md5: 9adbff9beec7edbee5e02836f7c0ad43
+    sha256: c0cee60a41b09bf39d648b1af75b0ec9b57252bd7be1812f786bb68168f58f23
+  manager: conda
+  name: keyring
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/keyring-23.11.0-py310h5588dad_0.tar.bz2
+  version: 23.11.0
+- category: main
+  dependencies:
+    cryptography: '>=38.0.0,<39'
+    python: '>=3.6'
+  hash:
+    md5: fbfa0a180d48c800f922a10a114a8632
+    sha256: 42f04dded77ac2597108378d62b121697d0e982aba7b20a462a7239030563628
+  manager: conda
+  name: pyopenssl
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2
+  version: 22.1.0
+- category: main
+  dependencies:
+    conda-package-streaming: '>=0.7.0'
+    python: '>=3.7'
+  hash:
+    md5: 44800e9bd13143292097c65e57323038
+    sha256: c453b2a648e7a059f26326d476069cf81627c9a3fa12da4ab22eb39e7bfdc095
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda
+  version: 2.0.2
+- category: main
+  dependencies:
+    brotlipy: '>=0.6.0'
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: <4.0
+  hash:
+    md5: 3078ef2359efd6ecadbc7e085c5e0592
+    sha256: 992f2d6ca50c98f865a4f2e4bada23f950e39f33ff7c64614a31ee152ec4d5ae
+  manager: conda
+  name: urllib3
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.13-pyhd8ed1ab_0.conda
+  version: 1.26.13
+- category: main
+  dependencies:
+    certifi: '>=2017.4.17'
+    charset-normalizer: '>=2,<3'
+    idna: '>=2.5,<4'
+    python: '>=3.7,<4.0'
+    urllib3: '>=1.21.1,<1.27'
+  hash:
+    md5: 089382ee0e2dc2eae33a04cc3c2bddb0
+    sha256: b45d0da6774c8231ab4fef0427b3050e7c54c84dfe453143dd4010999c89e050
+  manager: conda
+  name: requests
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2
+  version: 2.28.1
+- category: main
+  dependencies:
+    filelock: '>=3.8.0'
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: ''
+  hash:
+    md5: e4b40ac0d53e81ebf8892e3b3ca9c1cf
+    sha256: 9401cd2ef3cf7e70f154106686fe6c82bafc83ddd38f33c858eefd8a7734eefa
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.12-pyhd8ed1ab_1.tar.bz2
+  version: 0.12.12
+- category: main
+  dependencies:
+    conda-package-handling: '>=1.3.0'
+    menuinst: '>=1.4.11,<2'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.20.1,<3'
+    ruamel_yaml: '>=0.11.14,<0.17'
+    setuptools: '>=31.0.1'
+    toolz: '>=0.8.1'
+  hash:
+    md5: c69ac3dd1ebd4a6898f2b08f2639c1cc
+    sha256: bd7abec2f08e6e42e7dfe6446d8520401db98d1a1bcdc95b3f388dd6738e2885
+  manager: conda
+  name: conda
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/conda-22.9.0-py310h5588dad_2.tar.bz2
+  version: 22.9.0
+- category: main
+  dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
+    docutils: ''
+    flit-core: 3.8.0 pyhd8ed1ab_0
+    pip: ''
+    python: '>=3.6'
+    requests: ''
+    tomli-w: ''
+  hash:
+    md5: d37c34176396c5402cf80c32e67731b7
+    sha256: 5a09096b517adb83ee093b1f36a3af7b102bf86c3c80b3293f8141360f1bc402
+  manager: conda
+  name: flit
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/flit-3.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.8.0
+- category: main
+  dependencies:
+    python: ''
+    requests: '>=2.0.1,<=3.0.0'
+  hash:
+    md5: 402668adee8fcba9a9c265cdc2a88f5a
+    sha256: 1f2f3329127844be226bdc9bd9922d84a8767ae208d4a650c3ba655c84cb1e1c
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/noarch/requests-toolbelt-0.9.1-py_0.tar.bz2
+  version: 0.9.1
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9'
+    cachy: '>=0.3.0'
+    click: '>=8.0'
+    click-default-group: ''
+    clikit: '>=0.6.2'
+    crashtest: '>=0.3.0'
+    ensureconda: '>=1.3'
+    filelock: '>=3.8.0'
+    html5lib: '>=1.0'
+    importlib-metadata: '>=1.7.0'
+    jinja2: ''
+    keyring: '>=21.2.0'
+    packaging: '>=20.4'
+    pkginfo: '>=1.4'
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2.18'
+    ruamel.yaml: ''
+    tomli: ''
+    tomlkit: '>=0.7.0'
+    toolz: <1.0.0,>=0.12.0
+    typing-extensions: ''
+    virtualenv: '>=20.0.26'
+  hash:
+    md5: 7b1dde4760c5c554523fead6c2771af2
+    sha256: c259304878dc11109e8ee3c092b02115deeb4ce2545a722db96418b7082f32b9
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.2.1-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.1
+- category: main
+  dependencies:
+    conda: '>=4.8,<23.4'
+    libmambapy: 1.1.0 py310h3fe4c2e_2
+    openssl: '>=3.0.7,<4.0a0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: a61405ee533eff515ef5848ea77efac5
+    sha256: d14f3a2de4510ae24ac61084a83c325abf15b98a91e6e43e786579b6a1a82ef0
+  manager: conda
+  name: mamba
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/mamba-1.1.0-py310hd9d798f_2.conda
+  version: 1.1.0
+- category: main
+  dependencies:
+    cachecontrol: '>=0.12.9,<0.13.0'
+    cachy: '>=0.3.0,<0.4.0'
+    cleo: '>=0.8.1,<0.9.0'
+    clikit: '>=0.6.2,<0.7.0'
+    crashtest: '>=0.3.0,<0.4.0'
+    html5lib: '>=1.0,<2.0'
+    keyring: '>=21.2.0'
+    lockfile: '>=0.9'
+    packaging: '>=20.4,<21.0'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.4,<2.0'
+    poetry-core: '>=1.0.7,<1.1.0'
+    ptyprocess: '>=0.5'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<0.10.0'
+    shellingham: '>=1.1,<2.0'
+    tomlkit: '>=0.7.0,<1.0.0'
+    virtualenv: '>=20.0.26,<21.0.0'
+  hash:
+    md5: 0e9febdede429556c039b685d779fdc1
+    sha256: 31d83812fd55331e82ef4655fc72ddfe000fa9a03de5fb374a54a5c4a560d7f7
+  manager: conda
+  name: poetry
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/t/<TOKEN>/conda-forge/win-64/poetry-1.1.14-py310h5588dad_0.tar.bz2
+  version: 1.1.14
+version: 1
```

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/README.txt` & `lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/README.txt`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/links.csv` & `lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/links.csv`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/movies.csv` & `lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/movies.csv`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/ratings.csv` & `lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/ratings.csv`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/tags.csv` & `lenskit_build_helpers-0.3.0/lkbuild/data/ml-latest-small/tags.csv`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/datasets.py` & `lenskit_build_helpers-0.3.0/lkbuild/datasets.py`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/env.py` & `lenskit_build_helpers-0.3.0/lkbuild/env.py`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/lkbuild/tasks.py` & `lenskit_build_helpers-0.3.0/lkbuild/tasks.py`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/pyproject.toml` & `lenskit_build_helpers-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 readme = "README.md"
 license = { file = "LICENSE.md" }
 requires-python = ">= 3.7"
 dynamic = ['version', 'description']
 dependencies = [
     "flit >=3.2,<4",
     "requests ==2.*",
-    "invoke ==1.*",
+    "invoke ==2.*",
     "pip",
     "conda-lock >=1.2.1",
 ]
 
 [project.scripts]
 lkbuild = "lkbuild:lkbuild_main"
```

### Comparing `lenskit-build-helpers-0.2.0/tasks.py` & `lenskit_build_helpers-0.3.0/tasks.py`

 * *Files identical despite different names*

### Comparing `lenskit-build-helpers-0.2.0/PKG-INFO` & `lenskit_build_helpers-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lenskit-build-helpers
-Version: 0.2.0
+Version: 0.3.0
 Summary: LensKit build support helpers.
 Author-email: Michael Ekstrand <michaelekstrand@boisestate.edu>
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Requires-Dist: flit >=3.2,<4
 Requires-Dist: requests ==2.*
-Requires-Dist: invoke ==1.*
+Requires-Dist: invoke ==2.*
 Requires-Dist: pip
 Requires-Dist: conda-lock >=1.2.1
 
 # LensKit build support code
 
 This repository provides support code for use in LensKit builds and development.  If you are trying to
 use LensKit, you don't need it; it is only used for working on developing LensKit (and related packages).
```

