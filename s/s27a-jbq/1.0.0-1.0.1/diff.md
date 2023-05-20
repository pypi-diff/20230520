# Comparing `tmp/s27a_jbq-1.0.0.tar.gz` & `tmp/s27a_jbq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s27a_jbq-1.0.0.tar", last modified: Sun May 14 04:15:06 2023, max compression
+gzip compressed data, was "s27a_jbq-1.0.1.tar", last modified: Sat May 20 13:07:16 2023, max compression
```

## Comparing `s27a_jbq-1.0.0.tar` & `s27a_jbq-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:15:06.990480 s27a_jbq-1.0.0/
--rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    11359 2023-05-14 04:15:06.990480 s27a_jbq-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10864 2023-05-14 03:51:09.000000 s27a_jbq-1.0.0/README.md
--rw-rw-rw-   0        0        0      575 2023-05-14 04:00:28.000000 s27a_jbq-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 04:15:06.990480 s27a_jbq-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 04:15:06.951228 s27a_jbq-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 04:15:06.982957 s27a_jbq-1.0.0/src/s27a_jbq/
--rw-rw-rw-   0        0        0      661 2023-05-11 10:07:26.000000 s27a_jbq-1.0.0/src/s27a_jbq/__init__.py
--rw-rw-rw-   0        0        0     3912 2023-05-13 10:07:34.000000 s27a_jbq-1.0.0/src/s27a_jbq/extension.py
--rw-rw-rw-   0        0        0     9248 2023-05-12 15:01:56.000000 s27a_jbq-1.0.0/src/s27a_jbq/main.py
--rw-rw-rw-   0        0        0     8910 2023-05-13 10:04:37.000000 s27a_jbq-1.0.0/src/s27a_jbq/map.py
--rw-rw-rw-   0        0        0     1487 2023-05-05 11:23:38.000000 s27a_jbq-1.0.0/src/s27a_jbq/static.json.py
--rw-rw-rw-   0        0        0     5927 2023-05-14 04:14:00.000000 s27a_jbq-1.0.0/src/s27a_jbq/static.py
--rw-rw-rw-   0        0        0    12989 2023-05-14 04:01:00.000000 s27a_jbq-1.0.0/src/s27a_jbq/window.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:15:06.990480 s27a_jbq-1.0.0/src/s27a_jbq.egg-info/
--rw-rw-rw-   0        0        0    11359 2023-05-14 04:15:06.000000 s27a_jbq-1.0.0/src/s27a_jbq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-14 04:15:06.000000 s27a_jbq-1.0.0/src/s27a_jbq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:15:06.000000 s27a_jbq-1.0.0/src/s27a_jbq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 04:15:06.000000 s27a_jbq-1.0.0/src/s27a_jbq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.835660 s27a_jbq-1.0.1/
+-rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    11714 2023-05-20 13:07:16.835660 s27a_jbq-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11197 2023-05-20 10:36:24.000000 s27a_jbq-1.0.1/README.md
+-rw-rw-rw-   0        0        0      597 2023-05-18 13:05:59.000000 s27a_jbq-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:07:16.837428 s27a_jbq-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.796029 s27a_jbq-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.817998 s27a_jbq-1.0.1/src/s27a_jbq/
+-rw-rw-rw-   0        0        0      225 2023-05-20 12:22:46.000000 s27a_jbq-1.0.1/src/s27a_jbq/__constants__.py
+-rw-rw-rw-   0        0        0      719 2023-05-20 12:21:22.000000 s27a_jbq-1.0.1/src/s27a_jbq/__init__.py
+-rw-rw-rw-   0        0        0     3970 2023-05-16 13:59:35.000000 s27a_jbq-1.0.1/src/s27a_jbq/extension.py
+-rw-rw-rw-   0        0        0    10275 2023-05-20 13:04:44.000000 s27a_jbq-1.0.1/src/s27a_jbq/game.py
+-rw-rw-rw-   0        0        0     6379 2023-05-20 09:57:48.000000 s27a_jbq-1.0.1/src/s27a_jbq/map.py
+-rw-rw-rw-   0        0        0     6817 2023-05-20 12:52:08.000000 s27a_jbq-1.0.1/src/s27a_jbq/static.py
+-rw-rw-rw-   0        0        0    14907 2023-05-20 12:52:02.000000 s27a_jbq-1.0.1/src/s27a_jbq/window.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:07:16.832037 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/
+-rw-rw-rw-   0        0        0    11714 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 13:07:16.000000 s27a_jbq-1.0.1/src/s27a_jbq.egg-info/top_level.txt
```

### Comparing `s27a_jbq-1.0.0/LICENSE` & `s27a_jbq-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.0/PKG-INFO` & `s27a_jbq-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: s27a_jbq
-Version: 1.0.0
-Summary: A simple chess game
+Version: 1.0.1
+Summary: A board game with high degrees of freedom
 Author-email: amf <xyf081202@163.com>
 Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
 Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.0-blue)
