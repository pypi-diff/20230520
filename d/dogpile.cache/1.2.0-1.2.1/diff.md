# Comparing `tmp/dogpile.cache-1.2.0.tar.gz` & `tmp/dogpile.cache-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogpile.cache-1.2.0.tar", last modified: Wed Apr 26 15:47:54 2023, max compression
+gzip compressed data, was "dogpile.cache-1.2.1.tar", last modified: Sat May 20 15:56:55 2023, max compression
```

## Comparing `dogpile.cache-1.2.0.tar` & `dogpile.cache-1.2.1.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/
--rw-r--r--   0 classic   (1000) classic   (1000)     1059 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/LICENSE
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/MANIFEST.in
--rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     4176 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/README.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.428534 dogpile.cache-1.2.0/docs/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.430534 dogpile.cache-1.2.0/docs/_sources/
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/api.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    39402 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/changelog.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/core_usage.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/front.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/index.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/recipes.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/usage.rst.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.433534 dogpile.cache-1.2.0/docs/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/basic.css
--rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/changelog.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/doctools.js
--rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/documentation_options.js
--rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/file.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/language_data.js
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/minus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/nature.css
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/plus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/pygments.css
--rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/searchtools.js
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/site_custom_css.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/sphinx_highlight.js
--rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/sphinx_paramlinks.css
--rw-r--r--   0 classic   (1000) classic   (1000)   480795 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/api.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/
--rw-r--r--   0 classic   (1000) classic   (1000)     3373 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/Makefile
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_static/site_custom_css.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/_templates/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_templates/site_custom_sidebars.html
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/api.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      266 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/builder.py
--rw-------   0 classic   (1000) classic   (1000)    39402 2023-04-26 15:47:49.000000 dogpile.cache-1.2.0/docs/build/changelog.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     7408 2023-04-26 15:47:49.000000 dogpile.cache-1.2.0/docs/build/conf.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/core_usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/front.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/recipes.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/requirements.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/unreleased/
--rw-r--r--   0 classic   (1000) classic   (1000)      410 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/unreleased/README.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)   132742 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/changelog.html
--rw-r--r--   0 classic   (1000) classic   (1000)    28474 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/core_usage.html
--rw-r--r--   0 classic   (1000) classic   (1000)     6492 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/front.html
--rw-r--r--   0 classic   (1000) classic   (1000)    67476 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/genindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    14900 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)     5958 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/py-modindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    32468 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/recipes.html
--rw-r--r--   0 classic   (1000) classic   (1000)     3509 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/search.html
--rw-r--r--   0 classic   (1000) classic   (1000)    74849 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/searchindex.js
--rw-r--r--   0 classic   (1000) classic   (1000)   111861 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/usage.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.421533 dogpile.cache-1.2.0/dogpile/
--rw-r--r--   0 classic   (1000) classic   (1000)      106 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.422534 dogpile.cache-1.2.0/dogpile/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)      180 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16890 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/api.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.423534 dogpile.cache-1.2.0/dogpile/cache/backends/
--rw-r--r--   0 classic   (1000) classic   (1000)     1197 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13749 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/file.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20835 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/memcached.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3030 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/memory.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/null.py
--rw-r--r--   0 classic   (1000) classic   (1000)    11764 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/redis.py
--rw-r--r--   0 classic   (1000) classic   (1000)      601 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/exception.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.424533 dogpile.cache-1.2.0/dogpile/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2964 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/plugins/mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3610 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/proxy.py
--rw-r--r--   0 classic   (1000) classic   (1000)    68481 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/region.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5418 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/util.py
--rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/core.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7077 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/lock.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.425534 dogpile.cache-1.2.0/dogpile/util/
--rw-r--r--   0 classic   (1000) classic   (1000)      339 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1735 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/compat.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4479 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/langhelpers.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2801 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4532 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/readwrite_lock.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.437534 dogpile.cache-1.2.0/dogpile.cache.egg-info/
--rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     2933 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/SOURCES.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/dependency_links.txt
--rw-r--r--   0 classic   (1000) classic   (1000)       73 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/entry_points.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/not-zip-safe
--rw-r--r--   0 classic   (1000) classic   (1000)       34 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/requires.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/top_level.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      838 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/hash_port.py
--rw-r--r--   0 classic   (1000) classic   (1000)      513 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/log_tests.ini
--rw-r--r--   0 classic   (1000) classic   (1000)     1595 2023-04-26 15:47:54.442534 dogpile.cache-1.2.0/setup.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)      558 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/setup.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.437534 dogpile.cache-1.2.0/tests/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.439534 dogpile.cache-1.2.0/tests/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)      870 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16896 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/_fixtures.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.439534 dogpile.cache-1.2.0/tests/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1389 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/plugins/test_mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2972 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_dbm_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    18860 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_decorator.py
--rw-r--r--   0 classic   (1000) classic   (1000)      405 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_mako.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16050 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_memcached_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)      361 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_memory_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1934 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_null_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6693 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_redis_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3468 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_redis_sentinel_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    32235 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_region.py
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/conftest.py
--rw-r--r--   0 classic   (1000) classic   (1000)      552 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_backgrounding.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10397 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)      893 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_utils.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.440534 dogpile.cache-1.2.0/tests/tls/
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client-ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1692 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1679 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client.key
--rw-r--r--   0 classic   (1000) classic   (1000)     1675 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/server.key
--rw-r--r--   0 classic   (1000) classic   (1000)     4021 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/server_chain.pem
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/tests/util/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1535 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/util/test_nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2401 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1059 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/MANIFEST.in
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4176 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/README.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.658309 dogpile.cache-1.2.1/docs/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.659309 dogpile.cache-1.2.1/docs/_sources/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/api.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    39675 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/core_usage.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/front.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/recipes.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/usage.rst.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.661309 dogpile.cache-1.2.1/docs/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/nature.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/site_custom_css.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/sphinx_paramlinks.css
+-rw-r--r--   0 classic   (1000) classic   (1000)   480641 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/api.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     3373 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_static/site_custom_css.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/_templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_templates/site_custom_sidebars.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/api.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      266 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/builder.py
+-rw-------   0 classic   (1000) classic   (1000)    39675 2023-05-20 15:56:52.000000 dogpile.cache-1.2.1/docs/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     7408 2023-05-20 15:56:52.000000 dogpile.cache-1.2.1/docs/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/core_usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/front.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/recipes.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/requirements.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      410 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)   133773 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    28473 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/core_usage.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     6491 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/front.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    67475 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    15002 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     5957 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/py-modindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    32467 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/recipes.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3508 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    74956 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)   111860 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/usage.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.656309 dogpile.cache-1.2.1/dogpile/
+-rw-r--r--   0 classic   (1000) classic   (1000)      106 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.656309 dogpile.cache-1.2.1/dogpile/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      180 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16890 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/api.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/cache/backends/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1197 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13749 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/file.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20835 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/memcached.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3030 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/memory.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/null.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11764 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/redis.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      601 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/exception.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2964 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/plugins/mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3610 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/proxy.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    68481 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5418 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/core.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7077 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/py.typed
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)      339 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1735 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4479 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/langhelpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2801 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4532 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/readwrite_lock.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.664309 dogpile.cache-1.2.1/dogpile.cache.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     2952 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)       73 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)       34 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/top_level.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      838 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/hash_port.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      513 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/log_tests.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)     1660 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)      558 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.664309 dogpile.cache-1.2.1/tests/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      870 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    17363 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/_fixtures.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1389 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/plugins/test_mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2972 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_dbm_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18860 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_decorator.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      405 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_mako.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16050 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_memcached_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      361 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_memory_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1934 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_null_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6693 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_redis_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3468 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_redis_sentinel_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    32235 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/conftest.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      552 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_backgrounding.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10397 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      893 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/tls/
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client-ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1692 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1679 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     1675 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/server.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     4021 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/server_chain.pem
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1535 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/util/test_nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2401 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tox.ini
```

### Comparing `dogpile.cache-1.2.0/LICENSE` & `dogpile.cache-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/PKG-INFO` & `dogpile.cache-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.2.0
+Version: 1.2.1
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
```

### Comparing `dogpile.cache-1.2.0/README.rst` & `dogpile.cache-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/api.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/changelog.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/changelog.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.1
+    :released: Sat May 20 2023
+
+    .. change::
+        :tags: bug, typing
+        :tickets: 238
+
+        Added py.typed file to root so that typing tools such as Mypy recognize
+        dogpile as typed. Pull request courtesy Daverball.
+
+.. changelog::
     :version: 1.2.0
     :released: Wed Apr 26 2023
 
     .. change::
         :tags: feature, region
         :tickets: 236
