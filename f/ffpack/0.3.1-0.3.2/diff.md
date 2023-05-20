# Comparing `tmp/ffpack-0.3.1.tar.gz` & `tmp/ffpack-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffpack-0.3.1.tar", max compression
+gzip compressed data, was "ffpack-0.3.2.tar", max compression
```

## Comparing `ffpack-0.3.1.tar` & `ffpack-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0    35802 2022-12-06 23:05:33.040532 ffpack-0.3.1/LICENSE
--rw-r--r--   0        0        0     1036 2023-01-14 05:24:32.042058 ffpack-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5133 2023-01-27 02:08:37.629466 ffpack-0.3.1/README.md
--rw-r--r--   0        0        0       24 2022-12-10 04:24:17.086454 ffpack-0.3.1/src/ffpack/__init__.py
--rw-r--r--   0        0        0       80 2022-12-10 04:24:16.276455 ffpack-0.3.1/src/ffpack/__main__.py
--rw-r--r--   0        0        0     1612 2023-01-08 02:17:57.271348 ffpack-0.3.1/src/ffpack/config.py
--rw-r--r--   0        0        0       27 2023-01-26 03:02:18.865760 ffpack-0.3.1/src/ffpack/fdm/__init__.py
--rw-r--r--   0        0        0     4154 2023-01-26 03:03:09.198316 ffpack-0.3.1/src/ffpack/fdm/minerModel.py
--rw-r--r--   0        0        0      131 2023-01-13 23:04:53.792903 ffpack-0.3.1/src/ffpack/lcc/__init__.py
--rw-r--r--   0        0        0    16024 2023-01-14 05:24:32.042058 ffpack-0.3.1/src/ffpack/lcc/astmCounting.py
--rw-r--r--   0        0        0     3260 2023-01-14 05:24:32.042058 ffpack-0.3.1/src/ffpack/lcc/fourPointCounting.py
--rw-r--r--   0        0        0     2751 2023-01-14 05:24:32.043059 ffpack-0.3.1/src/ffpack/lcc/johannessonCounting.py
--rw-r--r--   0        0        0     3430 2023-01-14 05:24:32.043059 ffpack-0.3.1/src/ffpack/lcc/rychlikCounting.py
--rw-r--r--   0        0        0      100 2023-01-22 14:48:45.000235 ffpack-0.3.1/src/ffpack/lsg/__init__.py
--rw-r--r--   0        0        0     8007 2023-01-08 02:17:57.271348 ffpack-0.3.1/src/ffpack/lsg/autoregressiveModel.py
--rw-r--r--   0        0        0     1347 2023-01-22 14:48:45.002235 ffpack-0.3.1/src/ffpack/lsg/randomWalk.py
--rw-r--r--   0        0        0     4182 2023-01-25 02:49:27.605279 ffpack-0.3.1/src/ffpack/lsg/sequenceFromSpectrum.py
--rw-r--r--   0        0        0      124 2023-01-22 14:48:45.006235 ffpack-0.3.1/src/ffpack/lsm/__init__.py
--rw-r--r--   0        0        0    10540 2023-01-22 14:48:45.008235 ffpack-0.3.1/src/ffpack/lsm/cycleCountingMatrix.py
--rw-r--r--   0        0        0     2542 2023-01-22 14:48:45.010235 ffpack-0.3.1/src/ffpack/lsm/sequenceSpectra.py
--rw-r--r--   0        0        0     8908 2023-01-13 02:38:26.489893 ffpack-0.3.1/src/ffpack/lsm/waveSpectra.py
--rw-r--r--   0        0        0    10982 2023-01-13 02:38:26.490894 ffpack-0.3.1/src/ffpack/lsm/windSpectra.py
--rw-r--r--   0        0        0       57 2023-01-05 01:51:18.234952 ffpack-0.3.1/src/ffpack/rpm/__init__.py
--rw-r--r--   0        0        0    10316 2023-01-22 14:48:45.012237 ffpack-0.3.1/src/ffpack/rpm/metropolisHastings.py
--rw-r--r--   0        0        0    13222 2023-01-13 23:33:22.308609 ffpack-0.3.1/src/ffpack/rpm/nataf.py
--rw-r--r--   0        0        0      177 2023-01-22 14:48:45.014238 ffpack-0.3.1/src/ffpack/rrm/__init__.py
--rw-r--r--   0        0        0     7988 2023-01-25 02:49:27.605279 ffpack-0.3.1/src/ffpack/rrm/firstOrderReliabilityMethod.py
--rw-r--r--   0        0        0     2247 2023-01-25 02:49:27.605279 ffpack-0.3.1/src/ffpack/rrm/firstOrderSecondMoment.py
--rw-r--r--   0        0        0    11363 2023-01-25 02:49:27.606279 ffpack-0.3.1/src/ffpack/rrm/secondOrderReliabilityMethod.py
--rw-r--r--   0        0        0     7085 2023-01-22 14:48:45.022238 ffpack-0.3.1/src/ffpack/rrm/simulationBasedReliabilityMethod.py
--rw-r--r--   0        0        0      130 2023-01-10 03:21:47.924572 ffpack-0.3.1/src/ffpack/utils/__init__.py
--rw-r--r--   0        0        0     2618 2023-01-25 02:49:27.606279 ffpack-0.3.1/src/ffpack/utils/fdrUtils.py
--rw-r--r--   0        0        0     5688 2023-01-14 17:04:30.876970 ffpack-0.3.1/src/ffpack/utils/generalUtils.py
--rw-r--r--   0        0        0     1885 2022-12-31 01:17:32.005085 ffpack-0.3.1/src/ffpack/utils/lccUtils.py
--rw-r--r--   0        0        0     2049 2023-01-08 02:17:57.274349 ffpack-0.3.1/src/ffpack/utils/lsmUtils.py
--rw-r--r--   0        0        0    11870 2023-01-13 23:04:53.794903 ffpack-0.3.1/src/ffpack/utils/miscUtils.py
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 ffpack-0.3.1/setup.py
--rw-r--r--   0        0        0     6063 1970-01-01 00:00:00.000000 ffpack-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-12-06 23:05:33.040532 ffpack-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1036 2023-05-20 16:52:30.896205 ffpack-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5258 2023-05-20 14:46:21.677826 ffpack-0.3.2/README.md
+-rw-r--r--   0        0        0       24 2022-12-10 04:24:17.086454 ffpack-0.3.2/src/ffpack/__init__.py
+-rw-r--r--   0        0        0       80 2022-12-10 04:24:16.276455 ffpack-0.3.2/src/ffpack/__main__.py
+-rw-r--r--   0        0        0     1671 2023-05-20 14:46:21.722612 ffpack-0.3.2/src/ffpack/config.py
+-rw-r--r--   0        0        0       27 2023-01-26 03:02:18.865760 ffpack-0.3.2/src/ffpack/fdm/__init__.py
+-rw-r--r--   0        0        0     4156 2023-05-20 14:46:21.722612 ffpack-0.3.2/src/ffpack/fdm/minerModel.py
+-rw-r--r--   0        0        0      168 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/__init__.py
+-rw-r--r--   0        0        0    16040 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/astmCounting.py
+-rw-r--r--   0        0        0     3267 2023-05-20 14:46:21.723614 ffpack-0.3.2/src/ffpack/lcc/fourPointCounting.py
+-rw-r--r--   0        0        0     2757 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/johannessonCounting.py
+-rw-r--r--   0        0        0     8731 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/meanStressCorrection.py
+-rw-r--r--   0        0        0     3434 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lcc/rychlikCounting.py
+-rw-r--r--   0        0        0      108 2023-05-20 14:46:21.724612 ffpack-0.3.2/src/ffpack/lsg/__init__.py
+-rw-r--r--   0        0        0     9095 2023-05-20 14:46:21.727116 ffpack-0.3.2/src/ffpack/lsg/autoregressiveMovingAverage.py
+-rw-r--r--   0        0        0     1624 2023-05-20 14:46:21.731120 ffpack-0.3.2/src/ffpack/lsg/randomWalk.py
+-rw-r--r--   0        0        0     4415 2023-05-20 14:46:21.733121 ffpack-0.3.2/src/ffpack/lsg/sequenceFromSpectrum.py
+-rw-r--r--   0        0        0      124 2023-01-22 14:48:45.006235 ffpack-0.3.2/src/ffpack/lsm/__init__.py
+-rw-r--r--   0        0        0    10576 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/cycleCountingMatrix.py
+-rw-r--r--   0        0        0     2540 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/sequenceSpectra.py
+-rw-r--r--   0        0        0     8898 2023-05-20 14:46:21.734120 ffpack-0.3.2/src/ffpack/lsm/waveSpectra.py
+-rw-r--r--   0        0        0    10974 2023-05-20 14:46:21.735120 ffpack-0.3.2/src/ffpack/lsm/windSpectra.py
+-rw-r--r--   0        0        0       57 2023-01-05 01:51:18.234952 ffpack-0.3.2/src/ffpack/rpm/__init__.py
+-rw-r--r--   0        0        0    10896 2023-05-20 14:46:21.762318 ffpack-0.3.2/src/ffpack/rpm/metropolisHastings.py
+-rw-r--r--   0        0        0    13525 2023-05-20 14:46:21.765318 ffpack-0.3.2/src/ffpack/rpm/nataf.py
+-rw-r--r--   0        0        0      177 2023-01-22 14:48:45.014238 ffpack-0.3.2/src/ffpack/rrm/__init__.py
+-rw-r--r--   0        0        0     7990 2023-05-20 14:46:21.765318 ffpack-0.3.2/src/ffpack/rrm/firstOrderReliabilityMethod.py
+-rw-r--r--   0        0        0     2249 2023-05-20 14:46:21.766822 ffpack-0.3.2/src/ffpack/rrm/firstOrderSecondMoment.py
+-rw-r--r--   0        0        0    11367 2023-05-20 14:46:21.766822 ffpack-0.3.2/src/ffpack/rrm/secondOrderReliabilityMethod.py
+-rw-r--r--   0        0        0     7364 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/rrm/simulationBasedReliabilityMethod.py
+-rw-r--r--   0        0        0      170 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/utils/__init__.py
+-rw-r--r--   0        0        0     1887 2023-05-20 14:46:21.769832 ffpack-0.3.2/src/ffpack/utils/aggregation.py
+-rw-r--r--   0        0        0     2055 2023-05-20 14:46:21.771832 ffpack-0.3.2/src/ffpack/utils/countingMatrix.py
+-rw-r--r--   0        0        0    11870 2023-05-20 14:46:21.774832 ffpack-0.3.2/src/ffpack/utils/derivatives.py
+-rw-r--r--   0        0        0     1313 2023-05-20 14:46:21.774832 ffpack-0.3.2/src/ffpack/utils/digitization.py
+-rw-r--r--   0        0        0     2620 2023-05-20 14:46:21.775832 ffpack-0.3.2/src/ffpack/utils/fitter.py
+-rw-r--r--   0        0        0     4417 2023-05-20 14:46:21.775832 ffpack-0.3.2/src/ffpack/utils/sequenceFilter.py
+-rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 ffpack-0.3.2/PKG-INFO
```

### Comparing `ffpack-0.3.1/LICENSE` & `ffpack-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.1/pyproject.toml` & `ffpack-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ffpack"
-version = "0.3.1"
+version = "0.3.2"
 description = "Fatigue and fracture package"
 authors = [
     "Dongping Zhu",
     "Zhixia Ding",
     "Xiaogang Huang",
 ]
