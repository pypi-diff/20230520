# Comparing `tmp/colortextpy-0.0.3.1.tar.gz` & `tmp/colortextpy-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortextpy-0.0.3.1.tar", last modified: Mon May 15 03:21:43 2023, max compression
+gzip compressed data, was "colortextpy-0.0.3.2.tar", last modified: Sat May 20 14:42:17 2023, max compression
```

## Comparing `colortextpy-0.0.3.1.tar` & `colortextpy-0.0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-15 03:21:43.760657 colortextpy-0.0.3.1/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.3.1/LICENSE
--rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.3.1/MANIFEST.in
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1966 2023-05-15 03:21:43.758149 colortextpy-0.0.3.1/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      987 2023-05-14 12:19:37.000000 colortextpy-0.0.3.1/README.md
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-15 03:21:43.604177 colortextpy-0.0.3.1/colortextpy/
--rwxrwxrwx   0 ping      (1000) ping      (1000)      152 2023-05-15 03:15:58.000000 colortextpy-0.0.3.1/colortextpy/__init__.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)    12526 2023-05-15 03:15:59.000000 colortextpy-0.0.3.1/colortextpy/_modidx.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     6579 2023-05-15 03:15:58.000000 colortextpy-0.0.3.1/colortextpy/ansicolor.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)    13062 2023-05-15 03:15:58.000000 colortextpy-0.0.3.1/colortextpy/color.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     7114 2023-05-15 03:15:58.000000 colortextpy-0.0.3.1/colortextpy/colorizer.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     2704 2023-05-15 03:15:58.000000 colortextpy-0.0.3.1/colortextpy/printer.py
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-15 03:21:43.738418 colortextpy-0.0.3.1/colortextpy.egg-info/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1966 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      438 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/entry_points.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.3.1/colortextpy.egg-info/not-zip-safe
--rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/requires.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-15 03:21:43.000000 colortextpy-0.0.3.1/colortextpy.egg-info/top_level.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)      860 2023-05-15 03:16:15.000000 colortextpy-0.0.3.1/settings.ini
--rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-15 03:21:43.761157 colortextpy-0.0.3.1/setup.cfg
--rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.3.1/setup.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-20 14:42:17.197041 colortextpy-0.0.3.2/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.3.2/LICENSE
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.3.2/MANIFEST.in
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     8484 2023-05-20 14:42:17.194532 colortextpy-0.0.3.2/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     7505 2023-05-20 14:28:12.000000 colortextpy-0.0.3.2/README.md
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-20 14:42:17.047618 colortextpy-0.0.3.2/colortextpy/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      198 2023-05-20 14:11:33.000000 colortextpy-0.0.3.2/colortextpy/__init__.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)    12526 2023-05-20 14:30:42.000000 colortextpy-0.0.3.2/colortextpy/_modidx.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     6614 2023-05-20 14:11:33.000000 colortextpy-0.0.3.2/colortextpy/ansicolor.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)    13062 2023-05-20 14:11:33.000000 colortextpy-0.0.3.2/colortextpy/color.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     6808 2023-05-20 14:11:33.000000 colortextpy-0.0.3.2/colortextpy/colorizer.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     2704 2023-05-20 14:11:33.000000 colortextpy-0.0.3.2/colortextpy/printer.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-20 14:42:17.175781 colortextpy-0.0.3.2/colortextpy.egg-info/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     8484 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      438 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/entry_points.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.3.2/colortextpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/requires.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-20 14:42:16.000000 colortextpy-0.0.3.2/colortextpy.egg-info/top_level.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      860 2023-05-20 14:06:32.000000 colortextpy-0.0.3.2/settings.ini
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-20 14:42:17.198032 colortextpy-0.0.3.2/setup.cfg
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.3.2/setup.py
```

### Comparing `colortextpy-0.0.3.1/LICENSE` & `colortextpy-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `colortextpy-0.0.3.1/colortextpy/_modidx.py` & `colortextpy-0.0.3.2/colortextpy/_modidx.py`

 * *Files identical despite different names*

### Comparing `colortextpy-0.0.3.1/colortextpy/ansicolor.py` & `colortextpy-0.0.3.2/colortextpy/ansicolor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_ansicolor.ipynb.
 
 # %% auto 0
-__all__ = ['Fore', 'Back', 'Style', 'AnsiColor']
+__all__ = ['Fore', 'Back', 'Style', 'RESET_ALL', 'AnsiColor']
 
 # %% ../nbs/01_ansicolor.ipynb 4
 import re
 
 from .color import enum, _EnumMeta, Color, hex2rgb
 from .color import _ClassPropertyDescriptor
 
@@ -141,15 +141,15 @@
         '''
         return self.templates[name]
     
     
 Fore = _AnsiColor('fore')
 Back = _AnsiColor('back')
 Style = _AnsiColor('style')
-
+RESET_ALL = '\033[00m'
 
 class AnsiColor:
     r'''
     Integrate with `Fore`, `Back`, `Style`.
     
     Parameters
     ----------
```

### Comparing `colortextpy-0.0.3.1/colortextpy/color.py` & `colortextpy-0.0.3.2/colortextpy/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     def bgr(self):
         return self._bgr
     
     @property
     def __contains__(cls, other):
         return other in cls.available
 
-# %% ../nbs/00_color.ipynb 10
+# %% ../nbs/00_color.ipynb 11
 # def rgb2hex(*rgb) -> str:
 #     return '#{0:x}{1:x}{2:x}'.format(*rgb)
 
 
 def rgb2hex(r: int, g: int, b: int) -> str:
     '''
     convert rgb color to hex
```

### Comparing `colortextpy-0.0.3.1/colortextpy/colorizer.py` & `colortextpy-0.0.3.2/colortextpy/colorizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,45 +51,46 @@
             print('text')        
 
         @ColorStream(fore=Fore.dark_orange)
         def foo():
             print('FOO')
     ```
     '''
