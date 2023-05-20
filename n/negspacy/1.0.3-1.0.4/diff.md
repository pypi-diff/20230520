# Comparing `tmp/negspacy-1.0.3.tar.gz` & `tmp/negspacy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/negspacy-1.0.3.tar", last modified: Wed May 25 19:05:55 2022, max compression
+gzip compressed data, was "negspacy-1.0.4.tar", last modified: Sat May 20 18:29:18 2023, max compression
```

## Comparing `negspacy-1.0.3.tar` & `negspacy-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 jeno       (501) staff       (20)        0 2022-05-25 19:05:55.584921 negspacy-1.0.3/
--rw-r--r--   0 jeno       (501) staff       (20)     7975 2022-05-25 19:05:55.584520 negspacy-1.0.3/PKG-INFO
--rw-r--r--   0 jeno       (501) staff       (20)     5752 2021-05-07 20:29:56.000000 negspacy-1.0.3/README.md
-drwxr-xr-x   0 jeno       (501) staff       (20)        0 2022-05-25 19:05:55.581490 negspacy-1.0.3/negspacy/
--rw-r--r--   0 jeno       (501) staff       (20)        0 2019-08-09 01:31:08.000000 negspacy-1.0.3/negspacy/__init__.py
--rw-r--r--   0 jeno       (501) staff       (20)    11722 2021-02-22 17:08:30.000000 negspacy-1.0.3/negspacy/negation.py
--rw-r--r--   0 jeno       (501) staff       (20)     4954 2021-02-22 17:08:30.000000 negspacy-1.0.3/negspacy/termsets.py
--rw-r--r--   0 jeno       (501) staff       (20)     4326 2022-01-20 12:55:53.000000 negspacy-1.0.3/negspacy/test.py
--rw-r--r--   0 jeno       (501) staff       (20)     3829 2021-10-22 20:37:15.000000 negspacy-1.0.3/negspacy/test_scispacy_dep.py
-drwxr-xr-x   0 jeno       (501) staff       (20)        0 2022-05-25 19:05:55.583814 negspacy-1.0.3/negspacy.egg-info/
--rw-r--r--   0 jeno       (501) staff       (20)     7975 2022-05-25 19:05:55.000000 negspacy-1.0.3/negspacy.egg-info/PKG-INFO
--rw-r--r--   0 jeno       (501) staff       (20)      287 2022-05-25 19:05:55.000000 negspacy-1.0.3/negspacy.egg-info/SOURCES.txt
--rw-r--r--   0 jeno       (501) staff       (20)        1 2022-05-25 19:05:55.000000 negspacy-1.0.3/negspacy.egg-info/dependency_links.txt
--rw-r--r--   0 jeno       (501) staff       (20)       20 2022-05-25 19:05:55.000000 negspacy-1.0.3/negspacy.egg-info/requires.txt
--rw-r--r--   0 jeno       (501) staff       (20)        9 2022-05-25 19:05:55.000000 negspacy-1.0.3/negspacy.egg-info/top_level.txt
--rw-r--r--   0 jeno       (501) staff       (20)       38 2022-05-25 19:05:55.585059 negspacy-1.0.3/setup.cfg
--rw-r--r--   0 jeno       (501) staff       (20)     1146 2022-05-25 18:27:43.000000 negspacy-1.0.3/setup.py
+drwxr-xr-x   0 jeno       (502) staff       (20)        0 2023-05-20 18:29:18.305829 negspacy-1.0.4/
+-rw-r--r--   0 jeno       (502) staff       (20)     1069 2023-03-25 16:23:20.000000 negspacy-1.0.4/LICENSE
+-rw-r--r--   0 jeno       (502) staff       (20)     6856 2023-05-20 18:29:18.306129 negspacy-1.0.4/PKG-INFO
+-rw-r--r--   0 jeno       (502) staff       (20)     5752 2023-03-25 16:23:20.000000 negspacy-1.0.4/README.md
+drwxr-xr-x   0 jeno       (502) staff       (20)        0 2023-05-20 18:29:18.302101 negspacy-1.0.4/negspacy/
+-rw-r--r--   0 jeno       (502) staff       (20)        0 2023-03-25 16:23:20.000000 negspacy-1.0.4/negspacy/__init__.py
+-rw-r--r--   0 jeno       (502) staff       (20)    11722 2023-03-25 16:23:20.000000 negspacy-1.0.4/negspacy/negation.py
+-rw-r--r--   0 jeno       (502) staff       (20)    12441 2023-03-25 16:23:36.000000 negspacy-1.0.4/negspacy/termsets.py
+-rw-r--r--   0 jeno       (502) staff       (20)     4326 2023-03-25 16:23:20.000000 negspacy-1.0.4/negspacy/test.py
+-rw-r--r--   0 jeno       (502) staff       (20)     3829 2023-03-25 16:23:20.000000 negspacy-1.0.4/negspacy/test_scispacy_dep.py
+drwxr-xr-x   0 jeno       (502) staff       (20)        0 2023-05-20 18:29:18.305220 negspacy-1.0.4/negspacy.egg-info/
+-rw-r--r--   0 jeno       (502) staff       (20)     6856 2023-05-20 18:29:18.000000 negspacy-1.0.4/negspacy.egg-info/PKG-INFO
+-rw-r--r--   0 jeno       (502) staff       (20)      320 2023-05-20 18:29:18.000000 negspacy-1.0.4/negspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 jeno       (502) staff       (20)        1 2023-05-20 18:29:18.000000 negspacy-1.0.4/negspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 jeno       (502) staff       (20)       20 2023-05-20 18:29:18.000000 negspacy-1.0.4/negspacy.egg-info/requires.txt
+-rw-r--r--   0 jeno       (502) staff       (20)        9 2023-05-20 18:29:18.000000 negspacy-1.0.4/negspacy.egg-info/top_level.txt
+-rw-r--r--   0 jeno       (502) staff       (20)       80 2023-05-18 01:07:16.000000 negspacy-1.0.4/pyproject.toml
+-rw-r--r--   0 jeno       (502) staff       (20)     1024 2023-05-20 18:29:18.307708 negspacy-1.0.4/setup.cfg
+-rw-r--r--   0 jeno       (502) staff       (20)     1475 2023-05-18 01:00:49.000000 negspacy-1.0.4/setup.py
```

### Comparing `negspacy-1.0.3/PKG-INFO` & `negspacy-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,202 +1,210 @@
 Metadata-Version: 2.1
 Name: negspacy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A spaCy pipeline object for negation.
 Home-page: https://github.com/jenojp/negspacy
 Author: Jeno Pizarro
 Author-email: jenopizzaro@gmail.com
 License: MIT
