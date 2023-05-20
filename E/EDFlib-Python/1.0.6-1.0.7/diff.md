# Comparing `tmp/EDFlib-Python-1.0.6.tar.gz` & `tmp/EDFlib-Python-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/amos/python/EDFlib-Python/dist/tmpned03qyo/EDFlib-Python-1.0.6.tar", last modified: Sat Jan 15 08:43:20 2022, max compression
+gzip compressed data, was "/data/amos/python/EDFlib-Python/dist/tmp0g0oz9tp/EDFlib-Python-1.0.7.tar", last modified: Sat May 20 12:21:32 2023, max compression
```

## Comparing `EDFlib-Python-1.0.6.tar` & `EDFlib-Python-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 guv       (1000) users      (100)        0 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/
--rw-r--r--   0 guv       (1000) users      (100)     1770 2020-07-12 06:51:01.000000 EDFlib-Python-1.0.6/LICENSE
--rw-r--r--   0 guv       (1000) users      (100)     1290 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/PKG-INFO
--rw-r--r--   0 guv       (1000) users      (100)      615 2021-12-18 09:01:46.000000 EDFlib-Python-1.0.6/README.md
--rw-r--r--   0 guv       (1000) users      (100)      104 2021-08-05 18:52:14.000000 EDFlib-Python-1.0.6/pyproject.toml
--rw-r--r--   0 guv       (1000) users      (100)      783 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/setup.cfg
-drwxr-xr-x   0 guv       (1000) users      (100)        0 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/
-drwxr-xr-x   0 guv       (1000) users      (100)        0 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib/
--rw-r--r--   0 guv       (1000) users      (100)        2 2021-08-05 18:52:14.000000 EDFlib-Python-1.0.6/src/EDFlib/__init__.py
--rw-r--r--   0 guv       (1000) users      (100)    70780 2022-01-14 18:08:29.000000 EDFlib-Python-1.0.6/src/EDFlib/edfreader.py
--rw-r--r--   0 guv       (1000) users      (100)    56043 2022-01-14 18:08:29.000000 EDFlib-Python-1.0.6/src/EDFlib/edfwriter.py
-drwxr-xr-x   0 guv       (1000) users      (100)        0 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/
--rw-r--r--   0 guv       (1000) users      (100)     1290 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/PKG-INFO
--rw-r--r--   0 guv       (1000) users      (100)      317 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/SOURCES.txt
--rw-r--r--   0 guv       (1000) users      (100)        1 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/dependency_links.txt
--rw-r--r--   0 guv       (1000) users      (100)       12 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/requires.txt
--rw-r--r--   0 guv       (1000) users      (100)        7 2022-01-15 08:43:19.000000 EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/top_level.txt
+drwxr-xr-x   0 guv       (1000) users      (100)        0 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/
+-rw-r--r--   0 guv       (1000) users      (100)     1770 2020-07-12 06:51:01.000000 EDFlib-Python-1.0.7/LICENSE
+-rw-r--r--   0 guv       (1000) users      (100)     1290 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/PKG-INFO
+-rw-r--r--   0 guv       (1000) users      (100)      615 2021-12-18 09:01:46.000000 EDFlib-Python-1.0.7/README.md
+-rw-r--r--   0 guv       (1000) users      (100)      104 2021-08-05 18:52:14.000000 EDFlib-Python-1.0.7/pyproject.toml
+-rw-r--r--   0 guv       (1000) users      (100)      783 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/setup.cfg
+drwxr-xr-x   0 guv       (1000) users      (100)        0 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/
+drwxr-xr-x   0 guv       (1000) users      (100)        0 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib/
+-rw-r--r--   0 guv       (1000) users      (100)        2 2021-08-05 18:52:14.000000 EDFlib-Python-1.0.7/src/EDFlib/__init__.py
+-rw-r--r--   0 guv       (1000) users      (100)    71229 2023-05-20 12:14:36.000000 EDFlib-Python-1.0.7/src/EDFlib/edfreader.py
+-rw-r--r--   0 guv       (1000) users      (100)    55728 2023-05-20 12:14:20.000000 EDFlib-Python-1.0.7/src/EDFlib/edfwriter.py
+drwxr-xr-x   0 guv       (1000) users      (100)        0 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/
+-rw-r--r--   0 guv       (1000) users      (100)     1290 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/PKG-INFO
+-rw-r--r--   0 guv       (1000) users      (100)      317 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 guv       (1000) users      (100)        1 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 guv       (1000) users      (100)       12 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/requires.txt
+-rw-r--r--   0 guv       (1000) users      (100)        7 2023-05-20 12:21:32.000000 EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/top_level.txt
```

### Comparing `EDFlib-Python-1.0.6/LICENSE` & `EDFlib-Python-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `EDFlib-Python-1.0.6/PKG-INFO` & `EDFlib-Python-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EDFlib-Python
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library to read/write EDF+/BDF+ files written in pure Python by the same author as the original EDFlib.
 Home-page: https://www.teuniz.net/edflib_python/
 Author: Teunis van Beelen
 Author-email: teuniz@protonmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/Teuniz/EDFlib-Python/-/issues
 Platform: UNKNOWN
```

