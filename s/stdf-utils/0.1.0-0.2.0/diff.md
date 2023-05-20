# Comparing `tmp/stdf-utils-0.1.0.tar.gz` & `tmp/stdf-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf-utils-0.1.0.tar", last modified: Tue May 16 05:24:29 2023, max compression
+gzip compressed data, was "stdf-utils-0.2.0.tar", last modified: Sat May 20 07:49:24 2023, max compression
```

## Comparing `stdf-utils-0.1.0.tar` & `stdf-utils-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 05:24:29.054106 stdf-utils-0.1.0/
--rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1340 2023-05-16 05:24:29.052104 stdf-utils-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 05:24:29.054106 stdf-utils-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-16 00:47:39.000000 stdf-utils-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:24:28.981740 stdf-utils-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 05:24:29.014104 stdf-utils-0.1.0/src/stdf_utils/
--rw-rw-rw-   0        0        0      102 2023-05-16 00:48:39.000000 stdf-utils-0.1.0/src/stdf_utils/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-05-16 00:54:49.000000 stdf-utils-0.1.0/src/stdf_utils/stdf_reader.py
--rw-rw-rw-   0        0        0    27360 2023-05-16 00:49:16.000000 stdf-utils-0.1.0/src/stdf_utils/stdf_record.py
--rw-rw-rw-   0        0        0      663 2023-05-16 00:45:08.000000 stdf-utils-0.1.0/src/stdf_utils/util.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:24:29.037104 stdf-utils-0.1.0/src/stdf_utils.egg-info/
--rw-rw-rw-   0        0        0     1340 2023-05-16 05:24:28.000000 stdf-utils-0.1.0/src/stdf_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-16 05:24:28.000000 stdf-utils-0.1.0/src/stdf_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 05:24:28.000000 stdf-utils-0.1.0/src/stdf_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 05:24:28.000000 stdf-utils-0.1.0/src/stdf_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 05:24:29.046110 stdf-utils-0.1.0/tests/
--rw-rw-rw-   0        0        0      411 2023-05-16 00:58:10.000000 stdf-utils-0.1.0/tests/test_stdf_reader.py
--rw-rw-rw-   0        0        0      428 2023-05-16 00:49:02.000000 stdf-utils-0.1.0/tests/test_stdf_record.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.290698 stdf-utils-0.2.0/
+-rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1340 2023-05-20 07:49:24.288697 stdf-utils-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 07:49:24.291697 stdf-utils-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-20 07:32:15.000000 stdf-utils-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.226051 stdf-utils-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.257050 stdf-utils-0.2.0/src/stdf_utils/
+-rw-rw-rw-   0        0        0      208 2023-05-20 06:47:21.000000 stdf-utils-0.2.0/src/stdf_utils/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_patch.py
+-rw-rw-rw-   0        0        0     2340 2023-05-20 07:27:00.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_per_td.py
+-rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_record.py
+-rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_to_csv.py
+-rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_to_txt.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.0/src/stdf_utils/util.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.270049 stdf-utils-0.2.0/src/stdf_utils.egg-info/
+-rw-rw-rw-   0        0        0     1340 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.285715 stdf-utils-0.2.0/tests/
+-rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.0/tests/test_stdf_patch.py
+-rw-rw-rw-   0        0        0      449 2023-05-20 07:30:00.000000 stdf-utils-0.2.0/tests/test_stdf_per_td.py
+-rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.0/tests/test_stdf_record.py
+-rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.0/tests/test_stdf_to_csv.py
+-rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.0/tests/test_stdf_to_txt.py
```

### Comparing `stdf-utils-0.1.0/LICENSE` & `stdf-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.1.0/PKG-INFO` & `stdf-utils-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.1.0/setup.py` & `stdf-utils-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 NAME = 'stdf-utils'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'stdf file parser and emitter'
 LONG_DESCRIPTION = """\
 stdf is the standard format of ATE result, and this pacakge supports
 reading and (possibly) editing the stdf file comes form ATE.
 """
 AUTHOR = "Peter JC. Wu"
 AUTHOR_EMAIL = "wolf952@gmail.com"
```

### Comparing `stdf-utils-0.1.0/src/stdf_utils/stdf_reader.py` & `stdf-utils-0.2.0/src/stdf_utils/stdf_to_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import csv
 import statistics
 from collections import defaultdict
 from .stdf_record import StdfRecord
 from .util import OpenFile
 
 
-class StdfReader:
-    def __init__(self, file_path: str):
+class StdfToCsv:
+    def __init__(self, stdf_path: str, csv_path: str = None):
+        self.stdf_path = stdf_path
+        self.csv_path = csv_path or stdf_path.replace(".gz", "").replace(".stdf", ".csv")
         self.ptr_container = PTRContainer()
         self.handlers = {
             "Ptr": self.ptr_handler,
         }
-        with OpenFile(file_path) as f_in:
+        # read
+        with OpenFile(stdf_path) as f_in:
             for rec_type, rec in StdfRecord(f_in, set(self.handlers.keys())):
                 self.handlers[rec_type](rec)
+        # write
+        self._to_csv()
 
     def ptr_handler(self, rec: dict):
         self.ptr_container.push(rec)
 
