# Comparing `tmp/ffpack-0.3.2.tar.gz` & `tmp/ffpack-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffpack-0.3.2.tar", max compression
+gzip compressed data, was "ffpack-0.3.3.tar", max compression
```

## Comparing `ffpack-0.3.2.tar` & `ffpack-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35802 2022-12-06 23:05:33.040532 ffpack-0.3.2/LICENSE
--rw-r--r--   0        0        0     1036 2023-05-20 16:52:30.896205 ffpack-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5258 2023-05-20 14:46:21.677826 ffpack-0.3.2/README.md
--rw-r--r--   0        0        0       24 2022-12-10 04:24:17.086454 ffpack-0.3.2/src/ffpack/__init__.py
--rw-r--r--   0        0        0       80 2022-12-10 04:24:16.276455 ffpack-0.3.2/src/ffpack/__main__.py
--rw-r--r--   0        0        0     1671 2023-05-20 14:46:21.722612 ffpack-0.3.2/src/ffpack/config.py
--rw-r--r--   0        0        0       27 2023-01-26 03:02:18.865760 ffpack-0.3.2/src/ffpack/fdm/__init__.py
--rw-r--r--   0        0        0     4156 2023-05-20 14:46:21.722612 ffpack-0.3.2/src/ffpack/fdm/minerModel.py
--rw-r--r--   0        0        0      168 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/__init__.py
--rw-r--r--   0        0        0    16040 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/astmCounting.py
--rw-r--r--   0        0        0     3267 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/fourPointCounting.py
--rw-r--r--   0        0        0     2757 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/johannessonCounting.py
--rw-r--r--   0        0        0     8731 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/meanStressCorrection.py
--rw-r--r--   0        0        0     3434 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/rychlikCounting.py
--rw-r--r--   0        0        0      108 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lsg/__init__.py
--rw-r--r--   0        0        0     9095 2023-05-20 14:46:21.727116 ffpack-0.3.2/src/ffpack/lsg/autoregressiveMovingAverage.py
--rw-r--r--   0        0        0     1624 2023-05-20 14:46:21.731120 ffpack-0.3.2/src/ffpack/lsg/randomWalk.py
--rw-r--r--   0        0        0     4415 2023-05-20 14:46:21.733121 ffpack-0.3.2/src/ffpack/lsg/sequenceFromSpectrum.py
--rw-r--r--   0        0        0      124 2023-01-22 14:48:45.006235 ffpack-0.3.2/src/ffpack/lsm/__init__.py
--rw-r--r--   0        0        0    10576 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/cycleCountingMatrix.py
--rw-r--r--   0        0        0     2540 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/sequenceSpectra.py
--rw-r--r--   0        0        0     8898 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/waveSpectra.py
--rw-r--r--   0        0        0    10974 2023-05-20 14:46:21.735120 ffpack-0.3.2/src/ffpack/lsm/windSpectra.py
--rw-r--r--   0        0        0       57 2023-01-05 01:51:18.234952 ffpack-0.3.2/src/ffpack/rpm/__init__.py
--rw-r--r--   0        0        0    10896 2023-05-20 14:46:21.762318 ffpack-0.3.2/src/ffpack/rpm/metropolisHastings.py
--rw-r--r--   0        0        0    13525 2023-05-20 14:46:21.765318 ffpack-0.3.2/src/ffpack/rpm/nataf.py
--rw-r--r--   0        0        0      177 2023-01-22 14:48:45.014238 ffpack-0.3.2/src/ffpack/rrm/__init__.py
--rw-r--r--   0        0        0     7990 2023-05-20 14:46:21.765318 ffpack-0.3.2/src/ffpack/rrm/firstOrderReliabilityMethod.py
--rw-r--r--   0        0        0     2249 2023-05-20 14:46:21.766822 ffpack-0.3.2/src/ffpack/rrm/firstOrderSecondMoment.py
--rw-r--r--   0        0        0    11367 2023-05-20 14:46:21.766822 ffpack-0.3.2/src/ffpack/rrm/secondOrderReliabilityMethod.py
--rw-r--r--   0        0        0     7364 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/rrm/simulationBasedReliabilityMethod.py
--rw-r--r--   0        0        0      170 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/utils/__init__.py
--rw-r--r--   0        0        0     1887 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/utils/aggregation.py
--rw-r--r--   0        0        0     2055 2023-05-20 14:46:21.771832 ffpack-0.3.2/src/ffpack/utils/countingMatrix.py
--rw-r--r--   0        0        0    11870 2023-05-20 14:46:21.774832 ffpack-0.3.2/src/ffpack/utils/derivatives.py
--rw-r--r--   0        0        0     1313 2023-05-20 14:46:21.774832 ffpack-0.3.2/src/ffpack/utils/digitization.py
--rw-r--r--   0        0        0     2620 2023-05-20 14:46:21.775832 ffpack-0.3.2/src/ffpack/utils/fitter.py
--rw-r--r--   0        0        0     4417 2023-05-20 14:46:21.775832 ffpack-0.3.2/src/ffpack/utils/sequenceFilter.py
--rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 ffpack-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-12-06 23:05:33.040532 ffpack-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1036 2023-05-20 18:27:07.719799 ffpack-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5258 2023-05-20 14:46:21.677826 ffpack-0.3.3/README.md
+-rw-r--r--   0        0        0       24 2022-12-10 04:24:17.086454 ffpack-0.3.3/src/ffpack/__init__.py
+-rw-r--r--   0        0        0       80 2022-12-10 04:24:16.276455 ffpack-0.3.3/src/ffpack/__main__.py
+-rw-r--r--   0        0        0     1671 2023-05-20 14:46:21.722612 ffpack-0.3.3/src/ffpack/config.py
+-rw-r--r--   0        0        0       27 2023-01-26 03:02:18.865760 ffpack-0.3.3/src/ffpack/fdm/__init__.py
+-rw-r--r--   0        0        0     4156 2023-05-20 14:46:21.722612 ffpack-0.3.3/src/ffpack/fdm/minerModel.py
+-rw-r--r--   0        0        0      168 2023-05-20 14:46:21.723614 ffpack-0.3.3/src/ffpack/lcc/__init__.py
+-rw-r--r--   0        0        0    16040 2023-05-20 14:46:21.723614 ffpack-0.3.3/src/ffpack/lcc/astmCounting.py
+-rw-r--r--   0        0        0     3267 2023-05-20 14:46:21.723614 ffpack-0.3.3/src/ffpack/lcc/fourPointCounting.py
+-rw-r--r--   0        0        0     2757 2023-05-20 14:46:21.724612 ffpack-0.3.3/src/ffpack/lcc/johannessonCounting.py
+-rw-r--r--   0        0        0     8731 2023-05-20 14:46:21.724612 ffpack-0.3.3/src/ffpack/lcc/meanStressCorrection.py
+-rw-r--r--   0        0        0     3434 2023-05-20 14:46:21.724612 ffpack-0.3.3/src/ffpack/lcc/rychlikCounting.py
+-rw-r--r--   0        0        0      108 2023-05-20 14:46:21.724612 ffpack-0.3.3/src/ffpack/lsg/__init__.py
+-rw-r--r--   0        0        0     9095 2023-05-20 14:46:21.727116 ffpack-0.3.3/src/ffpack/lsg/autoregressiveMovingAverage.py
+-rw-r--r--   0        0        0     1624 2023-05-20 14:46:21.731120 ffpack-0.3.3/src/ffpack/lsg/randomWalk.py
+-rw-r--r--   0        0        0     4415 2023-05-20 14:46:21.733121 ffpack-0.3.3/src/ffpack/lsg/sequenceFromSpectrum.py
+-rw-r--r--   0        0        0      124 2023-01-22 14:48:45.006235 ffpack-0.3.3/src/ffpack/lsm/__init__.py
+-rw-r--r--   0        0        0    10576 2023-05-20 14:46:21.734120 ffpack-0.3.3/src/ffpack/lsm/cycleCountingMatrix.py
+-rw-r--r--   0        0        0     2540 2023-05-20 14:46:21.734120 ffpack-0.3.3/src/ffpack/lsm/sequenceSpectra.py
+-rw-r--r--   0        0        0     8898 2023-05-20 14:46:21.734120 ffpack-0.3.3/src/ffpack/lsm/waveSpectra.py
+-rw-r--r--   0        0        0    10974 2023-05-20 14:46:21.735120 ffpack-0.3.3/src/ffpack/lsm/windSpectra.py
+-rw-r--r--   0        0        0       57 2023-01-05 01:51:18.234952 ffpack-0.3.3/src/ffpack/rpm/__init__.py
+-rw-r--r--   0        0        0    10896 2023-05-20 14:46:21.762318 ffpack-0.3.3/src/ffpack/rpm/metropolisHastings.py
+-rw-r--r--   0        0        0    13525 2023-05-20 14:46:21.765318 ffpack-0.3.3/src/ffpack/rpm/nataf.py
+-rw-r--r--   0        0        0      177 2023-01-22 14:48:45.014238 ffpack-0.3.3/src/ffpack/rrm/__init__.py
+-rw-r--r--   0        0        0     7990 2023-05-20 14:46:21.765318 ffpack-0.3.3/src/ffpack/rrm/firstOrderReliabilityMethod.py
+-rw-r--r--   0        0        0     2249 2023-05-20 14:46:21.766822 ffpack-0.3.3/src/ffpack/rrm/firstOrderSecondMoment.py
+-rw-r--r--   0        0        0    11367 2023-05-20 14:46:21.766822 ffpack-0.3.3/src/ffpack/rrm/secondOrderReliabilityMethod.py
+-rw-r--r--   0        0        0     7364 2023-05-20 14:46:21.769832 ffpack-0.3.3/src/ffpack/rrm/simulationBasedReliabilityMethod.py
+-rw-r--r--   0        0        0      170 2023-05-20 14:46:21.769832 ffpack-0.3.3/src/ffpack/utils/__init__.py
+-rw-r--r--   0        0        0     1887 2023-05-20 14:46:21.769832 ffpack-0.3.3/src/ffpack/utils/aggregation.py
+-rw-r--r--   0        0        0     2055 2023-05-20 14:46:21.771832 ffpack-0.3.3/src/ffpack/utils/countingMatrix.py
+-rw-r--r--   0        0        0    11870 2023-05-20 14:46:21.774832 ffpack-0.3.3/src/ffpack/utils/derivatives.py
+-rw-r--r--   0        0        0     1313 2023-05-20 14:46:21.774832 ffpack-0.3.3/src/ffpack/utils/digitization.py
+-rw-r--r--   0        0        0     2620 2023-05-20 14:46:21.775832 ffpack-0.3.3/src/ffpack/utils/fitter.py
+-rw-r--r--   0        0        0     4417 2023-05-20 14:46:21.775832 ffpack-0.3.3/src/ffpack/utils/sequenceFilter.py
+-rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 ffpack-0.3.3/PKG-INFO
```

### Comparing `ffpack-0.3.2/LICENSE` & `ffpack-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/pyproject.toml` & `ffpack-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ffpack"
-version = "0.3.2"
+version = "0.3.3"
 description = "Fatigue and fracture package"
 authors = [
     "Dongping Zhu",
     "Zhixia Ding",
     "Xiaogang Huang",
 ]