### Comparing `EDFlib-Python-1.0.6/README.md` & `EDFlib-Python-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `EDFlib-Python-1.0.6/setup.cfg` & `EDFlib-Python-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EDFlib-Python
-version = 1.0.6
+version = 1.0.7
 author = Teunis van Beelen
 author_email = teuniz@protonmail.com
 description = Library to read/write EDF+/BDF+ files written in pure Python by the same author as the original EDFlib.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.teuniz.net/edflib_python/
 project_urls =
```

### Comparing `EDFlib-Python-1.0.6/src/EDFlib/edfreader.py` & `EDFlib-Python-1.0.7/src/EDFlib/edfreader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #############################################################################
 #
-# Copyright (c) 2020 Teunis van Beelen
+# Copyright (c) 2020 - 2023 Teunis van Beelen
 # All rights reserved.
 #
 # Email: teuniz@protonmail.com
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
@@ -28,15 +28,14 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 #############################################################################
 
 import sys
 import io
 import os
-import string
 import array
 from collections import namedtuple
 import numpy as np
 from datetime import datetime
 
 if sys.version_info[0] != 3 or sys.version_info[1] < 5:
   print("Must be using Python version >= 3.5.0")
@@ -163,15 +162,15 @@
   EDFLIB_TOO_MANY_SIGNALS           = -21
   EDFLIB_NO_SAMPLES_IN_RECORD       = -22
   EDFLIB_DIGMIN_IS_DIGMAX           = -23
   EDFLIB_DIGMAX_LOWER_THAN_DIGMIN   = -24
   EDFLIB_PHYSMIN_IS_PHYSMAX         = -25
   EDFLIB_DATARECORD_SIZE_TOO_BIG    = -26
 
-  EDFLIB_VERSION = 106
+  EDFLIB_VERSION = 107
 
 # max size of annotationtext
   __EDFLIB_WRITE_MAX_ANNOTATION_LEN = 40
 
 # bytes in datarecord for EDF annotations, must be an integer multiple of three and two
   __EDFLIB_ANNOTATION_BYTES = 114
 
@@ -214,15 +213,15 @@
 
     if sys.version_info[0] != 3 or sys.version_info[1] < 5:
       raise EDFexception("Must be using Python version >= 3.5.0")
 
     try:
       self.__file_in = open(path, "rb")
     except OSError as e:
-      raise EDFexception("Can not open file for reading: %s" %(e.strerror))
+      raise EDFexception("Cannot open file for reading: %s" %(e.strerror))
 
     self.__err = self.__checkEDFheader()
     if self.__err:
       self.__file_in.close()
       raise EDFexception("File is not valid EDF(+) or BDF(+).")
 
     if self.__discontinuous:
@@ -1006,14 +1005,16 @@
               duration_in_txt[j + 1] = 0
 
               duration = 1
               duration_start = 0
               n = 0
               continue
           n += 1
+    if error != 0:
+      return 9
     return 0
 
 ################################################################################
 # END __get_annotations
 ################################################################################
 
 ################################################################################
@@ -1138,27 +1139,34 @@
 
 ######################## RESERVED FIELD ########################################
 
     self.__reserved = hdr[192:236].decode("ascii")
 
     if self.__edf:
       self.__filetype = self.EDFLIB_FILETYPE_EDF
-      if self.__reserved[:5] == "EDF+C":
+      if self.__reserved[:44] == "EDF+C                                       ":
         self.__edfplus = 1
+        self.__discontinuous = 0
         self.__filetype = self.EDFLIB_FILETYPE_EDFPLUS
-      if self.__reserved[:5] == "EDF+D":
+      elif self.__reserved[:44] == "EDF+D                                       ":
         self.__edfplus = 1
         self.__discontinuous = 1
         self.__filetype = self.EDFLIB_FILETYPE_EDFPLUS
