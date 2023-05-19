# Comparing `tmp/jupyter_ai_magics-0.7.1.tar.gz` & `tmp/jupyter_ai_magics-0.7.2.tar.gz`

## Comparing `jupyter_ai_magics-0.7.1.tar` & `jupyter_ai_magics-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/setup.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    14961 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/README.md
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/setup.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/README.md
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.2/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.7.1/package.json` & `jupyter_ai_magics-0.7.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.7.2'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.7.1"
+    "version": "0.7.2"
 }
```

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/embedding_providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return ({'text/plain': self.text}, self.metadata)
 
 
 class Base64Image:
     def __init__(self, mimeData, metadata):
         mimeDataParts = mimeData.split(',')
         self.data = base64.b64decode(mimeDataParts[1]);
-        self.mimeType = mimeDataParts[0].removesuffix(';base64')
+        self.mimeType = re.sub(r';base64$', '', mimeDataParts[0])
         self.metadata = metadata
 
     def _repr_mimebundle_(self, include=None, exclude=None):
         return ({self.mimeType: self.data}, self.metadata)
 
 
 DISPLAYS_BY_FORMAT = {
@@ -142,15 +142,16 @@
 
         if (len(Provider.models) == 1 and Provider.models[0] == "*"):
             return PROVIDER_NO_MODELS
 
         for model_id in Provider.models:
             output += f", `{provider_id}:{model_id}`";
         
-        return output.removeprefix(', ')
+        # Remove initial comma
+        return re.sub(r'^, ', '', output)
     
     # Is the required environment variable set?
     def _ai_env_status_for_provider_markdown(self, provider_id):
         na_message = 'Not applicable. | <abbr title="Not applicable">N/A</abbr> '
 
         if (provider_id not in self.providers or
             self.providers[provider_id].auth_strategy == None):
@@ -363,15 +364,15 @@
         }
 
         # if the user wants code, add another cell with the output.
         if args.format == 'code':
             # Strip a leading language indicator and trailing triple-backticks
             lang_indicator = r'^```[a-zA-Z0-9]*\n'
             output = re.sub(lang_indicator, '', output)
-            output = output.removesuffix('\n```')
+            output = re.sub(r'\n```$', '', output)
             new_cell_payload = dict(
                 source='set_next_input',
                 text=output,
                 replace=False,
             )
             ip.payload_manager.write_payload(new_cell_payload)
             return HTML('AI generated code inserted below &#11015;&#65039;', metadata=md);
```

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-0.7.2/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/.gitignore` & `jupyter_ai_magics-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/LICENSE` & `jupyter_ai_magics-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/pyproject.toml` & `jupyter_ai_magics-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.1/PKG-INFO` & `jupyter_ai_magics-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.7.1
+Version: 0.7.2
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

