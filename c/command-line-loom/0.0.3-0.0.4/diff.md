# Comparing `tmp/command_line_loom-0.0.3.tar.gz` & `tmp/command_line_loom-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_line_loom-0.0.3.tar", max compression
+gzip compressed data, was "command_line_loom-0.0.4.tar", max compression
```

## Comparing `command_line_loom-0.0.3.tar` & `command_line_loom-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.3/LICENSE
--rw-r--r--   0        0        0     4466 2023-05-18 18:24:52.435855 command_line_loom-0.0.3/README.md
--rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.3/cll/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/__main__.py
--rw-r--r--   0        0        0     7645 2023-05-19 20:37:53.421731 command_line_loom-0.0.3/cll/app.py
--rw-r--r--   0        0        0     7096 2023-05-19 20:33:17.487868 command_line_loom-0.0.3/cll/config.py
--rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/data_structs/__init__.py
--rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.3/cll/data_structs/data_structs.py
--rw-r--r--   0        0        0     9817 2023-05-19 20:24:08.516125 command_line_loom-0.0.3/cll/data_structs/loom_index.py
--rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.3/cll/data_structs/node.py
--rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/io.py
--rw-r--r--   0        0        0     2292 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/store.py
--rw-r--r--   0        0        0     7963 2023-05-19 20:35:18.534930 command_line_loom-0.0.3/cll/templater.py
--rw-r--r--   0        0        0    12804 2023-05-19 20:48:25.868085 command_line_loom-0.0.3/cll/tree.py
--rw-r--r--   0        0        0     1052 2023-05-19 20:49:52.943636 command_line_loom-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4466 2023-05-19 21:06:05.942638 command_line_loom-0.0.4/README.md
+-rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.4/cll/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/__main__.py
+-rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.4/cll/app.py
+-rw-r--r--   0        0        0     7358 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/config.py
+-rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/data_structs/__init__.py
+-rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.4/cll/data_structs/data_structs.py
+-rw-r--r--   0        0        0     9817 2023-05-19 21:14:40.199467 command_line_loom-0.0.4/cll/data_structs/loom_index.py
+-rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.4/cll/data_structs/node.py
+-rwxr-xr-x   0        0        0     4133 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/encoder.py
+-rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/io.py
+-rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.4/cll/store.py
+-rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.4/cll/templater.py
+-rw-r--r--   0        0        0    15809 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/tree.py
+-rw-r--r--   0        0        0     1052 2023-05-20 12:28:48.275313 command_line_loom-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.4/PKG-INFO
```

### Comparing `command_line_loom-0.0.3/LICENSE` & `command_line_loom-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/README.md` & `command_line_loom-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/__main__.py` & `command_line_loom-0.0.4/cll/__main__.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/app.py` & `command_line_loom-0.0.4/cll/app.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/config.py` & `command_line_loom-0.0.4/cll/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import datetime
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional
 
 import tttp
@@ -14,26 +15,36 @@
 from typing_extensions import Annotated
 
 from typer_shell import make_typer_shell
 
 file_path = Path("/tmp/cll/")
 file_path.mkdir(parents=True, exist_ok=True)
 
-# log_path = file_path / "logs"
-# log_path.mkdir(parents=True, exist_ok=True)
+log_path = file_path / "logs"
+log_path.mkdir(parents=True, exist_ok=True)
 
 timestamp = datetime.datetime.now().replace(microsecond=0).isoformat()
-# logfile = log_path / f"{timestamp}.log"
+logfile = log_path / f"{timestamp}.log"
 
