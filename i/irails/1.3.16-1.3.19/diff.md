# Comparing `tmp/irails-1.3.16.tar.gz` & `tmp/irails-1.3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.16.tar", last modified: Thu May 18 07:50:29 2023, max compression
+gzip compressed data, was "irails-1.3.19.tar", last modified: Sat May 20 12:05:31 2023, max compression
```

## Comparing `irails-1.3.16.tar` & `irails-1.3.19.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.665364 irails-1.3.16/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.16/MANIFEST.in
--rw-rw-rw-   0        0        0     5518 2023-05-18 07:50:29.664366 irails-1.3.16/PKG-INFO
--rw-rw-rw-   0        0        0     4734 2023-05-15 07:02:13.000000 irails-1.3.16/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.565266 irails-1.3.16/irails/
--rw-rw-rw-   0        0        0      307 2023-05-18 07:49:44.000000 irails-1.3.16/irails/__init__.py
--rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.16/irails/_i18n.py
--rw-rw-rw-   0        0        0     2873 2023-05-16 07:25:29.000000 irails-1.3.16/irails/_loader.py
--rw-rw-rw-   0        0        0     3545 2023-05-16 07:12:34.000000 irails-1.3.16/irails/_utils.py
--rw-rw-rw-   0        0        0    11909 2023-05-16 08:07:09.000000 irails-1.3.16/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.16/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.577236 irails-1.3.16/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.579231 irails-1.3.16/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.16/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.16/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.16/irails/cbv.py
--rw-rw-rw-   0        0        0     6118 2023-05-15 06:53:38.000000 irails-1.3.16/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.16/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24864 2023-05-18 07:46:03.000000 irails-1.3.16/irails/core.py
--rw-rw-rw-   0        0        0     7871 2023-05-18 07:46:03.000000 irails-1.3.16/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.16/irails/log.py
--rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.16/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.16/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.16/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.16/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.591864 irails-1.3.16/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.16/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.16/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6898 2023-05-14 13:32:08.000000 irails-1.3.16/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.16/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.16/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.16/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.16/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.16/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4042 2023-05-15 06:46:20.000000 irails-1.3.16/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2426 2023-05-15 07:00:43.000000 irails-1.3.16/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.525398 irails-1.3.16/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.605284 irails-1.3.16/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.16/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.16/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.16/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.16/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0      999 2023-05-14 14:07:15.000000 irails-1.3.16/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1014 2023-05-14 14:04:24.000000 irails-1.3.16/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.16/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.16/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.16/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.607279 irails-1.3.16/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.16/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.609278 irails-1.3.16/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.16/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.623236 irails-1.3.16/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.16/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.16/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.16/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.640190 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.16/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.16/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.16/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.16/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.530383 irails-1.3.16/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.644938 irails-1.3.16/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.16/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.648409 irails-1.3.16/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.16/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.16/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.651415 irails-1.3.16/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.534373 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.655392 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.660384 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.535371 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.662377 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.16/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.16/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.573248 irails-1.3.16/irails.egg-info/
--rw-rw-rw-   0        0        0     5518 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3088 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 07:50:29.665364 irails-1.3.16/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.120375 irails-1.3.19/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.19/MANIFEST.in
+-rw-rw-rw-   0        0        0     6172 2023-05-20 12:05:31.119084 irails-1.3.19/PKG-INFO
+-rw-rw-rw-   0        0        0     5388 2023-05-18 08:26:27.000000 irails-1.3.19/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.034384 irails-1.3.19/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-20 12:05:11.000000 irails-1.3.19/irails/__init__.py
+-rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.19/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2875 2023-05-19 11:46:57.000000 irails-1.3.19/irails/_loader.py
+-rw-rw-rw-   0        0        0     5073 2023-05-19 15:28:59.000000 irails-1.3.19/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.19/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.19/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.043361 irails-1.3.19/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.044363 irails-1.3.19/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.19/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.19/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.19/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.19/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.19/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.19/irails/core.py
+-rw-rw-rw-   0        0        0    13243 2023-05-20 11:48:25.000000 irails-1.3.19/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.19/irails/log.py
+-rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.19/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.19/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.19/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.19/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.056327 irails-1.3.19/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.19/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.19/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.19/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.19/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.19/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.19/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.19/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.19/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4130 2023-05-20 08:45:35.000000 irails-1.3.19/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2431 2023-05-20 09:01:43.000000 irails-1.3.19/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:30.999179 irails-1.3.19/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.068294 irails-1.3.19/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.19/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.19/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.19/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.19/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.19/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      658 2023-05-20 10:49:39.000000 irails-1.3.19/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.19/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.19/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.19/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.070289 irails-1.3.19/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.19/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.071286 irails-1.3.19/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.19/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.082257 irails-1.3.19/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.19/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.19/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.19/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.097216 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.19/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.19/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.19/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.19/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.004584 irails-1.3.19/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.100208 irails-1.3.19/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.19/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.104198 irails-1.3.19/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.19/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.19/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.107116 irails-1.3.19/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.008129 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.109110 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.114099 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.009126 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.117092 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.19/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.19/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.040368 irails-1.3.19/irails.egg-info/
+-rw-rw-rw-   0        0        0     6172 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 12:05:31.120375 irails-1.3.19/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.19/setup.py
```

### Comparing `irails-1.3.16/PKG-INFO` & `irails-1.3.19/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.16
+Version: 1.3.19
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,17 +18,18 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # irails
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
-[Docs](https://irails.2rails.cn/) 
+[Online Docs](https://irails.2rails.cn/) 
 # Welcome to IRAILS(python on rails)
-
+IRAILS is not just an ordinary imitation of Ruby on rails, but based on the characteristics of the Python language itself, combined with rich Python class libraries, it refuses to create wheels repeatedly, and can achieve web development with minimal code and configuration, making Python web development fast and powerful, and can be easily deployed on various platforms.
+The design concept of IRails refers to some RORs, but it has its own soul. It does not pursue the ultimate configuration and development, but rather appropriate configuration and development. Currently, it is in a preview version and will continue to improve in the future.
  
 
 ## Installation  
 
 * `pip install irails` - install irails
 
 ## Commands
```

### Comparing `irails-1.3.16/README.md` & `irails-1.3.19/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # irails
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
-[Docs](https://irails.2rails.cn/) 
+[Online Docs](https://irails.2rails.cn/) 
 # Welcome to IRAILS(python on rails)
-
+IRAILS is not just an ordinary imitation of Ruby on rails, but based on the characteristics of the Python language itself, combined with rich Python class libraries, it refuses to create wheels repeatedly, and can achieve web development with minimal code and configuration, making Python web development fast and powerful, and can be easily deployed on various platforms.
+The design concept of IRails refers to some RORs, but it has its own soul. It does not pursue the ultimate configuration and development, but rather appropriate configuration and development. Currently, it is in a preview version and will continue to improve in the future.
  
 
 ## Installation  
 
 * `pip install irails` - install irails
 
 ## Commands
```

### Comparing `irails-1.3.16/irails/_i18n.py` & `irails-1.3.19/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/_loader.py` & `irails-1.3.19/irails/_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         module_name = f"{app_dir}.{m}"
         _log.info(_('Loading module:%s')%module_name)
         try:
             importlib.import_module(module_name) 
             if m=='controllers':
                 cnt += 1
         except ImportError as e:
-            if m=='controllers':
+            if m:#=='controllers':
                 _log.error(_("load app %s failed")%app_dir)
                 _log.error(e.args)
                 cnt -= 1
             else:
                 pass
     return cnt
 def _load_apps(debug=False,do_load:bool=True):
```

### Comparing `irails-1.3.16/irails/_utils.py` & `irails-1.3.19/irails/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,25 +7,71 @@
 controller_re = re.compile("([\\w]+)Controller")
 
 _pluralizer = None
 def get_controller_name(controller_name):
     return controller_re.match(controller_name).group(1)
  
 def to_camel_case(x):
-    """转大驼峰法命名"""
+    """
+    Converts variable_name to camel case notation.
+    """
+    # Using the regex module to find all instances of an underscore followed by a letter
+    # and then replacing that underscore with the uppercase of that letter.
+    # Example: hello_world -> HelloWorld
     s = re.sub('_([a-zA-Z])', lambda m: (m.group(1).upper()), x )
     return s[0].upper() + s[1:]
-def get_plural_name(name:str):
+def __init_inflect():
     import inflect
     global _pluralizer
     if not _pluralizer:
-        _pluralizer = inflect.engine()
+        _pluralizer=inflect.engine()
+     
+    return _pluralizer
+def get_plural_name(name:str):
+    """
+        Return the plural of text, where text is a noun.
+
+        If count supplied, then return text if count is one of:
+            1, a, an, one, each, every, this, that
+
+        otherwise return the plural.
+
+        Whitespace at the start and end is preserved.
+
+    """
+    _pluralizer = __init_inflect()
     return _pluralizer.plural(name)
+def get_singularize_name(name:str):
+    """
+    Return the singular of text, where text is a plural noun.
+
+        If count supplied, then return the singular if count is one of:
+            1, a, an, one, each, every, this, that or if count is None
+
+        otherwise return text unchanged.
+
+        Whitespace at the start and end is preserved.
+
+        >>> p = engine()
+        >>> p.singular_noun('horses')
+        'horse'
+        >>> p.singular_noun('knights')
+        'knight'
+    """
+    _pluralizer = __init_inflect()
+    return _pluralizer.singular_noun(name)
 
 def get_snaked_name(_name:str):
+    """
+    Converts a string to snake_case format.
+    :param name: string to be converted
+    :return: the string in snake_case format
+    """
+    # split the string at every occurrence of a capital letter that is not at the beginning of the string
+    # and insert "_" in between each splitted portion
     return snake_case_re.sub("_", _name).lower()
 def is_valid_filename(filename):
     if filename is None or len(filename) == 0:
         return False
     if len(filename) > 200:
         return False
     illegal_chars = set('/\\?%*:|"<>')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `irails-1.3.16/irails/auth.py` & `irails-1.3.19/irails/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 from ._i18n import _
 AUTH_EXPIRED='[EXPIRED]!'
 
+ 
 _session_name:str = ""
 
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
         self.enforcer = enforcer
         self.__session_name = _session_name = session_name
@@ -39,22 +40,25 @@
         if self.enforcer:
             if authorize:
                 return self.enforcer.add_policy(sub,obj,act)
             else:
                 return self.enforcer.remove_policy(sub,obj,act)
         raise RuntimeError("Casbin Enforcer is None")
     
-    def _auth(self,request:Request,username:str):
+    def _auth(self,request:Request,username):
         '''
         do verity,return True means `Success` and others `Failed`
         '''
         path = request.url.path
         method = request.method   
         if username:
-            user = username
+            if isinstance(username,BaseUser):
+                user = username.display_name
+            else:
+                user = username
         else:
             user = request.user.display_name if request.user.is_authenticated else 'anonymous'
 
         return self.enforcer.enforce(user, path, method)
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
         """Parses the Authorization header and returns only the token"""
         try:
@@ -129,14 +133,15 @@
             return False,None
         user = SimpleUser(username)
         request.scope['user'] = user
         auth_type:str = kwargs.get("auth_type")
         if not auth_type or auth_type.lower()=='public': 
             return True,  user
         result = _casbin_auth._auth(request=request,username=username)
+        
         return result, user
 
          
     def clear_userinfo(self,request:Request):
         global _session_name
         del request.session[_session_name] 
         
@@ -176,15 +181,15 @@
         self.prefix = prefix
         self.username_field = username_field
         self.audience = audience
         self.options = options or dict()
     
      
     
-    async def authenticate(self, request,**kwargs) -> Union[None, Tuple[AuthCredentials, BaseUser]]:
+    async def authenticate(self, request:Request,**kwargs) -> Union[None, Tuple[AuthCredentials, BaseUser]]:
         auth_type:str = kwargs.get("auth_type")
 
         args = {'username_field':self.username_field, 'key':self.secret_key, 'algorithms': self.algorithm , 'audience':self.audience ,
                                             'options':self.options }
         userobj,token,payload = _casbin_auth.get_user_from_request(request=request,
                                                                  prefix=self.prefix, 
                                                                  is_jwt=True,**args)
```

### Comparing `irails-1.3.16/irails/base_controller.py` & `irails-1.3.19/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.19/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.19/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/cbv.py` & `irails-1.3.19/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/config.py` & `irails-1.3.19/irails/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,16 @@
                 value = value.replace(
                     "{" + name + "}", self.config.get(name, ""))
         return value
 
 if is_in_app(ROOT_PATH):
     ROOT_PATH = os.path.join(ROOT_PATH,"../..")
     config = YamlConfig( os.path.join(ROOT_PATH,"configs"))
+    if not is_cli_mode():
+        os.chdir(ROOT_PATH)
 elif IS_IN_irails:
     config = YamlConfig(os.path.join(ROOT_PATH, "configs"))
 else:
     # print(f"configs dir not found anywhere!")
     config = {}
 _project_name = os.path.basename(ROOT_PATH)
 debug = False
```

### Comparing `irails-1.3.16/irails/controller_utils.py` & `irails-1.3.19/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/core.py` & `irails-1.3.19/irails/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,14 +369,16 @@
         _log.info(_("checking database migrations...."))
     try:
             
         alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
         uri = db_cfg.get("uri")
         if uri:
             database.check_migration(application.data_engine,uri,alembic_ini)
+    except database.InitDbError as e:
+        raise
     except Exception as e:
         _log.disabled = False
         _log.error(e.args)
 def generate_mvc_app():
     global __is_debug
      
     application.title = _project_name
```

### Comparing `irails-1.3.16/irails/log.py` & `irails-1.3.19/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/midware.py` & `irails-1.3.19/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/midware_casbin.py` & `irails-1.3.19/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/midware_session.py` & `irails-1.3.19/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/mvc_router.py` & `irails-1.3.19/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_app.py` & `irails-1.3.19/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_controller.py` & `irails-1.3.19/irails/scripts/_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,22 +101,22 @@
                 else:
                     _item = [items]
                 for item in _item:
                     tpl = item['tpl']
                     dest = os.path.join(_current_dir , item['dest'])
                     micro = item['micro']
                     #controller file will generate last time
-                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=dir=='controllers') 
+                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=True) 
             controller_file = os.path.join(_current_dir,'controllers',f"{controler_path_name}_controller.py")
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             ensure_line(__init_file,f"from . import {controler_path_name}_controller")
-            __init_file = os.path.join(_current_dir,'models','__init__.py')
-            ensure_line(__init_file,f"from . import {controler_path_name}_model")
-            __init_file = os.path.join(_current_dir,'services','__init__.py')
-            ensure_line(__init_file,f"from . import {controler_path_name}_service")
+            # __init_file = os.path.join(_current_dir,'models','__init__.py')
+            # ensure_line(__init_file,f"from . import {controler_path_name}_model")
+            # __init_file = os.path.join(_current_dir,'services','__init__.py')
+            # ensure_line(__init_file,f"from . import {controler_path_name}_service")
             
             for action in actions:
                 acts.append(f"""
     @api.get('/{action}')
     def {action}(self):
         return self.view()                
 """)
```

### Comparing `irails-1.3.16/irails/scripts/_i18n.py` & `irails-1.3.19/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_model.py` & `irails-1.3.19/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_project.py` & `irails-1.3.19/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_run.py` & `irails-1.3.19/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_shell.py` & `irails-1.3.19/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/_test.py` & `irails-1.3.19/irails/scripts/_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,16 +95,17 @@
                 tested_line.append(line)    #Ran 1 test in ..s
                 status = lines[lnt+2]
                 if status=="OK":
                     ok+=1
                 
                 tested_line.append(status) #OK or others
                 matched_fail = False
-            elif re.match(pattern=r"^FAIL:.*$", string=line):
-                fail+=1
+            elif re.match(pattern=r"^FAIL:.*$", string=line) or re.match(pattern=r"^ERROR:",string=line)  :
+                if not matched_fail:
+                    fail+=1
                 matched_fail=True
             elif  matched_fail:
                 tested_line.append(line) 
             lnt += 1
     sys.stdout = sys.__stdout__
     sys.stderr = sys.__stderr__
     print("\n\ntest finished ,results:")
```

### Comparing `irails-1.3.16/irails/scripts/main.py` & `irails-1.3.19/irails/scripts/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         p = os.path.join(path,src)
         if not os.path.exists(p):
             dev_mode = False
     return dev_mode
 curdir = os.path.abspath(os.curdir)
 project_root = os.path.abspath(os.path.join(curdir,"../.."))
 if is_dev_mode(os.path.join(project_root,'irails')): 
-    sys.path.insert(-1, project_root)
+    
+    sys.path.insert(0, project_root)
     
 sys.path.insert(-1,os.path.abspath(os.curdir))
 from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
```

### Comparing `irails-1.3.16/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.19/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/app/home.tpl` & `irails-1.3.19/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/app/model.jinja` & `irails-1.3.19/irails/scripts/tpls/app/model.jinja`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from irails import database
 from sqlalchemy import Table,Column,ForeignKey,String,Integer
 from sqlalchemy.orm import Mapped,mapped_column,relationship
  
 class {{model_name}}(database.Base):
-    __tablename__ = "{{model_plural_name}}" 
+    __tablename__ = f"{database.table_prefix}{{model_plural_name}}" 
     {% if not 'id' in columns -%}
     id: Mapped[int] = mapped_column(primary_key=True) 
     {%- endif -%} 
     {%- for col in columns -%}
         {% if ':' in col %}
             {% set col_type = col.split(":")[1]+'()' %}
             {% if col_type == 'int()' %}
```

### Comparing `irails-1.3.16/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.19/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.19/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.19/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.19/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.19/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.19/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.19/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/unit_test.py` & `irails-1.3.19/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails/view.py` & `irails-1.3.19/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/irails.egg-info/PKG-INFO` & `irails-1.3.19/irails.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.16
+Version: 1.3.19
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,17 +18,18 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # irails
 A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode
 
-[Docs](https://irails.2rails.cn/) 
+[Online Docs](https://irails.2rails.cn/) 
 # Welcome to IRAILS(python on rails)
-
+IRAILS is not just an ordinary imitation of Ruby on rails, but based on the characteristics of the Python language itself, combined with rich Python class libraries, it refuses to create wheels repeatedly, and can achieve web development with minimal code and configuration, making Python web development fast and powerful, and can be easily deployed on various platforms.
+The design concept of IRails refers to some RORs, but it has its own soul. It does not pursue the ultimate configuration and development, but rather appropriate configuration and development. Currently, it is in a preview version and will continue to improve in the future.
  
 
 ## Installation  
 
 * `pip install irails` - install irails
 
 ## Commands
```

### Comparing `irails-1.3.16/irails.egg-info/SOURCES.txt` & `irails-1.3.19/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.16/setup.py` & `irails-1.3.19/setup.py`

 * *Files identical despite different names*