-Description: 
-        <p align="center"><img width="40%" src="docs/icon.png" /></p>
-        
-        
-        # negspacy: negation for spaCy
-        
-        [![Build Status](https://dev.azure.com/jenopizzaro/negspacy/_apis/build/status/jenojp.negspacy?branchName=master)](https://dev.azure.com/jenopizzaro/negspacy/_build/latest?definitionId=2&branchName=master) [![Built with spaCy](https://img.shields.io/badge/made%20with%20❤%20and-spaCy-09a3d5.svg)](https://spacy.io) [![pypi Version](https://img.shields.io/pypi/v/negspacy.svg?style=flat-square)](https://pypi.org/project/negspacy/) [![DOI](https://zenodo.org/badge/201071164.svg)](https://zenodo.org/badge/latestdoi/201071164) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
-        
-        spaCy pipeline object for negating concepts in text. Based on the NegEx algorithm.
-        
-        ***NegEx - A Simple Algorithm for Identifying Negated Findings and Diseases in Discharge Summaries
-        Chapman, Bridewell, Hanbury, Cooper, Buchanan***
-        [https://doi.org/10.1006/jbin.2001.1029](https://doi.org/10.1006/jbin.2001.1029)
-        
-        ## What's new
-        Version 1.0 is a major version update providing support for spaCy 3.0's new interface for adding pipeline components. As a result, it is not backwards compatible with previous versions of negspacy.
-        
-        If your project uses spaCy 2.3.5 or earlier, you will need to use version 0.1.9. See [archived readme](https://github.com/jenojp/negspacy/blob/v0.1.9_spacy_2.3.5/README.md).
-        
-        ## Installation and usage
-        Install the library.
-        ```bash
-        pip install negspacy
-        ```
-        
-        Import library and spaCy.
-        ```python
-        import spacy
-        from negspacy.negation import Negex
-        ```
-        
-        Load spacy language model. Add negspacy pipeline object. Filtering on entity types is optional.
-        ```python
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})
-        
-        ```
-        
-        View negations.
-        ```python
-        doc = nlp("She does not like Steve Jobs but likes Apple products.")
-        
-        for e in doc.ents:
-        	print(e.text, e._.negex)
-        ```
-        
-        ```console
-        Steve Jobs True
-        Apple False
-        ```
-        
-        Consider pairing with [scispacy](https://allenai.github.io/scispacy/) to find UMLS concepts in text and process negations.
-        
-        ## NegEx Patterns
-        
-        * **pseudo_negations** - phrases that are false triggers, ambiguous negations, or double negatives
-        * **preceding_negations** - negation phrases that precede an entity
-        * **following_negations** - negation phrases that follow an entity
-        * **termination** - phrases that cut a sentence in parts, for purposes of negation detection (.e.g., "but")
-        
-        ### Termsets
-        
-        Designate termset to use, `en_clinical` is used by default.
-        
-        * `en` = phrases for general english language text
-        * `en_clinical` **DEFAULT** = adds phrases specific to clinical domain to general english
-        * `en_clinical_sensitive` = adds additional phrases to help rule out historical and possibly irrelevant entities
-        
-        To set:
-        ```python
-        from negspacy.negation import Negex
-        from negspacy.termsets import termset
-        
-        ts = termset("en")
-        
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe(
-            "negex",
-            config={
-                "neg_termset":ts.get_patterns()
-            }
-        )
-        
-        ```
-        
-        ## Additional Functionality
-        
-        ### Change patterns or view patterns in use
-        
-        Replace all patterns with your own set
-        ```python
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe(
-            "negex", 
-            config={
-                "neg_termset":{
-                    "pseudo_negations": ["might not"],
-                    "preceding_negations": ["not"],
-                    "following_negations":["declined"],
-                    "termination": ["but","however"]
-                }
-            }
-            )
-        ```
-        
-        Add and remove individual patterns on the fly from built-in termsets
-        ```python
-        from negspacy.termsets import termset
-        ts = termset("en")
-        ts.add_patterns({
-                    "pseudo_negations": ["my favorite pattern"],
-                    "termination": ["these are", "great patterns", "but"],
-                    "preceding_negations": ["wow a negation"],
-                    "following_negations": ["extra negation"],
-                })
-        #OR
-        ts.remove_patterns(
-                {
-                    "termination": ["these are", "great patterns"],
-                    "pseudo_negations": ["my favorite pattern"],
-                    "preceding_negations": ["denied", "wow a negation"],
-                    "following_negations": ["unlikely", "extra negation"],
-                }
-            )
-        ```
-        
-        View patterns in use
-        ```python
-        from negspacy.termsets import termset
-        ts = termset("en_clinical")
-        print(ts.get_patterns())
-        ```
-        
-        
-        ### Negations in noun chunks
-        
-        Depending on the Named Entity Recognition model you are using, you _may_ have negations "chunked together" with nouns. For example:
-        ```python
-        nlp = spacy.load("en_core_sci_sm")
-        doc = nlp("There is no headache.")
-        for e in doc.ents:
-            print(e.text)
-        
-        # no headache
-        ```
-        This would cause the Negex algorithm to miss the preceding negation. To account for this, you can add a ```chunk_prefix```:
-        
-        ```python
-        nlp = spacy.load("en_core_sci_sm")
-        ts = termset("en_clinical")
-        nlp.add_pipe(
-            "negex",
-            config={
-                "chunk_prefix": ["no"],
-            },
-            last=True,
-        )
-        doc = nlp("There is no headache.")
-        for e in doc.ents:
-            print(e.text, e._.negex)
-        
-        # no headache True
-        ```
-        
-        
-        ## Contributing
-        [contributing](https://github.com/jenojp/negspacy/blob/master/CONTRIBUTING.md)
-        
-        ## Authors
-        * Jeno Pizarro
-        
-        ## License
-        [license](https://github.com/jenojp/negspacy/blob/master/LICENSE)
-        
-        ## Other libraries
-        
-        This library is featured in the [spaCy Universe](https://spacy.io/universe). Check it out for other useful libraries and inspiration.
-        
-        If you're looking for a spaCy pipeline object to extract values that correspond to a named entity (e.g., birth dates, account numbers, or laboratory results) take a look at [extractacy](https://github.com/jenojp/extractacy).
-        
-        <p align="left"><img width="40%" src="https://github.com/jenojp/extractacy/blob/master/docs/icon.png?raw=true" /></p>
-        
 Keywords: nlp spacy SpaCy negation
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<p align="center"><img width="40%" src="docs/icon.png" /></p>
+
+
+# negspacy: negation for spaCy
+
+[![Build Status](https://dev.azure.com/jenopizzaro/negspacy/_apis/build/status/jenojp.negspacy?branchName=master)](https://dev.azure.com/jenopizzaro/negspacy/_build/latest?definitionId=2&branchName=master) [![Built with spaCy](https://img.shields.io/badge/made%20with%20❤%20and-spaCy-09a3d5.svg)](https://spacy.io) [![pypi Version](https://img.shields.io/pypi/v/negspacy.svg?style=flat-square)](https://pypi.org/project/negspacy/) [![DOI](https://zenodo.org/badge/201071164.svg)](https://zenodo.org/badge/latestdoi/201071164) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
+
+spaCy pipeline object for negating concepts in text. Based on the NegEx algorithm.
+
+***NegEx - A Simple Algorithm for Identifying Negated Findings and Diseases in Discharge Summaries
+Chapman, Bridewell, Hanbury, Cooper, Buchanan***
+[https://doi.org/10.1006/jbin.2001.1029](https://doi.org/10.1006/jbin.2001.1029)
+
+## What's new
+Version 1.0 is a major version update providing support for spaCy 3.0's new interface for adding pipeline components. As a result, it is not backwards compatible with previous versions of negspacy.
+
+If your project uses spaCy 2.3.5 or earlier, you will need to use version 0.1.9. See [archived readme](https://github.com/jenojp/negspacy/blob/v0.1.9_spacy_2.3.5/README.md).
+
+## Installation and usage
+Install the library.
+```bash
+pip install negspacy
+```
+
+Import library and spaCy.
+```python
+import spacy
+from negspacy.negation import Negex
+```
+
+Load spacy language model. Add negspacy pipeline object. Filtering on entity types is optional.
+```python
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})
+
+```
+
+View negations.
+```python
+doc = nlp("She does not like Steve Jobs but likes Apple products.")
+
+for e in doc.ents:
+	print(e.text, e._.negex)
+```
+
+```console
+Steve Jobs True
+Apple False
+```
+
+Consider pairing with [scispacy](https://allenai.github.io/scispacy/) to find UMLS concepts in text and process negations.
+
+## NegEx Patterns
+
+* **pseudo_negations** - phrases that are false triggers, ambiguous negations, or double negatives
+* **preceding_negations** - negation phrases that precede an entity
+* **following_negations** - negation phrases that follow an entity
+* **termination** - phrases that cut a sentence in parts, for purposes of negation detection (.e.g., "but")
+
+### Termsets
+
+Designate termset to use, `en_clinical` is used by default.
+
+* `en` = phrases for general english language text
+* `en_clinical` **DEFAULT** = adds phrases specific to clinical domain to general english
+* `en_clinical_sensitive` = adds additional phrases to help rule out historical and possibly irrelevant entities
+
+To set:
+```python
+from negspacy.negation import Negex
+from negspacy.termsets import termset
+
+ts = termset("en")
+
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe(
+    "negex",
+    config={
+        "neg_termset":ts.get_patterns()
+    }
+)
+
+```
+
+## Additional Functionality
+
+### Change patterns or view patterns in use
+
+Replace all patterns with your own set
+```python
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe(
+    "negex", 
+    config={
+        "neg_termset":{
+            "pseudo_negations": ["might not"],
+            "preceding_negations": ["not"],
+            "following_negations":["declined"],
+            "termination": ["but","however"]
+        }
+    }
+    )
+```
+
+Add and remove individual patterns on the fly from built-in termsets
+```python
+from negspacy.termsets import termset
+ts = termset("en")
+ts.add_patterns({
+            "pseudo_negations": ["my favorite pattern"],
+            "termination": ["these are", "great patterns", "but"],
+            "preceding_negations": ["wow a negation"],
+            "following_negations": ["extra negation"],
+        })
+#OR
+ts.remove_patterns(
+        {
+            "termination": ["these are", "great patterns"],
+            "pseudo_negations": ["my favorite pattern"],
+            "preceding_negations": ["denied", "wow a negation"],
+            "following_negations": ["unlikely", "extra negation"],
+        }
+    )
+```
+
+View patterns in use
+```python
+from negspacy.termsets import termset
+ts = termset("en_clinical")
+print(ts.get_patterns())
+```
+
+
+### Negations in noun chunks
+
+Depending on the Named Entity Recognition model you are using, you _may_ have negations "chunked together" with nouns. For example:
+```python
+nlp = spacy.load("en_core_sci_sm")
+doc = nlp("There is no headache.")
+for e in doc.ents:
+    print(e.text)
+
+# no headache
+```
+This would cause the Negex algorithm to miss the preceding negation. To account for this, you can add a ```chunk_prefix```:
+
+```python
+nlp = spacy.load("en_core_sci_sm")
+ts = termset("en_clinical")
+nlp.add_pipe(
+    "negex",
+    config={
+        "chunk_prefix": ["no"],
+    },
+    last=True,
+)
+doc = nlp("There is no headache.")
+for e in doc.ents:
+    print(e.text, e._.negex)
+
+# no headache True
+```
+
+
+## Contributing
+[contributing](https://github.com/jenojp/negspacy/blob/master/CONTRIBUTING.md)
+
+## Authors
+* Jeno Pizarro
+
+## License
+[license](https://github.com/jenojp/negspacy/blob/master/LICENSE)
+
+## Other libraries
+
+This library is featured in the [spaCy Universe](https://spacy.io/universe). Check it out for other useful libraries and inspiration.
+
+If you're looking for a spaCy pipeline object to extract values that correspond to a named entity (e.g., birth dates, account numbers, or laboratory results) take a look at [extractacy](https://github.com/jenojp/extractacy).
+
+<p align="left"><img width="40%" src="https://github.com/jenojp/extractacy/blob/master/docs/icon.png?raw=true" /></p>
```

### Comparing `negspacy-1.0.3/README.md` & `negspacy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `negspacy-1.0.3/negspacy/negation.py` & `negspacy-1.0.4/negspacy/negation.py`

 * *Files identical despite different names*

### Comparing `negspacy-1.0.3/negspacy/test.py` & `negspacy-1.0.4/negspacy/test.py`

 * *Files identical despite different names*

### Comparing `negspacy-1.0.3/negspacy/test_scispacy_dep.py` & `negspacy-1.0.4/negspacy/test_scispacy_dep.py`

 * *Files identical despite different names*

### Comparing `negspacy-1.0.3/negspacy.egg-info/PKG-INFO` & `negspacy-1.0.4/negspacy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,202 +1,210 @@
 Metadata-Version: 2.1
 Name: negspacy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A spaCy pipeline object for negation.
 Home-page: https://github.com/jenojp/negspacy
 Author: Jeno Pizarro
 Author-email: jenopizzaro@gmail.com
 License: MIT
-Description: 
-        <p align="center"><img width="40%" src="docs/icon.png" /></p>
-        
-        
-        # negspacy: negation for spaCy
-        
-        [![Build Status](https://dev.azure.com/jenopizzaro/negspacy/_apis/build/status/jenojp.negspacy?branchName=master)](https://dev.azure.com/jenopizzaro/negspacy/_build/latest?definitionId=2&branchName=master) [![Built with spaCy](https://img.shields.io/badge/made%20with%20❤%20and-spaCy-09a3d5.svg)](https://spacy.io) [![pypi Version](https://img.shields.io/pypi/v/negspacy.svg?style=flat-square)](https://pypi.org/project/negspacy/) [![DOI](https://zenodo.org/badge/201071164.svg)](https://zenodo.org/badge/latestdoi/201071164) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
-        
-        spaCy pipeline object for negating concepts in text. Based on the NegEx algorithm.
-        
-        ***NegEx - A Simple Algorithm for Identifying Negated Findings and Diseases in Discharge Summaries
-        Chapman, Bridewell, Hanbury, Cooper, Buchanan***
-        [https://doi.org/10.1006/jbin.2001.1029](https://doi.org/10.1006/jbin.2001.1029)
-        
-        ## What's new
-        Version 1.0 is a major version update providing support for spaCy 3.0's new interface for adding pipeline components. As a result, it is not backwards compatible with previous versions of negspacy.
-        
-        If your project uses spaCy 2.3.5 or earlier, you will need to use version 0.1.9. See [archived readme](https://github.com/jenojp/negspacy/blob/v0.1.9_spacy_2.3.5/README.md).
-        
-        ## Installation and usage
-        Install the library.
-        ```bash
-        pip install negspacy
-        ```
-        
-        Import library and spaCy.
-        ```python
-        import spacy
-        from negspacy.negation import Negex
-        ```
-        
-        Load spacy language model. Add negspacy pipeline object. Filtering on entity types is optional.
-        ```python
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})
-        
-        ```
-        
-        View negations.
-        ```python
-        doc = nlp("She does not like Steve Jobs but likes Apple products.")
-        
-        for e in doc.ents:
-        	print(e.text, e._.negex)
-        ```
-        
-        ```console
-        Steve Jobs True
-        Apple False
-        ```
-        
-        Consider pairing with [scispacy](https://allenai.github.io/scispacy/) to find UMLS concepts in text and process negations.
-        
-        ## NegEx Patterns
-        
-        * **pseudo_negations** - phrases that are false triggers, ambiguous negations, or double negatives
-        * **preceding_negations** - negation phrases that precede an entity
-        * **following_negations** - negation phrases that follow an entity
-        * **termination** - phrases that cut a sentence in parts, for purposes of negation detection (.e.g., "but")
-        
-        ### Termsets
-        
-        Designate termset to use, `en_clinical` is used by default.
-        
-        * `en` = phrases for general english language text
-        * `en_clinical` **DEFAULT** = adds phrases specific to clinical domain to general english
-        * `en_clinical_sensitive` = adds additional phrases to help rule out historical and possibly irrelevant entities
-        
-        To set:
-        ```python
-        from negspacy.negation import Negex
-        from negspacy.termsets import termset
-        
-        ts = termset("en")
-        
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe(
-            "negex",
-            config={
-                "neg_termset":ts.get_patterns()
-            }
-        )
-        
-        ```
-        
-        ## Additional Functionality
-        
-        ### Change patterns or view patterns in use
-        
-        Replace all patterns with your own set
-        ```python
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe(
-            "negex", 
-            config={
-                "neg_termset":{
-                    "pseudo_negations": ["might not"],
-                    "preceding_negations": ["not"],
-                    "following_negations":["declined"],
-                    "termination": ["but","however"]
-                }
-            }
-            )
-        ```
-        
-        Add and remove individual patterns on the fly from built-in termsets
-        ```python
-        from negspacy.termsets import termset
-        ts = termset("en")
-        ts.add_patterns({
-                    "pseudo_negations": ["my favorite pattern"],
-                    "termination": ["these are", "great patterns", "but"],
-                    "preceding_negations": ["wow a negation"],
-                    "following_negations": ["extra negation"],
-                })
-        #OR
-        ts.remove_patterns(
-                {
-                    "termination": ["these are", "great patterns"],
-                    "pseudo_negations": ["my favorite pattern"],
-                    "preceding_negations": ["denied", "wow a negation"],
-                    "following_negations": ["unlikely", "extra negation"],
-                }
-            )
-        ```
-        
-        View patterns in use
-        ```python
-        from negspacy.termsets import termset
-        ts = termset("en_clinical")
-        print(ts.get_patterns())
-        ```
-        
-        
-        ### Negations in noun chunks
-        
-        Depending on the Named Entity Recognition model you are using, you _may_ have negations "chunked together" with nouns. For example:
-        ```python
-        nlp = spacy.load("en_core_sci_sm")
-        doc = nlp("There is no headache.")
-        for e in doc.ents:
-            print(e.text)
-        
-        # no headache
-        ```
-        This would cause the Negex algorithm to miss the preceding negation. To account for this, you can add a ```chunk_prefix```:
-        
-        ```python
-        nlp = spacy.load("en_core_sci_sm")
-        ts = termset("en_clinical")
-        nlp.add_pipe(
-            "negex",
-            config={
-                "chunk_prefix": ["no"],
-            },
-            last=True,
-        )
-        doc = nlp("There is no headache.")
-        for e in doc.ents:
-            print(e.text, e._.negex)
-        
-        # no headache True
-        ```
-        
-        
-        ## Contributing
-        [contributing](https://github.com/jenojp/negspacy/blob/master/CONTRIBUTING.md)
-        
-        ## Authors
-        * Jeno Pizarro
-        
-        ## License
-        [license](https://github.com/jenojp/negspacy/blob/master/LICENSE)
-        
-        ## Other libraries
-        
-        This library is featured in the [spaCy Universe](https://spacy.io/universe). Check it out for other useful libraries and inspiration.
-        
-        If you're looking for a spaCy pipeline object to extract values that correspond to a named entity (e.g., birth dates, account numbers, or laboratory results) take a look at [extractacy](https://github.com/jenojp/extractacy).
-        
-        <p align="left"><img width="40%" src="https://github.com/jenojp/extractacy/blob/master/docs/icon.png?raw=true" /></p>
-        
 Keywords: nlp spacy SpaCy negation
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<p align="center"><img width="40%" src="docs/icon.png" /></p>
+
+
+# negspacy: negation for spaCy
+
+[![Build Status](https://dev.azure.com/jenopizzaro/negspacy/_apis/build/status/jenojp.negspacy?branchName=master)](https://dev.azure.com/jenopizzaro/negspacy/_build/latest?definitionId=2&branchName=master) [![Built with spaCy](https://img.shields.io/badge/made%20with%20❤%20and-spaCy-09a3d5.svg)](https://spacy.io) [![pypi Version](https://img.shields.io/pypi/v/negspacy.svg?style=flat-square)](https://pypi.org/project/negspacy/) [![DOI](https://zenodo.org/badge/201071164.svg)](https://zenodo.org/badge/latestdoi/201071164) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
+
+spaCy pipeline object for negating concepts in text. Based on the NegEx algorithm.
+
+***NegEx - A Simple Algorithm for Identifying Negated Findings and Diseases in Discharge Summaries
+Chapman, Bridewell, Hanbury, Cooper, Buchanan***
+[https://doi.org/10.1006/jbin.2001.1029](https://doi.org/10.1006/jbin.2001.1029)
+
+## What's new
+Version 1.0 is a major version update providing support for spaCy 3.0's new interface for adding pipeline components. As a result, it is not backwards compatible with previous versions of negspacy.
+
+If your project uses spaCy 2.3.5 or earlier, you will need to use version 0.1.9. See [archived readme](https://github.com/jenojp/negspacy/blob/v0.1.9_spacy_2.3.5/README.md).
+
+## Installation and usage
+Install the library.
+```bash
+pip install negspacy
+```
+
+Import library and spaCy.
+```python
+import spacy
+from negspacy.negation import Negex
+```
+
+Load spacy language model. Add negspacy pipeline object. Filtering on entity types is optional.
+```python
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})
+
+```
+
+View negations.
+```python
+doc = nlp("She does not like Steve Jobs but likes Apple products.")
+
+for e in doc.ents:
+	print(e.text, e._.negex)
+```
+
+```console
+Steve Jobs True
+Apple False
+```
+
+Consider pairing with [scispacy](https://allenai.github.io/scispacy/) to find UMLS concepts in text and process negations.
+
+## NegEx Patterns
+
+* **pseudo_negations** - phrases that are false triggers, ambiguous negations, or double negatives
+* **preceding_negations** - negation phrases that precede an entity
+* **following_negations** - negation phrases that follow an entity
+* **termination** - phrases that cut a sentence in parts, for purposes of negation detection (.e.g., "but")
+
+### Termsets
+
+Designate termset to use, `en_clinical` is used by default.
+
+* `en` = phrases for general english language text
+* `en_clinical` **DEFAULT** = adds phrases specific to clinical domain to general english
+* `en_clinical_sensitive` = adds additional phrases to help rule out historical and possibly irrelevant entities
+
+To set:
+```python
+from negspacy.negation import Negex
+from negspacy.termsets import termset
+
+ts = termset("en")
+
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe(
+    "negex",
+    config={
+        "neg_termset":ts.get_patterns()
+    }
+)
+
+```
+
+## Additional Functionality
+
+### Change patterns or view patterns in use
+
+Replace all patterns with your own set
+```python
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe(
+    "negex", 
+    config={
+        "neg_termset":{
+            "pseudo_negations": ["might not"],
+            "preceding_negations": ["not"],
+            "following_negations":["declined"],
+            "termination": ["but","however"]
+        }
+    }
+    )
+```
+
+Add and remove individual patterns on the fly from built-in termsets
+```python
+from negspacy.termsets import termset
+ts = termset("en")
+ts.add_patterns({
+            "pseudo_negations": ["my favorite pattern"],
+            "termination": ["these are", "great patterns", "but"],
+            "preceding_negations": ["wow a negation"],
+            "following_negations": ["extra negation"],
+        })
+#OR
+ts.remove_patterns(
+        {
+            "termination": ["these are", "great patterns"],
+            "pseudo_negations": ["my favorite pattern"],
+            "preceding_negations": ["denied", "wow a negation"],
+            "following_negations": ["unlikely", "extra negation"],
+        }
+    )
+```
+
+View patterns in use
+```python
+from negspacy.termsets import termset
+ts = termset("en_clinical")
+print(ts.get_patterns())
+```
+
+
+### Negations in noun chunks
+
+Depending on the Named Entity Recognition model you are using, you _may_ have negations "chunked together" with nouns. For example:
+```python
+nlp = spacy.load("en_core_sci_sm")
+doc = nlp("There is no headache.")
+for e in doc.ents:
+    print(e.text)
+
+# no headache
+```
+This would cause the Negex algorithm to miss the preceding negation. To account for this, you can add a ```chunk_prefix```:
+
+```python
+nlp = spacy.load("en_core_sci_sm")
+ts = termset("en_clinical")
+nlp.add_pipe(
+    "negex",
+    config={
+        "chunk_prefix": ["no"],
+    },
+    last=True,
+)
+doc = nlp("There is no headache.")
+for e in doc.ents:
+    print(e.text, e._.negex)
+
+# no headache True
+```
+
+
+## Contributing
+[contributing](https://github.com/jenojp/negspacy/blob/master/CONTRIBUTING.md)
+
+## Authors
+* Jeno Pizarro
+
+## License
+[license](https://github.com/jenojp/negspacy/blob/master/LICENSE)
+
+## Other libraries
+
+This library is featured in the [spaCy Universe](https://spacy.io/universe). Check it out for other useful libraries and inspiration.
+
+If you're looking for a spaCy pipeline object to extract values that correspond to a named entity (e.g., birth dates, account numbers, or laboratory results) take a look at [extractacy](https://github.com/jenojp/extractacy).
+
+<p align="left"><img width="40%" src="https://github.com/jenojp/extractacy/blob/master/docs/icon.png?raw=true" /></p>
```

