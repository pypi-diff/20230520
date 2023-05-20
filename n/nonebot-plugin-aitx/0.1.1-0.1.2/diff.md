# Comparing `tmp/nonebot_plugin_aitx-0.1.1.tar.gz` & `tmp/nonebot_plugin_aitx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aitx-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_aitx-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_aitx-0.1.1.tar` & `nonebot_plugin_aitx-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1843 2023-05-20 01:04:43.511853 nonebot_plugin_aitx-0.1.1/nonebot-plugin-aitx/__init__.py
--rw-r--r--   0        0        0      438 2023-05-20 01:47:11.505444 nonebot_plugin_aitx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      348 2023-05-20 01:15:21.570060 nonebot_plugin_aitx-0.1.1/README.md
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 nonebot_plugin_aitx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1843 2023-05-20 01:04:43.511853 nonebot_plugin_aitx-0.1.2/nonebot-plugin-aitx/__init__.py
+-rw-r--r--   0        0        0      476 2023-05-20 01:55:29.092898 nonebot_plugin_aitx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-05-20 01:15:21.570060 nonebot_plugin_aitx-0.1.2/README.md
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 nonebot_plugin_aitx-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_aitx-0.1.1/nonebot-plugin-aitx/__init__.py` & `nonebot_plugin_aitx-0.1.2/nonebot-plugin-aitx/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aitx-0.1.1/PKG-INFO` & `nonebot_plugin_aitx-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-aitx
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于腾讯云接口的ai聊天
 Author: lcy
 Author-email: 863109569@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: tencentcloud-sdk-python (>=3.0.889,<4.0.0)
 Description-Content-Type: text/markdown
 
 # 用之前的准备：
     * pip install --upgrade tencentcloud-sdk-python
     * https://console.cloud.tencent.com/cam/capi
     * 在以上网址中获取你的腾讯云apikey,并填入到该插件的__init__.py文件指定位置中
 ## 该插件优先级为100，若前面所有插件都无法拦截消息，则会使用ai聊天进行处理。
```