+      elif self.__reserved[:44] == "                                            ":
+        self.__edfplus = 0
+        self.__discontinuous = 0
+      else:
+        return -99
     if self.__bdf:
       self.__filetype = self.EDFLIB_FILETYPE_BDF
-      if self.__reserved[:5] == "BDF+C":
+      if self.__reserved[:44] == "BDF+C                                       ":
         self.__bdfplus = 1
+        self.__discontinuous = 0
         self.__filetype = self.EDFLIB_FILETYPE_BDFPLUS
-      if self.__reserved[:5] == "BDF+D":
+      if self.__reserved[:44] == "BDF+D                                       ":
         self.__bdfplus = 1
         self.__discontinuous = 1
         self.__filetype = self.EDFLIB_FILETYPE_BDFPLUS
 
 ##################### NUMBER OF DATARECORDS ####################################
 
     str8 = hdr[236:244]
@@ -1607,41 +1615,41 @@
       str128[4] += 32
       str128[5] += 32
       str128[6] = 32
       p += (i + 1)
       self.__plus_startdate = str128[0 : i].decode("ascii")
 
       if (str80[p] == ord('X')) and (str80[p + 1] == ord(' ')):
-        plus_admincode = ""
+        self.__plus_admincode = ""
         p += 2
       else:
         for i in range(0, 80 - p):
           if str80[i + p] == 32:
             break
           str128[i] = str80[i + p]
           if str128[i] == ord('_'):
             str128[i] = 32
         p += (i + 1)
         self.__plus_admincode = str128[0 : i].decode("ascii")
 
       if (str80[p] == ord('X')) and (str80[p + 1] == ord(' ')):
-        plus_technician = ""
+        self.__plus_technician = ""
         p += 2
       else:
         for i in range(0, 80 - p):
           if str80[i+p] == 32:
             break
           str128[i] = str80[i + p]
           if str128[i] == ord('_'):
             str128[i] = 32
         p += (i + 1)
         self.__plus_technician = str128[0 : i].decode("ascii")
 
       if (str80[p] == ord('X')) and (str80[p + 1] == ord(' ')):
-        plus_equipment = ""
+        self.__plus_equipment = ""
         p += 2
       else:
         for i in range(0, 80 - p):
           if str80[i + p] == 32:
             break
           str128[i] = str80[i + p]
           if str128[i] == ord('_'):
```

### Comparing `EDFlib-Python-1.0.6/src/EDFlib/edfwriter.py` & `EDFlib-Python-1.0.7/src/EDFlib/edfwriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #############################################################################
 #
-# Copyright (c) 2020 Teunis van Beelen
+# Copyright (c) 2020 - 2023 Teunis van Beelen
 # All rights reserved.
 #
 # Email: teuniz@protonmail.com
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright
@@ -27,17 +27,14 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 #############################################################################
 
 import sys
 import io
-import os
-import string
-import array
 from collections import namedtuple
 import numpy as np
 from datetime import datetime
 
 if sys.version_info[0] != 3 or sys.version_info[1] < 5:
   print("Must be using Python version >= 3.5.0")
   sys.exit()
@@ -104,18 +101,18 @@
 
   For a better explanation about the relation between digital data and physical data,
   read the document "Coding Schemes Used with Data Converters" (PDF):
 
   https://www.ti.com/general/docs/lit/getliterature.tsp?baseLiteratureNumber=sbaa042
 
   note: An EDF file usually contains multiple so-called datarecords. One datarecord usually has a duration of one second (this is the default but it is not mandatory!).
-  In that case a file with a duration of five minutes contains 300 datarecords. The duration of a datarecord can be freely choosen but, if possible, use values from
+  In that case a file with a duration of five minutes contains 300 datarecords. The duration of a datarecord can be freely chosen but, if possible, use values from
   0.1 to 1 second for easier handling. Just make sure that the total size of one datarecord, expressed in bytes, does not exceed 10MByte (15MBytes for BDF(+)).
 
-  The RECOMMENDATION of a maximum datarecordsize of 61440 bytes in the EDF and EDF+ specification was usefull in the time people were still using DOS as their main operating system.
+  The RECOMMENDATION of a maximum datarecordsize of 61440 bytes in the EDF and EDF+ specification was useful in the time people were still using DOS as their main operating system.
   Using DOS and fast (near) pointers (16-bit pointers), the maximum allocatable block of memory was 64KByte.
   This is not a concern anymore so the maximum datarecord size now is limited to 10MByte for EDF(+) and 15MByte for BDF(+). This helps to accommodate for higher samplingrates
   used by modern Analog to Digital Converters.
 
   EDF header character encoding: The EDF specification says that only (printable) ASCII characters are allowed.
   When writing the header info, EDFlib will assume you are using Latin1 encoding and it will automatically convert
   characters with accents, umlauts, tilde, etc. to their "normal" equivalent without the accent/umlaut/tilde/etc.