-    def export_csv(self, fp: str):
+    def _to_csv(self):
         fieldnames = ["Test ID", "Site", "Name", "Execs", "Fails", "Low Lim", "High Lim", "Min", "Max", "Mean"]
-        writer = csv.DictWriter(fp, fieldnames=fieldnames)
-        writer.writeheader()
-        for test_name, sites in self.ptr_container.data.items():
-            for i, site_data in enumerate(sites):
-                data = [d["RESULT"] for d in site_data]
-                if len(data) == 0:
-                    continue
-                writer.writerow({
-                    "Test ID": site_data[0]["TEST_NUM"],
-                    "Site": site_data[0]["SITE_NUM"],
-                    "Name": test_name,
-                    "Execs": len(data),
-                    "Fails": len([d for d in data if d < site_data[0]["LO_LIMIT"] or d > site_data[0]["HI_LIMIT"]]),
-                    "Low Lim": site_data[0]["LO_LIMIT"],
-                    "High Lim": site_data[0]["HI_LIMIT"],
-                    "Min": min(data),
-                    "Max": max(data),
-                    "Mean": statistics.mean(data),
-                })
+        with open(self.csv_path, "w", newline="") as f_out:
+            writer = csv.DictWriter(f_out, fieldnames=fieldnames)
+            writer.writeheader()
+            for test_name, sites in self.ptr_container.data.items():
+                for i, site_data in enumerate(sites):
+                    data = [d["RESULT"] for d in site_data]
+                    if len(data) == 0:
+                        continue
+                    writer.writerow({
+                        "Test ID": site_data[0]["TEST_NUM"],
+                        "Site": site_data[0]["SITE_NUM"],
+                        "Name": test_name.decode(),
+                        "Execs": len(data),
+                        "Fails": len([d for d in data if d < site_data[0]["LO_LIMIT"] or d > site_data[0]["HI_LIMIT"]]),
+                        "Low Lim": site_data[0]["LO_LIMIT"],
+                        "High Lim": site_data[0]["HI_LIMIT"],
+                        "Min": min(data),
+                        "Max": max(data),
+                        "Mean": statistics.mean(data),
+                    })
 
 
 class PTRContainer:
     def __init__(self, key_type: str = "name"):
         self._key_type = key_type
         self.data = defaultdict(list)
```

### Comparing `stdf-utils-0.1.0/src/stdf_utils/stdf_record.py` & `stdf-utils-0.2.0/src/stdf_utils/stdf_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,73 +8,80 @@
 class StdfRecord:
     def __init__(self, fp, parse_types: set = None):
         self.fp = fp
         self.record_table = self._get_record_table()
         self.parse_types: set = parse_types or {r["name"] for r in self.record_table.values()}
         self.endian = "@"
         # cache
-        self._rec_type: str = ""
+        self.buffer: bytes = b''
+        self.rec_type: str = ""
         self._rec_fields: Tuple[Tuple[str, str]] = tuple()
         self._data: Dict[str, Any] = {}
 
     def __iter__(self):
         while True:
             try:
-                record = self._get_next_record()
+                record = self.get_next_record()
                 if record is not None:
-                    yield self._rec_type, record
+                    yield self.rec_type, record
 
             except EOFError:
                 logging.debug("Completed...")
                 break
 
             except BufferError:
                 logging.error("Incomplete log...")
                 break
 
-    def _get_next_record(self):
+    def get_next_record(self):
         if self.endian == "@":
-            self.far_handler()
-            return None  # do not return Far
+            return self.far_handler()
 
         # reset
-        self._rec_type = ""
+        self.rec_type = ""
         self._rec_fields = tuple()
         self._data = {}
 
         # read header (4 bytes)
         header = self.fp.read(4)
         if len(header) == 0:
             raise EOFError
 
         elif len(header) != 4:
             raise BufferError
 
         body = self.fp.read(unp(self.endian, 'H', header[0:2]))
+        self.buffer = header + body
         key: int = header[2] * 1000 + header[3]  # typ * 1000 + sub
-        record = self.record_table.get(key)
-        if record is None:
+        if key not in self.record_table:
             logging.error(f"Unknown key: {key}")
             return None
 
         # parse type filter
-        self._rec_type = record["name"]
+        record = self.record_table[key]
+        self.rec_type = record["name"]
         if record["name"] in self.parse_types:
             return self.parse(record, body)
 
     def far_handler(self):
-        buf = self.fp.read(6)
+        self.rec_type = "Far"
+        self.buffer = self.fp.read(6)
+
+        buf = self.buffer
         cpu_type = buf[4]
         if cpu_type == 1:
             self.endian = ">"
         elif cpu_type == 2:
             self.endian = "<"
         else:
             raise ValueError(f"Cpu type '{cpu_type}' is not supported...")
 
+        return self.parse(self.record_table[10], buf[4:]) \
+            if "Far" in self.parse_types else None
+
     def parse(self, record, body):
         self._rec_fields = record["fields"]
         for field_name, fmt in self._rec_fields:
             val, body = self._get_parse_func(fmt)(fmt, body)
             self._data[field_name] = val
         return self._data
```

### Comparing `stdf-utils-0.1.0/src/stdf_utils/util.py` & `stdf-utils-0.2.0/src/stdf_utils/util.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.1.0/src/stdf_utils.egg-info/PKG-INFO` & `stdf-utils-0.2.0/src/stdf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

