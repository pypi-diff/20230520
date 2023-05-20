# Comparing `tmp/hagworm-5.5.3.tar.gz` & `tmp/hagworm-5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.3.tar", last modified: Fri May 19 06:03:20 2023, max compression
+gzip compressed data, was "hagworm-5.5.4.tar", last modified: Sat May 20 03:16:49 2023, max compression
```

## Comparing `hagworm-5.5.3.tar` & `hagworm-5.5.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.990197 hagworm-5.5.3/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.3/LICENSE
--rw-rw-rw-   0        0        0     7515 2023-05-19 06:03:20.990197 hagworm-5.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.874195 hagworm-5.5.3/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.3/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.878196 hagworm-5.5.3/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.884197 hagworm-5.5.3/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.887196 hagworm-5.5.3/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.3/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.3/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.889198 hagworm-5.5.3/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.890196 hagworm-5.5.3/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.3/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.892196 hagworm-5.5.3/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-19 06:01:12.000000 hagworm-5.5.3/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.931195 hagworm-5.5.3/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.962195 hagworm-5.5.3/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.3/hagworm/extend/asyncio/etcd.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1570 2023-05-18 08:40:46.000000 hagworm-5.5.3/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.3/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.3/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.3/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.967194 hagworm-5.5.3/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.974198 hagworm-5.5.3/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.977196 hagworm-5.5.3/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.979195 hagworm-5.5.3/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.982235 hagworm-5.5.3/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.988195 hagworm-5.5.3/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.5.3/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.899196 hagworm-5.5.3/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7515 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      701 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 06:03:20.991196 hagworm-5.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2372 2023-05-19 05:58:06.000000 hagworm-5.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.729966 hagworm-5.5.4/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.4/LICENSE
+-rw-rw-rw-   0        0        0     7515 2023-05-20 03:16:49.728966 hagworm-5.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.623966 hagworm-5.5.4/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.4/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.626965 hagworm-5.5.4/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.632966 hagworm-5.5.4/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.635966 hagworm-5.5.4/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.4/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.4/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.637966 hagworm-5.5.4/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.638966 hagworm-5.5.4/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.4/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.4/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.640966 hagworm-5.5.4/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-20 02:40:17.000000 hagworm-5.5.4/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.676965 hagworm-5.5.4/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.704965 hagworm-5.5.4/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.4/hagworm/extend/asyncio/etcd.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.4/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.4/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.4/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.4/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.707965 hagworm-5.5.4/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.715004 hagworm-5.5.4/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.4/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.717995 hagworm-5.5.4/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.718965 hagworm-5.5.4/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.721965 hagworm-5.5.4/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.727965 hagworm-5.5.4/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.4/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.4/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.4/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.4/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:16:49.647966 hagworm-5.5.4/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7515 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      723 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 03:16:49.000000 hagworm-5.5.4/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:16:49.729966 hagworm-5.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     2407 2023-05-20 02:38:55.000000 hagworm-5.5.4/setup.py
```

### Comparing `hagworm-5.5.3/LICENSE` & `hagworm-5.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/PKG-INFO` & `hagworm-5.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.3
+Version: 5.5.4
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.3/README.md` & `hagworm-5.5.4/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/c_extend/math.c` & `hagworm-5.5.4/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.5.4/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/example/fastapi_demo/main.py` & `hagworm-5.5.4/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.4/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/example/fastapi_demo/setting.py` & `hagworm-5.5.4/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/example/main_test.py` & `hagworm-5.5.4/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/base.py` & `hagworm-5.5.4/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.4/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/command.py` & `hagworm-5.5.4/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/etcd.py` & `hagworm-5.5.4/hagworm/extend/asyncio/etcd.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/event.py` & `hagworm-5.5.4/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/file.py` & `hagworm-5.5.4/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/future.py` & `hagworm-5.5.4/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.4/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.4/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.4/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/net.py` & `hagworm-5.5.4/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.4/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/pool.py` & `hagworm-5.5.4/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.4/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.4/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/task.py` & `hagworm-5.5.4/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.4/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/asyncio/zmq.py` & `hagworm-5.5.4/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/base.py` & `hagworm-5.5.4/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/cache.py` & `hagworm-5.5.4/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/compile.py` & `hagworm-5.5.4/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/config.py` & `hagworm-5.5.4/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/crypto.py` & `hagworm-5.5.4/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/error.py` & `hagworm-5.5.4/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/event.py` & `hagworm-5.5.4/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/igraph.py` & `hagworm-5.5.4/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/interface.py` & `hagworm-5.5.4/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/logging.py` & `hagworm-5.5.4/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/media.py` & `hagworm-5.5.4/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/metaclass.py` & `hagworm-5.5.4/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/process.py` & `hagworm-5.5.4/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/qrcode.py` & `hagworm-5.5.4/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/struct.py` & `hagworm-5.5.4/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/text.py` & `hagworm-5.5.4/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/trace.py` & `hagworm-5.5.4/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/transaction.py` & `hagworm-5.5.4/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/extend/validator.py` & `hagworm-5.5.4/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/fastapi/base.py` & `hagworm-5.5.4/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/fastapi/field.py` & `hagworm-5.5.4/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/fastapi/model.py` & `hagworm-5.5.4/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/fastapi/response.py` & `hagworm-5.5.4/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/gunicorn.py` & `hagworm-5.5.4/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/frame/stress_tests.py` & `hagworm-5.5.4/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/static/cacert.pem` & `hagworm-5.5.4/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/third/consul/config.py` & `hagworm-5.5.4/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.4/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.4/hagworm/third/rabbitmq/publish.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,45 +116,42 @@
 
     def __init__(self, url, pool_size, *, connection_config=None):
 
         self._mq_url = url
 
         self._connection_config = connection_config if connection_config else {}
 
