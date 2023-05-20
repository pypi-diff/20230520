# Comparing `tmp/memory_graph-0.1.5.tar.gz` & `tmp/memory_graph-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.5.tar", last modified: Sat May 20 18:04:11 2023, max compression
+gzip compressed data, was "memory_graph-0.1.6.tar", last modified: Sat May 20 19:00:01 2023, max compression
```

## Comparing `memory_graph-0.1.5.tar` & `memory_graph-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 18:04:11.950559 memory_graph-0.1.5/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.5/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.5/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4930 2023-05-20 18:04:11.950559 memory_graph-0.1.5/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4355 2023-05-20 17:53:20.000000 memory_graph-0.1.5/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 18:04:11.946559 memory_graph-0.1.5/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.5/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1226 2023-05-20 18:01:19.000000 memory_graph-0.1.5/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3696 2023-05-20 17:04:40.000000 memory_graph-0.1.5/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4468 2023-05-20 17:58:47.000000 memory_graph-0.1.5/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1142 2023-05-20 17:02:48.000000 memory_graph-0.1.5/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.5/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 18:04:11.950559 memory_graph-0.1.5/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4930 2023-05-20 18:04:11.000000 memory_graph-0.1.5/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 18:04:11.000000 memory_graph-0.1.5/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 18:04:11.000000 memory_graph-0.1.5/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 18:04:11.000000 memory_graph-0.1.5/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 18:04:11.000000 memory_graph-0.1.5/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 18:04:11.950559 memory_graph-0.1.5/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 18:01:06.000000 memory_graph-0.1.5/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.6/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.6/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-20 19:00:01.019402 memory_graph-0.1.6/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4366 2023-05-20 18:13:48.000000 memory_graph-0.1.6/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.6/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1190 2023-05-20 18:58:23.000000 memory_graph-0.1.6/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3696 2023-05-20 17:04:40.000000 memory_graph-0.1.6/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4498 2023-05-20 18:49:23.000000 memory_graph-0.1.6/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1142 2023-05-20 17:02:48.000000 memory_graph-0.1.6/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.6/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 19:00:01.019402 memory_graph-0.1.6/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 18:58:32.000000 memory_graph-0.1.6/setup.py
```

### Comparing `memory_graph-0.1.5/LICENSE.txt` & `memory_graph-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.5/PKG-INFO` & `memory_graph-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.1.5
+Version: 0.1.6
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -120,15 +120,15 @@
 ### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict) for classes
+  - determines if we reduce the references (to dict/mappingproxy) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
@@ -142,16 +142,16 @@
   - determines if we ignore dunder keys ('`__example__`') in mappingproxy
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
-memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
-memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
+memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
+memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' type
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
```

### Comparing `memory_graph-0.1.5/README.md` & `memory_graph-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 ### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict) for classes
+  - determines if we reduce the references (to dict/mappingproxy) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
@@ -125,16 +125,16 @@
   - determines if we ignore dunder keys ('`__example__`') in mappingproxy
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
-memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
-memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
+memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
+memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' type
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
```

### Comparing `memory_graph-0.1.5/memory_graph/Node.py` & `memory_graph-0.1.6/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.5/memory_graph/__init__.py` & `memory_graph-0.1.6/memory_graph/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import graphviz_nodes
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __author__ = 'Bas Terwijn'
 
 def create_graph(data):
     all_nodes=rewrite_to_node.rewrite_data(data)
     return graphviz_nodes.create_graph(all_nodes)
 
 def show(data,block=False):
@@ -28,10 +28,10 @@
             input(f"rendering '{graph.filename}', press <ENTER> to continue...")
 
 def filter(dictionary):
     filtered_dict={}
     for key in dictionary:
         value=dictionary[key]
         if type(key)==str and not rewrite.is_dunder_name(key) and not key in {'memory_graph'}:                
-            if rewrite.is_known_type(value) or rewrite.is_type_with_dict(value):
+            if rewrite.is_known_type(value):
                 filtered_dict[key]=value
     return filtered_dict
```

### Comparing `memory_graph-0.1.5/memory_graph/graphviz_nodes.py` & `memory_graph-0.1.6/memory_graph/graphviz_nodes.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.5/memory_graph/rewrite.py` & `memory_graph-0.1.6/memory_graph/rewrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 singular_types={NoneType, bool, int, float, complex, str, range, bytes}
 linear_types={tuple, list, set, frozenset, bytearray}
 dict_types={dict}
 mappingproxy_types={MappingProxyType}
 mappingproxy_ignore_dunder_keys=True
 
-known_types=singular_types | linear_types | dict_types | mappingproxy_types
+known_types=singular_types | linear_types | dict_types | mappingproxy_types | {type} # add 'type' for classes and class variables
 
 def is_singular_type(value):
     return type(value) in singular_types
 
 def is_linear_type(value):
     return type(value) in linear_types
 
@@ -49,15 +49,15 @@
 
 # just some helper functions
 
 def type_name(value):
     return get_name_attribute(type(value))
 
 def is_dunder_name(name):
-    return name.startswith('__') and name.endswith('__')
+    return name.startswith('__')
 
 def has_dict_attribute(value):
     return hasattr(value,"__dict__")
 
 def get_dict_attribute(value):
     return getattr(value,"__dict__")
```

### Comparing `memory_graph-0.1.5/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.6/memory_graph/rewrite_to_node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.5/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.6/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.5/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.6/memory_graph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.1.5
+Version: 0.1.6
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -120,15 +120,15 @@
 ### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict) for classes
+  - determines if we reduce the references (to dict/mappingproxy) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
@@ -142,16 +142,16 @@
   - determines if we ignore dunder keys ('`__example__`') in mappingproxy
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
-memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
-memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
+memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
+memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' type
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
```

### Comparing `memory_graph-0.1.5/setup.py` & `memory_graph-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.5',
+    version = '0.1.6',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

