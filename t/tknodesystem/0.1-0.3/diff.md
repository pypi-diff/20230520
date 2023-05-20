# Comparing `tmp/tknodesystem-0.1.tar.gz` & `tmp/tknodesystem-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tknodesystem-0.1.tar", last modified: Wed May 17 15:36:23 2023, max compression
+gzip compressed data, was "tknodesystem-0.3.tar", last modified: Sat May 20 07:42:12 2023, max compression
```

## Comparing `tknodesystem-0.1.tar` & `tknodesystem-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:36:23.560198 tknodesystem-0.1/
--rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.1/LICENSE
--rw-rw-rw-   0        0        0     2346 2023-05-17 15:36:23.561197 tknodesystem-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1794 2023-05-17 15:31:17.000000 tknodesystem-0.1/README.md
--rw-rw-rw-   0        0        0      570 2023-05-17 15:36:23.563198 tknodesystem-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-17 15:35:21.000000 tknodesystem-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:36:23.473131 tknodesystem-0.1/tknodesystem/
--rw-rw-rw-   0        0        0      278 2023-05-17 06:15:17.000000 tknodesystem-0.1/tknodesystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:36:23.558198 tknodesystem-0.1/tknodesystem/grid_images/
--rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.1/tknodesystem/grid_images/grid_dot.png
--rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.1/tknodesystem/grid_images/grid_lines.png
--rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.1/tknodesystem/grid_images/no_grid.png
--rw-rw-rw-   0        0        0     4693 2023-05-17 05:59:53.000000 tknodesystem-0.1/tknodesystem/node.py
--rw-rw-rw-   0        0        0     3074 2023-05-15 11:25:51.000000 tknodesystem-0.1/tknodesystem/node_args.py
--rw-rw-rw-   0        0        0    11412 2023-05-17 07:49:13.000000 tknodesystem-0.1/tknodesystem/node_canvas.py
--rw-rw-rw-   0        0        0     8522 2023-05-15 11:43:22.000000 tknodesystem-0.1/tknodesystem/node_menu.py
--rw-rw-rw-   0        0        0     4549 2023-05-17 06:00:55.000000 tknodesystem-0.1/tknodesystem/node_socket.py
--rw-rw-rw-   0        0        0    30830 2023-05-17 11:43:32.000000 tknodesystem-0.1/tknodesystem/node_types.py
--rw-rw-rw-   0        0        0     4340 2023-05-17 07:12:15.000000 tknodesystem-0.1/tknodesystem/node_wire.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:36:23.510089 tknodesystem-0.1/tknodesystem.egg-info/
--rw-rw-rw-   0        0        0     2346 2023-05-17 15:36:23.000000 tknodesystem-0.1/tknodesystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-05-17 15:36:23.000000 tknodesystem-0.1/tknodesystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-05-17 15:36:23.000000 tknodesystem-0.1/tknodesystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-17 15:36:23.000000 tknodesystem-0.1/tknodesystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 15:36:23.000000 tknodesystem-0.1/tknodesystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.3/LICENSE
+-rw-rw-rw-   0        0        0     2621 2023-05-20 07:42:12.262125 tknodesystem-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-05-20 06:28:49.000000 tknodesystem-0.3/README.md
+-rw-rw-rw-   0        0        0      570 2023-05-20 07:42:12.262125 tknodesystem-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-20 07:41:50.000000 tknodesystem-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.246496 tknodesystem-0.3/tknodesystem/
+-rw-rw-rw-   0        0        0      278 2023-05-20 07:41:30.000000 tknodesystem-0.3/tknodesystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/tknodesystem/grid_images/
+-rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.3/tknodesystem/grid_images/grid_dot.png
+-rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.3/tknodesystem/grid_images/grid_lines.png
+-rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.3/tknodesystem/grid_images/no_grid.png
+-rw-rw-rw-   0        0        0     4693 2023-05-20 06:06:47.000000 tknodesystem-0.3/tknodesystem/node.py
+-rw-rw-rw-   0        0        0     3074 2023-05-15 11:25:51.000000 tknodesystem-0.3/tknodesystem/node_args.py
+-rw-rw-rw-   0        0        0    11797 2023-05-19 11:52:04.000000 tknodesystem-0.3/tknodesystem/node_canvas.py
+-rw-rw-rw-   0        0        0     9357 2023-05-20 07:37:26.000000 tknodesystem-0.3/tknodesystem/node_menu.py
+-rw-rw-rw-   0        0        0     4549 2023-05-17 06:00:55.000000 tknodesystem-0.3/tknodesystem/node_socket.py
+-rw-rw-rw-   0        0        0    31498 2023-05-20 06:34:42.000000 tknodesystem-0.3/tknodesystem/node_types.py
+-rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.3/tknodesystem/node_wire.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/tknodesystem.egg-info/
+-rw-rw-rw-   0        0        0     2621 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/top_level.txt
```

### Comparing `tknodesystem-0.1/LICENSE` & `tknodesystem-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/PKG-INFO` & `tknodesystem-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.1
+Version: 0.3
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -28,19 +28,23 @@
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
 