@@ -161,15 +158,15 @@
   EDFLIB_TOO_MANY_SIGNALS           = -21
   EDFLIB_NO_SAMPLES_IN_RECORD       = -22
   EDFLIB_DIGMIN_IS_DIGMAX           = -23
   EDFLIB_DIGMAX_LOWER_THAN_DIGMIN   = -24
   EDFLIB_PHYSMIN_IS_PHYSMAX         = -25
   EDFLIB_DATARECORD_SIZE_TOO_BIG    = -26
 
-  EDFLIB_VERSION = 106
+  EDFLIB_VERSION = 107
 
 # max size of annotationtext
   __EDFLIB_WRITE_MAX_ANNOTATION_LEN = 40
 
 # bytes in datarecord for EDF annotations, must be an integer multiple of three and two
   __EDFLIB_ANNOTATION_BYTES = 114
 
@@ -232,15 +229,15 @@
 
     if (self.__filetype != self.EDFLIB_FILETYPE_EDFPLUS) and (self.__filetype != self.EDFLIB_FILETYPE_BDFPLUS):
       raise EDFexception("Invalid filetype.")
 
     try:
       self.__file_out = open(self.__path, "wb")
     except OSError as e:
-      raise EDFexception("Can not open file for writing: %s" %(e.strerror))
+      raise EDFexception("Cannot open file for writing: %s" %(e.strerror))
 
     if self.__filetype == self.EDFLIB_FILETYPE_EDFPLUS:
       self.__edf = 1
     else:
       self.__bdf = 1
 
     self.__param_label = [""] * self.__edfsignals
@@ -807,16 +804,14 @@
 ################################################################################
 
 # writes the EDF header
   def __write_edf_header(self):
     if self.__status_ok == 0:
       return -1
 
-    eq_sf = 1
-
     self.__recordsize = 0
 
     str_ = bytearray(256)
 
     self.__total_annot_bytes = self.__EDFLIB_ANNOTATION_BYTES * self.__nr_annot_chns
 
     for i in range(0, self.__edfsignals):
@@ -830,18 +825,14 @@
         return self.EDFLIB_DIGMAX_LOWER_THAN_DIGMIN
 
       if self.__param_phys_max[i] == self.__param_phys_min[i]:
         return self.EDFLIB_PHYSMIN_IS_PHYSMAX
 
       self.__recordsize += self.__param_smp_per_record[i]
 
-      if i > 0:
-        if self.__param_smp_per_record[i] != self.__param_smp_per_record[i-1]:
-          eq_sf = 0
-
     if self.__edf != 0:
       self.__recordsize *= 2
       self.__recordsize += self.__total_annot_bytes
       if self.__recordsize > (10 * 1024 * 1024):  # datarecord size should not exceed 10MB for EDF
         return self.EDFLIB_DATARECORD_SIZE_TOO_BIG
           # if your application gets hit by this limitation, lower the value for the datarecord duration
           # using the function edf_set_datarecord_duration()
@@ -873,16 +864,15 @@
 
     p = 0
     if self.__plus_birthdate_year == 0:
       rest = 73
     else:
       rest = 63
 
-    self.__plus_patientcode.lstrip(" ")
-    self.__plus_patientcode.rstrip(" ")
+    self.__plus_patientcode = self.__plus_patientcode.strip()
     l = len(self.__plus_patientcode)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_patientcode, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
         rest = 0
@@ -915,16 +905,15 @@
       p += 2
     else:
       month_str = ["JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"]
       header[8 + p : 8 + p + 12] = bytes("%02d-%s-%04d " \
       %(self.__plus_birthdate_day, month_str[self.__plus_birthdate_month - 1], self.__plus_birthdate_year), encoding="ascii")
       p += 12
 
-    self.__plus_patient_name.lstrip(" ")
-    self.__plus_patient_name.rstrip(" ")
+    self.__plus_patient_name = self.__plus_patient_name.strip()
     l = len(self.__plus_patient_name)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_patient_name, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
         rest = 0
@@ -939,16 +928,15 @@
       header[8 + p] = 32
       p += 1
     else:
       header[8 + p : 8 + p + 2] = bytes("X ", encoding="ascii")
       p += 2
       rest -= 1
 