```

### Comparing `ffpack-0.3.1/README.md` & `ffpack-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,28 +43,32 @@
 ## Contents
 
 * Fatigue damage model
     * Palmgren-miner damage model
         * Naive Palmgren-miner damage model
         * Classic Palmgren-miner damage model
 
-* Load correction and counting
+* Load counting and correction
     * ASTM counting
         * ASTM level crossing counting
         * ASTM peak counting
         * ASTM simple range counting
         * ASTM range pair counting
         * ASTM rainflow counting
         * ASTM rainflow counting for repeating history
     * Johannesson counting
         * Johannesson min max counting
     * Rychlik counting
         * Rychlik rainflow counting
     * Four point counting
         * Four point rainflow counting
+    * Mean stress correction
+        * Goodman correction
+        * Soderberg correction
+        * Gerber correction
 
 * Load sequence generator
     * Random walk
         * Uniform random walk
     * Autoregressive moving average model
         * Normal autoregressive (AR) model
         * Normal moving average (MA) model
@@ -119,27 +123,27 @@
         * Subset simulation
 
 * Utility 
     * Aggregation
         * Cycle counting aggregation
     * Counting matrix
         * Counting results to counting matrix
-    * Fitter
-        * SN curve fitter
-    * Sequence filter
-        * Sequence peakValley filter
-        * Sequence hysteresis filter
-    * Degitization
-        * Sequence degitization
     * Derivatives
         * Derivative
         * Central derivative weights
         * Gradient
         * Hessian matrix
