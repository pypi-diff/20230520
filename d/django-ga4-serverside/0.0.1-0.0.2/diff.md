# Comparing `tmp/django_ga4_serverside-0.0.1.tar.gz` & `tmp/django_ga4_serverside-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ga4_serverside-0.0.1.tar", last modified: Sun May 14 10:36:52 2023, max compression
+gzip compressed data, was "django_ga4_serverside-0.0.2.tar", last modified: Sat May 20 04:37:17 2023, max compression
```

## Comparing `django_ga4_serverside-0.0.1.tar` & `django_ga4_serverside-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-14 10:36:52.789887 django_ga4_serverside-0.0.1/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.1/.editorconfig
--rw-r--r--   0 mirec     (1000) mirec     (1000)      122 2023-05-13 09:42:18.000000 django_ga4_serverside-0.0.1/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.1/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)      736 2023-05-14 10:36:46.000000 django_ga4_serverside-0.0.1/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2023-05-13 10:29:29.000000 django_ga4_serverside-0.0.1/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2226 2023-05-14 10:36:52.789887 django_ga4_serverside-0.0.1/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1189 2023-05-14 10:32:57.000000 django_ga4_serverside-0.0.1/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-14 10:36:52.788887 django_ga4_serverside-0.0.1/django_ga4_serverside/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-05-13 09:41:44.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      267 2023-05-13 10:47:40.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/apps.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      431 2023-05-14 10:33:03.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/middleware.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-14 10:36:52.789887 django_ga4_serverside-0.0.1/django_ga4_serverside/signals/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-05-13 10:47:55.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/signals/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1530 2023-05-14 09:47:10.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/signals/handlers.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     6252 2023-05-14 10:24:13.000000 django_ga4_serverside-0.0.1/django_ga4_serverside/utils.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-14 10:36:52.788887 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2226 2023-05-14 10:36:52.000000 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      527 2023-05-14 10:36:52.000000 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-05-14 10:36:52.000000 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)      125 2023-05-14 10:36:52.000000 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       22 2023-05-14 10:36:52.000000 django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1468 2023-05-14 10:36:46.000000 django_ga4_serverside-0.0.1/pyproject.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-14 10:36:52.789887 django_ga4_serverside-0.0.1/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.1/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-20 04:37:17.125470 django_ga4_serverside-0.0.2/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.2/.editorconfig
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      122 2023-05-13 09:42:18.000000 django_ga4_serverside-0.0.2/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.2/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      898 2023-05-20 04:37:06.000000 django_ga4_serverside-0.0.2/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2023-05-13 10:29:29.000000 django_ga4_serverside-0.0.2/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2226 2023-05-20 04:37:17.125470 django_ga4_serverside-0.0.2/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1189 2023-05-14 10:32:57.000000 django_ga4_serverside-0.0.2/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-20 04:37:17.124470 django_ga4_serverside-0.0.2/django_ga4_serverside/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-05-13 09:41:44.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      267 2023-05-13 10:47:40.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/apps.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      431 2023-05-14 10:33:03.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/middleware.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-20 04:37:17.125470 django_ga4_serverside-0.0.2/django_ga4_serverside/signals/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-05-13 10:47:55.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/signals/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1616 2023-05-20 04:36:03.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/signals/handlers.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     6430 2023-05-20 04:19:56.000000 django_ga4_serverside-0.0.2/django_ga4_serverside/utils.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-05-20 04:37:17.124470 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2226 2023-05-20 04:37:17.000000 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      527 2023-05-20 04:37:17.000000 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-05-20 04:37:17.000000 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      125 2023-05-20 04:37:17.000000 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       22 2023-05-20 04:37:17.000000 django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1468 2023-05-20 04:37:06.000000 django_ga4_serverside-0.0.2/pyproject.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-20 04:37:17.125470 django_ga4_serverside-0.0.2/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-05-13 09:38:33.000000 django_ga4_serverside-0.0.2/setup.py
```

### Comparing `django_ga4_serverside-0.0.1/CHANGELOG.md` & `django_ga4_serverside-0.0.2/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 0.0.2 (2023-05-20)
+
+### Feat
+
+- Display request in debug mode
+- Send referer to page view event
+
+### Fix
+
+- send engagement_time_msec to enable user tracking
+
 ## 0.0.1 (2023-05-14)
 
 ### Feat
 
 - Added custom event documentation
 - Added crawler detection
 - Allow ignore paths using regex
