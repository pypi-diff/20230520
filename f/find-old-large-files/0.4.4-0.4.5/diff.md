# Comparing `tmp/find_old_large_files-0.4.4.tar.gz` & `tmp/find_old_large_files-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.4.4.tar", last modified: Fri May 19 21:51:22 2023, max compression
+gzip compressed data, was "find_old_large_files-0.4.5.tar", last modified: Fri May 19 22:04:56 2023, max compression
```

## Comparing `find_old_large_files-0.4.4.tar` & `find_old_large_files-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:04:56.154106 find_old_large_files-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 22:04:40.000000 find_old_large_files-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 22:04:56.154106 find_old_large_files-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 22:04:40.000000 find_old_large_files-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:04:56.150105 find_old_large_files-0.4.5/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 22:04:40.000000 find_old_large_files-0.4.5/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-19 22:04:40.000000 find_old_large_files-0.4.5/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:04:56.154106 find_old_large_files-0.4.5/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 22:04:56.000000 find_old_large_files-0.4.5/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:04:56.154106 find_old_large_files-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 22:04:40.000000 find_old_large_files-0.4.5/setup.py
```

### Comparing `find_old_large_files-0.4.4/LICENSE` & `find_old_large_files-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.4/PKG-INFO` & `find_old_large_files-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.4.4
+Version: 0.4.5
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.4/README.md` & `find_old_large_files-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.4/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.4.5/find_old_large_files/find_old_large_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,26 +73,41 @@
                 pbar.update()
         logging.info('Finished moving files')
 
 def main():
     home = str(Path.home())
 
     parser = argparse.ArgumentParser(description="Find and remove large, old files.")
-    parser.add_argument("--size", type=int, default=100, help="File size limit in MB")
+    parser.add_argument("--size", type=int, default=100, help="File size limit in MB, it will be converted to bytes")
     parser.add_argument("--days", type=int, default=365, help="File age limit in days")
     parser.add_argument("--dir", type=str, default=home, help="Directory to scan")
     parser.add_argument("--exclude", type=str, nargs='*', default=['.docx', '.xlsx'], help="File extensions to exclude")
     parser.add_argument("--trash", type=str, default=os.path.join(home, 'trash'), help="Directory to move files to")
 
     args = parser.parse_args()
 
-    scanner = FileScanner(args.dir_path, args.size_limit, args.days_limit, args.excluded_extensions, args.trash_dir)
+    # Ensure provided directories exist
+    if not os.path.isdir(args.dir):
+        print(f"The provided directory '{args.dir}' does not exist.")
+        return
+    if not os.path.exists(args.trash):
+        os.makedirs(args.trash, exist_ok=True)
+
+    size_limit = args.size * 1024 * 1024  # Convert size from MB to bytes
+
+    scanner = FileScanner(args.dir, size_limit, args.days, args.exclude, args.trash)
 
     scanner.scan_files()
     print(f"Total size to be moved to trash: {scanner.total_size_in_gb():.2f} GB")
 
-    choice = input("Do you want to move these files to trash? (yes/no): ")
-    if choice.lower() == 'yes':
-        scanner.move_files_to_trash()
+    while True:
+        choice = input("Do you want to move these files to trash? (yes/no): ")
+        if choice.lower() == 'yes':
+            scanner.move_files_to_trash()
+            break
+        elif choice.lower() == 'no':
+            break
+        else:
+            print("Invalid input. Please enter 'yes' or 'no'.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `find_old_large_files-0.4.4/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.4.5/find_old_large_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.4.4
+Version: 0.4.5
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.4/setup.py` & `find_old_large_files-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.4.4",  # Increment the version here
+    version="0.4.5",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