+![](https://img.shields.io/badge/release-1.0.1-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
-精班棋是一款自由度很高的将棋
+精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
 
 # 目录
 
@@ -32,37 +32,37 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您需要一个`Python 3`环境
-
 您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
 
 ``` python
 from s27a_jbq import generate_game
 
 generate_game(
    game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，使用相对路径时根目录为游戏文件夹路径
+   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
    display = "window" # 游戏打开方式，'window'为窗口模式
 )
 ```
 
-也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
+您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
+from s27a_jbq.game import App
+
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
@@ -78,17 +78,21 @@
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
+在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+
 ## 地图
 
-地图文件是`.xlsx`文件，其中包含3个表，分别对应棋子、棋盘与特殊规则
+地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
+
+地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
 您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图
 
 下文介绍了地图文件的构造以及自定义地图的方法
 
 ### 棋盘构造
 
@@ -325,8 +329,8 @@
 - `check_can_go`：函数
 - `after_move`：函数
 
 # 许可证
 
 [(返回目录)](#目录)
 
-[MIT License](./LICENSE)
+[MIT License](https://github.com/amf14151/s27a_jbq/blob/main/LICENSE)
```

### Comparing `s27a_jbq-1.0.0/README.md` & `s27a_jbq-1.0.1/src/s27a_jbq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+Metadata-Version: 2.1
+Name: s27a-jbq
+Version: 1.0.1
+Summary: A board game with high degrees of freedom
+Author-email: amf <xyf081202@163.com>
+Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
+Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.0-blue)
+![](https://img.shields.io/badge/release-1.0.1-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
-精班棋是一款自由度很高的将棋
+精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
 
 # 目录
 
@@ -18,37 +32,37 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您需要一个`Python 3`环境
-
 您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
 
 ``` python
 from s27a_jbq import generate_game
 
 generate_game(
    game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，使用相对路径时根目录为游戏文件夹路径
+   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
    display = "window" # 游戏打开方式，'window'为窗口模式
 )
 ```
 
-也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
+您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
+from s27a_jbq.game import App
+
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
@@ -64,17 +78,21 @@
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
+在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+
 ## 地图
 
-地图文件是`.xlsx`文件，其中包含3个表，分别对应棋子、棋盘与特殊规则
+地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
+
+地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
 您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图
 
 下文介绍了地图文件的构造以及自定义地图的方法
 
 ### 棋盘构造
 
@@ -311,8 +329,8 @@
 - `check_can_go`：函数
 - `after_move`：函数
 
 # 许可证
 
 [(返回目录)](#目录)
 
-[MIT License](./LICENSE)
+[MIT License](https://github.com/amf14151/s27a_jbq/blob/main/LICENSE)
```

### Comparing `s27a_jbq-1.0.0/src/s27a_jbq/extension.py` & `s27a_jbq-1.0.1/src/s27a_jbq/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     PATH = "extensions"
     def __init__(self,app):
         self.debug = app.debug
         self.extapi = ExtAPI(app)
         self.extensions = list[Extension]()
         ExtensionManager.Ext = self # 全局变量
         if not os.path.exists(ExtensionManager.PATH):
+            os.mkdir(ExtensionManager.PATH)
             return
         for i in os.listdir(ExtensionManager.PATH):
             self.load_extension(os.path.join(ExtensionManager.PATH,i))
 
     def load_extension(self,filename:str):
         def wrapper():
             if os.path.splitext(filename)[1] != ".py":
@@ -98,15 +99,15 @@
                 new_can_go = i.check_can_go(can_go,chess,arr)
                 if new_can_go == None:
                     raise TypeError("check_can_go函数无返回值")
             else:
                 try:
                     new_can_go = i.check_can_go(can_go,chess,arr)
                 except:
-                    pass
+                    new_can_go = None
             if new_can_go != None:
                 can_go = [j for j in new_can_go if j]
         return can_go
 
     def after_move(self,arr1:ARR,arr2:ARR):
         for i in self.extensions:
             if not i.use:
```

### Comparing `s27a_jbq-1.0.0/src/s27a_jbq/main.py` & `s27a_jbq-1.0.1/src/s27a_jbq/game.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 if sys.platform != "win32":
     sys.stdout("程序必须在Windows系统中运行")
     sys.exit()
 
 from tkinter.messagebox import showinfo,showwarning,showerror
 
-from .static import xlrd,ARR,MapViewer,static_data
+from .static import ARR,MapViewer,static_data,save_record
 from .map import Chess,Map,HistoryRecorder
 from .window import MainWindow,GameWindow,SettingWindow
 from .extension import ExtAPI,ExtensionManager
 
 class App:
     def __init__(self,record_path:str = None):
         self.map_data = None
         self.map_path = None
-        self.record_path = record_path
+        if record_path and not record_path.endswith(".csv"):
+            record_path += ".csv"
+        self.record_path = record_path 
 
     def run(self,debug:bool = False):
         self.debug = debug
         self.extension_manager = ExtensionManager(self)
         self.window = MainWindow({
             # 主窗口调用的函数
             "get_map":self.get_map,
@@ -42,34 +44,34 @@
         else:
             try:
                 self.map_data = Map(*MapViewer.view(filename))
             except FileNotFoundError:
                 if error_prompt:
                     showwarning("提示","未找到地图文件")
                 return
-            except (TypeError,xlrd.biffh.XLRDError):
+            except:
                 if error_prompt:
                     showwarning("提示","地图文件格式错误")
                 return
         if success_prompt:
             showinfo("提示","地图文件加载成功")
         self.map_path = filename
         self.window.set_map(self.map_path)
 
     def start_game(self):
         if not self.map_data:
             showinfo("提示","暂未选择地图")
             return
         self.window.withdraw()
         if self.debug:
-            game = Game(self.map_data,self.record_path)
+            game = Game(self.map_data,self.record_path,self.debug)
             game.start()
         else:
             try:
-                game = Game(self.map_data,self.record_path)
+                game = Game(self.map_data,self.record_path,self.debug)
                 game.start()
             except Exception as e:
                 showerror("错误",f"游戏运行错误：{e}")
         self.window.deiconify()
 
     def add_extension(self):
         filename = self.window.choose_extension_file()
@@ -79,17 +81,18 @@
     def setting(self):
         setting_window = SettingWindow(self.add_extension,self.window.refresh_extension)
         setting_window.mainloop()
 
 # 游戏类
 # 每场创建一个新的Game对象
 class Game:
-    def __init__(self,map_data:Map,record_path:str):
+    def __init__(self,map_data:Map,record_path:str,debug:bool):
         self.map_data = map_data
         self.record_path = record_path
+        self.debug = debug
         self.map_data.init_chessboard(self.win)
         self.history_recorder = HistoryRecorder(self.map_data)
         game_api = {
             "click":self.click,
             "info":self.get_info,
             "back":self.back,
             "stop":self.stop
@@ -191,28 +194,48 @@
                     can_go.append(can_go[-1] + [d_arr])
                 elif chess.belong != 3 and mp.belong != 3 and mp.belong != self.turn:
                     can_go.append(can_go[-1] + [d_arr])
                     break
                 else:
                     break
                 k += 1
-            if not can_go[-1]:
-                del can_go[-1]
-        can_go = ExtensionManager.Ext.check_can_go(can_go,chess,arr) # 载入扩展修改can_go
-        new_can_go = set[ARR]() # 集合去重
+        can_go = ExtensionManager.Ext.check_can_go([i for i in can_go if i],chess,arr) # 载入扩展修改can_go
+        can_go_set = set[ARR]() # 集合去重
         for i in can_go:
             for j in i:
-                new_can_go.add(j)
-        return list(new_can_go)
+                can_go_set.add(j)
+        return list(can_go_set)
 
     # 显示棋子基本信息
     def get_info(self,arr:ARR):
         chess = self.map_data.chessboard[arr[0]][arr[1]]
         if chess:
-            showinfo("棋子信息",chess.info)
+            belong = "红方" if chess.belong == 1 else "蓝方" if chess.belong == 2 else "中立"
+            is_captain = "是" if chess.is_captain else "否"
+            is_tran = ("是" if chess.is_tran else "否") if chess.tran_con else "无法升变"
+            info = f"名称：{chess.name}\n编号：{chess.id}\n归属：{belong}\n首领棋子：{is_captain}\n是否升变：{is_tran}"
+            if self.debug:
+                if chess.attr:
+                    attr = "\n    ".join([f"{i}：{j}" for i,j in zip(chess.attr.keys(),chess.attr.values())])
+                    info += f"\n其他参数：\n    {attr}"
+                move = chess.tran_move if chess.is_tran else chess.move
+                show_move = ""
+                for i in range(len(move)):
+                    show_move += f"\n    第{i + 1}项："
+                    if not move[i]:
+                        show_move += "无"
+                        continue
+                    for j in move[i]:
+                        show_move += f"\n        方向{j[0]}："
+                        if j[1:]:
+                            show_move += f"{j[1:]}"
+                        else:
+                            show_move += "任意"
+                info += f"\n目前可行走函数：{show_move}"
+            showinfo("棋子信息",info)
 
     # 悔棋及撤销
     def back(self,steps:int):
         data = self.history_recorder.rollback(steps)
         if data:
             self.map_data.chessboard,self.turn = data
             self.refresh()
@@ -225,15 +248,9 @@
     # 只能由扩展触发
     def stalemate(self):
         showinfo("提示","双方和棋")
         self.stop()
 
     def stop(self):
         if self.record_path:
-            # 记录棋局
-            with open(self.record_path,"w",encoding = "utf-8") as wfile:
-                for i in self.history_recorder.history:
-                    print_chessboard = "\n".join([" ".join([k.attr["name_withspace"] if k else " " * 4 for k in j]) for j in i[0]])
-                    wfile.write("—" * 30 + "\n")
-                    wfile.write(print_chessboard + "\n")
-                wfile.write("—" * 30)
+            save_record(self.record_path,self.history_recorder.history) # 记录棋局
         self.running = False
```

### Comparing `s27a_jbq-1.0.0/src/s27a_jbq/map.py` & `s27a_jbq-1.0.1/src/s27a_jbq/map.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,26 @@
 import copy
 
 from tkinter.messagebox import showinfo
 
-from .static import ARR,static_data
+from .static import ARR
 from .extension import ExtensionManager
 
 class Chess:
     def __init__(self,id:int,name:str,belong:int,is_captain:bool,move:list[list[tuple]],tran_con:list[tuple],tran_move:list[list[tuple]],attr:dict[str],map_data):
         self.id = id
         self.name = name
         self.belong = belong
         self.is_captain = is_captain
         self.move = move
         self.tran_con = tran_con
         self.tran_move = tran_move
         self.attr = copy.copy(attr) # 每个棋子都有独特的attr
         self.map_data = map_data
         self.is_tran = False
-        self.get_name_space()
-
-    # 计算name前后的空格
-    def get_name_space(self):
-        self.attr["name_withspace"] = self.name
-        name_length = len(self.name.encode(encoding = "gbk"))
-        side = True # True为右侧
-        while name_length < 4:
-            if side:
-                self.attr["name_withspace"] += " "
-            else:
-                self.attr["name_withspace"] = " " + self.attr["name_withspace"]
-            side = not side
-            name_length += 1
 
     # 当前可移动位置
     @property
     def now_move(self):
         arr = self.map_data.get_chess_arr(self)
         move = list[list[int]]()
         for i in (self.tran_move if self.is_tran else self.move):
@@ -43,66 +29,14 @@
                 if len(j) == 1: # 没有判断条件
                     move[-1].append(j[0])
                 elif len(j) == 2:
                     if self.map_data.is_in_position(arr,j[1]):
                         move[-1].append(j[0])
         return move
 
-    # 在按钮上显示的文字
-    def text(self,rev:bool):
-        text = ""
-        now_move = self.now_move # 先赋值中间变量，避免调用self.now_move属性时重新计算
-        def _in(num,string = " " * 3):
-            nonlocal text
-            if num in now_move[1]:
-                text += "*"
-            elif num in now_move[0]:
-                text += "·"
-            else:
-                text += " "
-            text += string
-        _in(1)
-        _in(2)
-        _in(3,"\n")
-        _in(4," " * 2) # 空出名字位置
-        _in(5,"\n")
-        _in(6)
-        _in(7)
-        _in(8,"")
-        # 插入名字
-        text = list(text)
-        if rev:
-            text.reverse()
-        text.insert(12,self.attr["name_withspace"])
-        text = "".join(text)
-        # 设置字体颜色
-        if self.belong == 1:
-            if self.is_tran or not self.tran_con:
-                self.fg = static_data["colors"]["red-tran-chess-fg"]
-            else:
-                self.fg = static_data["colors"]["red-chess-fg"]
-        elif self.belong == 2:
-            if self.is_tran or not self.tran_con:
-                self.fg = static_data["colors"]["blue-tran-chess-fg"]
-            else:
-                self.fg = static_data["colors"]["blue-chess-fg"]
-        else:
-            self.fg = static_data["colors"]["neutral-chess-fg"]
-        return text
-
-    # 获取基本信息
-    @property
-    def info(self):
-        belong = "红方" if self.belong == 1 else "蓝方" if self.belong == 2 else "中立"
-        is_captain = "是" if self.is_captain else "否"
-        is_tran = ("是" if self.is_tran else "否") if self.tran_con else "无法升变"
-        move = self.tran_move if self.is_tran else self.move
-        info = f"名称：{self.name}\n编号：{self.id}\n归属：{belong}\n首领棋子：{is_captain}\n是否升变：{is_tran}\n其他参数：{self.attr}\n目前可行走函数：{move}"
-        return info
-
     # 升变条件检测
     def tran(self,arr:ARR):
         if self.is_tran:
             return
         if self.map_data.is_in_position(arr,self.tran_con):
             self.is_tran = True
```

### Comparing `s27a_jbq-1.0.0/src/s27a_jbq/window.py` & `s27a_jbq-1.0.1/src/s27a_jbq/window.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import tkinter as tk
 import webbrowser
 
 from tkinter.messagebox import showinfo
 from tkinter.filedialog import askopenfilename
 
-from .static import ARR,static_data,refresh_extension,refresh_color
+from .__constants__ import __version__
+from .static import ARR,RELEASE_DATE,static_data,refresh_extension,refresh_color
 from .map import Map
 from .extension import Extension,ExtensionManager
 
 class MainWindow(tk.Tk):
     def __init__(self,app_api:dict,debug:bool):
         super().__init__()
         self.app_api = app_api
-        self.title(f"精班棋 {static_data['VERSION']}{' [debug mode]' if debug else ''}")
+        self.title(f"精班棋 {__version__}{' [debug mode]' if debug else ''}")
         self.minsize(480,360)
         self.resizable(width = False,height = False)
         self.start_btn = tk.Button(self,text = "开始游戏",width = 60,height = 3,**static_data["shape-style"]["btn-style"],command = self.app_api["start_game"])
         self.start_btn.pack(pady = 5)
-        self.map_label = tk.Label(self,text = "暂未选择",width = 60,height = 3,**static_data["shape-style"]["label-style"])
+        self.map_label = tk.Label(self,text = "未选择地图",width = 60,height = 3,**static_data["shape-style"]["label-style"])
         self.map_label.pack(pady = 5)
         self.map_btn_frame = tk.Frame(self)
         self.map_btn_frame.pack(pady = 5)
         self.get_map_btn = tk.Button(self.map_btn_frame,text = "选择地图",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["get_map"])
         self.get_map_btn.pack(side = "left",padx = 5)
         self.refresh_map_btn = tk.Button(self.map_btn_frame,text = "刷新地图",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["refresh_map"])
         self.refresh_map_btn.pack(side = "right",padx = 5)
-        self.extension_label = tk.Label(self,text = "暂无扩展",width = 60,**static_data["shape-style"]["label-style"])
+        self.extension_label = tk.Label(self,width = 60,**static_data["shape-style"]["label-style"])
         self.extension_label.pack(pady = 5)
         self.set_extension_btn = tk.Button(self,text = "设置扩展",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["setting"])
         self.set_extension_btn.pack(pady = 5)
 
         self.refresh_extension()
         self.init_menu()
 
@@ -50,49 +51,50 @@
         self.game_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "游戏(G)",underline = 3,menu = self.game_menu)
         self.game_menu.add_command(label = "开始游戏",command = self.app_api["start_game"])
         # 帮助菜单
         self.help_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "帮助(H)",underline = 3,menu = self.help_menu)
         self.help_menu.add_command(label = "精班棋文档",command = self.open_url("https://github.com/amf14151/s27a_jbq/blob/main/README.md"))
-        self.help_menu.add_command(label = "获取扩展",command = self.open_url("https://github.com/amf14151/s27a_jbq/tree/main/extensions"))
         self.help_menu.add_command(label = "获取地图",command = self.open_url("https://github.com/amf14151/s27a_jbq/tree/main/map"))
+        self.help_menu.add_command(label = "获取扩展",command = self.open_url("https://github.com/amf14151/s27a_jbq/tree/main/extensions"))
         self.help_menu.add_separator()
         self.help_menu.add_command(label = "反馈",command = self.open_url("https://github.com/amf14151/s27a_jbq/issues"))
         self.help_menu.add_separator()
         self.help_menu.add_command(label = "关于精班棋",command = self.show_about)
 
     def choose_map_file(self):
-        filename = askopenfilename(filetypes = [("Excel Files","*.xls *.xlsx"),("All Files","*.*")],title = "选择地图文件")
+        filename = askopenfilename(filetypes = [("Excel Files","*.xlsx"),("All Files","*.*")],title = "选择地图文件")
         return filename
     
     def choose_extension_file(self):
-        filename = askopenfilename(filetypes = [("Python Files","*.py"),("All Files","*.*")],title = "选择扩展文件")
+        filename = askopenfilename(filetypes = [("Python Files","*.py")],title = "选择扩展文件")
         return filename
 
     def refresh_extension(self):
         refresh_extension(ExtensionManager.Ext.extensions)
         ext = "\n".join([(i.text() + ("" if i.use else "(未启用)")) for i in ExtensionManager.Ext.extensions])
-        self.extension_label["text"] = f"当前已添加扩展：\n{ext}"
+        self.extension_label["text"] = f"当前已加载扩展：\n{ext}" if ext else "未加载扩展"
 
     def set_map(self,filename:str):
         self.map_label["text"] = f"当前地图: \n{filename}"
 
     def open_url(self,url:str):
         return lambda:webbrowser.open(url)
 
     def show_about(self):
-        showinfo("关于精班棋",static_data["about"].format(static_data["VERSION"]))
+        showinfo("关于精班棋",f"版本: {__version__}\n发布日期: {RELEASE_DATE}")
 
 class GameWindow(tk.Tk):
     def __init__(self,belong:int,map_data:Map,game_api:dict):
         super().__init__()
         self.belong = belong
         self.map_data = map_data
         self.game_api = game_api
+        self.can_go_prompt_list = ["·","*","o","x"]
         self.title("红方" if self.belong == 1 else "蓝方")
         self.resizable(width = False,height = False)
         self.protocol("WM_DELETE_WINDOW",self.game_api["stop"])
         self.init_menu()
         self.init_chessboard()
         self.refresh_map()
 
@@ -120,20 +122,23 @@
 
     def map_info(self):
         rules = {
             "tran":"启用升变",
             "back":"启用悔棋",
             "restrict_move_ne":"限制连续3步以上移动中立棋子"
         }
-        info = ""
+        info = "特殊规则：\n"
         for i in rules:
             info += f"{rules[i]}：{'是' if self.map_data.rules[i] else '否'}\n"
         exts = "\n    ".join([i.text() for i in ExtensionManager.Ext.extensions if i.use])
-        info += f"当前已启用扩展：\n    {exts if exts else '当前未启用扩展'}"
-        showinfo("特殊规则",info)
+        if exts:
+            info += f"已启用扩展：\n    {exts}"
+        else:
+            info = info[:-1]
+        showinfo("地图信息",info)
 
     def change_chess_height(self):
         for i in self.chess_btn:
             for j in i:
                 if j["height"] == 3: # 大棋子
                     j["height"] = 2
                     j["width"] = 5
@@ -186,20 +191,68 @@
             self.chess_btn[self.getx(i[0])][self.gety(i[1])]["bg"] = static_data["colors"][bg]
 
     def refresh_map(self):
         for i in range(self.map_data.rl):
             for j in range(self.map_data.cl):
                 chess = self.map_data.chessboard[self.getx(i)][self.gety(j)]
                 if chess:
-                    self.chess_btn[i][j]["text"] = chess.text(self.belong == 2)
-                    self.chess_btn[i][j]["fg"] = chess.fg
+                    text,fg = self.get_chess_text(chess)
+                    self.chess_btn[i][j]["text"] = text
+                    self.chess_btn[i][j]["fg"] = fg
                 else:
                     self.chess_btn[i][j]["text"] = ""
                 self.chess_btn[i][j]["bg"] = static_data["colors"]["chess-bg"]
 
+    # 在按钮上显示的文字及颜色
+    def get_chess_text(self,chess):
+        can_go_prompt = list[str]()
+        now_move = chess.now_move # 先赋值中间变量，避免调用self.now_move属性时重新计算
+        for i in range(1,9):
+            is_add = False
+            for j,k in enumerate(now_move):
+                if i in k:
+                    can_go_prompt.append(self.can_go_prompt_list[j])
+                    is_add = True
+                    break
+            if not is_add:
+                can_go_prompt.append(" ")
+        if self.belong == 2: # 反方棋盘
+            can_go_prompt.reverse()
+        # 生成名字
+        name_withspace = chess.name
+        name_length = len(chess.name.encode(encoding = "gbk"))
+        side = True # True为右侧
+        while name_length < 6:
+            if side:
+                name_withspace += " "
+            else:
+                name_withspace = " " + name_withspace
+            side = not side
+            name_length += 1
+        can_go_prompt.insert(4,name_withspace)
+        # 合并空格
+        text = ""
+        whitespace = ["   ","   ","\n","","","\n","   ","   ",""]
+        for i in range(9):
+            text += (can_go_prompt[i] + whitespace[i])
+        # 设置颜色
+        if chess.belong == 1:
+            if chess.is_tran or not chess.tran_con:
+                fg = "red-tran-chess-fg"
+            else:
+                fg = "red-chess-fg"
+        elif chess.belong == 2:
+            if chess.is_tran or not chess.tran_con:
+                fg = "blue-tran-chess-fg"
+            else:
+                fg = "blue-chess-fg"
+        else:
+            fg = "neutral-chess-fg"
+        return text,static_data["colors"][fg]
+
 class SettingWindow(tk.Tk):
     def __init__(self,add_ext_func,refresh_ext_func):
         super().__init__()
         self.title("设置")
         self.minsize(480,360)
         self.resizable(width = False,height = False)
         self.main_frame = tk.Frame(self) # 解决布局分布在两侧的问题
```

### Comparing `s27a_jbq-1.0.0/src/s27a_jbq.egg-info/PKG-INFO` & `s27a_jbq-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,14 @@
-Metadata-Version: 2.1
-Name: s27a-jbq
-Version: 1.0.0
-Summary: A simple chess game
-Author-email: amf <xyf081202@163.com>
-Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
-Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.0-blue)
+![](https://img.shields.io/badge/release-1.0.1-blue)
 ![](https://img.shields.io/badge/last%20commit-may-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
-精班棋是一款自由度很高的将棋
+精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
 
 # 目录
 
@@ -32,37 +18,37 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您需要一个`Python 3`环境
-
 您可以从[这里](https://github.com/amf14151/s27a_jbq/archive/refs/heads/main.zip)直接下载文件并自行安装，或使用以下指令来安装
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
+在安装`s27a_jbq`模块后，建立一个`.py`文件并使用以下代码来构建游戏文件夹
 
 ``` python
 from s27a_jbq import generate_game
 
 generate_game(
    game_path = "JBQ", # 游戏文件夹位置
-   record_path = None, # 棋局记录位置，使用相对路径时根目录为游戏文件夹路径
+   record_path = None, # 棋局记录位置，格式为.csv，使用相对路径时根目录为游戏文件夹路径
    display = "window" # 游戏打开方式，'window'为窗口模式
 )
 ```
 
-也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
+您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
 
 ``` python
+from s27a_jbq.game import App
+
 def main():
    app = App()
    app.run()
 ```
 
 在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
@@ -78,17 +64,21 @@
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
 
 一些棋子在不同的位置会有不同的可移动格子，每个棋子的具体可移动格子根据地图、扩展决定
 
+在对局结束后，如果设置了`record_path`，则会在文件夹中创建同名文件，格式为`.csv`
+
 ## 地图
 
-地图文件是`.xlsx`文件，其中包含3个表，分别对应棋子、棋盘与特殊规则
+地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
+
+地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
 您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图
 
 下文介绍了地图文件的构造以及自定义地图的方法
 
 ### 棋盘构造
 
@@ -325,8 +315,8 @@
 - `check_can_go`：函数
 - `after_move`：函数
 
 # 许可证
 
 [(返回目录)](#目录)
 
-[MIT License](./LICENSE)
+[MIT License](https://github.com/amf14151/s27a_jbq/blob/main/LICENSE)
```

