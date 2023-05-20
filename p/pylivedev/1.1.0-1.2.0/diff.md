# Comparing `tmp/pylivedev-1.1.0.tar.gz` & `tmp/pylivedev-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylivedev-1.1.0.tar", last modified: Mon Jan 16 16:23:48 2023, max compression
+gzip compressed data, was "pylivedev-1.2.0.tar", last modified: Sat May 20 20:34:14 2023, max compression
```

## Comparing `pylivedev-1.1.0.tar` & `pylivedev-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-01-16 16:23:48.316091 pylivedev-1.1.0/
--rw-r--r--   0 bast      (1002) bast      (1002)    11357 2021-06-08 11:58:06.000000 pylivedev-1.1.0/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)     4747 2023-01-16 16:23:48.316091 pylivedev-1.1.0/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)     4165 2023-01-16 16:22:41.000000 pylivedev-1.1.0/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-01-16 16:23:48.316091 pylivedev-1.1.0/pylivedev/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1411 2023-01-16 16:22:41.000000 pylivedev-1.1.0/pylivedev/__init__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1144 2022-02-24 19:29:26.000000 pylivedev-1.1.0/pylivedev/__main__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     7649 2023-01-16 16:22:41.000000 pylivedev-1.1.0/pylivedev/app.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3851 2022-03-04 22:22:15.000000 pylivedev-1.1.0/pylivedev/imports.py
--rw-rw-r--   0 bast      (1002) bast      (1002)      931 2022-03-03 16:55:55.000000 pylivedev-1.1.0/pylivedev/output.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-01-16 16:23:48.316091 pylivedev-1.1.0/pylivedev.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)     4747 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      366 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       54 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/entry_points.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       33 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       10 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 16:23:48.000000 pylivedev-1.1.0/pylivedev.egg-info/zip-safe
--rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-01-16 16:23:48.316091 pylivedev-1.1.0/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)      884 2023-01-16 16:22:41.000000 pylivedev-1.1.0/setup.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/
+-rw-r--r--   0 bast      (1002) bast      (1002)    11357 2021-06-08 11:58:06.000000 pylivedev-1.2.0/LICENSE
+-rw-rw-r--   0 bast      (1002) bast      (1002)     4766 2023-05-20 20:34:14.641251 pylivedev-1.2.0/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)     4184 2023-05-20 20:12:25.000000 pylivedev-1.2.0/README.md
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/pylivedev/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1410 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/__init__.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1143 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/__main__.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     7935 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/app.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     3850 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/imports.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)      930 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/output.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)       21 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/version.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/pylivedev.egg-info/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     4766 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      387 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       54 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/entry_points.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       33 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       10 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 16:23:48.000000 pylivedev-1.2.0/pylivedev.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-05-20 20:34:14.641251 pylivedev-1.2.0/setup.cfg
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1111 2023-05-20 20:34:00.000000 pylivedev-1.2.0/setup.py
```

### Comparing `pylivedev-1.1.0/LICENSE` & `pylivedev-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylivedev-1.1.0/PKG-INFO` & `pylivedev-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pylivedev
-Version: 1.1.0
+Version: 1.2.0
 Summary: PyLiveDev is used to keep track of files associated with your script so it can be re-started if any file is updated.
 Home-page: https://ouroboroscoding.com/pylivedev
 Author: Chris Nasr - OuroborosCoding
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/pylivedev
 Project-URL: Tracker, https://github.com/ouroboroscoding/pylivedev/issues
 Keywords: python,live,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyLiveDev](https://ouroboroscoding.com/pylivedev/PyLiveDev_128.png)
+![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
```

### Comparing `pylivedev-1.1.0/README.md` & `pylivedev-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![PyLiveDev](https://ouroboroscoding.com/pylivedev/PyLiveDev_128.png)
+![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
```

### Comparing `pylivedev-1.1.0/pylivedev/__init__.py` & `pylivedev-1.2.0/pylivedev/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,8 @@
 		for o in lApps:
 			o.stop()
 			del o
 
 	color('magenta', '\nGoodbye\n')
 
 	# Return OK
-	return True
+	return True
```

### Comparing `pylivedev-1.1.0/pylivedev/__main__.py` & `pylivedev-1.2.0/pylivedev/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 			)
 
 	except IOError as e:
 		print(e)
 
 # Only run if main
 if __name__ == '__main__':
-	cli()
+	cli()
```

### Comparing `pylivedev-1.1.0/pylivedev/app.py` & `pylivedev-1.2.0/pylivedev/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 		self._arguments = arguments
 		self._mode = mode and mode or 'script'
 		self._tracked = tracked
 		self._python = python or sys.executable
 		self._unbuffered = unbuffered
 		self._verbose = verbose
 
+		# If the mode is exe, override the tracked
+		if self._mode == 'exe':
+			self._tracked = False
+
 		# Init internal members
 		self._files = []
 		self._fresh_line = True
 
 		# Create a new observer if we are tracking
 		if self._tracked:
 			self._observer = Observer()
@@ -97,27 +101,36 @@
 		Private method to generate the full list of arguments based on the data
 		associated with the app
 
 		Returns:
 			None
 		"""
 
-		# Init the list with the python executable
-		self._args = [self._python]
+		# If we are running an exe
+		if self._mode == 'exe':
 
-		# If we are running unbuffered
-		if self._unbuffered:
-			self._args.append('-u')
+			# Init the list with the command passed
+			self._args = [self._command]
 
-		# If we are running a module
-		if self._mode == 'module':
-			self._args.append('-m')
+		# Else, we are running a python file
+		else:
+
+			# Init the list with the python executable
+			self._args = [self._python]
+
+			# If we are running unbuffered
+			if self._unbuffered:
+				self._args.append('-u')
+
+			# If we are running a module
+			if self._mode == 'module':
+				self._args.append('-m')
 
-		# Add the script/module
-		self._args.append(self._command)
+			# Add the script/module
+			self._args.append(self._command)
 
 		# If there's additional arguments to the script
 		if self._arguments and isinstance(self._arguments, list):
 			self._args.extend(self._arguments)
 
 		# If verbose, display list of arguments
 		if self._verbose:
@@ -328,8 +341,8 @@
 					output.verbose('\nProcessing not terminating, attempting to kill...')
 				self._process.kill()
 
 			if self._verbose:
 				output.verbose(' done\n')
 
 		# Delete the process
-		del self._process
+		del self._process
```

### Comparing `pylivedev-1.1.0/pylivedev/imports.py` & `pylivedev-1.2.0/pylivedev/imports.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -173,8 +173,8 @@
 
 		# Catch syntax errors from broken code
 		except SyntaxError as e:
 			output.error('Syntax Error parsing "%s" at line %d, column %d\n' % (
 				file,
 				e.args[1][1],
 				e.args[1][2]
-			))
+			))
```

### Comparing `pylivedev-1.1.0/pylivedev/output.py` & `pylivedev-1.2.0/pylivedev/output.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 	"""
 	sys.stdout.write(
 		colored(
 			msg,
 			color='white',
 			attrs=['bold']
 		)
-	)
+	)
```

### Comparing `pylivedev-1.1.0/pylivedev.egg-info/PKG-INFO` & `pylivedev-1.2.0/pylivedev.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pylivedev
-Version: 1.1.0
+Version: 1.2.0
 Summary: PyLiveDev is used to keep track of files associated with your script so it can be re-started if any file is updated.
 Home-page: https://ouroboroscoding.com/pylivedev
 Author: Chris Nasr - OuroborosCoding
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/pylivedev
 Project-URL: Tracker, https://github.com/ouroboroscoding/pylivedev/issues
 Keywords: python,live,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyLiveDev](https://ouroboroscoding.com/pylivedev/PyLiveDev_128.png)
+![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
```

### Comparing `pylivedev-1.1.0/setup.py` & `pylivedev-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-from setuptools import setup
+# Python imports
+from setuptools import setup, find_packages
+from distutils.util import convert_path
 
+# Shared long description
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
+# Shared version
+with open(convert_path('pylivedev/version.py')) as oF:
+	d = {}
+	exec(oF.read(), d)
+	version = d['__version__']
+
 setup(
 	name='pylivedev',
-	version='1.1.0',
+	version=version,
 	description='PyLiveDev is used to keep track of files associated with your script so it can be re-started if any file is updated.',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/pylivedev',
 	project_urls={
 		'Source': 'https://github.com/ouroboroscoding/pylivedev',
 		'Tracker': 'https://github.com/ouroboroscoding/pylivedev/issues'
```

