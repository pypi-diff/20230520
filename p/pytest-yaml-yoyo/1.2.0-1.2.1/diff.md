# Comparing `tmp/pytest-yaml-yoyo-1.2.0.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.0.tar", last modified: Mon May  8 00:53:51 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.1.tar", last modified: Fri May 19 16:30:43 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.0.tar` & `pytest-yaml-yoyo-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.287394 pytest-yaml-yoyo-1.2.0/
--rw-rw-rw-   0        0        0    21942 2023-05-08 00:53:51.286394 pytest-yaml-yoyo-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    21443 2022-12-14 00:24:42.000000 pytest-yaml-yoyo-1.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-08 00:53:51.287394 pytest-yaml-yoyo-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-08 00:50:03.000000 pytest-yaml-yoyo-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.251592 pytest-yaml-yoyo-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.277442 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     3741 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0      991 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     8780 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4122 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    26263 2023-05-08 00:53:10.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3380 2023-05-08 00:50:48.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-05-08 00:53:51.285397 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    21942 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 00:53:51.000000 pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/
+-rw-rw-rw-   0        0        0    23645 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    23146 2023-05-19 16:29:16.000000 pytest-yaml-yoyo-1.2.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-19 16:29:16.000000 pytest-yaml-yoyo-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.963861 pytest-yaml-yoyo-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.987797 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9257 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28442 2023-05-19 16:19:35.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3524 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.995775 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    23645 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.0/PKG-INFO` & `pytest-yaml-yoyo-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.0
+Version: 1.2.1
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -112,23 +112,78 @@
 
 - 1.config.py 实现多环境配置
 - 2.支持mysql 数据库操作
 
 v1.1.1 发布时间 2022.12.14
 
 钉钉机器人通知测试结果
-- 1.config.py 配置钉钉机器人
-- 2.支持mysql requests_function和requests_module 内置fixture功能
+
+- 1.config.py 配置钉钉机器人access_token
+- 2.测试结果钉钉群通知
+- 3.支持 requests_function 和 requests_module 内置 fixture 切换
+
+v1.1.2 发布时间 2022.12.16
+
+内置方法提供
+
+- 1.提供3个常用的内置函数：current_time， rand_value， rand_str
+- 2.一个内置fake对象
+- 3.修复yaml文件为空或格式不正确时，执行报错的问题
+
+v1.1.3 发布时间 2022.12.17
+
+- 文件上传multipart/form-data 格式支持
+
+v1.1.4 发布时间 2023.2.13
+
+新增3个关键字
+- 1.sleep  添加用例之间的sleep 等待时间
+- 2.skip   跳过用例功能
+- 3.skipif   条件为真时跳过用例
+
+v1.1.5 发布时间 2023.2.16
+
+支持 2 中方式生成 yaml 用例
+- 1.本地 swagger.json 文件
+- 2.在线 swagger.json 地址
+
+v1.1.8 发布时间 2023.3.17
+
+int 转 str 类型
+
+v1.1.9 发布时间 2023-03-21
+
+做了以下优化
+- 1.validate 校验加了text 关键字获取全部body文本内容
+- 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
+- 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
+- 4.log 日志文件优化，只保留最近的5个日志文件
+
+v1.2.0 发布时间 2023-05-08
+
+优化以下问题
+- 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
+- 2.添加局部变量variables
+- 3.优化request 下的hook 功能
+- 4.其它细节优化
+
+v1.2.1 发布
+
+1.兼容python3.8, python3.9, python3.10版本
+2.支持在case 用例中针对单个用例的参数化了
+3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+5.内置to_json() 函数，字典转 json
 
 Installation / 安装
 --------------------------
-最近环境体验
+最佳环境体验
 
-- Python 3.8 版本
-- Pytest 7.2.0 最新版
+- Python 3.8, 3.9. 3.10 版本
+- Pytest 7.2.0+
 
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
```

### Comparing `pytest-yaml-yoyo-1.2.0/README.rst` & `pytest-yaml-yoyo-1.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -97,23 +97,78 @@
 
 - 1.config.py 实现多环境配置
 - 2.支持mysql 数据库操作
 
 v1.1.1 发布时间 2022.12.14
 
 钉钉机器人通知测试结果
