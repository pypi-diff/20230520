# Comparing `tmp/mosek_license_server-0.0.6.tar.gz` & `tmp/mosek_license_server-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.0.6.tar", max compression
+gzip compressed data, was "mosek_license_server-0.0.7.tar", max compression
```

## Comparing `mosek_license_server-0.0.6.tar` & `mosek_license_server-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-20 07:21:20.347461 mosek_license_server-0.0.6/mosek_license/__init__.py
--rw-r--r--   0        0        0      449 2023-05-20 07:21:20.347461 mosek_license_server-0.0.6/mosek_license/license.py
--rw-r--r--   0        0        0      409 2023-05-20 07:21:37.383456 mosek_license_server-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1162 2023-05-20 07:21:20.347461 mosek_license_server-0.0.6/readme.md
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 mosek_license_server-0.0.6/setup.py
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 mosek_license_server-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-20 07:23:44.477858 mosek_license_server-0.0.7/mosek_license/__init__.py
+-rw-r--r--   0        0        0      449 2023-05-20 07:23:44.477858 mosek_license_server-0.0.7/mosek_license/license.py
+-rw-r--r--   0        0        0      409 2023-05-20 07:24:00.318150 mosek_license_server-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1161 2023-05-20 07:23:44.477858 mosek_license_server-0.0.7/readme.md
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 mosek_license_server-0.0.7/setup.py
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 mosek_license_server-0.0.7/PKG-INFO
```

### Comparing `mosek_license_server-0.0.6/readme.md` & `mosek_license_server-0.0.7/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -43,11 +43,11 @@
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
 license.upsert()
 
-# only know import mosek
+# only now import mosek
 import mosek
 ```
```

### Comparing `mosek_license_server-0.0.6/setup.py` & `mosek_license_server-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['urllib3']
 
 setup_kwargs = {
     'name': 'mosek-license-server',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Expose a mosek license via a nginx server',
-    'long_description': "# Mosek License Server\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\n## License server\n\n### Copy your license file into folder \n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via http://localhost:8080\n\nAs an alternative you can run the script\n\n```bash\n./license_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only know import mosek\nimport mosek\n```\n\n",
+    'long_description': "# Mosek License Server\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\n## License server\n\n### Copy your license file into folder \n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via http://localhost:8080\n\nAs an alternative you can run the script\n\n```bash\n./license_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only now import mosek\nimport mosek\n```\n\n",
     'author': 'Thomas Schmelzer',
     'author_email': 'thomas.schmelzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mosek_license_server-0.0.6/PKG-INFO` & `mosek_license_server-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.0.6
+Version: 0.0.7
 Summary: Expose a mosek license via a nginx server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -59,12 +59,12 @@
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
 license.upsert()
 
-# only know import mosek
+# only now import mosek
 import mosek
 ```
```

