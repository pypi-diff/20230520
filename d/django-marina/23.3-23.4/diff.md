# Comparing `tmp/django-marina-23.3.tar.gz` & `tmp/django_marina-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marina-23.3.tar", last modified: Fri Apr 28 10:18:00 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-marina-23.3.tar` & `django_marina-23.4.tar`

### file list

```diff
@@ -1,48 +1,298 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.478948 django-marina-23.3/
--rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.3/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      281 2023-04-25 19:11:55.000000 django-marina-23.3/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     1747 2023-04-28 10:18:00.479018 django-marina-23.3/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      666 2020-10-31 06:45:14.000000 django-marina-23.3/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.474386 django-marina-23.3/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-14 04:57:27.000000 django-marina-23.3/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1023 2023-04-27 11:05:22.000000 django-marina-23.3/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      217 2021-12-04 17:34:31.000000 django-marina-23.3/docs/db.rst
--rw-r--r--   0 dylan      (501) staff       (20)      152 2020-06-15 12:42:52.000000 django-marina-23.3/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-27 10:53:35.000000 django-marina-23.3/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)      220 2022-01-03 06:11:13.000000 django-marina-23.3/docs/test.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.3/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     1368 2023-04-26 05:42:59.000000 django-marina-23.3/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)     1175 2023-04-28 10:18:00.479442 django-marina-23.3/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.471983 django-marina-23.3/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.474493 django-marina-23.3/src/django_marina/
--rw-r--r--   0 dylan      (501) staff       (20)       55 2023-04-28 10:17:53.000000 django-marina-23.3/src/django_marina/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475633 django-marina-23.3/src/django_marina/db/
--rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.3/src/django_marina/db/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      709 2023-04-25 07:56:49.000000 django-marina-23.3/src/django_marina/db/migrations.py
--rw-r--r--   0 dylan      (501) staff       (20)     1998 2023-04-23 07:42:51.000000 django-marina-23.3/src/django_marina/db/models.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475968 django-marina-23.3/src/django_marina/test/
--rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.3/src/django_marina/test/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.3/src/django_marina/test/clients.py
--rw-r--r--   0 dylan      (501) staff       (20)     9271 2023-04-23 07:48:36.000000 django-marina-23.3/src/django_marina/test/test_cases.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475298 django-marina-23.3/src/django_marina.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1747 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      899 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-26 05:41:51.000000 django-marina-23.3/src/django_marina.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       34 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       14 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.477971 django-marina-23.3/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.3/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.478791 django-marina-23.3/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.3/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/views.py
--rw-r--r--   0 dylan      (501) staff       (20)      617 2023-04-23 07:22:32.000000 django-marina-23.3/tests/models.py
--rw-r--r--   0 dylan      (501) staff       (20)     1995 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_db.py
--rw-r--r--   0 dylan      (501) staff       (20)      694 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_extended_client.py
--rw-r--r--   0 dylan      (501) staff       (20)     8518 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_extended_test_case.py
--rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.3/tests/test_imports.py
--rw-r--r--   0 dylan      (501) staff       (20)      303 2021-12-04 17:34:51.000000 django-marina-23.3/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.3/tests/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     1996 2023-04-27 10:53:35.000000 django-marina-23.3/tox.ini
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_marina-23.4/.DS_Store
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 django_marina-23.4/.readthedocs.yml
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 django_marina-23.4/CHANGELOG.md
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 django_marina-23.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 django_marina-23.4/Makefile
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/manage.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_marina-23.4/requirements-dev.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_marina-23.4/tox.ini
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_marina-23.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 django_marina-23.4/.github/workflows/dependabot-auto-approve-and-merge.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_marina-23.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1024c46eeebfddd9
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11c104e958fca970
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11f1cbea2e7c1ef3
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/11f70c0dd6e655e2
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/13083e3d792d3151
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/133247f993b34e0d
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/142785e97b4cf74f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/143e80cb705de0b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/154ac96b7a9c4c26
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/15d1a8f69df6395
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/18d06dc21b74bfd2
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/190b08956f165527
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/19a968c1275adfdf
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1abea56c7d1ab303
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1b1308a706406783
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1b53ba39e1f57e58
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1bb1eb28ecbe1fd
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1c70287f931fd26f
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1d5212aad6aa1740
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1e7643c29d4d410
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/1fc507464a0e6288
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/221f399498345b28
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/22d256aa42f4eeda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2543204f398cb739
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2623a935f18c2389
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/26cb16652fde39d7
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/27bf07d792f63194
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2a86af9fbe9f5871
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2ac6b5f709e2223a
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2ad7e8df3f10e03
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2b90dd378c3d45bb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2cd00f2b457dca82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d486d58c50ef5d7
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d9464ac3cccc68b
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2d9b1f2723f75b46
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/2e2d73549bcbd61e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/30cac57ee17b54d1
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/33869e8b2a934d4
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/33fbb16a8b89fbcc
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3486a583c5aae9c7
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/36e6efd54df5afda
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/36f56c23a36b0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3867c51af477cf8d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/398b3cd46b054c5f
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3d59ae216a1c8181
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3ed6018cf5986c69
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/3f0a57d8e69fb2da
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/41e0cb6bd3f98ee7
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/426cc96891369f10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/42c20bab2f436d88
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4313e83d0210a742
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/44097d4abe3025ec
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/44942ac379b31cf6
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/45ce23f60dd162f5
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/46a11b89a78d7ffd
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/472c3f1f2242535d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/47443eca57e44398
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/47594234b4ccf212
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/480bf6ada218a25
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/480cc16ccd1404aa
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/487962ffa1611e85
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/497399ebe720f9f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/49a09ccc457b7f8b
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4b66ca14605f82bd
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4cf1f7dc83495933
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/4e3954633a0bf2c7
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5146d8a06953ab21
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/515c8d28fb372ac5
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/51dc5c6c713b9817
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/52250ca9a5c62bef
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5486c94fca9b1c86
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/55430fc79027d1a4
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5594aca919406ac5
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/55dd803e72f04fe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/56c1a9758a8f943b
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/56f9652bf17b47c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/578c047a3a0f989d
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/583248f9f63239ea
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5878ea8c01a175da
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/58c51b85d06e4d50
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5abb45f46cb2832b
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5bf79e77047465ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/5cd5ffb8cf153388
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/602da119750b3c0f
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/608f1cb6c8d08d58
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/612cc2c4101efdd3
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/619e52f91b053290
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/630db95a305be885
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/630fe3444c7a9094
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6482a66319d710a8
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/64c23f13928d78e5
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/65afbecf5a75a81f
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/67b3a5b865e402f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/68b9472faaa1823f
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/69641bc8de3b442
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6a3063597a8f25f5
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6cb371e95d06ba12
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6df151341fbfb8fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6e212e1d6037d4e9
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6e87d3cd8e10064c
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6f068a2700da29d6
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6faf75218bac593c
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/6fe58ded543446d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7099ef80a1047a93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/72063909866fadb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/73da658a4784702c
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/73e7a5b4e3ea202b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/74fd2e3339bcf92c
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/75b4b597d009513b
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/76f0cbdaaae53850
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/77489570a19c7986
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/797af1fa82c5ae92
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7a556dfd6c4b2fb
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7ac66889f8779e3d
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7bd79d720f2a2380
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7d149554663b0573
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/7f6beb0d17265650
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/81920bc911181e1d
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/829977667da261ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/82a0d542c75229cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/830bb9643cae8f59
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/857794017ccd3c9a
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/85d8fe88d14c01ed
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8aff278ff88851fc
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8c720e348bd5351
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8cecabf7e2e19ce0
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8de8c7f68e3bd5e8
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8ebd74a1c0aa90ef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8f67a558c3de3d82
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/8f701c80389b53e5
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/915d0a3fd2d99117
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/91883a456f61783b
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/91faf7bebf5a0364
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9208aef60c2e233d
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/92293a3e521c27c2
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/93357306a59c700
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/933b6c3b6533ae7d
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/94e658d64ad183ca
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/95862bd589a59374
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/97353516d8c365c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/97a2fe8e0165782a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/984410d645d90d0f
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9c0c889ee7eadadf
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9c25e661e2484ef9
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9d74f5d5028ef03e
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/9ef744015358e12d
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a040d7c9218123ca
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a04c25f87109c873
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a156d024a5d30cab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a313e9f602097400
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a42fb8397a68c523
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a4cdec6301ee4304
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a5790219187b8cd3
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a57a669de607793f
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a62363bb26f41068
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a85868f8fbb6c1ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/a951830ea8bdeb48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/abe363314a4cd4c3
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ace934c109ecdcbc
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ad78c14c4521b7e3
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ae55027ec67feed3
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ae7d2ea132c983db
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/aec4a4843275828b
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/aed55d37c0eca6f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b07b696460410c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b0eb3a72a03e2dce
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b13e7fe605f50044
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b176e5c537beec8f
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b28fa1841f276735
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b2c1c0a97e5c5a2d
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b2e33bf0db76941f
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b3836daea2af04d4
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b3ee4610a623f211
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b7d63c347a5fe5f4
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/b9c6cb6048b64e78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ba0e2ad2cf9080ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bb6c759e4234e819
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bba357a2a553736b
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bcd30fab31815a22
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/be51610ec1a12bc5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/bfec558574a0ce1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c00d832ea903c6b6
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0afc5ec6a4435df
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0eb8a3bdca2990a
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c0f033672632e320
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c1b467e3796f4775
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c31fda6c6821b979
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c492c7e2ddc3dcd6
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c657a362d04d077b
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c7d52283449db1df
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c7db73965c27bd00
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c908f0a8b8ed958c
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/c90e56c8d6ff7fd0
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ca76bb035fabb17a
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cb31010082d0f9ca
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cd5d973a118b540c
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cd6f88b3f5a646f7
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ce4b8e3da3bd4378
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cec6d33d480a81c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/cf9d347a029f0c4c
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d197a4566a9aeb60
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d2d267fd74594e2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d305c95ff130f87a
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d3b50f2bd146c177
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d421acad960b4b1d
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d42337bba7e72aa2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d541581fe3c63f5b
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d694971b4d6e1708
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d782ea9dfb88a52b
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d89f6a905ffeb903
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d8bbf3c13b622b23
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d8f0c9ea00f7d767
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/d955d31049876a9e
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dcdbcc59efe7feb8
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dd5a06354ad32b52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/dd606e7425a82b27
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/df64d7830e598803
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e594e679f8c51a75
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e6e171d221302e2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e832b40f0167219d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e8422fbc9844014
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e91ae7e7dfb71ee9
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/e9d43a4ab7777f4b
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/eb93428e64dfc11d
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ebf6d3e0e21cd288
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ec4e0461e9f0bb0a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ed90c1891d1c4c28
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/edf638e5425bc575
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ee5c67b2c7b04b78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ee5d8217eb6b77ce
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f0092ea403d607dd
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f0dba3adf8827dcd
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f2ebff90091264a9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f380f7e060fff472
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f3b226ff878e709b
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f4cf21d861535529
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f6b3728a298392a6
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f821074c685e8812
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f8c4de0113634448
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/f966030a24ff0426
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fa7aa006d1768adf
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fc4989c1ceacb12c
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd2e452f49df5be2
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd8e2a019a79dee8
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd92e20ca5a2e7f
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fd9f160121419046
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/fe2baf07747246f2
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 django_marina-23.4/.ruff_cache/content/ff2d2a2e93c4719
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/configurationCache.log
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/dryrun.log
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/settings.json
+-rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 django_marina-23.4/.vscode/targets.log
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_marina-23.4/docs/changelog.rst
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 django_marina-23.4/docs/conf.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_marina-23.4/docs/contributing.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_marina-23.4/docs/db.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_marina-23.4/docs/index.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_marina-23.4/docs/requirements.txt
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 django_marina-23.4/docs/test.rst
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 django_marina-23.4/example/README.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/__about__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/migrations.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/db/models.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/__init__.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/clients.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 django_marina-23.4/src/django_marina/test/test_cases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.4/tests/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 django_marina-23.4/tests/models.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_db.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_extended_client.py
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_extended_test_case.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_imports.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_marina-23.4/tests/test_version.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_marina-23.4/tests/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/settings.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/urls.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 django_marina-23.4/tests/app/views.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 django_marina-23.4/.gitignore
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 django_marina-23.4/LICENSE
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_marina-23.4/README.md
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 django_marina-23.4/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 django_marina-23.4/PKG-INFO
```