-
+    * Digitization
+        * Sequence digitization
+    * Fitter
+        * SN curve fitter
+    * Sequence filter
+        * Sequence peakValley filter
+        * Sequence hysteresis filter
+    
 ## Document
 
 You can find the latest documentation for setting up `FFPACK` at the [Read the Docs site](https://ffpack.readthedocs.io/en/latest/).
 
 ## Credits
 
 This project was made possible by the help from [DM2L lab](https://dm2l.uconn.edu/).
```

### Comparing `ffpack-0.3.1/src/ffpack/config.py` & `ffpack-0.3.2/src/ffpack/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
+
 class GlobalConfig:
     '''
     Global config for FFPACK
     '''
     def __init__( self ):
         '''
         Initialize a global config instance with default values.
@@ -53,12 +54,13 @@
         Set seed to None can clean the seed
         
         Examples
         --------
         >>> from ffpack.config import globalConfig
         >>> globalConfig.setSeed( 0 )
         '''
-        self.seed = seed
-        np.random.seed( self.seed )
+        if isinstance(seed, (int, type(None))):
+            self.seed = seed
+            np.random.seed( self.seed )
 
 
 globalConfig = GlobalConfig()
```

### Comparing `ffpack-0.3.1/src/ffpack/fdm/minerModel.py` & `ffpack-0.3.2/src/ffpack/fdm/minerModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Reference: Miner, M.A., 1945. Cumulative damage in fatigue.
 '''
 
 import numpy as np
 from ffpack import utils
 
+
 def minerDamageModelNaive( fatigueData ):
     '''
     Naive Palmgren-miner damage model directly calcuates the damage results.
 
     Parameters
     ----------
     fatigueData: 2d array
```

### Comparing `ffpack-0.3.1/src/ffpack/lcc/astmCounting.py` & `ffpack-0.3.2/src/ffpack/lcc/astmCounting.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 '''
 This module implements the standard cycle counting methods in 
 ASTM E1049-85(2017) Standard Practices for Cycle Counting in Fatigue Analysis
 '''
 
 import numpy as np
-from ffpack.utils import generalUtils
+from ffpack.utils import sequenceFilter
 from ffpack.config import globalConfig
 from collections import defaultdict, deque
 
+
 def astmLevelCrossingCounting( data, refLevel=0.0, levels=None, aggregate=True ):
     '''
     ASTM level crossing counting in E1049-85: sec 5.1.1.
 
     Parameters
     ----------
     data: 1d array
@@ -54,15 +55,15 @@
         maxElement = np.ceil( np.max( data ) )
         numElement = maxElement - minElement + 1
         levels = np.linspace( minElement, maxElement, numElement.astype(int) )
     else:
         levels = np.array( sorted( set( levels ) ) )
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
 
     rstDict = defaultdict( int )
     rstSeq = [ ]
     # Check each interval
     # Each interval will be searched from small to large value
     for i in range( len( data ) - 1 ):
         intervalStart = data[ i ]
@@ -178,15 +179,15 @@
     data = np.array( data )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2")
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
 
     rstDict = defaultdict( int )
     rstSeq = [ ]
     for i, cur in enumerate( data ):
         if i == 0:
             continue
         prev = data[ i - 1 ]
@@ -233,15 +234,15 @@
     data = np.array( data )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2")
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
 
     dequeA = deque()
     dequeB = deque( [ i for i in data ] )
     S = None
     YContainsS = None
     rstDict = defaultdict( int )
     rstSeq = [ ]
@@ -326,15 +327,15 @@
     data = np.array( data )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2")
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
     indices = np.array( range( -1, len( data ) - 1 ) )
 
     def checkPreviousThree( indices, i ):
         if ( indices[ i ] < 0 ):
             return False
         if ( indices[ indices[ i ] ] < 0 ):
             return False
@@ -428,24 +429,24 @@
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[ 0 ] <= 1:
         raise ValueError( "Input data length should be at least 2")
     if data[ 0 ] != data[ len( data ) - 1 ]:
         raise ValueError( "Input data should be repeating")
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
     # search the peak and shift the data
     index = data.argmax( axis=0 )
     n = len( data )
     if index != 0 or index != n - 1:
         for i in range( index ):
             data[ i ] = data[ i + 1 ]
         data = np.roll( data, -index )
         # need to remove the intermediate value again
-        data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+        data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
 
     indices = np.array( range( -1, len( data ) - 1 ) )
 
     def checkPreviousThree( indices, i ):
         if ( indices[ i ] < 0 ):
             return False
         if ( indices[ indices[ i ] ] < 0 ):
```

### Comparing `ffpack-0.3.1/src/ffpack/lcc/fourPointCounting.py` & `ffpack-0.3.2/src/ffpack/lcc/fourPointCounting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import numpy as np
-from ffpack.utils import generalUtils
+from ffpack.utils import sequenceFilter
 from ffpack.config import globalConfig
 from collections import defaultdict
 
 
 def fourPointRainflowCounting( data, aggregate=True ):
     '''
     Four point rainflow counting in [Lee2011]_.
@@ -40,19 +40,19 @@
     .. [Lee2011] Lee, Y.L., Barkey, M.E. and Kang, H.T., 2011. Metal fatigue analysis 
        handbook: practical problem-solving techniques for computer-aided engineering. 
        Elsevier.
     '''
     data = np.array( data )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
-    if data.shape[0] < 4:
-        raise ValueError( "Input data length should be at least 4")
+    if data.shape[ 0 ] < 4:
+        raise ValueError( "Input data length should be at least 4" )
 
     # Remove the intermediate value first
-    data = np.array( generalUtils.sequencePeakValleyFilter( data, keepEnds=True ) )
+    data = np.array( sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True ) )
     n = len( data )
     indices = np.array( range( 1, n + 1 ) )
     indices[ n - 1 ] = -1
 
     def oneRound( indices, data ):
         rst = [ -1, -1, -1, -1 ]
         first = 0
```

### Comparing `ffpack-0.3.1/src/ffpack/lcc/johannessonCounting.py` & `ffpack-0.3.2/src/ffpack/lcc/johannessonCounting.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 Reference: 
 Johannesson, P., 1998. Rainflow cycles for switching processes with Markov structure. 
 Probability in the Engineering and Informational Sciences, 12(2), pp.143-175.
 '''
 
 import numpy as np
-from ffpack.utils import generalUtils 
+from ffpack.utils import sequenceFilter 
 from ffpack.config import globalConfig
 from collections import defaultdict 
 
+
 def johannessonMinMaxCounting( data, aggregate=True ):
     '''
     Johannesson min-max counting 
 
     Parameters
     ----------
     data: 1d array 
@@ -61,15 +62,15 @@
             left = min( left, data[ j ] )
             j -= 1
 
         return left
 
     # we need to use this util function since it keeps one peak 
     # if there are two or more points together with the same peak value
-    data = generalUtils.sequencePeakValleyFilter( data, keepEnds=True )
+    data = sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True )
     rstSeq = [ ]
     for i in range( 1, len( data ) - 1 ):
         if ( data[ i ] > data[ i - 1 ] and data[ i ] > data[ i + 1 ] ):
             left = getMinLeft( data, i )
             rstSeq.append( [ left, data[ i ], 1 ] )
     
     if ( not aggregate ):
```

### Comparing `ffpack-0.3.1/src/ffpack/lcc/rychlikCounting.py` & `ffpack-0.3.2/src/ffpack/lcc/rychlikCounting.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 required for further analysis.
 
 Reference: Rychlik, I., 1987. A new definition of the rainflow cycle counting method. 
 International journal of fatigue, 9(2), pp.119-121.
 '''
 
 import numpy as np
-from ffpack.utils import generalUtils 
+from ffpack.utils import sequenceFilter 
 from ffpack.config import globalConfig
 from collections import defaultdict 
 
+
 def rychlikRainflowCounting( data, aggregate=True ):
     '''
     Rychilk rainflow counting (toplevel-up cycle TUC)
 
     Parameters
     ----------
     data: 1d array 
@@ -74,18 +75,17 @@
         j = i + 2
         while ( j < len( data ) and data[ j ] < data[ i ] ):
             right = min( right, data[ j ] )
             j += 1
 
         return right 
 
-
     # we need to use this util function since it keeps one peak 
     # if there are two or more points together with the same peak value
-    data = generalUtils.sequencePeakValleyFilter( data, keepEnds=True )
+    data = sequenceFilter.sequencePeakValleyFilter( data, keepEnds=True )
     rstSeq = [ ]
     for i in range( 1, len( data ) - 1 ):
         if ( data[ i ] > data[ i - 1 ] and data[ i ] > data[ i + 1 ] ):
             higher = max( getMinLeft( data, i ), getMinRight( data, i ) )
             rstSeq.append( [ higher, data[ i ], 1 ] )
     
     if ( not aggregate ):
```

### Comparing `ffpack-0.3.1/src/ffpack/lsg/autoregressiveModel.py` & `ffpack-0.3.2/src/ffpack/lsg/autoregressiveMovingAverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
-def arNormal( numSteps, obs, phis, mu, sigma ):
+
+def arNormal( numSteps, obs, phis, mu, sigma, randomSeed=None ):
     '''
     Generate load sequence by an autoregressive model.
 
     The white noise is generated by the normal distribution.
 
     Parameters
     ----------
@@ -16,14 +17,17 @@
         Initial observed values.
     phis: 1d array
         Coefficients for the autoregressive model.
     mu: scalar
         Mean of the white noise.
     sigma: scalar
         Standard deviation of the white noise.
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     rst: 1d array
         Generated sequence includes the observed values.
     
     Raises
@@ -46,30 +50,31 @@
         raise ValueError( "numSteps should be at least 1" )
     if len( obs ) != len( phis ):
         raise ValueError( "lengths of obs and phis should be same" )
     if len( obs ) < 1:
         raise ValueError( "length of obs or phis should be at least 1" )
 
     p = len( obs )
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
     eps = np.random.normal( mu, sigma, numSteps )
 
     rst = [ 0 ] * numSteps
     for i in range( numSteps ):
         if i < p:
             rst[ i ] = obs[ i ]
         else:
             rst[ i ] += eps[ i ]
             for j in range( p ):
                 rst[ i ] += phis[ j ] * rst[ i - j - 1]
     
     return rst
 
 
-
-def maNormal( numSteps, c, thetas, mu, sigma ):
+def maNormal( numSteps, c, thetas, mu, sigma, randomSeed=None ):
     '''
     Generate load sequence by a moving-average model.
 
     The white noise is generated by the normal distribution.
 
     Parameters
     ----------
@@ -79,14 +84,17 @@
         Mean of the series.
     thetas: 1d array
         Coefficients for the white noise in the moving-average model.
     mu: scalar
         Mean of the white noise.
     sigma: scalar
         Standard deviation of the white noise.
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     rst: 1d array
         Generated sequence with moving-average model.
     
     Raises
@@ -108,29 +116,31 @@
     if numSteps < 1:
         raise ValueError( "numSteps should be at least 1" )
     if not isinstance( c, int ) and not isinstance( c, float ):
         raise ValueError( "mean of the series should be a scalar" )
     if len( thetas ) < 1:
         raise ValueError( "length of coefficients for the white noise should be at least 1" )
 
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
     eps = np.random.normal( mu, sigma, numSteps )
 
     rst = [ 0 ] * numSteps
     q = len( thetas )
     for i in range( numSteps ):
         ept = eps[ i ]
         for j in range( q ):
             if ( i > j ): 
                 ept += thetas[ j ] * eps[ i - j - 1 ]
         rst[ i ] = c + ept
     
     return rst
 
 
-def armaNormal( numSteps, obs, phis, thetas, mu, sigma ):
+def armaNormal( numSteps, obs, phis, thetas, mu, sigma, randomSeed=None ):
     '''
     Generate load sequence by an autoregressive-moving-average model.
 
     The white noise is generated by the normal distribution.
 
     Parameters
     ----------
@@ -142,14 +152,17 @@
         Coefficients for the autoregressive part.
     thetas: 1d array
         Coefficients for the white noise for the moving-average part.
     mu: scalar
         Mean of the white noise.
     sigma: scalar
         Standard deviation of the white noise.
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     rst: 1d array
         Generated sequence includes the observed values.
     
     Raises
@@ -176,14 +189,16 @@
         raise ValueError( "length of phis should be at least 1" )
     if len( thetas ) < 1:
         raise ValueError( "length of coefficients for the white noise should be at least 1" )
 
     p = len( phis )
     q = len( thetas )
     n = len( obs )
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
     eps = np.random.normal( mu, sigma, numSteps )
 
     rst = [ 0 ] * numSteps
     if ( n > 0 ):
         for i in range( min( n, numSteps ) ):
             rst[ i ] = obs[ i ]
     
@@ -199,15 +214,15 @@
                 epm += thetas[ j ] * eps[ i - j - 1 ]
         
         rst[ i ] = eps[ i ] + epa + epm 
 
     return rst
 
 
-def arimaNormal( numSteps, c, phis, thetas, mu, sigma ):
+def arimaNormal( numSteps, c, phis, thetas, mu, sigma, randomSeed=None ):
     '''
     Generate load sequence by an autoregressive integrated moving average model.
 
     The white noise is generated by the normal distribution.
 
     First-order diference is used in this function.
 
@@ -221,15 +236,18 @@
         Coefficients for the autoregressive part.
     thetas: 1d array
         Coefficients for the white noise for the moving-average part.
     mu: scalar
         Mean of the white noise.
     sigma: scalar
         Standard deviation of the white noise.
-    
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
+        
     Returns
     -------
     rst: 1d array
         Generated sequence with the autoregressive integrated moving average model.
     
     Raises
     ------
@@ -256,14 +274,16 @@
     if len( phis ) < 1:
         raise ValueError( "length of phis should be at least 1" )
     if len( thetas ) < 1:
         raise ValueError( "length of coefficients for the white noise should be at least 1" )
 
     p = len( phis )
     q = len( thetas )
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
     eps = np.random.normal( mu, sigma, numSteps )
 
     rst = [ 0 ] * numSteps
     
     for i in range( numSteps ):
         epa = 0
         for j in range( p ):
```

### Comparing `ffpack-0.3.1/src/ffpack/lsg/randomWalk.py` & `ffpack-0.3.2/src/ffpack/lsg/randomWalk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
 
-def randomWalkUniform( numSteps, dim=1 ):
+def randomWalkUniform( numSteps, dim=1, randomSeed=None ):
     '''
     Generate load sequence by a random walk.
 
     Parameters
     ----------
     numSteps: integer 
         Number of steps for generating.
     dim: scalar, optional
         Data dimension.
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     rst: 2d array
         A 2d (numSteps by dim) matrix holding the coordinates 
         of the position at each step.
     
@@ -35,14 +38,17 @@
     if not isinstance( numSteps, int ) or not isinstance( dim, int ):
         raise ValueError( "numSteps should be int" )
     if numSteps < 1:
         raise ValueError( "numSteps should be at least 1" )
     if dim < 1:
         raise ValueError( "dim should be at least 1" )
 
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
+    
     rst = [ [ 0 ] * dim ]
     for i in range( numSteps ):
         randomInt = np.random.randint( 2 * dim )
         randomDim = randomInt % dim
         randomDir = 1 if randomInt >= dim else -1
         lastCoords = np.copy( rst[ -1 ] )
         lastCoords[ randomDim ] += randomDir
```

### Comparing `ffpack-0.3.1/src/ffpack/lsg/sequenceFromSpectrum.py` & `ffpack-0.3.2/src/ffpack/lsg/sequenceFromSpectrum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 import numpy as np
-from ffpack.config import globalConfig
 
 
-def spectralRepresentation( fs, time, freq, psd, freqBandwidth=None ):
+def spectralRepresentation( fs, time, freq, psd, freqBandwidth=None, randomSeed=None ):
     '''
     Generate a sequence from a given power spectrum density with spectral
     representation method.
 
     Parameters
     ----------
     fs: scalar 
@@ -19,14 +18,17 @@
         Frequency array for psd.
         The freq array should be in equally spaced increasing. 
     psd: 1darray
         Power spectrum density array. 
     freqBandwidth: scalar, optional
         Frequency bandwidth used to generate the time series from psd.
         Default to None, every frequency in freq will be used. 
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     ts: 1darray
         Array containing all the time data for the time series.
     amps: 1darray
         Amplitude array containing the amplitudes of the time series 
@@ -98,15 +100,18 @@
     if freqBandwidth is None or freqBandwidth < freq[ 1 ] - freq[ 0 ]:
         freqBandwidth = freq[ 1 ] - freq[ 0 ]
     next = round( freqBandwidth / ( freq[ 1 ] - freq[ 0 ] ) )
 
     n = round( fs * time )
     ts = 1 / fs * np.arange( n, dtype=float )
     amps = np.zeros( n )
+
     # generate phase angle
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
     phis = -np.pi + 2 * np.pi * np.random.randn( len( freq ) )
 
     i = 0
     while i < len( freq ):
         for j in range( n ):
             amps[ j ] += np.sqrt( 2 * psd[ i ] * freqBandwidth ) * \
                 np.sin( 2 * np.pi * freq[ i ] * ts[ j ] + phis[ i ] )
```

### Comparing `ffpack-0.3.1/src/ffpack/lsm/cycleCountingMatrix.py` & `ffpack-0.3.2/src/ffpack/lsm/cycleCountingMatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from ffpack.lcc import astmCounting
 from ffpack.lcc import rychlikCounting
 from ffpack.lcc import johannessonCounting
 from ffpack.lcc import fourPointCounting
-from ffpack.utils import generalUtils 
-from ffpack.utils import lsmUtils 
+from ffpack.utils import digitization 
+from ffpack.utils import countingMatrix 
 import numpy as np
 
 
 def astmSimpleRangeCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate ASTM simple range counting matrix.
 
@@ -45,18 +45,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = astmCounting.astmSimpleRangeCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def astmRainflowCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate ASTM rainflow counting matrix.
 
     Parameters
@@ -91,18 +90,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = astmCounting.astmRainflowCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def astmRangePairCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate ASTM range pair counting matrix.
 
     Parameters
@@ -137,18 +135,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = astmCounting.astmRangePairCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def astmRainflowRepeatHistoryCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate ASTM simplified rainflow counting matrix for repeating histories.
 
     Parameters
@@ -184,18 +181,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = astmCounting.astmRainflowRepeatHistoryCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def rychlikRainflowCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate Rychlik rainflow counting matrix.
 
     Parameters
@@ -230,18 +226,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = rychlikCounting.rychlikRainflowCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def johannessonMinMaxCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate Johannesson minMax cycle counting matrix.
 
     Parameters
@@ -276,18 +271,17 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = johannessonCounting.johannessonMinMaxCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
-
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
 
 
 def fourPointCountingMatrix( data, resolution=0.5 ):
     '''
     Calculate Four point cycle counting matrix.
 
     Parameters
@@ -322,10 +316,10 @@
     '''
     data = np.array( data, dtype=float )
     if len( data.shape ) != 1:
         raise ValueError( "Input data dimension should be 1" )
     if data.shape[0] <= 1:
         raise ValueError( "Input data length should be at least 2" )
 
-    data = generalUtils.sequenceDigitization( data, resolution )
+    data = digitization.sequenceDigitization( data, resolution )
     countingRst = fourPointCounting.fourPointRainflowCounting( data, aggregate=False )
-    return lsmUtils.countingRstToCountingMatrix( countingRst )
+    return countingMatrix.countingRstToCountingMatrix( countingRst )
```

### Comparing `ffpack-0.3.1/src/ffpack/lsm/sequenceSpectra.py` & `ffpack-0.3.2/src/ffpack/lsm/sequenceSpectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     if not isinstance( fs, int ) and not isinstance( fs, float ):
         raise ValueError( "fs should be a scalar" )
 
     ( freq, psd ) = signal.periodogram( data, fs, scaling='density' )
     return freq, psd
 
 
-
 def welchSpectrum( data, fs, nperseg=1024 ):
     '''
     Power spectral density with `scipy.signal.welch`.
 
     Parameters
     ----------
     data: 1darray
```

### Comparing `ffpack-0.3.1/src/ffpack/lsm/waveSpectra.py` & `ffpack-0.3.2/src/ffpack/lsm/waveSpectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         raise ValueError( "Uw should be a scalar" )
 
     rst = alpha * g * g / np.power( w, 5 ) * \
         np.exp( -beta * np.power( ( g / Uw ) / w, 4 ) )
     return rst
 
 
-
 def jonswapSpectrum( w, wp, alpha=0.0081, beta=1.25, gamma=3.3, g=9.81 ):
     '''
     JONSWAP (Joint North Sea Wave Project) spectrum is an empirical relationship 
     that defines the distribution of energy with frequency within the ocean.
 
     Parameters
     ----------
@@ -102,15 +101,14 @@
         sigma = 0.09
     r = np.exp( -( w - wp ) * ( w - wp ) / ( 2 * wp * wp * sigma * sigma ) )
     rst = alpha * g * g / np.power( w, 5 ) * \
         np.exp( -beta * np.power( wp / w, 4 ) ) * np.power( gamma, r )
     return rst
 
 
-
 def isscSpectrum( w, wp, Hs ):
     '''
     ISSC spectrum, also known as Bretschneider or modified Pierson-Moskowitz. 
 
     Parameters
     ----------
     w: scalar
@@ -148,15 +146,14 @@
         raise ValueError( "Hs should be a scalar" )
     
     wwp4 = np.power( wp / w, 4 )
     rst = 5 / 16 * Hs * Hs * wwp4 / w * np.exp( -1.25 * wwp4 )
     return rst
 
 
-
 def gaussianSwellSpectrum( w, wp, Hs, sigma ):
     '''
     Gaussian Swell spectrum, typically used to model long period 
     swell seas [Guidance2016A]_. 
 
     Parameters
     ----------
@@ -207,15 +204,14 @@
     
     twoPi = 2 * np.pi
     pexp = np.power( ( w - wp ) / ( twoPi * sigma ), 2 ) / 2
     rst = Hs * Hs / ( 16 * sigma * np.power( twoPi, 1.5 ) ) * np.exp( -pexp )
     return rst
 
 
-
 def ochiHubbleSpectrum( w, wp1, wp2, Hs1, Hs2, lambda1, lambda2 ):
     '''
     Ochi-Hubble spectrum covers shapes of wave spectra associated with the growth 
     and decay of a storm, including swells. [Guidance2016B]_. 
 
     Parameters
     ----------
@@ -275,15 +271,14 @@
         raise ValueError( "Hs2 should be a scalar" )
     if not isinstance( lambda1, int ) and not isinstance( lambda1, float ):
         raise ValueError( "lambda1 should be a scalar" )
     if not isinstance( lambda2, int ) and not isinstance( lambda2, float ):
         raise ValueError( "lambda2 should be a scalar" )
     if wp1 >= wp2:
         raise ValueError( "wp1 must be less than wp2" )
-
     
     def oneTerm( w, wp, Hs, lambdaVal ):
         fourLambda = ( 4 * lambdaVal + 1 ) / 4
         firstPart = np.power( fourLambda * np.power( wp, 4 ), lambdaVal ) / \
             special.gamma( lambdaVal )
         expc = np.exp( -fourLambda * np.power( wp / w, 4 ) )
         rst = firstPart * Hs * Hs / np.power( w, fourLambda * 4 ) * expc
```

### Comparing `ffpack-0.3.1/src/ffpack/lsm/windSpectra.py` & `ffpack-0.3.2/src/ffpack/lsm/windSpectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         return rightPart( x )
     
     x = 1200 * n / delta1
     rst = rightPart( x ) * kappa * delta1 * delta1 / n
     return rst
 
 
-
 def davenportSpectrumWithRoughnessLength( n, uz, z=10, z0=0.03, normalized=True ):
     '''
     Davenport spectrum in the paper by Hiriart et al. [Hiriart2001]_.
 
     Parameters
     ----------
     n: scalar
@@ -132,15 +131,14 @@
     
     x = 1200 * n / uz
     uf = 0.4 * uz / np.log( z / z0 )
     rst = rightPart( x ) * uf * uf / n
     return rst
 
 
-
 def ec1Spectrum( n, uz, sigma=0.03, z=10, tcat=0, normalized=True ):
     '''
     EC1 spectrum is implemented according to Annex B [EN1991-1-42005]_.
 
     Parameters
     ----------
     n: scalar
@@ -208,15 +206,14 @@
     alpha = 0.67 + 0.05 * np.log( z0 )
     lz = 300 * np.power( max( z, zmin ) / 200, alpha )
     f = n * lz / uz
     rst = rightPart( f ) * sigma * sigma / n
     return rst
 
 
-
 def iecSpectrum( f, vhub, sigma=0.03, z=10, k=1, normalized=True ):
     '''
     IEC spectrum is implemented according to [IEC2005]_.
 
     Parameters
     ----------
     f: scalar
@@ -287,15 +284,14 @@
     sigmak = factors[ 0 ] * sigma
     lk = factors[ 1 ] * lambda1
     nf = f * lk / vhub
     rst = rightPart( nf ) * sigmak * sigmak / f
     return rst
 
 
-
 def apiSpectrum( f, u0, z=10 ):
     '''
     API spectrum is implemented according to [API2007]_.
 
     Parameters
     ----------
     f: scalar
```

### Comparing `ffpack-0.3.1/src/ffpack/rpm/metropolisHastings.py` & `ffpack-0.3.2/src/ffpack/rpm/metropolisHastings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
+
 class MetropolisHastingsSampler:
     '''
     Metropolis-Hastings sampler to sample data [Bourinet2018]_.
 
     References
     ----------
     .. [Bourinet2018] Bourinet, J.M., 2018. Reliability analysis and optimal design 
        under uncertainty-Focus on adaptive surrogate-based approaches (Doctoral 
        dissertation, Université Clermont Auvergne).
     '''
     def __init__( self, initialVal=None, targetPdf=None, proposalCSampler=None, 
-                  sampleDomain=None, **sdKwargs ):
+                  sampleDomain=None, randomSeed=None, **sdKwargs ):
         r'''
         Initialize the Metropolis-Hastings sampler
         
         Parameters
         ----------
         initialVal: scalar or array_like
             Initial observed data point.
@@ -31,20 +32,23 @@
             is a sampler that will return a sample for the given observed data point. 
             A usual choice is to let proposalCSampler be a Gaussian/normal 
             distribution centered at the observed data point. It will be called as 
             proposalCSampler( X ) where X is the same type as initialVal, and a 
             sample with the same type of initialVal should be returned.
         sampleDomain: function, optional
             Sample domain function. sampleDomain is a function to determine if a
-            sample is in the sample domain. For example, it the sample doamin is 
+            sample is in the sample domain. For example, if the sample doamin is 
             [ 0, inf ] and the sample is -2, the sample will be rejected. For the 
             sampling on field of real numbers, it should return True regardless of 
             the sample value. It called as sampleDomain( cur, nxt, \**sdKwargs ) 
             where cur, nxt are the same type as initivalVal, and a boolean value 
             should be returned.
+        randomSeed: integer, optional
+            Random seed. If randomSeed is none or is not an integer, the random seed in 
+            global config will be used. 
         
         Raises
         ------
         ValueError
             If initialVal, targetPdf, or proposalCSampler is None.
             If targetPdf returns negative value.
 
@@ -67,14 +71,16 @@
         if sampleDomain is None:
             sampleDomain = lambda cur, nxt, **sdKwargs: True
         self.cur = np.copy( initialVal ).astype( float )
         self.nxt = np.copy( initialVal ).astype( float )
         self.targetPdf = targetPdf
         self.proposalCSampler = proposalCSampler
         self.sampleDomain = sampleDomain
+        if isinstance( randomSeed, ( int, type( None ) ) ):
+            np.random.seed( randomSeed )
     
     def getAcceptanceRatio( self, candi ):
         fcur = self.targetPdf( self.cur )
         fcandi = self.targetPdf( candi )
         if fcur < 0 or fcandi < 0:
             raise ValueError( "targetPdf cannot return negative value" )
         return fcandi / fcur
@@ -114,15 +120,15 @@
     References
     ----------
     .. [Au2001] Au, S.K. and Beck, J.L., 2001. Estimation of small failure 
        probabilities in high dimensions by subset simulation. Probabilistic 
        engineering mechanics, 16(4), pp.263-277.
     '''
     def __init__( self, initialVal=None, targetPdf=None, proposalCSampler=None, 
-                  sampleDomain=None, **sdKwargs ):
+                  sampleDomain=None, randomSeed=None, **sdKwargs ):
         r'''
         Initialize the Au modified Metropolis-Hastings sampler
         
         Parameters
         ----------
         initialVal: array_like
             Initial observed data point.
@@ -140,21 +146,24 @@
             data point.  A usual choice is to let proposalCSampler[ i ] be a 
             Gaussian/normal distribution centered at the observed data point. 
             It will be called as proposalCSampler[ i ]( X[ i ] ) where X is a list 
             in which each element is the same type as initialVal[ i ], and a 
             sample with the same type of initialVal[ i ] should be returned.
         sampleDomain: function, optional
             Sample domain function. sampleDomain is a function to determine if a
-            sample is in the sample domain. For example, it the sample doamin is 
+            sample is in the sample domain. For example, if the sample doamin is 
             [ 0, inf ] and the sample is -2, the sample will be rejected. For the 
             sampling on field of real numbers, it should return True regardless of 
             the sample value. It called as sampleDomain( cur, nxt, \**sdKwargs ) 
             where cur, nxt are lists in which each element is the same type as 
             initivalVal[ i ], and a boolean value should be returned.
-        
+        randomSeed: integer, optional
+            Random seed. If randomSeed is none or is not an integer, the random seed in 
+            global config will be used. 
+
         Raises
         ------
         ValueError
             If initialVal, targetPdf, or proposalCSampler is None.
             If dims of initialVal, targetPdf, and proposalCSampler are not equal.
             If targetPdf returns negative value.
 
@@ -185,15 +194,17 @@
             raise ValueError( "dimensions of initialVal, targetPdf, and "
                               "proposalCSampler should be equal." )
         self.cur = np.copy( initialVal ).astype( float )
         self.nxt = np.copy( initialVal ).astype( float )
         self.targetPdf = targetPdf
         self.proposalCSampler = proposalCSampler
         self.sampleDomain = sampleDomain
-    
+        if isinstance( randomSeed, ( int, type( None ) ) ):
+            np.random.seed( randomSeed )
+        
     def getAcceptanceRatio( self, candi, i ):
         fcur = self.targetPdf[ i ]( self.cur[ i ] )
         fcandi = self.targetPdf[ i ]( candi )
         if fcur < 0 or fcandi < 0:
             raise ValueError( f"targetPdf[ { i } ] cannot return negative value" )
         return fcandi / fcur
```

### Comparing `ffpack-0.3.1/src/ffpack/rpm/nataf.py` & `ffpack-0.3.2/src/ffpack/rpm/nataf.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,20 @@
        estimate method. Chinese Science Bulletin, 53(17), pp.2586-2592.
 
 '''
 
 import numpy as np
 from scipy import stats, optimize
 