```

### Comparing `django_ga4_serverside-0.0.1/LICENSE` & `django_ga4_serverside-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ga4_serverside-0.0.1/PKG-INFO` & `django_ga4_serverside-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_ga4_serverside
-Version: 0.0.1
+Version: 0.0.2
 Summary: Server side GA4 tracking
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-ga4-serverside
 Project-URL: documentation, https://github.com/mireq/django-ga4-serverside
 Project-URL: repository, https://github.com/mireq/django-ga4-serverside
 Project-URL: changelog, https://github.com/mireq/django-ga4-serverside/blob/master/CHANGELOG.md
```

### Comparing `django_ga4_serverside-0.0.1/README.rst` & `django_ga4_serverside-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_ga4_serverside-0.0.1/django_ga4_serverside/signals/handlers.py` & `django_ga4_serverside-0.0.2/django_ga4_serverside/signals/handlers.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,19 +32,21 @@
 	finally:
 		clear_context()
 
 	debug = getattr(settings, 'GA4_DEBUG', False)
 	query = urlencode({'measurement_id': settings.GA4_ID, 'api_secret': settings.GA4_SECRET})
 	url = MEASUREMENT_DEBUG_URL if debug else MEASUREMENT_URL
 	url = f'{url}{query}'
+	if debug:
+		sys.stdout.write(f"URL {url}\n")
+		sys.stdout.write(json.dumps(payload, indent=2) + '\n')
 
 	payload = json.dumps(payload).encode('utf-8')
 
 	req = request.Request(url)
 	req.add_header('Content-Type', 'application/json; charset=utf-8')
 	req.add_header('User-Agent', 'django_ga4_serverside')
 	result = request.urlopen(req, payload)
 	if result.status < 200 or result.status >= 300:
 		logger.warning("Failed to send event: %s", str(result.status))
 	if debug:
-		sys.stdout.write(f"URL {url}\n")
-		__import__('pprint').pprint(json.loads(result.read()))
+		sys.stdout.write(json.dumps(json.loads(result.read()), indent=2) + '\n')
```

### Comparing `django_ga4_serverside-0.0.1/django_ga4_serverside/utils.py` & `django_ga4_serverside-0.0.2/django_ga4_serverside/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,19 +184,23 @@
 				'name': 'page_view',
 				'params': page_info,
 			})
 
 	user_agent = context.request.headers.get('User-Agent')
 	if user_agent:
 		user_agent = user_agent[:100]
+	referer = context.request.headers.get('Referer')
 
 	for event in payload['events']:
-		if event['name'] == 'page_view':
-			if user_agent:
-				event['params']['user_agent'] = user_agent
+		event.setdefault('params', {})
+		event['params'].setdefault('engagement_time_msec', 1)
+
+		for field, value in [('user_agent', user_agent), ('page_referrer', referer)]:
+			if value:
+				event['params'].setdefault(field, value)
 
 	# don't send empty payloads
 	if not payload['events']:
 		return
 
 	return payload
```

### Comparing `django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/PKG-INFO` & `django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ga4-serverside
-Version: 0.0.1
+Version: 0.0.2
 Summary: Server side GA4 tracking
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-ga4-serverside
 Project-URL: documentation, https://github.com/mireq/django-ga4-serverside
 Project-URL: repository, https://github.com/mireq/django-ga4-serverside
 Project-URL: changelog, https://github.com/mireq/django-ga4-serverside/blob/master/CHANGELOG.md
```

### Comparing `django_ga4_serverside-0.0.1/django_ga4_serverside.egg-info/SOURCES.txt` & `django_ga4_serverside-0.0.2/django_ga4_serverside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_ga4_serverside-0.0.1/pyproject.toml` & `django_ga4_serverside-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -50,9 +50,9 @@
 where = ["."]
 include = ["django_ga4_serverside*"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.1"
+version = "0.0.2"
 tag_format = "$version"
```