-- 1.config.py 配置钉钉机器人
-- 2.支持mysql requests_function和requests_module 内置fixture功能
+
+- 1.config.py 配置钉钉机器人access_token
+- 2.测试结果钉钉群通知
+- 3.支持 requests_function 和 requests_module 内置 fixture 切换
+
+v1.1.2 发布时间 2022.12.16
+
+内置方法提供
+
+- 1.提供3个常用的内置函数：current_time， rand_value， rand_str
+- 2.一个内置fake对象
+- 3.修复yaml文件为空或格式不正确时，执行报错的问题
+
+v1.1.3 发布时间 2022.12.17
+
+- 文件上传multipart/form-data 格式支持
+
+v1.1.4 发布时间 2023.2.13
+
+新增3个关键字
+- 1.sleep  添加用例之间的sleep 等待时间
+- 2.skip   跳过用例功能
+- 3.skipif   条件为真时跳过用例
+
+v1.1.5 发布时间 2023.2.16
+
+支持 2 中方式生成 yaml 用例
+- 1.本地 swagger.json 文件
+- 2.在线 swagger.json 地址
+
+v1.1.8 发布时间 2023.3.17
+
+int 转 str 类型
+
+v1.1.9 发布时间 2023-03-21
+
+做了以下优化
+- 1.validate 校验加了text 关键字获取全部body文本内容
+- 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
+- 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
+- 4.log 日志文件优化，只保留最近的5个日志文件
+
+v1.2.0 发布时间 2023-05-08
+
+优化以下问题
+- 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
+- 2.添加局部变量variables
+- 3.优化request 下的hook 功能
+- 4.其它细节优化
+
+v1.2.1 发布
+
+1.兼容python3.8, python3.9, python3.10版本
+2.支持在case 用例中针对单个用例的参数化了
+3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+5.内置to_json() 函数，字典转 json
 
 Installation / 安装
 --------------------------
-最近环境体验
+最佳环境体验
 
