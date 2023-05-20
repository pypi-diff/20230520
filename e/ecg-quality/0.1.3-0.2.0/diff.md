# Comparing `tmp/ecg_quality-0.1.3.tar.gz` & `tmp/ecg_quality-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecg_quality-0.1.3.tar", last modified: Wed May 10 08:12:38 2023, max compression
+gzip compressed data, was "ecg_quality-0.2.0.tar", last modified: Sat May 20 19:54:26 2023, max compression
```

## Comparing `ecg_quality-0.1.3.tar` & `ecg_quality-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.320969 ecg_quality-0.1.3/
--rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3296 2023-05-10 08:12:38.320969 ecg_quality-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2023-05-10 07:54:02.000000 ecg_quality-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.293178 ecg_quality-0.1.3/ecg_quality/
--rw-rw-rw-   0        0        0    10411 2023-05-10 08:09:39.000000 ecg_quality-0.1.3/ecg_quality/ECGQualityChecker.py
--rw-rw-rw-   0        0        0       41 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/__init__.py
--rw-rw-rw-   0        0        0      807 2023-04-22 20:35:15.000000 ecg_quality-0.1.3/ecg_quality/model.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.319927 ecg_quality-0.1.3/ecg_quality/models/
--rw-rw-rw-   0        0        0   128640 2023-04-29 16:55:23.000000 ecg_quality-0.1.3/ecg_quality/models/CNN2s.h5
--rw-rw-rw-   0        0        0  7528704 2023-05-02 21:37:58.000000 ecg_quality-0.1.3/ecg_quality/models/CNN5s.h5
--rw-rw-rw-   0        0        0  1224424 2023-04-29 16:55:22.000000 ecg_quality-0.1.3/ecg_quality/models/LSTM2s.h5
--rw-rw-rw-   0        0        0   472672 2023-05-05 11:00:32.000000 ecg_quality-0.1.3/ecg_quality/models/OSCNN2s.h5
--rw-rw-rw-   0        0        0        0 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/models/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/tf_model.py
--rw-rw-rw-   0        0        0     1140 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.301756 ecg_quality-0.1.3/ecg_quality.egg-info/
--rw-rw-rw-   0        0        0     3296 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-10 08:12:38.322937 ecg_quality-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-05-10 08:03:01.000000 ecg_quality-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:54:26.667323 ecg_quality-0.2.0/
+-rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3704 2023-05-20 19:54:26.667323 ecg_quality-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3186 2023-05-10 13:17:08.000000 ecg_quality-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 19:54:25.992050 ecg_quality-0.2.0/ecg_quality/
+-rw-rw-rw-   0        0        0    11857 2023-05-20 19:48:25.000000 ecg_quality-0.2.0/ecg_quality/ECGQualityChecker.py
+-rw-rw-rw-   0        0        0       41 2023-05-10 07:25:34.000000 ecg_quality-0.2.0/ecg_quality/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-04-22 20:35:15.000000 ecg_quality-0.2.0/ecg_quality/model.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:54:26.665289 ecg_quality-0.2.0/ecg_quality/models/
+-rw-rw-rw-   0        0        0   128640 2023-04-29 16:55:23.000000 ecg_quality-0.2.0/ecg_quality/models/CNN2s.h5
+-rw-rw-rw-   0        0        0  7528704 2023-05-02 21:37:58.000000 ecg_quality-0.2.0/ecg_quality/models/CNN5s.h5
+-rw-rw-rw-   0        0        0  1224424 2023-04-29 16:55:22.000000 ecg_quality-0.2.0/ecg_quality/models/LSTM2s.h5
+-rw-rw-rw-   0        0        0   472672 2023-05-05 11:00:32.000000 ecg_quality-0.2.0/ecg_quality/models/OSCNN2s.h5
+-rw-rw-rw-   0        0        0        0 2023-05-10 07:25:34.000000 ecg_quality-0.2.0/ecg_quality/models/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-05-10 07:25:34.000000 ecg_quality-0.2.0/ecg_quality/tf_model.py
+-rw-rw-rw-   0        0        0     1140 2023-05-10 07:25:34.000000 ecg_quality-0.2.0/ecg_quality/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:54:26.028540 ecg_quality-0.2.0/ecg_quality.egg-info/
+-rw-rw-rw-   0        0        0     3704 2023-05-20 19:54:25.000000 ecg_quality-0.2.0/ecg_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-05-20 19:54:25.000000 ecg_quality-0.2.0/ecg_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 19:54:25.000000 ecg_quality-0.2.0/ecg_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 19:54:25.000000 ecg_quality-0.2.0/ecg_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 19:54:25.000000 ecg_quality-0.2.0/ecg_quality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-20 19:54:26.668292 ecg_quality-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-05-20 19:51:05.000000 ecg_quality-0.2.0/setup.py
```

### Comparing `ecg_quality-0.1.3/LICENSE` & `ecg_quality-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/PKG-INFO` & `ecg_quality-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,59 @@
-Metadata-Version: 2.1
-Name: ecg_quality
-Version: 0.1.3
-Summary: Library that classifies quality of ECG signal using deep learning methods
-Home-page: https://github.com/koledjoz/ecg_quality
-Download-URL: https://github.com/koledjoz/ecg_quality/releases/tag/v0.1.3
-Author: Jozef Koleda
-Author-email: koledjoz@cvut.cz
-License: gpl-3.0
-Keywords: ECG,quality,classification,deep learning
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Library description
-================
-
-This library is meant to be used to check quality of ECG signal. Recordings of any length can be processed, memory is the only limit. The library work with three basic levels of quality:
-
- - Quality 1 : All important segment of ECG can be detected in the signal
- - Quality 2 : Noise is present, but the QRS complex can still be detected
- - Quality 3 : Noise is too large, not even QRS complex can be detected
-
-Each model works with a sliding window. At each step, the window is evaluated using one of 4 models and one score from range 0 to 1 is returned. The length of sliding windows for individual models can be found in their names. The 4 supported models are:
-
-- cnn2s
-- cnn5s
-- lstm2s
-- oscnn2s
-
-The stride of the sliding window can be specified. The class limits so this value is at least 1 second and is a divisor of the length of the sliding window. 
-
-There are currently 4 return modes supported:
- 
-
- - score : The model returns the score between 0 and 1. 0 is meant to represent quality 1, 0.5 to represent quality 2 and 1 to represent quality 3. This is however not given and the score distributions of different qualities can differ between models.
- - three_value : Three qualities are given using thresholds.
- - bin_clean : Signal is either marked as quality 1 or as quality 2/3
- - bin_qrs: Signal is either marked as quality 1/2 or as quality 3
-
-The thresholds used in each of these modes, except of score, can be specified by the user. However, there are default thresholds, that aim to prioritize precision with the better classes. When using three_value, the returned values are one of 1, 2 and 3, depending on the quality of the signal. When using either of the binary modes, the returned values are either 1 or 2. 1 is for the better quality signal and 2 is for the worse quality.
-
-In terms of length of output, there are two return_types supported:
-
- -  intervals : value is returned for each window of the size stride, since the value of the quality ill not change in these
- - full : value is returned for each value in the input
-
-Models were trained on cleaned data. These data were cleaned using default NeuroKit2 ecg_clean method. The class can clean signal it is meant to process using ecg_clean. It can be specified not to do this. 
-
-Full explanation of all the modes can be found inside the source code documentation.
-
-Installation
--------------
-
-The library can be easily installed through the pip utility.
-
-		pip install ecg-quality
-
-Usage
--------
-The library offers a high-level interface. The simplest example using all the default settings:
-
-	from ecg_quality.ECGQualityChecker import ECGQualityChecker  
-  
-	checker = ECGQualityChecker()  
-	 
-	signal = ...	 
-  
-	output = checker.process_signal(signal)  
-  
-
+Library description
+================
+
+This library is meant to be used to check quality of ECG signal. Recordings of any length can be processed, memory is the only limit. The library work with three basic levels of quality:
+
+ - Quality 1 : All important segment of ECG can be detected in the signal
+ - Quality 2 : Noise is present, but the QRS complex can still be detected
+ - Quality 3 : Noise is too large, not even QRS complex can be detected
+
+Each model works with a sliding window. At each step, the window is evaluated using one of 4 models and one score from range 0 to 1 is returned. The length of sliding windows for individual models can be found in their names. The 4 supported models are:
+
+- cnn2s
+- cnn5s
+- lstm2s
+- oscnn2s
+
+The stride of the sliding window can be specified. The class limits so this value is at least 1 second and is a divisor of the length of the sliding window. 
+
+There are currently 4 return modes supported:
+ 
+
+ - score : The model returns the score between 0 and 1. 0 is meant to represent quality 1, 0.5 to represent quality 2 and 1 to represent quality 3. This is however not given and the score distributions of different qualities can differ between models.
+ - three_value : Three qualities are given using thresholds.
+ - bin_clean : Signal is either marked as quality 1 or as quality 2/3
+ - bin_qrs: Signal is either marked as quality 1/2 or as quality 3
+
+The thresholds used in each of these modes, except of score, can be specified by the user. However, there are default thresholds, that aim to prioritize precision with the better classes. When using three_value, the returned values are one of 1, 2 and 3, depending on the quality of the signal. When using either of the binary modes, the returned values are either 1 or 2. 1 is for the better quality signal and 2 is for the worse quality.
+
+In terms of length of output, there are two return_types supported:
+
+ -  intervals : value is returned for each window of the size stride, since the value of the quality ill not change in these
+ - full : value is returned for each value in the input
+
+Models were trained on cleaned data. These data were cleaned using default NeuroKit2 ecg_clean method. The class can clean signal it is meant to process using ecg_clean. Currently only default version of ecg_clean us supported. It can be specified not to do this. However, it is advised to either use this option, or to pass cleaned signal to the method. We give no guarantee about the quality of the signal if uncleaned signal is processed and no cleaning is done..  
+
+Signal processed must have frequency of 250 Hz. Signal of other frequencies is not supported as the models are not trained on such a signal.
+
+Full explanation of all the modes can be found inside the source code documentation.
+
+Installation
+-------------
+
+The library can be easily installed through the pip utility.
+
+    pip install ecg-quality
+
+Usage
+-------
+The library offers a high-level interface. The simplest example using all the default settings:
+
+	from ecg_quality.ECGQualityChecker import ECGQualityChecker  
+  
+	checker = ECGQualityChecker()  
+	 
+	signal = ...	 
+  
+	output = checker.process_signal(signal)  
+  
+
```

### Comparing `ecg_quality-0.1.3/ecg_quality/ECGQualityChecker.py` & `ecg_quality-0.2.0/ecg_quality/ECGQualityChecker.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 
 
 
 
 
-    def __init__(self, model:str = 'cnn2s', stride:float = 0.0, return_mode:str = 'score', thresholds:list = None, return_type:str = 'full', sampling_rate:int = 250, clean_data:bool=True):
+    def __init__(self, model:str = 'cnn2s', stride:float = 0.0, return_mode:str = 'score', thresholds:list = None, return_type:str = 'full', sampling_rate:int = 250, clean_data:bool=True, check_window_range:bool=True, window_min_range:float=0.1):
         """
         Parameters
         --------------
 
         **model : str**
             This is the model to be used by the class. There are currently 4 possible models to use:
         * cnn2s : This model uses CNN architecture with the size of the sliding window being 2 seconds.
@@ -68,24 +68,33 @@
 
         The models currently only support 250 Hz. Using any other frequency will result in fail. Slightly different frequencies can theoretically be used, but that is to be done at your own risk.
 
         **clean_data : bool**
 
         Whether the data should be cleaned before processing. The models were trained on cleaned data so this is advised unless you already cleaned data beforehand. For cleaning, we are using neurokit2 function ecg_clean with its default settings as of version 0.2.4.
 
+        **check_window_range : bool**
 
+        Whether each window should be checked for range. If the range of signal values is not larger than the value of the window_min_range, the widow will automatically be marked as a signal of quality 3. This is temporary solution to be used because of the models inability to detect low amplitude noise
 
+        **window_min_range : float**
+
+        This is the range that is to be used if the check_window_range parameter is true. If tha difference of the minimum and maximum value in window is smaller than this difference, automatically markt he signal as of the worst quality type.
+
+check_window_range:bool=False, window_min_range:float=0.05
 
         :param model: Model to be used
         :param stride: The soze of the step of the moving window
         :param return_mode: The type of classification to be done by the class
         :param thresholds: The thresholds to be used when and if other return_mode than socre is chosen
         :param return_type: how mnay values should be returned
         :param sampling_rate: The sampling rate of the ECG signal to be processed, currently just 250 Hz is supported
         :param clean_data: Whether to clean data before processing them.
+        :param check_window_range: Whether to check each window for value range
+        :param window_min_range: What the minimum range of signal values should be in case the window min range test is done
         """
         # urobime checks vsetkych modelov
 
         if model not in list(MODEL_PATH_DICT.keys()):
             raise ValueError(model + ' is not a known model that can be used')
 
         if return_mode not in ['score', 'three_value', 'binary_clean', 'binary_qrs']:
@@ -127,14 +136,16 @@
 
         self.stride = utils.get_stride_length(self.model.get_input_length(), stride, sampling_rate)
         self.return_mode = return_mode
         self.return_type = return_type
         self.thresholds = thresholds
         self.sampling_rate = sampling_rate
         self.clean_data = clean_data
+        self.check_window = check_window_range
+        self.min_window = window_min_range
 
     def process_signal(self, signal):
         """
 
         This method processes ECG signal and returns specified values.
 
         Parameters:
@@ -157,23 +168,33 @@
 
 
         if self.return_type == 'full':
             return self._process_signal_full(signal)
         elif self.return_type == 'intervals':
             return self._process_signal_interval(signal)
 
+
+
+    def _check_window_smaller(self, window_signal):
+        minimum = np.min(window_signal)
+        maximum = np.max(window_signal)
+
+        range = maximum - minimum
+
+        return range < self.min_window
+
     def _process_signal_full(self, signal):
         if self.clean_data:
             signal = nk.ecg_clean(signal, sampling_rate=self.sampling_rate)
 
         output = np.zeros_like(signal)
         win_count = np.zeros_like(signal)
 
         for win_start in range(0, len(signal)-self.input_length + 1, self.stride):
-            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
+            score = 1.0 if self._check_window_smaller(signal[win_start:win_start + self.input_length]) else self.model.process_ecg(signal[win_start:win_start + self.input_length])
             output[win_start:win_start + self.input_length] = output[win_start:win_start + self.input_length] + score
             win_count[win_start:win_start + self.input_length] = win_count[win_start:win_start + self.input_length] + 1
         return self._calc_precise_scores(output, win_count)
 
     def _process_signal_interval(self, signal):
 
         if self.clean_data:
@@ -182,15 +203,15 @@
         output = np.zeros(len(signal) // self.stride)
         win_count = np.zeros(len(signal) // self.stride)
 
         for win_start in range(0, len(signal) - self.input_length + 1, self.stride):
             a = win_start // self.stride
             b = (win_start + self.input_length) // self.stride
 
-            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
+            score = 1.0 if self._check_window_smaller(signal[win_start:win_start + self.input_length]) else self.model.process_ecg(signal[win_start:win_start + self.input_length])
             output[a:b] = output[a:b] + score
             win_count[a:b] = win_count[a:b] + 1
         return self._calc_precise_scores(output, win_count)
 
     def _get_binary(self, scores):
         return [1.0 if x < self.thresholds[0] else 2.0 for x in scores]
```

### Comparing `ecg_quality-0.1.3/ecg_quality/model.py` & `ecg_quality-0.2.0/ecg_quality/model.py`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/models/CNN2s.h5` & `ecg_quality-0.2.0/ecg_quality/models/CNN2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/models/CNN5s.h5` & `ecg_quality-0.2.0/ecg_quality/models/CNN5s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/models/LSTM2s.h5` & `ecg_quality-0.2.0/ecg_quality/models/LSTM2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/models/OSCNN2s.h5` & `ecg_quality-0.2.0/ecg_quality/models/OSCNN2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/tf_model.py` & `ecg_quality-0.2.0/ecg_quality/tf_model.py`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality/utils.py` & `ecg_quality-0.2.0/ecg_quality/utils.py`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.3/ecg_quality.egg-info/PKG-INFO` & `ecg_quality-0.2.0/ecg_quality.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ecg-quality
-Version: 0.1.3
+Version: 0.2.0
 Summary: Library that classifies quality of ECG signal using deep learning methods
 Home-page: https://github.com/koledjoz/ecg_quality
-Download-URL: https://github.com/koledjoz/ecg_quality/releases/tag/v0.1.3
+Download-URL: https://github.com/koledjoz/ecg_quality/releases/tag/v0.2.0
 Author: Jozef Koleda
 Author-email: koledjoz@cvut.cz
 License: gpl-3.0
 Keywords: ECG,quality,classification,deep learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -40,24 +40,26 @@
 The thresholds used in each of these modes, except of score, can be specified by the user. However, there are default thresholds, that aim to prioritize precision with the better classes. When using three_value, the returned values are one of 1, 2 and 3, depending on the quality of the signal. When using either of the binary modes, the returned values are either 1 or 2. 1 is for the better quality signal and 2 is for the worse quality.
 
 In terms of length of output, there are two return_types supported:
 
  -  intervals : value is returned for each window of the size stride, since the value of the quality ill not change in these
  - full : value is returned for each value in the input
 
-Models were trained on cleaned data. These data were cleaned using default NeuroKit2 ecg_clean method. The class can clean signal it is meant to process using ecg_clean. It can be specified not to do this. 
+Models were trained on cleaned data. These data were cleaned using default NeuroKit2 ecg_clean method. The class can clean signal it is meant to process using ecg_clean. Currently only default version of ecg_clean us supported. It can be specified not to do this. However, it is advised to either use this option, or to pass cleaned signal to the method. We give no guarantee about the quality of the signal if uncleaned signal is processed and no cleaning is done..  
+
+Signal processed must have frequency of 250 Hz. Signal of other frequencies is not supported as the models are not trained on such a signal.
 
 Full explanation of all the modes can be found inside the source code documentation.
 
 Installation
 -------------
 
 The library can be easily installed through the pip utility.
 
-		pip install ecg-quality
+    pip install ecg-quality
 
 Usage
 -------
 The library offers a high-level interface. The simplest example using all the default settings:
 
 	from ecg_quality.ECGQualityChecker import ECGQualityChecker
```

### Comparing `ecg_quality-0.1.3/setup.py` & `ecg_quality-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 setuptools.setup(
   name = 'ecg_quality',
   packages = setuptools.find_packages(),
   package_data={'ecg_quality': ['models/*.h5']},
   long_description=long_description,
   long_description_content_type='text/markdown',
-  version = '0.1.3',
+  version = '0.2.0',
   license='gpl-3.0',
   description = 'Library that classifies quality of ECG signal using deep learning methods',
   author = 'Jozef Koleda',
   author_email = 'koledjoz@cvut.cz',
   url = 'https://github.com/koledjoz/ecg_quality',
-  download_url = 'https://github.com/koledjoz/ecg_quality/releases/tag/v0.1.3',
+  download_url = 'https://github.com/koledjoz/ecg_quality/releases/tag/v0.2.0',
   keywords = ['ECG', 'quality', 'classification', 'deep learning'],
   install_requires=[
           'tensorflow',
           'numpy',
           'neurokit2',
       ]
 )
```