+
 class NatafTransformation:
     '''
     Nataf distribution for correlated marginal distributions.
     '''
-    def __init__( self, distObjs, corrMat, quadDeg=99, quadRange=8 ):
+    def __init__( self, distObjs, corrMat, quadDeg=99, quadRange=8, randomSeed=None ):
         '''
         Initialize the Nataf distribution.
         
         Parameters
         ----------
         distObjs: array_like of distributions
             Marginal distribution objects. It should be the freezed distribution 
@@ -42,14 +43,17 @@
         corrMat: 2d matrix
             Correlation matrix of the marginal distributions.
         quadDeg: integer
             Quadrature degree.
         quadRange: scalar
             Quadrature range. The integral will be performed in the range
             [ -quadRange, quadRange ].
+        randomSeed: integer, optional
+            Random seed. If randomSeed is none or is not an integer, the random seed in 
+            global config will be used. 
         
         Raises
         ------
         ValueError
             If distObjs is empty.
             If dimensions are not match for distObjs and corrMat.
             If corrMat is not 2d matrix.
@@ -83,14 +87,17 @@
             raise ValueError( "corrMat should be symmetric" )
         
         try:
             _ = np.linalg.cholesky( corrMat )
         except np.linalg.LinAlgError:
             raise ValueError( "corrMat should be positive definite" )
 
+        if isinstance( randomSeed, ( int, type( None ) ) ):
+            np.random.seed( randomSeed )
+        
         self.distObjs = distObjs
         self.rhoX = np.array( corrMat )
         self.dim = len( distObjs )
         self.deg = quadDeg
         self.ran = quadRange
 
         self.rhoZ = np.identity( self.dim )
```

### Comparing `ffpack-0.3.1/src/ffpack/rrm/firstOrderReliabilityMethod.py` & `ffpack-0.3.2/src/ffpack/rrm/firstOrderReliabilityMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import numpy as np
 from scipy import stats, optimize
 from ffpack.utils import gradient
 from ffpack import rpm
 
+
 def hlrfFORM( dim, g, dg, distObjs, corrMat, iter=1000, tol=1e-6, 
               quadDeg=99, quadRange=8, dx=1e-6 ):
     '''
     First order reliability method based on Hasofer-Lind-Rackwitz-Fiessler algorithm.
 
     Parameters
     ----------
