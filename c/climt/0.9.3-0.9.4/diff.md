# Comparing `tmp/climt-0.9.3.tar.gz` & `tmp/climt-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/climt-0.9.3.tar", last modified: Tue Mar 27 11:10:57 2018, max compression
+gzip compressed data, was "dist/climt-0.9.4.tar", last modified: Thu Mar 29 11:11:36 2018, max compression
```

## Comparing `climt-0.9.3.tar` & `climt-0.9.4.tar`

### file list

```diff
@@ -1,280 +1,281 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2018-03-27 11:05:26.000000 climt-0.9.3/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2632 2018-03-27 11:05:26.000000 climt-0.9.3/docs/component_types.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2018-03-27 11:05:26.000000 climt-0.9.3/docs/naming.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      395 2018-03-27 11:05:26.000000 climt-0.9.3/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6758 2018-03-27 11:05:26.000000 climt-0.9.3/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2018-03-27 11:05:26.000000 climt-0.9.3/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      529 2018-03-27 11:05:26.000000 climt-0.9.3/docs/utilities.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2018-03-27 11:05:26.000000 climt-0.9.3/docs/initialisation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2018-03-27 11:05:26.000000 climt-0.9.3/docs/climt.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2018-03-27 11:05:26.000000 climt-0.9.3/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3300 2018-03-27 11:05:26.000000 climt-0.9.3/docs/memory_management.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5528 2018-03-27 11:05:26.000000 climt-0.9.3/docs/configuration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2854 2018-03-27 11:05:26.000000 climt-0.9.3/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2134 2018-03-27 11:05:26.000000 climt-0.9.3/docs/quickstart.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6457 2018-03-27 11:05:26.000000 climt-0.9.3/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2018-03-27 11:05:26.000000 climt-0.9.3/docs/introduction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2018-03-27 11:05:26.000000 climt-0.9.3/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2018-03-27 11:05:26.000000 climt-0.9.3/docs/components.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2018-03-27 11:05:26.000000 climt-0.9.3/docs/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2018-03-27 11:05:26.000000 climt-0.9.3/docs/realistic.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6213 2018-03-27 11:05:26.000000 climt-0.9.3/docs/interaction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9132 2018-03-27 11:05:26.000000 climt-0.9.3/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3672 2018-03-27 11:05:26.000000 climt-0.9.3/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8421 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9186 2018-03-27 11:10:57.000000 climt-0.9.3/climt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8131 2018-03-27 11:05:26.000000 climt-0.9.3/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2687 2018-03-27 11:05:26.000000 climt-0.9.3/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      405 2018-03-27 11:05:26.000000 climt-0.9.3/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1510 2018-03-27 11:05:26.000000 climt-0.9.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2018-03-27 11:10:57.000000 climt-0.9.3/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/tests/cached_component_output/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetSeaIce-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGridScaleCondensation-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)  7349464 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGFSDycore-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     4404 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSimplePhysics-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSlabSurface-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithClouds-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolation-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      728 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestFrierson06LongwaveOpticalDepth-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSlabSurface-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheet-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheet-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestHeldSuarezCachedCoordinates-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetLand-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwave-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithClouds-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestEmanuel-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestHeldSuarezCachedCoordinates-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetLandIce-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGrayLongwaveRadiation-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGFSDycore-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestInstellation-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetSeaIce-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGrayLongwaveRadiation-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolationDifferentTime-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)  7349464 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGFSDycoreWithPrognostic-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolationWithSolarConstant-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     4772 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestDcmip-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetLand-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      888 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSimplePhysicsPrognostic-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestHeldSuarez-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     4916 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSimplePhysicsPrognostic-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestHeldSuarez-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGShortwave-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestIceSheetLandIce-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwave-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     7540 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestRRTMGShortwave-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     4552 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestEmanuel-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)      888 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestSimplePhysics-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1224 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGridScaleCondensation-0.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)  2996564 2018-03-27 11:05:26.000000 climt-0.9.3/tests/cached_component_output/TestGFSDycoreWithPrognostic-1.cache
--rw-rw-r--   0 travis    (2000) travis    (2000)    31892 2018-03-27 11:05:26.000000 climt-0.9.3/tests/test_components.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2018-03-27 11:05:26.000000 climt-0.9.3/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2996 2018-03-27 11:05:26.000000 climt-0.9.3/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4424 2018-03-27 11:05:26.000000 climt-0.9.3/tests/test_classes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4972 2018-03-27 11:05:26.000000 climt-0.9.3/tests/test_arrays.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11196 2018-03-27 11:05:26.000000 climt-0.9.3/tests/test_initialization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      668 2018-03-27 11:05:26.000000 climt-0.9.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     8421 2018-03-27 11:10:57.000000 climt-0.9.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5184 2018-03-27 11:05:26.000000 climt-0.9.3/CONTRIBUTING.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_data/ozone_profile.npy
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_core/
--rw-rw-r--   0 travis    (2000) travis    (2000)      912 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_core/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29906 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_core/initialization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      936 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4918 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_core/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23644 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_core/climt_components.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2018-03-27 11:05:26.000000 climt-0.9.3/climt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/GFS/
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/driver.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      795 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/Makefile.conf.gfortran
--rw-rw-r--   0 travis    (2000) travis    (2000)    11550 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/params.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      733 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/Makefile.conf.ifort
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/init.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    16693 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/run.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/spectral_data.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_finalize_stub.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     5168 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/pressure_data.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/dyn_finalize.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    16323 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/shtns.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     4604 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/kinds.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      795 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/Makefile.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)     4878 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/physcons.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    26494 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/dyn_run.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    13213 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/dyn_init.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      506 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/finalize.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_init.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/gfs_namelist
--rw-rw-r--   0 travis    (2000) travis    (2000)     2667 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_data_stub.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_finalize.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    11077 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/semimp_data.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_init_stub.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_run_hs.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2667 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_data.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/grid_data.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_run.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      725 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/GFS/phy_run_stub.f90
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/simple_physics/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23713 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/simple_physics/simple_physics_v5_1.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/simple_physics/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    26846 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/simple_physics/simple_physics_custom.f90
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/dcmip/
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/dcmip/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    11057 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_5_v1.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    47792 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_1_2_3_v5.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    21382 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_4_v3.f90
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/rrtmg_lw/
--rw-rw-r--   0 travis    (2000) travis    (2000)  4311641 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_k_g.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2222 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg01.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg07.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2921 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35611 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmr.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2440 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg11.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg04.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    44318 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_read_nc.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    13817 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_cldprop.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     6457 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/_rrtm_lw.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_wvn.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    27187 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/mcica_subcol_gen_lw.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)   127134 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_taumol.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)   110455 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_init.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     4683 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/parrrtm.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg12.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    13016 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_cldprmc.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      988 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/parkind.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_tbl.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg15.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1773 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_ncpar.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2338 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg05.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      995 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_cld.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2240 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg06.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)   140141 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_setcoef.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg02.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     3096 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg08.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg16.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    27582 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmc.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg10.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg09.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    50320 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rad.nomcica.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2308 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg03.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_ref.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg13.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    50999 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rad.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_vsn.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2490 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_con.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    28016 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrn.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2193 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg14.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    16930 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_lw/mcica_random_numbers.f90
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/Linux/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-25 08:10:52.000000 climt-0.9.3/climt/_lib/Linux/.temp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4275 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/Darwin/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/Darwin/.temp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/emanuel/
--rw-rw-r--   0 travis    (2000) travis    (2000)    41790 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/emanuel/convect43c.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/emanuel/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/rrtmg_sw/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3886505 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_k_g.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    18516 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_cldprmc.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    29271 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/mcica_subcol_gen_sw.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2570 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg29.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2433 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg22.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2313 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg23.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2932 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_aer.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)      945 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_ref.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2524 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg20.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    30726 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_spcvmc.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2422 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg16.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    90964 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_rad.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_ncpar.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2166 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_wvn.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2296 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg27.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     7516 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_vrtqdr.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2316 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg25.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    12420 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_reftra.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2453 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg17.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    30533 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_spcvrt.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/parkind.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    12791 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/README
--rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_con.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2437 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg19.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2224 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg28.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2437 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg18.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_tbl.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     8005 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/_rrtm_sw.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)    19113 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_cldprop.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg21.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     4924 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/parrrsw.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)   197570 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_init.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1481 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_vsn.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    89470 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_rad.nomcica.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2262 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_cld.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    79141 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_taumol.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     1942 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg26.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    17277 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_setcoef.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg24.f90
--rw-rw-r--   0 travis    (2000) travis    (2000)    16891 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/rrtmg_sw/mcica_random_numbers.f90
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_lib/Windows/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_lib/Windows/.temp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8282 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/held_suarez.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/simple_physics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/simple_physics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9844 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/simple_physics/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7536 2018-03-27 11:07:05.000000 climt-0.9.3/climt/_components/simple_physics/_simple_physics.pyx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/second_best/
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/second_best/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8375 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/radiation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/dcmip/
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/dcmip/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4299 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/dcmip/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5072 2018-03-27 11:07:41.000000 climt-0.9.3/climt/_components/dcmip/_dcmip.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/slab_surface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4021 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/grid_scale_condensation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11346 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/_berger_solar_insolation.pyx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/gfs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/gfs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18843 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/gfs/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22079 2018-03-27 11:07:05.000000 climt-0.9.3/climt/_components/gfs/_gfs_dynamics.pyx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/emanuel/
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/emanuel/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12199 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/emanuel/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6852 2018-03-27 11:07:06.000000 climt-0.9.3/climt/_components/emanuel/_emanuel_convection.pyx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/instellation/
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/instellation/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/instellation/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4072 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/berger_solar_insolation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/rrtmg/
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/rrtmg/sw/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/sw/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18842 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/sw/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9216 2018-03-27 11:07:41.000000 climt-0.9.3/climt/_components/rrtmg/sw/_rrtmg_sw.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/rrtmg_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/rrtmg/lw/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/lw/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7391 2018-03-27 11:07:24.000000 climt-0.9.3/climt/_components/rrtmg/lw/_rrtmg_lw.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)    13649 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/rrtmg/lw/component.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-27 11:10:57.000000 climt-0.9.3/climt/_components/monitors/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/monitors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13585 2018-03-27 11:05:26.000000 climt-0.9.3/climt/_components/surface_ice.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2018-03-29 11:06:23.000000 climt-0.9.4/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2632 2018-03-29 11:06:23.000000 climt-0.9.4/docs/component_types.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2018-03-29 11:06:23.000000 climt-0.9.4/docs/naming.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      395 2018-03-29 11:06:23.000000 climt-0.9.4/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6758 2018-03-29 11:06:23.000000 climt-0.9.4/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2018-03-29 11:06:23.000000 climt-0.9.4/docs/authors.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      529 2018-03-29 11:06:23.000000 climt-0.9.4/docs/utilities.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2018-03-29 11:06:23.000000 climt-0.9.4/docs/initialisation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2018-03-29 11:06:23.000000 climt-0.9.4/docs/climt.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2018-03-29 11:06:23.000000 climt-0.9.4/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3300 2018-03-29 11:06:23.000000 climt-0.9.4/docs/memory_management.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5528 2018-03-29 11:06:23.000000 climt-0.9.4/docs/configuration.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2854 2018-03-29 11:06:23.000000 climt-0.9.4/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2134 2018-03-29 11:06:23.000000 climt-0.9.4/docs/quickstart.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6457 2018-03-29 11:06:23.000000 climt-0.9.4/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2018-03-29 11:06:23.000000 climt-0.9.4/docs/introduction.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2018-03-29 11:06:23.000000 climt-0.9.4/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2018-03-29 11:06:23.000000 climt-0.9.4/docs/components.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2018-03-29 11:06:23.000000 climt-0.9.4/docs/modules.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2018-03-29 11:06:23.000000 climt-0.9.4/docs/realistic.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6213 2018-03-29 11:06:23.000000 climt-0.9.4/docs/interaction.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9132 2018-03-29 11:06:23.000000 climt-0.9.4/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3672 2018-03-29 11:06:23.000000 climt-0.9.4/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       78 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8871 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9209 2018-03-29 11:11:36.000000 climt-0.9.4/climt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8131 2018-03-29 11:06:23.000000 climt-0.9.4/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2018-03-29 11:06:23.000000 climt-0.9.4/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      405 2018-03-29 11:06:23.000000 climt-0.9.4/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1510 2018-03-29 11:06:23.000000 climt-0.9.4/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2018-03-29 11:11:36.000000 climt-0.9.4/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/tests/cached_component_output/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetSeaIce-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      216 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGridScaleCondensation-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)  7349464 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestGFSDycore-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4404 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSimplePhysics-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSlabSurface-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithClouds-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolation-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      728 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestFrierson06LongwaveOpticalDepth-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      444 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSlabSurface-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheet-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheet-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1108 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestHeldSuarezCachedCoordinates-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetLand-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwave-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithClouds-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2344 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestEmanuel-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestHeldSuarezCachedCoordinates-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetLandIce-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGrayLongwaveRadiation-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestGFSDycore-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestInstellation-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetSeaIce-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGrayLongwaveRadiation-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolationDifferentTime-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)  7349464 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGFSDycoreWithPrognostic-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolationWithSolarConstant-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4772 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestDcmip-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetLand-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      888 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSimplePhysicsPrognostic-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1108 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestHeldSuarez-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4916 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSimplePhysicsPrognostic-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestHeldSuarez-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGShortwave-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5812 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestIceSheetLandIce-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7532 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwave-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7540 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestRRTMGShortwave-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4552 2018-03-29 11:06:23.000000 climt-0.9.4/tests/cached_component_output/TestEmanuel-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)      888 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestSimplePhysics-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1224 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGridScaleCondensation-0.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2996564 2018-03-29 11:06:24.000000 climt-0.9.4/tests/cached_component_output/TestGFSDycoreWithPrognostic-1.cache
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30006 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_components.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2018-03-29 11:06:23.000000 climt-0.9.4/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3689 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5224 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_classes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_wrappers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6007 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_arrays.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11395 2018-03-29 11:06:24.000000 climt-0.9.4/tests/test_initialization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      668 2018-03-29 11:06:23.000000 climt-0.9.4/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8871 2018-03-29 11:11:36.000000 climt-0.9.4/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5184 2018-03-29 11:06:23.000000 climt-0.9.4/CONTRIBUTING.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      320 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_data/ozone_profile.npy
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      912 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_core/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30134 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_core/initialization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      936 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_core/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4918 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_core/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24104 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_core/climt_components.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2018-03-29 11:06:23.000000 climt-0.9.4/climt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/GFS/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/driver.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/Makefile.conf.gfortran
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11550 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/params.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      733 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/Makefile.conf.ifort
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/init.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16693 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/run.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/spectral_data.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_finalize_stub.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5168 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/pressure_data.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2521 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/dyn_finalize.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16323 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/shtns.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4604 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/kinds.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/Makefile.conf
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4878 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/physcons.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26494 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/dyn_run.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13213 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/dyn_init.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      506 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/finalize.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      257 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_init.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/gfs_namelist
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2667 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_data_stub.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_finalize.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11077 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/semimp_data.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      257 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_init_stub.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_run_hs.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2667 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_data.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/grid_data.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_run.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      725 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/GFS/phy_run_stub.f90
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/simple_physics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23713 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/simple_physics/simple_physics_v5_1.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      358 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/simple_physics/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26846 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/simple_physics/simple_physics_custom.f90
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/dcmip/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/dcmip/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11057 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_5_v1.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47792 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_1_2_3_v5.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21382 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_4_v3.f90
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/rrtmg_lw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  4311641 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_k_g.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2222 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg01.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg07.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2921 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35611 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmr.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2440 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg11.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg04.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44318 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_read_nc.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13817 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_cldprop.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6457 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/_rrtm_lw.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_wvn.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27187 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/mcica_subcol_gen_lw.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)   127134 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_taumol.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110455 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_init.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4683 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/parrrtm.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg12.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13016 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_cldprmc.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      988 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/parkind.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_tbl.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg15.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1773 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_ncpar.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2338 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg05.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      995 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_cld.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2240 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg06.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)   140141 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_setcoef.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg02.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3096 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg08.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg16.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27582 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmc.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg10.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg09.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50320 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rad.nomcica.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2308 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg03.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_ref.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg13.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50999 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rad.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_vsn.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2490 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_con.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28016 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrn.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2193 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg14.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16930 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_lw/mcica_random_numbers.f90
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/Linux/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-25 08:10:52.000000 climt-0.9.4/climt/_lib/Linux/.temp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4275 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/Darwin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/Darwin/.temp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/emanuel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41790 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/emanuel/convect43c.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      242 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/emanuel/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/rrtmg_sw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3886505 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_k_g.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18516 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_cldprmc.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29271 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/mcica_subcol_gen_sw.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2570 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg29.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2433 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg22.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2313 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg23.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2932 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_aer.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)      945 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_ref.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2524 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg20.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30726 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_spcvmc.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2422 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg16.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90964 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_rad.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_ncpar.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2166 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_wvn.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2296 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg27.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7516 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_vrtqdr.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2316 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg25.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12420 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_reftra.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2453 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg17.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30533 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_spcvrt.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/parkind.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12791 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/README
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_con.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2437 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg19.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2224 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg28.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2437 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg18.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_tbl.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8005 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/_rrtm_sw.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19113 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_cldprop.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg21.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4924 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/parrrsw.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)   197570 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_init.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1481 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_vsn.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89470 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_rad.nomcica.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2262 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_cld.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79141 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_taumol.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1942 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg26.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17277 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_setcoef.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg24.f90
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16891 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/rrtmg_sw/mcica_random_numbers.f90
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_lib/Windows/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_lib/Windows/.temp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8282 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/held_suarez.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/simple_physics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/simple_physics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9881 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/simple_physics/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7536 2018-03-29 11:07:57.000000 climt-0.9.4/climt/_components/simple_physics/_simple_physics.pyx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/second_best/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/second_best/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8375 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/radiation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/dcmip/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/dcmip/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4299 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/dcmip/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5072 2018-03-29 11:08:29.000000 climt-0.9.4/climt/_components/dcmip/_dcmip.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/slab_surface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4021 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/grid_scale_condensation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      838 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11346 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/_berger_solar_insolation.pyx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/gfs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/gfs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18843 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/gfs/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22079 2018-03-29 11:07:57.000000 climt-0.9.4/climt/_components/gfs/_gfs_dynamics.pyx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/emanuel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/emanuel/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12199 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/emanuel/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6852 2018-03-29 11:07:58.000000 climt-0.9.4/climt/_components/emanuel/_emanuel_convection.pyx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/instellation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/instellation/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/instellation/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4072 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/berger_solar_insolation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/rrtmg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/rrtmg/sw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/sw/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18842 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/sw/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9216 2018-03-29 11:08:29.000000 climt-0.9.4/climt/_components/rrtmg/sw/_rrtmg_sw.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/rrtmg_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/rrtmg/lw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/lw/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7391 2018-03-29 11:08:14.000000 climt-0.9.4/climt/_components/rrtmg/lw/_rrtmg_lw.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13649 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/rrtmg/lw/component.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-03-29 11:11:36.000000 climt-0.9.4/climt/_components/monitors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/monitors/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13585 2018-03-29 11:06:23.000000 climt-0.9.4/climt/_components/surface_ice.py
```

### Comparing `climt-0.9.3/docs/component_types.rst` & `climt-0.9.4/docs/component_types.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/Makefile` & `climt-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/utilities.rst` & `climt-0.9.4/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/memory_management.rst` & `climt-0.9.4/docs/memory_management.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/configuration.rst` & `climt-0.9.4/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/installation.rst` & `climt-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/quickstart.rst` & `climt-0.9.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/make.bat` & `climt-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/introduction.rst` & `climt-0.9.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/components.rst` & `climt-0.9.4/docs/components.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/realistic.rst` & `climt-0.9.4/docs/realistic.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/interaction.rst` & `climt-0.9.4/docs/interaction.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/docs/conf.py` & `climt-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/README.rst` & `climt-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt.egg-info/PKG-INFO` & `climt-0.9.4/climt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: climt
-Version: 0.9.3
+Version: 0.9.4
 Summary: CliMT is a Toolkit for building Earth system models in Python.
 Home-page: https://github.com/CliMT/climt
 Author: Rodrigo Caballero
 Author-email: rodrigo.caballero@misu.su.se
 License: BSD license
 Description: =====
         CliMT
