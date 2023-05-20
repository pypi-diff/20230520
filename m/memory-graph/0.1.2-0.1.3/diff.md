# Comparing `tmp/memory_graph-0.1.2.tar.gz` & `tmp/memory_graph-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.2.tar", last modified: Sat May 20 09:51:22 2023, max compression
+gzip compressed data, was "memory_graph-0.1.3.tar", last modified: Sat May 20 11:20:35 2023, max compression
```

## Comparing `memory_graph-0.1.2.tar` & `memory_graph-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 09:51:22.914925 memory_graph-0.1.2/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.2/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.2/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4600 2023-05-20 09:51:22.914925 memory_graph-0.1.2/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4025 2023-05-20 09:47:19.000000 memory_graph-0.1.2/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 09:51:22.914925 memory_graph-0.1.2/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.2/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1281 2023-05-20 09:49:47.000000 memory_graph-0.1.2/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3678 2023-05-20 07:40:48.000000 memory_graph-0.1.2/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4934 2023-05-20 07:54:16.000000 memory_graph-0.1.2/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1380 2023-05-20 07:54:31.000000 memory_graph-0.1.2/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.2/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 09:51:22.914925 memory_graph-0.1.2/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4600 2023-05-20 09:51:22.000000 memory_graph-0.1.2/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 09:51:22.000000 memory_graph-0.1.2/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 09:51:22.000000 memory_graph-0.1.2/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 09:51:22.000000 memory_graph-0.1.2/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 09:51:22.000000 memory_graph-0.1.2/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 09:51:22.914925 memory_graph-0.1.2/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 09:49:58.000000 memory_graph-0.1.2/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.3/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.3/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4666 2023-05-20 11:20:35.230037 memory_graph-0.1.3/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4091 2023-05-20 11:15:35.000000 memory_graph-0.1.3/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.3/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1281 2023-05-20 11:18:05.000000 memory_graph-0.1.3/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3688 2023-05-20 10:54:04.000000 memory_graph-0.1.3/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4986 2023-05-20 10:51:23.000000 memory_graph-0.1.3/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1380 2023-05-20 07:54:31.000000 memory_graph-0.1.3/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.3/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4666 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 11:20:35.230037 memory_graph-0.1.3/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 11:17:51.000000 memory_graph-0.1.3/setup.py
```

### Comparing `memory_graph-0.1.2/LICENSE.txt` & `memory_graph-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.2/PKG-INFO` & `memory_graph-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.1.2
+Version: 0.1.3
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -47,35 +47,38 @@
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
 ```
 import memory_graph
 
-my_list = [10, 20, 30]
+my_list = [10, 20, 10]
 
 class My_Class:
-    my_class_var = 1000 # class variable: shared by different objects
+    my_class_var = 20 # class variable: shared by different objects
     
     def __init__(self):
         self.var1 = "foo"
         self.var2 = "bar"
+        self.var3 = 20
 
 obj1 = My_Class()
 obj2 = My_Class()
 
 data=[my_list, my_list, obj1, obj2]
 
 my_list.append(data) # recursive reference
 
 memory_graph.show( data )
 ```
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example2.png)
 
-Often it is useful to show all local variables using:
+## Graph all Local Variables ##
+
+Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
 ## Install ##
 
@@ -85,15 +88,15 @@
 pip install memory-graph
 ```
 
 ## Config ##
 
 Different aspects of memory_graph can be configured.
 
-### Config visualization, graphviz_nodes ###
+### Config Visualization, graphviz_nodes ###
 
 Configure how the nodes of the graph are visualized with:
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
@@ -104,45 +107,47 @@
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config node structure, rewrite_to_node ###
+### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
   - determines if we reduce the references (to dict) in objects of classes
 - ***memory_graph.rewrite_to_node.class_variables_label*** : str
   - the label used to reference the class varibles (mappingproxy)
 
-### Config node creation, rewrite ###
+### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
   - all types rewritten to node as dictionary values (dict, mappingproxy)
 
 ### Config example ###
 
 With configuration:
 ```
-memory_graph.graphviz_nodes.layout_vertical = True                        # draw list/tuple/set/... vertically
+memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
 memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
 ```
+
 the last example looks like:
+
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
 ## Author ##
 Bas Terwijn
```

### Comparing `memory_graph-0.1.2/README.md` & `memory_graph-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,35 +30,38 @@
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
 ```
 import memory_graph
 
-my_list = [10, 20, 30]
+my_list = [10, 20, 10]
 
 class My_Class:
-    my_class_var = 1000 # class variable: shared by different objects
+    my_class_var = 20 # class variable: shared by different objects
     
     def __init__(self):
         self.var1 = "foo"
         self.var2 = "bar"
+        self.var3 = 20
 
 obj1 = My_Class()
 obj2 = My_Class()
 
 data=[my_list, my_list, obj1, obj2]
 
 my_list.append(data) # recursive reference
 
 memory_graph.show( data )
 ```
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example2.png)
 
-Often it is useful to show all local variables using:
+## Graph all Local Variables ##
+
+Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
 ## Install ##
 