```

### Comparing `ffpack-0.3.1/src/ffpack/rrm/firstOrderSecondMoment.py` & `ffpack-0.3.2/src/ffpack/rrm/firstOrderSecondMoment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import numpy as np
 from scipy import stats
 from ffpack.utils import gradient
 
+
 def mvalFOSM( dim, g, dg, mus, sigmas, dx=1e-6 ):
     '''
     First order second moment method based on mean value algorithm.
 
     Parameters
     ----------
     dim: integer
```

### Comparing `ffpack-0.3.1/src/ffpack/rrm/secondOrderReliabilityMethod.py` & `ffpack-0.3.2/src/ffpack/rrm/secondOrderReliabilityMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 from scipy import stats
 from ffpack.utils import gradient, hessianMatrix, gramSchmidOrth
 from ffpack.rrm import firstOrderReliabilityMethod
 from ffpack import rpm
 
+
 def mainCurvaturesAtDesignPoint( dim, g, dg, distObjs, corrMat, 
                                  quadDeg=99, quadRange=8, dx=1e-6 ):
     # This function is internal use only.
     # Return curvature, beta, uCoord, xCoord based on the FORM.
     # Check edge cases
     if dim < 1:
         raise ValueError( "dim cannot be less than 1" )
@@ -60,14 +61,15 @@
 
     HBH = np.dot( np.dot( H, lsfHmAtU / lsfGradNormAtU ), H.T )
     eigVal = np.linalg.eig( HBH[ : dim - 1, : dim - 1 ] )
     ks = eigVal[ 0 ].tolist()
 
     return ks, beta, uCoord, xCoord
 
+
 def breitungSORM( dim, g, dg, distObjs, corrMat, quadDeg=99, quadRange=8, dx=1e-6 ):
     '''
     Second order reliability method based on Breitung algorithm.
 
     Parameters
     ----------
     dim: integer