```

### Comparing `ffpack-0.3.2/README.md` & `ffpack-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/config.py` & `ffpack-0.3.3/src/ffpack/config.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/fdm/minerModel.py` & `ffpack-0.3.3/src/ffpack/fdm/minerModel.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lcc/astmCounting.py` & `ffpack-0.3.3/src/ffpack/lcc/astmCounting.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lcc/fourPointCounting.py` & `ffpack-0.3.3/src/ffpack/lcc/fourPointCounting.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lcc/johannessonCounting.py` & `ffpack-0.3.3/src/ffpack/lcc/johannessonCounting.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lcc/meanStressCorrection.py` & `ffpack-0.3.3/src/ffpack/lcc/meanStressCorrection.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lcc/rychlikCounting.py` & `ffpack-0.3.3/src/ffpack/lcc/rychlikCounting.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsg/autoregressiveMovingAverage.py` & `ffpack-0.3.3/src/ffpack/lsg/autoregressiveMovingAverage.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsg/randomWalk.py` & `ffpack-0.3.3/src/ffpack/lsg/randomWalk.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsg/sequenceFromSpectrum.py` & `ffpack-0.3.3/src/ffpack/lsg/sequenceFromSpectrum.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsm/cycleCountingMatrix.py` & `ffpack-0.3.3/src/ffpack/lsm/cycleCountingMatrix.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsm/sequenceSpectra.py` & `ffpack-0.3.3/src/ffpack/lsm/sequenceSpectra.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsm/waveSpectra.py` & `ffpack-0.3.3/src/ffpack/lsm/waveSpectra.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/lsm/windSpectra.py` & `ffpack-0.3.3/src/ffpack/lsm/windSpectra.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rpm/metropolisHastings.py` & `ffpack-0.3.3/src/ffpack/rpm/metropolisHastings.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rpm/nataf.py` & `ffpack-0.3.3/src/ffpack/rpm/nataf.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rrm/firstOrderReliabilityMethod.py` & `ffpack-0.3.3/src/ffpack/rrm/firstOrderReliabilityMethod.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rrm/firstOrderSecondMoment.py` & `ffpack-0.3.3/src/ffpack/rrm/firstOrderSecondMoment.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rrm/secondOrderReliabilityMethod.py` & `ffpack-0.3.3/src/ffpack/rrm/secondOrderReliabilityMethod.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/rrm/simulationBasedReliabilityMethod.py` & `ffpack-0.3.3/src/ffpack/rrm/simulationBasedReliabilityMethod.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/aggregation.py` & `ffpack-0.3.3/src/ffpack/utils/aggregation.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/countingMatrix.py` & `ffpack-0.3.3/src/ffpack/utils/countingMatrix.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/derivatives.py` & `ffpack-0.3.3/src/ffpack/utils/derivatives.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/digitization.py` & `ffpack-0.3.3/src/ffpack/utils/digitization.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/fitter.py` & `ffpack-0.3.3/src/ffpack/utils/fitter.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/src/ffpack/utils/sequenceFilter.py` & `ffpack-0.3.3/src/ffpack/utils/sequenceFilter.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.2/PKG-INFO` & `ffpack-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffpack
-Version: 0.3.2
+Version: 0.3.3
 Summary: Fatigue and fracture package
 Home-page: https://pypi.org/project/ffpack
 Keywords: fatigue,fracture,load,reliability
 Author: Dongping Zhu
 Maintainer: Dongping Zhu
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