-- Python 3.8 版本
-- Pytest 7.2.0 最新版
+- Python 3.8, 3.9. 3.10 版本
+- Pytest 7.2.0+
 
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
```

### Comparing `pytest-yaml-yoyo-1.2.0/setup.py` & `pytest-yaml-yoyo-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.0',
+    version='v1.2.1',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
@@ -28,15 +28,15 @@
     python_requires=">=3.8",
     install_requires=[
         'Jinja2>=3.1.2',
         'jmespath>=0.9.5',
         'jsonpath>=0.82',
         'pytest>=7.2.0',
         'PyYAML>=6.0',
-        'requests==2.18.4',
+        'requests>=2.18.4',
         'allure-pytest>=2.12.0',
         'pymysql>=1.0.2',
         'DingtalkChatbot>=1.5.7',
         'Faker>=15.3.4',
         'requests_toolbelt>=0.10.1',
     ],
     entry_points={
```

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,17 +95,25 @@
         run.run()  # 执行用例
         # 重写属性
         py_module._getobj = lambda: module  # noqa
         return py_module
 
 
 def pytest_generate_tests(metafunc):  # noqa
-    """测试用例参数化功能实现"""
-    if hasattr(metafunc.module, 'params_data'):
-        params_data = getattr(metafunc.module, 'params_data')
+    """测试用例参数化功能实现
+    :param metafunc:共有五个属性值
+         metafunc.fixturenames:参数化收集时的参数名称
+         metafunc.module:使用参数名称进行参数化的测试用例所在的模块d对象
+         metafunc.config:测试用例会话
+         metafunc.function:测试用例对象,即函数或方法对象
+         metafunc.cls: 测试用例所属的类的类对象
+    :return: none
+    """
+    if hasattr(metafunc.module, f'{metafunc.function.__qualname__}_params_data'):
+        params_data = getattr(metafunc.module, f'{metafunc.function.__qualname__}_params_data')
         params_len = 0    # 参数化 参数的个数
         if isinstance(params_data, list):
             if isinstance(params_data[0], list):
                 params_len = len(params_data[0])
             elif isinstance(params_data[0], dict):
                 params_len = len(params_data[0].keys())
             else:
```

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import json
 
 
 class RunYaml(object):
     """ 运行yaml """
 
     def __init__(self, raw: dict, module: types.ModuleType, g: dict):
-        self.raw = raw   # 读取yaml 原始数据
-        self.module = module   # 动态创建的 module 模型
+        self.raw = raw  # 读取yaml 原始数据
+        self.module = module  # 动态创建的 module 模型
         self.module_variable = {}  # 模块变量
         self.context = {}
         self.hooks = {}  # 全局hooks
         self.g = g  # 全局配置
 
     def run(self):
         if not self.raw.get('config'):
@@ -51,24 +51,44 @@
         if isinstance(self.module_variable, dict):
             self.context.update(self.module_variable)
         # 支持 2 种参数化格式数据
         config_params = render_template_obj.rend_template_any(config_params, **self.context)
         config_fixtures = render_template_obj.rend_template_any(config_fixtures, **self.context)
         config_fixtures, config_params = self.parameters_date(config_fixtures, config_params)
         case = {}  # 收集用例名称和执行内容
+
         for case_name, case_value in self.raw.items():
+            case_fixtures = []
+            case_params = []
             if case_name == 'config':
                 continue  # 跳过config 非用例部分
             # case_name 必须 test 开头
             if not str(case_name).startswith('test'):
-                case_name = 'test_'+str(case_name)
+                case_name = 'test_' + str(case_name)
             if isinstance(case_value, list):
                 case[case_name] = case_value
             else:
                 case[case_name] = [case_value]
+            # 用例参数获取
+            if len(case[case_name]) < 1:
+                log.debug('test case not item to run !')
+            else:
+                log.info(f'--------{case[case_name]}')
+                if 'fixtures' in case[case_name][0]:
+                    case_raw_fixtures = case[case_name][0].get('fixtures', [])
+                    case_fixtures = render_template_obj.rend_template_any(case_raw_fixtures, **self.context)
+                if "parameters" in case[case_name][0]:
+                    log.info('parameters 参数化执行用例')
+                    case_raw_parameters = case[case_name][0].get('parameters', [])
+                    # case_raw_fixtures = case[case_name][0].get('fixtures', [])
+                    # 支持 2 种参数化格式数据
+                    case_params = render_template_obj.rend_template_any(case_raw_parameters, **self.context)
+                    # case_fixtures = render_template_obj.rend_template_any(case_raw_fixtures, **self.context)
+                    # case 中的参数化 覆盖 config 的参数化
+                case_fixtures, case_params = self.parameters_date(case_fixtures, case_params)
 
             def execute_yaml_case(args):
                 # 获取被调用函数名称
                 log.info(f'执行文件-> {self.module.__name__}.yml')
                 log.info(f'base_url-> {base_url or args.get("request").config.option.base_url}')
                 log.info(f'config variables-> {self.module_variable}')
                 call_function_name = inspect.getframeinfo(inspect.currentframe().f_back)[2]
@@ -89,47 +109,52 @@
                     with allure.step(step_name):
                         pass
                     if 'validate' not in step.keys():
                         step['validate'] = []
                     for item, value in step.items():
                         # 执行用例里面的方法
                         if item == 'name':
-                            pass          # noqa
-                        elif item == 'variables':    # step 步骤变量获取
+                            pass  # noqa
+                        elif item == 'parameters':
+                            pass
+                        elif item == 'fixtures':
+                            pass
+                        elif item == 'variables':  # step 步骤变量获取
                             copy_value = copy.deepcopy(value)
                             if not isinstance(copy_value, dict):
                                 log.error('step variables->variables must be dict type!')
                             else:
                                 step_variables_value = render_template_obj.rend_template_any(
                                     copy_value, **self.context
                                 )
                                 step_context.update(step_variables_value)
                         elif item == 'api':
-                            root_dir = args.get('request').config.rootdir   # 内置request 获取root_dir
+                            root_dir = args.get('request').config.rootdir  # 内置request 获取root_dir
                             api_path = Path(root_dir).joinpath(value)
                             raw_api = yaml.safe_load(api_path.open(encoding='utf-8'))
                             api_validate = raw_api.get('validate', [])
                             copy_value = copy.deepcopy(raw_api.get('request'))  # 深拷贝一份新的value
                             response = self.run_request(args, copy_value, config_hooks, base_url, context=step_context)
                         elif item == 'request':
                             copy_value = copy.deepcopy(value)  # 深拷贝一份新的value
                             copy_config_hooks = copy.deepcopy(config_hooks)
-                            response = self.run_request(args, copy_value, copy_config_hooks, base_url, context=step_context)
+                            response = self.run_request(args, copy_value, copy_config_hooks, base_url,
+                                                        context=step_context)
                         elif item == 'extract':
                             # 提取变量
                             copy_value = copy.deepcopy(value)
                             extract_value = render_template_obj.rend_template_any(copy_value, **step_context)
                             extract_result = self.extract_response(response, extract_value)
                             log.info(f'extract  提取变量-> {extract_result}')
                             # 添加到模块变量
                             self.module_variable.update(extract_result)
                             # 添加到步骤变量
                             step_context.update(extract_result)
                             if isinstance(self.module_variable, dict):
-                                self.context.update(self.module_variable)    # 加载模块变量
+                                self.context.update(self.module_variable)  # 加载模块变量
                         elif item == 'validate':
                             copy_value = copy.deepcopy(value)
                             # 合并校验
                             copy_value.extend([v for v in api_validate if v not in copy_value])
                             validate_value = render_template_obj.rend_template_any(copy_value, **step_context)
                             log.info(f'validate 校验内容-> {validate_value}')
                             self.validate_response(response, validate_value)
@@ -140,41 +165,46 @@
                                 time.sleep(sleep_value)
                             except Exception as msg:
                                 log.error(f'Run error: sleep value must be int or float, error msg: {msg}')
                         elif item == 'skip':
                             skip_reason = render_template_obj.rend_template_any(value, **step_context)
                             import pytest
                             pytest.skip(skip_reason)
-                        elif item == 'skipif':   # noqa
+                        elif item == 'skipif':  # noqa
                             if_exp = render_template_obj.rend_template_any(value, **step_context)
                             log.info(f'skipif : {eval(str(if_exp))}')  # noqa
                             if eval(str(if_exp)):
                                 import pytest
                                 pytest.skip(str(if_exp))
                         else:
                             value = render_template_obj.rend_template_any(value, **step_context)
                             try:
                                 eval(item)(value)
                             except Exception as msg:
                                 raise exceptions.ParserError(f'Parsers error: {msg}') from None
-
+            fun_fixtures = []
+            # 合并config 和 case 用例 fixtures
+            fun_fixtures.extend(config_fixtures)
+            [fun_fixtures.append(fixt) for fixt in case_fixtures if fixt not in fun_fixtures]
+            # 参数化以 case 用例 优先
+            fun_params = case_params or config_params
             f = create_funtion.create_function_from_parameters(
                 func=execute_yaml_case,
                 # parameters 传内置fixture 和 用例fixture
-                parameters=self.function_parameters(config_fixtures),
+                parameters=self.function_parameters(fun_fixtures),
                 documentation=case_name,
                 func_name=case_name,
                 func_filename=f"{self.module.__name__}.py",
             )
 
             # 向 module 中加入函数
             setattr(self.module, str(case_name), f)
-            if config_params:
+            if fun_params:
                 # 向 module 中加参数化数据的属性
-                setattr(self.module, 'params_data', config_params)
+                setattr(self.module, f'{case_name}_params_data', fun_params)
 
     def run_request(self, args, copy_value, config_hooks, base_url, context=None):
         """运行request请求"""
         request_session = args.get('requests_function') or args.get('requests_module') or args.get('requests_session')
         # 加载参数化的值和fixture的值
         if context is None:
             request_value = render_template_obj.rend_template_any(copy_value, **self.context)
@@ -191,36 +221,37 @@
             self.run_request_hooks(request_pre, request_value, context=context)
         # request请求 带上hooks "response"参数
         self.response_hooks(config_hooks, request_value)
 
         # multipart/form-data 文件上传支持
         root_dir = args.get('request').config.rootdir  # 内置request 获取root_dir
         request_value = self.multipart_encoder_request(request_value, root_dir)
-
         log.info(f'--------  request info ----------')
-        log.info(f'raw    -> {request_value}')
-        log.debug(f'method -> {request_value.get("method", "")}')
-        log.debug(f'url    -> {request_value.get("url", "")}')
-        request_headers = request_session.headers
+        log.info(f'yml raw  -->: {request_value}')
+        log.info(f'method   -->: {request_value.get("method", "")}')
+        log.info(f'url      -->: {request_value.get("url", "")}')
+        request_headers = {}
+        request_headers.update(request_session.headers)
         if request_value.get("headers", {}):
             request_headers.update(request_value.get("headers", {}))
-        log.debug(f'headers-> {request_headers}')
+        log.info(f'headers  -->: {request_headers}')
         if request_value.get('json'):
-            log.debug(f'json   -> {json.dumps(request_value.get("json", {}))}')
+            log.info(f'json     -->: {json.dumps(request_value.get("json", {}))}')
         else:
-            log.debug(f'data   -> {request_value.get("data", {})}')
+            log.info(f'data     -->: {request_value.get("data", {})}')
         response = request_session.send_request(
             base_url=base_url,
             **request_value
         )
-        log.info(f'------  response info  {getattr(response, "status_code")} {getattr(response, "reason", "")}')
-        log.info(f'耗时: {getattr(response, "elapsed", "").total_seconds() if getattr(response, "elapsed", "") else ""}s')
-        log.debug(f'url: {getattr(response, "url", "")}')
-        log.debug(f'headers:{getattr(response, "headers", "")}')
-        log.info(f'text:  {getattr(response, "text", "")}')
+        log.info(f'------  response info  {getattr(response, "status_code")} {getattr(response, "reason", "")} ------ ')
+        log.info(f'耗时     <--: {getattr(response, "elapsed", "").total_seconds() if getattr(response, "elapsed", "") else ""}s')
+        log.info(f'url      <--: {getattr(response, "url", "")}')
+        log.info(f'headers  <--: {getattr(response, "headers", "")}')
+        log.info(f'cookies  <--: {dict(getattr(response, "cookies", {}))}')
+        log.info(f'raw text <--: {getattr(response, "text", "")}')
         return response
 
     @staticmethod
     def function_parameters(config_fixtures) -> list:
         """ 测试函数传 fixture """
         # 测试函数的默认请求参数
         function_parameters = [
@@ -444,39 +475,41 @@
                     validate.equals(actual_value, expect_value)
                 elif check_type in ["lt", "less_than"]:
                     validate.less_than(actual_value, expect_value)
                 elif check_type in ["le", "less_or_equals"]:
                     validate.less_than_or_equals(actual_value, expect_value)
                 elif check_type in ["gt", "greater_than"]:
                     validate.greater_than(actual_value, expect_value)
-                elif check_type in ["ne", "not_equal"]:
+                elif check_type in ["ne", "not_equal", "not_equal"]:
                     validate.not_equals(actual_value, expect_value)
-                elif check_type in ["str_eq", "string_equals"]:
+                elif check_type in ["str_eq", "str_equals", "string_equals", "string_equal"]:
                     validate.string_equals(actual_value, expect_value)
-                elif check_type in ["len_eq", "length_equal"]:
+                elif check_type in ["len_eq", "length_equal", "length_equals"]:
                     validate.length_equals(actual_value, expect_value)
                 elif check_type in ["len_gt", "length_greater_than"]:
                     validate.length_greater_than(actual_value, expect_value)
                 elif check_type in ["len_ge", "length_greater_or_equals"]:
                     validate.length_greater_than_or_equals(actual_value, expect_value)
                 elif check_type in ["len_lt", "length_less_than"]:
                     validate.length_less_than(actual_value, expect_value)
                 elif check_type in ["len_le", "length_less_or_equals"]:
                     validate.length_less_than_or_equals(actual_value, expect_value)
-                elif check_type in ["contains"]:
+                elif check_type in ["contains", "contain"]:
                     validate.contains(actual_value, expect_value)
+                elif check_type in ["bool_eq", "bool_equal", "bool_equals"]:
+                    validate.bool_equals(actual_value, expect_value)
                 else:
                     if hasattr(validate, check_type):
                         getattr(validate, check_type)(actual_value, expect_value)
                     else:
                         log.error(f'{check_type}  not valid check type')
 
     def execute_mysql(self):
         """执行 mysql 操作"""
-        env_obj = self.g.get('env')    # 获取环境配置
+        env_obj = self.g.get('env')  # 获取环境配置
         if not hasattr(env_obj, 'MYSQL_HOST'):
             return {
                 "query_sql": lambda x: log.error("MYSQL_HOST not found in config.py"),
                 "execute_sql": lambda x: log.error("MYSQL_HOST not found in config.py")
             }
         try:
             db = ConnectMysql(
```

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,94 +3,98 @@
 """
 import re
 
 
 def equals(check_value, expect_value):
     check_value = None if check_value == 'None' else check_value
     expect_value = None if expect_value == 'None' else expect_value
-    assert check_value == expect_value, f'{check_value}->{type(check_value)} == {expect_value}->{type(expect_value)})'
+    assert check_value == expect_value, f'{check_value}->{type(check_value)} == {expect_value}->{type(expect_value)}'
 
 
 def less_than(check_value, expect_value):
-    assert check_value < expect_value, f'{check_value} < {expect_value})'
+    assert check_value < expect_value, f'{check_value} < {expect_value}'
 
 
 def less_than_or_equals(check_value, expect_value):
-    assert check_value <= expect_value, f'{check_value} <= {expect_value})'
+    assert check_value <= expect_value, f'{check_value} <= {expect_value}'
 
 
 def greater_than(check_value, expect_value):
-    assert check_value > expect_value, f'{check_value} > {expect_value})'
+    assert check_value > expect_value, f'{check_value} > {expect_value}'
 
 
 def greater_than_or_equals(check_value, expect_value):
-    assert check_value >= expect_value, f'{check_value} >= {expect_value})'
+    assert check_value >= expect_value, f'{check_value} >= {expect_value}'
 
 
 def not_equals(check_value, expect_value):
-    assert check_value != expect_value, f'{check_value} != {expect_value})'
+    assert check_value != expect_value, f'{check_value} != {expect_value}'
 
 
 def string_equals(check_value, expect_value):
-    assert str(check_value) == str(expect_value), f'{check_value} == {expect_value})'
+    assert str(check_value) == str(expect_value), f'{check_value} == {expect_value}'
 
 
 def length_equals(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(str(check_value)) == expect_len, f'{len(str(check_value))} == {expect_value})'
+    assert len(str(check_value)) == expect_len, f'{len(str(check_value))} == {expect_value}'
 
 
 def length_greater_than(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(check_value) > expect_len, f'{len(check_value)} > {expect_value})'
+    assert len(check_value) > expect_len, f'{len(check_value)} > {expect_value}'
 
 
 def length_greater_than_or_equals(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(check_value) >= expect_len, f'{len(check_value)} >= {expect_value})'
+    assert len(check_value) >= expect_len, f'{len(check_value)} >= {expect_value}'
 
 
 def length_less_than(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(check_value) < expect_len, f'{len(check_value)} < {expect_value})'
+    assert len(check_value) < expect_len, f'{len(check_value)} < {expect_value}'
 
 
 def length_less_than_or_equals(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(check_value) <= expect_len, f'{len(check_value)} <= {expect_value})'
+    assert len(check_value) <= expect_len, f'{len(check_value)} <= {expect_value}'
 
 
 def contains(check_value, expect_value):
     if isinstance(check_value, (list, tuple, dict, str)):
-        assert expect_value in check_value, f'{expect_value} in {check_value})'
+        assert expect_value in check_value, f'{expect_value} in {check_value}'
     else:
         # 数字类型包含
-        assert expect_value in str(check_value), f'{expect_value} in {check_value})'
+        assert expect_value in str(check_value), f'{expect_value} in {check_value}'
 
 
 def contained_by(check_value, expect_value):
     if isinstance(expect_value, (list, tuple, dict, str)):
-        assert check_value in expect_value, f'{check_value} in {expect_value})'
+        assert check_value in expect_value, f'{check_value} in {expect_value}'
     else:
         # 数字类型包含
-        assert str(check_value) in expect_value, f'{check_value} in {check_value})'
+        assert str(check_value) in expect_value, f'{check_value} in {check_value}'
 
 
 def regex_match(check_value, expect_value):
     assert isinstance(expect_value, str)
     assert isinstance(check_value, str)
     assert re.match(expect_value, check_value)
 
 
 def startswith(check_value, expect_value):
-    assert str(check_value).startswith(str(expect_value)), f'{str(check_value)} startswith {str(expect_value)})'
+    assert str(check_value).startswith(str(expect_value)), f'{str(check_value)} startswith {str(expect_value)}'
 
 
 def endswith(check_value, expect_value):
-    assert str(check_value).endswith(str(expect_value)), f'{str(check_value)} endswith {str(expect_value)})'
+    assert str(check_value).endswith(str(expect_value)), f'{str(check_value)} endswith {str(expect_value)}'
 
 
 def _cast_to_int(expect_value):
     try:
         return int(expect_value)
     except Exception:
-        raise AssertionError(f"%{expect_value} can't cast to int")
+        raise AssertionError(f"%{expect_value} can't cast to int")
+
+
+def bool_equals(check_value, expect_value):
+    assert bool(check_value) == bool(expect_value), f'{check_value} -> {bool(check_value)} == {expect_value}'
```

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.0
+Version: 1.2.1
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -112,23 +112,78 @@
 
 - 1.config.py 实现多环境配置
 - 2.支持mysql 数据库操作
 
 v1.1.1 发布时间 2022.12.14
 
 钉钉机器人通知测试结果
-- 1.config.py 配置钉钉机器人
-- 2.支持mysql requests_function和requests_module 内置fixture功能
+
+- 1.config.py 配置钉钉机器人access_token
+- 2.测试结果钉钉群通知
+- 3.支持 requests_function 和 requests_module 内置 fixture 切换
+
+v1.1.2 发布时间 2022.12.16
+
+内置方法提供
+
+- 1.提供3个常用的内置函数：current_time， rand_value， rand_str
+- 2.一个内置fake对象
+- 3.修复yaml文件为空或格式不正确时，执行报错的问题
+
+v1.1.3 发布时间 2022.12.17
+
+- 文件上传multipart/form-data 格式支持
+
+v1.1.4 发布时间 2023.2.13
+
+新增3个关键字
+- 1.sleep  添加用例之间的sleep 等待时间
+- 2.skip   跳过用例功能
+- 3.skipif   条件为真时跳过用例
+
+v1.1.5 发布时间 2023.2.16
+
+支持 2 中方式生成 yaml 用例
+- 1.本地 swagger.json 文件
+- 2.在线 swagger.json 地址
+
+v1.1.8 发布时间 2023.3.17
+
+int 转 str 类型
+
+v1.1.9 发布时间 2023-03-21
+
+做了以下优化
+- 1.validate 校验加了text 关键字获取全部body文本内容
+- 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
+- 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
+- 4.log 日志文件优化，只保留最近的5个日志文件
+
+v1.2.0 发布时间 2023-05-08
+
+优化以下问题
+- 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
+- 2.添加局部变量variables
+- 3.优化request 下的hook 功能
+- 4.其它细节优化
+
+v1.2.1 发布
+
+1.兼容python3.8, python3.9, python3.10版本
+2.支持在case 用例中针对单个用例的参数化了
+3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+5.内置to_json() 函数，字典转 json
 
 Installation / 安装
 --------------------------
-最近环境体验
+最佳环境体验
 
-- Python 3.8 版本
-- Pytest 7.2.0 最新版
+- Python 3.8, 3.9. 3.10 版本
+- Pytest 7.2.0+
 
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
```

### Comparing `pytest-yaml-yoyo-1.2.0/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

