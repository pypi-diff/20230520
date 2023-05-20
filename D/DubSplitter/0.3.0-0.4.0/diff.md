# Comparing `tmp/DubSplitter-0.3.0.tar.gz` & `tmp/DubSplitter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DubSplitter-0.3.0.tar", last modified: Wed Apr 12 01:29:10 2023, max compression
+gzip compressed data, was "DubSplitter-0.4.0.tar", last modified: Sat May 20 12:33:20 2023, max compression
```

## Comparing `DubSplitter-0.3.0.tar` & `DubSplitter-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.316105 DubSplitter-0.3.0/DubSplitter.egg-info/
--rw-rw-rw-   0        0        0     6158 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 00:03:48.000000 DubSplitter-0.3.0/DubSplitter.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6158 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.318110 DubSplitter-0.3.0/dubSplitter/
--rw-rw-rw-   0        0        0        0 2023-04-07 01:02:52.000000 DubSplitter-0.3.0/dubSplitter/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-04-12 01:10:41.000000 DubSplitter-0.3.0/dubSplitter/constants.py
--rw-rw-rw-   0        0        0     5084 2023-04-12 01:25:22.000000 DubSplitter-0.3.0/dubSplitter/dubSplitter.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.322276 DubSplitter-0.3.0/dubSplitter/functions/
--rw-rw-rw-   0        0        0        0 2023-04-07 01:03:14.000000 DubSplitter-0.3.0/dubSplitter/functions/__init__.py
--rw-rw-rw-   0        0        0      130 2023-04-08 09:55:32.000000 DubSplitter-0.3.0/dubSplitter/functions/exitWithInfo.py
--rw-rw-rw-   0        0        0      630 2023-04-12 00:43:28.000000 DubSplitter-0.3.0/dubSplitter/functions/path.py
--rw-rw-rw-   0        0        0     3772 2023-04-12 01:25:45.000000 DubSplitter-0.3.0/dubSplitter/functions/slicer.py
--rw-rw-rw-   0        0        0      445 2023-04-11 15:43:19.000000 DubSplitter-0.3.0/dubSplitter/functions/stringEx.py
--rw-rw-rw-   0        0        0     3478 2023-04-12 01:22:36.000000 DubSplitter-0.3.0/dubSplitter/functions/voiceRecognition.py
--rw-rw-rw-   0        0        0       42 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1345 2023-04-12 01:28:25.000000 DubSplitter-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:33:20.237864 DubSplitter-0.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:33:20.224139 DubSplitter-0.4.0/DubSplitter.egg-info/
+-rw-rw-rw-   0        0        0     6227 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 00:03:48.000000 DubSplitter-0.4.0/DubSplitter.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 12:33:20.000000 DubSplitter-0.4.0/DubSplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6227 2023-05-20 12:33:20.237864 DubSplitter-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 12:33:20.234142 DubSplitter-0.4.0/dubSplitter/
+-rw-rw-rw-   0        0        0        0 2023-04-07 01:02:52.000000 DubSplitter-0.4.0/dubSplitter/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-04-12 01:10:41.000000 DubSplitter-0.4.0/dubSplitter/constants.py
+-rw-rw-rw-   0        0        0     5865 2023-05-20 12:02:08.000000 DubSplitter-0.4.0/dubSplitter/dubSplitter.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:33:20.236859 DubSplitter-0.4.0/dubSplitter/functions/
+-rw-rw-rw-   0        0        0        0 2023-04-07 01:03:14.000000 DubSplitter-0.4.0/dubSplitter/functions/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-04-08 09:55:32.000000 DubSplitter-0.4.0/dubSplitter/functions/exitWithInfo.py
+-rw-rw-rw-   0        0        0      630 2023-04-12 00:43:28.000000 DubSplitter-0.4.0/dubSplitter/functions/path.py
+-rw-rw-rw-   0        0        0     3812 2023-05-20 12:00:48.000000 DubSplitter-0.4.0/dubSplitter/functions/slicer.py
+-rw-rw-rw-   0        0        0      445 2023-04-11 15:43:19.000000 DubSplitter-0.4.0/dubSplitter/functions/stringEx.py
+-rw-rw-rw-   0        0        0     3478 2023-04-12 01:22:36.000000 DubSplitter-0.4.0/dubSplitter/functions/voiceRecognition.py
+-rw-rw-rw-   0        0        0       42 2023-05-20 12:33:20.237864 DubSplitter-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2023-04-12 01:28:25.000000 DubSplitter-0.4.0/setup.py
```

### Comparing `DubSplitter-0.3.0/DubSplitter.egg-info/PKG-INFO` & `DubSplitter-0.4.0/DubSplitter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DubSplitter
-Version: 0.3.0
+Version: 0.4.0
 Summary: an easy tool to split dubs based on given silence
 Home-page: https://github.com/defisym/HibiscusAVGEngine/tree/main/Utilities/DubSplitter
 Author: defisym
 Author-email: defisym@outlook.com
 License: MIT
 Keywords: DubSplitter dub splitter Hibiscus AVG Galgame VisualNovel VN
 Classifier: Development Status :: 4 - Beta
