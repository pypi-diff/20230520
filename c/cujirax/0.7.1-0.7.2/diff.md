# Comparing `tmp/cujirax-0.7.1.tar.gz` & `tmp/cujirax-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.7.1.tar", last modified: Mon Apr 24 16:53:31 2023, max compression
+gzip compressed data, was "cujirax-0.7.2.tar", last modified: Sat May 20 15:08:32 2023, max compression
```

## Comparing `cujirax-0.7.1.tar` & `cujirax-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.1/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.1/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.1/README.md
--rw-r--r--   0        0        0    10469 2023-04-24 16:52:25.141875 cujirax-0.7.1/cujirax/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.7.1/cujirax/cucumber.py
--rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.1/cujirax/jira.py
--rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.1/cujirax/xray/__init__.py
--rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.1/cujirax/xray/graphql.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.1/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.1/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.2/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.2/README.md
+-rw-r--r--   0        0        0    10592 2023-05-20 15:08:26.246966 cujirax-0.7.2/cujirax/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.7.2/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.2/cujirax/jira.py
+-rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.2/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.2/cujirax/xray/graphql.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.2/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.2/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.2/PKG-INFO
```

### Comparing `cujirax-0.7.1/.gitignore` & `cujirax-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/LICENSE` & `cujirax-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/README.md` & `cujirax-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/__init__.py` & `cujirax-0.7.2/cujirax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
 from cujirax.cucumber import Element
 from cujirax.jira import Jirakey, JiraX, Project
 from loguru import logger
 from collections import Counter
 
 
+class DuplicateValueError(Exception):
+    """Raised when a duplicate Scenario is found."""
+    pass
+
+
 class CuJiraX:
     def __init__(self, jira_project: str, parent_testset_key: str = None, addional_identifier: str = None) -> None:
         self.jira_project = jira_project
         self.jira = JiraX(jira_project)
         
         self.testexecution = None
         self.testexecution_name = None
@@ -109,15 +114,15 @@
                 try:
                     exists, new = self._split_elements_to_exist_and_new(
                         elements=f.elements, 
                         j=self.jira, 
                         ignore_duplicate=ignore_duplicate
                     )
                 except ValueError as e:
-                    raise type(e)(f"{f.uri}: {str(e)}") from e
+                    raise DuplicateValueError(f"{str(ticket_te)}:{f.uri}:{str(e)}")
                 
                 tests = [str(n) for n in map(
                     lambda x: self._update_description_if_exist(x,self.jira), exists)]
                 root.update({
                     'existing_tests': tests,
                 })
```

### Comparing `cujirax-0.7.1/cujirax/cucumber.py` & `cujirax-0.7.2/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/jira.py` & `cujirax-0.7.2/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/xray/__init__.py` & `cujirax-0.7.2/cujirax/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/xray/graphql.py` & `cujirax-0.7.2/cujirax/xray/graphql.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/xray/import_results.py` & `cujirax-0.7.2/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/cujirax/xray/import_tests.py` & `cujirax-0.7.2/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.1/PKG-INFO` & `cujirax-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.7.1
+Version: 0.7.2
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