@@ -96,14 +96,28 @@
         .. _documentation: http://climt.readthedocs.io/en/latest/installation.html
         
         
         =======
         History
         =======
         
+        v.0.9.4
+        -------
+        
+        * Added attributes to inputs/outputs/ etc., to work with ScalingWrapper
+          Added tests as well.
+        * Added tests for constants functions
+        * Fixed requirements to ensure this version of climt installs
+          the correct versions of sympl and numpy.
+        
+        v.0.9.3
+        -------
+        
+        * Released because of a labelling issue. See 0.9.2 for details.
+        
         v.0.9.2
         --------
         * Updated documentation
         * Cleaned up examples
         * Added (*)_properties as a property to all components
         * The gas constant for dry air in the Emanuel scheme is now renamed _Rdair
         * RRTMG LW and SW are now OpenMP parallel
```

### Comparing `climt-0.9.3/climt.egg-info/SOURCES.txt` & `climt-0.9.4/climt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 docs/utilities.rst
 tests/__init__.py
 tests/test_arrays.py
 tests/test_classes.py
 tests/test_components.py
 tests/test_initialization.py
 tests/test_utils.py
+tests/test_wrappers.py
 tests/cached_component_output/TestBergerSolarInsolation-0.cache
 tests/cached_component_output/TestBergerSolarInsolationDifferentTime-0.cache
 tests/cached_component_output/TestBergerSolarInsolationWithSolarConstant-0.cache
 tests/cached_component_output/TestDcmip-0.cache
 tests/cached_component_output/TestEmanuel-0.cache
 tests/cached_component_output/TestEmanuel-1.cache
 tests/cached_component_output/TestFrierson06LongwaveOpticalDepth-0.cache