@@ -113,14 +113,18 @@
 
 use `--prompt 简体中文` -> `真辛苦真辛苦啊 我会跳个好天气出去运动的`
 
 use `--prompt 正體中文` -> `真辛苦真辛苦啊我會跳個好天氣出去運動的`
 
 ## Changelog
 
+### 230520 0.4.0
+
+- set silence threshold & keep silence length
+
 ### 230412 0.3.0
 
 - add color for outputs
 - add custom file format support
 - add custom filename format support
 - add prompt support
 - add omit len option
```

### Comparing `DubSplitter-0.3.0/DubSplitter.egg-info/SOURCES.txt` & `DubSplitter-0.4.0/DubSplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DubSplitter-0.3.0/PKG-INFO` & `DubSplitter-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DubSplitter
-Version: 0.3.0
+Version: 0.4.0
 Summary: an easy tool to split dubs based on given silence
 Home-page: https://github.com/defisym/HibiscusAVGEngine/tree/main/Utilities/DubSplitter
 Author: defisym
 Author-email: defisym@outlook.com
 License: MIT
 Keywords: DubSplitter dub splitter Hibiscus AVG Galgame VisualNovel VN
 Classifier: Development Status :: 4 - Beta
@@ -113,14 +113,18 @@
 
 use `--prompt 简体中文` -> `真辛苦真辛苦啊 我会跳个好天气出去运动的`
 
 use `--prompt 正體中文` -> `真辛苦真辛苦啊我會跳個好天氣出去運動的`
 
 ## Changelog
 
+### 230520 0.4.0
+
+- set silence threshold & keep silence length
+
 ### 230412 0.3.0
 
 - add color for outputs
 - add custom file format support
 - add custom filename format support
 - add prompt support
 - add omit len option
```

### Comparing `DubSplitter-0.3.0/dubSplitter/constants.py` & `DubSplitter-0.4.0/dubSplitter/constants.py`

 * *Files identical despite different names*

### Comparing `DubSplitter-0.3.0/dubSplitter/dubSplitter.py` & `DubSplitter-0.4.0/dubSplitter/dubSplitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 
 import dubSplitter.constants as consts
 from .constants import update_path
 from .functions.slicer import do_slice, update_output_format, update_filename_format, update_filename_vr_format, \
     update_filename_custom, update_result_omit_length
 from .functions.voiceRecognition import update_whisper_model, update_model_language, update_model_prompt
 
+# -f "F:\DEV\Mobius\资产\语音\基利尔\01_初\干音\初.wav" -o "F:\DEV\Mobius\资产\语音\基利尔\01_初\Out" -s 800 -r 1200 --keepSilence 500
+
 init(autoreset=True)
 
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 print(Fore.LIGHTGREEN_EX + '====================================')
 print(Fore.LIGHTGREEN_EX + 'DubSplitter {}'.format(VERSION))
 print(Fore.LIGHTGREEN_EX + '====================================')
 
 bFromPackage = true
 
 
 def update_runtime(runtime):
     global bFromPackage
     bFromPackage = runtime
 
 