-    self.__plus_patient_additional.lstrip(" ")
-    self.__plus_patient_additional.rstrip(" ")
+    self.__plus_patient_additional = self.__plus_patient_additional.strip()
     l = len(self.__plus_patient_additional)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_patient_additional, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
       self.__latin1_to_ascii(str_, l)
@@ -970,16 +958,15 @@
     month_str = ["JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"]
     header[88 : 110] = bytes("Startdate %02d-%s-%04d " \
     %(self.__startdate_day, month_str[self.__startdate_month - 1], self.__startdate_year), encoding="ascii")
 
     p = 22
     rest = 50
 
-    self.__plus_admincode.lstrip(" ")
-    self.__plus_admincode.rstrip(" ")
+    self.__plus_admincode = self.__plus_admincode.strip()
     l = len(self.__plus_admincode)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_admincode, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
         rest = 0
@@ -994,16 +981,15 @@
       header[88 + p] = 32
       p += 1
     else:
       header[88 + p : 88 + p + 2] =  bytes("X ", encoding="ascii")
       p += 2
       rest -= 1
 
-    self.__plus_technician.lstrip(" ")
-    self.__plus_technician.rstrip(" ")
+    self.__plus_technician = self.__plus_technician.strip()
     l = len(self.__plus_technician)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_technician, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
         rest = 0
@@ -1018,16 +1004,15 @@
       header[88 + p] = 32
       p += 1
     else:
       header[88 + p : 88 + p + 2] =  bytes("X ", encoding="ascii")
       p += 2
       rest -= 1
 
-    self.__plus_equipment.lstrip(" ")
-    self.__plus_equipment.rstrip(" ")
+    self.__plus_equipment = self.__plus_equipment.strip()
     l = len(self.__plus_equipment)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_equipment, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
         rest = 0
@@ -1042,16 +1027,15 @@
       header[88 + p] = 32
       p += 1
     else:
       header[88 + p : 88 + p + 2] =  bytes("X ", encoding="ascii")
       p += 2
       rest -= 1
 
-    self.__plus_recording_additional.lstrip(" ")
-    self.__plus_recording_additional.rstrip(" ")
+    self.__plus_recording_additional = self.__plus_recording_additional.strip()
     l = len(self.__plus_recording_additional)
     if (l != 0) and (rest > 0):
       str_ = bytearray(self.__plus_recording_additional, encoding="latin_1")
       l = len(str_)
       if l > rest:
         l = rest
       self.__latin1_to_ascii(str_, l)
@@ -1208,15 +1192,14 @@
       scratchpad[i] = 0
     f.write(scratchpad)
 
     return 0
 
 # writes the annotations to the file
   def __write_annotations(self):
-    err = 0
     datrecs = 0
 
     str_ = bytearray(self.__EDFLIB_ANNOTATION_BYTES)
 
     offset = (self.__edfsignals + self.__nr_annot_chns + 1) * 256
 
     file_sz = offset + (self.__datarecords * self.__recordsize)
@@ -1277,17 +1260,17 @@
         if (annot2.duration % 10000) != 0:
           str_[p] = 46
           p += 1
           n = self.__snprint_ll_number_nonlocalized(str_, p, annot2.duration % 10000, 4, 0)
           p += n
       str_[p] = 20
       p += 1
-      annot2.description.lstrip(" ")
-      annot2.description.rstrip(" ")
-      ba_tmp = bytearray(annot2.description, encoding="utf-8")
+      tmp_str = str(annot2.description)
+      tmp_str = tmp_str.strip()
+      ba_tmp = bytearray(tmp_str, encoding="utf-8")
       l = self.__strlen(ba_tmp)
       if l > self.__EDFLIB_WRITE_MAX_ANNOTATION_LEN:
         l = self.__EDFLIB_WRITE_MAX_ANNOTATION_LEN
       str_[p : p + l] = ba_tmp[0 : l]
       p += l
       str_[p] = 20
       p += 1
```

### Comparing `EDFlib-Python-1.0.6/src/EDFlib_Python.egg-info/PKG-INFO` & `EDFlib-Python-1.0.7/src/EDFlib_Python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EDFlib-Python
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library to read/write EDF+/BDF+ files written in pure Python by the same author as the original EDFlib.
 Home-page: https://www.teuniz.net/edflib_python/
 Author: Teunis van Beelen
 Author-email: teuniz@protonmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/Teuniz/EDFlib-Python/-/issues
 Platform: UNKNOWN
```

