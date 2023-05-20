# Comparing `tmp/tldextract-3.4.3.tar.gz` & `tmp/tldextract-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldextract-3.4.3.tar", last modified: Thu May 18 18:35:52 2023, max compression
+gzip compressed data, was "tldextract-3.4.4.tar", last modified: Sat May 20 00:33:31 2023, max compression
```

## Comparing `tldextract-3.4.3.tar` & `tldextract-3.4.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.241761 tldextract-3.4.3/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.231246 tldextract-3.4.3/.github/
--rw-r--r--   0 john       (501) staff       (20)       25 2022-06-05 23:30:19.000000 tldextract-3.4.3/.github/FUNDING.yml
--rw-r--r--   0 john       (501) staff       (20)      129 2022-05-03 19:53:33.000000 tldextract-3.4.3/.gitignore
--rw-r--r--   0 john       (501) staff       (20)      469 2023-01-14 03:27:06.000000 tldextract-3.4.3/.travis.yml
--rw-r--r--   0 john       (501) staff       (20)    13548 2023-05-18 18:31:25.000000 tldextract-3.4.3/CHANGELOG.md
--rw-r--r--   0 john       (501) staff       (20)     1522 2022-05-03 19:53:33.000000 tldextract-3.4.3/LICENSE
--rw-r--r--   0 john       (501) staff       (20)      116 2022-05-03 19:53:33.000000 tldextract-3.4.3/MANIFEST.in
--rw-r--r--   0 john       (501) staff       (20)     2188 2023-05-18 18:35:52.241953 tldextract-3.4.3/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     9874 2023-05-13 22:04:35.000000 tldextract-3.4.3/README.md
--rw-r--r--   0 john       (501) staff       (20)       68 2023-05-17 23:47:07.000000 tldextract-3.4.3/conftest.py
--rw-r--r--   0 john       (501) staff       (20)       37 2022-05-03 19:53:33.000000 tldextract-3.4.3/pytest.ini
--rw-r--r--   0 john       (501) staff       (20)      327 2023-05-18 18:35:52.242624 tldextract-3.4.3/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     2780 2023-05-18 00:31:14.000000 tldextract-3.4.3/setup.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.235210 tldextract-3.4.3/tests/
--rw-r--r--   0 john       (501) staff       (20)       21 2023-05-18 00:31:14.000000 tldextract-3.4.3/tests/__init__.py
--rw-r--r--   0 john       (501) staff       (20)      783 2022-06-05 23:30:19.000000 tldextract-3.4.3/tests/cli_test.py
--rw-r--r--   0 john       (501) staff       (20)      435 2023-05-18 00:31:14.000000 tldextract-3.4.3/tests/conftest.py
--rw-r--r--   0 john       (501) staff       (20)     1935 2022-09-20 19:51:12.000000 tldextract-3.4.3/tests/custom_suffix_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.235619 tldextract-3.4.3/tests/fixtures/
--rw-r--r--   0 john       (501) staff       (20)       31 2021-01-11 20:42:27.000000 tldextract-3.4.3/tests/fixtures/fake_suffix_list_fixture.dat
--rw-r--r--   0 john       (501) staff       (20)      248 2022-06-05 23:30:19.000000 tldextract-3.4.3/tests/integration_test.py
--rw-r--r--   0 john       (501) staff       (20)    13880 2023-05-18 18:25:10.000000 tldextract-3.4.3/tests/main_test.py
--rw-r--r--   0 john       (501) staff       (20)     3420 2023-05-18 18:25:10.000000 tldextract-3.4.3/tests/test_cache.py
--rw-r--r--   0 john       (501) staff       (20)     1545 2023-05-18 00:31:14.000000 tldextract-3.4.3/tests/test_parallel.py
--rw-r--r--   0 john       (501) staff       (20)     1502 2023-05-18 00:28:46.000000 tldextract-3.4.3/tests/test_trie.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.239544 tldextract-3.4.3/tldextract/
--rw-r--r--   0 john       (501) staff       (20)   238022 2023-05-13 22:04:35.000000 tldextract-3.4.3/tldextract/.tld_set_snapshot
--rw-r--r--   0 john       (501) staff       (20)      216 2023-01-27 07:03:29.000000 tldextract-3.4.3/tldextract/__init__.py
--rw-r--r--   0 john       (501) staff       (20)       90 2022-06-05 23:36:58.000000 tldextract-3.4.3/tldextract/__main__.py
--rw-r--r--   0 john       (501) staff       (20)      160 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract/_version.py
--rw-r--r--   0 john       (501) staff       (20)     8725 2023-05-18 18:25:10.000000 tldextract-3.4.3/tldextract/cache.py
--rw-r--r--   0 john       (501) staff       (20)     2416 2023-05-18 00:28:46.000000 tldextract-3.4.3/tldextract/cli.py
--rw-r--r--   0 john       (501) staff       (20)        0 2022-05-03 19:53:33.000000 tldextract-3.4.3/tldextract/py.typed
--rw-r--r--   0 john       (501) staff       (20)     1541 2023-05-18 00:31:14.000000 tldextract-3.4.3/tldextract/remote.py
--rw-r--r--   0 john       (501) staff       (20)     3400 2023-05-18 18:25:10.000000 tldextract-3.4.3/tldextract/suffix_list.py
--rw-r--r--   0 john       (501) staff       (20)    15971 2023-05-18 18:25:10.000000 tldextract-3.4.3/tldextract/tldextract.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-18 18:35:52.241472 tldextract-3.4.3/tldextract.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     2188 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      802 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       51 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)       56 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       11 2023-05-18 18:35:52.000000 tldextract-3.4.3/tldextract.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)      676 2023-05-18 18:25:10.000000 tldextract-3.4.3/tox.ini
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.880680 tldextract-3.4.4/
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.868456 tldextract-3.4.4/.github/
+-rw-r--r--   0 john       (501) staff       (20)       25 2022-06-05 23:30:19.000000 tldextract-3.4.4/.github/FUNDING.yml
+-rw-r--r--   0 john       (501) staff       (20)      129 2022-05-03 19:53:33.000000 tldextract-3.4.4/.gitignore
+-rw-r--r--   0 john       (501) staff       (20)      469 2023-01-14 03:27:06.000000 tldextract-3.4.4/.travis.yml
+-rw-r--r--   0 john       (501) staff       (20)    13779 2023-05-20 00:30:51.000000 tldextract-3.4.4/CHANGELOG.md
+-rw-r--r--   0 john       (501) staff       (20)     1522 2022-05-03 19:53:33.000000 tldextract-3.4.4/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)      116 2022-05-03 19:53:33.000000 tldextract-3.4.4/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     2188 2023-05-20 00:33:31.880953 tldextract-3.4.4/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     9874 2023-05-13 22:04:35.000000 tldextract-3.4.4/README.md
+-rw-r--r--   0 john       (501) staff       (20)       68 2023-05-17 23:47:07.000000 tldextract-3.4.4/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)       37 2022-05-03 19:53:33.000000 tldextract-3.4.4/pytest.ini
+-rw-r--r--   0 john       (501) staff       (20)      327 2023-05-20 00:33:31.882174 tldextract-3.4.4/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     2780 2023-05-20 00:25:26.000000 tldextract-3.4.4/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.871747 tldextract-3.4.4/tests/
+-rw-r--r--   0 john       (501) staff       (20)       21 2023-05-20 00:25:26.000000 tldextract-3.4.4/tests/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      783 2022-06-05 23:30:19.000000 tldextract-3.4.4/tests/cli_test.py
+-rw-r--r--   0 john       (501) staff       (20)      435 2023-05-20 00:25:26.000000 tldextract-3.4.4/tests/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)     1935 2022-09-20 19:51:12.000000 tldextract-3.4.4/tests/custom_suffix_test.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.872234 tldextract-3.4.4/tests/fixtures/
+-rw-r--r--   0 john       (501) staff       (20)       31 2021-01-11 20:42:27.000000 tldextract-3.4.4/tests/fixtures/fake_suffix_list_fixture.dat
+-rw-r--r--   0 john       (501) staff       (20)      248 2022-06-05 23:30:19.000000 tldextract-3.4.4/tests/integration_test.py
+-rw-r--r--   0 john       (501) staff       (20)    14314 2023-05-20 00:30:02.000000 tldextract-3.4.4/tests/main_test.py
+-rw-r--r--   0 john       (501) staff       (20)     3420 2023-05-20 00:25:26.000000 tldextract-3.4.4/tests/test_cache.py
+-rw-r--r--   0 john       (501) staff       (20)     1545 2023-05-20 00:25:26.000000 tldextract-3.4.4/tests/test_parallel.py
+-rw-r--r--   0 john       (501) staff       (20)     1502 2023-05-20 00:25:26.000000 tldextract-3.4.4/tests/test_trie.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.877445 tldextract-3.4.4/tldextract/
+-rw-r--r--   0 john       (501) staff       (20)   238022 2023-05-13 22:04:35.000000 tldextract-3.4.4/tldextract/.tld_set_snapshot
+-rw-r--r--   0 john       (501) staff       (20)      216 2023-01-27 07:03:29.000000 tldextract-3.4.4/tldextract/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)       90 2022-06-05 23:36:58.000000 tldextract-3.4.4/tldextract/__main__.py
+-rw-r--r--   0 john       (501) staff       (20)      160 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract/_version.py
+-rw-r--r--   0 john       (501) staff       (20)     8725 2023-05-20 00:25:26.000000 tldextract-3.4.4/tldextract/cache.py
+-rw-r--r--   0 john       (501) staff       (20)     2416 2023-05-20 00:25:26.000000 tldextract-3.4.4/tldextract/cli.py
+-rw-r--r--   0 john       (501) staff       (20)        0 2022-05-03 19:53:33.000000 tldextract-3.4.4/tldextract/py.typed
+-rw-r--r--   0 john       (501) staff       (20)     1541 2023-05-20 00:25:26.000000 tldextract-3.4.4/tldextract/remote.py
+-rw-r--r--   0 john       (501) staff       (20)     3400 2023-05-20 00:25:26.000000 tldextract-3.4.4/tldextract/suffix_list.py
+-rw-r--r--   0 john       (501) staff       (20)    16095 2023-05-20 00:30:02.000000 tldextract-3.4.4/tldextract/tldextract.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-20 00:33:31.880228 tldextract-3.4.4/tldextract.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     2188 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      802 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       51 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)       56 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       11 2023-05-20 00:33:31.000000 tldextract-3.4.4/tldextract.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)      676 2023-05-18 18:25:10.000000 tldextract-3.4.4/tox.ini
```

### Comparing `tldextract-3.4.3/CHANGELOG.md` & `tldextract-3.4.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # tldextract Changelog
 
 After upgrading, update your cache file by deleting it or via `tldextract
 --update`.
 