-# -f "F:\DEV\Mobius\资产\语音\基利尔\01_初\干音\初.wav" -o "F:\DEV\Mobius\资产\语音\基利尔\01_初\Out" -s 800 -r 400
 def main():
     # https://docs.python.org/zh-cn/3.6/library/argparse.html
     parser = argparse.ArgumentParser(description='Slice dubs.')
 
     parser.add_argument('-f', '--fileName',
                         help='file to process')
     parser.add_argument('-o', '--outFilePath',
@@ -55,14 +56,24 @@
                         type=int, default=1000)
     parser.add_argument('-r', '--range',
                         help='range, default is 100ms. e.g., silence = 400, range = 100 will slice in 400ms and 500ms',
                         type=int, default=100)
     parser.add_argument('--step',
                         help='loop step, default is 100ms',
                         type=int, default=100)
+    parser.add_argument('--threshold',
+                        help='(in dBFS) anything quieter than this will be considered silence',
+                        type=int, default=-40)
+    parser.add_argument('--keepSilence',
+                        help='leave some silence at the beginning and end of the chunks. Keeps the sound from '
+                             'sounding like it is abruptly cut off. When the length of the silence is less than the '
+                             'given duration it is split evenly between the preceding and following non-silent '
+                             'segments.',
+                        type=int, default=100)
+
     parser.add_argument('--noVR',
                         help='don\'t use voice recognition, default is false',
                         type=bool, default=false)
     parser.add_argument('--model',
                         help='whisper model, default is base',
                         default='base')
     parser.add_argument('--prompt',
@@ -92,14 +103,17 @@
     print('prepare to process file {}'.format(inName))
     print('output to folder {}'.format(outPath))
 
     silenceStart = args.silence
     silenceEnd = silenceStart + args.range
     silenceStep = args.step
 
+    threshold = args.threshold
+    keepSilence = args.keepSilence
+
     print(Fore.WHITE + Style.DIM + '  reading file...')
     sound = AudioSegment.from_file(inName)
     print(Fore.WHITE + Style.DIM + '  read complete...')
 
     noVR = args.noVR
 
     if not noVR:
@@ -110,12 +124,12 @@
         update_whisper_model(args.model)
 
     print(Fore.LIGHTGREEN_EX + '============================')
     print(Fore.LIGHTGREEN_EX + 'processing...')
     print(Fore.LIGHTGREEN_EX + '============================')
 
     for silence in range(silenceStart, silenceEnd + 1, silenceStep):
-        do_slice(sound, silence, outPath, not noVR)
+        do_slice(sound, silence, threshold, keepSilence, outPath, not noVR)
 
     print(Fore.LIGHTGREEN_EX + '============================')
     print(Fore.LIGHTGREEN_EX + 'process complete')
     print(Fore.LIGHTGREEN_EX + '============================')
```

### Comparing `DubSplitter-0.3.0/dubSplitter/functions/path.py` & `DubSplitter-0.4.0/dubSplitter/functions/path.py`

 * *Files identical despite different names*

### Comparing `DubSplitter-0.3.0/dubSplitter/functions/slicer.py` & `DubSplitter-0.4.0/dubSplitter/functions/slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 
 
 def update_result_omit_length(new_length):
     global resultOmitLength
     resultOmitLength = new_length
 
 
-def do_slice(sound, silence, out_path, b_vr):
+def do_slice(sound, silence, threshold, keep_silence, out_path, b_vr):
     print('slice audio by silence length {}'.format(silence))
 
-    dubs = split_on_silence(sound, silence, -40, 100, 1)
+    dubs = split_on_silence(sound, silence, threshold, keep_silence, 1)
     length = len(dubs)
     print('slice complete, got {} lines'.format(length))
 
     mkdir(tempPath)
 
     localPath = process_path(out_path) + '\\' + 'Silence_' + str(silence)
     mkdir(localPath)
```

### Comparing `DubSplitter-0.3.0/dubSplitter/functions/voiceRecognition.py` & `DubSplitter-0.4.0/dubSplitter/functions/voiceRecognition.py`

 * *Files identical despite different names*

### Comparing `DubSplitter-0.3.0/setup.py` & `DubSplitter-0.4.0/setup.py`

 * *Files identical despite different names*