```

### Comparing `ffpack-0.3.1/src/ffpack/rrm/simulationBasedReliabilityMethod.py` & `ffpack-0.3.2/src/ffpack/rrm/simulationBasedReliabilityMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 import numpy as np
 from scipy.stats import norm
 from ffpack.rpm import metropolisHastings, nataf
 
+
 def subsetSimulation( dim, g, distObjs, corrMat, numSamples, 
-                      maxSubsets, probLevel=0.1, quadDeg=99, quadRange=8 ):
+                      maxSubsets, probLevel=0.1, quadDeg=99, quadRange=8, randomSeed=None ):
     '''
     Second order reliability method based on Breitung algorithm.
 
     Parameters
     ----------
     dim: integer
         Space dimension ( number of random variables ).
@@ -27,14 +28,17 @@
     probLevel: scalar, optional
         Probability level for intermediate subsets.
     quadDeg: integer, optional
         Quadrature degree for Nataf transformation
     quadRange: scalar, optional
         Quadrature range for Nataf transformation. The integral will be performed 
         in the range [ -quadRange, quadRange ].
+    randomSeed: integer, optional
+        Random seed. If randomSeed is none or is not an integer, the random seed in 
+        global config will be used. 
     
     Returns
     -------
     pf: scalar
         Probability of failure.
     allLsfValue: array_like
         Values of limit state function in each subset.
@@ -96,14 +100,17 @@
 
     # Define paramters for MCMC sampling
     def tpdf( x ):
         return norm.pdf( x )
     
     targetPdf = [ tpdf ] * dim
     
+    if isinstance( randomSeed, ( int, type( None ) ) ):
+        np.random.seed( randomSeed )
+    
     def pcs( x ):
         return x - 0.5 + np.random.uniform()
     
     proposalCSampler = [ pcs ] * dim 
 
     def sampleDomainFunc( curU, nxtU, **kwargs ):
         lsfFunc = kwargs[ 'lsfFunc' ]
```

### Comparing `ffpack-0.3.1/src/ffpack/utils/fdrUtils.py` & `ffpack-0.3.2/src/ffpack/utils/fitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
+
 class SnCurveFitter:
     '''
     Fitter for a SN curve based on the experimental data.
     '''
     def __init__( self, data, fatigueLimit ):
         '''
         Initialize a fitter for a SN curve based on the experimental data.