```

### Comparing `climt-0.9.3/setup.py` & `climt-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-    'numpy>=1.10',
+    'numpy>=0.10',
     'pint>=0.7.0',
     'xarray>=0.8.0',
-    'sympl>=0.2.1',
+    'sympl==0.3.2',
     'cython>=0.25',
     'scipy>=0.18.1',
 ]
 
 test_requirements = [
     'pytest>=2.9.2',
     'mock>=2.0.0',
@@ -221,15 +221,15 @@
             extra_compile_args=default_compile_args,
             library_dirs=[lib_path],
             extra_link_args=[lib_path+'/libdcmip.a'] + default_link_args),
     ]
 
 setup(
     name='climt',
-    version='0.9.3',
+    version='0.9.4',
     description='CliMT is a Toolkit for building Earth system models in Python.',
     long_description=readme + '\n\n' + history,
     author="Rodrigo Caballero",
     author_email='rodrigo.caballero@misu.su.se',
     url='https://github.com/CliMT/climt',
     packages=[
         'climt',
```

### Comparing `climt-0.9.3/HISTORY.rst` & `climt-0.9.4/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 =======
 History
 =======
 
+v.0.9.4
+-------
+
+* Added attributes to inputs/outputs/ etc., to work with ScalingWrapper
+  Added tests as well.
+* Added tests for constants functions
+* Fixed requirements to ensure this version of climt installs
+  the correct versions of sympl and numpy.
+
+v.0.9.3
+-------
+
+* Released because of a labelling issue. See 0.9.2 for details.
+
 v.0.9.2
 --------
 * Updated documentation
 * Cleaned up examples
 * Added (*)_properties as a property to all components
 * The gas constant for dry air in the Emanuel scheme is now renamed _Rdair
 * RRTMG LW and SW are now OpenMP parallel
```

### Comparing `climt-0.9.3/LICENSE` & `climt-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetSeaIce-0.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetSeaIce-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGFSDycore-0.cache` & `climt-0.9.4/tests/cached_component_output/TestGFSDycore-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestSimplePhysics-1.cache` & `climt-0.9.4/tests/cached_component_output/TestSimplePhysics-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithClouds-1.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithClouds-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolation-0.cache` & `climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolation-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestFrierson06LongwaveOpticalDepth-0.cache` & `climt-0.9.4/tests/cached_component_output/TestFrierson06LongwaveOpticalDepth-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheet-0.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheet-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheet-1.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheet-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetLand-1.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetLand-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-1.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwave-0.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwave-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithClouds-0.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithClouds-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestEmanuel-1.cache` & `climt-0.9.4/tests/cached_component_output/TestEmanuel-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetLandIce-1.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetLandIce-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGrayLongwaveRadiation-1.cache` & `climt-0.9.4/tests/cached_component_output/TestGrayLongwaveRadiation-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestInstellation-0.cache` & `climt-0.9.4/tests/cached_component_output/TestInstellation-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetSeaIce-1.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetSeaIce-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGrayLongwaveRadiation-0.cache` & `climt-0.9.4/tests/cached_component_output/TestGrayLongwaveRadiation-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolationDifferentTime-0.cache` & `climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolationDifferentTime-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGFSDycoreWithPrognostic-0.cache` & `climt-0.9.4/tests/cached_component_output/TestGFSDycoreWithPrognostic-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestBergerSolarInsolationWithSolarConstant-0.cache` & `climt-0.9.4/tests/cached_component_output/TestBergerSolarInsolationWithSolarConstant-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestDcmip-0.cache` & `climt-0.9.4/tests/cached_component_output/TestDcmip-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetLand-0.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetLand-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestSimplePhysicsPrognostic-1.cache` & `climt-0.9.4/tests/cached_component_output/TestSimplePhysicsPrognostic-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestSimplePhysicsPrognostic-0.cache` & `climt-0.9.4/tests/cached_component_output/TestSimplePhysicsPrognostic-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGShortwave-0.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGShortwave-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestIceSheetLandIce-0.cache` & `climt-0.9.4/tests/cached_component_output/TestIceSheetLandIce-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwave-1.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwave-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-0.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGLongwaveWithExternalInterfaceTemperature-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestRRTMGShortwave-1.cache` & `climt-0.9.4/tests/cached_component_output/TestRRTMGShortwave-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestEmanuel-0.cache` & `climt-0.9.4/tests/cached_component_output/TestEmanuel-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestSimplePhysics-0.cache` & `climt-0.9.4/tests/cached_component_output/TestSimplePhysics-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGridScaleCondensation-0.cache` & `climt-0.9.4/tests/cached_component_output/TestGridScaleCondensation-0.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/cached_component_output/TestGFSDycoreWithPrognostic-1.cache` & `climt-0.9.4/tests/cached_component_output/TestGFSDycoreWithPrognostic-1.cache`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/tests/test_components.py` & `climt-0.9.4/tests/test_components.py`

 * *Files 15% similar despite different names*

```diff
@@ -225,63 +225,26 @@
     for key in cached.keys():
         assert key in current.keys()
 
 
 class TestHeldSuarez(ComponentBase):
 
     def get_3d_input_state(self):
-        random = np.random.RandomState(0)
-        return {
-            'latitude': DataArray(
-                random.randn(3), dims=['latitude'], attrs={'units': 'degrees_N'}),
-            'air_pressure': DataArray(
-                random.rand(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'hPa'},),
-            'surface_air_pressure': DataArray(
-                random.rand(2, 3), dims=['longitude', 'latitude'],
-                attrs={'units': 'hPa'},),
-            'air_temperature': DataArray(
-                270. + random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'degK'}),
-            'eastward_wind': DataArray(
-                random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'm/s'}),
-            'northward_wind': DataArray(
-                random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'm/s'}),
-        }
+        hs = self.get_component_instance()
+        return climt.get_default_state([hs])
 
     def get_component_instance(self, state_modification_func=lambda x: x):
         return HeldSuarez()
 
 
 class TestHeldSuarezCachedCoordinates(ComponentBase):
 
     def get_3d_input_state(self):
-        random = np.random.RandomState(0)
-        return {
-            'latitude': DataArray(
-                np.linspace(-90, 90, num=3),
-                dims=['latitude'], attrs={'units': 'degrees_N'}),
-            'air_pressure': DataArray(
-                random.rand(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'hPa'},),
-            'surface_air_pressure': DataArray(
-                random.rand(2, 3), dims=['longitude', 'latitude'],
-                attrs={'units': 'hPa'},),
-            'air_temperature': DataArray(
-                270. + random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'degK'}),
-            'eastward_wind': DataArray(
-                random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'm/s'}),
-            'northward_wind': DataArray(
-                random.randn(2, 3, 6), dims=['longitude', 'latitude', 'mid_levels'],
-                attrs={'units': 'm/s'}),
-        }
+        hs = self.get_component_instance()
+        return climt.get_default_state([hs])
 
     def get_component_instance(self, state_modification_func=lambda x: x):
         return HeldSuarez()
 
     def test_1d_output_matches_cached_output(self):
         state = state_3d_to_1d(self.get_3d_input_state())
         component = self.get_component_instance()
```

### Comparing `climt-0.9.3/tests/test_utils.py` & `climt-0.9.4/tests/test_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 from climt import (
     mass_to_volume_mixing_ratio,
     get_interface_values,
     calculate_q_sat, numpy_version_of,
-    RRTMGShortwave, get_default_state)
+    RRTMGShortwave, get_default_state,
+    set_constants_from_dict, get_constant,
+    list_available_constants)
 
 from sympl import DataArray
 import numpy as np
 import pytest
 
