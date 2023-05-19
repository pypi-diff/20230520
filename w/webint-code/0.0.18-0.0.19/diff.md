# Comparing `tmp/webint_code-0.0.18.tar.gz` & `tmp/webint_code-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_code-0.0.18.tar", max compression
+gzip compressed data, was "webint_code-0.0.19.tar", max compression
```

## Comparing `webint_code-0.0.18.tar` & `webint_code-0.0.19.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1131 2023-05-19 19:02:23.791472 webint_code-0.0.18/pyproject.toml
--rw-r--r--   0        0        0    18936 2023-05-19 19:00:48.178126 webint_code-0.0.18/webint_code/__init__.py
--rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.18/webint_code/templates/__init__.py
--rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.18/webint_code/templates/index.html
--rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.18/webint_code/templates/project/commit.html
--rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.18/webint_code/templates/project/commit_log.html
--rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.18/webint_code/templates/project/created.html
--rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.18/webint_code/templates/project/index.html
--rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.18/webint_code/templates/project/issues.html
--rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.18/webint_code/templates/project/namespace.html
--rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.18/webint_code/templates/project/release.html
--rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.18/webint_code/templates/project/release_file.html
--rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.18/webint_code/templates/project/repository_file.html
--rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.18/webint_code/templates/project/settings.html
--rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.18/webint_code/templates/projects.html
--rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.18/webint_code/templates/pypi/index.html
--rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.18/webint_code/templates/pypi/project.html
--rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.18/webint_code/templates/search/index.html
--rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.18/webint_code/templates/search/results.html
--rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.18/webint_code/templates/system.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.18/webint_code/templates/template.html
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.18/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-19 23:00:52.259625 webint_code-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0    19164 2023-05-19 23:00:45.875528 webint_code-0.0.19/webint_code/__init__.py
+-rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.19/webint_code/templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.19/webint_code/templates/index.html
+-rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.19/webint_code/templates/project/commit.html
+-rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.19/webint_code/templates/project/commit_log.html
+-rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.19/webint_code/templates/project/created.html
+-rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.19/webint_code/templates/project/index.html
+-rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.19/webint_code/templates/project/issues.html
+-rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.19/webint_code/templates/project/namespace.html
+-rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.19/webint_code/templates/project/release.html
+-rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.19/webint_code/templates/project/release_file.html
+-rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.19/webint_code/templates/project/repository_file.html
+-rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.19/webint_code/templates/project/settings.html
+-rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.19/webint_code/templates/projects.html
+-rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.19/webint_code/templates/pypi/index.html
+-rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.19/webint_code/templates/pypi/project.html
+-rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.19/webint_code/templates/search/index.html
+-rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.19/webint_code/templates/search/results.html
+-rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.19/webint_code/templates/system.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.19/webint_code/templates/template.html
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.19/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.19/PKG-INFO
```

### Comparing `webint_code-0.0.18/pyproject.toml` & `webint_code-0.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-code"
-version = "0.0.18"
+version = "0.0.19"
 description = "manage code on your website"
 keywords = ["webint", "Git", "PyPI"]
 homepage = "https://ragt.ag/code/projects/webint-code"
 repository = "https://ragt.ag/code/projects/webint-code.git"
 documentation = "https://ragt.ag/code/projects/webint-code/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `webint_code-0.0.18/webint_code/__init__.py` & `webint_code-0.0.19/webint_code/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,21 +172,28 @@
     subprocess.run(["chgrp", "www-data", bare_repo, working_repo, "-R"])
     subprocess.run(["chmod", "g+w", bare_repo, working_repo, "-R"])
     if not (meta_dir / "gitpasswd").exists():
         token = web.application("webint_auth").model.generate_local_token(
             "/code", "webint_code", "git_owner"
         )
         subprocess.run(["htpasswd", "-cb", meta_dir / "gitpasswd", "owner", token])
-
     # XXX subprocess.run(["sudo", "service", "nginx", "restart"])
 
     # XXX gmpg.clone_repo(
     # XXX     f"{web.tx.origin}/code/projects/{name}.git", f"{working_dir}/{name}"
     # XXX )
 
+    web.application("webint_posts").model.create(
+        "entry",
+        url=f"/code/projects/{name}",
+        content=(
+            f"Created repository <a href=/code/projects/{name}><code>{name}</code></a>"
+        ),
+    )
+
 
 @app.query
 def get_projects(db):
     """Return a list of project names."""
     visibility_wheres = ["public"]
     if web.tx.user.is_owner:
         visibility_wheres.extend(["protected", "private"])
```

### Comparing `webint_code-0.0.18/webint_code/templates/project/commit.html` & `webint_code-0.0.19/webint_code/templates/project/commit.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/commit_log.html` & `webint_code-0.0.19/webint_code/templates/project/commit_log.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/index.html` & `webint_code-0.0.19/webint_code/templates/project/index.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/issues.html` & `webint_code-0.0.19/webint_code/templates/project/issues.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/namespace.html` & `webint_code-0.0.19/webint_code/templates/project/namespace.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/release_file.html` & `webint_code-0.0.19/webint_code/templates/project/release_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/project/repository_file.html` & `webint_code-0.0.19/webint_code/templates/project/repository_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/search/results.html` & `webint_code-0.0.19/webint_code/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/webint_code/templates/system.html` & `webint_code-0.0.19/webint_code/templates/system.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.18/setup.py` & `webint_code-0.0.19/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['code = webint_code:app']}
 
 setup_kwargs = {
     'name': 'webint-code',
-    'version': '0.0.18',
+    'version': '0.0.19',
     'description': 'manage code on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-code',
```

### Comparing `webint_code-0.0.18/PKG-INFO` & `webint_code-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-code
-Version: 0.0.18
+Version: 0.0.19
 Summary: manage code on your website
 Home-page: https://ragt.ag/code/projects/webint-code
 License: BSD-2-Clause
 Keywords: webint,Git,PyPI
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

