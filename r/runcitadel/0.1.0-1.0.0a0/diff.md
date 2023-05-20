# Comparing `tmp/runcitadel-0.1.0.tar.gz` & `tmp/runcitadel-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runcitadel-0.1.0.tar", max compression
+gzip compressed data, was "runcitadel-1.0.0a0.tar", max compression
```

## Comparing `runcitadel-0.1.0.tar` & `runcitadel-1.0.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1077 2023-03-09 12:04:21.106208 runcitadel-0.1.0/LICENSE
--rw-r--r--   0        0        0      846 2023-03-15 08:26:50.113260 runcitadel-0.1.0/README.md
--rw-r--r--   0        0        0      480 2023-03-09 12:04:21.106208 runcitadel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-03-09 12:04:21.106208 runcitadel-0.1.0/src/runcitadel/__init__.py
--rw-r--r--   0        0        0    11785 2023-03-09 13:33:21.528747 runcitadel-0.1.0/src/runcitadel/runcitadel.py
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 runcitadel-0.1.0/setup.py
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 runcitadel-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-15 09:37:56.646433 runcitadel-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0      920 2023-03-15 11:53:00.789948 runcitadel-1.0.0a0/README.md
+-rw-r--r--   0        0        0      482 2023-05-20 11:27:46.410583 runcitadel-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-03-15 09:37:56.646433 runcitadel-1.0.0a0/src/runcitadel/__init__.py
+-rw-r--r--   0        0        0    12218 2023-05-20 11:18:40.040663 runcitadel-1.0.0a0/src/runcitadel/runcitadel.py
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 runcitadel-1.0.0a0/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 runcitadel-1.0.0a0/PKG-INFO
```

### Comparing `runcitadel-0.1.0/LICENSE` & `runcitadel-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `runcitadel-0.1.0/README.md` & `runcitadel-1.0.0a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,7 +20,9 @@
 ## License
 
 `runcitadel` was created by Miles van der Lely. It is licensed under the terms of the MIT license.
 
 ## Credits
 
 `runcitadel` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+
+Developed in the Visualisation Lab at the University of Amsterdam (UvA).
```

### Comparing `runcitadel-0.1.0/src/runcitadel/runcitadel.py` & `runcitadel-1.0.0a0/src/runcitadel/runcitadel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import websockets
 import ssl
 import pathlib
 import json
 from jsonschema import validate
 from jsonschema import exceptions
 import jsonschema
@@ -226,31 +227,31 @@
 def process_response(connection: websockets.WebSocketClientProtocol, response,
                      simulatefun):
     try:
         jsonObj = json.loads(response)
 
         params = {}
 
-        for param in jsonObj['data']['params']:
+        for param in jsonObj['payload']['params']:
             if (param['type'] == 'integer'):
                 params[param['attribute']] = int(param['value'])
             elif (param['type'] == 'string'):
                 params[param['attribute']] = str(param['value'])
             elif (param['type'] == 'float'):
                 params[param['attribute']] = float(param['value'])
             elif (param['type'] == 'boolean'):
                 params[param['attribute']] = bool(param['value'])
 
-        fun = types.FunctionType(simulatefun.__code__, {})
+        # fun = types.FunctionType(simulatefun.__code__, {})
 
-        res = fun(connection, jsonObj['data']['nodes'],
-                  jsonObj['data']['edges'], params)
+        res = simulatefun(connection, jsonObj['payload']['nodes'],
+                  jsonObj['payload']['edges'], params, jsonObj['payload']['globals'])
 
         params = [res[2][param['attribute']]
-                  for param in jsonObj['data']['params']]
+                  for param in jsonObj['payload']['params']]
 
         return res
     except Exception as e:
         print(f'Error! {e}')
 
 
 def filter_globals(fun):
@@ -291,18 +292,19 @@
     if (len(title) == 0):
         raise ValueError("Title must be at least 1 character")
 
     # Check if startParams is valid.
     validate_params_schema(startParams)
 
     # Filter globals
