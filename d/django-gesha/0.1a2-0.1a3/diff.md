# Comparing `tmp/django-gesha-0.1a2.tar.gz` & `tmp/django-gesha-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gesha-0.1a2.tar", last modified: Sun May 14 01:41:01 2023, max compression
+gzip compressed data, was "django-gesha-0.1a3.tar", last modified: Sat May 20 05:09:16 2023, max compression
```

## Comparing `django-gesha-0.1a2.tar` & `django-gesha-0.1a3.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-14 01:40:47.000000 django-gesha-0.1a2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 01:40:47.000000 django-gesha-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-14 01:41:01.680786 django-gesha-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 01:40:47.000000 django-gesha-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/django_gesha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/settings.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/gesha/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/gesha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/gesha/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/gesha/static/gesha/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/gesha/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/templatetags/gesha.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/js_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/context.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/converters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/urls.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/js_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/context.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/converters.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/helpers.ts
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/main.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/urls.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 01:40:47.000000 django-gesha-0.1a2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-14 01:40:47.000000 django-gesha-0.1a2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-14 01:40:47.000000 django-gesha-0.1a2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-14 01:40:47.000000 django-gesha-0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:41:01.680786 django-gesha-0.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/commands/printtestpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_jscontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.963458 django-gesha-0.1a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-20 05:09:05.000000 django-gesha-0.1a3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-20 05:09:05.000000 django-gesha-0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-20 05:09:16.975458 django-gesha-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-20 05:09:05.000000 django-gesha-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/django_gesha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/assets/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/settings.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/gesha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/gesha/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/static/gesha/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/templatetags/gesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/js_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/converters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/urls.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/js_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/context.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/converters.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/main.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/urls.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-20 05:09:05.000000 django-gesha-0.1a3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-20 05:09:05.000000 django-gesha-0.1a3/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-20 05:09:05.000000 django-gesha-0.1a3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-20 05:09:05.000000 django-gesha-0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 05:09:16.975458 django-gesha-0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/commands/printtestpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_jscontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tsconfig.json
```

### Comparing `django-gesha-0.1a2/.github/workflows/python-publish.yml` & `django-gesha-0.1a3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/.github/workflows/test.yml` & `django-gesha-0.1a3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/.gitignore` & `django-gesha-0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/LICENSE` & `django-gesha-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/PKG-INFO` & `django-gesha-0.1a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a2
+Version: 0.1a3
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
-Project-URL: homepage, https://django-gesha.readthedocs.io/en/latest/
-Project-URL: repository, https://github.com/ely-as/django-gesha
-Project-URL: changelog, https://github.com/ely-as/django-gesha/blob/main/CHANGELOG.md
-Keywords: django,javascript
+Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
+Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
+Project-URL: Source, https://github.com/ely-as/django-gesha
+Keywords: django,javascript,typescript
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-gesha-0.1a2/README.md` & `django-gesha-0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/django_gesha.egg-info/PKG-INFO` & `django-gesha-0.1a3/django_gesha.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a2
+Version: 0.1a3
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
-Project-URL: homepage, https://django-gesha.readthedocs.io/en/latest/
-Project-URL: repository, https://github.com/ely-as/django-gesha
-Project-URL: changelog, https://github.com/ely-as/django-gesha/blob/main/CHANGELOG.md
-Keywords: django,javascript
+Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
+Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
+Project-URL: Source, https://github.com/ely-as/django-gesha
+Keywords: django,javascript,typescript
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-gesha-0.1a2/django_gesha.egg-info/SOURCES.txt` & `django-gesha-0.1a3/django_gesha.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 django_gesha.egg-info/top_level.txt
 docs/changelog.md
 docs/contributing.md
 docs/index.md
 docs/installation.md
 docs/settings.md
 docs/user_guide.md
+docs/assets/favicon.svg
+docs/assets/logo.svg
 docs/stylesheets/extra.css
 gesha/__init__.py
 gesha/conf.py
 gesha/mixins.py
 gesha/types.py
 gesha/urls.py
 gesha/views.py
```

### Comparing `django-gesha-0.1a2/docs/contributing.md` & `django-gesha-0.1a3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/docs/index.md` & `django-gesha-0.1a3/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/docs/installation.md` & `django-gesha-0.1a3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/docs/settings.md` & `django-gesha-0.1a3/docs/settings.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## **django-gesha** Settings
 
 ---
 
 ### <pre>**GESHA_ALLOWED_URL_PATTERNS**</pre>
 
