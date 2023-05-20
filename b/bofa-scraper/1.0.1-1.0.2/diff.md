# Comparing `tmp/bofa_scraper-1.0.1.tar.gz` & `tmp/bofa_scraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofa_scraper-1.0.1.tar", last modified: Sun Sep 11 03:24:23 2022, max compression
+gzip compressed data, was "bofa_scraper-1.0.2.tar", last modified: Sat May 20 04:30:39 2023, max compression
```

## Comparing `bofa_scraper-1.0.1.tar` & `bofa_scraper-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 soupsu    (1000) soupsu    (1000)        0 2022-09-11 03:24:23.001031 bofa_scraper-1.0.1/
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)    35148 2022-09-09 23:02:51.000000 bofa_scraper-1.0.1/LICENSE
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     2719 2022-09-11 03:24:23.001031 bofa_scraper-1.0.1/PKG-INFO
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     2351 2022-09-11 03:09:36.000000 bofa_scraper-1.0.1/README.md
-drwxr-xr-x   0 soupsu    (1000) soupsu    (1000)        0 2022-09-11 03:24:22.991031 bofa_scraper-1.0.1/bofa_scraper/
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     2335 2022-09-11 03:07:54.000000 bofa_scraper-1.0.1/bofa_scraper/__init__.py
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     1040 2022-09-11 03:04:32.000000 bofa_scraper-1.0.1/bofa_scraper/account.py
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     2200 2022-09-11 03:05:15.000000 bofa_scraper-1.0.1/bofa_scraper/scrape_session.py
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)      263 2022-09-11 01:29:05.000000 bofa_scraper-1.0.1/bofa_scraper/util.py
-drwxr-xr-x   0 soupsu    (1000) soupsu    (1000)        0 2022-09-11 03:24:23.001031 bofa_scraper-1.0.1/bofa_scraper.egg-info/
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)     2719 2022-09-11 03:24:22.000000 bofa_scraper-1.0.1/bofa_scraper.egg-info/PKG-INFO
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)      312 2022-09-11 03:24:22.000000 bofa_scraper-1.0.1/bofa_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)        1 2022-09-11 03:24:22.000000 bofa_scraper-1.0.1/bofa_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)        9 2022-09-11 03:24:22.000000 bofa_scraper-1.0.1/bofa_scraper.egg-info/requires.txt
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)       13 2022-09-11 03:24:22.000000 bofa_scraper-1.0.1/bofa_scraper.egg-info/top_level.txt
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)      416 2022-09-11 03:24:08.000000 bofa_scraper-1.0.1/pyproject.toml
--rw-r--r--   0 soupsu    (1000) soupsu    (1000)       38 2022-09-11 03:24:23.001031 bofa_scraper-1.0.1/setup.cfg
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-05-20 04:30:39.196675 bofa_scraper-1.0.2/
+-rw-r--r--   0 felix     (1000) felix     (1000)    35148 2023-05-20 04:05:51.000000 bofa_scraper-1.0.2/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     2719 2023-05-20 04:30:39.196675 bofa_scraper-1.0.2/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     2351 2023-05-20 04:05:51.000000 bofa_scraper-1.0.2/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-05-20 04:30:39.196675 bofa_scraper-1.0.2/bofa_scraper/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2356 2023-05-20 04:26:04.000000 bofa_scraper-1.0.2/bofa_scraper/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1040 2023-05-20 04:05:51.000000 bofa_scraper-1.0.2/bofa_scraper/account.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2200 2023-05-20 04:05:51.000000 bofa_scraper-1.0.2/bofa_scraper/scrape_session.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      263 2023-05-20 04:05:51.000000 bofa_scraper-1.0.2/bofa_scraper/util.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-05-20 04:30:39.196675 bofa_scraper-1.0.2/bofa_scraper.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2719 2023-05-20 04:30:39.000000 bofa_scraper-1.0.2/bofa_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      312 2023-05-20 04:30:39.000000 bofa_scraper-1.0.2/bofa_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-05-20 04:30:39.000000 bofa_scraper-1.0.2/bofa_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        9 2023-05-20 04:30:39.000000 bofa_scraper-1.0.2/bofa_scraper.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       13 2023-05-20 04:30:39.000000 bofa_scraper-1.0.2/bofa_scraper.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      416 2023-05-20 04:28:27.000000 bofa_scraper-1.0.2/pyproject.toml
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-05-20 04:30:39.196675 bofa_scraper-1.0.2/setup.cfg
```

### Comparing `bofa_scraper-1.0.1/LICENSE` & `bofa_scraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bofa_scraper-1.0.1/PKG-INFO` & `bofa_scraper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofa_scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple Python web-scraper to get personal transaction data from BofA account.
 Author-email: Wllew4 <willjanelle2@gmail.com>
 License: GNU General Public License v3 (GPLv3) (GPL3)
 Project-URL: Homepage, https://github.com/Wllew4/bofa_scraper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bofa_scraper-1.0.1/README.md` & `bofa_scraper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bofa_scraper-1.0.1/bofa_scraper/__init__.py` & `bofa_scraper-1.0.2/bofa_scraper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 		Timeout.timeout()
 
 		# 2fa
 		if self.driver.current_url == "https://secure.bankofamerica.com/login/sign-in/signOnSuccessRedirect.go":
 			Log.log('2fa required')
 			self.driver.find_element(By.ID, "btnARContinue").click()
 			print("input 2fa code: ")
+			Timeout.timeout()
 			self.driver.find_element(By.CLASS_NAME, "authcode").send_keys(input())
 			self.driver.find_element(By.ID, "yes-recognize").click()
 			self.driver.find_element(By.ID, "continue-auth-number").click()
 			Timeout.timeout()
 
 		if self.driver.current_url.startswith('https://secure.bankofamerica.com/myaccounts/'):
 			Log.log('Sign in success!')
```

### Comparing `bofa_scraper-1.0.1/bofa_scraper/account.py` & `bofa_scraper-1.0.2/bofa_scraper/account.py`

 * *Files identical despite different names*

### Comparing `bofa_scraper-1.0.1/bofa_scraper/scrape_session.py` & `bofa_scraper-1.0.2/bofa_scraper/scrape_session.py`

 * *Files identical despite different names*

### Comparing `bofa_scraper-1.0.1/bofa_scraper.egg-info/PKG-INFO` & `bofa_scraper-1.0.2/bofa_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofa-scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple Python web-scraper to get personal transaction data from BofA account.
 Author-email: Wllew4 <willjanelle2@gmail.com>
 License: GNU General Public License v3 (GPLv3) (GPL3)
 Project-URL: Homepage, https://github.com/Wllew4/bofa_scraper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

