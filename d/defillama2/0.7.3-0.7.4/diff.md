# Comparing `tmp/defillama2-0.7.3.tar.gz` & `tmp/defillama2-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillama2-0.7.3.tar", last modified: Mon Jan 16 09:28:36 2023, max compression
+gzip compressed data, was "defillama2-0.7.4.tar", last modified: Fri May 19 23:19:20 2023, max compression
```

## Comparing `defillama2-0.7.3.tar` & `defillama2-0.7.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.180125 defillama2-0.7.3/
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.155927 defillama2-0.7.3/.github/
--rw-r--r--   0 gmlang     (501) staff       (20)       70 2023-01-16 09:23:00.000000 defillama2-0.7.3/.github/FUNDING.yml
--rw-r--r--   0 gmlang     (501) staff       (20)       36 2022-10-05 00:39:49.000000 defillama2-0.7.3/.gitignore
--rw-r--r--   0 gmlang     (501) staff       (20)     1073 2022-10-05 00:37:39.000000 defillama2-0.7.3/LICENSE
--rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-01-16 09:28:36.179644 defillama2-0.7.3/PKG-INFO
--rw-r--r--   0 gmlang     (501) staff       (20)     4745 2023-01-16 09:23:00.000000 defillama2-0.7.3/README.md
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.156952 defillama2-0.7.3/defillama2/
--rw-r--r--   0 gmlang     (501) staff       (20)       33 2022-10-05 02:49:32.000000 defillama2-0.7.3/defillama2/__init__.py
--rw-r--r--   0 gmlang     (501) staff       (20)    48829 2023-01-16 09:21:58.000000 defillama2-0.7.3/defillama2/defillama2.py
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.160662 defillama2-0.7.3/defillama2/deprecated/
--rw-r--r--   0 gmlang     (501) staff       (20)     2580 2022-12-25 02:07:22.000000 defillama2-0.7.3/defillama2/deprecated/get_daily_open_close.py
--rw-r--r--   0 gmlang     (501) staff       (20)     3548 2022-12-25 02:07:35.000000 defillama2-0.7.3/defillama2/deprecated/get_tokens_hist_prices.py
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.159466 defillama2-0.7.3/defillama2.egg-info/
--rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-01-16 09:28:36.000000 defillama2-0.7.3/defillama2.egg-info/PKG-INFO
--rw-r--r--   0 gmlang     (501) staff       (20)      651 2023-01-16 09:28:36.000000 defillama2-0.7.3/defillama2.egg-info/SOURCES.txt
--rw-r--r--   0 gmlang     (501) staff       (20)        1 2023-01-16 09:28:36.000000 defillama2-0.7.3/defillama2.egg-info/dependency_links.txt
--rw-r--r--   0 gmlang     (501) staff       (20)       45 2023-01-16 09:28:36.000000 defillama2-0.7.3/defillama2.egg-info/requires.txt
--rw-r--r--   0 gmlang     (501) staff       (20)       11 2023-01-16 09:28:36.000000 defillama2-0.7.3/defillama2.egg-info/top_level.txt
-drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-01-16 09:28:36.176098 defillama2-0.7.3/notebooks/
--rw-r--r--   0 gmlang     (501) staff       (20)    37377 2022-12-29 06:01:51.000000 defillama2-0.7.3/notebooks/defillama_api_bridges.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    66566 2022-12-29 06:07:03.000000 defillama2-0.7.3/notebooks/defillama_api_coins.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    86058 2022-12-29 06:10:14.000000 defillama2-0.7.3/notebooks/defillama_api_fees_and_revenue.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    74996 2022-12-29 06:12:00.000000 defillama2-0.7.3/notebooks/defillama_api_stablecoins.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)  1281090 2022-12-29 06:39:00.000000 defillama2-0.7.3/notebooks/defillama_api_tvl.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)    69598 2022-12-29 06:41:14.000000 defillama2-0.7.3/notebooks/defillama_api_volumes.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)   363834 2022-12-29 06:55:51.000000 defillama2-0.7.3/notebooks/defillama_api_yields.ipynb
--rw-r--r--   0 gmlang     (501) staff       (20)       38 2023-01-16 09:28:36.180276 defillama2-0.7.3/setup.cfg
--rw-r--r--   0 gmlang     (501) staff       (20)     1080 2023-01-16 09:25:49.000000 defillama2-0.7.3/setup.py
--rw-r--r--   0 gmlang     (501) staff       (20)   305716 2022-10-05 03:53:55.000000 defillama2-0.7.3/splash.png
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.955956 defillama2-0.7.4/
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.931118 defillama2-0.7.4/.github/
+-rw-r--r--   0 gmlang     (501) staff       (20)       70 2023-01-16 09:23:00.000000 defillama2-0.7.4/.github/FUNDING.yml
+-rw-r--r--   0 gmlang     (501) staff       (20)       36 2022-10-05 00:39:49.000000 defillama2-0.7.4/.gitignore
+-rw-r--r--   0 gmlang     (501) staff       (20)     1073 2022-10-05 00:37:39.000000 defillama2-0.7.4/LICENSE
+-rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-05-19 23:19:20.955559 defillama2-0.7.4/PKG-INFO
+-rw-r--r--   0 gmlang     (501) staff       (20)     4745 2023-01-16 09:23:00.000000 defillama2-0.7.4/README.md
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.932647 defillama2-0.7.4/defillama2/
+-rw-r--r--   0 gmlang     (501) staff       (20)       33 2022-10-05 02:49:32.000000 defillama2-0.7.4/defillama2/__init__.py
+-rw-r--r--   0 gmlang     (501) staff       (20)    48782 2023-05-19 23:09:12.000000 defillama2-0.7.4/defillama2/defillama2.py
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.936743 defillama2-0.7.4/defillama2/deprecated/
+-rw-r--r--   0 gmlang     (501) staff       (20)     2580 2022-12-25 02:07:22.000000 defillama2-0.7.4/defillama2/deprecated/get_daily_open_close.py
+-rw-r--r--   0 gmlang     (501) staff       (20)     3548 2022-12-25 02:07:35.000000 defillama2-0.7.4/defillama2/deprecated/get_tokens_hist_prices.py
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.935711 defillama2-0.7.4/defillama2.egg-info/
+-rw-r--r--   0 gmlang     (501) staff       (20)     5455 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/PKG-INFO
+-rw-r--r--   0 gmlang     (501) staff       (20)      713 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/SOURCES.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)        1 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/dependency_links.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)       45 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/requires.txt
+-rw-r--r--   0 gmlang     (501) staff       (20)       11 2023-05-19 23:19:20.000000 defillama2-0.7.4/defillama2.egg-info/top_level.txt
+drwxr-xr-x   0 gmlang     (501) staff       (20)        0 2023-05-19 23:19:20.952210 defillama2-0.7.4/notebooks/
+-rw-r--r--   0 gmlang     (501) staff       (20)    37377 2022-12-29 06:01:51.000000 defillama2-0.7.4/notebooks/defillama_api_bridges.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    66566 2022-12-29 06:07:03.000000 defillama2-0.7.4/notebooks/defillama_api_coins.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    86058 2022-12-29 06:10:14.000000 defillama2-0.7.4/notebooks/defillama_api_fees_and_revenue.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    74996 2022-12-29 06:12:00.000000 defillama2-0.7.4/notebooks/defillama_api_stablecoins.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)     1443 2023-04-28 00:46:34.000000 defillama2-0.7.4/notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py
+-rw-r--r--   0 gmlang     (501) staff       (20)  1281090 2022-12-29 06:39:00.000000 defillama2-0.7.4/notebooks/defillama_api_tvl.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)    69598 2022-12-29 06:41:14.000000 defillama2-0.7.4/notebooks/defillama_api_volumes.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)   363834 2022-12-29 06:55:51.000000 defillama2-0.7.4/notebooks/defillama_api_yields.ipynb
+-rw-r--r--   0 gmlang     (501) staff       (20)       38 2023-05-19 23:19:20.956065 defillama2-0.7.4/setup.cfg
+-rw-r--r--   0 gmlang     (501) staff       (20)     1080 2023-05-19 23:10:11.000000 defillama2-0.7.4/setup.py
+-rw-r--r--   0 gmlang     (501) staff       (20)   305716 2022-10-05 03:53:55.000000 defillama2-0.7.4/splash.png
```

### Comparing `defillama2-0.7.3/LICENSE` & `defillama2-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/PKG-INFO` & `defillama2-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillama2
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python client for DefiLlama API
 Home-page: https://github.com/coindataschool/defillama2
 Author: Coin Data School
 Author-email: <coindataschool@gmail.com>
 Keywords: python 3,defillama,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama2-0.7.3/README.md` & `defillama2-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/defillama2/defillama2.py` & `defillama2-0.7.4/defillama2/defillama2.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,15 @@
         protocol : string
             Protocol name.
         
         Returns 
         -------
         float
         """
-        resp = self._get('TVL', f'/tvl/{protocol}')
-        return resp['lastHourlyRecord']
+        return self._get('TVL', f'/tvl/{protocol}')
 
     def get_chains_curr_tvl(self):
         """Get current TVL of all chains.
         
         Returns 
         -------
         data frame
