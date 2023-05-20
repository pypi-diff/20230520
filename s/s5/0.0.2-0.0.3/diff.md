# Comparing `tmp/s5-0.0.2.tar.gz` & `tmp/s5-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ym/Code/s5/dist/.tmp-zov782fz/s5-0.0.2.tar", last modified: Mon May 15 02:41:46 2023, max compression
+gzip compressed data, was "/home/ym/Code/s5/dist/.tmp-bnbdp7fv/s5-0.0.3.tar", last modified: Sat May 20 20:40:34 2023, max compression
```

## Comparing `s5-0.0.2.tar` & `s5-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-15 02:41:46.047285 s5-0.0.2/
--rw-r--r--   0 ym        (1000) ym        (1000)    35149 2023-03-18 16:19:20.000000 s5-0.0.2/LICENSE
--rw-r--r--   0 ym        (1000) ym        (1000)     2146 2023-05-15 02:41:46.047285 s5-0.0.2/PKG-INFO
--rw-r--r--   0 ym        (1000) ym        (1000)     1715 2023-03-19 02:34:39.000000 s5-0.0.2/README.md
--rw-r--r--   0 ym        (1000) ym        (1000)      483 2023-05-15 02:41:38.000000 s5-0.0.2/pyproject.toml
-drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-15 02:41:46.043952 s5-0.0.2/s5/
--rw-r--r--   0 ym        (1000) ym        (1000)       53 2023-03-18 17:17:48.000000 s5-0.0.2/s5/__init__.py
--rw-r--r--   0 ym        (1000) ym        (1000)       21 2023-05-15 02:41:39.000000 s5-0.0.2/s5/_version.py
--rw-r--r--   0 ym        (1000) ym        (1000)     1244 2023-03-18 17:18:08.000000 s5-0.0.2/s5/client.py
--rw-r--r--   0 ym        (1000) ym        (1000)     5536 2023-03-30 03:41:52.000000 s5-0.0.2/s5/server.py
-drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-15 02:41:46.047285 s5-0.0.2/s5.egg-info/
--rw-r--r--   0 ym        (1000) ym        (1000)     2146 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/PKG-INFO
--rw-r--r--   0 ym        (1000) ym        (1000)      255 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/SOURCES.txt
--rw-r--r--   0 ym        (1000) ym        (1000)        1 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/dependency_links.txt
--rw-r--r--   0 ym        (1000) ym        (1000)       60 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/entry_points.txt
--rw-r--r--   0 ym        (1000) ym        (1000)        7 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/requires.txt
--rw-r--r--   0 ym        (1000) ym        (1000)        3 2023-05-15 02:41:46.000000 s5-0.0.2/s5.egg-info/top_level.txt
--rw-r--r--   0 ym        (1000) ym        (1000)       38 2023-05-15 02:41:46.047285 s5-0.0.2/setup.cfg
--rw-r--r--   0 ym        (1000) ym        (1000)      550 2023-05-15 02:28:07.000000 s5-0.0.2/setup.py
+drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-20 20:40:34.175095 s5-0.0.3/
+-rw-r--r--   0 ym        (1000) ym        (1000)    35149 2023-03-18 16:19:20.000000 s5-0.0.3/LICENSE
+-rw-r--r--   0 ym        (1000) ym        (1000)     2146 2023-05-20 20:40:34.175095 s5-0.0.3/PKG-INFO
+-rw-r--r--   0 ym        (1000) ym        (1000)     1715 2023-03-19 02:34:39.000000 s5-0.0.3/README.md
+-rw-r--r--   0 ym        (1000) ym        (1000)      483 2023-05-20 20:39:11.000000 s5-0.0.3/pyproject.toml
+drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-20 20:40:34.175095 s5-0.0.3/s5/
+-rw-r--r--   0 ym        (1000) ym        (1000)       53 2023-03-18 17:17:48.000000 s5-0.0.3/s5/__init__.py
+-rw-r--r--   0 ym        (1000) ym        (1000)       21 2023-05-20 20:38:39.000000 s5-0.0.3/s5/_version.py
+-rw-r--r--   0 ym        (1000) ym        (1000)     1244 2023-03-18 17:18:08.000000 s5-0.0.3/s5/client.py
+-rw-r--r--   0 ym        (1000) ym        (1000)     5650 2023-05-20 20:38:34.000000 s5-0.0.3/s5/server.py
+drwxr-xr-x   0 ym        (1000) ym        (1000)        0 2023-05-20 20:40:34.175095 s5-0.0.3/s5.egg-info/
+-rw-r--r--   0 ym        (1000) ym        (1000)     2146 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/PKG-INFO
+-rw-r--r--   0 ym        (1000) ym        (1000)      255 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/SOURCES.txt
+-rw-r--r--   0 ym        (1000) ym        (1000)        1 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/dependency_links.txt
+-rw-r--r--   0 ym        (1000) ym        (1000)       60 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/entry_points.txt
+-rw-r--r--   0 ym        (1000) ym        (1000)        7 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/requires.txt
+-rw-r--r--   0 ym        (1000) ym        (1000)        3 2023-05-20 20:40:34.000000 s5-0.0.3/s5.egg-info/top_level.txt
+-rw-r--r--   0 ym        (1000) ym        (1000)       38 2023-05-20 20:40:34.175095 s5-0.0.3/setup.cfg
+-rw-r--r--   0 ym        (1000) ym        (1000)      550 2023-05-15 02:28:07.000000 s5-0.0.3/setup.py
```

### Comparing `s5-0.0.2/LICENSE` & `s5-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s5-0.0.2/PKG-INFO` & `s5-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5
-Version: 0.0.2
+Version: 0.0.3
 Summary: SciNet Super Simple Secrets Server
 Author: Yohai Meiron
 Author-email: Yohai Meiron <yohai.meiron@scinet.utoronto.ca>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `s5-0.0.2/README.md` & `s5-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `s5-0.0.2/s5/client.py` & `s5-0.0.3/s5/client.py`

 * *Files identical despite different names*

### Comparing `s5-0.0.2/s5/server.py` & `s5-0.0.3/s5/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     ptr = (ctypes.c_byte * size).from_address(id(obj) + sys.getsizeof(obj) - size - 1)
     mask = b'X'*size
     ctypes.memmove(ptr, mask, size)
 
 def server():
     parser = argparse.ArgumentParser(description='Store a short secret in memory.', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('--bind-address', default='0.0.0.0', help='Bind address')
-    parser.add_argument('--port-min', default='13500', help='First port to try to bind to')
-    parser.add_argument('--port-max', default='13599', help='Maximum port number to attempt')
+    parser.add_argument('--port-min', type=int, default=13500, help='First port to try to bind to')
+    parser.add_argument('--port-max', type=int, default=13599, help='Maximum port number to attempt')
     parser.add_argument('--client-file', default='~/.s5client.json', help='File for client process')
     parser.add_argument('--no-client-file', action='store_true', help='If set, no client file is produced, token shown on screen')
     parser.add_argument('--foreground', action='store_true', help='Do not go to background')
-    parser.add_argument('--logfile', default='~/s5server.log', help='Log filename')
-    parser.add_argument('--success-max', default=1, help='Turn server off after that many successful attempts (0 for unlimited)')
-    parser.add_argument('--failure-max', default=0, help='Turn server off after that many failed attempts (0 for unlimited)')
+    parser.add_argument('--logfile', default='~/s5server.log', help='Log filename (use "stdout" to output to screen)')
+    parser.add_argument('--success-max', type=int, default=1, help='Turn server off after that many successful attempts (0 for unlimited)')
+    parser.add_argument('--failure-max', type=int, default=0, help='Turn server off after that many failed attempts (0 for unlimited)')
     args = parser.parse_args()
 
     token = secrets.token_bytes(96)
     identifier = token[:48]
     symkey = token[48:]
 
     secret_text = getpass.getpass('Enter secret: ')
@@ -97,19 +97,21 @@
     gc.collect()
 
     if not args.foreground:
         if (pid := os.fork()) > 0: exit(0)
 
     app = application = falcon.App()
 
-    Request_handler.logfile = open(os.path.expanduser(args.logfile), 'a')
+    if args.logfile == 'stdout':
+        Request_handler.logfile = sys.stdout
+    else:
+        Request_handler.logfile = open(os.path.expanduser(args.logfile), 'a')
 
-    port_min, port_max = int(args.port_min), int(args.port_max)
-    for port in range(port_min, port_max+2):
-        if port > port_max: raise RuntimeError('Could not find a free port.')
+    for port in range(args.port_min, args.port_max+2):
+        if port > args.port_max: raise RuntimeError('Could not find a free port.')
         try:
             httpd = wsgiref.simple_server.make_server(args.bind_address, port, app, handler_class=Request_handler)
             break
         except OSError:
             pass
     hostname = socket.gethostname()
     print(f'Process {os.getpid()} listening on {hostname} on port {port}.')
```

### Comparing `s5-0.0.2/s5.egg-info/PKG-INFO` & `s5-0.0.3/s5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5
-Version: 0.0.2
+Version: 0.0.3
 Summary: SciNet Super Simple Secrets Server
 Author: Yohai Meiron
 Author-email: Yohai Meiron <yohai.meiron@scinet.utoronto.ca>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `s5-0.0.2/setup.py` & `s5-0.0.3/setup.py`

 * *Files identical despite different names*