+
     
-    _regex_tag = re.compile('stdout|stderr')
-    
-    def __init__(self, fore=None, back=None, style=None, autoreset=True, streams=('stdout', )):
+    def __init__(self, fore=None, back=None, style=None, autoreset=True, streams='stdout'):
         '''
         Parameters
         ----------
         fore : `Fore`, str, int, optional
             Foreground color. Could be hex, rgb string or tuple, `Fore`, 8-bits color
 
         back : `Back`, str, rgb, int, optional
             Background color, Could be hex, rgb string or tuple, `Back`, 8-bits color
 
         style : `Style`, str, tuple, optional
             Text style. Seee `Style.available`.
             
         autoreset: bool
         
-        streams: str, tuple
-            One of {stdout, stderr}, Could be tuple
+        streams: str
+            One of {stdout, stderr}
         '''
         self.ansi = AnsiColor(fore, back, style)
         
         self._global_flag = False
         self.autoreset = autoreset
         self._ori_reset = autoreset
         
-        self.streams = streams if isinstance(streams, (list, tuple)) else (streams, )
-        
-        self.files = [getattr(sys, stream) for stream in streams]
-        self.ori_files = []
+        if streams not in ('stdout', 'stderr'): 
+            raise ValueError(f'{streams} is not acceptable')
+
+        self.stream = streams
+        self.ori_file = None
+        self.file = getattr(sys, streams)
 
             
     def affect_global_stream(self):
         if not self._global_flag:
             self.__enter__()
             self._ori_reset = self.autoreset
             
@@ -98,74 +99,75 @@
         
     def unAffect_global_stream(self):
         self.__exit__()
         self._global_flag = False
         self.autoreset = self._ori_reset
         
     def __enter__(self):
-        if not self.ori_files:
-            for stream in self.streams:
-                self.ori_files.append(getattr(system_stream, stream))
-                setattr(sys, stream, self)
+        if self.ori_file is None:
+            self.ori_file = getattr(system_stream, self.stream)
+            setattr(sys, self.stream, self)
+
 
     def __exit__(self, *args):
-        if self.ori_files:
-            for stream, ori_file in zip(self.streams, self.ori_files):
-                setattr(sys, stream, ori_file)
-            self.ori_files = []
+        if self.ori_file:
+            setattr(sys, self.stream, self.ori_file)
+            self.ori_file = None
 
     def write(self, text):
-        for file in self.ori_files:
-            reset = Style.reset_all if self.autoreset else ''
-            file.write(f'{self.ansi.ansi_fmt}{text}{reset}')
-            file.flush()
-            
+        reset = Style.reset_all if self.autoreset else ''
+        self.file.write(f'{self.ansi.ansi_fmt}{text}{reset}')
+        self.flush()
+
     def flush(self):
-        for file in self.ori_files:
-            file.flush()           
+        self.file.flush()
       
     
 class AnsiColorizer:
-    r'''
-    For `text` parameter, you can add color tag. Start with <tag> end with </tag>.
+    '''
+    
+    For `text` parameter,  you can add color tag. Start with \<tag\> end with \</tag\>.
     
     Some usage:
+    
+    ```python
         text = 'something'
-        
-        1. blue text tag: 
+
+        # 1. blue text tag: 
+
             f'<blue>{text}</fg>'
             f'<blue>{text}</blue>'
-            
-        2. specify fg:
-            f'<fg red>{text}</fg>
-            
-        3. specify bg:
-            f'<bg purple>{text}</bg>
-            
-        4. style:
+
+        # 2. specify fg:
+            f'<fg red>{text}</fg>'
+
+        # 3. specify bg:
+            f'<bg purple>{text}</bg>'
+
+        # 4. style:
             f'<bold>{text}</bold>'
-            
-        5. support rgb format:
+
+        # 5. support rgb format:
             f'<255, 255, 255>{text}</fg>'
             f'<fg 255, 255, 255>{text}</fg>'
             f'<bg 255, 255, 255>{text}</bg>'
-            
-        6. support hex format:
+
+        # 6. support hex format:
             f'<#FFFFFF>{text}</fg>'
             f'<fg #FFFFFF>{text}</fg>'
             f'<bg #FFFFFF>{text}</bg>'
-        
-        7. support 8-bits color:
+
+        # 7. support 8-bits color:
             f'<50>{text}</fg>'
             f'<fg 50>{text}</fg>'
             f'<bg 50>{text}</bg>'
-            
-        8. mix of above is ok:
+
+        # 8. mix of above is ok:
             f'<fg red>{text}--<bg green>{text}--</fg>{text}--</bg>{text}'
-            
+    ```
     '''
     
     _regex_tag = re.compile(r"<([/\w\s,#]*)>")
     
     def __call__(self, text, fore=None, back=None, style=None, raw=False, strip=False):
         '''
         Parameters
```

### Comparing `colortextpy-0.0.3.1/colortextpy/printer.py` & `colortextpy-0.0.3.2/colortextpy/printer.py`

 * *Files identical despite different names*

### Comparing `colortextpy-0.0.3.1/settings.ini` & `colortextpy-0.0.3.2/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = colortextpy
 lib_name = colortextpy
-version = 0.0.3.1
+version = 0.0.3.2
 min_python = 3.6
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = colortextpy
 nbs_path = nbs
 recursive = True
```

### Comparing `colortextpy-0.0.3.1/setup.py` & `colortextpy-0.0.3.2/setup.py`

 * *Files identical despite different names*