```

### Comparing `ffpack-0.3.1/src/ffpack/utils/generalUtils.py` & `ffpack-0.3.2/src/ffpack/utils/sequenceFilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,15 +56,14 @@
                ( prev > cur and cur < next ):
                 rst.append( cur )
                 prev = cur
         
     return rst
 
 
-
 def sequenceHysteresisFilter( data, gateSize ):
     '''
     Filter data within the gateSize.
 
     Any cycle that has an amplitude smaller than the gate is removed from the data. 
     This is done by scan the data, i.e., point i, to check if the next points, 
     i.e., i + 1, i + 2, ... are within the gate from point i. 
@@ -140,55 +139,7 @@
     
     rst = [ ]
     for i in range( n ):
         if ( keep[ i ] > 0 ):
             rst.append( data[ i ] )
     
     return rst
-
-
-
-def sequenceDigitization( data, resolution=1.0 ):
-    '''
-    Digitize the sequence data to a specific resolution
-
-    The sequence data are digitized by the round method. 
-
-    Parameters
-    ----------
-    data: 1d array
-        Sequence data to digitize.
-    
-    resolution: bool, optional
-        The desired resolution to round the data points.
-    
-    Returns
-    -------
-    rst: 1d array
-        A list contains the digitized data.
-    
-    Raises
-    ------
-    ValueError
-        If the data dimension is not 1.
-        If the data length is less than 2 with keedEnds == False
-        If the data length is less than 3 with keedEnds == True
-
-    Notes
-    -----
-    The default round function will round half to even: 1.5, 2.5 => 2.0:
-
-    Examples
-    --------
-    >>> from ffpack.utils import sequenceDigitization 
-    >>> data = [ -1.0, 2.3, 1.8, 0.6, -0.4, 0.8, -1.6, -2.5, 3.4, 0.3, 0.1 ]
-    >>> rst = sequenceDigitization( data )
-    '''
-    # Egde cases
-    data = np.array( data, dtype=float )
-    if len( data.shape ) != 1:
-        raise ValueError( "Input data dimension should be 1" )
-
-    rst = [ ]
-    for d in data:
-        rst.append( np.rint( d / resolution) * resolution )
-    return rst
```

### Comparing `ffpack-0.3.1/src/ffpack/utils/lccUtils.py` & `ffpack-0.3.2/src/ffpack/utils/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import numpy as np
 from collections import defaultdict
 
+
 def cycleCountingAggregation( data, binSize=1.0 ):
     '''
     Count the number of occurrences of each cycle digitized to the nearest bin.
 
     Parameters
     ----------
     data: 2d array