```

### Comparing `dogpile.cache-1.2.0/docs/_sources/core_usage.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/core_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/front.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/front.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/index.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/recipes.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/recipes.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_sources/usage.rst.txt` & `dogpile.cache-1.2.1/docs/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/basic.css` & `dogpile.cache-1.2.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/doctools.js` & `dogpile.cache-1.2.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/language_data.js` & `dogpile.cache-1.2.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/nature.css` & `dogpile.cache-1.2.1/docs/_static/nature.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/pygments.css` & `dogpile.cache-1.2.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/searchtools.js` & `dogpile.cache-1.2.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/_static/sphinx_highlight.js` & `dogpile.cache-1.2.1/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/api.html` & `dogpile.cache-1.2.1/docs/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>API &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>API &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -30,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1725,17 +1724,17 @@
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.SerializedReturnType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">SerializedReturnType</span></span><a class="headerlink" href="#dogpile.cache.api.SerializedReturnType" title="Permalink to this definition">¶</a></dt>
 <dd><p>the serialized form of what may be returned from a backend get method.</p>
 <p>alias of <code class="xref py py-obj docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code>, <a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">NoValue</span></code></a>]</p>
 </dd></dl>
 
-<dl class="py data">
+<dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.ValuePayload">
-<span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">ValuePayload</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">typing.Any</span></em><a class="headerlink" href="#dogpile.cache.api.ValuePayload" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">ValuePayload</span></span><a class="headerlink" href="#dogpile.cache.api.ValuePayload" title="Permalink to this definition">¶</a></dt>
 <dd><p>An object to be placed in the cache against a key.</p>
 </dd></dl>
 
 </section>
 <section id="module-dogpile.cache.backends.memory">
 <span id="backends"></span><h2>Backends<a class="headerlink" href="#module-dogpile.cache.backends.memory" title="Permalink to this heading">¶</a></h2>
 <section id="memory-backends">
