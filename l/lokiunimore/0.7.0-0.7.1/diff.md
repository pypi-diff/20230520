# Comparing `tmp/lokiunimore-0.7.0.tar.gz` & `tmp/lokiunimore-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokiunimore-0.7.0.tar", max compression
+gzip compressed data, was "lokiunimore-0.7.1.tar", max compression
```

## Comparing `lokiunimore-0.7.0.tar` & `lokiunimore-0.7.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0    34523 2022-09-12 07:14:39.309540 lokiunimore-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     3234 2023-05-20 17:24:22.739375 lokiunimore-0.7.0/README.md
--rw-r--r--   0        0        0       22 2022-09-09 23:37:05.679098 lokiunimore-0.7.0/lokiunimore/config/__init__.py
--rw-r--r--   0        0        0       41 2022-09-11 01:13:26.488730 lokiunimore-0.7.0/lokiunimore/config/__main__.py
--rw-r--r--   0        0        0     6187 2022-09-16 12:02:50.924023 lokiunimore-0.7.0/lokiunimore/config/config.py
--rw-r--r--   0        0        0       22 2022-09-12 07:14:39.419540 lokiunimore-0.7.0/lokiunimore/matrix/__init__.py
--rw-r--r--   0        0        0      758 2023-05-20 16:25:25.326851 lokiunimore-0.7.0/lokiunimore/matrix/__main__.py
--rw-r--r--   0        0        0    21685 2023-05-20 16:52:12.169800 lokiunimore-0.7.0/lokiunimore/matrix/client.py
--rw-r--r--   0        0        0     3083 2023-05-20 17:15:57.638520 lokiunimore-0.7.0/lokiunimore/matrix/templates/messages.py
--rw-r--r--   0        0        0       22 2022-09-09 23:45:02.955105 lokiunimore-0.7.0/lokiunimore/sql/__init__.py
--rw-r--r--   0        0        0      260 2022-09-14 02:12:05.840975 lokiunimore-0.7.0/lokiunimore/sql/__main__.py
--rw-r--r--   0        0        0     4905 2023-05-20 16:07:43.524933 lokiunimore-0.7.0/lokiunimore/sql/tables.py
--rw-r--r--   0        0        0      348 2022-09-11 02:48:06.533186 lokiunimore-0.7.0/lokiunimore/utils/device_names.py
--rw-r--r--   0        0        0      888 2022-09-12 07:14:39.521540 lokiunimore-0.7.0/lokiunimore/utils/logs.py
--rw-r--r--   0        0        0       19 2022-09-12 07:14:39.708540 lokiunimore-0.7.0/lokiunimore/web/__init__.py
--rw-r--r--   0        0        0      236 2022-09-16 12:02:50.925022 lokiunimore-0.7.0/lokiunimore/web/__main__.py
--rw-r--r--   0        0        0     5511 2023-05-20 15:09:54.328778 lokiunimore-0.7.0/lokiunimore/web/app.py
--rw-r--r--   0        0        0     1907 2023-05-20 14:09:26.998276 lokiunimore-0.7.0/lokiunimore/web/extensions/matrix_client.py
--rw-r--r--   0        0        0    67646 2022-09-12 07:40:28.587432 lokiunimore-0.7.0/lokiunimore/web/static/favicon.ico
--rw-r--r--   0        0        0     8288 2022-09-12 07:40:19.534432 lokiunimore-0.7.0/lokiunimore/web/static/icon.png
--rw-r--r--   0        0        0     9408 2022-12-22 19:17:21.649603 lokiunimore-0.7.0/lokiunimore/web/static/newcode.png
--rw-r--r--   0        0        0   151500 2022-09-14 02:23:19.041943 lokiunimore-0.7.0/lokiunimore/web/static/opengraph.png
--rw-r--r--   0        0        0    13849 2022-12-22 17:36:27.101505 lokiunimore-0.7.0/lokiunimore/web/static/rooms.png
--rw-r--r--   0        0        0    11414 2022-12-22 19:29:55.750615 lokiunimore-0.7.0/lokiunimore/web/static/s-192.png
--rw-r--r--   0        0        0    12609 2022-12-22 17:35:11.929504 lokiunimore-0.7.0/lokiunimore/web/static/spaces.png
--rw-r--r--   0        0        0     9703 2022-12-22 18:25:58.877553 lokiunimore-0.7.0/lokiunimore/web/static/thor.png
--rw-r--r--   0        0        0     2380 2022-12-22 19:27:04.461613 lokiunimore-0.7.0/lokiunimore/web/static/unimore.css
--rw-r--r--   0        0        0    15136 2022-12-22 17:54:43.661523 lokiunimore-0.7.0/lokiunimore/web/static/verify.png
--rw-r--r--   0        0        0     1941 2022-12-22 19:27:29.637613 lokiunimore-0.7.0/lokiunimore/web/templates/_base.html
--rw-r--r--   0        0        0      593 2022-09-12 08:32:11.762215 lokiunimore-0.7.0/lokiunimore/web/templates/errors/_base.html
--rw-r--r--   0        0        0      521 2022-12-22 19:33:02.285618 lokiunimore-0.7.0/lokiunimore/web/templates/errors/failed-invite.html
--rw-r--r--   0        0        0      470 2022-12-22 19:33:15.098619 lokiunimore-0.7.0/lokiunimore/web/templates/errors/no-link.html
--rw-r--r--   0        0        0      330 2022-09-12 08:33:58.481208 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-found.html
--rw-r--r--   0        0        0      645 2022-09-12 08:32:21.533214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-student.html
--rw-r--r--   0        0        0      599 2022-09-12 08:32:25.528214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-verified.html
--rw-r--r--   0        0        0      300 2022-09-12 08:32:29.441214 lokiunimore-0.7.0/lokiunimore/web/templates/errors/oidc.html
--rw-r--r--   0        0        0      418 2022-12-22 19:34:20.990620 lokiunimore-0.7.0/lokiunimore/web/templates/errors/rate-invite.html
--rw-r--r--   0        0        0     2125 2022-12-22 19:34:44.869620 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/complete.html
--rw-r--r--   0        0        0     2481 2022-12-22 19:34:59.842620 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/join.html
--rw-r--r--   0        0        0     1764 2022-12-22 19:35:47.109621 lokiunimore-0.7.0/lokiunimore/web/templates/matrix/verify.html
--rw-r--r--   0        0        0     5933 2022-12-25 04:58:24.750659 lokiunimore-0.7.0/lokiunimore/web/templates/privacy.html
--rw-r--r--   0        0        0     5336 2022-12-22 19:19:19.669605 lokiunimore-0.7.0/lokiunimore/web/templates/root.html
--rw-r--r--   0        0        0     4702 2023-05-20 16:57:00.499419 lokiunimore-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 lokiunimore-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     3428 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/config/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/config/__main__.py
+-rw-r--r--   0        0        0     6187 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/config/config.py
+-rw-r--r--   0        0        0       22 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/matrix/__init__.py
+-rw-r--r--   0        0        0      758 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/matrix/__main__.py
+-rw-r--r--   0        0        0    21685 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/matrix/client.py
+-rw-r--r--   0        0        0     3083 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/matrix/templates/messages.py
+-rw-r--r--   0        0        0       22 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/sql/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/sql/__main__.py
+-rw-r--r--   0        0        0     4905 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/sql/tables.py
+-rw-r--r--   0        0        0      348 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/utils/device_names.py
+-rw-r--r--   0        0        0      888 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/utils/logs.py
+-rw-r--r--   0        0        0       19 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/__main__.py
+-rw-r--r--   0        0        0     5511 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/app.py
+-rw-r--r--   0        0        0     1907 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/extensions/matrix_client.py
+-rw-r--r--   0        0        0    67646 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/static/favicon.ico
+-rw-r--r--   0        0        0     8288 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/static/icon.png
+-rw-r--r--   0        0        0     9408 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/static/newcode.png
+-rw-r--r--   0        0        0   151500 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/static/opengraph.png
+-rw-r--r--   0        0        0    13849 2023-05-20 17:39:33.626880 lokiunimore-0.7.1/lokiunimore/web/static/rooms.png
+-rw-r--r--   0        0        0    11414 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/static/s-192.png
+-rw-r--r--   0        0        0    12609 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/static/spaces.png
+-rw-r--r--   0        0        0     9703 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/static/thor.png
+-rw-r--r--   0        0        0     2380 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/static/unimore.css
+-rw-r--r--   0        0        0    15136 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/static/verify.png
+-rw-r--r--   0        0        0     1941 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/_base.html
+-rw-r--r--   0        0        0      593 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/_base.html
+-rw-r--r--   0        0        0      521 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/failed-invite.html
+-rw-r--r--   0        0        0      470 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/no-link.html
+-rw-r--r--   0        0        0      330 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/not-found.html
+-rw-r--r--   0        0        0      645 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/not-student.html
+-rw-r--r--   0        0        0      599 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/not-verified.html
+-rw-r--r--   0        0        0      300 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/oidc.html
+-rw-r--r--   0        0        0      418 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/errors/rate-invite.html
+-rw-r--r--   0        0        0     2125 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/matrix/complete.html
+-rw-r--r--   0        0        0     2481 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/matrix/join.html
+-rw-r--r--   0        0        0     1764 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/matrix/verify.html
+-rw-r--r--   0        0        0     5933 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/privacy.html
+-rw-r--r--   0        0        0     5336 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/lokiunimore/web/templates/root.html
+-rw-r--r--   0        0        0     4702 2023-05-20 17:39:33.630880 lokiunimore-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 lokiunimore-0.7.1/setup.py
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 lokiunimore-0.7.1/PKG-INFO
```

### Comparing `lokiunimore-0.7.0/LICENSE.txt` & `lokiunimore-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/README.md` & `lokiunimore-0.7.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Loki Bot
 