-Default: `["*"]`
+Default: `[]`
 
 A list of allowed patterns for use in [reversing URLs](../user_guide/#reverse-urls).
 Supports [Unix shell-style wildcards](https://docs.python.org/3/library/fnmatch.html)
 <span style="white-space:nowrap;">(`*`, `?`, `[seq]` and `[!seq]`)</span>. Example to
 match `login`, `logout` and all paths in the `myapp` namespace:
 
 ``` py
 GESHA_ALLOWED_URL_PATTERNS = ["log*", "myapp:*"]
 ```
 
-Set to an empty list to disable all patterns.
+The default setting (an empty list) disables all patterns.
 
 ---
```

### Comparing `django-gesha-0.1a2/docs/user_guide.md` & `django-gesha-0.1a3/docs/user_guide.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 ### Configure views
 
 **django-gesha** requires you to add some context data to your views to work. See the
 following examples for class-based views and function-based views.
 
 !!! example "Example class-based view"
 
-    Add `#!py gesha.mixins.JSContextMixin` to your class-based view, and add JavaScript
-    context data by extending its `#!py get_js_context_data()` method:
+    Add `#!py gesha.JSContextMixin` to your class-based view, and add JavaScript context
+    data by extending its `#!py get_js_context_data()` method:
 
     === "myapp/views.py"
 
         ``` py hl_lines="2 5 8 9 10 11" linenums="1"
+        import gesha
         from django.views.generic import TemplateView
-        from gesha.mixins import JSContextMixin
 
 
-        class HomeView(JSContextMixin, TemplateView):
+        class HomeView(gesha.JSContextMixin, TemplateView):
             template_name = "myapp/home.html"
 
             def get_js_context_data(self, **kwargs) -> dict:
                 context = super().get_js_context_data(**kwargs)
                 context.update({"myNumber": 5, "myString": "this is my string"})
                 return context
         ```
@@ -42,23 +42,23 @@
         ```
 
 !!! example "Example function-based view"
 
     === "myapp.views.py"
 
         ``` py hl_lines="3 9 10 11" linenums="1"
+        import gesha
         from django.http import HttpRequest, HttpResponse
         from django.shortcuts import render
-        from gesha.views import create_js_context_data
 
 
         def home(request: HttpRequest) -> HttpResponse:
             context = {}
             context.update(
-                create_js_context_data(
+                gesha.create_js_context_data(
                     {"myNumber": 5, "myString": "this is my string"}
                 )
             )
             return render(request, "myapp/home.html", context=context)
         ```
 
     === "myapp/urls.py"
@@ -126,15 +126,15 @@
 Any context data added using the methods below must be JSON serializable.
 
 !!! example "Adding context in class-based views"
 
     For class-based views override `#!py get_js_context_data()` to add context data:
 
     ``` py
-    class HomeView(JSContextMixin, TemplateView):
+    class HomeView(gesha.JSContextMixin, TemplateView):
         template_name = "myapp/home.html"
 
         def get_js_context_data(self, **kwargs) -> dict:
             context = super().get_js_context_data(**kwargs)
             context.update({"myNumber": 5, "myString": "this is my string"})
             return context
     ```
@@ -144,15 +144,15 @@
     For function-based views pass a dict to `#!py create_js_context_data()` to add
     context data:
 
     ``` py
     def home(request):
         context = {}
         context.update(
-            create_js_context_data(
+            gesha.create_js_context_data(
                 {"myNumber": 5, "myString": "this is my string"}
             )
         )
         return render(request, "myapp/home.html", context=context)
     ```
 
 ### Reverse URLs
@@ -184,32 +184,32 @@
 
         ``` django title="In templates"
         {% url 'myapp:page' page=5 %}
         ```
 
 !!! tip
 
-    `#!js django.urls.reverse()` is aliased to `#!js django.reverse()`
-
-!!! tip
-
-    To limit the URLs available for reversing (e.g. for security reasons) configure
-    the [`GESHA_ALLOWED_URL_PATTERNS`](../settings/#gesha_allowed_url_patterns) setting.
+    To set the URLs available for reversing configure the
+    [`GESHA_ALLOWED_URL_PATTERNS`](../settings/#gesha_allowed_url_patterns) setting.
 
     These patterns can also be set in class-based views by overriding the
     `#!py get_allowed_url_patterns()` method, for example:
 
     ``` py
-    class HomeView(JSContextMixin, TemplateView):
+    class HomeView(gesha.JSContextMixin, TemplateView):
         ...
 
         def get_allowed_url_patterns(self):
             return ["myapp:home", "otherapp:*"]
     ```
 
+!!! tip
+
+    `#!js django.urls.reverse()` is aliased to `#!js django.reverse()`
+
 #### Custom converters
 
 If you have
 [registered custom path converters](https://docs.djangoproject.com/en/stable/topics/http/urls/#registering-custom-path-converters)
 in your Django project, you can also register them using the JavaScript API, for
 example:
```

### Comparing `django-gesha-0.1a2/gesha/mixins.py` & `django-gesha-0.1a3/gesha/mixins.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js` & `django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map` & `django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gesha/templatetags/gesha.py` & `django-gesha-0.1a3/gesha/templatetags/gesha.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gesha/types.py` & `django-gesha-0.1a3/gesha/types.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gesha/urls.py` & `django-gesha-0.1a3/gesha/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/gulpfile.js` & `django-gesha-0.1a3/gulpfile.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_src/context.ts` & `django-gesha-0.1a3/js_src/context.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_src/converters.ts` & `django-gesha-0.1a3/js_src/converters.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_src/main.ts` & `django-gesha-0.1a3/js_src/main.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_src/urls.ts` & `django-gesha-0.1a3/js_src/urls.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_tests/converters.spec.ts` & `django-gesha-0.1a3/js_tests/converters.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_tests/helpers.ts` & `django-gesha-0.1a3/js_tests/helpers.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_tests/test.html` & `django-gesha-0.1a3/js_tests/test.html`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/js_tests/urls.spec.ts` & `django-gesha-0.1a3/js_tests/urls.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/mkdocs.yml` & `django-gesha-0.1a3/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
   name: material
   palette:
     scheme: slate
     primary: gesha
     accent: amber
   features:
     - content.code.annotate
+  logo: assets/logo.svg
+  favicon: assets/favicon.svg
 markdown_extensions:
   - admonition
   - footnotes
   - pymdownx.details
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
```

### Comparing `django-gesha-0.1a2/package-lock.json` & `django-gesha-0.1a3/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999922744128555%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.0-alpha3'}}", "'version'": "'0.1.0-alpha3'"}*

```diff
@@ -23,15 +23,15 @@
                 "typescript": "^5.0.4",
                 "vinyl-buffer": "^1.0.1",
                 "vinyl-source-stream": "^2.0.0",
                 "watchify": "^4.0.0"
             },
             "license": "MIT",
             "name": "django-gesha",
-            "version": "0.1.0-alpha2"
+            "version": "0.1.0-alpha3"
         },
         "node_modules/@cspotcode/source-map-support": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "0.3.9"
             },
             "dev": true,
             "engines": {
@@ -9298,9 +9298,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0-alpha2"
+    "version": "0.1.0-alpha3"
 }
```

### Comparing `django-gesha-0.1a2/package.json` & `django-gesha-0.1a3/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.1.0-alpha3'"}*

```diff
@@ -37,9 +37,9 @@
         "type": "git",
         "url": "git+https://github.com/ely-as/django-gesha.git"
     },
     "scripts": {
         "lint": "eslint ./js_*/**/*.ts",
         "test": "mocha"
     },
-    "version": "0.1.0-alpha2"
+    "version": "0.1.0-alpha3"
 }
```

### Comparing `django-gesha-0.1a2/pyproject.toml` & `django-gesha-0.1a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "django-gesha"
 authors = [
     {name = "elyas", email = "elyas@ely.as"},
 ]
 description = "JavaScript utilities for Django projects."
 requires-python = ">=3.8"
-keywords = ["django", "javascript"]
+keywords = ["django", "javascript", "typescript"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: JavaScript",
     "Programming Language :: Python :: 3",
@@ -34,17 +34,17 @@
 ]
 dependencies = [
     "Django",
 ]
 dynamic = ["version", "readme"]
 
 [project.urls]
-homepage = "https://django-gesha.readthedocs.io/en/latest/"
-repository = "https://github.com/ely-as/django-gesha"
-changelog = "https://github.com/ely-as/django-gesha/blob/main/CHANGELOG.md"
+"Documentation" = "https://django-gesha.readthedocs.io/en/latest/"
+"Issue Tracker" = "https://github.com/ely-as/django-gesha/issues"
+"Source" = "https://github.com/ely-as/django-gesha"
 
 [tool.setuptools.dynamic]
 version = {attr = "gesha.__version__"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.packages.find]
 where = ["."]
```

### Comparing `django-gesha-0.1a2/test_project/fake/management/commands/printtestpage.py` & `django-gesha-0.1a3/test_project/fake/management/commands/printtestpage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/test_project/fake/settings.py` & `django-gesha-0.1a3/test_project/fake/settings.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/test_project/fake/urls.py` & `django-gesha-0.1a3/test_project/fake/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/test_project/fake/views.py` & `django-gesha-0.1a3/test_project/fake/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from __future__ import annotations
 
 from django.http import HttpRequest, HttpResponse
 from django.shortcuts import render
 from django.views.generic import TemplateView
 
-from gesha.mixins import JSContextMixin
-from gesha.views import create_js_context_data
+import gesha
 
 TEMPLATE_NAME = "test.html"
 CONTEXT = {
     "myNumber": 5,
     "myString": "this is a string",
 }
 
 
-class FakeView(JSContextMixin, TemplateView):
+class FakeView(gesha.JSContextMixin, TemplateView):
     template_name = TEMPLATE_NAME
 
     def get_js_context_data(self, **kwargs) -> dict:
         context = super().get_js_context_data(**kwargs)
         context.update(CONTEXT)
         return context
 
 
 def function_based_view(request: HttpRequest) -> HttpResponse:
-    context = create_js_context_data(CONTEXT)
+    context = gesha.create_js_context_data(CONTEXT)
     return render(request, TEMPLATE_NAME, context=context)
 
 
 # Async views
 
 
 async def async_view(request: HttpRequest) -> HttpResponse:
     context = {}
-    js_context = create_js_context_data(CONTEXT)
+    js_context = gesha.create_js_context_data(CONTEXT)
     context.update(js_context)
     return render(request, TEMPLATE_NAME, context=context)
```

### Comparing `django-gesha-0.1a2/test_project/manage.py` & `django-gesha-0.1a3/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/tests/test_jscontext.py` & `django-gesha-0.1a3/tests/test_jscontext.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from collections.abc import Iterator
 
 import django
 import pytest
 from bs4 import BeautifulSoup
 from django.test import Client, override_settings
 
 
@@ -14,43 +15,58 @@
 
 
 paths_to_test_for_presence_of_valid_script_html: list[str] = [
     "/",  # tests JSContextMixin
     "/func-based/",  # tests create_js_context_data()
 ]
 
-if django.VERSION[0] >= 4 or (django.VERSION[0] == 3 and django.VERSION[1] >= 1):
+if django.VERSION[:2] >= (3, 1):
     paths_to_test_for_presence_of_valid_script_html += [
         "/async/",  # tests async
     ]
 
 
-@pytest.mark.parametrize("path", paths_to_test_for_presence_of_valid_script_html)
+@pytest.fixture(params=paths_to_test_for_presence_of_valid_script_html)
+def path(request: pytest.FixtureRequest) -> Iterator[str]:
+    yield request.param
+
+
 def test_jscontext_tag_generates_script_html(path: str) -> None:
     soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     assert json_script
     js_context = json.loads(json_script.text)
     assert "myString" in js_context
 
 
-def test_jscontext_tag_works_when_setting_GESHA_JSCONTEXT_KEY_is_changed() -> None:
+def test_jscontext_tag_works_when_setting_GESHA_JSCONTEXT_KEY_is_changed(
+    path: str,
+) -> None:
     with override_settings(GESHA_JSCONTEXT_KEY="different_key"):
-        soup = request_soup("GET", "/")
+        soup = request_soup("GET", path)
     json_script = soup.find("script", id="different_key")
     assert json_script
 
 
-def test_paths_are_empty_when_GESHA_ALLOWED_URL_PATTERNS_is_empty() -> None:
+def test_paths_are_empty_by_default(path: str) -> None:
+    soup = request_soup("GET", path)
+    json_script = soup.find("script", id="js_context_data")
+    js_context = json.loads(json_script.text)  # type: ignore[union-attr]
+    assert js_context["_gesha"]["paths"] == {}
+
+
+def test_paths_are_empty_when_GESHA_ALLOWED_URL_PATTERNS_is_empty_list(
+    path: str,
+) -> None:
     with override_settings(GESHA_ALLOWED_URL_PATTERNS=[]):
-        soup = request_soup("GET", "/")
+        soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     js_context = json.loads(json_script.text)  # type: ignore[union-attr]
     assert js_context["_gesha"]["paths"] == {}
 
 
-def test_paths_are_filtered_when_GESHA_ALLOWED_URL_PATTERNS_is_set() -> None:
+def test_paths_are_filtered_when_GESHA_ALLOWED_URL_PATTERNS_is_set(path: str) -> None:
     with override_settings(GESHA_ALLOWED_URL_PATTERNS=["fake:test"]):
-        soup = request_soup("GET", "/")
+        soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     js_context = json.loads(json_script.text)  # type: ignore[union-attr]
     assert len(js_context["_gesha"]["paths"]) == 1
```

### Comparing `django-gesha-0.1a2/tests/test_package_json.py` & `django-gesha-0.1a3/tests/test_package_json.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/tests/test_urls.py` & `django-gesha-0.1a3/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a2/tox.ini` & `django-gesha-0.1a3/tox.ini`

 * *Files identical despite different names*