+## 3.4.4 (2023-05-19)
+
+* Bugfixes
+  * Honor private domains flag on `self`, not only when passed to `__call__` ([#289](https://github.com/john-kurkowski/tldextract/issues/289))
+
 ## 3.4.3 (2023-05-18)
 
 * Bugfixes
   * Speed up 10-15% over all inputs
     * Refactor `suffix_index()` to use a trie ([#285](https://github.com/john-kurkowski/tldextract/issues/285))
-  * Docs
-    * Adopt PEP257 doc style
+* Docs
+  * Adopt PEP257 doc style
 
 ## 3.4.2 (2023-05-16)
 
 * Bugfixes
   * Speed up 10-40% on "average" inputs, and even more on pathological inputs, like long subdomains
-    * Optimize `suffix_index()` ([#283](https://github.com/john-kurkowski/tldextract/issues/283))
-    * Optimize netloc extraction ([#284](https://github.com/john-kurkowski/tldextract/issues/284))
+    * Optimize `suffix_index()`: search from right to left ([#283](https://github.com/john-kurkowski/tldextract/issues/283))
+    * Optimize netloc extraction: switch from regex to if/else ([#284](https://github.com/john-kurkowski/tldextract/issues/284))
 
 ## 3.4.1 (2023-04-26)
 
 * Bugfixes
   * Fix Pyright not finding tldextract public interface ([#279](https://github.com/john-kurkowski/tldextract/issues/279))
   * Fix various Pyright checks
   * Use SPDX license identifier ([#280](https://github.com/john-kurkowski/tldextract/issues/280))
```

### Comparing `tldextract-3.4.3/LICENSE` & `tldextract-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/PKG-INFO` & `tldextract-3.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.3
+Version: 3.4.4
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
 License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tldextract-3.4.3/README.md` & `tldextract-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/setup.py` & `tldextract-3.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tests/cli_test.py` & `tldextract-3.4.4/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tests/custom_suffix_test.py` & `tldextract-3.4.4/tests/custom_suffix_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tests/main_test.py` & `tldextract-3.4.4/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,14 +380,25 @@
     responses.add(responses.GET, server, status=408)
     cache = DiskCache(tmpdir)
 
     with pytest.raises(SuffixListNotFound):
         tldextract.suffix_list.find_first_response(cache, [server], 5)
 
 
+def test_include_psl_private_domain_attr():
+    extract_private = tldextract.TLDExtract(include_psl_private_domains=True)
+    extract_public = tldextract.TLDExtract(include_psl_private_domains=False)
+    assert extract_private("foo.uk.com") == ExtractResult(
+        subdomain="", domain="foo", suffix="uk.com"
+    )
+    assert extract_public("foo.uk.com") == ExtractResult(
+        subdomain="foo", domain="uk", suffix="com"
+    )
+
+
 def test_tlds_property():
     extract_private = tldextract.TLDExtract(
         cache_dir=None, suffix_list_urls=(), include_psl_private_domains=True
     )
     extract_public = tldextract.TLDExtract(
         cache_dir=None, suffix_list_urls=(), include_psl_private_domains=False
     )
```

### Comparing `tldextract-3.4.3/tests/test_cache.py` & `tldextract-3.4.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tests/test_parallel.py` & `tldextract-3.4.4/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tests/test_trie.py` & `tldextract-3.4.4/tests/test_trie.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/.tld_set_snapshot` & `tldextract-3.4.4/tldextract/.tld_set_snapshot`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/cache.py` & `tldextract-3.4.4/tldextract/cache.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/cli.py` & `tldextract-3.4.4/tldextract/cli.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/remote.py` & `tldextract-3.4.4/tldextract/remote.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/suffix_list.py` & `tldextract-3.4.4/tldextract/suffix_list.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tldextract/tldextract.py` & `tldextract-3.4.4/tldextract/tldextract.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,17 @@
     def suffix_index(
         self, spl: List[str], include_psl_private_domains: Optional[bool] = None
     ) -> int:
         """Return the index of the first suffix label.
 
         Returns len(spl) if no suffix is found.
         """
+        if include_psl_private_domains is None:
+            include_psl_private_domains = self.include_psl_private_domains
+
         node = (
             self.tlds_incl_private_trie
             if include_psl_private_domains
             else self.tlds_excl_private_trie
         )
         i = len(spl)
         j = i
```

### Comparing `tldextract-3.4.3/tldextract.egg-info/PKG-INFO` & `tldextract-3.4.4/tldextract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.3
+Version: 3.4.4
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
 License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tldextract-3.4.3/tldextract.egg-info/SOURCES.txt` & `tldextract-3.4.4/tldextract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.3/tox.ini` & `tldextract-3.4.4/tox.ini`

 * *Files identical despite different names*