-logging.basicConfig(
-    # filename=logfile,
-    format="%(asctime)s - %(levelname)s - %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-    level=logging.INFO,
-)
+DEBUG = os.environ.get("DEBUG", False)
+
+if DEBUG:
+    print("DEBUG MODE")
+    logging.basicConfig(
+        format="%(asctime)s - %(levelname)s - %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+        level=logging.INFO,
+    )
+else:
+    logging.basicConfig(
+        filename=logfile,
+        format="%(asctime)s - %(levelname)s - %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+        level=logging.INFO,
+    )
 logger = logging.getLogger()
 
 
 @dataclass
 class Config:
     model_tokens = {
         "gpt-4": 4096 - 8,
```

### Comparing `command_line_loom-0.0.3/cll/data_structs/data_structs.py` & `command_line_loom-0.0.4/cll/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/data_structs/loom_index.py` & `command_line_loom-0.0.4/cll/data_structs/loom_index.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/data_structs/node.py` & `command_line_loom-0.0.4/cll/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/io.py` & `command_line_loom-0.0.4/cll/io.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/store.py` & `command_line_loom-0.0.4/cll/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,13 +66,14 @@
 def file(
     ctx: Context,
     default_file: Annotated[Optional[str], Argument()] = None,
     toggle: bool = False,
     list: bool = False,
     dump: bool = False,
 ):
+    """Manages the chat file. If you want to create an entirely new tree, do it here."""
     config = ctx.obj.config
     config.check_file(toggle, default_file, config)
     if list:
         Store(config=config).list_files()
     if dump:
         print(Store(config=config).dump())
```

### Comparing `command_line_loom-0.0.3/cll/templater.py` & `command_line_loom-0.0.4/cll/templater.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.3/cll/tree.py` & `command_line_loom-0.0.4/cll/tree.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import iterfzf
+import binascii
 from copy import deepcopy
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
+import iterfzf
 import click
 from cll.data_structs import LoomIndex
 from rich import print
 from rich.console import Console
 from rich.panel import Panel
 from typer import Argument, Context, get_app_dir
 from typing_extensions import Annotated
 
 from typer_shell import make_typer_shell
+from .encoder import Encoder
 
 
 @dataclass
 class DummyTree:
     params: Optional[dict] = None
     prompt: str = ""
 
@@ -32,14 +34,16 @@
 
 @dataclass
 class Tree:
     file: Optional[str] = None
     index: Optional[LoomIndex] = None
     params: Optional[dict] = None
     name: Optional[str] = None
+    encoder: Encoder = Encoder(Encoder.none)
+    decoder: Encoder = Encoder(Encoder.none)
 
     def __post_init__(self):
         self.file = Path(self.file)
 
         if self.file and self.file.exists():
             self.index = LoomIndex.load_from_disk(str(self.file))
             return
@@ -50,15 +54,25 @@
     def prompt_context(self):
         path = self.index.path_formatted
         prompt = self.index.context + "\n" + path
         return prompt
 
     @property
     def prompt(self):
-        return self.index.path_formatted
+        if self.encoder.callback == Encoder.none:
+            return self.index.path_formatted
+        return self._prompt
+
+    @property
+    def _prompt(self):
+        prompt = ""
+        for node in self.index.index_struct.path_nodes:
+            prompt += node.prefix
+            prompt += self.encoder(node.text)
+        return prompt
 
     def input(self, node):
         self.extend(node, save=True)
 
     def output(self, node):
         self.extend(node, save=True)
 
@@ -79,22 +93,16 @@
         return len(self.index.index_struct.all_nodes)
 
 
 def path_with_current(ctx):
     index = ctx.obj.tree.index
     Console().clear()
 
-    name = ctx.command.name
-    if name not in ctx.obj.params_groups:
-        if ctx.parent:
-            name = ctx.parent.command.name
-    if name not in ctx.obj.params_groups:
-        print("Cant find params!")
-    else:
-        params = ctx.obj.params_groups[name]['params']
+    params = get_params(ctx)
+    if params:
         index.index_struct.path_neighborhood = params["path_neighborhood"]
         index.index_struct.head_neighborhood = params["head_neighborhood"]
 
     index.index_struct.legend()
     print(index.index_struct._get_repr())
     path = index.index_struct.path
     if not len(path):
@@ -104,25 +112,57 @@
         path_str += "".join([str(node) for node in path[:-1]])
     path_str += "[bold red]"
     path_str += str(path[-1])
     path_str += "[/bold red]"
     print(Panel.fit(path_str, title="Prompt", border_style="bold magenta"))
 
 
+def get_params(ctx):
+    name = ctx.command.name
+    if name not in ctx.obj.params_groups:
+        if ctx.parent:
+            name = ctx.parent.command.name
+    if name not in ctx.obj.params_groups:
+        print("Cant find params!")
+    else:
+        params = ctx.obj.params_groups[name]['params']
+        return params
+
+
+def set_encoder(ctx, string=None):
+    params = get_params(ctx)
+    if not string and params:
+        string = params.get("encoder", "none")
+    if not string:
+        string = "none"
+    ctx.obj.tree.encoder = Encoder.get_encoder(string)
+    ctx.obj.tree.decoder = Encoder.get_decoder(string)
+    if Encoder._get_encoder(string) == Encoder.none:
+        string = "none"
+    params = get_params(ctx)
+    if params:
+        params["encoder"] = string
+    print(params)
+    path_with_current(ctx)
+
+
 cli = make_typer_shell(
     prompt="🌲: ",
-    launch=path_with_current,
+    launch=set_encoder,
     params={"path_neighborhood": 3, "head_neighborhood": 10},
     params_path=Path(get_app_dir("cll")) / "tree.yaml"
 )
 
 
-@cli.command()
+@cli.command(hidden=True)
 def default(ctx: Context, line: str):
     """Default command"""
+    if len(line) < 20:
+        print("Ill assume you didn't mean to send that. If you do, use 'send X'. (Below 20 chars.)")
+        return
     ctx.invoke(send, ctx=ctx, msg=line.split(" "))
 
 
 @cli.command(hidden=True)
 def h(ctx: Context, count: int = 1):
     "Move to left sibling"
     for _ in range(count):
@@ -162,14 +202,57 @@
     "View may be rotated 90 degrees."
     for _ in range(count):
         ctx.obj.tree.index.step(direction)
     path_with_current(ctx)
 
 
 @cli.command()
+@cli.command(name="en", hidden=True)
+@cli.command(name="encoding", hidden=True)
+def encoder(ctx: Context, encoder: str):
+    '(en) Set the encoder to use. Text will be encoded and decoded before being sent.\n'
+    'Available encoders:\n'
+    '\t"none": no encoding\n'
+    '\t"base64": base64 encoding\n'
+    '\t"rot13": rot13 encoding\n'
+    '\t"caesar X": caesar encoding, rot by X (rot13 == "ceaser 13")\n'
+    set_encoder(ctx, encoder)
+
+
+@cli.command()
+@cli.command(name="re", hidden=True)
+def reencode(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
+    "(re) Reencode the current node."
+    if not index:
+        index = ctx.obj.tree.index.path[-1].index
+    index = int(index)
+
+    node = ctx.obj.tree.index.index_struct.all_nodes[index]
+    node.text = ctx.obj.tree.encoder(node.text)
+    ctx.obj.tree.index.index_struct.all_nodes[index] = node
+    ctx.obj.tree.save()
+    path_with_current(ctx)
+
+
+@cli.command()
+@cli.command(name="de", hidden=True)
+def redecode(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
+    "(de) Reencode the current node backwards."
+    if not index:
+        index = ctx.obj.tree.index.path[-1].index
+    index = int(index)
+
+    node = ctx.obj.tree.index.index_struct.all_nodes[index]
+    node.text = ctx.obj.tree.decoder(node.text)
+    ctx.obj.tree.index.index_struct.all_nodes[index] = node
+    ctx.obj.tree.save()
+    path_with_current(ctx)
+
+
+@cli.command()
 @cli.command(name="d", hidden=True)
 @cli.command(name="p", hidden=True)
 def display(
     ctx: Context,
     type: Annotated[Optional[str], Argument()] = "p",
     index: Annotated[Optional[str], Argument()] = None,
 ):
@@ -249,43 +332,54 @@
 ):
     """(s) Adds a new message to the chain and sends it all."""
     _append(ctx, msg)
     _send(ctx)
 
 
 def _send(ctx):
+    # Encoding happens in the tree
     prompt = ctx.obj.tree.prompt
-    prompt = ctx.obj.templater.prompt(prompt)
-
     params = deepcopy(ctx.obj.tree.params)
+
+    # Then templating (so template stays in english)
+    prompt = ctx.obj.templater.prompt(prompt)
     params["prompt"] = prompt
+
     responses, choice = ctx.obj.simple_gen(ctx.obj.config, params)
     if len(responses) == 1:
-        response = ctx.obj.tree.index._create_node(responses[0])
-        response = ctx.obj.templater.out(response)
-        ctx.obj.tree.extend(response)
+        callback = ctx.obj.tree.extend
     else:
-        for response in responses.values():
-            response = ctx.obj.tree.index._create_node(response)
-            response = ctx.obj.templater.out(response)
-            ctx.obj.tree.insert(response)
+        callback = ctx.obj.tree.insert
+
+    for response in responses.values():
+        # Decode the response first
+        try:
+            response = ctx.obj.tree.decoder(response)
+        except (binascii.Error, UnicodeDecodeError):
+            # Probably the response wasn't encoded?
+            pass
+        response = ctx.obj.tree.index._create_node(response)
+        # Then template
+        response = ctx.obj.templater.out(response)
+        callback(response)
 
     if choice is not None:
         index = len(responses) - choice
         node_indexes = list(ctx.obj.tree.index.index_struct.all_nodes.keys())
         ctx.obj.tree.index.checkout(node_indexes[-index])
     ctx.obj.tree.save()
 
     path_with_current(ctx)
 
 
 @cli.command()
 @cli.command(name="pu", hidden=True)
+@cli.command(name="r", hidden=True)
 def push(ctx: Context):
-    """(pu) sends the tree with no new message."""
+    """(pu, r) sends the tree with no new message."""
     _send(ctx)
 
 
 @cli.command()
 @cli.command(name="n", hidden=True)
 def new(ctx: Context):
     """n[ew] starts a new chain (a new root)"""
@@ -352,15 +446,18 @@
     print(output)
 
 
 @cli.command()
 @cli.command(name="prompt", hidden=True)
 def edit_prompt(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
     """(prompt) Export the full prompt to an editor for saving."""
+    prev_encoder = ctx.obj.tree.encoder
+    ctx.obj.tree.encoder = Encoder.get_encoder("none")
     input = str(ctx.obj.tree.prompt)
+    ctx.obj.tree.encoder = prev_encoder
     click.edit(input)
 
 
 # @cli.command()
 # @cli.command(name="del", hidden=True)
 # def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None):
 #     "(del) delete some nodes (space separated) (last one by default)"
```

### Comparing `command_line_loom-0.0.3/pyproject.toml` & `command_line_loom-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "command-line-loom"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 homepage = "https://github.com/fergusfettes/command-line-loom"
 readme = "README.md"
 packages = [{include = "cll"}]
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 turbo-text-transformer-prompts = "^0.1.10"
 python-dotenv = "^1.0.0"
 click-shell = "^2.1"
 typer = "^0.9.0"
 rich = "^13.3.5"
 iterfzf = "^0.5.0.20.0"
 llama-index = "^0.6.8"
-typer-shell = "^0.1.3"
+typer-shell = "^0.1.4"
 networkx = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.11"
 ipython = "^8.10.0"
 memory-profiler = "^0.61.0"
```

### Comparing `command_line_loom-0.0.3/PKG-INFO` & `command_line_loom-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command-line-loom
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Home-page: https://github.com/fergusfettes/command-line-loom
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: tiktoken (>=0.3.0,<0.4.0)
 Requires-Dist: turbo-text-transformer-prompts (>=0.1.10,<0.2.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: typer-shell (>=0.1.3,<0.2.0)
+Requires-Dist: typer-shell (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Command Line Loom
 
 Command Line Loom is a Python command-line tool for generating text using OpenAI's GPT-3 and other models. It includes a modular model system that allows for easy integration of new models and customization of existing ones.
 
 Includes templates, look in the [Turbo Text Transformer Prompts](https://github.com/fergusfettes/turbo-text-transformer-prompts) repository for more documentation and to find a list of the templates!
```