```

### Comparing `ffpack-0.3.1/src/ffpack/utils/lsmUtils.py` & `ffpack-0.3.2/src/ffpack/utils/countingMatrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Examples
     --------
     >>> from ffpack.lsm import countingRstToCountingMatrix
     >>> countingRst = [ [ -2.0, 1.0, 1.0 ], [ 5.0, -1.0, 3.0 ], [ -4.0, 4.0, 0.5 ] ]
     >>> rst, matrixIndexKey = countingRstToCountingMatrix( countingRst )
     '''
-    countingRst = np.array( countingRst )
+    countingRst = np.array( countingRst ) + 0.0
     if len( countingRst.shape ) != 2:
         raise ValueError( "Input data dimension should be 2" )
     if countingRst.shape[ 1 ] != 0 and len( countingRst[ 0 ] ) != 3:
         raise ValueError( "Input data should be either empty or in dimension of n by 3")
     
     matrixIndexKey = np.unique( np.array( countingRst )[ :, 0: 2 ].flatten() )
     matrixIndexKey = [ "{1:,.{0}f}".format( globalConfig.atol, key ) for key in matrixIndexKey ]
```

### Comparing `ffpack-0.3.1/src/ffpack/utils/miscUtils.py` & `ffpack-0.3.2/src/ffpack/utils/derivatives.py`

 * *Files identical despite different names*

### Comparing `ffpack-0.3.1/setup.py` & `ffpack-0.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,178 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ffpack
+Version: 0.3.2
+Summary: Fatigue and fracture package
+Home-page: https://pypi.org/project/ffpack
+Keywords: fatigue,fracture,load,reliability
+Author: Dongping Zhu
+Maintainer: Dongping Zhu
+Requires-Python: >=3.7,<3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: scipy (>=1.2,<1.8) ; python_version == "3.7"
+Requires-Dist: scipy (>=1.8,<2.0) ; python_version >= "3.8" and python_version < "3.11"
+Project-URL: Documentation, https://ffpack.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/dpzhuX/ffpack
+Description-Content-Type: text/markdown
+
+# FFPACK - Fatigue and Fracture PACKage
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dpzhuX/ffpack/python-package.yml?color=brightgreen&label=Test&logo=github&logoColor=white)
+![PyPI](https://img.shields.io/pypi/v/ffpack?color=brightgreen&label=PyPI&logo=python&logoColor=white)
+![GitHub](https://img.shields.io/github/license/dpzhuX/ffpack?color=brightgreen&logo=gnu&label=License&logoColor=white)
+![Read the Docs](https://img.shields.io/readthedocs/ffpack?color=brigthgreen&label=Docs&logo=read%20the%20docs&logoColor=white)
+[![Downloads](https://static.pepy.tech/personalized-badge/ffpack?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/ffpack)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.7478424-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.7478424)
+
+
+## Purpose
+`FFPACK` ( Fatigue and Fracture PACKage ) is an open-source Python library for fatigue and fracture analysis. It supports ASTM cycle counting, load sequence generation, fatigue damage evaluation, etc. A lot of features are under active development. `FFPACK` is designed to help engineers analyze fatigue and fracture behavior in engineering practice.
+
+## Installation
+
+`FFPACK` can be installed via [PyPI](https://pypi.org/project/ffpack/):
+
+```bash
+pip install ffpack
+```
+
+## Usage
+
+The following example shows the usage of ASTM rainflow counting,
+
+```python
+# Import the ASTM rainflow counting function
+from ffpack.lcc import astmRainflowCounting
+
+# Prepare the data
+data = [ -2.0, 1.0, -3.0, 5.0, -1.0, 3.0, -4.0, 4.0, -2.0 ]
+
+# Get counting results
+results = astmRainflowCounting( data )
+```
+
+See the package document for more details and examples.
+
+## Status
+
+`FFPACK` is currently under active development. 
+
+## Contents
+
+* Fatigue damage model
+    * Palmgren-miner damage model
+        * Naive Palmgren-miner damage model
+        * Classic Palmgren-miner damage model
+
+* Load counting and correction
+    * ASTM counting
+        * ASTM level crossing counting
+        * ASTM peak counting
+        * ASTM simple range counting
+        * ASTM range pair counting
+        * ASTM rainflow counting
+        * ASTM rainflow counting for repeating history
+    * Johannesson counting
+        * Johannesson min max counting
+    * Rychlik counting
+        * Rychlik rainflow counting
+    * Four point counting
+        * Four point rainflow counting
+    * Mean stress correction
+        * Goodman correction
+        * Soderberg correction
+        * Gerber correction
+
+* Load sequence generator
+    * Random walk
+        * Uniform random walk
+    * Autoregressive moving average model
+        * Normal autoregressive (AR) model
+        * Normal moving average (MA) model
+        * Normal ARMA model
+        * Normal ARIMA model
+    * Sequence from spectrum
+        * Spectral representation
+
+* Load spectra and matrices
+    * Cycle counting matrix
+        * ASTM simple range counting matrix
+        * ASTM range pair counting matrix
+        * ASTM rainflow counting matrix
+        * ASTM rainflow counting matrix for repeating history
+        * Johannesson min max counting matrix
+        * Rychlik rainflow counting matrix
+        * Four point rainflow counting matrix
+    * Wave spectra
+        * Jonswap spectrum
+        * Pierson Moskowitz spectrum
+        * ISSC spectrum
+        * Gaussian Swell spectrum
+        * Ochi-Hubble spectrum
+    * Wind spectra
+        * Davenport spectrum with drag coefficient
+        * Davenport spectrum with roughness length
+        * EC1 spectrum
+        * IEC spectrum
+        * API spectrum
+    * Sequence spectra
+        * Periodogram spectrum
+        * Welch spectrum
+
+* Random and probabilistic model
+    * Metropolis-Hastings algorithm
+        * Metropolis-Hastings sampler
+        * Au modified Metropolis-Hastings sampler
+    * Nataf algorithm
+        * Nataf transformation
+
+* Risk and reliability model
+    * First order second moment
+        * Mean value FOSM
+    * First order reliability method
+        * Hasofer-Lind-Rackwitz-Fiessler FORM
+        * Constrained optimization FORM
+    * Second order reliability method
+        * Breitung SORM
+        * Tvedt SORM
+        * Hohenbichler and Rackwitz SORM
+    * Simulation based reliability method
+        * Subset simulation
+
+* Utility 
+    * Aggregation
+        * Cycle counting aggregation
+    * Counting matrix
+        * Counting results to counting matrix
+    * Derivatives
+        * Derivative
+        * Central derivative weights
+        * Gradient
+        * Hessian matrix
+    * Digitization
+        * Sequence digitization
+    * Fitter
+        * SN curve fitter
+    * Sequence filter
+        * Sequence peakValley filter
+        * Sequence hysteresis filter
+    
+## Document
+
+You can find the latest documentation for setting up `FFPACK` at the [Read the Docs site](https://ffpack.readthedocs.io/en/latest/).
 
-package_dir = \
-{'': 'src'}
+## Credits
 
-packages = \
-['ffpack',
- 'ffpack.fdm',
- 'ffpack.lcc',
- 'ffpack.lsg',
- 'ffpack.lsm',
- 'ffpack.rpm',
- 'ffpack.rrm',
- 'ffpack.utils']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':python_version == "3.7"': ['scipy>=1.2,<1.8'],
- ':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.8,<2.0']}
-
-setup_kwargs = {
-    'name': 'ffpack',
-    'version': '0.3.1',
-    'description': 'Fatigue and fracture package',
-    'long_description': '# FFPACK - Fatigue and Fracture PACKage\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dpzhuX/ffpack/python-package.yml?color=brightgreen&label=Test&logo=github&logoColor=white)\n![PyPI](https://img.shields.io/pypi/v/ffpack?color=brightgreen&label=PyPI&logo=python&logoColor=white)\n![GitHub](https://img.shields.io/github/license/dpzhuX/ffpack?color=brightgreen&logo=gnu&label=License&logoColor=white)\n![Read the Docs](https://img.shields.io/readthedocs/ffpack?color=brigthgreen&label=Docs&logo=read%20the%20docs&logoColor=white)\n[![Downloads](https://static.pepy.tech/personalized-badge/ffpack?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/ffpack)\n[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.7478424-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.7478424)\n\n\n## Purpose\n`FFPACK` ( Fatigue and Fracture PACKage ) is an open-source Python library for fatigue and fracture analysis. It supports ASTM cycle counting, load sequence generation, fatigue damage evaluation, etc. A lot of features are under active development. `FFPACK` is designed to help engineers analyze fatigue and fracture behavior in engineering practice.\n\n## Installation\n\n`FFPACK` can be installed via [PyPI](https://pypi.org/project/ffpack/):\n\n```bash\npip install ffpack\n```\n\n## Usage\n\nThe following example shows the usage of ASTM rainflow counting,\n\n```python\n# Import the ASTM rainflow counting function\nfrom ffpack.lcc import astmRainflowCounting\n\n# Prepare the data\ndata = [ -2.0, 1.0, -3.0, 5.0, -1.0, 3.0, -4.0, 4.0, -2.0 ]\n\n# Get counting results\nresults = astmRainflowCounting( data )\n```\n\nSee the package document for more details and examples.\n\n## Status\n\n`FFPACK` is currently under active development. \n\n## Contents\n\n* Fatigue damage model\n    * Palmgren-miner damage model\n        * Naive Palmgren-miner damage model\n        * Classic Palmgren-miner damage model\n\n* Load correction and counting\n    * ASTM counting\n        * ASTM level crossing counting\n        * ASTM peak counting\n        * ASTM simple range counting\n        * ASTM range pair counting\n        * ASTM rainflow counting\n        * ASTM rainflow counting for repeating history\n    * Johannesson counting\n        * Johannesson min max counting\n    * Rychlik counting\n        * Rychlik rainflow counting\n    * Four point counting\n        * Four point rainflow counting\n\n* Load sequence generator\n    * Random walk\n        * Uniform random walk\n    * Autoregressive moving average model\n        * Normal autoregressive (AR) model\n        * Normal moving average (MA) model\n        * Normal ARMA model\n        * Normal ARIMA model\n    * Sequence from spectrum\n        * Spectral representation\n\n* Load spectra and matrices\n    * Cycle counting matrix\n        * ASTM simple range counting matrix\n        * ASTM range pair counting matrix\n        * ASTM rainflow counting matrix\n        * ASTM rainflow counting matrix for repeating history\n        * Johannesson min max counting matrix\n        * Rychlik rainflow counting matrix\n        * Four point rainflow counting matrix\n    * Wave spectra\n        * Jonswap spectrum\n        * Pierson Moskowitz spectrum\n        * ISSC spectrum\n        * Gaussian Swell spectrum\n        * Ochi-Hubble spectrum\n    * Wind spectra\n        * Davenport spectrum with drag coefficient\n        * Davenport spectrum with roughness length\n        * EC1 spectrum\n        * IEC spectrum\n        * API spectrum\n    * Sequence spectra\n        * Periodogram spectrum\n        * Welch spectrum\n\n* Random and probabilistic model\n    * Metropolis-Hastings algorithm\n        * Metropolis-Hastings sampler\n        * Au modified Metropolis-Hastings sampler\n    * Nataf algorithm\n        * Nataf transformation\n\n* Risk and reliability model\n    * First order second moment\n        * Mean value FOSM\n    * First order reliability method\n        * Hasofer-Lind-Rackwitz-Fiessler FORM\n        * Constrained optimization FORM\n    * Second order reliability method\n        * Breitung SORM\n        * Tvedt SORM\n        * Hohenbichler and Rackwitz SORM\n    * Simulation based reliability method\n        * Subset simulation\n\n* Utility \n    * Aggregation\n        * Cycle counting aggregation\n    * Counting matrix\n        * Counting results to counting matrix\n    * Fitter\n        * SN curve fitter\n    * Sequence filter\n        * Sequence peakValley filter\n        * Sequence hysteresis filter\n    * Degitization\n        * Sequence degitization\n    * Derivatives\n        * Derivative\n        * Central derivative weights\n        * Gradient\n        * Hessian matrix\n\n## Document\n\nYou can find the latest documentation for setting up `FFPACK` at the [Read the Docs site](https://ffpack.readthedocs.io/en/latest/).\n\n## Credits\n\nThis project was made possible by the help from [DM2L lab](https://dm2l.uconn.edu/).\n\n## License\n\n[GPLv3](https://github.com/dpzhuX/ffpack/blob/main/LICENSE)\n',
-    'author': 'Dongping Zhu',
-    'author_email': 'None',
-    'maintainer': 'Dongping Zhu',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/ffpack',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<3.12',
-}
+This project was made possible by the help from [DM2L lab](https://dm2l.uconn.edu/).
 
+## License
+
+[GPLv3](https://github.com/dpzhuX/ffpack/blob/main/LICENSE)
 
-setup(**setup_kwargs)
```