+sample_constants = dict(
+    constant_one=dict(
+        value=10.0,
+        units='J kg^-1 m^-2'),
+    constant_two=dict(
+        value=1.002,
+        units='J kg^-1'),
+    constant_three=dict(
+        value=1.024e6,
+        units='kg^-1'))
+
 
 def test_mol_weight_not_passed():
 
     with pytest.raises(ValueError) as excinfo:
         mass_to_volume_mixing_ratio(None)
 
     assert 'molecular weight' in str(excinfo.value)
@@ -107,9 +120,26 @@
     state['test_values'] = np.arange(100)
 
     raw_array = numpy_version_of(state)
 
     assert np.all(raw_array['test_values'] == np.arange(100))
 
 
+def test_adding_constant():
+
+    set_constants_from_dict(sample_constants)
+
+    for constant in sample_constants.keys():
+
+        constant_value = get_constant(constant,
+                                      sample_constants[constant]['units'])
+
+        assert constant_value == sample_constants[constant]['value']
+
+
+def test_print_constant():
+
+    list_available_constants()
+
+
 if __name__ == '__main__':
     pytest.main([__file__])
```

### Comparing `climt-0.9.3/tests/test_classes.py` & `climt-0.9.4/tests/test_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from climt import ClimtPrognostic, ClimtImplicit
+from climt import ClimtPrognostic, ClimtImplicit, ClimtSpectralDynamicalCore
 import numpy as np
 
 
 class MockPrognostic(ClimtPrognostic):
 
     _climt_inputs = {
         'air_temperature': 'degK',
@@ -169,14 +169,46 @@
     _climt_inputs = {
         'air_temperature': 'degK',
         'mole_fraction_of_oxygen_in_air': 'millimole/mole',
         'some_quantity': 'dimensionless',
     }
 
     _climt_diagnostics = {
+        'air_pressure': 'Pa',
+        'mass_content_of_cloud_liquid_water_in_atmosphere_layer': 'kg m^-2'
+    }
+
+    _climt_outputs = {
+        'air_temperature': 'degK',
+        'mole_fraction_of_oxygen_in_air': 'millimole/mole',
+    }
+
+    quantity_descriptions = {
+        'some_quantity': {
+            'dims': ['x', 'y', 'mid_levels'],
+            'units': 'dimensionless',
+            'default_value': 1.
+        }
+    }
+
+    def __init__(self):
+        return
+
+    def __call__(self, state):
+        return
+
+
+class MockDycoreWithAllAttributes(ClimtSpectralDynamicalCore):
+    _climt_inputs = {
+        'air_temperature': 'degK',
+        'mole_fraction_of_oxygen_in_air': 'millimole/mole',
+        'some_quantity': 'dimensionless',
+    }
+
+    _climt_diagnostics = {
         'air_pressure': 'Pa',
         'mass_content_of_cloud_liquid_water_in_atmosphere_layer': 'kg m^-2'
     }
 
     _climt_outputs = {
         'air_temperature': 'degK',
         'mole_fraction_of_oxygen_in_air': 'millimole/mole',
```

### Comparing `climt-0.9.3/tests/test_arrays.py` & `climt-0.9.4/tests/test_arrays.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import numpy as np
 
 from .test_classes import (
     MockPrognostic,
     MockPrognosticWithExtraQuantities,
     MockPrognosticWithExtraQuantitiesNotDefined,
     MockPrognosticWithAllAttributes,
-    MockImplicitWithAllAttributes
+    MockImplicitWithAllAttributes,
+    MockDycoreWithAllAttributes
 )
 
 
 def test_get_diagnostics():
 
     dummy = MockPrognosticWithAllAttributes()
     state = get_default_state([dummy])
@@ -53,23 +54,58 @@
 
     diag = dummy.create_state_dict_for('_climt_tendencies', state)
 
     for quantity in dummy.tendencies:
         assert quantity in diag
 
 
-def test_get_outputs():
+def test_get_outputs_and_diagnostics():
 
     dummy = MockImplicitWithAllAttributes()
     state = get_default_state([dummy])
 
-    diag = dummy.create_state_dict_for('_climt_outputs', state)
+    output = dummy.create_state_dict_for('_climt_outputs', state)
 
     for quantity in dummy.outputs:
+        assert quantity in output
+
+    diag = dummy.create_state_dict_for('_climt_diagnostics', state)
+
+    for quantity in dummy.diagnostics:
+        assert quantity in diag
+        assert quantity in dummy.diagnostic_properties
+
+
+def test_dycore_inputs_are_valid():
+
+    dummy = MockDycoreWithAllAttributes()
+    state = get_default_state([dummy])
+
+    for input in dummy.inputs:
+        if input not in ['x', 'y', 'mid_levels', 'interface_levels']:
+            assert input in state
+            assert input in dummy.input_properties
+
+
+def test_get_dycore_outputs_and_diagnostics():
+
+    dummy = MockDycoreWithAllAttributes()
+    state = get_default_state([dummy])
+
+    output = dummy.create_state_dict_for('_climt_outputs', state)
+
+    for quantity in dummy.outputs:
+        assert quantity in output
+
+    diag = dummy.create_state_dict_for('_climt_diagnostics', state)
+
+    for quantity in dummy.diagnostics:
         assert quantity in diag
+        assert quantity in dummy.diagnostic_properties
+
 
 
 def test_get_diagnostics_with_real_component_with_2d_coordinates():
     dummy = RRTMGLongwave()
     state = get_default_state([dummy],
                               x=dict(label='shore', values=np.random.randn(2, 2), units='km'),
                               y=dict(label='latitude', values=np.random.randn(2, 2), units='degrees east'))
@@ -86,15 +122,15 @@
 
 def test_extracting_arrays_from_real_component():
     dummy = RRTMGLongwave()
     state = get_default_state([dummy])
 
     arrays = dummy.get_numpy_arrays_from_state('_climt_inputs', state)
 
-    for quantity in dummy.inputs:
+    for quantity in dummy._climt_inputs.keys():
         units = dummy._climt_inputs[quantity]
         state_values = state[quantity].to_units(units).values
         assert np.all(arrays[quantity] == state_values)
 
 
 def test_inputs_is_not_dict():
```

### Comparing `climt-0.9.3/tests/test_initialization.py` & `climt-0.9.4/tests/test_initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import numpy as np
 import pytest
 from .test_classes import (MockPrognostic,
                            MockPrognosticWithExtraDimensions,
                            MockPrognosticWithExtraQuantities,
                            MockPrognosticWithMalformedExtraQuantities,
                            MockPrognosticWithExtraDimensionsAndSigmaLevels,
-                           MockPrognosticWithExtraDimensionsIn2d)
+                           MockPrognosticWithExtraDimensionsIn2d,
+                           MockImplicitWithAllAttributes)
 
 
 def test_no_components():
 
     with pytest.raises(ValueError) as excinfo:
         get_default_state([])
     assert 'at least one' in str(excinfo.value)
@@ -284,15 +285,15 @@
 
     assert state['y'].values.shape[0] == 3
     assert state['y'].values.shape[1] == 4
 
     assert np.all(state['x'].values == random_x_values)
     assert np.all(state['y'].values == random_y_values)
 
-    for quantity in dummy.inputs:
+    for quantity in dummy._climt_inputs.keys():
         assert 'shore' in state[quantity].coords
         assert 'latitude' in state[quantity].coords
         assert state[quantity].coords['shore'].units is 'km'
         assert state[quantity].coords['latitude'].units is 'degrees east'
 
 
 def test_2d_coordinates_wrong_shape():
@@ -311,9 +312,16 @@
     dummy = MockPrognosticWithExtraDimensionsIn2d()
 
     with pytest.raises(NotImplementedError) as excinfo:
         get_default_state([dummy])
     assert 'not yet supported' in str(excinfo.value)
 
 
+def test_create_implicit_diagnostics():
+
+    dummy = MockImplicitWithAllAttributes()
+
+    state = get_default_state([dummy])
+
+
 if __name__ == '__main__':
     pytest.main([__file__])
```

### Comparing `climt-0.9.3/MANIFEST.in` & `climt-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/PKG-INFO` & `climt-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: climt
-Version: 0.9.3
+Version: 0.9.4
 Summary: CliMT is a Toolkit for building Earth system models in Python.
 Home-page: https://github.com/CliMT/climt
 Author: Rodrigo Caballero
 Author-email: rodrigo.caballero@misu.su.se
 License: BSD license
 Description: =====
         CliMT
@@ -96,14 +96,28 @@
         .. _documentation: http://climt.readthedocs.io/en/latest/installation.html
         
         
         =======
         History
         =======
         
+        v.0.9.4
+        -------
+        
+        * Added attributes to inputs/outputs/ etc., to work with ScalingWrapper
+          Added tests as well.
+        * Added tests for constants functions
+        * Fixed requirements to ensure this version of climt installs
+          the correct versions of sympl and numpy.
+        
+        v.0.9.3
+        -------
+        
+        * Released because of a labelling issue. See 0.9.2 for details.
+        
         v.0.9.2
         --------
         * Updated documentation
         * Cleaned up examples
         * Added (*)_properties as a property to all components
         * The gas constant for dry air in the Emanuel scheme is now renamed _Rdair
         * RRTMG LW and SW are now OpenMP parallel
```

### Comparing `climt-0.9.3/CONTRIBUTING.rst` & `climt-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_core/constants.py` & `climt-0.9.4/climt/_core/constants.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_core/initialization.py` & `climt-0.9.4/climt/_core/initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,24 @@
 
     init_array[:] = target_profile[np.newaxis, np.newaxis, :]
 
     return init_array
 
 
 climt_quantity_descriptions = {
+    'latitude': {
+        'dims': ['x', 'y'],
+        'units': 'degrees_north',
+        'default_value': 0
+    },
+    'longitude': {
+        'dims': ['x', 'y'],
+        'units': 'degrees_east',
+        'default_value': 0
+    },
     'air_pressure': {
         'dims': ['x', 'y', 'mid_levels'],
         'units': 'Pa',
         'init_func': init_mid_level_pressures
     },
     'air_pressure_on_interface_levels': {
         'dims': ['x', 'y', 'interface_levels'],
```

### Comparing `climt-0.9.3/climt/_core/__init__.py` & `climt-0.9.4/climt/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_core/util.py` & `climt-0.9.4/climt/_core/util.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_core/climt_components.py` & `climt-0.9.4/climt/_core/climt_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,15 +288,16 @@
 
     _climt_tendencies = {}
 
     _climt_diagnostics = {}
 
     @property
     def inputs(self):
-        return tuple(self._climt_inputs.keys())
+        return tuple(list(self._climt_inputs.keys()) +
+                     ['x', 'y', 'mid_levels', 'interface_levels'])
 
     @property
     def tendencies(self):
         return tuple(self._climt_tendencies.keys())
 
     @property
     def diagnostics(self):
@@ -327,17 +328,17 @@
                 A "piecewise constant" component.
 
         """
 
         return UpdateFrequencyWrapper(self, update_time)
 
     def scaled_version(self,
-                       input_scale_factors,
-                       diagnostic_scale_factors,
-                       tendency_scale_factors):
+                       input_scale_factors=None,
+                       diagnostic_scale_factors=None,
+                       tendency_scale_factors=None):
         """
         Returns component whose input/outputs/tendencies/diagnostics are scaled
         by the given scale factors.
 
         Args:
             input_scale_factors (dict):
                 a dictionary whose keys are the inputs that will be scaled
@@ -379,31 +380,32 @@
 
     _climt_inputs = {}
 
     _climt_tendencies = {}
 
     @property
     def inputs(self):
-        return tuple(self._climt_inputs.keys())
+        return tuple(list(self._climt_inputs.keys()) +
+                     ['x', 'y', 'mid_levels', 'interface_levels'])
 
     @property
     def diagnostics(self):
         return tuple(self._climt_diagnostics.keys())
 
     @property
     def input_properties(self):
         return self.create_properties_dict(self._climt_inputs)
 
     @property
     def diagnostic_properties(self):
         return self.create_properties_dict(self._climt_diagnostics)
 
     def scaled_version(self,
-                       input_scale_factors,
-                       diagnostic_scale_factors):
+                       input_scale_factors=None,
+                       diagnostic_scale_factors=None):
         """
         Returns component whose input/outputs/tendencies/diagnostics are scaled
         by the given scale factors.
 
         Args:
             input_scale_factors (dict):
                 a dictionary whose keys are the inputs that will be scaled
@@ -447,15 +449,16 @@
 
     _climt_outputs = {}
 
     _climt_diagnostics = {}
 
     @property
     def inputs(self):
-        return tuple(self._climt_inputs.keys())
+        return tuple(list(self._climt_inputs.keys()) +
+                     ['x', 'y', 'mid_levels', 'interface_levels'])
 
     @property
     def outputs(self):
         return tuple(self._climt_outputs.keys())
 
     @property
     def diagnostics(self):
@@ -478,17 +481,17 @@
         Returns a Prognostic component whose tendencies are the time differenced
         outputs of this Implicit component.
 
         """
         return ClimtTimeDifferenced(self)
 
     def scaled_version(self,
-                       input_scale_factors,
-                       diagnostic_scale_factors,
-                       output_scale_factors):
+                       input_scale_factors=None,
+                       diagnostic_scale_factors=None,
+                       output_scale_factors=None):
         """
         Returns component whose input/outputs/tendencies/diagnostics are scaled
         by the given scale factors.
 
         Args:
             input_scale_factors (dict):
                 a dictionary whose keys are the inputs that will be scaled
@@ -588,26 +591,30 @@
     @prognostics.setter
     def prognostics(self, prognostic_list):
         self._prognostic = PrognosticComposite(*prognostic_list)
 
     @property
     def inputs(self):
         if self._prognostic is not None:
-            return set(self._prognostic.inputs).union(set(self._climt_inputs.keys()))
+            return set(self._prognostic.inputs).union(
+                set(list(self._climt_inputs.keys()) +
+                    ['x', 'y', 'mid_levels', 'interface_levels']))
         else:
-            return set(self._climt_inputs.keys())
+            return set(list(self._climt_inputs.keys()) +
+                       ['x', 'y', 'mid_levels', 'interface_levels'])
 
     @property
     def outputs(self):
         return set(self._climt_outputs.keys())
 
     @property
     def diagnostics(self):
         if self._prognostic is not None:
-            return set(self._prognostic.diagnostics).union(set(self._climt_diagnostics.keys()))
+            return set(self._prognostic.diagnostics).union(
+                set(self._climt_diagnostics.keys()))
         else:
             return set(self._climt_diagnostics.keys())
 
     @property
     def input_properties(self):
         return self.create_properties_dict(self._climt_inputs)
 
@@ -616,17 +623,17 @@
         return self.create_properties_dict(self._climt_outputs)
 
     @property
     def diagnostic_properties(self):
         return self.create_properties_dict(self._climt_diagnostics)
 
     def scaled_version(self,
-                       input_scale_factors,
-                       diagnostic_scale_factors,
-                       output_scale_factors):
+                       input_scale_factors=None,
+                       diagnostic_scale_factors=None,
+                       output_scale_factors=None):
         """
         Returns component whose input/outputs/tendencies/diagnostics are scaled
         by the given scale factors.
 
         Args:
             input_scale_factors (dict):
                 a dictionary whose keys are the inputs that will be scaled
```

### Comparing `climt-0.9.3/climt/__init__.py` & `climt-0.9.4/climt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     ClimtImplicitPrognostic, ClimtPrognostic, ClimtImplicit, ClimtDiagnostic,
     ClimtSpectralDynamicalCore,
     Frierson06LongwaveOpticalDepth, GrayLongwaveRadiation, HeldSuarez,
     GridScaleCondensation, BergerSolarInsolation, SimplePhysics, RRTMGLongwave, RRTMGShortwave,
     EmanuelConvection, SlabSurface, GFSDynamicalCore, DcmipInitialConditions, IceSheet,
     Instellation)
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
```

### Comparing `climt-0.9.3/climt/_lib/GFS/Makefile.conf.gfortran` & `climt-0.9.4/climt/_lib/GFS/Makefile.conf.gfortran`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/params.f90` & `climt-0.9.4/climt/_lib/GFS/params.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/Makefile.conf.ifort` & `climt-0.9.4/climt/_lib/GFS/Makefile.conf.ifort`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/run.f90` & `climt-0.9.4/climt/_lib/GFS/run.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/spectral_data.f90` & `climt-0.9.4/climt/_lib/GFS/spectral_data.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/pressure_data.f90` & `climt-0.9.4/climt/_lib/GFS/pressure_data.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/Makefile` & `climt-0.9.4/climt/_lib/GFS/Makefile`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/dyn_finalize.f90` & `climt-0.9.4/climt/_lib/GFS/dyn_finalize.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/shtns.f90` & `climt-0.9.4/climt/_lib/GFS/shtns.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/kinds.f90` & `climt-0.9.4/climt/_lib/GFS/kinds.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/Makefile.conf` & `climt-0.9.4/climt/_lib/GFS/Makefile.conf`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/physcons.f90` & `climt-0.9.4/climt/_lib/GFS/physcons.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/dyn_run.f90` & `climt-0.9.4/climt/_lib/GFS/dyn_run.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/dyn_init.f90` & `climt-0.9.4/climt/_lib/GFS/dyn_init.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/phy_data_stub.f90` & `climt-0.9.4/climt/_lib/GFS/phy_data_stub.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/semimp_data.f90` & `climt-0.9.4/climt/_lib/GFS/semimp_data.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/phy_run_hs.f90` & `climt-0.9.4/climt/_lib/GFS/phy_run_hs.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/phy_data.f90` & `climt-0.9.4/climt/_lib/GFS/phy_data.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/grid_data.f90` & `climt-0.9.4/climt/_lib/GFS/grid_data.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/phy_run.f90` & `climt-0.9.4/climt/_lib/GFS/phy_run.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/GFS/phy_run_stub.f90` & `climt-0.9.4/climt/_lib/GFS/phy_run_stub.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/simple_physics/simple_physics_v5_1.f90` & `climt-0.9.4/climt/_lib/simple_physics/simple_physics_v5_1.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/simple_physics/simple_physics_custom.f90` & `climt-0.9.4/climt/_lib/simple_physics/simple_physics_custom.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_5_v1.f90` & `climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_5_v1.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_1_2_3_v5.f90` & `climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_1_2_3_v5.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/dcmip/dcmip_initial_conditions_test_4_v3.f90` & `climt-0.9.4/climt/_lib/dcmip/dcmip_initial_conditions_test_4_v3.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_k_g.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_k_g.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg01.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg01.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg07.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg07.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/setup.py` & `climt-0.9.4/climt/_lib/rrtmg_lw/setup.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmr.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmr.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg11.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg11.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg04.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg04.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/Makefile` & `climt-0.9.4/climt/_lib/rrtmg_lw/Makefile`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_read_nc.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_read_nc.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_cldprop.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_cldprop.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/_rrtm_lw.pyx` & `climt-0.9.4/climt/_lib/rrtmg_lw/_rrtm_lw.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_wvn.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_wvn.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/mcica_subcol_gen_lw.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/mcica_subcol_gen_lw.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_taumol.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_taumol.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_init.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_init.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/parrrtm.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/parrrtm.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg12.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg12.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_cldprmc.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_cldprmc.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/parkind.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/parkind.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_tbl.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_tbl.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg15.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg15.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_ncpar.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_ncpar.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg05.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg05.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_cld.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_cld.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg06.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg06.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_setcoef.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_setcoef.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg02.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg02.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg08.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg08.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg16.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg16.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmc.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrnmc.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg10.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg10.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg09.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg09.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rad.nomcica.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rad.nomcica.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg03.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg03.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_ref.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_ref.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg13.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg13.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rad.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rad.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_vsn.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_vsn.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_con.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_con.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrtmg_lw_rtrn.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrtmg_lw_rtrn.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/rrlw_kg14.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/rrlw_kg14.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_lw/mcica_random_numbers.f90` & `climt-0.9.4/climt/_lib/rrtmg_lw/mcica_random_numbers.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/Makefile` & `climt-0.9.4/climt/_lib/Makefile`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/emanuel/convect43c.f90` & `climt-0.9.4/climt/_lib/emanuel/convect43c.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_k_g.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_k_g.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_cldprmc.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_cldprmc.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/mcica_subcol_gen_sw.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/mcica_subcol_gen_sw.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg29.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg29.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg22.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg22.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg23.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg23.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/setup.py` & `climt-0.9.4/climt/_lib/rrtmg_sw/setup.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_aer.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_aer.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_ref.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_ref.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg20.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg20.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/Makefile` & `climt-0.9.4/climt/_lib/rrtmg_sw/Makefile`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_spcvmc.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_spcvmc.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg16.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg16.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_rad.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_rad.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_ncpar.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_ncpar.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_wvn.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_wvn.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg27.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg27.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_vrtqdr.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_vrtqdr.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg25.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg25.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_reftra.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_reftra.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg17.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg17.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_spcvrt.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_spcvrt.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/parkind.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/parkind.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/README` & `climt-0.9.4/climt/_lib/rrtmg_sw/README`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_con.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_con.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg19.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg19.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg28.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg28.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg18.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg18.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_tbl.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_tbl.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/_rrtm_sw.pyx` & `climt-0.9.4/climt/_lib/rrtmg_sw/_rrtm_sw.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_cldprop.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_cldprop.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg21.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg21.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/parrrsw.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/parrrsw.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_init.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_init.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_vsn.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_vsn.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_rad.nomcica.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_rad.nomcica.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_cld.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_cld.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_taumol.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_taumol.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg26.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg26.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrtmg_sw_setcoef.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrtmg_sw_setcoef.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/rrsw_kg24.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/rrsw_kg24.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_lib/rrtmg_sw/mcica_random_numbers.f90` & `climt-0.9.4/climt/_lib/rrtmg_sw/mcica_random_numbers.f90`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/held_suarez.py` & `climt-0.9.4/climt/_components/held_suarez.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/simple_physics/component.py` & `climt-0.9.4/climt/_components/simple_physics/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     title = {Idealized tropical cyclone simulations of intermediate complexity: a test case for {AGCMs}}
     journal = {Journal of Advances in Modeling Earth Systems}
 
     """
 
     _climt_inputs = {
         'air_temperature': 'degK',
+        'latitude': 'degrees_north',
         'air_pressure': 'mbar',
         'air_pressure_on_interface_levels': 'mbar',
         'surface_air_pressure': 'mbar',
         'surface_temperature': 'degK',
         'specific_humidity': 'g/g',
         'northward_wind': 'm s^-1',
         'eastward_wind': 'm s^-1',
```