-        self._connections: List[RabbitMQProducer] = []
-
         super().__init__(pool_size)
 
-    def _create_obj(self):
+    async def _create_obj(self):
 
         connection = RabbitMQProducer(self._mq_url, **self._connection_config)
 
-        self._connections.append(connection)
-
         return connection
 
+    async def _delete_obj(self, obj):
+
+        await obj.close()
+
     async def connect(
             self, *,
             publisher_confirms: bool = True, on_return_raises: bool = False,
             timeout: aio_pika.abc.TimeoutType = None
     ):
 
-        for connection in self._connections:
-            await connection.connect(
-                publisher_confirms=publisher_confirms,
-                on_return_raises=on_return_raises,
-                timeout=timeout,
-            )
-
-        Utils.log.info(f'rabbitmq producer pool connected: {self._queue.qsize()}')
+        await self.open()
 
-    async def close(self):
+        for _ in range(self._queue.qsize()):
 
-        for connection in self._connections:
-            await connection.close()
+            with self.get_nowait() as connection:
+                await connection.connect(
+                    publisher_confirms=publisher_confirms,
+                    on_return_raises=on_return_raises,
+                    timeout=timeout,
+                )
 
     async def publish(self, message, routing_key=r'', **kwargs):
 
         async with self.get() as connection:
             return await connection.publish(
                 message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
                 routing_key, **kwargs
@@ -172,15 +169,13 @@
 
         self._exchange_name = exchange_name
         self._exchange_type = exchange_type
         self._exchange_config = exchange_config
 
         super().__init__(url, pool_size, connection_config=connection_config)
 
-    def _create_obj(self):
+    async def _create_obj(self):
 
         connection = RabbitMQProducerForExchange(self._mq_url, **self._connection_config)
         connection.config(self._exchange_name, self._exchange_type, exchange_config=self._exchange_config)
 
-        self._connections.append(connection)
-
         return connection
```

### Comparing `hagworm-5.5.3/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.4/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.4/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.3
+Version: 5.5.4
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.3/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.4/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.3/hagworm.egg-info/requires.txt` & `hagworm-5.5.4/hagworm.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-APScheduler==3.9.1
-Pillow==9.0.1
-PyJWT==2.3.0
+APScheduler==3.10.1
+Pillow==9.5.0
+PyJWT==2.7.0
 PyYAML==6.0
-SQLAlchemy==1.3.24
+SQLAlchemy==2.0.14
 aredis==1.1.8
-aiohttp==3.8.1
+aiohttp==3.8.4
 aiomysql==0.1.1
-aiosmtplib==1.1.6
-aio-pika==8.0.3
-async-etcd3gw==0.6
-cachetools==5.0.0
-confluent-kafka==1.9.2
-cryptography==37.0.2
-fastapi==0.76.0
+aiosmtplib==2.0.1
+aio-pika==9.0.7
+async-etcd3gw==0.8
+cachetools==5.3.0
+confluent-kafka==2.1.1
+cryptography==40.0.2
+elasticsearch==8.1.1
+fastapi==0.95.2
 fastapi-health==0.4.0
 gunicorn==20.1.0
-hiredis==2.0.0
-httptools==0.4.0
+hiredis==2.2.3
+httptools==0.5.0
 igraph==0.10.4
-loguru==0.6.0
-motor==3.0.0
-msgpack==1.0.3
+loguru==0.7.0
+motor==3.1.2
+msgpack==1.0.5
 ntplib==0.4.0
-numpy==1.22.3
-psutil==5.9.0
-pyahocorasick==1.4.4
-pytest-asyncio==0.18.3
+numpy==1.24.3
+psutil==5.9.5
+pyahocorasick==2.0.0
+pytest-asyncio==0.21.0
 python-dateutil==2.8.2
-python-stdnum==1.17
+python-stdnum==1.18
 python-consul2==0.1.5
-python-multipart==0.0.5
-pyzmq==22.3.0
-qrcode==7.3.1
-texttable==1.6.4
-ujson==5.2.0
-uvicorn[standard]==0.17.6
+python-multipart==0.0.6
+pyzmq==25.0.2
+qrcode==7.4.2
+texttable==1.6.7
+ujson==5.7.0
+uvicorn[standard]==0.22.0
 xmltodict==0.13.0
 
 [:sys_platform != "win32"]
-uvloop==0.16.0
+uvloop==0.17.0
```

### Comparing `hagworm-5.5.3/setup.py` & `hagworm-5.5.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,52 +24,53 @@
     long_description=long_description,
     long_description_content_type=r'text/markdown',
     url=r'https://gitee.com/wsb310/hagworm',
     packages=setuptools.find_packages(),
     package_data={r'hagworm': [r'static/*.*']},
     python_requires=r'>=3.9, <3.10',
     install_requires=[
-        r'APScheduler==3.9.1',
-        r'Pillow==9.0.1',
-        r'PyJWT==2.3.0',
+        r'APScheduler==3.10.1',
+        r'Pillow==9.5.0',
+        r'PyJWT==2.7.0',
         r'PyYAML==6.0',
-        r'SQLAlchemy==1.3.24',
+        r'SQLAlchemy==2.0.14',
         r'aredis==1.1.8',
-        r'aiohttp==3.8.1',
+        r'aiohttp==3.8.4',
         r'aiomysql==0.1.1',
-        r'aiosmtplib==1.1.6',
-        r'aio-pika==8.0.3',
-        r'async-etcd3gw==0.6',
-        r'cachetools==5.0.0',
-        r'confluent-kafka==1.9.2',
-        r'cryptography==37.0.2',
-        r'fastapi==0.76.0',
+        r'aiosmtplib==2.0.1',
+        r'aio-pika==9.0.7',
+        r'async-etcd3gw==0.8',
+        r'cachetools==5.3.0',
+        r'confluent-kafka==2.1.1',
+        r'cryptography==40.0.2',
+        r'elasticsearch==8.1.1',
+        r'fastapi==0.95.2',
         r'fastapi-health==0.4.0',
         r'gunicorn==20.1.0',
-        r'hiredis==2.0.0',
-        r'httptools==0.4.0',
+        r'hiredis==2.2.3',
+        r'httptools==0.5.0',
         r'igraph==0.10.4',
-        r'loguru==0.6.0',
-        r'motor==3.0.0',
-        r'msgpack==1.0.3',
+        r'loguru==0.7.0',
+        r'motor==3.1.2',
+        r'msgpack==1.0.5',
         r'ntplib==0.4.0',
-        r'numpy==1.22.3',
-        r'psutil==5.9.0',
-        r'pyahocorasick==1.4.4',
-        r'pytest-asyncio==0.18.3',
+        r'numpy==1.24.3',
+        r'psutil==5.9.5',
+        r'pyahocorasick==2.0.0',
+        r'pytest-asyncio==0.21.0',
         r'python-dateutil==2.8.2',
-        r'python-stdnum==1.17',
+        r'python-stdnum==1.18',
         r'python-consul2==0.1.5',
-        r'python-multipart==0.0.5',
-        r'pyzmq==22.3.0',
-        r'qrcode==7.3.1',
-        r'texttable==1.6.4',
-        r'ujson==5.2.0',
-        r'uvicorn[standard]==0.17.6',
-        r'uvloop==0.16.0;sys_platform!="win32"',
+        r'python-multipart==0.0.6',
+        r'pyzmq==25.0.2',
+        r'qrcode==7.4.2',
+        r'texttable==1.6.7',
+        r'ujson==5.7.0',
+        r'uvicorn[standard]==0.22.0',
+        r'uvloop==0.17.0;sys_platform!="win32"',
         r'xmltodict==0.13.0',
     ],
     classifiers=[
         r'Programming Language :: Python :: 3.8',
         r'License :: OSI Approved :: Apache Software License',
         r'Operating System :: POSIX :: Linux',
     ],
```