@@ -145,15 +144,15 @@
         Returns 
         -------
         data frame
         """
         df = pd.DataFrame(self._get('TVL', '/protocols'))
         cols = ['name', 'symbol', 'chain', 'category', 'chains', 
                 'tvl', 'change_1d', 'change_7d', 
-                'fdv', 'mcap', 'forkedFrom']
+                'mcap', 'forkedFrom']
         df = df.loc[:, cols].rename(columns={'forkedFrom':'forked_from'})
         return df
 
     def get_protocol(self, protocol):
         """Get detailed info on a protocol and breakdowns by token and chain.
         
         Parameters
```

### Comparing `defillama2-0.7.3/defillama2/deprecated/get_daily_open_close.py` & `defillama2-0.7.4/defillama2/deprecated/get_daily_open_close.py`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/defillama2/deprecated/get_tokens_hist_prices.py` & `defillama2-0.7.4/defillama2/deprecated/get_tokens_hist_prices.py`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/defillama2.egg-info/PKG-INFO` & `defillama2-0.7.4/defillama2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillama2
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python client for DefiLlama API
 Home-page: https://github.com/coindataschool/defillama2
 Author: Coin Data School
 Author-email: <coindataschool@gmail.com>
 Keywords: python 3,defillama,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama2-0.7.3/defillama2.egg-info/SOURCES.txt` & `defillama2-0.7.4/defillama2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 defillama2.egg-info/top_level.txt
 defillama2/deprecated/get_daily_open_close.py
 defillama2/deprecated/get_tokens_hist_prices.py
 notebooks/defillama_api_bridges.ipynb
 notebooks/defillama_api_coins.ipynb
 notebooks/defillama_api_fees_and_revenue.ipynb
 notebooks/defillama_api_stablecoins.ipynb
+notebooks/defillama_api_top30_protocols_hist_tvls_by_chain.py
 notebooks/defillama_api_tvl.ipynb
 notebooks/defillama_api_volumes.ipynb
 notebooks/defillama_api_yields.ipynb
```

### Comparing `defillama2-0.7.3/notebooks/defillama_api_bridges.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_bridges.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_coins.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_coins.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_fees_and_revenue.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_fees_and_revenue.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_stablecoins.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_stablecoins.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_tvl.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_tvl.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_volumes.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_volumes.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/notebooks/defillama_api_yields.ipynb` & `defillama2-0.7.4/notebooks/defillama_api_yields.ipynb`

 * *Files identical despite different names*

### Comparing `defillama2-0.7.3/setup.py` & `defillama2-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
-VERSION = '0.7.3'
+VERSION = '0.7.4'
 
 packages = ['defillama2']
 requires = ['requests>=2.28.1', 'pandas>=1.4.4', 'numpy>=1.22.4']
 
 with open('README.md', mode='r') as f:
     readme = f.read()
```

### Comparing `defillama2-0.7.3/splash.png` & `defillama2-0.7.4/splash.png`

 * *Files identical despite different names*

