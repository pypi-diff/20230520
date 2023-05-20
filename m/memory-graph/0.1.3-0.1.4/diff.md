# Comparing `tmp/memory_graph-0.1.3.tar.gz` & `tmp/memory_graph-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.3.tar", last modified: Sat May 20 11:20:35 2023, max compression
+gzip compressed data, was "memory_graph-0.1.4.tar", last modified: Sat May 20 15:48:58 2023, max compression
```

## Comparing `memory_graph-0.1.3.tar` & `memory_graph-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.3/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.3/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4666 2023-05-20 11:20:35.230037 memory_graph-0.1.3/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4091 2023-05-20 11:15:35.000000 memory_graph-0.1.3/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.3/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1281 2023-05-20 11:18:05.000000 memory_graph-0.1.3/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3688 2023-05-20 10:54:04.000000 memory_graph-0.1.3/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4986 2023-05-20 10:51:23.000000 memory_graph-0.1.3/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1380 2023-05-20 07:54:31.000000 memory_graph-0.1.3/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.3/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 11:20:35.230037 memory_graph-0.1.3/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4666 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 11:20:35.000000 memory_graph-0.1.3/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 11:20:35.230037 memory_graph-0.1.3/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 11:17:51.000000 memory_graph-0.1.3/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 15:48:58.164579 memory_graph-0.1.4/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.4/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.4/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4797 2023-05-20 15:48:58.164579 memory_graph-0.1.4/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4222 2023-05-20 15:39:02.000000 memory_graph-0.1.4/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 15:48:58.164579 memory_graph-0.1.4/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.4/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1283 2023-05-20 15:48:12.000000 memory_graph-0.1.4/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3688 2023-05-20 10:54:04.000000 memory_graph-0.1.4/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4986 2023-05-20 10:51:23.000000 memory_graph-0.1.4/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1380 2023-05-20 07:54:31.000000 memory_graph-0.1.4/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.4/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 15:48:58.164579 memory_graph-0.1.4/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4797 2023-05-20 15:48:58.000000 memory_graph-0.1.4/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 15:48:58.000000 memory_graph-0.1.4/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 15:48:58.000000 memory_graph-0.1.4/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 15:48:58.000000 memory_graph-0.1.4/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 15:48:58.000000 memory_graph-0.1.4/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 15:48:58.164579 memory_graph-0.1.4/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 15:47:14.000000 memory_graph-0.1.4/setup.py
```

### Comparing `memory_graph-0.1.3/LICENSE.txt` & `memory_graph-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/PKG-INFO` & `memory_graph-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.1.3
+Version: 0.1.4
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,29 +22,28 @@
 
 Just call `memory_graph.show(your_data)`, an example:
 
 ```
 import memory_graph
 
 data = [ (1, 2), [3, 4], {5:'five', 6:'six'} ]
-memory_graph.show( data )
+memory_graph.show( data, block=True )
 ```
 
 This shows the graph with the starting point of your 'data' drawn
 using thick lines, the program blocks until the ENTER key is pressed.
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example1.png)
 
 If `show()` doesn't work well on your system (the PDF viewer
 integration is platform specific) use `render()` to output the graph
-in the format of your choosing. Use `block=False` to turn off
-blocking.
+in the format of your choosing and open it yourself.
 
 ```
-memory_graph.render( data, "my_graph.png", block=False )
+memory_graph.render( data, "my_graph.png", block=True )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -76,14 +75,20 @@
 
 Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
+Also useful to set as 'watch' during a debug session:
+
+```
+memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+```
+
 ## Install ##
 
 Install using pip:
 
 ```
 pip install memory-graph
 ```
```

### Comparing `memory_graph-0.1.3/README.md` & `memory_graph-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 
 Just call `memory_graph.show(your_data)`, an example:
 
 ```
 import memory_graph
 
 data = [ (1, 2), [3, 4], {5:'five', 6:'six'} ]
-memory_graph.show( data )
+memory_graph.show( data, block=True )
 ```
 
 This shows the graph with the starting point of your 'data' drawn
 using thick lines, the program blocks until the ENTER key is pressed.
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example1.png)
 
 If `show()` doesn't work well on your system (the PDF viewer
 integration is platform specific) use `render()` to output the graph
-in the format of your choosing. Use `block=False` to turn off
-blocking.
+in the format of your choosing and open it yourself.
 
 ```
-memory_graph.render( data, "my_graph.png", block=False )
+memory_graph.render( data, "my_graph.png", block=True )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -59,14 +58,20 @@
 
 Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
+Also useful to set as 'watch' during a debug session:
+
+```
+memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+```
+
 ## Install ##
 
 Install using pip:
 
 ```
 pip install memory-graph
 ```
```

### Comparing `memory_graph-0.1.3/memory_graph/Node.py` & `memory_graph-0.1.4/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/memory_graph/__init__.py` & `memory_graph-0.1.4/memory_graph/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import graphviz_nodes
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = 'Bas Terwijn'
 
 def create_graph(data):
     all_nodes=rewrite_to_node.rewrite_data(data)
     return graphviz_nodes.create_graph(all_nodes)
 
-def show(data,block=True):
+def show(data,block=False):
     graph=create_graph(data)
     graph.view()
     if block:
         input(f"showing '{graph.filename}', press <ENTER> to continue...")
 
-def render(data,output_filename=None,block=True):
+def render(data,output_filename=None,block=False):
     graph=create_graph(data)
     if output_filename:
         graph.render(outfile=output_filename)
         if block:
             input(f"rendering '{output_filename}', press <ENTER> to continue...")
     else:
         graph.render()
```

### Comparing `memory_graph-0.1.3/memory_graph/graphviz_nodes.py` & `memory_graph-0.1.4/memory_graph/graphviz_nodes.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/memory_graph/rewrite.py` & `memory_graph-0.1.4/memory_graph/rewrite.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.4/memory_graph/rewrite_to_node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.4/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.3/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.4/memory_graph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.1.3
+Version: 0.1.4
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,29 +22,28 @@
 
 Just call `memory_graph.show(your_data)`, an example:
 
 ```
 import memory_graph
 
 data = [ (1, 2), [3, 4], {5:'five', 6:'six'} ]
-memory_graph.show( data )
+memory_graph.show( data, block=True )
 ```
 
 This shows the graph with the starting point of your 'data' drawn
 using thick lines, the program blocks until the ENTER key is pressed.
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example1.png)
 
 If `show()` doesn't work well on your system (the PDF viewer
 integration is platform specific) use `render()` to output the graph
-in the format of your choosing. Use `block=False` to turn off
-blocking.
+in the format of your choosing and open it yourself.
 
 ```
-memory_graph.render( data, "my_graph.png", block=False )
+memory_graph.render( data, "my_graph.png", block=True )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -76,14 +75,20 @@
 
 Often it is useful to graph all the local variables using:
 
 ```
 memory_graph.show( memory_graph.filter(locals()) )
 ```
 
+Also useful to set as 'watch' during a debug session:
+
+```
+memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+```
+
 ## Install ##
 
 Install using pip:
 
 ```
 pip install memory-graph
 ```
```

### Comparing `memory_graph-0.1.3/setup.py` & `memory_graph-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.3',
+    version = '0.1.4',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

