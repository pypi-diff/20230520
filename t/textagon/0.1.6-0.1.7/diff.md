# Comparing `tmp/textagon-0.1.6.tar.gz` & `tmp/textagon-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.6.tar", last modified: Sat May 20 02:08:20 2023, max compression
+gzip compressed data, was "textagon-0.1.7.tar", last modified: Sat May 20 03:33:23 2023, max compression
```

## Comparing `textagon-0.1.6.tar` & `textagon-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.747487 textagon-0.1.6/
--rw-rw-rw-   0        0        0      181 2023-05-20 02:08:20.747487 textagon-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-20 02:08:20.747487 textagon-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-20 01:51:48.000000 textagon-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.630220 textagon-0.1.6/textagon/
--rw-rw-rw-   0        0        0      218 2023-05-20 01:44:59.000000 textagon-0.1.6/textagon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.616546 textagon-0.1.6/textagon/external/
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.616546 textagon-0.1.6/textagon/external/extracted/
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.647225 textagon-0.1.6/textagon/external/extracted/WNAffect-master/
--rw-rw-rw-   0        0        0    33762 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/WNAffect-master/README.md
--rw-rw-rw-   0        0        0     2953 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/WNAffect-master/emotion.py
--rw-rw-rw-   0        0        0     3523 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/WNAffect-master/wnaffect.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.698147 textagon-0.1.6/textagon/external/extracted/wn-domains/
--rw-rw-rw-   0        0        0    84063 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf
--rw-rw-rw-   0        0        0     2247 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/README
--rw-rw-rw-   0        0        0    47416 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf
--rw-rw-rw-   0        0        0     8688 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf
--rw-rw-rw-   0        0        0    39740 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf
--rw-rw-rw-   0        0        0    51492 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf
--rw-rw-rw-   0        0        0     2278 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/version-history.txt
--rw-rw-rw-   0        0        0  2213039 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210
--rw-rw-rw-   0        0        0  2543843 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.737482 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/
--rw-rw-rw-   0        0        0     3788 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/CHANGES
--rw-rw-rw-   0        0        0     6176 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/INSTALL
--rw-rw-rw-   0        0        0     1625 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/LICENSE
--rw-rw-rw-   0        0        0     7217 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/Makefile
--rw-rw-rw-   0        0        0    11453 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README
--rw-rw-rw-   0        0        0     1996 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README.ml
--rw-rw-rw-   0        0        0     1612 2023-05-19 15:50:31.000000 textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README.tcltk
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.746488 textagon-0.1.6/textagon/external/lexicons/
--rw-rw-rw-   0        0        0   477716 2023-05-19 15:50:35.000000 textagon-0.1.6/textagon/external/lexicons/Lexicons_v5.zip
--rw-rw-rw-   0        0        0    43255 2023-05-19 15:50:35.000000 textagon-0.1.6/textagon/external/lexicons/exclusions.txt
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.6/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0      309 2023-05-19 22:15:17.000000 textagon-0.1.6/textagon/post_install.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.6/textagon/process-text.py
--rw-rw-rw-   0        0        0    26155 2023-05-20 02:05:19.000000 textagon-0.1.6/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:20.639225 textagon-0.1.6/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 02:08:20.000000 textagon-0.1.6/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.568892 textagon-0.1.7/
+-rw-rw-rw-   0        0        0      181 2023-05-20 03:33:23.567892 textagon-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:33:23.568892 textagon-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-20 03:33:14.000000 textagon-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.400491 textagon-0.1.7/textagon/
+-rw-rw-rw-   0        0        0      218 2023-05-20 01:44:59.000000 textagon-0.1.7/textagon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.378476 textagon-0.1.7/textagon/external/
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.377477 textagon-0.1.7/textagon/external/extracted/
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.429484 textagon-0.1.7/textagon/external/extracted/WNAffect-master/
+-rw-rw-rw-   0        0        0    33762 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/WNAffect-master/README.md
+-rw-rw-rw-   0        0        0     2953 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/WNAffect-master/emotion.py
+-rw-rw-rw-   0        0        0     3523 2023-05-20 03:32:24.000000 textagon-0.1.7/textagon/external/extracted/WNAffect-master/wnaffect.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.495635 textagon-0.1.7/textagon/external/extracted/wn-domains/
+-rw-rw-rw-   0        0        0    84063 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf
+-rw-rw-rw-   0        0        0     2247 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/README
+-rw-rw-rw-   0        0        0    47416 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf
+-rw-rw-rw-   0        0        0     8688 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf
+-rw-rw-rw-   0        0        0    39740 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf
+-rw-rw-rw-   0        0        0    51492 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf
+-rw-rw-rw-   0        0        0     2278 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/version-history.txt
+-rw-rw-rw-   0        0        0  2213039 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210
+-rw-rw-rw-   0        0        0  2543843 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.542898 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/
+-rw-rw-rw-   0        0        0     3788 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/CHANGES
+-rw-rw-rw-   0        0        0     6176 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/INSTALL
+-rw-rw-rw-   0        0        0     1625 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/LICENSE
+-rw-rw-rw-   0        0        0     7217 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/Makefile
+-rw-rw-rw-   0        0        0    11453 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README
+-rw-rw-rw-   0        0        0     1996 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README.ml
+-rw-rw-rw-   0        0        0     1612 2023-05-19 15:50:31.000000 textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README.tcltk
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.566896 textagon-0.1.7/textagon/external/lexicons/
+-rw-rw-rw-   0        0        0   477716 2023-05-19 15:50:35.000000 textagon-0.1.7/textagon/external/lexicons/Lexicons_v5.zip
+-rw-rw-rw-   0        0        0    43255 2023-05-19 15:50:35.000000 textagon-0.1.7/textagon/external/lexicons/exclusions.txt
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.7/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0      309 2023-05-19 22:15:17.000000 textagon-0.1.7/textagon/post_install.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.7/textagon/process-text.py
+-rw-rw-rw-   0        0        0    26155 2023-05-20 02:05:19.000000 textagon-0.1.7/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:33:23.415476 textagon-0.1.7/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 03:33:23.000000 textagon-0.1.7/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.6/setup.py` & `textagon-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'textagon',
-    version = '0.1.6',
+    version = '0.1.7',
     packages = find_packages(),
     description = 'Start building textagon',
     author = 'Mendoza',
     classifiers=[
         "License :: OSI Approved :: Python Software Foundation License"
     ],
     install_requires=[
```

### Comparing `textagon-0.1.6/textagon/external/extracted/WNAffect-master/README.md` & `textagon-0.1.7/textagon/external/extracted/WNAffect-master/README.md`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/WNAffect-master/emotion.py` & `textagon-0.1.7/textagon/external/extracted/WNAffect-master/emotion.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/WNAffect-master/wnaffect.py` & `textagon-0.1.7/textagon/external/extracted/WNAffect-master/wnaffect.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
 class WNAffect:
     """WordNet-Affect ressource."""
     
     def __init__(self, wordnet16_dir, wn_domains_dir):
         """Initializes the WordNet-Affect object."""
         
-        cwd = os.getcwd()
-        nltk.data.path.append(cwd)
-        wn16_path = "{0}/dict".format(wordnet16_dir)
+        wn16_path = os.path.join(wordnet16_dir, 'dict')
+        nltk.data.path.append(os.path.dirname(wn16_path))
         self.wn16 = WordNetCorpusReader(wn16_path, nltk.data.find(wn16_path))
         self.flat_pos = {'NN':'NN', 'NNS':'NN', 'JJ':'JJ', 'JJR':'JJ', 'JJS':'JJ', 'RB':'RB', 'RBR':'RB', 'RBS':'RB', 'VB':'VB', 'VBD':'VB', 'VGB':'VB', 'VBN':'VB', 'VBP':'VB', 'VBZ':'VB'}
         self.wn_pos = {'NN':self.wn16.NOUN, 'JJ':self.wn16.ADJ, 'VB':self.wn16.VERB, 'RB':self.wn16.ADV}
         self._load_emotions(wn_domains_dir)
         self.synsets = self._load_synsets(wn_domains_dir)
```

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf` & `textagon-0.1.7/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/README` & `textagon-0.1.7/textagon/external/extracted/wn-domains/README`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf` & `textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf` & `textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf` & `textagon-0.1.7/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf` & `textagon-0.1.7/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/version-history.txt` & `textagon-0.1.7/textagon/external/extracted/wn-domains/version-history.txt`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210` & `textagon-0.1.7/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223` & `textagon-0.1.7/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/CHANGES` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/CHANGES`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/INSTALL` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/INSTALL`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/LICENSE` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/Makefile` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/Makefile`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README.ml` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README.ml`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/extracted/wordnet-1.6/README.tcltk` & `textagon-0.1.7/textagon/external/extracted/wordnet-1.6/README.tcltk`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/lexicons/Lexicons_v5.zip` & `textagon-0.1.7/textagon/external/lexicons/Lexicons_v5.zip`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/external/lexicons/exclusions.txt` & `textagon-0.1.7/textagon/external/lexicons/exclusions.txt`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/process-text.py` & `textagon-0.1.7/textagon/process-text.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon/textagon.py` & `textagon-0.1.7/textagon/textagon.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.6/textagon.egg-info/SOURCES.txt` & `textagon-0.1.7/textagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