-    fun = types.FunctionType(simulatefun.__code__, filter_globals(simulatefun),
+    fun = types.FunctionType(simulatefun.__code__, simulatefun.__globals__,
                              simulatefun.__name__, simulatefun.__defaults__,
                              simulatefun.__closure__)
 
+
     uri = f"wss://{url}:{int(port)}?sid={sid}&key={key}"
 
     print(f"Connecting to wss://{url}:{port}")
 
     validator = jsonschema.Validator
 
     try:
@@ -318,33 +320,42 @@
         context = externalContext
 
     async with(websockets.connect(uri, max_size=2 ** 25, ssl=context)) as websocket:
         print("Connected")
 
         await websocket.send(json.dumps({
             'sessionID': sid,
+            'senderType': 'simulator',
+            'senderID': key,
+            'type': 'registerSimulator',
             'messageSource': 'simulator',
-            'messageType': 'set',
-            'dataType': 'register',
-            'apiKey': key,
-            'data': json.dumps(startParams),
-            'validator': has_schema,
-            'title': title,
+            'receiverType': 'server',
+            'receiverID': 'server',
+            'payload': {
+                'apikey': key,
+                'params': json.dumps(startParams),
+                'validator': has_schema,
+                'title': title,
+            }
         }))
 
         while (1):
             response = await websocket.recv()
 
             result = process_response(websocket, response, fun)
 
             await websocket.send(json.dumps({
                 'sessionID': sid,
-                'messageSource': 'simulator',
-                'messageType': 'set',
-                'dataType': 'data',
-                'apiKey': key,
-                'params': {
+                'senderType': 'simulator',
+                'type': 'simulatorResponse',
+                'senderID': key,
+                'receiverType': 'server',
+                'receiverID': 'server',
+                'timestamp': datetime.datetime.now().timestamp(),
+                'payload': {
+                    'apiKey': key,
                     'nodes': result[0],
                     'edges': result[1],
-                    'params': result[2]
+                    'params': result[2],
+                    'globals': result[3],
                 },
             }))
```

### Comparing `runcitadel-0.1.0/setup.py` & `runcitadel-1.0.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0', 'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'runcitadel',
-    'version': '0.1.0',
+    'version': '1.0.0a0',
     'description': 'A package for developing and running citadel simulations.',
-    'long_description': '# runcitadel\n\nA package for developing and running citadel simulations.\n\n## Installation\n\n```bash\n$ pip install runcitadel\n```\n\n## Usage\n\n`runcitadel` can be used to connect a local simulation to a citadel session to perform\ninteractive computation on graphs. For usage examples, see the examples notebook in /docs/.\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`runcitadel` was created by Miles van der Lely. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`runcitadel` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
+    'long_description': '# runcitadel\n\nA package for developing and running citadel simulations.\n\n## Installation\n\n```bash\n$ pip install runcitadel\n```\n\n## Usage\n\n`runcitadel` can be used to connect a local simulation to a citadel session to perform\ninteractive computation on graphs. For usage examples, see the examples notebook in /docs/.\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`runcitadel` was created by Miles van der Lely. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`runcitadel` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n\nDeveloped in the Visualisation Lab at the University of Amsterdam (UvA).\n',
     'author': 'Miles van der Lely',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `runcitadel-0.1.0/PKG-INFO` & `runcitadel-1.0.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runcitadel
-Version: 0.1.0
+Version: 1.0.0a0
 Summary: A package for developing and running citadel simulations.
 License: MIT
 Author: Miles van der Lely
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -37,7 +37,9 @@
 
 `runcitadel` was created by Miles van der Lely. It is licensed under the terms of the MIT license.
 
 ## Credits
 
 `runcitadel` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
 
+Developed in the Visualisation Lab at the University of Amsterdam (UvA).
+
```

