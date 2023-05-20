# Comparing `tmp/chainy-0.1.0.dev3.tar.gz` & `tmp/chainy-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainy-0.1.0.dev3.tar", last modified: Fri May 19 23:23:07 2023, max compression
+gzip compressed data, was "chainy-0.1.0.dev4.tar", last modified: Sat May 20 01:16:02 2023, max compression
```

## Comparing `chainy-0.1.0.dev3.tar` & `chainy-0.1.0.dev4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.427887 chainy-0.1.0.dev3/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 chainy-0.1.0.dev3/LICENSE
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2413 2023-05-19 23:23:07.427677 chainy-0.1.0.dev3/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1826 2023-05-19 23:22:27.000000 chainy-0.1.0.dev3/README.md
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-19 23:23:07.427952 chainy-0.1.0.dev3/setup.cfg
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      934 2023-05-19 23:23:03.000000 chainy-0.1.0.dev3/setup.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.425075 chainy-0.1.0.dev3/src/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.426267 chainy-0.1.0.dev3/src/chainy/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 22:02:43.000000 chainy-0.1.0.dev3/src/chainy/__init__.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      543 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/config.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      376 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/llm.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     3089 2023-05-19 22:30:45.000000 chainy-0.1.0.dev3/src/chainy/model.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 23:23:07.427370 chainy-0.1.0.dev3/src/chainy.egg-info/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2413 2023-05-19 23:23:06.000000 chainy-0.1.0.dev3/src/chainy.egg-info/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      277 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/SOURCES.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/dependency_links.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       12 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/requires.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        7 2023-05-19 23:23:07.000000 chainy-0.1.0.dev3/src/chainy.egg-info/top_level.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-20 01:16:02.527412 chainy-0.1.0.dev4/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 chainy-0.1.0.dev4/LICENSE
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     3120 2023-05-20 01:16:02.527215 chainy-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2533 2023-05-20 00:32:45.000000 chainy-0.1.0.dev4/README.md
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-20 01:16:02.527486 chainy-0.1.0.dev4/setup.cfg
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      934 2023-05-20 01:15:44.000000 chainy-0.1.0.dev4/setup.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-20 01:16:02.524873 chainy-0.1.0.dev4/src/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-20 01:16:02.526049 chainy-0.1.0.dev4/src/chainy/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-19 22:02:43.000000 chainy-0.1.0.dev4/src/chainy/__init__.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      572 2023-05-19 23:33:32.000000 chainy-0.1.0.dev4/src/chainy/config.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      376 2023-05-19 22:30:45.000000 chainy-0.1.0.dev4/src/chainy/llm.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     3270 2023-05-20 01:13:04.000000 chainy-0.1.0.dev4/src/chainy/model.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-20 01:16:02.526955 chainy-0.1.0.dev4/src/chainy.egg-info/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     3120 2023-05-20 01:16:02.000000 chainy-0.1.0.dev4/src/chainy.egg-info/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      277 2023-05-20 01:16:02.000000 chainy-0.1.0.dev4/src/chainy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-20 01:16:02.000000 chainy-0.1.0.dev4/src/chainy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       12 2023-05-20 01:16:02.000000 chainy-0.1.0.dev4/src/chainy.egg-info/requires.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        7 2023-05-20 01:16:02.000000 chainy-0.1.0.dev4/src/chainy.egg-info/top_level.txt
```

### Comparing `chainy-0.1.0.dev3/LICENSE` & `chainy-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `chainy-0.1.0.dev3/PKG-INFO` & `chainy-0.1.0.dev4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainy
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Declarative prompt chaining
 Home-page: https://github.com/FyZyX/chainy
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -32,60 +32,80 @@
 pip install chainy
 ```
 
 You can find the package repository [here](https://pypi.org/project/chainy/).
 
 ## Usage
 
+### Configuration
+
 Chainy uses YAML configuration files to define chains of prompts.
 Here's an example of what these configuration files look like:
 
 ```yaml
 inputs:
   - input_1
   - input_2
 prompts:
   prompt_1:
+    model: my_model
     template: tmpl01.md
     substitute:
       var_1: input_1
       var_2: input_2
   prompt_2:
+    model: my_model
     template: tmpl02.md
     substitute:
       res_1: prompt_1
 ```
 
 In this example, `prompt_1` and `prompt_2` are the prompts to be run.
 Each prompt includes a template file and a dictionary of variables to be substituted into the template.
 The dependencies between prompts are defined in the substitute section: `prompt_2` depends on `prompt_1`.
 
-To run a chain, call the `Chain.start()` method with the required input values:
-
-```python
-import pathlib
-import chainy.config
-
-chain_path = pathlib.Path("chains/example-1.yml")
-chain = chainy.config.parse_config(chain_path)
-chain.start("hey", "bud")
-```
-
 ### Expected Directory Structure
 
 ```
 |- yourproject/
 |--- prompts/
 |----- tmpl01.md
 |----- tmpl02.md
 |--- chains/
 |----- example-1.yml
 |--- entrypoint.py
 ```
 
+### Bring Your Own Model (BYOM)
+
+Each prompt must specify the alias of the model that will be used to generate the response.
+Models must be added to a chain with `Chain.add_model(name, model)` before the chain is started.
+
+Models are user defined classes that adhere to the `LanguageModelProtocol` or `ChatModelProtocol`,
+which can be found in the [`llm`](src/chainy/llm.py) module.
+Essentially, the model needs to expose the appropriate `generate()` method, then `chainy` will take it from there.
+
+### Running a Chain
+
+To run a chain, call the `Chain.start()` method with the required input values:
+
+```python
+from chainy.model import Chain
+
+# STEP 1: Load your chain from configuration
+chain = Chain.from_config("chains/example-1.yml")
+
+# STEP 2: Add your model(s)
+model = ...  # instantiate your model here!
+chain.add_model("my_model", model)
+
+# STEP 3: Start the chain
+chain.start("hey", "bud")
+```
+
 ## Testing
 
 Tests are located in the `tests/` directory. To run them, use your preferred test runner.
 
 ## Contributing
 
 We welcome contributions! Please open an issue or submit a pull request if you have something to add.
```

### Comparing `chainy-0.1.0.dev3/setup.py` & `chainy-0.1.0.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name="chainy",
-    version="0.1.0-dev3",
+    version="0.1.0-dev4",
     description="Declarative prompt chaining",
     author="Lucas Lofaro",
     author_email="lucasmlofaro@gmail.com",
     url="https://github.com/FyZyX/chainy",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
```

### Comparing `chainy-0.1.0.dev3/src/chainy/config.py` & `chainy-0.1.0.dev4/src/chainy/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pathlib
 
 import yaml
 
 from . import model
 
 
-def parse_config(path: pathlib.Path) -> model.Chain:
+def parse_chain_config(path: pathlib.Path) -> model.Chain:
     with open(path, "r") as file:
         chain: dict = yaml.safe_load(file)
     name = path.name.removesuffix(".yml").removesuffix(".yaml")
     inputs = chain.pop("inputs")
-    prompts = {name: model.Prompt(
-        model=prompt["model"],
-        template_path=prompt["template"],
-        variables=prompt["substitute"],
-    )
-               for name, prompt in chain.pop("prompts").items()}
+    prompts = {
+        name: model.Prompt(
+            model=prompt["model"],
+            template_path=prompt["template"],
+            variables=prompt["substitute"],
+        )
+        for name, prompt in chain.pop("prompts").items()
+    }
     return model.Chain(name, inputs, prompts)
```

### Comparing `chainy-0.1.0.dev3/src/chainy/model.py` & `chainy-0.1.0.dev4/src/chainy/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 import asyncio
 import pathlib
 import string
 from typing import TypeAlias, Generator
 
-from . import llm
+from . import llm, config
 
 
 class Prompt:
     _default_path = pathlib.Path("prompts")
 
     def __init__(self, model: str, template_path: str, variables: dict[str, str]):
         self._model = model
-        self._template = self._load(template_path)
+        self._template_path = template_path
         self._variables = variables
 
     def _load(self, filename):
         path = self._default_path / filename
         if not path.exists():
             return ""
         with open(path) as file:
             return file.read()
 
     def model(self) -> str:
         return self._model
 
+    def template(self):
+        return string.Template(self._load(self._template_path))
+
     def dependencies(self):
-        return self._variables.values()
+        return set(self._variables.values())
 
     def substitute(self, inputs, outputs):
-        template = string.Template(self._template)
-        variables = {name: inputs.get(key) or outputs.get(key)
-                     for name, key in self._variables.items()}
-        return template.substitute(variables)
+        return self.template().substitute({
+            name: inputs.get(key) or outputs.get(key)
+            for name, key in self._variables.items()
+        })
 
 
 DependencyGraph: TypeAlias = dict[str, set[str]]
 
 
 class Chain:
-    def __init__(self, name, inputs: list[str], prompts: dict[str, Prompt]):
+    def __init__(self, name: str, inputs: list[str], prompts: dict[str, Prompt]):
         self._name = name
         self._inputs = inputs
         self._prompts = prompts
         self._outputs = {}
         self._graph: DependencyGraph = {}
         self._models: dict[str, llm.LargeLanguageModel] = {}
 
+    @classmethod
+    def from_config(cls, path: pathlib.Path | str) -> "Chain":
+        return config.parse_chain_config(pathlib.Path(path))
+
     def _build_dependency_graph(self):
         self._graph = {prompt: set() for prompt in self._prompts}
         for name, prompt in self._prompts.items():
             for var in prompt.dependencies():
                 is_prompt = var in self._prompts
                 is_self = var == name
                 if is_self or not is_prompt:
```

### Comparing `chainy-0.1.0.dev3/src/chainy.egg-info/PKG-INFO` & `chainy-0.1.0.dev4/src/chainy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainy
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Declarative prompt chaining
 Home-page: https://github.com/FyZyX/chainy
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -32,60 +32,80 @@
 pip install chainy
 ```
 
 You can find the package repository [here](https://pypi.org/project/chainy/).
 
 ## Usage
 
+### Configuration
+
 Chainy uses YAML configuration files to define chains of prompts.
 Here's an example of what these configuration files look like:
 
 ```yaml
 inputs:
   - input_1
   - input_2
 prompts:
   prompt_1:
+    model: my_model
     template: tmpl01.md
     substitute:
       var_1: input_1
       var_2: input_2
   prompt_2:
+    model: my_model
     template: tmpl02.md
     substitute:
       res_1: prompt_1
 ```
 
 In this example, `prompt_1` and `prompt_2` are the prompts to be run.
 Each prompt includes a template file and a dictionary of variables to be substituted into the template.
 The dependencies between prompts are defined in the substitute section: `prompt_2` depends on `prompt_1`.
 
-To run a chain, call the `Chain.start()` method with the required input values:
-
-```python
-import pathlib
-import chainy.config
-
-chain_path = pathlib.Path("chains/example-1.yml")
-chain = chainy.config.parse_config(chain_path)
-chain.start("hey", "bud")
-```
-
 ### Expected Directory Structure
 
 ```
 |- yourproject/
 |--- prompts/
 |----- tmpl01.md
 |----- tmpl02.md
 |--- chains/
 |----- example-1.yml
 |--- entrypoint.py
 ```
 
+### Bring Your Own Model (BYOM)
+
+Each prompt must specify the alias of the model that will be used to generate the response.
+Models must be added to a chain with `Chain.add_model(name, model)` before the chain is started.
+
+Models are user defined classes that adhere to the `LanguageModelProtocol` or `ChatModelProtocol`,
+which can be found in the [`llm`](src/chainy/llm.py) module.
+Essentially, the model needs to expose the appropriate `generate()` method, then `chainy` will take it from there.
+
+### Running a Chain
+
+To run a chain, call the `Chain.start()` method with the required input values:
+
+```python
+from chainy.model import Chain
+
+# STEP 1: Load your chain from configuration
+chain = Chain.from_config("chains/example-1.yml")
+
+# STEP 2: Add your model(s)
+model = ...  # instantiate your model here!
+chain.add_model("my_model", model)
+
+# STEP 3: Start the chain
+chain.start("hey", "bud")
+```
+
 ## Testing
 
 Tests are located in the `tests/` directory. To run them, use your preferred test runner.
 
 ## Contributing
 
 We welcome contributions! Please open an issue or submit a pull request if you have something to add.
```