-Gatekeeper bot for the Unimore Informatica unofficial Matrix space.
+Gatekeeper bot for the Unimore Informatica unofficial Matrix space, successor to [Thor Bot](https://github.com/Steffo99/thorunimore).
 
-## Links
-
-
-
-\[ [**Website**](https://loki.steffo.eu) | [PyPI](https://pypi.org/project/lokiunimore/) \]
-
-> TIP: You may be looking for its predecessor, [Thor Bot](https://github.com/Steffo99/thorunimore).
+[![Website](https://img.shields.io/website?url=https%3A%2F%2Floki.steffo.eu%2F)](https://loki.steffo.eu/)
+ 
+[![On PyPI](https://img.shields.io/pypi/v/lokiunimore)](https://pypi.org/project/lokiunimore/)
+ 
+[![Chat](https://img.shields.io/matrix/loki-bot:ryg.one?server_fqdn=matrix.ryg.one)](https://matrix.to/#/#loki-bot:ryg.one)
 
 ![](lokiunimore/web/static/opengraph.png)
 
 ## Functionality
 
 This bot monitors a [pre-configured *public* Matrix space][config-public-space] for join events, sending a [welcome message][welcome-msg] to every new joiner.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lokiunimore-0.7.0/lokiunimore/config/config.py` & `lokiunimore-0.7.1/lokiunimore/config/config.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/matrix/__main__.py` & `lokiunimore-0.7.1/lokiunimore/matrix/__main__.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/matrix/client.py` & `lokiunimore-0.7.1/lokiunimore/matrix/client.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/matrix/templates/messages.py` & `lokiunimore-0.7.1/lokiunimore/matrix/templates/messages.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/sql/tables.py` & `lokiunimore-0.7.1/lokiunimore/sql/tables.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/utils/logs.py` & `lokiunimore-0.7.1/lokiunimore/utils/logs.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/app.py` & `lokiunimore-0.7.1/lokiunimore/web/app.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/extensions/matrix_client.py` & `lokiunimore-0.7.1/lokiunimore/web/extensions/matrix_client.py`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/favicon.ico` & `lokiunimore-0.7.1/lokiunimore/web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/icon.png` & `lokiunimore-0.7.1/lokiunimore/web/static/icon.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/newcode.png` & `lokiunimore-0.7.1/lokiunimore/web/static/newcode.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/opengraph.png` & `lokiunimore-0.7.1/lokiunimore/web/static/opengraph.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/rooms.png` & `lokiunimore-0.7.1/lokiunimore/web/static/rooms.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/s-192.png` & `lokiunimore-0.7.1/lokiunimore/web/static/s-192.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/spaces.png` & `lokiunimore-0.7.1/lokiunimore/web/static/spaces.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/thor.png` & `lokiunimore-0.7.1/lokiunimore/web/static/thor.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/unimore.css` & `lokiunimore-0.7.1/lokiunimore/web/static/unimore.css`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/static/verify.png` & `lokiunimore-0.7.1/lokiunimore/web/static/verify.png`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/_base.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/errors/_base.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/errors/_base.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/errors/failed-invite.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/errors/failed-invite.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-student.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/errors/not-student.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/errors/not-verified.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/errors/not-verified.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/complete.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/matrix/complete.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/join.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/matrix/join.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/matrix/verify.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/matrix/verify.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/privacy.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/privacy.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/lokiunimore/web/templates/root.html` & `lokiunimore-0.7.1/lokiunimore/web/templates/root.html`

 * *Files identical despite different names*

### Comparing `lokiunimore-0.7.0/pyproject.toml` & `lokiunimore-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "lokiunimore"
 
 # The version of the package.
-version = "0.7.0"
+version = "0.7.1"
 
 # A brief, one-sentence description about your project.
 description = "Matrix room gatekeeper bot for the unofficial Unimore space"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
```

### Comparing `lokiunimore-0.7.0/PKG-INFO` & `lokiunimore-0.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokiunimore
-Version: 0.7.0
+Version: 0.7.1
 Summary: Matrix room gatekeeper bot for the unofficial Unimore space
 Home-page: https://loki.steffo.eu/
 License: AGPL-3.0-or-later
 Keywords: bot,matrix,authentication,unimore,oauth2
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
@@ -27,23 +27,21 @@
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/Steffo99/lokiunimore
 Description-Content-Type: text/markdown
 
 # Loki Bot
 
-Gatekeeper bot for the Unimore Informatica unofficial Matrix space.
+Gatekeeper bot for the Unimore Informatica unofficial Matrix space, successor to [Thor Bot](https://github.com/Steffo99/thorunimore).
 
-## Links
-
-
-
-\[ [**Website**](https://loki.steffo.eu) | [PyPI](https://pypi.org/project/lokiunimore/) \]
-
-> TIP: You may be looking for its predecessor, [Thor Bot](https://github.com/Steffo99/thorunimore).
+[![Website](https://img.shields.io/website?url=https%3A%2F%2Floki.steffo.eu%2F)](https://loki.steffo.eu/)
+ 
+[![On PyPI](https://img.shields.io/pypi/v/lokiunimore)](https://pypi.org/project/lokiunimore/)
+ 
+[![Chat](https://img.shields.io/matrix/loki-bot:ryg.one?server_fqdn=matrix.ryg.one)](https://matrix.to/#/#loki-bot:ryg.one)
 
 ![](lokiunimore/web/static/opengraph.png)
 
 ## Functionality
 
 This bot monitors a [pre-configured *public* Matrix space][config-public-space] for join events, sending a [welcome message][welcome-msg] to every new joiner.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