### Comparing `climt-0.9.3/climt/_components/simple_physics/_simple_physics.pyx` & `climt-0.9.4/climt/_components/simple_physics/_simple_physics.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/radiation.py` & `climt-0.9.4/climt/_components/radiation.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/dcmip/component.py` & `climt-0.9.4/climt/_components/dcmip/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/dcmip/_dcmip.pyx` & `climt-0.9.4/climt/_components/dcmip/_dcmip.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/slab_surface.py` & `climt-0.9.4/climt/_components/slab_surface.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/grid_scale_condensation.py` & `climt-0.9.4/climt/_components/grid_scale_condensation.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/__init__.py` & `climt-0.9.4/climt/_components/__init__.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/_berger_solar_insolation.pyx` & `climt-0.9.4/climt/_components/_berger_solar_insolation.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/gfs/component.py` & `climt-0.9.4/climt/_components/gfs/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/gfs/_gfs_dynamics.pyx` & `climt-0.9.4/climt/_components/gfs/_gfs_dynamics.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/emanuel/component.py` & `climt-0.9.4/climt/_components/emanuel/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/emanuel/_emanuel_convection.pyx` & `climt-0.9.4/climt/_components/emanuel/_emanuel_convection.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/instellation/component.py` & `climt-0.9.4/climt/_components/instellation/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/berger_solar_insolation.py` & `climt-0.9.4/climt/_components/berger_solar_insolation.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/rrtmg/sw/component.py` & `climt-0.9.4/climt/_components/rrtmg/sw/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/rrtmg/sw/_rrtmg_sw.pyx` & `climt-0.9.4/climt/_components/rrtmg/sw/_rrtmg_sw.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/rrtmg/rrtmg_common.py` & `climt-0.9.4/climt/_components/rrtmg/rrtmg_common.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/rrtmg/lw/_rrtmg_lw.pyx` & `climt-0.9.4/climt/_components/rrtmg/lw/_rrtmg_lw.pyx`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/rrtmg/lw/component.py` & `climt-0.9.4/climt/_components/rrtmg/lw/component.py`

 * *Files identical despite different names*

### Comparing `climt-0.9.3/climt/_components/surface_ice.py` & `climt-0.9.4/climt/_components/surface_ice.py`

 * *Files identical despite different names*