@@ -68,15 +71,15 @@
 pip install memory-graph
 ```
 
 ## Config ##
 
 Different aspects of memory_graph can be configured.
 
-### Config visualization, graphviz_nodes ###
+### Config Visualization, graphviz_nodes ###
 
 Configure how the nodes of the graph are visualized with:
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
@@ -87,45 +90,47 @@
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config node structure, rewrite_to_node ###
+### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
   - determines if we reduce the references (to dict) in objects of classes
 - ***memory_graph.rewrite_to_node.class_variables_label*** : str
   - the label used to reference the class varibles (mappingproxy)
 
-### Config node creation, rewrite ###
+### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
   - all types rewritten to node as dictionary values (dict, mappingproxy)
 
 ### Config example ###
 
 With configuration:
 ```
-memory_graph.graphviz_nodes.layout_vertical = True                        # draw list/tuple/set/... vertically
+memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
 memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
 ```
+
 the last example looks like:
+
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
 ## Author ##
 Bas Terwijn
```

### Comparing `memory_graph-0.1.2/memory_graph/Node.py` & `memory_graph-0.1.3/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.2/memory_graph/__init__.py` & `memory_graph-0.1.3/memory_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import graphviz_nodes
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = 'Bas Terwijn'
 
 def create_graph(data):
     all_nodes=rewrite_to_node.rewrite_data(data)
     return graphviz_nodes.create_graph(all_nodes)
 
 def show(data,block=True):
```

### Comparing `memory_graph-0.1.2/memory_graph/graphviz_nodes.py` & `memory_graph-0.1.3/memory_graph/graphviz_nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from types import NoneType
 from types import MappingProxyType
 import graphviz
 
 from memory_graph import Node
 from memory_graph import rewrite
 
-layout_vertical=False
+layout_vertical=True
 type_category_to_color_map={
     "NoneType":"gray", "type":"lime", "bool":"pink", "int":"green", "float":"yellow", "str":"cyan", # fundamental types
-    "tuple":"orange", "list":"brown1", "set":"darkolivegreen1", "frozenset":"darkolivegreen3", "dict":"blue", "mappingproxy":"blue3", "class":"purple" # containers
+    "tuple":"orange", "list":"brown1", "set":"darkolivegreen1", "frozenset":"darkolivegreen3", "dict":"royalblue1", "mappingproxy":"royalblue3", "class":"orchid" # containers
 }
 uncategorized_color="red"
 
 def type_category_to_color(type_catergory):
     if type_catergory in type_category_to_color_map:
         return type_category_to_color_map[type_catergory]
     return uncategorized_color
```

### Comparing `memory_graph-0.1.2/memory_graph/rewrite.py` & `memory_graph-0.1.3/memory_graph/rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from types import NoneType
 from types import MappingProxyType
 
 # the types of the values we rewrite
 
-singular_types={NoneType, bool, int, float, complex, str, range, bytes, type}
+singular_types={NoneType, bool, int, float, complex, str, range, bytes} # not 'type' to prevent issues with reading class methods
 linear_types={tuple, list, set, frozenset, bytearray}
 dict_types={dict, MappingProxyType}
 known_types=singular_types | linear_types | dict_types
 
 def is_singular_type(value):
     return type(value) in singular_types
```

### Comparing `memory_graph-0.1.2/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.3/memory_graph/rewrite_to_node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.2/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.3/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.2/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.3/memory_graph.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.1.2
+Version: 0.1.3
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -47,35 +47,38 @@
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
 ```
 import memory_graph
 
-my_list = [10, 20, 30]
+my_list = [10, 20, 10]
 
 class My_Class:
-    my_class_var = 1000 # class variable: shared by different objects
+    my_class_var = 20 # class variable: shared by different objects
     
     def __init__(self):
         self.var1 = "foo"
         self.var2 = "bar"
+        self.var3 = 20
 
 obj1 = My_Class()
 obj2 = My_Class()
 
 data=[my_list, my_list, obj1, obj2]
 
 my_list.append(data) # recursive reference
 
 memory_graph.show( data )
 ```
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example2.png)
 
-Often it is useful to show all local variables using:
+## Graph all Local Variables ##
+
+Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
 ## Install ##
 
@@ -85,15 +88,15 @@
 pip install memory-graph
 ```
 
 ## Config ##
 
 Different aspects of memory_graph can be configured.
 
-### Config visualization, graphviz_nodes ###
+### Config Visualization, graphviz_nodes ###
 
 Configure how the nodes of the graph are visualized with:
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
@@ -104,45 +107,47 @@
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config node structure, rewrite_to_node ###
+### Config Node Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
   - the types we copy to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
   - determines if we reduce the references (to dict) in objects of classes
 - ***memory_graph.rewrite_to_node.class_variables_label*** : str
   - the label used to reference the class varibles (mappingproxy)
 
-### Config node creation, rewrite ###
+### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
   - all types rewritten to node as dictionary values (dict, mappingproxy)
 
 ### Config example ###
 
 With configuration:
 ```
-memory_graph.graphviz_nodes.layout_vertical = True                        # draw list/tuple/set/... vertically
+memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' types
 memory_graph.rewrite_to_node.reduce_reference_types.remove(int)           # draw references to 'int' types
 ```
+
 the last example looks like:
+
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
 ## Author ##
 Bas Terwijn
```

### Comparing `memory_graph-0.1.2/setup.py` & `memory_graph-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.2',
+    version = '0.1.3',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