### Comparing `django-marina-23.3/LICENSE` & `django_marina-23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/PKG-INFO` & `django_marina-23.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.3
+Version: 23.4
 Summary: Django extensions by Zostera
-Home-page: https://github.com/zostera/django-marina
-Author: Dylan Verheul
-Author-email: dylan@dyve.net
-License: BSD-3-Clause
+Project-URL: Changelog, https://github.com/zostera/django-marina/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://django-marina.readthedocs.io/
+Project-URL: Homepage, https://github.com/zostera/django-marina
+Project-URL: Issues, https://github.com/zostera/django-marina/issues
+Project-URL: Source, https://github.com/zostera/django-marina
+Author-email: Dylan Verheul <dylan@dyve.net>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -20,20 +24,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
+Requires-Dist: beautifulsoup4>=4.8.0
+Requires-Dist: django>=3.2
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # django-marina
 
 [![image](https://github.com/zostera/django-marina/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-marina/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-marina/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-marina?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-marina.svg)](https://pypi.python.org/pypi/django-marina)
 [![Any color you like](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 Django extensions by Zostera.
 
 Documentation is available at <https://django-marina.readthedocs.io/>.
+
+## Requirements
+
+This package requires a combination of Python and Django that is currently supported.
+
+See "Supported Versions" on https://www.djangoproject.com/download/.
```

### Comparing `django-marina-23.3/src/django_marina/db/migrations.py` & `django_marina-23.4/src/django_marina/db/migrations.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/src/django_marina/db/models.py` & `django_marina-23.4/src/django_marina/db/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/src/django_marina/test/clients.py` & `django_marina-23.4/src/django_marina/test/clients.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/src/django_marina/test/test_cases.py` & `django_marina-23.4/src/django_marina/test/test_cases.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/app/settings.py` & `django_marina-23.4/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/app/urls.py` & `django_marina-23.4/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/app/views.py` & `django_marina-23.4/tests/app/views.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/models.py` & `django_marina-23.4/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/test_db.py` & `django_marina-23.4/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/test_extended_client.py` & `django_marina-23.4/tests/test_extended_client.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/test_extended_test_case.py` & `django_marina-23.4/tests/test_extended_test_case.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/test_imports.py` & `django_marina-23.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.3/tests/urls.py` & `django_marina-23.4/tests/urls.py`

 * *Files identical despite different names*