@@ -4357,17 +4356,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * API
 ****** APIÂ¶ ******
 ***** RegionÂ¶ *****
   classdogpile.cache.region.CacheRegion(name: str | None = None,
   function_key_generator: ~typing.Callable[[...], ~typing.Callable[[...], str]]
   = <function function_key_generator>, function_multi_key_generator:
   ~typing.Callable[[...], ~typing.Callable[[...], ~typing.Sequence[str]]] =
@@ -774,15 +773,15 @@
   classdogpile.cache.api.NoValueÂ¶
       Bases: object
       Describe a missing cache value.
       The NO_VALUE constant should be used.
   dogpile.cache.api.SerializedReturnTypeÂ¶
       the serialized form of what may be returned from a backend get method.
       alias of Union[bytes, NoValue]
-  dogpile.cache.api.ValuePayload= typing.AnyÂ¶
+  dogpile.cache.api.ValuePayloadÂ¶
       An object to be placed in the cache against a key.
 
 ***** BackendsÂ¶ *****
 **** Memory BackendsÂ¶ ****
 Provides simple dictionary-based backends.
 The two backends are MemoryBackend and MemoryPickleBackend; the latter applies
 a serialization step to cached values while the former places the value as
@@ -2136,10 +2135,10 @@
 *** Next topic ***
 Changelog
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * API
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/build/Makefile` & `dogpile.cache-1.2.1/docs/build/Makefile`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/api.rst` & `dogpile.cache-1.2.1/docs/build/api.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/changelog.rst` & `dogpile.cache-1.2.1/docs/build/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.1
+    :released: Sat May 20 2023
+
+    .. change::
+        :tags: bug, typing
+        :tickets: 238
+
+        Added py.typed file to root so that typing tools such as Mypy recognize
+        dogpile as typed. Pull request courtesy Daverball.
+
+.. changelog::
     :version: 1.2.0
     :released: Wed Apr 26 2023
 
     .. change::
         :tags: feature, region
         :tickets: 236
```

### Comparing `dogpile.cache-1.2.0/docs/build/conf.py` & `dogpile.cache-1.2.1/docs/build/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = dogpile.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.2.0"
+release = "1.2.1"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `dogpile.cache-1.2.0/docs/build/core_usage.rst` & `dogpile.cache-1.2.1/docs/build/core_usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/front.rst` & `dogpile.cache-1.2.1/docs/build/front.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/index.rst` & `dogpile.cache-1.2.1/docs/build/index.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/recipes.rst` & `dogpile.cache-1.2.1/docs/build/recipes.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/build/usage.rst` & `dogpile.cache-1.2.1/docs/build/usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/docs/changelog.html` & `dogpile.cache-1.2.1/docs/changelog.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Changelog &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -26,26 +25,39 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
+<section id="change-1.2.1">
+<h2 class="release-version">1.2.1<a class="headerlink" href="#change-1.2.1" title="Permalink to this heading">¶</a></h2>
+Released: Sat May 20 2023<section id="change-1.2.1-bug">
+<h3>bug<a class="headerlink" href="#change-1.2.1-bug" title="Permalink to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.2.1-0"><span class="target" id="change-75c1354759a03cf148c4d208630af607"><strong>[bug] [typing]</strong> <a class="changelog-reference headerlink reference internal" href="#change-75c1354759a03cf148c4d208630af607">¶</a></span><p>Added py.typed file to root so that typing tools such as Mypy recognize
+dogpile as typed. Pull request courtesy Daverball.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/dogpile.cache/issues/238">#238</a></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.2.0">
 <h2 class="release-version">1.2.0<a class="headerlink" href="#change-1.2.0" title="Permalink to this heading">¶</a></h2>
 Released: Wed Apr 26 2023<section id="change-1.2.0-feature">
 <h3>feature<a class="headerlink" href="#change-1.2.0-feature" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p class="caption" id="change-1.2.0-0"><span class="target" id="change-cb55fd53c03c5bae407507cf0cd7453c"><strong>[feature] [region]</strong> <a class="changelog-reference headerlink reference internal" href="#change-cb55fd53c03c5bae407507cf0cd7453c">¶</a></span><p>Added new construct <a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> which can be
 raised by user-defined deserializer functions which would be passed to
@@ -1353,14 +1365,18 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
+<li><a class="reference internal" href="#change-1.2.1">1.2.1</a><ul>
+<li><a class="reference internal" href="#change-1.2.1-bug">bug</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.2.0">1.2.0</a><ul>
 <li><a class="reference internal" href="#change-1.2.0-feature">feature</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.1.8">1.1.8</a><ul>
 <li><a class="reference internal" href="#change-1.1.8-bug">bug</a></li>
 </ul>
@@ -1580,17 +1596,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,22 +1,29 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** 1.2.1Â¶ *****
+Released: Sat May 20 2023
+**** bugÂ¶ ****
+    * [bug] [typing] Â¶
+      Added py.typed file to root so that typing tools such as Mypy recognize
+      dogpile as typed. Pull request courtesy Daverball.
+      References: #238
+
 ***** 1.2.0Â¶ *****
 Released: Wed Apr 26 2023
 **** featureÂ¶ ****
     * [feature] [region] Â¶
       Added new construct api.CantDeserializeException which can be raised by
       user-defined deserializer functions which would be passed to
       CacheRegion.deserializer, to indicate a cache value that canât be
@@ -840,14 +847,16 @@
     * [no_tags] Â¶
       Initial release.
 [no_tags] Â¶
 Includes a pylibmc backend and a plain dictionary backend.
 
 **** Table_of_Contents ****
     * Changelog
+          o 1.2.1
+                # bug
           o 1.2.0
                 # feature
           o 1.1.8
                 # bug
           o 1.1.7
                 # usecase
           o 1.1.6
@@ -957,10 +966,10 @@
 [q                   ] [Go]
 *** Previous topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Changelog
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/core_usage.html` & `dogpile.cache-1.2.1/docs/core_usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>dogpile Core &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>dogpile Core &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -30,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -328,17 +327,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * dogpile Core
 ****** dogpile CoreÂ¶ ******
 dogpile provides a locking interface around a âvalue creationâ and âvalue
 retrievalâ pair of functions.
 Changed in version 0.6.0: The dogpile package encapsulates the functionality
 that was previously provided by the separate dogpile.core package.
 The primary interface is the Lock object, which provides for the invocation of
@@ -235,10 +234,10 @@
 *** Next topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * dogpile Core
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/front.html` & `dogpile.cache-1.2.1/docs/front.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Front Matter &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Front Matter &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -30,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -121,17 +120,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Front Matter
 ****** Front MatterÂ¶ ******
 Information about the dogpile.cache project.
 ***** Project HomepageÂ¶ *****
 dogpile.cache is hosted on GitHub at https://github.com/sqlalchemy/
 dogpile.cache.
 Releases and project status are available on Pypi at https://pypi.python.org/
@@ -45,10 +44,10 @@
 *** Next topic ***
 Usage_Guide
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Front Matter
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/genindex.html` & `dogpile.cache-1.2.1/docs/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Index &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -21,15 +20,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1136,17 +1135,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Index
 ****** Index ******
 Symbols | A | B | C | D | E | F | G | H | I | K | L | M | N | P | R | S | T | U
 | V | W
 ***** Symbols *****
     * **kw_(dogpile.cache.plugins.mako_cache.MakoPlugin.get_parameter)
           o (dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create
@@ -370,10 +369,10 @@
           o (dogpile.cache.region.RegionInvalidationStrategy       method)
             method)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Index
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/index.html` & `dogpile.cache-1.2.1/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -26,15 +25,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -93,14 +92,15 @@
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.exception">Exceptions</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.plugins.mako_cache">Plugins</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#utilities">Utilities</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#dogpile-core">dogpile Core</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.1">1.2.1</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.0">1.2.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.8">1.1.8</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.7">1.1.7</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.6">1.1.6</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.5">1.1.5</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.4">1.1.4</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.3">1.1.3</a></li>
@@ -204,17 +204,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Welcome to dogpile.cacheâs documentation!
 ****** Welcome to dogpile.cacheâs documentation!Â¶ ******
 Dogpile consists of two subsystems, one building on top of the other.
 dogpile provides the concept of a âdogpile lockâ, a control structure which
 allows a single thread of execution to be selected as the âcreatorâ of some
 resource, while allowing other threads of execution to refer to the previous
 version of this resource as the creation proceeds; if there is no previous
@@ -52,14 +51,15 @@
           o Backend_API
           o Backends
           o Exceptions
           o Plugins
           o Utilities
           o dogpile_Core
     * Changelog
+          o 1.2.1
           o 1.2.0
           o 1.1.8
           o 1.1.7
           o 1.1.6
           o 1.1.5
           o 1.1.4
           o 1.1.3
@@ -117,10 +117,10 @@
 [q                   ] [Go]
 *** Next topic ***
 Front_Matter
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Welcome to dogpile.cacheâs documentation!
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/py-modindex.html` & `dogpile.cache-1.2.1/docs/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Python Module Index &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -24,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -133,17 +132,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Python Module Index
 ****** Python Module Index ******
 d
      
     d
 [-] dogpile
         dogpile.cache.api
@@ -26,10 +25,10 @@
         dogpile.cache.proxy
         dogpile.cache.region
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Python Module Index
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/recipes.html` & `dogpile.cache-1.2.1/docs/recipes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Recipes &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Recipes &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -30,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -342,17 +341,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Recipes
 ****** RecipesÂ¶ ******
 ***** Invalidating a group of related keysÂ¶ *****
 This recipe presents a way to track the cache keys related to a particular
 region, for the purposes of invalidating a series of keys that relate to a
 particular id.
 Three cached functions, user_fn_one(), user_fn_two(), user_fn_three() each
@@ -248,10 +247,10 @@
 *** Next topic ***
 dogpile_Core
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Recipes
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/search.html` & `dogpile.cache-1.2.1/docs/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Search &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -27,15 +26,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -87,17 +86,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Search
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/docs/searchindex.js` & `dogpile.cache-1.2.1/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
         "class": [0, 1, 2, 5, 6],
         "cach": [0, 1, 3, 5, 6],
         "cacheregion": [0, 1, 5, 6],
         "name": [0, 1, 6],
         "str": [0, 1, 5, 6],
         "none": [0, 1, 2, 6],
         "function_key_gener": [0, 1, 5, 6],
-        "type": [0, 6],
+        "type": [0, 1, 6],
         "callabl": [0, 1, 5, 6],
         "function": [0, 1, 2, 5, 6],
         "function_multi_key_gener": [0, 1, 6],
         "sequenc": [0, 5, 6],
         "key_mangl": [0, 1, 5, 6],
         "serial": [0, 1, 5, 6],
         "ani": [0, 1, 2, 4, 6],
@@ -978,22 +978,30 @@
         "registri": [0, 5],
         "my_foo": 0,
         "foo1": 0,
         "refer": [0, 1, 2, 4],
         "garbag": 0,
         "collect": 0,
         "possibli": 0,
+        "sat": 1,
+        "20": 1,
+        "2023": 1,
+        "file": [1, 4, 6],
+        "root": 1,
+        "mypi": 1,
+        "dogpil": [1, 3, 5, 6],
+        "courtesi": 1,
+        "daverbal": 1,
+        "238": 1,
         "wed": 1,
         "apr": 1,
         "26": 1,
-        "2023": 1,
         "region": [1, 4, 5],
         "api": [1, 4, 5, 6],
         "defin": [1, 5, 6],
-        "courtesi": 1,
         "simon": 1,
         "hewitt": 1,
         "236": 1,
         "fri": 1,
         "jul": 1,
         "2022": 1,
         "memcach": [1, 2, 6],
@@ -1012,20 +1020,18 @@
         "sep": 1,
         "2021": 1,
         "deprec": 1,
         "warn": 1,
         "karthikeyan": 1,
         "singaravelan": 1,
         "203": 1,
-        "20": 1,
         "repair": 1,
         "__signature__": 1,
         "202": 1,
         "subject": 1,
-        "dogpil": [1, 3, 5, 6],
         "bastien": 1,
         "gerard": 1,
         "101": 1,
         "backend": [1, 2, 4, 5],
         "mois\u00e9": 1,
         "guimar\u00e3": 1,
         "de": 1,
@@ -1062,15 +1068,14 @@
         "pep": 1,
         "484": 1,
         "annot": 1,
         "aug": 1,
         "173": 1,
         "instal": [1, 4, 6],
         "cfg": 1,
-        "file": [1, 4, 6],
         "wheel": 1,
         "micha\u0142": 1,
         "g\u00f3rny": 1,
         "21": 1,
         "due": 1,
         "184": 1,
         "univers": 1,
@@ -1168,15 +1173,14 @@
         "ankitpatel96": 1,
         "small": [1, 6],
         "enhanc": [1, 3],
         "137": 1,
         "inspect": 1,
         "getargspec": 1,
         "129": 1,
-        "sat": 1,
         "24": 1,
         "organ": 1,
         "had": 1,
         "ben": 1,
         "usual": [1, 2, 6],
         "typeerror": 1,
         "less": 1,
@@ -1693,15 +1697,15 @@
             [0, 3, 1, "", "CacheReturnType"],
             [0, 0, 1, "", "CachedValue"],
             [0, 6, 1, "", "CantDeserializeException"],
             [0, 5, 1, "", "KeyType"],
             [0, 3, 1, "", "NO_VALUE"],
             [0, 0, 1, "", "NoValue"],
             [0, 3, 1, "", "SerializedReturnType"],
-            [0, 3, 1, "", "ValuePayload"]
+            [0, 5, 1, "", "ValuePayload"]
         ],
         "dogpile.cache.api.BytesBackend": [
             [0, 4, 1, "", "get_serialized"],
             [0, 4, 1, "", "get_serialized_multi"],
             [0, 4, 1, "", "set_serialized"],
             [0, 4, 1, "", "set_serialized_multi"]
         ],
@@ -2281,18 +2285,18 @@
         "integr": 0,
         "util": 0,
         "dogpil": [0, 2, 4],
         "core": [0, 2],
         "changelog": 1,
         "1": 1,
         "2": 1,
+        "bug": [1, 3],
         "0": 1,
         "featur": 1,
         "8": 1,
-        "bug": [1, 3],
         "7": 1,
         "usecas": 1,
         "6": 1,
         "5": 1,
         "4": 1,
         "3": 1,
         "misc": 1,
@@ -2406,45 +2410,19 @@
         "dogpile Core": [
             [0, "dogpile-core"],
             [2, "dogpile-core"]
         ],
         "Changelog": [
             [1, "changelog"]
         ],
-        "1.2.0": [
-            [1, "change-1.2.0"]
-        ],
-        "feature": [
-            [1, "change-1.2.0-feature"],
-            [1, "change-1.1.2-feature"],
-            [1, "change-1.1.0-feature"],
-            [1, "change-1.0.2-feature"],
-            [1, "change-1.0.0-feature"],
-            [1, "change-0.9.0-feature"],
-            [1, "change-0.6.6-feature"],
-            [1, "change-0.6.3-feature"],
-            [1, "change-0.6.2-feature"],
-            [1, "change-0.6.0-feature"],
-            [1, "change-0.5.7-feature"],
-            [1, "change-0.5.6-feature"],
-            [1, "change-0.5.5-feature"],
-            [1, "change-0.5.4-feature"],
-            [1, "change-0.5.3-feature"],
-            [1, "change-0.5.2-feature"],
-            [1, "change-0.5.1-feature"],
-            [1, "change-0.5.0-feature"],
-            [1, "change-0.4.3-feature"],
-            [1, "change-0.4.2-feature"],
-            [1, "change-0.4.1-feature"],
-            [1, "change-0.3.0-feature"]
-        ],
-        "1.1.8": [
-            [1, "change-1.1.8"]
+        "1.2.1": [
+            [1, "change-1.2.1"]
         ],
         "bug": [
+            [1, "change-1.2.1-bug"],
             [1, "change-1.1.8-bug"],
             [1, "change-1.1.6-bug"],
             [1, "change-1.1.4-bug"],
             [1, "change-1.1.3-bug"],
             [1, "change-1.1.1-bug"],
             [1, "change-1.0.2-bug"],
             [1, "change-1.0.1-bug"],
@@ -2469,14 +2447,44 @@
             [1, "change-0.5.0-bug"],
             [1, "change-0.4.3-bug"],
             [1, "change-0.4.1-bug"],
             [1, "change-0.4.0-bug"],
             [1, "change-0.3.1-bug"],
             [1, "change-0.3.0-bug"]
         ],
+        "1.2.0": [
+            [1, "change-1.2.0"]
+        ],
+        "feature": [
+            [1, "change-1.2.0-feature"],
+            [1, "change-1.1.2-feature"],
+            [1, "change-1.1.0-feature"],
+            [1, "change-1.0.2-feature"],
+            [1, "change-1.0.0-feature"],
+            [1, "change-0.9.0-feature"],
+            [1, "change-0.6.6-feature"],
+            [1, "change-0.6.3-feature"],
+            [1, "change-0.6.2-feature"],
+            [1, "change-0.6.0-feature"],
+            [1, "change-0.5.7-feature"],
+            [1, "change-0.5.6-feature"],
+            [1, "change-0.5.5-feature"],
+            [1, "change-0.5.4-feature"],
+            [1, "change-0.5.3-feature"],
+            [1, "change-0.5.2-feature"],
+            [1, "change-0.5.1-feature"],
+            [1, "change-0.5.0-feature"],
+            [1, "change-0.4.3-feature"],
+            [1, "change-0.4.2-feature"],
+            [1, "change-0.4.1-feature"],
+            [1, "change-0.3.0-feature"]
+        ],
+        "1.1.8": [
+            [1, "change-1.1.8"]
+        ],
         "1.1.7": [
             [1, "change-1.1.7"]
         ],
         "usecase": [
             [1, "change-1.1.7-usecase"],
             [1, "change-1.1.6-usecase"],
             [1, "change-1.1.5-usecase"],
```

### Comparing `dogpile.cache-1.2.0/docs/usage.html` & `dogpile.cache-1.2.1/docs/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Usage Guide &#8212; dogpile.cache 1.2.0 documentation</title>
+    <title>Usage Guide &#8212; dogpile.cache 1.2.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -30,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -947,17 +946,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
 
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Usage Guide
 ****** Usage GuideÂ¶ ******
 ***** OverviewÂ¶ *****
 At the time of this writing, popular key/value servers include Memcached, Redis
 and many others. While these tools all have different usage focuses, they all
 have in common that the storage model is based on the retrieval of a value
 based on a key; as such, they are all potentially suitable for caching,
@@ -428,10 +427,10 @@
 *** Next topic ***
 Recipes
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.0_documentation »
+    * dogpile.cache_1.2.1_documentation »
     * Usage Guide
-© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.0/dogpile/cache/api.py` & `dogpile.cache-1.2.1/dogpile/cache/api.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/__init__.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/file.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/file.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/memcached.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/memory.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/null.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/null.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/backends/redis.py` & `dogpile.cache-1.2.1/dogpile/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/exception.py` & `dogpile.cache-1.2.1/dogpile/cache/exception.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/plugins/mako_cache.py` & `dogpile.cache-1.2.1/dogpile/cache/plugins/mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/proxy.py` & `dogpile.cache-1.2.1/dogpile/cache/proxy.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/region.py` & `dogpile.cache-1.2.1/dogpile/cache/region.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/cache/util.py` & `dogpile.cache-1.2.1/dogpile/cache/util.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/core.py` & `dogpile.cache-1.2.1/dogpile/core.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/lock.py` & `dogpile.cache-1.2.1/dogpile/lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/util/compat.py` & `dogpile.cache-1.2.1/dogpile/util/compat.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/util/langhelpers.py` & `dogpile.cache-1.2.1/dogpile/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/util/nameregistry.py` & `dogpile.cache-1.2.1/dogpile/util/nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile/util/readwrite_lock.py` & `dogpile.cache-1.2.1/dogpile/util/readwrite_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/dogpile.cache.egg-info/PKG-INFO` & `dogpile.cache-1.2.1/dogpile.cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.2.0
+Version: 1.2.1
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
```

### Comparing `dogpile.cache-1.2.0/dogpile.cache.egg-info/SOURCES.txt` & `dogpile.cache-1.2.1/dogpile.cache.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 log_tests.ini
 setup.cfg
 setup.py
 tox.ini
 ./dogpile/__init__.py
 ./dogpile/core.py
 ./dogpile/lock.py
+./dogpile/py.typed
 ./dogpile/cache/__init__.py
 ./dogpile/cache/api.py
 ./dogpile/cache/exception.py
 ./dogpile/cache/proxy.py
 ./dogpile/cache/region.py
 ./dogpile/cache/util.py
 ./dogpile/cache/backends/__init__.py
```

### Comparing `dogpile.cache-1.2.0/hash_port.py` & `dogpile.cache-1.2.1/hash_port.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/log_tests.ini` & `dogpile.cache-1.2.1/log_tests.ini`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/setup.cfg` & `dogpile.cache-1.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,29 @@
 [options]
 install_requires = 
 	decorator>=4.0.0
 	stevedore>=3.0.0
 zip_safe = False
 packages = find:
 python_requires = >=3.6
+include_package_data = True
 package_dir = 
 	=.
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [options.exclude_package_data]
 '' = tests*
 
+[options.package_data]
+* = py.typed
+
 [options.entry_points]
 mako.cache = 
 	dogpile.cache = dogpile.cache.plugins.mako_cache:MakoPlugin
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dogpile.cache-1.2.0/setup.py` & `dogpile.cache-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/__init__.py` & `dogpile.cache-1.2.1/tests/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/_fixtures.py` & `dogpile.cache-1.2.1/tests/cache/_fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,37 @@
 from dogpile.cache.api import CantDeserializeException
 from dogpile.cache.api import NO_VALUE
 from dogpile.cache.region import _backend_loader
 from . import assert_raises_message
 from . import eq_
 
 
+def gen_some_key():
+    return f"some_key_{random.randint(1, 100000)}"
+
+
 class _GenericBackendFixture(object):
     @classmethod
     def setup_class(cls):
         backend_cls = _backend_loader.load(cls.backend)
         try:
             arguments = cls.config_args.get("arguments", {})
             backend = backend_cls(arguments)
         except ImportError:
             pytest.skip("Backend %s not installed" % cls.backend)
         cls._check_backend_available(backend)
 
     def tearDown(self):
+        some_key = gen_some_key()
         if self._region_inst:
             for key in self._keys:
                 self._region_inst.delete(key)
             self._keys.clear()
         elif self._backend_inst:
-            self._backend_inst.delete("some_key")
+            self._backend_inst.delete(some_key)
 
     @classmethod
     def _check_backend_available(cls, backend):
         pass
 
     region_args = {}
     config_args = {}
@@ -90,30 +95,34 @@
         self._backend_inst = backend_cls(arguments)
         return self._backend_inst
 
 
 class _GenericBackendTest(_GenericBackendFixture, TestCase):
     def test_backend_get_nothing(self):
         backend = self._backend()
-        eq_(backend.get_serialized("some_key"), NO_VALUE)
+        some_key = gen_some_key()
+        eq_(backend.get_serialized(some_key), NO_VALUE)
 
     def test_backend_delete_nothing(self):
         backend = self._backend()
-        backend.delete("some_key")
+        some_key = gen_some_key()
+        backend.delete(some_key)
 
     def test_backend_set_get_value(self):
         backend = self._backend()
-        backend.set_serialized("some_key", b"some value")
-        eq_(backend.get_serialized("some_key"), b"some value")
+        some_key = gen_some_key()
+        backend.set_serialized(some_key, b"some value")
+        eq_(backend.get_serialized(some_key), b"some value")
 
     def test_backend_delete(self):
         backend = self._backend()
-        backend.set_serialized("some_key", b"some value")
-        backend.delete("some_key")
-        eq_(backend.get_serialized("some_key"), NO_VALUE)
+        some_key = gen_some_key()
+        backend.set_serialized(some_key, b"some value")
+        backend.delete(some_key)
+        eq_(backend.get_serialized(some_key), NO_VALUE)
 
     def test_region_is_key_locked(self):
         reg = self._region()
         random_key = str(uuid.uuid1())
         assert not reg.get(random_key)
         eq_(reg.key_is_locked(random_key), False)
         # ensures that calling key_is_locked doesn't acquire the lock
@@ -124,16 +133,17 @@
             mutex.acquire()
             eq_(reg.key_is_locked(random_key), True)
             mutex.release()
             eq_(reg.key_is_locked(random_key), False)
 
     def test_region_set_get_value(self):
         reg = self._region()
-        reg.set("some key", "some value")
-        eq_(reg.get("some key"), "some value")
+        some_key = gen_some_key()
+        reg.set(some_key, "some value")
+        eq_(reg.get(some_key), "some value")
 
     def test_region_set_multiple_values(self):
         reg = self._region()
         values = {"key1": "value1", "key2": "value2", "key3": "value3"}
         reg.set_multi(values)
         eq_(values["key1"], reg.get("key1"))
         eq_(values["key2"], reg.get("key2"))
@@ -198,45 +208,48 @@
         eq_(values["key1"], reg.get("key1"))
         eq_(NO_VALUE, reg.get("key2"))
         eq_(values["key3"], reg.get("key3"))
         eq_(NO_VALUE, reg.get("key10"))
 
     def test_region_set_get_nothing(self):
         reg = self._region()
-        reg.delete_multi(["some key"])
-        eq_(reg.get("some key"), NO_VALUE)
+        some_key = gen_some_key()
+        reg.delete_multi([some_key])
+        eq_(reg.get(some_key), NO_VALUE)
 
     def test_region_creator(self):
         reg = self._region()
 
         def creator():
             return "some value"
 
-        eq_(reg.get_or_create("some key", creator), "some value")
+        some_key = gen_some_key()
+        eq_(reg.get_or_create(some_key, creator), "some value")
 
     @pytest.mark.time_intensive
     def test_threaded_dogpile(self):
         # run a basic dogpile concurrency test.
         # note the concurrency of dogpile itself
         # is intensively tested as part of dogpile.
         reg = self._region(config_args={"expiration_time": 0.25})
         lock = Lock()
         canary = []
+        some_key = gen_some_key()
 
         def creator():
             ack = lock.acquire(False)
             canary.append(ack)
             time.sleep(0.25)
             if ack:
                 lock.release()
             return "some value"
 
         def f():
             for x in range(5):
-                reg.get_or_create("some key", creator)
+                reg.get_or_create(some_key, creator)
                 time.sleep(0.5)
 
         threads = [Thread(target=f) for i in range(10)]
         for t in threads:
             t.start()
         for t in threads:
             t.join()
@@ -249,16 +262,17 @@
         """This test is testing that when we get inside the "creator" for
         a certain key, there are no other "creators" running at all for
         that key.
 
         With "distributed" locks, this is not 100% the case.
 
         """
+        some_key = gen_some_key()
         reg = self._region(config_args={"expiration_time": 0.25})
-        backend_mutex = reg.backend.get_mutex("some_key")
+        backend_mutex = reg.backend.get_mutex(some_key)
         is_custom_mutex = backend_mutex is not None
 
         locks = dict((str(i), Lock()) for i in range(11))
 
         canary = collections.defaultdict(list)
 
         def creator(*keys):
@@ -306,48 +320,50 @@
         # running at once
         if not is_custom_mutex:
             for l in canary.values():
                 assert False not in l
 
     def test_region_delete(self):
         reg = self._region()
-        reg.set("some key", "some value")
-        reg.delete("some key")
-        reg.delete("some key")
-        eq_(reg.get("some key"), NO_VALUE)
+        some_key = gen_some_key()
+        reg.set(some_key, "some value")
+        reg.delete(some_key)
+        reg.delete(some_key)
+        eq_(reg.get(some_key), NO_VALUE)
 
     @pytest.mark.time_intensive
     def test_region_expire(self):
         # TODO: ideally tests like these would not be using actual
         # time(); instead, an artificial function where the increment
         # can be controlled would be preferred.  this way tests need not
         # have any delay in running and additionally there is no issue
         # with very slow processing missing a timeout, as is often the
         # case with this particular test
 
+        some_key = gen_some_key()
         expire_time = 1.00
 
         reg = self._region(config_args={"expiration_time": expire_time})
         counter = itertools.count(1)
 
         def creator():
             return "some value %d" % next(counter)
 
-        eq_(reg.get_or_create("some key", creator), "some value 1")
+        eq_(reg.get_or_create(some_key, creator), "some value 1")
         time.sleep(expire_time + (0.2 * expire_time))
         # expiration is definitely hit
-        post_expiration = reg.get("some key", ignore_expiration=True)
+        post_expiration = reg.get(some_key, ignore_expiration=True)
         if post_expiration is not NO_VALUE:
             eq_(post_expiration, "some value 1")
 
-        eq_(reg.get_or_create("some key", creator), "some value 2")
+        eq_(reg.get_or_create(some_key, creator), "some value 2")
 
         # this line needs to run less the expire_time sec before the previous
         # two or it hits the expiration
-        eq_(reg.get("some key"), "some value 2")
+        eq_(reg.get(some_key), "some value 2")
 
     def test_decorated_fn_functionality(self):
         # test for any quirks in the fn decoration that interact
         # with the backend.
 
         reg = self._region()
 
@@ -367,21 +383,22 @@
         eq_(my_function(3, 4), 8)
         eq_(my_function(4, 3), 10)
 
         my_function.invalidate(4, 3)
         eq_(my_function(4, 3), 11)
 
     def test_exploding_value_fn(self):
+        some_key = gen_some_key()
         reg = self._region()
 
         def boom():
             raise Exception("boom")
 
         assert_raises_message(
-            Exception, "boom", reg.get_or_create, "some_key", boom
+            Exception, "boom", reg.get_or_create, some_key, boom
         )
 
 
 def raise_cant_deserialize_exception(v):
     raise CantDeserializeException()
```

### Comparing `dogpile.cache-1.2.0/tests/cache/plugins/test_mako_cache.py` & `dogpile.cache-1.2.1/tests/cache/plugins/test_mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_dbm_backend.py` & `dogpile.cache-1.2.1/tests/cache/test_dbm_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_decorator.py` & `dogpile.cache-1.2.1/tests/cache/test_decorator.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_memcached_backend.py` & `dogpile.cache-1.2.1/tests/cache/test_memcached_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_null_backend.py` & `dogpile.cache-1.2.1/tests/cache/test_null_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_redis_backend.py` & `dogpile.cache-1.2.1/tests/cache/test_redis_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_redis_sentinel_backend.py` & `dogpile.cache-1.2.1/tests/cache/test_redis_sentinel_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/cache/test_region.py` & `dogpile.cache-1.2.1/tests/cache/test_region.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/conftest.py` & `dogpile.cache-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/test_backgrounding.py` & `dogpile.cache-1.2.1/tests/test_backgrounding.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/test_lock.py` & `dogpile.cache-1.2.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/test_utils.py` & `dogpile.cache-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/ca-root.crt` & `dogpile.cache-1.2.1/tests/tls/ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/client-ca-root.crt` & `dogpile.cache-1.2.1/tests/tls/client-ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/client.crt` & `dogpile.cache-1.2.1/tests/tls/client.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/client.key` & `dogpile.cache-1.2.1/tests/tls/client.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/server.key` & `dogpile.cache-1.2.1/tests/tls/server.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/tls/server_chain.pem` & `dogpile.cache-1.2.1/tests/tls/server_chain.pem`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tests/util/test_nameregistry.py` & `dogpile.cache-1.2.1/tests/util/test_nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.0/tox.ini` & `dogpile.cache-1.2.1/tox.ini`

 * *Files identical despite different names*