+[![PyPI](https://img.shields.io/pypi/v/tknodesystem)](https://pypi.org/project/tknodesystem)
+[![Downloads](https://static.pepy.tech/badge/tknodesystem)](https://pepy.tech/project/tknodesystem)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
 ### Requirements
 - tkinter
 - customtkinter _(for the node menu)_
 
-## Overview:
+## Overview
 
 - Node Types
 
 ![node_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/cccf82dd-8207-4894-9e9e-ef240e511d85)
 
 - Node Menu
 
@@ -49,17 +53,17 @@
 - Node Canvas
 
 ![canvas_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/d5568962-50c0-404c-bf71-79d66f79e3b7)
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
-[<img src="https://img.shields.io/badge/View-Docs-informational?&color=yellow&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
+[<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
 Examples are given in the `examples` folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
-**So, please report the bugs at the issues/discussions. A pull request is always welcomed :)**
+**So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.1/README.md` & `tknodesystem-0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,23 @@
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
 
+[![PyPI](https://img.shields.io/pypi/v/tknodesystem)](https://pypi.org/project/tknodesystem)
+[![Downloads](https://static.pepy.tech/badge/tknodesystem)](https://pepy.tech/project/tknodesystem)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
 ### Requirements
 - tkinter
 - customtkinter _(for the node menu)_
 
-## Overview:
+## Overview
 
 - Node Types
 
 ![node_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/cccf82dd-8207-4894-9e9e-ef240e511d85)
 
 - Node Menu
 
@@ -34,17 +38,17 @@
 - Node Canvas
 
 ![canvas_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/d5568962-50c0-404c-bf71-79d66f79e3b7)
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
-[<img src="https://img.shields.io/badge/View-Docs-informational?&color=yellow&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
+[<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
 Examples are given in the `examples` folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
-**So, please report the bugs at the issues/discussions. A pull request is always welcomed :)**
+**So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.1/setup.cfg` & `tknodesystem-0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b6e 6f64 6573 7973 7465 6d0d   = tknodesystem.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 0d0a  .version = 0.1..
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 0d0a  .version = 0.3..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5369  description = Si
 00000040: 6d70 6c65 2056 6973 7561 6c20 4e6f 6465  mple Visual Node
 00000050: 2073 7973 7465 6d20 7769 7468 2054 6b69   system with Tki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `tknodesystem-0.1/setup.py` & `tknodesystem-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tknodesystem',
-    version = '0.1',
+    version = '0.3',
     description = "Simple visual node system (DAG) with tkinter!",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/TkNodeSystem",
```

### Comparing `tknodesystem-0.1/tknodesystem/grid_images/grid_dot.png` & `tknodesystem-0.3/tknodesystem/grid_images/grid_dot.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/grid_images/grid_lines.png` & `tknodesystem-0.3/tknodesystem/grid_images/grid_lines.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/grid_images/no_grid.png` & `tknodesystem-0.3/tknodesystem/grid_images/no_grid.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/node.py` & `tknodesystem-0.3/tknodesystem/node.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/node_args.py` & `tknodesystem-0.3/tknodesystem/node_args.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/node_canvas.py` & `tknodesystem-0.3/tknodesystem/node_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tkinter
 import platform
 import os
 import json
-
+import sys
 from .node_wire import NodeWire
 from .node_types import NodeValue, NodeOperation, NodeCompile
 
 class NodeCanvas(tkinter.Canvas):
     def __init__(self, master, bg="grey10", width=500, height=500, wire_color="white", wire_width=3,
                  grid_image="lines", zoom=True, wire_dash=True, move=True, wire_hover_color="red", **kwargs):
         
@@ -31,16 +31,20 @@
         self.obj_list = set()
         self.line_ids = []
         self.gain_in = 1
         self.gain_out = 1
         self.set_grid_image(grid_image)
         
         if move:
-            self.tag_bind(self.grid, '<ButtonPress-2>', lambda e: self.getpos(e, 1))
-            self.tag_bind(self.grid, '<ButtonRelease-2>', lambda e: self.getpos(e, 0))
+            if sys.platform.startswith("darwin"):
+                self.tag_bind(self.grid, '<ButtonPress-3>', lambda e: self.getpos(e, 1))
+                self.tag_bind(self.grid, '<ButtonRelease-3>', lambda e: self.getpos(e, 0))
+            else:
+                self.tag_bind(self.grid, '<ButtonPress-2>', lambda e: self.getpos(e, 1))
+                self.tag_bind(self.grid, '<ButtonRelease-2>', lambda e: self.getpos(e, 0))
             self.tag_bind(self.grid, "<B2-Motion>", self.move_grid)
         
         if zoom:
             self.bind("<MouseWheel>", self.do_zoom)
             self.tag_bind(self.grid, "<Button-4>", lambda e: self.do_zoom(e, 120))
             self.tag_bind(self.grid, "<Button-5>", lambda e: self.do_zoom(e, -120))
             
@@ -178,15 +182,18 @@
             obj_dict = {f'{obj.type} {id}': (obj.args, round(obj.output_.center[0]-obj.width,2),
                                              round(obj.output_.center[1]-obj.height,2), obj.socket_nums) for id, obj in enumerate(sorted_obj_list)}
             obj_dict.update({"Lines" : list(self.line_list)})
             json.dump(obj_dict, file)
 
     def load(self, filename):
         """ load the node tree back to the canvas """
-        
+
+        if not os.path.exists(filename):
+            raise FileNotFoundError("No such file found: " + str(filename))
+  
         self.clear()
         self.connect_wire = False
         self.wire_color = self.bg  # hides an unwanted glitch
         
         obj_type_dict = {'NodeValue': NodeValue,
                          'NodeOperation': NodeOperation,
                          'NodeCompile': NodeCompile}
```

### Comparing `tknodesystem-0.1/tknodesystem/node_menu.py` & `tknodesystem-0.3/tknodesystem/node_menu.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,38 +11,51 @@
                  scrollbar=True, scrollbar_button_hover_color=None, frame_border_width=2,
                  command=None, alpha: float = 0.97, frame_corner_radius=20, label="Search Nodes", 
                  resize=True, border_color=None, **kwargs):
         
         super().__init__(takefocus=1)
         
         self.focus()
-        self.overrideredirect(True)
         self.alpha = alpha
-        self.attributes('-alpha', self.alpha)
+        self.attributes('-alpha', 0)
         self.corner = frame_corner_radius
 
         self.attach = attach
         self.height = height
         self.width = width
         self.command = command
         self.fade = False
         self.resize = resize
         self.button_num = 0
         self.node = {}
+        self.padding = 0
+        self.focus_something = False
         
+        self.withdraw()
         if sys.platform.startswith("win"):
+            self.overrideredirect(True)
             self.transparent_color = self._apply_appearance_mode(self._fg_color)
-            self.attributes("-transparentcolor", self.transparent_color) 
+            self.attributes("-transparentcolor", self.transparent_color)
+            self.attach.bind("<Double-Button-3>", self.popup, add="+")
+            self.bind("<FocusOut>", lambda e: self._withdraw())
         elif sys.platform.startswith("darwin"):
+            self.overrideredirect(True)
             self.transparent_color = 'systemTransparent'
             self.attributes("-transparent", True)
             self.transient(self.master)
+            self.attach.bind("<Button-1>", lambda e: self._withdraw(), add="+")
+            self.attach.bind("<Double-Button-2>", self.popup, add="+")
+            self.focus_something = True
         else:
+            self.attributes("-type", "splash")
             self.transparent_color = '#000001'
             self.corner = 0
+            self.padding = 20
+            self.attach.bind("<Double-Button-3>", self.popup, add="+")
+            self.bind("<FocusOut>", lambda e: self._withdraw())
             
         self.fg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"] if fg_color is None else fg_color
         self.scroll_button_color = customtkinter.ThemeManager.theme["CTkScrollbar"]["button_color"] if scrollbar_button_color is None else scrollbar_button_color
         self.scroll_hover_color = customtkinter.ThemeManager.theme["CTkScrollbar"]["button_hover_color"] if scrollbar_button_hover_color is None else scrollbar_button_hover_color
         self.border_color = customtkinter.ThemeManager.theme["CTkFrame"]["border_color"] if border_color is None else border_color
         self.button_color = customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"] if button_color is None else button_color
         self.text_color = customtkinter.ThemeManager.theme["CTkLabel"]["text_color"] if text_color is None else text_color
@@ -71,114 +84,118 @@
         
         self.frame = customtkinter.CTkScrollableFrame(self.frame_top, fg_color=self.fg_color,
                                         scrollbar_button_hover_color=self.scroll_hover_color,
                                         corner_radius=self.corner, scrollbar_button_color=self.scroll_button_color,)
         
         self.frame._scrollbar.grid_configure(padx=3)
         
-        self.frame.pack(expand=True, fill="both", padx=8, pady=(0,6))
+        if self.padding:
+            frame_padding = 10
+        else:
+            frame_padding = (0,6)
+            
+        self.frame.pack(expand=True, fill="both", padx=8, pady=frame_padding)
         self.no_match = customtkinter.CTkLabel(self.frame, text="No Match")
         
         if justify.lower()=="left":
             self.justify = "w"
         elif justify.lower()=="right":
             self.justify = "e"
         else:
             self.justify = "c"
             
         self.button_height = button_height
         
         self.resizable(width=False, height=False)
         self.disable = False
     
-        self.attach.bind("<Double-Button-3>", self.popup, add="+")
         self.attach.bind_all("<space>", self.popup)
-        self.bind("<FocusOut>", lambda e: self._withdraw())
         
         self.update_idletasks()
-        self.withdraw()
         self.attach.focus_set()
 
     def _withdraw(self):
         if not self.disable:
             self.withdraw() 
             self.attach.bind_all("<space>", self.popup)
             
     def fade_out(self):
         for i in range(100,0,-10):
             if not self.winfo_exists():
                 break
             self.attributes("-alpha", i/100)
             self.update()
-            time.sleep(1/1000)
+            time.sleep(1/100)
             
     def fade_in(self):
         for i in range(0,100,10):
             if not self.winfo_exists():
                 break
             self.attributes("-alpha", i/100)
             self.update()
-            time.sleep(1/1000)
+            time.sleep(1/100)
             
     def search(self, a,b,c):
         self.live_update(self.var.get())
         
     def add_node(self, label, command, **button_kwargs):                         
         self.node[self.button_num] = customtkinter.CTkButton(self.frame,
                                                              text=label,
                                                              text_color=self.text_color,
                                                              height=self.button_height,
                                                              fg_color=self.button_color,
                                                              anchor=self.justify, 
                                                              command=lambda: self._attach_key_press(command), **button_kwargs)
-        self.node[self.button_num].pack(fill="x", pady=5)
+        self.node[self.button_num].pack(fill="x", pady=5, padx=(self.padding,0))
         self.button_num +=1
 
     def destroy_popup(self):
         self.destroy()
         self.disable = True
 
     def place_dropdown(self, x=None, y=None):
         self.geometry('{}x{}+{}+{}'.format(self.width, self.height, x, y))
         self.fade_in()
         self.attributes('-alpha', self.alpha)
         
     def _iconify(self, x=None, y=None):
         self.focus_set()
+        self.search_entry.focus_set()
         self._deiconify()
+        if self.focus_something: self.node[0].focus_set()
         self.place_dropdown(x,y)
 
     def _attach_key_press(self, command):
         self.fade_out()
-        command()
         self.withdraw()
+        command()
         
     def live_update(self, string=None):
         if self.disable: return
         if self.fade: return
         if string:
             i=1
             for key in self.node.keys():
                 s = self.node[key].cget("text").lower()
                 if not s.startswith(string.lower()):
                     self.node[key].pack_forget()
                 else:
-                    self.node[key].pack(fill="x", pady=5)
+                    self.node[key].pack(fill="x", pady=5, padx=(self.padding,0))
                     i+=1
                     
             if i==1:
-                self.no_match.pack(fill="x", pady=2)
+                self.no_match.pack(fill="x", pady=2, padx=(self.padding,0))
             else:
                 self.no_match.pack_forget()
             self.button_num = i
             
         else:
             self.no_match.pack_forget()
             for key in self.node.keys():
-                self.node[key].pack(fill="x", pady=5)
+                self.node[key].pack(fill="x", pady=5, padx=(self.padding,0))
            
     def _deiconify(self):
         if self.button_num>0:
             self.deiconify()
         
     def popup(self, event):
         if self.disable: return
```

### Comparing `tknodesystem-0.1/tknodesystem/node_socket.py` & `tknodesystem-0.3/tknodesystem/node_socket.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem/node_types.py` & `tknodesystem-0.3/tknodesystem/node_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .node_socket import NodeSocket
 from .node_args import Args
 
 class NodeValue(Node):
     def __init__(self, canvas, width=100, height=50, value=0, border_color='white', text=None, corner_radius=25,
                  border_width=0, fg_color='#37373D', text_color='white', font=("",10), socket_radius=8, socket_hover=True,
                  socket_color="green", socket_hover_color="grey50", highlightcolor='#52d66c', hover=True,
-                 click_command=None, side="right", x=None, y=None, num=None):
+                 click_command=None, side="right", x=0, y=0, num=None):
 
         self.text = text
         self.canvas = canvas
         
         self.args = Args.value_args(locals())
         
         if click_command:
@@ -60,15 +60,15 @@
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 0.9, 0.9)
                 
-        if x and y:
+        if x or y:
             super().move(x,y)
      
         self.canvas.obj_list.add(self)
 
     def get(self):
         """ get the current value of node """
         return self.output_.value
@@ -89,15 +89,18 @@
 
         self.output_.value = None
         for i in self.allIDs:
             self.canvas.delete(i)
             
         self.canvas.obj_list.remove(self)
         super().destroy()
-
+        
+        for i in self.connected_func:
+            i.update()
+                
     def exists(self):
         if self.ID in self.canvas.find_all():
             return True
         else:
             return False
         
     def configure(self, **kwargs):
@@ -131,15 +134,15 @@
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
 
 class NodeOperation(Node):
     def __init__(self, canvas, width=100, height=None, inputs=2, border_color='white', text=None,
                  socket_radius=8, corner_radius=25, border_width=0, fg_color='#37373D', text_color='white', font=("",10),
-                 highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=None, y=None,
+                 highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=0, y=0,
                  multiside=False, command=None, output_socket_color="green", click_command=None, socket_hover=True, num=None):
 
         self.text = text
         self.canvas = canvas
         self.type = 'NodeOperation'
         
         if self.text is None:
@@ -181,15 +184,16 @@
 
         self.line1 = None
         self.line2 = None
         self.line3 = None
         self.line4 = None
         self.line5 = None
         self.socket_colors = []
-        self.connected_node = None
+        self.connected_node = set()
+        self.connected_node_first = None
         x_pos = x
         y_pos = y
             
         if type(socket_color) is list:
             self.socket_colors = socket_color
         else:
             for i in range(5):
@@ -292,15 +296,15 @@
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 0.9, 0.9)
                 
-        if x_pos and y_pos:
+        if x_pos or y_pos:
             super().move(x_pos,y_pos)
             
         self.canvas.obj_list.add(self)
         
     def connect_output(self, event):
         """ connect output socket """
 
@@ -310,42 +314,46 @@
         if self.canvas.clickcount == 2:
             self.canvas.clickcount = 0
             
         self.output_.connect_wire()
  
     def connect_input(self, line_id, input_id):
         """ connect input sockets """
-        
-        if self.canvas.outputcell==self.connected_node:
+        if self.canvas.outputcell is None:
+            return
+        if self.canvas.outputcell in self.connected_node:
             return
         if self.canvas.outputcell==self:
             return
+ 
+        m = self.connected_node_first
 
-        m = self.connected_node
         for i in range(self.canvas.operation_num):
             if m is None:
                 break
             if m.type=="NodeOperation":
-                if self.canvas.outputcell==m:
+                if self.canvas.outputcell in m.connected_node:
                     return
-            m = m.connected_node
+            m = m.connected_node_first
         
         try: self.canvas.delete(line_id.ID)
         except: None
         
         self.canvas.clickcount += 1
         self.canvas.IDc = input_id
         self.canvas.inputcell = self
         
         if self.canvas.clickcount == 2:
             self.canvas.clickcount = 0
             self.canvas.conectcells()
-            if self.canvas.outputcell: self.canvas.outputcell.connected_node = self
             if self.canvas.outputcell.type=="NodeValue":
                 self.canvas.outputcell.connected_func.add(self)
+            elif self.canvas.outputcell.type=="NodeOperation":
+                self.canvas.outputcell.connected_node.add(self)
+                self.canvas.outputcell.connected_node_first = self
             try:
                 if input_id=="input1":
                     for x in self.canvas.line_list:
                         if x[1]==self.input_1.socket_num:
                             self.canvas.line_list.remove(x)
                             break
                     l = (self.canvas.outputcell.output_.socket_num, self.canvas.inputcell.input_1.socket_num)
@@ -376,18 +384,22 @@
                         if x[1]==self.input_5.socket_num:
                             self.canvas.line_list.remove(x)
                             break
                     l = (self.canvas.outputcell.output_.socket_num, self.canvas.inputcell.input_5.socket_num)
                     self.canvas.line_list.add(l)
             except AttributeError: None
         else:
-            if self.canvas.outputcell: self.canvas.outputcell.connected_node = None
             if self.canvas.outputcell.type=="NodeValue":
                 try: self.canvas.outputcell.connected_func.remove(self)
                 except KeyError: None
+            elif self.canvas.outputcell.type=="NodeOperation":
+                try:
+                    self.canvas.outputcell.connected_node.remove(self)
+                    self.canvas.outputcell.connected_node_first = None
+                except KeyError: None
             try:
                 if input_id=="input1":
                     self.cellinput1 = None
                     self.canvas.line_list.remove((self.canvas.outputcell.output_.socket_num, self.canvas.inputcell.input_1.socket_num))
                 if input_id=="input2":
                     self.cellinput2 = None
                     self.canvas.line_list.remove((self.canvas.outputcell.output_.socket_num, self.canvas.inputcell.input_2.socket_num))
@@ -431,30 +443,35 @@
                         self.output_.value = 1
                         
                 if self.output_.value:
                     self.output_.value = self.command(*values_args[0:self.inputs])
         else:
             self.output_.value = None
 
-        if self.connected_node:
-            self.connected_node.update()
-
+        if len(self.connected_node)>0:
+            for i in self.connected_node:
+                i.update()
+        
     def get(self):
         """ get the current value of node """
         return self.output_.value
     
     def destroy(self):
         if self.ID not in self.canvas.find_all(): return
         self.output_.value = None
         for i in self.id_list:
             self.canvas.delete(i)
 
         self.canvas.obj_list.remove(self)
         super().destroy()
         
+        if len(self.connected_node)>0:
+            for i in self.connected_node:
+                i.update()
+                
     def exists(self):
         if self.ID in self.canvas.find_all():
             return True
         else:
             return False
         
     def configure(self, **kwargs):
@@ -518,15 +535,15 @@
                 self.input_5.configure(hover=hover)
             except: None
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
         
 class NodeCompile(Node):
-    def __init__(self, canvas, width=100, height=50, border_color='white', text="Compile", socket_radius=8, corner_radius=25, x=None, y=None,
+    def __init__(self, canvas, width=100, height=50, border_color='white', text="Compile", socket_radius=8, corner_radius=25, x=0, y=0,
                  border_width=0, fg_color='#37373D',text_color='white', font=("",10), highlightcolor='#52d66c', hover=True, socket_hover=True,
                  socket_color="green", socket_hover_color="grey50", show_value=True, command=None, click_command=None, side="left", num=None):
 
         self.canvas = canvas
         self.text = text
         self.type = 'NodeCompile'
         
@@ -591,15 +608,15 @@
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 0.9, 0.9)
                 
-        if x and y:
+        if x or y:
             super().move(x,y)
             
         self.canvas.obj_list.add(self)
         
     def connect_input(self, event):
         """ connect input sockets """
```

### Comparing `tknodesystem-0.1/tknodesystem/node_wire.py` & `tknodesystem-0.3/tknodesystem/node_wire.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.1/tknodesystem.egg-info/PKG-INFO` & `tknodesystem-0.3/tknodesystem.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.1
+Version: 0.3
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -28,19 +28,23 @@
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
 
+[![PyPI](https://img.shields.io/pypi/v/tknodesystem)](https://pypi.org/project/tknodesystem)
+[![Downloads](https://static.pepy.tech/badge/tknodesystem)](https://pepy.tech/project/tknodesystem)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
 ### Requirements
 - tkinter
 - customtkinter _(for the node menu)_
 
-## Overview:
+## Overview
 
 - Node Types
 
 ![node_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/cccf82dd-8207-4894-9e9e-ef240e511d85)
 
 - Node Menu
 
@@ -49,17 +53,17 @@
 - Node Canvas
 
 ![canvas_types](https://github.com/Akascape/TkNodeSystem/assets/89206401/d5568962-50c0-404c-bf71-79d66f79e3b7)
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
-[<img src="https://img.shields.io/badge/View-Docs-informational?&color=yellow&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
+[<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
 Examples are given in the `examples` folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
-**So, please report the bugs at the issues/discussions. A pull request is always welcomed :)**
+**So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.1/tknodesystem.egg-info/SOURCES.txt` & `tknodesystem-0.3/tknodesystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

