# Comparing `tmp/spothinta-0.1.0.tar.gz` & `tmp/spothinta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spothinta-0.1.0.tar", max compression
+gzip compressed data, was "spothinta-0.1.1.tar", max compression
```

## Comparing `spothinta-0.1.0.tar` & `spothinta-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-18 18:50:45.683146 spothinta-0.1.0/LICENSE
--rw-r--r--   0        0        0     5123 2023-05-18 18:50:45.687147 spothinta-0.1.0/README.md
--rw-r--r--   0        0        0     3639 2023-05-18 18:50:59.811289 spothinta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      363 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/__init__.py
--rw-r--r--   0        0        0      399 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/const.py
--rw-r--r--   0        0        0      303 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/exceptions.py
--rw-r--r--   0        0        0     5844 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/models.py
--rw-r--r--   0        0        0        0 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/py.typed
--rw-r--r--   0        0        0     4348 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/spothinta.py
--rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 spothinta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-20 18:21:48.935418 spothinta-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5123 2023-05-20 18:21:48.935418 spothinta-0.1.1/README.md
+-rw-r--r--   0        0        0     3639 2023-05-20 18:22:12.371571 spothinta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/const.py
+-rw-r--r--   0        0        0      303 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/exceptions.py
+-rw-r--r--   0        0        0     5844 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/models.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/py.typed
+-rw-r--r--   0        0        0     4348 2023-05-20 18:21:48.939418 spothinta-0.1.1/spothinta/spothinta.py
+-rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 spothinta-0.1.1/PKG-INFO
```

### Comparing `spothinta-0.1.0/LICENSE` & `spothinta-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spothinta-0.1.0/README.md` & `spothinta-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 ## About
 
 A Python package with which you can retrieve the energy market prices from [spot-hinta.fi][spothinta].
 
-Based on the [easyEnergy][easyenergy] library by [@klassnicolaas][klassnicolaas].
+Based on the [easyEnergy][easyenergy] library by [@klaasnicolaas][klaasnicolaas].
 
 ## Installation
 
 ```bash
 pip install spothinta
 ```
 
@@ -123,15 +123,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 <!-- MARKDOWN LINKS & IMAGES -->
 [easyenergy]: https://github.com/klaasnicolaas/python-easyenergy
 [spothinta]: https://spot-hinta.fi/
 [spothinta-api-docs]: https://api.spot-hinta.fi/swagger/ui#/(JSON)%20Price%20today%20and%20tomorrow%20(if%20tomorrow%20prices%20exist)/TodayAndDayForward
-[klassnicolaas]: https://github.com/klaasnicolaas
+[klaasnicolaas]: https://github.com/klaasnicolaas
 
 [build-shield]: https://github.com/slovdahl/python-spothinta/actions/workflows/tests.yaml/badge.svg
 [build-url]: https://github.com/slovdahl/python-spothinta/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/slovdahl/python-spothinta/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/slovdahl/python-spothinta/actions/workflows/codeql.yaml
 [codecov-shield]: https://codecov.io/gh/slovdahl/python-spothinta/branch/main/graph/badge.svg?token=RYhiDUamT6
 [codecov-url]: https://codecov.io/gh/slovdahl/python-spothinta
```

### Comparing `spothinta-0.1.0/pyproject.toml` & `spothinta-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spothinta"
-version = "0.1.0"
+version = "0.1.1"
 description = "Asynchronous Python client providing energy prices from spot-hinta.fi"
 authors = [
   "Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>",
   "Klaas Schoute <hello@student-techlife.com>"
 ]
 maintainers = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 license = "MIT"
```

### Comparing `spothinta-0.1.0/spothinta/models.py` & `spothinta-0.1.1/spothinta/models.py`

 * *Files identical despite different names*

### Comparing `spothinta-0.1.0/spothinta/spothinta.py` & `spothinta-0.1.1/spothinta/spothinta.py`

 * *Files identical despite different names*

### Comparing `spothinta-0.1.0/PKG-INFO` & `spothinta-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spothinta
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asynchronous Python client providing energy prices from spot-hinta.fi
 License: MIT
 Keywords: energy,spothinta,prices,api,async,client
 Author: Sebastian Lövdahl
 Author-email: sebastian.lovdahl@hibox.fi
 Maintainer: Sebastian Lövdahl
 Maintainer-email: sebastian.lovdahl@hibox.fi
@@ -13,18 +13,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Description-Content-Type: text/markdown
 
 # Spot-Hinta.fi Python client
 
@@ -36,15 +32,15 @@
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
 ## About
 
 A Python package with which you can retrieve the energy market prices from [spot-hinta.fi][spothinta].
 
-Based on the [easyEnergy][easyenergy] library by [@klassnicolaas][klassnicolaas].
+Based on the [easyEnergy][easyenergy] library by [@klaasnicolaas][klaasnicolaas].
 
 ## Installation
 
 ```bash
 pip install spothinta
 ```
 
@@ -151,15 +147,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 <!-- MARKDOWN LINKS & IMAGES -->
 [easyenergy]: https://github.com/klaasnicolaas/python-easyenergy
 [spothinta]: https://spot-hinta.fi/
 [spothinta-api-docs]: https://api.spot-hinta.fi/swagger/ui#/(JSON)%20Price%20today%20and%20tomorrow%20(if%20tomorrow%20prices%20exist)/TodayAndDayForward
-[klassnicolaas]: https://github.com/klaasnicolaas
+[klaasnicolaas]: https://github.com/klaasnicolaas
 
 [build-shield]: https://github.com/slovdahl/python-spothinta/actions/workflows/tests.yaml/badge.svg
 [build-url]: https://github.com/slovdahl/python-spothinta/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/slovdahl/python-spothinta/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/slovdahl/python-spothinta/actions/workflows/codeql.yaml
 [codecov-shield]: https://codecov.io/gh/slovdahl/python-spothinta/branch/main/graph/badge.svg?token=RYhiDUamT6
 [codecov-url]: https://codecov.io/gh/slovdahl/python-spothinta
```

