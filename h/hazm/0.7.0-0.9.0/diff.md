# Comparing `tmp/hazm-0.7.0.tar.gz` & `tmp/hazm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hazm-0.7.0.tar", last modified: Fri Oct 12 12:01:33 2018, max compression
+gzip compressed data, was "hazm-0.9.0.tar", max compression
```

## Comparing `hazm-0.7.0.tar` & `hazm-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,39 @@
-drwxr-xr-x   0 nournia   (1000) nournia   (1000)        0 2018-10-12 12:01:33.000000 hazm-0.7.0/
-drwxr-xr-x   0 nournia   (1000) nournia   (1000)        0 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm/
--rw-r--r--   0 nournia   (1000) nournia   (1000)      952 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/utils.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)      759 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/Stemmer.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1157 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/TokenSplitter.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     6755 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/InformalNormalizer.py
--rwxr-xr-x   0 nournia   (1000) nournia   (1000)     8803 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/DadeganReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     5105 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/PeykareReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1092 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/VerbValencyReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2718 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/SequenceTagger.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2154 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/QuranCorpusReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     8890 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/TreebankReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)      833 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/PersicaReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)      594 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/SentenceTokenizer.py
--rwxr-xr-x   0 nournia   (1000) nournia   (1000)   116216 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/WikiExtractor.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2163 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/BijankhanReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2676 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/HamshahriReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1409 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/__init__.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1854 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/TNewsReader.py
-drwxr-xr-x   0 nournia   (1000) nournia   (1000)        0 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm/data/
--rw-r--r--   0 nournia   (1000) nournia   (1000)   850556 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/data/words.dat
--rw-r--r--   0 nournia   (1000) nournia   (1000)     3664 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/data/stopwords.dat
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1671 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/data/verbs.dat
--rw-r--r--   0 nournia   (1000) nournia   (1000)      324 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/data/iwords.dat
--rw-r--r--   0 nournia   (1000) nournia   (1000)      328 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/data/iverbs.dat
--rwxr-xr-x   0 nournia   (1000) nournia   (1000)     1217 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/POSTagger.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     6547 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/Lemmatizer.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     7648 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/WordTokenizer.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     6766 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/Normalizer.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     3886 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/DependencyParser.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     1138 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/WikipediaReader.py
--rwxr-xr-x   0 nournia   (1000) nournia   (1000)     1932 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/Chunker.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2223 2018-10-12 03:48:13.000000 hazm-0.7.0/hazm/SentiPersReader.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)     2901 2018-10-12 03:48:13.000000 hazm-0.7.0/README.md
--rw-r--r--   0 nournia   (1000) nournia   (1000)     4161 2018-10-12 12:01:33.000000 hazm-0.7.0/PKG-INFO
--rw-r--r--   0 nournia   (1000) nournia   (1000)     3129 2018-10-12 03:55:25.000000 hazm-0.7.0/README.txt
-drwxr-xr-x   0 nournia   (1000) nournia   (1000)        0 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/
--rw-r--r--   0 nournia   (1000) nournia   (1000)        5 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/top_level.txt
--rw-r--r--   0 nournia   (1000) nournia   (1000)        1 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/dependency_links.txt
--rw-r--r--   0 nournia   (1000) nournia   (1000)      817 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/SOURCES.txt
--rw-r--r--   0 nournia   (1000) nournia   (1000)     4161 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/PKG-INFO
--rw-r--r--   0 nournia   (1000) nournia   (1000)       87 2018-10-12 12:01:33.000000 hazm-0.7.0/hazm.egg-info/requires.txt
--rwxr-xr-x   0 nournia   (1000) nournia   (1000)      919 2018-10-12 12:01:07.000000 hazm-0.7.0/setup.py
--rw-r--r--   0 nournia   (1000) nournia   (1000)       38 2018-10-12 12:01:33.000000 hazm-0.7.0/setup.cfg
+-rw-r--r--   0        0        0     1083 2023-05-20 15:46:10.182773 hazm-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4452 2023-05-20 15:46:10.182773 hazm-0.9.0/README.md
+-rw-r--r--   0        0        0     2480 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/__init__.py
+-rwxr-xr-x   0        0        0    11943 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/chunker.py
+-rw-r--r--   0        0        0      586 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/__init__.py
+-rw-r--r--   0        0        0     4470 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/bijankhan_reader.py
+-rw-r--r--   0        0        0    16979 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/dadegan_reader.py
+-rw-r--r--   0        0        0     6360 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/degarbayan_reader.py
+-rw-r--r--   0        0        0     6136 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/hamshahri_reader.py
+-rw-r--r--   0        0        0     1858 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/mirastext_reader.py
+-rw-r--r--   0        0        0     1267 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/persian_plain_text_reader.py
+-rw-r--r--   0        0        0     3332 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/persica_reader.py
+-rw-r--r--   0        0        0    11630 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/peykare_reader.py
+-rw-r--r--   0        0        0     4392 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/quran_reader.py
+-rw-r--r--   0        0        0     4731 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/sentipers_reader.py
+-rw-r--r--   0        0        0     4609 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/tnews_reader.py
+-rw-r--r--   0        0        0    14539 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/treebank_reader.py
+-rw-r--r--   0        0        0     2733 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/verbvalency_reader.py
+-rw-r--r--   0        0        0    64232 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/wiki_extractor.py
+-rw-r--r--   0        0        0     3481 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/corpus_readers/wikipedia_reader.py
+-rw-r--r--   0        0        0      656 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/iverbs.dat
+-rw-r--r--   0        0        0     5172 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/iwords.dat
+-rw-r--r--   0        0        0     3664 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/stopwords.dat
+-rw-r--r--   0        0        0     8328 2023-05-20 15:46:10.250774 hazm-0.9.0/hazm/data/verbs.dat
+-rw-r--r--   0        0        0  1335405 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/data/words.dat
+-rw-r--r--   0        0        0     8559 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/dependency_parser.py
+-rw-r--r--   0        0        0    15568 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/embedding.py
+-rw-r--r--   0        0        0    36078 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/informal_normalizer.py
+-rw-r--r--   0        0        0   107981 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/lemmatizer.py
+-rw-r--r--   0        0        0    24507 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/normalizer.py
+-rw-r--r--   0        0        0    10011 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/pos_tagger.py
+-rw-r--r--   0        0        0     1348 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/sentence_tokenizer.py
+-rw-r--r--   0        0        0    17158 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/sequence_tagger.py
+-rw-r--r--   0        0        0     2495 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/stemmer.py
+-rw-r--r--   0        0        0     2593 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/token_splitter.py
+-rw-r--r--   0        0        0     3027 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/utils.py
+-rw-r--r--   0        0        0    13819 2023-05-20 15:46:10.258774 hazm-0.9.0/hazm/word_tokenizer.py
+-rw-r--r--   0        0        0     4160 2023-05-20 15:46:10.258774 hazm-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 hazm-0.9.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hazm-0.7.0/hazm/WikiExtractor.py` & `hazm-0.9.0/hazm/corpus_readers/wiki_extractor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,232 +1,631 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # =============================================================================
-#  Version: 2.75 (March 4, 2017)
-#  Author: Giuseppe Attardi (attardi@di.unipi.it), University of Pisa
-#
-#  Contributors:
-#   Antonio Fuschetto (fuschett@aol.com)
-#   Leonardo Souza (lsouza@amtera.com.br)
-#   Juan Manuel Caicedo (juan@cavorite.com)
-#   Humberto Pereira (begini@gmail.com)
-#   Siegfried-A. Gevatter (siegfried@gevatter.com)
-#   Pedro Assis (pedroh2306@gmail.com)
-#   Wim Muskee (wimmuskee@gmail.com)
-#   Radics Geza (radicsge@gmail.com)
-#   orangain (orangain@gmail.com)
-#   Seth Cleveland (scleveland@turnitin.com)
-#   Bren Barn
-#
-# =============================================================================
-#  Copyright (c) 2011-2017. Giuseppe Attardi (attardi@di.unipi.it).
+#  Copyright (c) 2020. Giuseppe Attardi (attardi@di.unipi.it).
 # =============================================================================
 #  This file is part of Tanl.
 #
 #  Tanl is free software; you can redistribute it and/or modify it
-#  under the terms of the GNU General Public License, version 3,
+#  under the terms of the GNU Affero General Public License, version 3,
 #  as published by the Free Software Foundation.
 #
 #  Tanl is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License at <http://www.gnu.org/licenses/> for more details.
+#  GNU Affero General Public License for more details.
 #
+#  You should have received a copy of the GNU Affero General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # =============================================================================
 
-"""Wikipedia Extractor:
-Extracts and cleans text from a Wikipedia database dump and stores output in a
-number of files of similar size in a given directory.
-Each file will contain several documents in the format:
-
-    <doc id="" revid="" url="" title="">
-        ...
-        </doc>
-
-If the program is invoked with the --json flag, then each file will
-contain several documents formatted as json ojects, one per line, with
-the following structure
-
-    {"id": "", "revid": "", "url":"", "title": "", "text": "..."}
-
-Template expansion requires preprocesssng first the whole dump and
-collecting template definitions.
-
-"""
-
-from __future__ import unicode_literals, division
-
-import sys
-import argparse
-import bz2
-import codecs
-import cgi
-import fileinput
+import re
+import html
+import json
+from itertools import zip_longest
+from urllib.parse import quote as urlencode
+from html.entities import name2codepoint
 import logging
-import os.path
-import re  # TODO use regex when it will be standard
 import time
-import json
-from io import StringIO
-from multiprocessing import Queue, Process, Value, cpu_count
-from timeit import default_timer
-
-
-PY2 = sys.version_info[0] == 2
-# Python 2.7 compatibiity
-if PY2:
-    from urllib import quote
-    from htmlentitydefs import name2codepoint
-    from itertools import izip as zip, izip_longest as zip_longest
-    range = xrange  # Use Python 3 equivalent
-    chr = unichr    # Use Python 3 equivalent
-    text_type = unicode
-
-    class SimpleNamespace(object):
-        def __init__ (self, **kwargs):
-            self.__dict__.update(kwargs)
-        def __repr__ (self):
-            keys = sorted(self.__dict__)
-            items = ("{}={!r}".format(k, self.__dict__[k]) for k in keys)
-            return "{}({})".format(type(self).__name__, ", ".join(items))
-        def __eq__ (self, other):
-            return self.__dict__ == other.__dict__
-else:
-    from urllib.parse import quote
-    from html.entities import name2codepoint
-    from itertools import zip_longest
-    from types import SimpleNamespace
-    text_type = str
 
+# ----------------------------------------------------------------------
 
-# ===========================================================================
-
-# Program version
-version = '2.75'
+# match tail after wikilink
+tailRE = re.compile('\w+')
+syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
 
 ## PARAMS ####################################################################
 
-options = SimpleNamespace(
+##
+# Defined in <siteinfo>
+# We include as default Template, when loading external template file.
+knownNamespaces = set(['Template'])
 
-    ##
-    # Defined in <siteinfo>
-    # We include as default Template, when loading external template file.
-    knownNamespaces = {'Template': 10},
+##
+# Drop these elements from article text
+#
+discardElements = [
+    'gallery', 'timeline', 'noinclude', 'pre',
+    'table', 'tr', 'td', 'th', 'caption', 'div',
+    'form', 'input', 'select', 'option', 'textarea',
+    'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
+    'ref', 'references', 'img', 'imagemap', 'source', 'small'
+]
 
-    ##
-    # The namespace used for template definitions
-    # It is the name associated with namespace key=10 in the siteinfo header.
-    templateNamespace = '',
-    templatePrefix = '',
+##
+# Recognize only these namespaces
+# w: Internal links to the Wikipedia
+# wiktionary: Wiki dictionary
+# wikt: shortcut for Wiktionary
+#
+acceptedNamespaces = ['w', 'wiktionary', 'wikt']
 
-    ##
-    # The namespace used for module definitions
-    # It is the name associated with namespace key=828 in the siteinfo header.
-    moduleNamespace = '',
 
-    ##
-    # Recognize only these namespaces in links
-    # w: Internal links to the Wikipedia
-    # wiktionary: Wiki dictionary
-    # wikt: shortcut for Wiktionary
-    #
-    acceptedNamespaces = ['w', 'wiktionary', 'wikt'],
+def get_url(urlbase, uid):
+    return "%s?curid=%s" % (urlbase, uid)
 
-    # This is obtained from <siteinfo>
-    urlbase = '',
 
-    ##
-    # Filter disambiguation pages
-    filter_disambig_pages = False,
+# ======================================================================
 
-    ##
-    # Drop tables from the article
-    keep_tables = False,
 
-    ##
-    # Whether to preserve links in output
-    keepLinks = False,
+def clean(extractor, text, expand_templates=False, html_safe=True):
+    """
+    Transforms wiki markup. If the command line flag --escapedoc is set then the text is also escaped
+    @see https://www.mediawiki.org/wiki/Help:Formatting
+    :param extractor: the Extractor t use.
+    :param text: the text to clean.
+    :param expand_templates: whether to perform template expansion.
+    :param html_safe: whether to convert reserved HTML characters to entities.
+    @return: the cleaned text.
+    """
 
-    ##
-    # Whether to preserve section titles
-    keepSections = True,
+    if expand_templates:
+        # expand templates
+        # See: http://www.mediawiki.org/wiki/Help:Templates
+        text = extractor.expandTemplates(text)
+    else:
+        # Drop transclusions (template, parser functions)
+        text = dropNested(text, r'{{', r'}}')
 
-    ##
-    # Whether to preserve lists
-    keepLists = False,
+    # Drop tables
+    text = dropNested(text, r'{\|', r'\|}')
 
-    ##
-    # Whether to output HTML instead of text
-    toHTML = False,
+    # replace external links
+    text = replaceExternalLinks(text)
 
-    ##
-    # Whether to write json instead of the xml-like default output format
-    write_json = False,
+    # replace internal links
+    text = replaceInternalLinks(text)
 
-    ##
-    # Whether to expand templates
-    expand_templates = True,
+    # drop MagicWords behavioral switches
+    text = magicWordsRE.sub('', text)
 
-    ##
-    ## Whether to escape doc content
-    escape_doc = False,
+    # ############### Process HTML ###############
 
-    ##
-    # Print the wikipedia article revision
-    print_revision = False,
+    # turn into HTML, except for the content of <syntaxhighlight>
+    res = ''
+    cur = 0
+    for m in syntaxhighlight.finditer(text):
+        end = m.end()
+        res += unescape(text[cur:m.start()]) + m.group(1)
+        cur = end
+    text = res + unescape(text[cur:])
 
-    ##
-    # Minimum expanded text length required to print document
-    min_text_length = 0,
+    # Handle bold/italic/quote
+    if extractor.HtmlFormatting:
+        text = bold_italic.sub(r'<b>\1</b>', text)
+        text = bold.sub(r'<b>\1</b>', text)
+        text = italic.sub(r'<i>\1</i>', text)
+    else:
+        text = bold_italic.sub(r'\1', text)
+        text = bold.sub(r'\1', text)
+        text = italic_quote.sub(r'"\1"', text)
+        text = italic.sub(r'"\1"', text)
+        text = quote_quote.sub(r'"\1"', text)
+    # residuals of unbalanced quotes
+    text = text.replace("'''", '').replace("''", '"')
+
+    # Collect spans
+
+    spans = []
+    # Drop HTML comments
+    for m in comment.finditer(text):
+        spans.append((m.start(), m.end()))
+
+    # Drop self-closing tags
+    for pattern in selfClosing_tag_patterns:
+        for m in pattern.finditer(text):
+            spans.append((m.start(), m.end()))
 
-    # Shared objects holding templates, redirects and cache
-    templates = {},
-    redirects = {},
-    # cache of parser templates
-    # FIXME: sharing this with a Manager slows down.
-    templateCache = {},
-
-    # Elements to ignore/discard
-
-    ignored_tag_patterns = [],
-
-    discardElements = [
-        'gallery', 'timeline', 'noinclude', 'pre',
-        'table', 'tr', 'td', 'th', 'caption', 'div',
-        'form', 'input', 'select', 'option', 'textarea',
-        'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
-        'ref', 'references', 'img', 'imagemap', 'source', 'small',
-        'sub', 'sup', 'indicator'
-    ],
-)
+    # Drop ignored tags
+    for left, right in ignored_tag_patterns:
+        for m in left.finditer(text):
+            spans.append((m.start(), m.end()))
+        for m in right.finditer(text):
+            spans.append((m.start(), m.end()))
 
-##
-# Keys for Template and Module namespaces
-templateKeys = set(['10', '828'])
+    # Bulk remove all spans
+    text = dropSpans(spans, text)
 
-##
-# Regex for identifying disambig pages
-filter_disambig_page_pattern = re.compile("{{disambig(uation)?(\|[^}]*)?}}")
+    # Drop discarded elements
+    for tag in discardElements:
+        text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
+
+    if not extractor.HtmlFormatting:
+        # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
+        text = unescape(text)
+
+    # Expand placeholders
+    for pattern, placeholder in placeholder_tag_patterns:
+        index = 1
+        for match in pattern.finditer(text):
+            text = text.replace(match.group(), '%s_%d' % (placeholder, index))
+            index += 1
+
+    text = text.replace('<<', u'«').replace('>>', u'»')
+
+    #############################################
+
+    # Cleanup text
+    text = text.replace('\t', ' ')
+    text = spaces.sub(' ', text)
+    text = dots.sub('...', text)
+    text = re.sub(u' (,:\.\)\]»)', r'\1', text)
+    text = re.sub(u'(\[\(«) ', r'\1', text)
+    text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
+    text = text.replace(',,', ',').replace(',.', '.')
+    if html_safe:
+        text = html.escape(text, quote=False)
+    return text
+
+
+# skip level 1, it is page name level
+section = re.compile(r'(==+)\s*(.*?)\s*\1')
+
+listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
+listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
+listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
+            ':': '<dd>%s</dd>'}
+
+
+def compact(text, mark_headers=False):
+    """Deal with headers, lists, empty sections, residuals of tables.
+    :param text: convert to HTML
+    """
+
+    page = []  # list of paragraph
+    headers = {}  # Headers for unfilled sections
+    emptySection = False  # empty sections are discarded
+    listLevel = ''  # nesting of lists
+
+    for line in text.split('\n'):
+
+        if not line:
+            if len(listLevel):    # implies Extractor.HtmlFormatting
+                for c in reversed(listLevel):
+                    page.append(listClose[c])
+                    listLevel = ''
+            continue
+
+        # Handle section titles
+        m = section.match(line)
+        if m:
+            title = m.group(2)
+            lev = len(m.group(1))
+            if Extractor.HtmlFormatting:
+                page.append("<h%d>%s</h%d>" % (lev, title, lev))
+            if title and title[-1] not in '!?':
+                title += '.'
+
+            if mark_headers:
+                title = "## " + title
+
+            headers[lev] = title
+            # drop previous headers
+            headers = { k:v for k,v in headers.items() if k <= lev }
+            emptySection = True
+            continue
+        # Handle page title
+        if line.startswith('++'):
+            title = line[2:-2]
+            if title:
+                if title[-1] not in '!?':
+                    title += '.'
+                page.append(title)
+        # handle indents
+        elif line[0] == ':':
+            page.append(line.lstrip(':'))
+        # handle lists
+        # @see https://www.mediawiki.org/wiki/Help:Formatting
+        elif line[0] in '*#;':
+            if Extractor.HtmlFormatting:
+                # close extra levels
+                l = 0
+                for c in listLevel:
+                    if l < len(line) and c != line[l]:
+                        for extra in reversed(listLevel[l:]):
+                            page.append(listClose[extra])
+                        listLevel = listLevel[:l]
+                        break
+                    l += 1
+                if l < len(line) and line[l] in '*#;:':
+                    # add new level (only one, no jumps)
+                    # FIXME: handle jumping levels
+                    type = line[l]
+                    page.append(listOpen[type])
+                    listLevel += type
+                    line = line[l+1:].strip()
+                else:
+                    # continue on same level
+                    type = line[l-1]
+                    line = line[l:].strip()
+                page.append(listItem[type] % line)
+            else:
+                continue
+        elif len(listLevel):    # implies Extractor.HtmlFormatting
+            for c in reversed(listLevel):
+                page.append(listClose[c])
+            listLevel = []
+
+        # Drop residuals of lists
+        elif line[0] in '{|' or line[-1] == '}':
+            continue
+        # Drop irrelevant lines
+        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
+            continue
+        elif len(headers):
+            if Extractor.keepSections:
+                items = sorted(headers.items())
+                for (i, v) in items:
+                    page.append(v)
+            headers.clear()
+            page.append(line)  # first line
+            emptySection = False
+        elif not emptySection:
+            page.append(line)
+            # dangerous
+            # # Drop preformatted
+            # elif line[0] == ' ':
+            #     continue
+
+    return page
+
+
+# ----------------------------------------------------------------------
+
+def dropNested(text, openDelim, closeDelim):
+    """
+    A matching function for nested expressions, e.g. namespaces and tables.
+    """
+    openRE = re.compile(openDelim, re.IGNORECASE)
+    closeRE = re.compile(closeDelim, re.IGNORECASE)
+    # partition text in separate blocks { } { }
+    spans = []  # pairs (s, e) for each partition
+    nest = 0  # nesting level
+    start = openRE.search(text, 0)
+    if not start:
+        return text
+    end = closeRE.search(text, start.end())
+    next = start
+    while end:
+        next = openRE.search(text, next.end())
+        if not next:  # termination
+            while nest:  # close all pending
+                nest -= 1
+                end0 = closeRE.search(text, end.end())
+                if end0:
+                    end = end0
+                else:
+                    break
+            spans.append((start.start(), end.end()))
+            break
+        while end.end() < next.start():
+            # { } {
+            if nest:
+                nest -= 1
+                # try closing more
+                last = end.end()
+                end = closeRE.search(text, end.end())
+                if not end:  # unbalanced
+                    if spans:
+                        span = (spans[0][0], last)
+                    else:
+                        span = (start.start(), last)
+                    spans = [span]
+                    break
+            else:
+                spans.append((start.start(), end.end()))
+                # advance start, find next close
+                start = next
+                end = closeRE.search(text, next.end())
+                break  # { }
+        if next != start:
+            # { { }
+            nest += 1
+    # collect text outside partitions
+    return dropSpans(spans, text)
+
+
+def dropSpans(spans, text):
+    """
+    Drop from text the blocks identified in :param spans:, possibly nested.
+    """
+    spans.sort()
+    res = ''
+    offset = 0
+    for s, e in spans:
+        if offset <= s:  # handle nesting
+            if offset < s:
+                res += text[offset:s]
+            offset = e
+    res += text[offset:]
+    return res
+
+
+# ----------------------------------------------------------------------
+# External links
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
+
+wgUrlProtocols = [
+    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
+    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
+    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
+    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
+]
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
+
+# Constants needed for external link processing
+# Everything except bracket, space, or control characters
+# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
+# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
+EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
+ExtLinkBracketedRegex = re.compile(
+    '(?i)\[((' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
+    re.S | re.U)
+EXT_IMAGE_REGEX = re.compile(
+    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
+    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
+    re.X | re.S | re.U)
+
+
+def replaceExternalLinks(text):
+    s = ''
+    cur = 0
+    for m in ExtLinkBracketedRegex.finditer(text):
+        s += text[cur:m.start()]
+        cur = m.end()
+
+        url = m.group(1)
+        label = m.group(3)
+
+        # # The characters '<' and '>' (which were escaped by
+        # # removeHTMLtags()) should not be included in
+        # # URLs, per RFC 2396.
+        # m2 = re.search('&(lt|gt);', url)
+        # if m2:
+        #     link = url[m2.end():] + ' ' + link
+        #     url = url[0:m2.end()]
+
+        # If the link text is an image URL, replace it with an <img> tag
+        # This happened by accident in the original parser, but some people used it extensively
+        m = EXT_IMAGE_REGEX.match(label)
+        if m:
+            label = makeExternalImage(label)
+
+        # Use the encoded URL
+        # This means that users can paste URLs directly into the text
+        # Funny characters like ö aren't valid in URLs anyway
+        # This was changed in August 2004
+        s += makeExternalLink(url, label)  # + trail
+
+    return s + text[cur:]
+
+
+def makeExternalLink(url, anchor):
+    """Function applied to wikiLinks"""
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(url), anchor)
+    else:
+        return anchor
+
+
+def makeExternalImage(url, alt=''):
+    if Extractor.keepLinks:
+        return '<img src="%s" alt="%s">' % (url, alt)
+    else:
+        return alt
+
+
+# ----------------------------------------------------------------------
+# WikiLinks
+# See https://www.mediawiki.org/wiki/Help:Links#Internal_links
+
+# Can be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
+# Also: [[Help:IPA for Catalan|[andora]]]
+
+
+def replaceInternalLinks(text):
+    """
+    Replaces external links of the form:
+    [[title |...|label]]trail
+
+    with title concatenated with trail, when present, e.g. 's' for plural.
+    """
+    # call this after removal of external links, so we need not worry about
+    # triple closing ]]].
+    cur = 0
+    res = ''
+    for s, e in findBalanced(text, ['[['], [']]']):
+        m = tailRE.match(text, e)
+        if m:
+            trail = m.group(0)
+            end = m.end()
+        else:
+            trail = ''
+            end = e
+        inner = text[s + 2:e - 2]
+        # find first |
+        pipe = inner.find('|')
+        if pipe < 0:
+            title = inner
+            label = title
+        else:
+            title = inner[:pipe].rstrip()
+            # find last |
+            curp = pipe + 1
+            for s1, e1 in findBalanced(inner, ['[['], [']]']):
+                last = inner.rfind('|', curp, s1)
+                if last >= 0:
+                    pipe = last  # advance
+                curp = e1
+            label = inner[pipe + 1:].strip()
+        res += text[cur:s] + makeInternalLink(title, label) + trail
+        cur = end
+    return res + text[cur:]
+
+
+def makeInternalLink(title, label):
+    colon = title.find(':')
+    if colon > 0 and title[:colon] not in acceptedNamespaces:
+        return ''
+    if colon == 0:
+        # drop also :File:
+        colon2 = title.find(':', colon + 1)
+        if colon2 > 1 and title[colon + 1:colon2] not in acceptedNamespaces:
+            return ''
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(title), label)
+    else:
+        return label
 
-##
-# page filtering logic -- remove templates, undesired xml namespaces, and disambiguation pages
-def keepPage(ns, page):
-    if ns != '0':               # Aritcle
-        return False
-    # remove disambig pages if desired
-    if options.filter_disambig_pages:
-        for line in page:
-            if filter_disambig_page_pattern.match(line):
-                return False
-    return True
 
+# ----------------------------------------------------------------------
+# variables
 
-def get_url(uid):
-    return "%s?curid=%s" % (options.urlbase, uid)
+
+class MagicWords():
+
+    """
+    One copy in each Extractor.
+
+    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
+    """
+    names = [
+        '!',
+        'currentmonth',
+        'currentmonth1',
+        'currentmonthname',
+        'currentmonthnamegen',
+        'currentmonthabbrev',
+        'currentday',
+        'currentday2',
+        'currentdayname',
+        'currentyear',
+        'currenttime',
+        'currenthour',
+        'localmonth',
+        'localmonth1',
+        'localmonthname',
+        'localmonthnamegen',
+        'localmonthabbrev',
+        'localday',
+        'localday2',
+        'localdayname',
+        'localyear',
+        'localtime',
+        'localhour',
+        'numberofarticles',
+        'numberoffiles',
+        'numberofedits',
+        'articlepath',
+        'pageid',
+        'sitename',
+        'server',
+        'servername',
+        'scriptpath',
+        'stylepath',
+        'pagename',
+        'pagenamee',
+        'fullpagename',
+        'fullpagenamee',
+        'namespace',
+        'namespacee',
+        'namespacenumber',
+        'currentweek',
+        'currentdow',
+        'localweek',
+        'localdow',
+        'revisionid',
+        'revisionday',
+        'revisionday2',
+        'revisionmonth',
+        'revisionmonth1',
+        'revisionyear',
+        'revisiontimestamp',
+        'revisionuser',
+        'revisionsize',
+        'subpagename',
+        'subpagenamee',
+        'talkspace',
+        'talkspacee',
+        'subjectspace',
+        'subjectspacee',
+        'talkpagename',
+        'talkpagenamee',
+        'subjectpagename',
+        'subjectpagenamee',
+        'numberofusers',
+        'numberofactiveusers',
+        'numberofpages',
+        'currentversion',
+        'rootpagename',
+        'rootpagenamee',
+        'basepagename',
+        'basepagenamee',
+        'currenttimestamp',
+        'localtimestamp',
+        'directionmark',
+        'contentlanguage',
+        'numberofadmins',
+        'cascadingsources',
+    ]
+
+    def __init__(self):
+        self.values = {'!': '|'}
+
+    def __getitem__(self, name):
+        return self.values.get(name)
+
+    def __setitem__(self, name, value):
+        self.values[name] = value
+
+    switches = (
+        '__NOTOC__',
+        '__FORCETOC__',
+        '__TOC__',
+        '__TOC__',
+        '__NEWSECTIONLINK__',
+        '__NONEWSECTIONLINK__',
+        '__NOGALLERY__',
+        '__HIDDENCAT__',
+        '__NOCONTENTCONVERT__',
+        '__NOCC__',
+        '__NOTITLECONVERT__',
+        '__NOTC__',
+        '__START__',
+        '__END__',
+        '__INDEX__',
+        '__NOINDEX__',
+        '__STATICREDIRECT__',
+        '__DISAMBIG__'
+    )
+
+
+magicWordsRE = re.compile('|'.join(MagicWords.switches))
 
 
 # =========================================================================
 #
 # MediaWiki Markup Grammar
 # https://www.mediawiki.org/wiki/Preprocessor_ABNF
 
@@ -259,14 +658,23 @@
 #                   line-eating-comment / unclosed-comment / xmlish-element /
 #                   *wikitext-L3
 
 # ------------------------------------------------------------------------------
 
 selfClosingTags = ('br', 'hr', 'nobr', 'ref', 'references', 'nowiki')
 
+# These tags are dropped, keeping their content.
+# handle 'a' separately, depending on keepLinks
+ignoredTags = (
+    'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'div', 'em',
+    'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd', 'nowiki',
+    'p', 'plaintext', 's', 'span', 'strike', 'strong',
+    'sub', 'sup', 'tt', 'u', 'var'
+)
+
 placeholder_tags = {'math': 'formula', 'code': 'codice'}
 
 
 def normalizeTitle(title):
     """Normalize title"""
     # remove leading/trailing whitespace and underscores
     title = title.strip(' _')
@@ -279,15 +687,15 @@
         if m.group(2):
             optionalWhitespace = ' '
         else:
             optionalWhitespace = ''
         rest = m.group(3)
 
         ns = normalizeNamespace(prefix)
-        if ns in options.knownNamespaces:
+        if ns in knownNamespaces:
             # If the prefix designates a known namespace, then it might be
             # followed by optional whitespace that should be removed to get
             # the canonical page name
             # (e.g., "Category:  Births" should become "Category:Births").
             title = ns + ":" + ucfirst(rest)
         else:
             # No namespace, just capitalize first letter.
@@ -329,34 +737,42 @@
     return re.sub("&#?(\w+);", fixup, text)
 
 
 # Match HTML comments
 # The buggy template {{Template:T}} has a comment terminating with just "->"
 comment = re.compile(r'<!--.*?-->', re.DOTALL)
 
-
-# Match <nowiki>...</nowiki>
-nowiki = re.compile(r'<nowiki>.*?</nowiki>')
+# Match ignored tags
+ignored_tag_patterns = []
 
 
 def ignoreTag(tag):
     left = re.compile(r'<%s\b.*?>' % tag, re.IGNORECASE | re.DOTALL)  # both <ref> and <reference>
     right = re.compile(r'</\s*%s>' % tag, re.IGNORECASE)
-    options.ignored_tag_patterns.append((left, right))
+    ignored_tag_patterns.append((left, right))
+
+
+def resetIgnoredTags():
+    global ignored_tag_patterns
+    ignored_tag_patterns = []
+
+
+for tag in ignoredTags:
+    ignoreTag(tag)
 
 # Match selfClosing HTML tags
 selfClosing_tag_patterns = [
     re.compile(r'<\s*%s\b[^>]*/\s*>' % tag, re.DOTALL | re.IGNORECASE) for tag in selfClosingTags
-    ]
+]
 
 # Match HTML placeholder tags
 placeholder_tag_patterns = [
     (re.compile(r'<\s*%s(\s*| [^>]+?)>.*?<\s*/\s*%s\s*>' % (tag, tag), re.DOTALL | re.IGNORECASE),
      repl) for tag, repl in placeholder_tags.items()
-    ]
+]
 
 # Match preformatted lines
 preformatted = re.compile(r'^ .*?$')
 
 # Match external links (space separates second optional parameter)
 externalLink = re.compile(r'\[\w+[^ ]*? (.*?)]')
 externalLinkNoAnchor = re.compile(r'\[\w+[&\]]*\]')
@@ -370,40 +786,37 @@
 
 # Matches space
 spaces = re.compile(r' {2,}')
 
 # Matches dots
 dots = re.compile(r'\.{4,}')
 
-
 # ======================================================================
 
-
 class Template(list):
     """
     A Template is a list of TemplateText or TemplateArgs
     """
 
     @classmethod
     def parse(cls, body):
         tpl = Template()
         # we must handle nesting, s.a.
         # {{{1|{{PAGENAME}}}
         # {{{italics|{{{italic|}}}
         # {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|
         #
         start = 0
-        for s, e in findMatchingBraces(body, 3):
+        for s,e in findMatchingBraces(body, 3):
             tpl.append(TemplateText(body[start:s]))
-            tpl.append(TemplateArg(body[s + 3:e - 3]))
+            tpl.append(TemplateArg(body[s+3:e-3]))
             start = e
-        tpl.append(TemplateText(body[start:]))  # leftover
+        tpl.append(TemplateText(body[start:])) # leftover
         return tpl
 
-
     def subst(self, params, extractor, depth=0):
         # We perform parameter substitutions recursively.
         # We also limit the maximum number of iterations to avoid too long or
         # even endless loops (in case of malformed input).
 
         # :see: http://meta.wikimedia.org/wiki/Help:Expansion#Distinction_between_variables.2C_parser_functions.2C_and_templates
         #
@@ -411,51 +824,49 @@
         # Therefore a parameter name in a template can depend on the value of
         # another parameter of the same template, regardless of the order in
         # which they are specified in the template call, for example, using
         # Template:ppp containing "{{{{{{p}}}}}}", {{ppp|p=q|q=r}} and even
         # {{ppp|q=r|p=q}} gives r, but using Template:tvvv containing
         # "{{{{{{{{{p}}}}}}}}}", {{tvvv|p=q|q=r|r=s}} gives s.
 
-        # logging.debug('&*ssubst tpl %d %s', extractor.frame.length, '', depth, self)
+        logging.debug('subst tpl (%d, %d) %s', len(extractor.frame), depth, self)
 
         if depth > extractor.maxParameterRecursionLevels:
             extractor.recursion_exceeded_3_errs += 1
             return ''
 
         return ''.join([tpl.subst(params, extractor, depth) for tpl in self])
 
     def __str__(self):
-        return ''.join([text_type(x) for x in self])
+        return ''.join([str(x) for x in self])
 
 
-class TemplateText(text_type):
+class TemplateText(str):
     """Fixed text of template"""
 
-
     def subst(self, params, extractor, depth):
         return self
 
 
-class TemplateArg(object):
+class TemplateArg():
     """
     parameter to a template.
     Has a name and a default value, both of which are Templates.
     """
-
     def __init__(self, parameter):
         """
         :param parameter: the parts of a tplarg.
         """
         # the parameter name itself might contain templates, e.g.:
         #   appointe{{#if:{{{appointer14|}}}|r|d}}14|
         #   4|{{{{{subst|}}}CURRENTYEAR}}
 
         # any parts in a tplarg after the first (the parameter default) are
         # ignored, and an equals sign in the first part is treated as plain text.
-        # logging.debug('TemplateArg %s', parameter)
+        #logging.debug('TemplateArg %s', parameter)
 
         parts = splitParts(parameter)
         self.name = Template.parse(parts[0])
         if len(parts) > 1:
             # This parameter has a default value
             self.default = Template.parse(parts[1])
         else:
@@ -463,352 +874,149 @@
 
     def __str__(self):
         if self.default:
             return '{{{%s|%s}}}' % (self.name, self.default)
         else:
             return '{{{%s}}}' % self.name
 
-
     def subst(self, params, extractor, depth):
         """
         Substitute value for this argument from dict :param params:
         Use :param extractor: to evaluate expressions for name and default.
         Limit substitution to the maximun :param depth:.
         """
         # the parameter name itself might contain templates, e.g.:
         # appointe{{#if:{{{appointer14|}}}|r|d}}14|
-        paramName = self.name.subst(params, extractor, depth + 1)
-        paramName = extractor.transform(paramName)
+        paramName = self.name.subst(params, extractor, depth+1)
+        paramName = extractor.expandTemplates(paramName)
         res = ''
         if paramName in params:
             res = params[paramName]  # use parameter value specified in template invocation
-        elif self.default:  # use the default value
-            defaultValue = self.default.subst(params, extractor, depth + 1)
-            res = extractor.transform(defaultValue)
-        # logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
+        elif self.default:            # use the default value
+            defaultValue = self.default.subst(params, extractor, depth+1)
+            res =  extractor.expandTemplates(defaultValue)
+        #logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
         return res
 
 
-class Frame(object):
-
-    def __init__(self, title='', args=[], prev=None):
-        self.title = title
-        self.args = args
-        self.prev = prev
-        self.depth = prev.depth + 1 if prev else 0
-
+# ======================================================================
 
-    def push(self, title, args):
-        return Frame(title, args, self)
+substWords = 'subst:|safesubst:'
 
 
-    def pop(self):
-        return self.prev
+class Extractor():
+    """
+    An extraction task on a article.
+    """
+    ##
+    # Whether to preserve links in output
+    keepLinks = False
 
+    ##
+    # Whether to preserve section titles
+    keepSections = True
 
-    def __str__(self):
-        res = ''
-        prev = self.prev
-        while prev:
-            if res: res += ', '
-            res += '(%s, %s)' % (prev.title, prev.args)
-            prev = prev.prev
-        return '<Frame [' + res + ']>'
+    ##
+    # Whether to output text with HTML formatting elements in <doc> files.
+    HtmlFormatting = False
 
-# ======================================================================
+    ##
+    # Whether to produce json instead of the default <doc> output format.
+    toJson = False
 
-substWords = 'subst:|safesubst:'
+    ##
+    # Obtained from TemplateNamespace
+    templatePrefix = ''
 
-class Extractor(object):
-    """
-    An extraction task on a article.
-    """
-    def __init__(self, id, revid, title, lines):
+    def __init__(self, id, revid, urlbase, title, page):
         """
-        :param id: id of page.
-        :param title: tutle of page.
-        :param lines: a list of lines.
+        :param page: a list of lines.
         """
         self.id = id
         self.revid = revid
+        self.url = get_url(urlbase, id)
         self.title = title
-        self.text = ''.join(lines)
+        self.page = page
         self.magicWords = MagicWords()
-        self.frame = Frame()
-        self.recursion_exceeded_1_errs = 0  # template recursion within expand()
+        self.frame = []
+        self.recursion_exceeded_1_errs = 0  # template recursion within expandTemplates()
         self.recursion_exceeded_2_errs = 0  # template recursion within expandTemplate()
         self.recursion_exceeded_3_errs = 0  # parameter recursion
         self.template_title_errs = 0
 
-    def write_output(self, out, text):
+    def clean_text(self, text, mark_headers=False, expand_templates=True,
+                   html_safe=True):
+        """
+        :param mark_headers: True to distinguish headers from paragraphs
+          e.g. "## Section 1"
         """
-        :param out: a memory file
-        :param text: the text of the page
+        self.magicWords['namespace'] = self.title[:max(0, self.title.find(":"))]
+        #self.magicWords['namespacenumber'] = '0' # for article,
+        self.magicWords['pagename'] = self.title
+        self.magicWords['fullpagename'] = self.title
+        self.magicWords['currentyear'] = time.strftime('%Y')
+        self.magicWords['currentmonth'] = time.strftime('%m')
+        self.magicWords['currentday'] = time.strftime('%d')
+        self.magicWords['currenthour'] = time.strftime('%H')
+        self.magicWords['currenttime'] = time.strftime('%H:%M:%S')
+
+        text = clean(self, text, expand_templates=expand_templates,
+                     html_safe=html_safe)
+
+        text = compact(text, mark_headers=mark_headers)
+        return text
+
+    def extract(self, out, html_safe=True):
         """
-        url = get_url(self.id)
-        if options.write_json:
+        :param out: a memory file.
+        :param html_safe: whether to escape HTML entities.
+        """
+        logging.debug("%s\t%s", self.id, self.title)
+        text = ''.join(self.page)
+        text = self.clean_text(text, html_safe=html_safe)
+
+        if self.to_json:
             json_data = {
-                'id': self.id,
-                'url': url,
+		'id': self.id,
+                'revid': self.revid,
+                'url': self.url,
                 'title': self.title,
                 'text': "\n".join(text)
             }
-            if options.print_revision:
-                json_data['revid'] = self.revid
-            # We don't use json.dump(data, out) because we want to be
-            # able to encode the string if the output is sys.stdout
-            out_str = json.dumps(json_data, ensure_ascii=False)
-            if out == sys.stdout:   # option -a or -o -
-                out_str = out_str.encode('utf-8')
+            out_str = json.dumps(json_data)
             out.write(out_str)
             out.write('\n')
         else:
-            if options.print_revision:
-                header = '<doc id="%s" revid="%s" url="%s" title="%s">\n' % (self.id, self.revid, url, self.title)
-            else:
-                header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, url, self.title)
+            header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, self.url, self.title)
+            # Separate header from text with a newline.
+            header += self.title + '\n\n'
             footer = "\n</doc>\n"
-            if out == sys.stdout:   # option -a or -o -
-                header = header.encode('utf-8')
             out.write(header)
-            for line in text:
-                if out == sys.stdout:   # option -a or -o -
-                    line = line.encode('utf-8')
-                out.write(line)
-                out.write('\n')
+            out.write('\n'.join(text))
+            out.write('\n')
             out.write(footer)
 
-    def extract(self, out):
-        """
-        :param out: a memory file.
-        """
-        # logging.info('%s\t%s', self.id, self.title)
-
-        # Separate header from text with a newline.
-        if options.toHTML:
-            title_str = '<h1>' + self.title + '</h1>'
-        else:
-            title_str = self.title + '\n'
-        # https://www.mediawiki.org/wiki/Help:Magic_words
-        colon = self.title.find(':')
-        if colon != -1:
-            ns = self.title[:colon]
-            pagename = self.title[colon+1:]
-        else:
-            ns = '' # Main
-            pagename = self.title
-        self.magicWords['NAMESPACE'] = ns
-        self.magicWords['NAMESPACENUMBER'] = options.knownNamespaces.get(ns, '0')
-        self.magicWords['PAGENAME'] = pagename
-        self.magicWords['FULLPAGENAME'] = self.title
-        slash = pagename.rfind('/')
-        if slash != -1:
-            self.magicWords['BASEPAGENAME'] = pagename[:slash]
-            self.magicWords['SUBPAGENAME'] = pagename[slash+1:]
-        else:
-            self.magicWords['BASEPAGENAME'] = pagename
-            self.magicWords['SUBPAGENAME'] = ''
-        slash = pagename.find('/')
-        if slash != -1:
-            self.magicWords['ROOTPAGENAME'] = pagename[:slash]
-        else:
-            self.magicWords['ROOTPAGENAME'] = pagename
-        self.magicWords['CURRENTYEAR'] = time.strftime('%Y')
-        self.magicWords['CURRENTMONTH'] = time.strftime('%m')
-        self.magicWords['CURRENTDAY'] = time.strftime('%d')
-        self.magicWords['CURRENTHOUR'] = time.strftime('%H')
-        self.magicWords['CURRENTTIME'] = time.strftime('%H:%M:%S')
-        text = self.text
-        self.text = ''          # save memory
-        #
-        # @see https://doc.wikimedia.org/mediawiki-core/master/php/classParser.html
-        # This does the equivalent of internalParse():
-        #
-        # $dom = $this->preprocessToDom( $text, $flag );
-        # $text = $frame->expand( $dom );
-        #
-        text = self.transform(text)
-        text = self.wiki2text(text)
-        text = compact(self.clean(text))
-        text = [title_str] + text
-
-        if sum(len(line) for line in text) < options.min_text_length:
-            return
-
-        self.write_output(out, text)
-
         errs = (self.template_title_errs,
                 self.recursion_exceeded_1_errs,
                 self.recursion_exceeded_2_errs,
                 self.recursion_exceeded_3_errs)
         if any(errs):
             logging.warn("Template errors in article '%s' (%s): title(%d) recursion(%d, %d, %d)",
                          self.title, self.id, *errs)
 
-
-    def transform(self, wikitext):
-        """
-        Transforms wiki markup.
-        @see https://www.mediawiki.org/wiki/Help:Formatting
-        """
-        # look for matching <nowiki>...</nowiki>
-        res = ''
-        cur = 0
-        for m in nowiki.finditer(wikitext, cur):
-            res += self.transform1(wikitext[cur:m.start()]) + wikitext[m.start():m.end()]
-            cur = m.end()
-        # leftover
-        res += self.transform1(wikitext[cur:])
-        return res
-
-
-    def transform1(self, text):
-        """Transform text not containing <nowiki>"""
-        if options.expand_templates:
-            # expand templates
-            # See: http://www.mediawiki.org/wiki/Help:Templates
-            return self.expand(text)
-        else:
-            # Drop transclusions (template, parser functions)
-            return dropNested(text, r'{{', r'}}')
-
-
-    def wiki2text(self, text):
-        #
-        # final part of internalParse().)
-        #
-        # $text = $this->doTableStuff( $text );
-        # $text = preg_replace( '/(^|\n)-----*/', '\\1<hr />', $text );
-        # $text = $this->doDoubleUnderscore( $text );
-        # $text = $this->doHeadings( $text );
-        # $text = $this->replaceInternalLinks( $text );
-        # $text = $this->doAllQuotes( $text );
-        # $text = $this->replaceExternalLinks( $text );
-        # $text = str_replace( self::MARKER_PREFIX . 'NOPARSE', '', $text );
-        # $text = $this->doMagicLinks( $text );
-        # $text = $this->formatHeadings( $text, $origText, $isMain );
-
-        # Drop tables
-        # first drop residual templates, or else empty parameter |} might look like end of table.
-        if not options.keep_tables:
-            text = dropNested(text, r'{{', r'}}')
-            text = dropNested(text, r'{\|', r'\|}')
-
-        # Handle bold/italic/quote
-        if options.toHTML:
-            text = bold_italic.sub(r'<b>\1</b>', text)
-            text = bold.sub(r'<b>\1</b>', text)
-            text = italic.sub(r'<i>\1</i>', text)
-        else:
-            text = bold_italic.sub(r'\1', text)
-            text = bold.sub(r'\1', text)
-            text = italic_quote.sub(r'"\1"', text)
-            text = italic.sub(r'"\1"', text)
-            text = quote_quote.sub(r'"\1"', text)
-        # residuals of unbalanced quotes
-        text = text.replace("'''", '').replace("''", '"')
-
-        # replace internal links
-        text = replaceInternalLinks(text)
-
-        # replace external links
-        text = replaceExternalLinks(text)
-
-        # drop MagicWords behavioral switches
-        text = magicWordsRE.sub('', text)
-
-        # ############### Process HTML ###############
-
-        # turn into HTML, except for the content of <syntaxhighlight>
-        res = ''
-        cur = 0
-        for m in syntaxhighlight.finditer(text):
-            res += unescape(text[cur:m.start()]) + m.group(1)
-            cur = m.end()
-        text = res + unescape(text[cur:])
-        return text
-
-
-    def clean(self, text):
-        """
-        Removes irrelevant parts from :param: text.
-        """
-
-        # Collect spans
-        spans = []
-        # Drop HTML comments
-        for m in comment.finditer(text):
-            spans.append((m.start(), m.end()))
-
-        # Drop self-closing tags
-        for pattern in selfClosing_tag_patterns:
-            for m in pattern.finditer(text):
-                spans.append((m.start(), m.end()))
-
-        # Drop ignored tags
-        for left, right in options.ignored_tag_patterns:
-            for m in left.finditer(text):
-                spans.append((m.start(), m.end()))
-            for m in right.finditer(text):
-                spans.append((m.start(), m.end()))
-
-        # Bulk remove all spans
-        text = dropSpans(spans, text)
-
-        # Drop discarded elements
-        for tag in options.discardElements:
-            text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
-
-        if not options.toHTML:
-            # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
-            text = unescape(text)
-
-        # Expand placeholders
-        for pattern, placeholder in placeholder_tag_patterns:
-            index = 1
-            for match in pattern.finditer(text):
-                text = text.replace(match.group(), '%s_%d' % (placeholder, index))
-                index += 1
-
-        text = text.replace('<<', '«').replace('>>', '»')
-
-        #############################################
-
-        # Cleanup text
-        text = text.replace('\t', ' ')
-        text = spaces.sub(' ', text)
-        text = dots.sub('...', text)
-        text = re.sub(' (,:\.\)\]»)', r'\1', text)
-        text = re.sub('(\[\(«) ', r'\1', text)
-        text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
-        text = text.replace(',,', ',').replace(',.', '.')
-        if options.keep_tables:
-            # the following regular expressions are used to remove the wikiml chartacters around table strucutures
-            # yet keep the content. The order here is imporant so we remove certain markup like {| and then
-            # then the future html attributes such as 'style'. Finally we drop the remaining '|-' that delimits cells.
-            text = re.sub(r'!(?:\s)?style=\"[a-z]+:(?:\d+)%;\"', r'', text)
-            text = re.sub(r'!(?:\s)?style="[a-z]+:(?:\d+)%;[a-z]+:(?:#)?(?:[0-9a-z]+)?"', r'', text)
-            text = text.replace('|-', '')
-            text = text.replace('|', '')
-        if options.toHTML:
-            text = cgi.escape(text)
-        return text
-
-
     # ----------------------------------------------------------------------
     # Expand templates
 
     maxTemplateRecursionLevels = 30
-    maxParameterRecursionLevels = 10
+    maxParameterRecursionLevels = 16
 
     # check for template beginning
     reOpen = re.compile('(?<!{){{(?!{)', re.DOTALL)
 
-
-    def expand(self, wikitext):
+    def expandTemplates(self, wikitext):
         """
         :param wikitext: the text to be expanded.
 
         Templates are frequently nested. Occasionally, parsing mistakes may
         cause template insertion to enter an infinite loop, for instance when
         trying to instantiate Template:Country
 
@@ -821,44 +1029,42 @@
         more than once, with different parameters in different parts of the
         article.  Therefore, we limit the number of iterations of nested
         template inclusion.
 
         """
         # Test template expansion at:
         # https://en.wikipedia.org/wiki/Special:ExpandTemplates
-        # https://it.wikipedia.org/wiki/Speciale:EspandiTemplate
 
         res = ''
-        if self.frame.depth >= self.maxTemplateRecursionLevels:
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
             self.recursion_exceeded_1_errs += 1
             return res
 
-        # logging.debug('%*s<expand', self.frame.depth, '')
+        # logging.debug('<expandTemplates ' + str(len(self.frame)))
 
         cur = 0
         # look for matching {{...}}
         for s, e in findMatchingBraces(wikitext, 2):
             res += wikitext[cur:s] + self.expandTemplate(wikitext[s + 2:e - 2])
             cur = e
         # leftover
         res += wikitext[cur:]
-        # logging.debug('%*sexpand> %s', self.frame.depth, '', res)
+        # logging.debug('   expandTemplates> %d %s', len(self.frame), res)
         return res
 
-
     def templateParams(self, parameters):
         """
         Build a dictionary with positional or name key to expanded parameters.
         :param parameters: the parts[1:] of a template, i.e. all except the title.
         """
         templateParams = {}
 
         if not parameters:
             return templateParams
-        # logging.debug('%*s<templateParams: %s', self.frame.length, '', '|'.join(parameters))
+        logging.debug('<templateParams: %s', '|'.join(parameters))
 
         # Parameters can be either named or unnamed. In the latter case, their
         # name is defined by their ordinal position (1, 2, 3, ...).
 
         unnamedParameterCounter = 0
 
         # It's legal for unnamed parameters to be skipped, in which case they
@@ -886,15 +1092,19 @@
             # Parameters may span several lines, like:
             # {{Reflist|colwidth=30em|refs=
             # &lt;ref name=&quot;Goode&quot;&gt;Title&lt;/ref&gt;
 
             # The '=' might occurr within an HTML attribute:
             #   "&lt;ref name=value"
             # but we stop at first.
-            m = re.match(' *([^=]*?) *?=(.*)', param, re.DOTALL)
+
+            # The '=' might occurr within quotes:
+            # ''''<span lang="pt-pt" xml:lang="pt-pt">cénicas</span>'''
+
+            m = re.match(" *([^=']*?) *=(.*)", param, re.DOTALL)
             if m:
                 # This is a named parameter.  This case also handles parameter
                 # assignments like "2=xxx", where the number of an unnamed
                 # parameter ("2") is specified explicitly - this is handled
                 # transparently.
 
                 parameterName = m.group(1).strip()
@@ -906,18 +1116,17 @@
             else:
                 # this is an unnamed parameter
                 unnamedParameterCounter += 1
 
                 if ']]' not in param:  # if the value does not contain a link, trim whitespace
                     param = param.strip()
                 templateParams[str(unnamedParameterCounter)] = param
-        # logging.debug('%*stemplateParams> %s', self.frame.length, '', '|'.join(templateParams.values()))
+        logging.debug('   templateParams> %s', '|'.join(templateParams.values()))
         return templateParams
 
-
     def expandTemplate(self, body):
         """Expands template invocation.
         :param body: the parts of a template.
 
         :see http://meta.wikimedia.org/wiki/Help:Expansion for an explanation
         of the process.
 
@@ -927,15 +1136,15 @@
         For most parser functions all names and values are expanded,
         regardless of what is relevant for the result. The branching functions
         (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are exceptions.
 
         All names in a template call are expanded, and the titles of the
         tplargs in the template body, after which it is determined which
         values must be expanded, and for which tplargs in the template body
-        the first part (default) [sic in the original doc page].
+        the first part (default).
 
         In the case of a tplarg, any parts beyond the first are never
         expanded.  The possible name and the value of the first part is
         expanded if the title does not match a name in the template call.
 
         :see code for braceSubstitution at
         https://doc.wikimedia.org/mediawiki-core/master/php/html/Parser_8php_source.html#3397:
@@ -955,85 +1164,72 @@
 
         # If a part has one or more equals signs in it, the first equals sign
         # determines the division into name = value. Equals signs inside inner
         # templates and tplargs, or inside double rectangular brackets within the
         # part are not taken into account in this decomposition. Parts without
         # equals sign are indexed 1, 2, .., given as attribute in the <name> tag.
 
-        if self.frame.depth >= self.maxTemplateRecursionLevels:
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
             self.recursion_exceeded_2_errs += 1
-            # logging.debug('%*sEXPAND> %s', self.frame.depth, '', body)
+            # logging.debug('   INVOCATION> %d %s', len(self.frame), body)
             return ''
 
-        logging.debug('%*sEXPAND %s', self.frame.depth, '', body)
+        logging.debug('INVOCATION %d %s', len(self.frame), body)
+
         parts = splitParts(body)
         # title is the portion before the first |
-        title = parts[0].strip()
-        title = self.expand(title)
+        logging.debug('TITLE %s', parts[0].strip())
+        title = self.expandTemplates(parts[0].strip())
 
         # SUBST
         # Apply the template tag to parameters without
         # substituting into them, e.g.
         # {{subst:t|a{{{p|q}}}b}} gives the wikitext start-a{{{p|q}}}b-end
         # @see https://www.mediawiki.org/wiki/Manual:Substitution#Partial_substitution
         subst = False
         if re.match(substWords, title, re.IGNORECASE):
             title = re.sub(substWords, '', title, 1, re.IGNORECASE)
             subst = True
 
-        if title in self.magicWords.values:
-            ret = self.magicWords[title]
-            logging.debug('%*s<EXPAND %s %s', self.frame.depth, '', title, ret)
-            return ret
-
-        # Parser functions.
-
-        # For most parser functions all names and values are expanded,
-        # regardless of what is relevant for the result. The branching
-        # functions (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are
-        # exceptions: for #if, #iferror, #ifexist, #ifexp, only the part that
-        # is applicable is expanded; for #ifeq the first and the applicable
-        # part are expanded; for #switch, expanded are the names up to and
-        # including the match (or all if there is no match), and the value in
-        # the case of a match or if there is no match, the default, if any.
+        if title.lower() in self.magicWords.values:
+            return self.magicWords[title.lower()]
 
+        # Parser functions
         # The first argument is everything after the first colon.
         # It has been evaluated above.
         colon = title.find(':')
         if colon > 1:
             funct = title[:colon]
             parts[0] = title[colon + 1:].strip()  # side-effect (parts[0] not used later)
             # arguments after first are not evaluated
-            ret = callParserFunction(funct, parts, self)
-            logging.debug('%*s<EXPAND %s %s', self.frame.depth, '', funct, ret)
-            return ret
+            ret = callParserFunction(funct, parts, self.frame)
+            return self.expandTemplates(ret)
 
         title = fullyQualifiedTemplateTitle(title)
         if not title:
             self.template_title_errs += 1
             return ''
 
-        redirected = options.redirects.get(title)
+        redirected = redirects.get(title)
         if redirected:
             title = redirected
 
         # get the template
-        if title in options.templateCache:
-            template = options.templateCache[title]
-        elif title in options.templates:
-            template = Template.parse(options.templates[title])
+        if title in templateCache:
+            template = templateCache[title]
+        elif title in templates:
+            template = Template.parse(templates[title])
             # add it to cache
-            options.templateCache[title] = template
-            del options.templates[title]
+            templateCache[title] = template
+            del templates[title]
         else:
             # The page being included could not be identified
-            logging.debug('%*s<EXPAND %s %s', self.frame.depth, '', title, '')
             return ''
 
-        logging.debug('%*sTEMPLATE %s: %s', self.frame.depth, '', title, template)
+        # logging.debug('TEMPLATE %s: %s', title, template)
 
         # tplarg          = "{{{" parts "}}}"
         # parts           = [ title *( "|" part ) ]
         # part            = ( part-name "=" part-value ) / ( part-value )
         # part-name       = wikitext-L3
         # part-value      = wikitext-L3
         # wikitext-L3     = literal / template / tplarg / link / comment /
@@ -1057,35 +1253,33 @@
         #   {{{{ }}}} -> { {{{ }}} }
         #   {{{{{ }}}}} -> {{ {{{ }}} }}
         #
         # :see: https://en.wikipedia.org/wiki/Help:Template#Handling_parameters
 
         params = parts[1:]
 
-        # Order of evaluation.
-        # Template parameters are fully evaluated before they are passed to the template.
-        # :see: https://www.mediawiki.org/wiki/Help:Templates#Order_of_evaluation
         if not subst:
             # Evaluate parameters, since they may contain templates, including
             # the symbol "=".
             # {{#ifexpr: {{{1}}} = 1 }}
-            params = [self.transform(p) for p in params]
+            params = [self.expandTemplates(p) for p in params]
 
         # build a dict of name-values for the parameter values
         params = self.templateParams(params)
 
-        # Perform parameter substitution.
-        # Extend frame before subst, since there may be recursion in default
+        # Perform parameter substitution
+        # extend frame before subst, since there may be recursion in default
         # parameter value, e.g. {{OTRS|celebrative|date=April 2015}} in article
         # 21637542 in enwiki.
-        self.frame = self.frame.push(title, params)
+        self.frame.append((title, params))
         instantiated = template.subst(params, self)
-        value = self.transform(instantiated)
-        self.frame = self.frame.pop()
-        logging.debug('%*s<EXPAND %s %s', self.frame.depth, '', title, value)
+        # logging.debug('instantiated %d %s', len(self.frame), instantiated)
+        value = self.expandTemplates(instantiated)
+        self.frame.pop()
+        # logging.debug('   INVOCATION> %s %d %s', title, len(self.frame), value)
         return value
 
 
 # ----------------------------------------------------------------------
 # parameter handling
 
 
@@ -1125,15 +1319,14 @@
     #    4|{{{{{subst|}}}CURRENTYEAR}}
     # and tpl parameters like:
     #    ||[[Category:People|{{#if:A|A|{{PAGENAME}}}}]]
 
     sep = '|'
     parameters = []
     cur = 0
-
     for s, e in findMatchingBraces(paramsList):
         par = paramsList[cur:s].split(sep)
         if par:
             if parameters:
                 # portion before | belongs to previous parameter
                 parameters[-1] += par[0]
                 if len(par) > 1:
@@ -1154,15 +1347,15 @@
             parameters[-1] += par[0]
             if len(par) > 1:
                 # rest are new parameters
                 parameters.extend(par[1:])
         else:
             parameters = par
 
-    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, text_type(parameters))
+    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, str(parameters))
     return parameters
 
 
 def findMatchingBraces(text, ldelim=0):
     """
     :param ldelim: number of braces to match. 0 means match [[]], {{}} and {{{}}}.
     """
@@ -1190,24 +1383,23 @@
 
     # We must skip individual { like in:
     #   {{#ifeq: {{padleft:|1|}} | { | | &nbsp;}}
     # We must resolve ambiguities like this:
     #   {{{{ }}}} -> { {{{ }}} }
     #   {{{{{ }}}}} -> {{ {{{ }}} }}
     #   {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|...}}
-    #   {{{!}} {{!}}}
 
     # Handle:
     #   {{{{{|safesubst:}}}#Invoke:String|replace|{{{1|{{{{{|safesubst:}}}PAGENAME}}}}}|%s+%([^%(]-%)$||plain=false}}
     # as well as expressions with stray }:
     #   {{{link|{{ucfirst:{{{1}}}}}} interchange}}}
 
     if ldelim:  # 2-3
         reOpen = re.compile('[{]{%d,}' % ldelim)  # at least ldelim
-        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2
+        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2 open or close bracces
     else:
         reOpen = re.compile('{{2,}|\[{2,}')
         reNext = re.compile('{{2,}|}{2,}|\[{2,}|]{2,}')  # at least 2
 
     cur = 0
     while True:
         m1 = reOpen.search(text, cur)
@@ -1244,15 +1436,15 @@
                         break
                 if not stack:
                     yield m1.start(), end - lmatch
                     cur = end
                     break
                 elif len(stack) == 1 and 0 < stack[0] < ldelim:
                     # ambiguous {{{{{ }}} }}
-                    #yield m1.start() + stack[0], end
+                    yield m1.start() + stack[0], end
                     cur = end
                     break
             elif brac == '[':  # [[
                 stack.append(-lmatch)
             else:  # ]]
                 while stack and stack[-1] < 0:  # matching [[
                     openCount = -stack.pop()
@@ -1268,24 +1460,24 @@
                     yield m1.start(), end - lmatch
                     cur = end
                     break
                 # unmatched ]] are discarded
                 cur = end
 
 
-def findBalanced(text, openDelim=['[['], closeDelim=[']]']):
+def findBalanced(text, openDelim, closeDelim):
     """
     Assuming that text contains a properly balanced expression using
     :param openDelim: as opening delimiters and
     :param closeDelim: as closing delimiters.
     :return: an iterator producing pairs (start, end) of start and end
     positions in text containing a balanced expression.
     """
     openPat = '|'.join([re.escape(x) for x in openDelim])
-    # pattern for delimiters expected after each opening delimiter
+    # patter for delimiters expected after each opening delimiter
     afterPat = {o: re.compile(openPat + '|' + c, re.DOTALL) for o, c in zip(openDelim, closeDelim)}
     stack = []
     start = 0
     cur = 0
     # end = len(text)
     startSet = False
     startPat = re.compile(openPat)
@@ -1309,355 +1501,27 @@
             else:
                 yield start, next.end()
                 nextPat = startPat
                 start = next.end()
                 startSet = False
         cur = next.end()
 
-
-# ----------------------------------------------------------------------
-# Modules
-
-# Only minimal support
-# FIXME: import Lua modules.
-
-def if_empty(*rest):
-    """
-    This implements If_empty from English Wikipedia module:
-
-       <title>Module:If empty</title>
-       <ns>828</ns>
-       <text>local p = {}
-
-    function p.main(frame)
-            local args = require('Module:Arguments').getArgs(frame, {wrappers = 'Template:If empty', removeBlanks = false})
-
-            -- For backwards compatibility reasons, the first 8 parameters can be unset instead of being blank,
-            -- even though there's really no legitimate use case for this. At some point, this will be removed.
-            local lowestNil = math.huge
-            for i = 8,1,-1 do
-                    if args[i] == nil then
-                            args[i] = ''
-                            lowestNil = i
-                    end
-            end
-
-            for k,v in ipairs(args) do
-                    if v ~= '' then
-                            if lowestNil &lt; k then
-                                    -- If any uses of this template depend on the behavior above, add them to a tracking category.
-                                    -- This is a rather fragile, convoluted, hacky way to do it, but it ensures that this module's output won't be modified
-                                    -- by it.
-                                    frame:extensionTag('ref', '[[Category:Instances of Template:If_empty missing arguments]]', {group = 'TrackingCategory'})
-                                    frame:extensionTag('references', '', {group = 'TrackingCategory'})
-                            end
-                            return v
-                    end
-            end
-    end
-
-    return p   </text>
-    """
-    for arg in rest:
-        if arg:
-            return arg
-    return ''
-
-
-# ----------------------------------------------------------------------
-# String module emulation
-# https://en.wikipedia.org/wiki/Module:String
-
-def functionParams(args, vars):
-    """
-    Build a dictionary of var/value from :param: args.
-    Parameters can be either named or unnamed. In the latter case, their
-    name is taken fron :param: vars.
-    """
-    params = {}
-    index = 1
-    for var in vars:
-        value = args.get(var)
-        if value is None:
-            value = args.get(str(index)) # positional argument
-            if value is None:
-                value = ''
-            else:
-                index += 1
-        params[var] = value
-    return params
-
-
-def string_sub(args):
-    params = functionParams(args, ('s', 'i', 'j'))
-    s = params.get('s', '')
-    i = int(params.get('i', 1) or 1) # or handles case of '' value
-    j = int(params.get('j', -1) or -1)
-    if i > 0: i -= 1             # lua is 1-based
-    if j < 0: j += 1
-    if j == 0: j = len(s)
-    return s[i:j]
-
-
-def string_sublength(args):
-    params = functionParams(args, ('s', 'i', 'len'))
-    s = params.get('s', '')
-    i = int(params.get('i', 1) or 1) - 1 # lua is 1-based
-    len = int(params.get('len', 1) or 1)
-    return s[i:i+len]
-
-
-def string_len(args):
-    params = functionParams(args, ('s'))
-    s = params.get('s', '')
-    return len(s)
-
-
-def string_find(args):
-    params = functionParams(args, ('source', 'target', 'start', 'plain'))
-    source = params.get('source', '')
-    pattern = params.get('target', '')
-    start = int('0'+params.get('start', 1)) - 1 # lua is 1-based
-    plain = int('0'+params.get('plain', 1))
-    if source == '' or pattern == '':
-        return 0
-    if plain:
-        return source.find(pattern, start) + 1 # lua is 1-based
-    else:
-        return (re.compile(pattern).search(source, start) or -1) + 1
-
-
-def string_pos(args):
-    params = functionParams(args, ('target', 'pos'))
-    target = params.get('target', '')
-    pos = int(params.get('pos', 1) or 1)
-    if pos > 0:
-        pos -= 1 # The first character has an index value of 1
-    return target[pos]
-
-
-def string_replace(args):
-    params = functionParams(args, ('source', 'pattern', 'replace', 'count', 'plain'))
-    source = params.get('source', '')
-    pattern = params.get('pattern', '')
-    replace = params.get('replace', '')
-    count = int(params.get('count', 0) or 0)
-    plain = int(params.get('plain', 1) or 1)
-    if plain:
-        if count:
-            return source.replace(pattern, replace, count)
-        else:
-            return source.replace(pattern, replace)
-    else:
-        return re.compile(pattern).sub(replace, source, count)
-
-
-def string_rep(args):
-    params = functionParams(args, ('s'))
-    source = params.get('source', '')
-    count = int(params.get('count', '1'))
-    return source * count
-
-
-# ----------------------------------------------------------------------
-# Module:Roman
-# http://en.wikipedia.org/w/index.php?title=Module:Roman
-# Modulo:Numero_romano
-# https://it.wikipedia.org/wiki/Modulo:Numero_romano
-
-def roman_main(args):
-    """Convert first arg to roman numeral if <= 5000 else :return: second arg."""
-    num = int(float(args.get('1')))
-
-    # Return a message for numbers too big to be expressed in Roman numerals.
-    if 0 > num or num >= 5000:
-        return args.get('2', 'N/A')
-
-    def toRoman(n, romanNumeralMap):
-        """convert integer to Roman numeral"""
-        result = ""
-        for integer, numeral in romanNumeralMap:
-            while n >= integer:
-                result += numeral
-                n -= integer
-        return result
-
-    # Find the Roman numerals for numbers 4999 or less.
-    smallRomans = (
-        (1000, "M"),
-        (900, "CM"), (500, "D"), (400, "CD"), (100, "C"),
-        (90, "XC"), (50, "L"), (40, "XL"), (10, "X"),
-        (9, "IX"), (5, "V"), (4, "IV"), (1, "I")
-    )
-    return toRoman(num, smallRomans)
-
-# ----------------------------------------------------------------------
-
-modules = {
-    'convert': {
-        'convert': lambda x, u, *rest: x + ' ' + u,  # no conversion
-    },
-
-    'If empty': {
-        'main': if_empty
-    },
-
-    'String': {
-        'len': string_len,
-        'sub': string_sub,
-        'sublength': string_sublength,
-        'pos': string_pos,
-        'find': string_find,
-        'replace': string_replace,
-        'rep': string_rep,
-    },
-
-    'Roman': {
-        'main': roman_main
-    },
-
-    'Numero romano': {
-        'main': roman_main
-    }
-}
-
-# ----------------------------------------------------------------------
-# variables
-
-
-class MagicWords(object):
-    """
-    One copy in each Extractor.
-
-    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
-    """
-    names = [
-        '!',
-        'currentmonth',
-        'currentmonth1',
-        'currentmonthname',
-        'currentmonthnamegen',
-        'currentmonthabbrev',
-        'currentday',
-        'currentday2',
-        'currentdayname',
-        'currentyear',
-        'currenttime',
-        'currenthour',
-        'localmonth',
-        'localmonth1',
-        'localmonthname',
-        'localmonthnamegen',
-        'localmonthabbrev',
-        'localday',
-        'localday2',
-        'localdayname',
-        'localyear',
-        'localtime',
-        'localhour',
-        'numberofarticles',
-        'numberoffiles',
-        'numberofedits',
-        'articlepath',
-        'pageid',
-        'sitename',
-        'server',
-        'servername',
-        'scriptpath',
-        'stylepath',
-        'pagename',
-        'pagenamee',
-        'fullpagename',
-        'fullpagenamee',
-        'namespace',
-        'namespacee',
-        'namespacenumber',
-        'currentweek',
-        'currentdow',
-        'localweek',
-        'localdow',
-        'revisionid',
-        'revisionday',
-        'revisionday2',
-        'revisionmonth',
-        'revisionmonth1',
-        'revisionyear',
-        'revisiontimestamp',
-        'revisionuser',
-        'revisionsize',
-        'subpagename',
-        'subpagenamee',
-        'talkspace',
-        'talkspacee',
-        'subjectspace',
-        'subjectspacee',
-        'talkpagename',
-        'talkpagenamee',
-        'subjectpagename',
-        'subjectpagenamee',
-        'numberofusers',
-        'numberofactiveusers',
-        'numberofpages',
-        'currentversion',
-        'rootpagename',
-        'rootpagenamee',
-        'basepagename',
-        'basepagenamee',
-        'currenttimestamp',
-        'localtimestamp',
-        'directionmark',
-        'contentlanguage',
-        'numberofadmins',
-        'cascadingsources',
-    ]
-
-    def __init__(self):
-        self.values = {'!': '|'}
-
-    def __getitem__(self, name):
-        return self.values.get(name)
-
-    def __setitem__(self, name, value):
-        self.values[name] = value
-
-    switches = (
-        '__NOTOC__',
-        '__FORCETOC__',
-        '__TOC__',
-        '__TOC__',
-        '__NEWSECTIONLINK__',
-        '__NONEWSECTIONLINK__',
-        '__NOGALLERY__',
-        '__HIDDENCAT__',
-        '__NOCONTENTCONVERT__',
-        '__NOCC__',
-        '__NOTITLECONVERT__',
-        '__NOTC__',
-        '__START__',
-        '__END__',
-        '__INDEX__',
-        '__NOINDEX__',
-        '__STATICREDIRECT__',
-        '__DISAMBIG__'
-    )
-
-
-magicWordsRE = re.compile('|'.join(MagicWords.switches))
-
-
 # ----------------------------------------------------------------------
 # parser functions utilities
 
 
 def ucfirst(string):
     """:return: a string with just its first character uppercase
     We can't use title() since it coverts all words.
     """
     if string:
-        return string[0].upper() + string[1:]
+        if len(string) > 1:
+            return string[0].upper() + string[1:]
+        else:
+            return string.upper()
     else:
         return ''
 
 
 def lcfirst(string):
     """:return: a string with its first character lowercase"""
     if string:
@@ -1679,44 +1543,45 @@
         return ucfirst(templateTitle[1:])
     else:
         m = re.match('([^:]*)(:.*)', templateTitle)
         if m:
             # colon found but not in the first position - check if it
             # designates a known namespace
             prefix = normalizeNamespace(m.group(1))
-            if prefix in options.knownNamespaces:
+            if prefix in knownNamespaces:
                 return prefix + ucfirst(m.group(2))
     # The title of the page being included is NOT in the main namespace and
     # lacks any other explicit designation of the namespace - therefore, it
     # is resolved to the Template namespace (that's the default for the
     # template inclusion mechanism).
 
     # This is a defense against pages whose title only contains UTF-8 chars
     # that are reduced to an empty string. Right now I can think of one such
     # case - <C2><A0> which represents the non-breaking space.
     # In this particular case, this page is a redirect to [[Non-nreaking
     # space]], but having in the system a redirect page with an empty title
     # causes numerous problems, so we'll live happier without it.
     if templateTitle:
-        return options.templatePrefix + ucfirst(templateTitle)
+        return Extractor.templatePrefix + ucfirst(templateTitle)
     else:
         return ''  # caller may log as error
 
 
 def normalizeNamespace(ns):
     return ucfirst(ns)
 
 
 # ----------------------------------------------------------------------
 # Parser functions
 # see http://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
 # https://github.com/Wikia/app/blob/dev/extensions/ParserFunctions/ParserFunctions_body.php
 
 
-class Infix:
+class Infix():
+
     """Infix operators.
     The calling sequence for the infix is:
       x |op| y
     """
 
     def __init__(self, function):
         self.function = function
@@ -1736,72 +1601,67 @@
     def __call__(self, value1, value2):
         return self.function(value1, value2)
 
 
 ROUND = Infix(lambda x, y: round(x, y))
 
 
-from math import floor, ceil, pi, e, trunc, exp, log as ln, sin, cos, tan, asin, acos, atan
-
-
-def sharp_expr(extr, expr):
-    """Tries converting a lua expr into a Python expr."""
+def sharp_expr(expr):
     try:
-        expr = extr.expand(expr)
-        expr = re.sub('(?<![!<>])=', '==', expr) # negative lookbehind
-        expr = re.sub('mod', '%', expr)          # no \b here
+        expr = re.sub('=', '==', expr)
+        expr = re.sub('mod', '%', expr)
         expr = re.sub('\bdiv\b', '/', expr)
         expr = re.sub('\bround\b', '|ROUND|', expr)
-        return text_type(eval(expr))
+        return str(eval(expr))
     except:
-        return '<span class="error">%s</span>' % expr
+        return '<span class="error"></span>'
 
 
-def sharp_if(extr, testValue, valueIfTrue, valueIfFalse=None, *args):
+def sharp_if(testValue, valueIfTrue, valueIfFalse=None, *args):
     # In theory, we should evaluate the first argument here,
     # but it was evaluated while evaluating part[0] in expandTemplate().
     if testValue.strip():
         # The {{#if:}} function is an if-then-else construct.
         # The applied condition is: "The condition string is non-empty".
-        valueIfTrue = extr.expand(valueIfTrue.strip()) # eval
+        valueIfTrue = valueIfTrue.strip()
         if valueIfTrue:
             return valueIfTrue
     elif valueIfFalse:
-        return extr.expand(valueIfFalse.strip()) # eval
+        return valueIfFalse.strip()
     return ""
 
 
-def sharp_ifeq(extr, lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
+def sharp_ifeq(lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
     rvalue = rvalue.strip()
     if rvalue:
-        # lvalue is always evaluated
+        # lvalue is always defined
         if lvalue.strip() == rvalue:
             # The {{#ifeq:}} function is an if-then-else construct. The
             # applied condition is "is rvalue equal to lvalue". Note that this
             # does only string comparison while MediaWiki implementation also
             # supports numerical comparissons.
 
             if valueIfTrue:
-                return extr.expand(valueIfTrue.strip())
+                return valueIfTrue.strip()
         else:
             if valueIfFalse:
-                return extr.expand(valueIfFalse.strip())
+                return valueIfFalse.strip()
     return ""
 
 
-def sharp_iferror(extr, test, then='', Else=None, *args):
+def sharp_iferror(test, then='', Else=None, *args):
     if re.match('<(?:strong|span|p|div)\s(?:[^\s>]*\s+)*?class="(?:[^"\s>]*\s+)*?error(?:\s[^">]*)?"', test):
-        return extr.expand(then.strip())
+        return then
     elif Else is None:
         return test.strip()
     else:
-        return extr.expand(Else.strip())
+        return Else.strip()
 
 
-def sharp_switch(extr, primary, *params):
+def sharp_switch(primary, *params):
     # FIXME: we don't support numeric expressions in primary
 
     # {{#switch: comparison string
     #  | case1 = result1
     #  | case2
     #  | case4 = result2
     #  | 1 | case5 = result3
@@ -1813,19 +1673,19 @@
     default = None
     rvalue = None
     lvalue = ''
     for param in params:
         # handle cases like:
         #  #default = [http://www.perseus.tufts.edu/hopper/text?doc=Perseus...]
         pair = param.split('=', 1)
-        lvalue = extr.expand(pair[0].strip())
+        lvalue = pair[0].strip()
         rvalue = None
         if len(pair) > 1:
             # got "="
-            rvalue = extr.expand(pair[1].strip())
+            rvalue = pair[1].strip()
             # check for any of multiple values pipe separated
             if found or primary in [v.strip() for v in lvalue.split('|')]:
                 # Found a match, return now
                 return rvalue
             elif lvalue == '#default':
                 default = rvalue
             rvalue = None  # avoid defaulting to last case
@@ -1837,21 +1697,33 @@
     if rvalue is not None:
         return lvalue
     elif default is not None:
         return default
     return ''
 
 
-# Extension Scribunto: https://www.mediawiki.org/wiki/Extension:Scribunto
-def sharp_invoke(module, function, args):
+# Extension Scribuntu
+def sharp_invoke(module, function, frame):
     functions = modules.get(module)
     if functions:
         funct = functions.get(function)
         if funct:
-            return text_type(funct(args))
+            # find parameters in frame whose title is the one of the original
+            # template invocation
+            templateTitle = fullyQualifiedTemplateTitle(function)
+            if not templateTitle:
+                logging.warn("Template with empty title")
+            pair = next((x for x in frame if x[0] == templateTitle), None)
+            if pair:
+                params = pair[1]
+                # extract positional args
+                params = [params.get(str(i + 1)) for i in range(len(params))]
+                return funct(*params)
+            else:
+                return funct()
     return ''
 
 
 parserFunctions = {
 
     '#expr': sharp_expr,
 
@@ -1859,121 +1731,102 @@
 
     '#ifeq': sharp_ifeq,
 
     '#iferror': sharp_iferror,
 
     '#ifexpr': lambda *args: '',  # not supported
 
-    '#ifexist': lambda extr, title, ifex, ifnex: extr.expand(ifnex), # assuming title is not present
+    '#ifexist': lambda *args: '',  # not supported
 
     '#rel2abs': lambda *args: '',  # not supported
 
     '#switch': sharp_switch,
 
-    '#language': lambda *args: '', # not supported
+    '# language': lambda *args: '',  # not supported
 
-    '#time': lambda *args: '',     # not supported
+    '#time': lambda *args: '',  # not supported
 
-    '#timel': lambda *args: '',    # not supported
+    '#timel': lambda *args: '',  # not supported
 
-    '#titleparts': lambda *args: '', # not supported
+    '#titleparts': lambda *args: '',  # not supported
 
     # This function is used in some pages to construct links
     # http://meta.wikimedia.org/wiki/Help:URL
-    'urlencode': lambda extr, string, *rest: quote(string.encode('utf-8')),
+    'urlencode': lambda string, *rest: urlencode(string),
 
-    'lc': lambda extr, string, *rest: string.lower() if string else '',
+    'lc': lambda string, *rest: string.lower() if string else '',
 
-    'lcfirst': lambda extr, string, *rest: lcfirst(string),
+    'lcfirst': lambda string, *rest: lcfirst(string),
 
-    'uc': lambda extr, string, *rest: string.upper() if string else '',
+    'uc': lambda string, *rest: string.upper() if string else '',
 
-    'ucfirst': lambda extr, string, *rest: ucfirst(string),
+    'ucfirst': lambda string, *rest: ucfirst(string),
 
-    'int': lambda extr, string, *rest: text_type(int(string)),
+    'int': lambda string, *rest: str(int(string)),
+
+    'padleft': lambda char, width, string: string.ljust(char, int(pad)), # CHECK_ME
 
 }
 
 
-def callParserFunction(functionName, args, extractor):
+def callParserFunction(functionName, args, frame):
     """
     Parser functions have similar syntax as templates, except that
     the first argument is everything after the first colon.
+    :param functionName: nameof the parser function
+    :param args: the arguments to the function
     :return: the result of the invocation, None in case of failure.
 
-    :param: args not yet expanded (see branching functions).
-    https://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
+    http://meta.wikimedia.org/wiki/Help:ParserFunctions
     """
 
     try:
-        # https://it.wikipedia.org/wiki/Template:Str_endswith has #Invoke
-        functionName = functionName.lower()
         if functionName == '#invoke':
-            module, fun = args[0].strip(), args[1].strip()
-            logging.debug('%*s#invoke %s %s %s', extractor.frame.depth, '', module, fun, args[2:])
             # special handling of frame
-            if len(args) == 2:
-                # find parameters in frame whose title is the one of the original
-                # template invocation
-                templateTitle = fullyQualifiedTemplateTitle(module)
-                if not templateTitle:
-                    logging.warn("Template with empty title")
-                params = None
-                frame = extractor.frame
-                while frame:
-                    if frame.title == templateTitle:
-                        params = frame.args
-                        break
-                    frame = frame.prev
-            else:
-                params = [extractor.transform(p) for p in args[2:]] # evaluates them
-                params = extractor.templateParams(params)
-            ret = sharp_invoke(module, fun, params)
-            logging.debug('%*s<#invoke %s %s %s', extractor.frame.depth, '', module, fun, ret)
+            ret = sharp_invoke(args[0].strip(), args[1].strip(), frame)
+            # logging.debug('parserFunction> %s %s', args[1], ret)
             return ret
         if functionName in parserFunctions:
-            # branching functions use the extractor to selectively evaluate args
-            return parserFunctions[functionName](extractor, *args)
+            ret = parserFunctions[functionName](*args)
+            # logging.debug('parserFunction> %s(%s) %s', functionName, args, ret)
+            return ret
     except:
         return ""  # FIXME: fix errors
-    return ""
-
 
-# ----------------------------------------------------------------------
-# Expand using WikiMedia API
-# import json
+    return ""
 
-# def expand(text):
-#     """Expand templates invoking MediaWiki API"""
-#     text = urlib.urlencodew(text.encode('utf-8'))
-#     base = urlbase[:urlbase.rfind('/')]
-#     url = base + "/w/api.php?action=expandtemplates&format=json&text=" + text
-#     exp = json.loads(urllib.urlopen(url))
-#     return exp['expandtemplates']['*']
 
 # ----------------------------------------------------------------------
 # Extract Template definition
 
 reNoinclude = re.compile(r'<noinclude>(?:.*?)</noinclude>', re.DOTALL)
 reIncludeonly = re.compile(r'<includeonly>|</includeonly>', re.DOTALL)
 
+# These are built before spawning processes, hence they are shared.
+templates = {}
+redirects = {}
+# cache of parser templates
+# FIXME: sharing this with a Manager slows down.
+templateCache = {}
+
+
 def define_template(title, page):
     """
     Adds a template defined in the :param page:.
     @see https://en.wikipedia.org/wiki/Help:Template#Noinclude.2C_includeonly.2C_and_onlyinclude
     """
-    # title = normalizeTitle(title)
+    global templates
+    global redirects
 
-    # sanity check (empty template, e.g. Template:Crude Oil Prices))
-    if not page: return
+    # title = normalizeTitle(title)
 
     # check for redirects
     m = re.match('#REDIRECT.*?\[\[([^\]]*)]]', page[0], re.IGNORECASE)
     if m:
-        options.redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
+        redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
         return
 
     text = unescape(''.join(page))
 
     # We're storing template text for future inclusion, therefore,
     # remove all <noinclude> text and keep all <includeonly> text
     # (but eliminate <includeonly> tags per se).
@@ -1997,1243 +1850,10 @@
         onlyincludeAccumulator += m.group(1)
     if onlyincludeAccumulator:
         text = onlyincludeAccumulator
     else:
         text = reIncludeonly.sub('', text)
 
     if text:
-        if title in options.templates:
+        if title in templates and templates[title] != text:
             logging.warn('Redefining: %s', title)
-        options.templates[title] = text
-
-
-# ----------------------------------------------------------------------
-
-def dropNested(text, openDelim, closeDelim):
-    """
-    A matching function for nested expressions, e.g. namespaces and tables.
-    """
-    openRE = re.compile(openDelim, re.IGNORECASE)
-    closeRE = re.compile(closeDelim, re.IGNORECASE)
-    # partition text in separate blocks { } { }
-    spans = []                  # pairs (s, e) for each partition
-    nest = 0                    # nesting level
-    start = openRE.search(text, 0)
-    if not start:
-        return text
-    end = closeRE.search(text, start.end())
-    next = start
-    while end:
-        next = openRE.search(text, next.end())
-        if not next:            # termination
-            while nest:         # close all pending
-                nest -= 1
-                end0 = closeRE.search(text, end.end())
-                if end0:
-                    end = end0
-                else:
-                    break
-            spans.append((start.start(), end.end()))
-            break
-        while end.end() < next.start():
-            # { } {
-            if nest:
-                nest -= 1
-                # try closing more
-                last = end.end()
-                end = closeRE.search(text, end.end())
-                if not end:     # unbalanced
-                    if spans:
-                        span = (spans[0][0], last)
-                    else:
-                        span = (start.start(), last)
-                    spans = [span]
-                    break
-            else:
-                spans.append((start.start(), end.end()))
-                # advance start, find next close
-                start = next
-                end = closeRE.search(text, next.end())
-                break           # { }
-        if next != start:
-            # { { }
-            nest += 1
-    # collect text outside partitions
-    return dropSpans(spans, text)
-
-
-def dropSpans(spans, text):
-    """
-    Drop from text the blocks identified in :param spans:, possibly nested.
-    """
-    spans.sort()
-    res = ''
-    offset = 0
-    for s, e in spans:
-        if offset <= s:         # handle nesting
-            if offset < s:
-                res += text[offset:s]
-            offset = e
-    res += text[offset:]
-    return res
-
-
-# ----------------------------------------------------------------------
-# WikiLinks
-
-# May be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
-# Also: [[Help:IPA for Catalan|[andora]]]
-
-
-def replaceInternalLinks(text):
-    """
-    Replaces internal links of the form:
-    [[title |...|label]]trail
-
-    with title concatenated with trail, when present, e.g. 's' for plural.
-
-    See https://www.mediawiki.org/wiki/Help:Links#Internal_links
-    """
-    # call this after removal of external links, so we need not worry about
-    # triple closing ]]].
-    cur = 0
-    res = ''
-    for s, e in findBalanced(text):
-        m = tailRE.match(text, e)
-        if m:
-            trail = m.group(0)
-            end = m.end()
-        else:
-            trail = ''
-            end = e
-        inner = text[s + 2:e - 2]
-        # find first |
-        pipe = inner.find('|')
-        if pipe < 0:
-            title = inner
-            label = title
-        else:
-            title = inner[:pipe].rstrip()
-            # find last |
-            curp = pipe + 1
-            for s1, e1 in findBalanced(inner):
-                last = inner.rfind('|', curp, s1)
-                if last >= 0:
-                    pipe = last  # advance
-                curp = e1
-            label = inner[pipe + 1:].strip()
-        res += text[cur:s] + makeInternalLink(title, label) + trail
-        cur = end
-    return res + text[cur:]
-
-
-# the official version is a method in class Parser, similar to this:
-# def replaceInternalLinks2(text):
-#     global wgExtraInterlanguageLinkPrefixes
-
-#     # the % is needed to support urlencoded titles as well
-#     tc = Title::legalChars() + '#%'
-#     # Match a link having the form [[namespace:link|alternate]]trail
-#     e1 = re.compile("([%s]+)(?:\\|(.+?))?]](.*)" % tc, re.S | re.D)
-#     # Match cases where there is no "]]", which might still be images
-#     e1_img = re.compile("([%s]+)\\|(.*)" % tc, re.S | re.D)
-
-#     holders = LinkHolderArray(self)
-
-#     # split the entire text string on occurrences of [[
-#     iterBrackets = re.compile('[[').finditer(text)
-
-#     m in iterBrackets.next()
-#     # get the first element (all text up to first [[)
-#     s = text[:m.start()]
-#     cur = m.end()
-
-#     line = s
-
-#     useLinkPrefixExtension = self.getTargetLanguage().linkPrefixExtension()
-#     e2 = None
-#     if useLinkPrefixExtension:
-#         # Match the end of a line for a word that is not followed by whitespace,
-#         # e.g. in the case of "The Arab al[[Razi]]",  "al" will be matched
-#         global wgContLang
-#         charset = wgContLang.linkPrefixCharset()
-#         e2 = re.compile("((?>.*[^charset]|))(.+)", re.S | re.D | re.U)
-
-#     if self.mTitle is None:
-#         raise MWException(__METHOD__ + ": \self.mTitle is null\n")
-
-#     nottalk = not self.mTitle.isTalkPage()
-
-#     if useLinkPrefixExtension:
-#         m = e2.match(s)
-#         if m:
-#             first_prefix = m.group(2)
-#         else:
-#             first_prefix = false
-#     else:
-#         prefix = ''
-
-#     useSubpages = self.areSubpagesAllowed()
-
-#     for m in iterBrackets:
-#         line = text[cur:m.start()]
-#         cur = m.end()
-
-#         # TODO: Check for excessive memory usage
-
-#         if useLinkPrefixExtension:
-#             m = e2.match(e2)
-#             if m:
-#                 prefix = m.group(2)
-#                 s = m.group(1)
-#             else:
-#                 prefix = ''
-#             # first link
-#             if first_prefix:
-#                 prefix = first_prefix
-#                 first_prefix = False
-
-#         might_be_img = False
-
-#         m = e1.match(line)
-#         if m: # page with normal label or alt
-#             label = m.group(2)
-#             # If we get a ] at the beginning of m.group(3) that means we have a link that is something like:
-#             # [[Image:Foo.jpg|[http://example.com desc]]] <- having three ] in a row fucks up,
-#             # the real problem is with the e1 regex
-#             # See bug 1300.
-#             #
-#             # Still some problems for cases where the ] is meant to be outside punctuation,
-#             # and no image is in sight. See bug 2095.
-#             #
-#             if label and m.group(3)[0] == ']' and '[' in label:
-#                 label += ']' # so that replaceExternalLinks(label) works later
-#                 m.group(3) = m.group(3)[1:]
-#             # fix up urlencoded title texts
-#             if '%' in m.group(1):
-#                 # Should anchors '#' also be rejected?
-#                 m.group(1) = str_replace(array('<', '>'), array('&lt', '&gt'), rawurldecode(m.group(1)))
-#             trail = m.group(3)
-#         else:
-#             m = e1_img.match(line):
-#             if m:
-#                 # Invalid, but might be an image with a link in its caption
-#                 might_be_img = true
-#                 label = m.group(2)
-#                 if '%' in m.group(1):
-#                     m.group(1) = rawurldecode(m.group(1))
-#                 trail = ""
-#             else:		# Invalid form; output directly
-#                 s += prefix + '[[' + line
-#                 continue
-
-#         origLink = m.group(1)
-
-#         # Dont allow internal links to pages containing
-#         # PROTO: where PROTO is a valid URL protocol these
-#         # should be external links.
-#         if (preg_match('/^(?i:' + self.mUrlProtocols + ')/', origLink)) {
-#             s += prefix + '[[' + line
-#             continue
-#         }
-
-#         # Make subpage if necessary
-#         if useSubpages:
-#             link = self.maybeDoSubpageLink(origLink, label)
-#         else:
-#             link = origLink
-
-#         noforce = origLink[0] != ':'
-#         if not noforce:
-#             # Strip off leading ':'
-#             link = link[1:]
-
-#         nt = Title::newFromText(self.mStripState.unstripNoWiki(link))
-#         if nt is None:
-#             s += prefix + '[[' + line
-#             continue
-
-#         ns = nt.getNamespace()
-#         iw = nt.getInterwiki()
-
-#         if might_be_img {	# if this is actually an invalid link
-#             if (ns == NS_FILE and noforce) { # but might be an image
-#                 found = False
-#                 while True:
-#                     # look at the next 'line' to see if we can close it there
-#                     next_line = iterBrakets.next()
-#                     if not next_line:
-#                         break
-#                     m = explode(']]', next_line, 3)
-#                     if m.lastindex == 3:
-#                         # the first ]] closes the inner link, the second the image
-#                         found = True
-#                         label += "[[%s]]%s" % (m.group(0), m.group(1))
-#                         trail = m.group(2)
-#                         break
-#                     elif m.lastindex == 2:
-#                         # if there is exactly one ]] that is fine, we will keep looking
-#                         label += "[[{m[0]}]]{m.group(1)}"
-#                     else:
-#                         # if next_line is invalid too, we need look no further
-#                         label += '[[' + next_line
-#                         break
-#                 if not found:
-#                     # we couldnt find the end of this imageLink, so output it raw
-#                     # but dont ignore what might be perfectly normal links in the text we ve examined
-#                     holders.merge(self.replaceInternalLinks2(label))
-#                     s += "{prefix}[[%s|%s" % (link, text)
-#                     # note: no trail, because without an end, there *is* no trail
-#                     continue
-#             } else: # it is not an image, so output it raw
-#                 s += "{prefix}[[%s|%s" % (link, text)
-#                 # note: no trail, because without an end, there *is* no trail
-#                      continue
-#         }
-
-#         wasblank = (text == '')
-#         if wasblank:
-#             text = link
-#         else:
-#             # Bug 4598 madness.  Handle the quotes only if they come from the alternate part
-#             # [[Lista d''e paise d''o munno]] . <a href="...">Lista d''e paise d''o munno</a>
-#             # [[Criticism of Harry Potter|Criticism of ''Harry Potter'']]
-#             #    . <a href="Criticism of Harry Potter">Criticism of <i>Harry Potter</i></a>
-#             text = self.doQuotes(text)
-
-#         # Link not escaped by : , create the various objects
-#         if noforce and not nt.wasLocalInterwiki():
-#             # Interwikis
-#             if iw and mOptions.getInterwikiMagic() and nottalk and (
-#                     Language::fetchLanguageName(iw, None, 'mw') or
-#                     in_array(iw, wgExtraInterlanguageLinkPrefixes)):
-#                 # Bug 24502: filter duplicates
-#                 if iw not in mLangLinkLanguages:
-#                     self.mLangLinkLanguages[iw] = True
-#                     self.mOutput.addLanguageLink(nt.getFullText())
-
-#                 s = rstrip(s + prefix)
-#                 s += strip(trail, "\n") == '' ? '': prefix + trail
-#                 continue
-
-#             if ns == NS_FILE:
-#                 if not wfIsBadImage(nt.getDBkey(), self.mTitle):
-#                     if wasblank:
-#                         # if no parameters were passed, text
-#                         # becomes something like "File:Foo.png",
-#                         # which we dont want to pass on to the
-#                         # image generator
-#                         text = ''
-#                     else:
-#                         # recursively parse links inside the image caption
-#                         # actually, this will parse them in any other parameters, too,
-#                         # but it might be hard to fix that, and it doesnt matter ATM
-#                         text = self.replaceExternalLinks(text)
-#                         holders.merge(self.replaceInternalLinks2(text))
-#                     # cloak any absolute URLs inside the image markup, so replaceExternalLinks() wont touch them
-#                     s += prefix + self.armorLinks(
-#                         self.makeImage(nt, text, holders)) + trail
-#                 else:
-#                     s += prefix + trail
-#                 continue
-
-#             if ns == NS_CATEGORY:
-#                 s = rstrip(s + "\n") # bug 87
-
-#                 if wasblank:
-#                     sortkey = self.getDefaultSort()
-#                 else:
-#                     sortkey = text
-#                 sortkey = Sanitizer::decodeCharReferences(sortkey)
-#                 sortkey = str_replace("\n", '', sortkey)
-#                 sortkey = self.getConverterLanguage().convertCategoryKey(sortkey)
-#                 self.mOutput.addCategory(nt.getDBkey(), sortkey)
-
-#                 s += strip(prefix + trail, "\n") == '' ? '' : prefix + trail
-
-#                 continue
-#             }
-#         }
-
-#         # Self-link checking. For some languages, variants of the title are checked in
-#         # LinkHolderArray::doVariants() to allow batching the existence checks necessary
-#         # for linking to a different variant.
-#         if ns != NS_SPECIAL and nt.equals(self.mTitle) and !nt.hasFragment():
-#             s += prefix + Linker::makeSelfLinkObj(nt, text, '', trail)
-#                  continue
-
-#         # NS_MEDIA is a pseudo-namespace for linking directly to a file
-#         # @todo FIXME: Should do batch file existence checks, see comment below
-#         if ns == NS_MEDIA:
-#             # Give extensions a chance to select the file revision for us
-#             options = []
-#             descQuery = False
-#             Hooks::run('BeforeParserFetchFileAndTitle',
-#                        [this, nt, &options, &descQuery])
-#             # Fetch and register the file (file title may be different via hooks)
-#             file, nt = self.fetchFileAndTitle(nt, options)
-#             # Cloak with NOPARSE to avoid replacement in replaceExternalLinks
-#             s += prefix + self.armorLinks(
-#                 Linker::makeMediaLinkFile(nt, file, text)) + trail
-#             continue
-
-#         # Some titles, such as valid special pages or files in foreign repos, should
-#         # be shown as bluelinks even though they are not included in the page table
-#         #
-#         # @todo FIXME: isAlwaysKnown() can be expensive for file links; we should really do
-#         # batch file existence checks for NS_FILE and NS_MEDIA
-#         if iw == '' and nt.isAlwaysKnown():
-#             self.mOutput.addLink(nt)
-#             s += self.makeKnownLinkHolder(nt, text, array(), trail, prefix)
-#         else:
-#             # Links will be added to the output link list after checking
-#             s += holders.makeHolder(nt, text, array(), trail, prefix)
-#     }
-#     return holders
-
-
-def makeInternalLink(title, label):
-    colon = title.find(':')
-    if colon > 0 and title[:colon] not in options.acceptedNamespaces:
-        return ''
-    if colon == 0:
-        # drop also :File:
-        colon2 = title.find(':', colon + 1)
-        if colon2 > 1 and title[colon + 1:colon2] not in options.acceptedNamespaces:
-            return ''
-    if options.keepLinks:
-        return '<a href="%s">%s</a>' % (quote(title.encode('utf-8')), label)
-    else:
-        return label
-
-
-# ----------------------------------------------------------------------
-# External links
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
-
-wgUrlProtocols = [
-    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
-    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
-    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
-    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
-]
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
-
-# Constants needed for external link processing
-# Everything except bracket, space, or control characters
-# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
-# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
-EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
-ANCHOR_CLASS = r'[^][\x00-\x08\x0a-\x1F]'
-ExtLinkBracketedRegex = re.compile(
-    '\[(((?i)' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)' +
-    r'\s*((?:' + ANCHOR_CLASS + r'|\[\[' + ANCHOR_CLASS + r'+\]\])' + r'*?)\]',
-    re.S | re.U)
-# A simpler alternative:
-# ExtLinkBracketedRegex = re.compile(r'\[(.*?)\](?!])')
-
-EXT_IMAGE_REGEX = re.compile(
-    r"""^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
-    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.((?i)gif|png|jpg|jpeg)$""",
-    re.X | re.S | re.U)
-
-
-def replaceExternalLinks(text):
-    """
-    https://www.mediawiki.org/wiki/Help:Links#External_links
-    [URL anchor text]
-    """
-    s = ''
-    cur = 0
-    for m in ExtLinkBracketedRegex.finditer(text):
-        s += text[cur:m.start()]
-        cur = m.end()
-
-        url = m.group(1)
-        label = m.group(3)
-
-        # # The characters '<' and '>' (which were escaped by
-        # # removeHTMLtags()) should not be included in
-        # # URLs, per RFC 2396.
-        # m2 = re.search('&(lt|gt);', url)
-        # if m2:
-        #     link = url[m2.end():] + ' ' + link
-        #     url = url[0:m2.end()]
-
-        # If the link text is an image URL, replace it with an <img> tag
-        # This happened by accident in the original parser, but some people used it extensively
-        m = EXT_IMAGE_REGEX.match(label)
-        if m:
-            label = makeExternalImage(label)
-
-        # Use the encoded URL
-        # This means that users can paste URLs directly into the text
-        # Funny characters like ö aren't valid in URLs anyway
-        # This was changed in August 2004
-        s += makeExternalLink(url, label)  # + trail
-
-    return s + text[cur:]
-
-
-def makeExternalLink(url, anchor):
-    """Function applied to wikiLinks"""
-    if options.keepLinks:
-        return '<a href="%s">%s</a>' % (quote(url.encode('utf-8')), anchor)
-    else:
-        return anchor
-
-
-def makeExternalImage(url, alt=''):
-    if options.keepLinks:
-        return '<img src="%s" alt="%s">' % (url, alt)
-    else:
-        return alt
-
-
-# ----------------------------------------------------------------------
-
-# match tail after wikilink
-tailRE = re.compile('\w+')
-
-syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
-
-# skip level 1, it is page name level
-section = re.compile(r'(==+)\s*(.*?)\s*\1')
-
-listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
-listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
-listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
-            ':': '<dd>%s</dd>'}
-
-
-def compact(text):
-    """Deal with headers, lists, empty sections, residuals of tables.
-    :param text: convert to HTML.
-    """
-
-    page = []             # list of paragraph
-    headers = {}          # Headers for unfilled sections
-    emptySection = False  # empty sections are discarded
-    listLevel = []        # nesting of lists
-    listCount = []        # count of each list (it should be always in the same length of listLevel)
-    for line in text.split('\n'):
-        if not line:            # collapse empty lines
-            # if there is an opening list, close it if we see an empty line
-            if len(listLevel):
-                page.append(line)
-                if options.toHTML:
-                    for c in reversed(listLevel):
-                        page.append(listClose[c])
-                listLevel = []
-                listCount = []
-                emptySection = False
-            elif page and page[-1]:
-                page.append('')
-            continue
-        # Handle section titles
-        m = section.match(line)
-        if m:
-            title = m.group(2)
-            lev = len(m.group(1)) # header level
-            if options.toHTML:
-                page.append("<h%d>%s</h%d>" % (lev, title, lev))
-            if title and title[-1] not in '!?':
-                title += '.'    # terminate sentence.
-            headers[lev] = title
-            # drop previous headers
-            for i in list(headers.keys()):
-                if i > lev:
-                    del headers[i]
-            emptySection = True
-            listLevel = []
-            listCount = []
-            continue
-        # Handle page title
-        elif line.startswith('++'):
-            title = line[2:-2]
-            if title:
-                if title[-1] not in '!?':
-                    title += '.'
-                page.append(title)
-        # handle indents
-        elif line[0] == ':':
-            # page.append(line.lstrip(':*#;'))
-            continue
-        # handle lists
-        elif line[0] in '*#;:':
-            i = 0
-            # c: current level char
-            # n: next level char
-            for c, n in zip_longest(listLevel, line, fillvalue=''):
-                if not n or n not in '*#;:': # shorter or different
-                    if c:
-                        if options.toHTML:
-                            page.append(listClose[c])
-                        listLevel = listLevel[:-1]
-                        listCount = listCount[:-1]
-                        continue
-                    else:
-                        break
-                # n != ''
-                if c != n and (not c or (c not in ';:' and n not in ';:')):
-                    if c:
-                        # close level
-                        if options.toHTML:
-                            page.append(listClose[c])
-                        listLevel = listLevel[:-1]
-                        listCount = listCount[:-1]
-                    listLevel += n
-                    listCount.append(0)
-                    if options.toHTML:
-                        page.append(listOpen[n])
-                i += 1
-            n = line[i - 1]  # last list char
-            line = line[i:].strip()
-            if line:  # FIXME: n is '"'
-                if options.keepLists:
-                    if options.keepSections:
-                        # emit open sections
-                        items = sorted(headers.items())
-                        for _, v in items:
-                            page.append(v)
-                    headers.clear()
-                    # use item count for #-lines
-                    listCount[i - 1] += 1
-                    bullet = '%d. ' % listCount[i - 1] if n == '#' else '- '
-                    page.append('{0:{1}s}'.format(bullet, len(listLevel)) + line)
-                elif options.toHTML:
-                    page.append(listItem[n] % line)
-        elif len(listLevel):
-            if options.toHTML:
-                for c in reversed(listLevel):
-                    page.append(listClose[c])
-            listLevel = []
-            listCount = []
-            page.append(line)
-
-        # Drop residuals of lists
-        elif line[0] in '{|' or line[-1] == '}':
-            continue
-        # Drop irrelevant lines
-        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
-            continue
-        elif len(headers):
-            if options.keepSections:
-                items = sorted(headers.items())
-                for i, v in items:
-                    page.append(v)
-            headers.clear()
-            page.append(line)  # first line
-            emptySection = False
-        elif not emptySection:
-            # Drop preformatted
-            if line[0] != ' ':  # dangerous
-                page.append(line)
-    return page
-
-
-def handle_unicode(entity):
-    numeric_code = int(entity[2:-1])
-    if numeric_code >= 0x10000: return ''
-    return chr(numeric_code)
-
-
-# ------------------------------------------------------------------------------
-# Output
-
-
-class NextFile(object):
-    """
-    Synchronous generation of next available file name.
-    """
-
-    filesPerDir = 100
-
-    def __init__(self, path_name):
-        self.path_name = path_name
-        self.dir_index = -1
-        self.file_index = -1
-
-    def __next__(self):
-        self.file_index = (self.file_index + 1) % NextFile.filesPerDir
-        if self.file_index == 0:
-            self.dir_index += 1
-        dirname = self._dirname()
-        if not os.path.isdir(dirname):
-            os.makedirs(dirname)
-        return self._filepath()
-
-    next = __next__
-
-    def _dirname(self):
-        char1 = self.dir_index % 26
-        char2 = self.dir_index // 26 % 26
-        return os.path.join(self.path_name, '%c%c' % (ord('A') + char2, ord('A') + char1))
-
-    def _filepath(self):
-        return '%s/wiki_%02d' % (self._dirname(), self.file_index)
-
-
-class OutputSplitter(object):
-    """
-    File-like object, that splits output to multiple files of a given max size.
-    """
-
-    def __init__(self, nextFile, max_file_size=0, compress=True):
-        """
-        :param nextFile: a NextFile object from which to obtain filenames
-            to use.
-        :param max_file_size: the maximum size of each file.
-        :para compress: whether to write data with bzip compression.
-        """
-        self.nextFile = nextFile
-        self.compress = compress
-        self.max_file_size = max_file_size
-        self.file = self.open(next(self.nextFile))
-
-    def reserve(self, size):
-        if self.file.tell() + size > self.max_file_size:
-            self.close()
-            self.file = self.open(next(self.nextFile))
-
-    def write(self, data):
-        self.reserve(len(data))
-        self.file.write(data)
-
-    def close(self):
-        self.file.close()
-
-    def open(self, filename):
-        if self.compress:
-            return bz2.BZ2File(filename + '.bz2', 'w')
-        else:
-            return open(filename, 'wb')
-
-
-# ----------------------------------------------------------------------
-# READER
-
-tagRE = re.compile(r'(.*?)<(/?\w+)[^>]*?>(?:([^<]*)(<.*?>)?)?')
-#                    1     2               3      4
-keyRE = re.compile(r'key="(\d*)"')
-
-def load_templates(file, output_file=None):
-    """
-    Load templates from :param file:.
-    :param output_file: file where to save templates and modules.
-    """
-    options.templatePrefix = options.templateNamespace + ':'
-    options.modulePrefix = options.moduleNamespace + ':'
-
-    if output_file:
-        output = codecs.open(output_file, 'wb', 'utf-8')
-    for page_count, page_data in enumerate(pages_from(file)):
-        id, revid, title, ns, page = page_data
-        if not output_file and (not options.templateNamespace or
-                                not options.moduleNamespace):  # do not know it yet
-            # reconstruct templateNamespace and moduleNamespace from the first title
-            if ns in templateKeys:
-                colon = title.find(':')
-                if colon > 1:
-                    if ns == '10':
-                        options.templateNamespace = title[:colon]
-                        options.templatePrefix = title[:colon + 1]
-                    elif ns == '828':
-                        options.moduleNamespace = title[:colon]
-                        options.modulePrefix = title[:colon + 1]
-        if ns in templateKeys:
-            text = ''.join(page)
-            define_template(title, text)
-            # save templates and modules to file
-            if output_file:
-                output.write('<page>\n')
-                output.write('   <title>%s</title>\n' % title)
-                output.write('   <ns>%s</ns>\n' % ns)
-                output.write('   <id>%s</id>\n' % id)
-                output.write('   <text>')
-                for line in page:
-                    output.write(line)
-                output.write('   </text>\n')
-                output.write('</page>\n')
-        if page_count and page_count % 100000 == 0:
-            logging.info("Preprocessed %d pages", page_count)
-    if output_file:
-        output.close()
-        logging.info("Saved %d templates to '%s'", len(options.templates), output_file)
-
-
-def pages_from(input):
-    """
-    Scans input extracting pages.
-    :return: (id, revid, title, namespace key, page), page is a list of lines.
-    """
-    # we collect individual lines, since str.join() is significantly faster
-    # than concatenation
-    page = []
-    id = None
-    ns = '0'
-    last_id = None
-    revid = None
-    inText = False
-    redirect = False
-    title = None
-    for line in input:
-        if not isinstance(line, text_type): line = line.decode('utf-8')
-        if '<' not in line:  # faster than doing re.search()
-            if inText:
-                page.append(line)
-            continue
-        m = tagRE.search(line)
-        if not m:
-            continue
-        tag = m.group(2)
-        if tag == 'page':
-            page = []
-            redirect = False
-        elif tag == 'id' and not id:
-            id = m.group(3)
-        elif tag == 'id' and id:
-            revid = m.group(3)
-        elif tag == 'title':
-            title = m.group(3)
-        elif tag == 'ns':
-            ns = m.group(3)
-        elif tag == 'redirect':
-            redirect = True
-        elif tag == 'text':
-            if m.lastindex == 3 and line[m.start(3)-2] == '/': # self closing
-                # <text xml:space="preserve" />
-                continue
-            inText = True
-            line = line[m.start(3):m.end(3)]
-            page.append(line)
-            if m.lastindex == 4:  # open-close
-                inText = False
-        elif tag == '/text':
-            if m.group(1):
-                page.append(m.group(1))
-            inText = False
-        elif inText:
-            page.append(line)
-        elif tag == '/page':
-            if id != last_id and not redirect:
-                yield (id, revid, title, ns, page)
-                last_id = id
-                ns = '0'
-            id = None
-            revid = None
-            title = None
-            page = []
-
-
-def process_dump(input_file, template_file, out_file, file_size, file_compress,
-                 process_count):
-    """
-    :param input_file: name of the wikipedia dump file; '-' to read from stdin
-    :param template_file: optional file with template definitions.
-    :param out_file: directory where to store extracted data, or '-' for stdout
-    :param file_size: max size of each extracted file, or None for no max (one file)
-    :param file_compress: whether to compress files with bzip.
-    :param process_count: number of extraction processes to spawn.
-    """
-
-    if input_file == '-':
-        input = sys.stdin
-    else:
-        input = fileinput.FileInput(input_file, openhook=fileinput.hook_compressed)
-
-    # collect siteinfo
-    for line in input:
-        # When an input file is .bz2 or .gz, line can be a bytes even in Python 3.
-        if not isinstance(line, text_type): line = line.decode('utf-8')
-        m = tagRE.search(line)
-        if not m:
-            continue
-        tag = m.group(2)
-        if tag == 'base':
-            # discover urlbase from the xml dump file
-            # /mediawiki/siteinfo/base
-            base = m.group(3)
-            options.urlbase = base[:base.rfind("/")]
-        elif tag == 'namespace':
-            mk = keyRE.search(line)
-            if mk:
-                nsid = mk.group(1)
-            else:
-                nsid = ''
-            options.knownNamespaces[m.group(3)] = nsid
-            if re.search('key="10"', line):
-                options.templateNamespace = m.group(3)
-                options.templatePrefix = options.templateNamespace + ':'
-            elif re.search('key="828"', line):
-                options.moduleNamespace = m.group(3)
-                options.modulePrefix = options.moduleNamespace + ':'
-        elif tag == '/siteinfo':
-            break
-
-    if options.expand_templates:
-        # preprocess
-        template_load_start = default_timer()
-        if template_file:
-            if os.path.exists(template_file):
-                logging.info("Loading template definitions from: %s", template_file)
-                # can't use with here:
-                file = fileinput.FileInput(template_file,
-                                           openhook=fileinput.hook_compressed)
-                load_templates(file)
-                file.close()
-            else:
-                if input_file == '-':
-                    # can't scan then reset stdin; must error w/ suggestion to specify template_file
-                    raise ValueError("to use templates with stdin dump, must supply explicit template-file")
-                logging.info("Preprocessing '%s' to collect template definitions: this may take some time.", input_file)
-                load_templates(input, template_file)
-                input.close()
-                input = fileinput.FileInput(input_file, openhook=fileinput.hook_compressed)
-        template_load_elapsed = default_timer() - template_load_start
-        logging.info("Loaded %d templates in %.1fs", len(options.templates), template_load_elapsed)
-
-    # process pages
-    logging.info("Starting page extraction from %s.", input_file)
-    extract_start = default_timer()
-
-    # Parallel Map/Reduce:
-    # - pages to be processed are dispatched to workers
-    # - a reduce process collects the results, sort them and print them.
-
-    process_count = max(1, process_count)
-    maxsize = 10 * process_count
-    # output queue
-    output_queue = Queue(maxsize=maxsize)
-
-    if out_file == '-':
-        out_file = None
-
-    worker_count = process_count
-
-    # load balancing
-    max_spool_length = 10000
-    spool_length = Value('i', 0, lock=False)
-
-    # reduce job that sorts and prints output
-    reduce = Process(target=reduce_process,
-                     args=(options, output_queue, spool_length,
-                           out_file, file_size, file_compress))
-    reduce.start()
-
-    # initialize jobs queue
-    jobs_queue = Queue(maxsize=maxsize)
-
-    # start worker processes
-    logging.info("Using %d extract processes.", worker_count)
-    workers = []
-    for i in range(worker_count):
-        extractor = Process(target=extract_process,
-                            args=(options, i, jobs_queue, output_queue))
-        extractor.daemon = True  # only live while parent process lives
-        extractor.start()
-        workers.append(extractor)
-
-    # Mapper process
-    page_num = 0
-    for page_data in pages_from(input):
-        id, revid, title, ns, page = page_data
-        if keepPage(ns, page):
-            # slow down
-            delay = 0
-            if spool_length.value > max_spool_length:
-                # reduce to 10%
-                while spool_length.value > max_spool_length/10:
-                    time.sleep(10)
-                    delay += 10
-            if delay:
-                logging.info('Delay %ds', delay)
-            job = (id, revid, title, page, page_num)
-            jobs_queue.put(job) # goes to any available extract_process
-            page_num += 1
-        page = None             # free memory
-
-    input.close()
-
-    # signal termination
-    for _ in workers:
-        jobs_queue.put(None)
-    # wait for workers to terminate
-    for w in workers:
-        w.join()
-
-    # signal end of work to reduce process
-    output_queue.put(None)
-    # wait for it to finish
-    reduce.join()
-
-    extract_duration = default_timer() - extract_start
-    extract_rate = page_num / extract_duration
-    logging.info("Finished %d-process extraction of %d articles in %.1fs (%.1f art/s)",
-                 process_count, page_num, extract_duration, extract_rate)
-
-
-# ----------------------------------------------------------------------
-# Multiprocess support
-
-
-def extract_process(opts, i, jobs_queue, output_queue):
-    """Pull tuples of raw page content, do CPU/regex-heavy fixup, push finished text
-    :param i: process id.
-    :param jobs_queue: where to get jobs.
-    :param output_queue: where to queue extracted text for output.
-    """
-
-    global options
-    options = opts
-
-    createLogger(options.quiet, options.debug)
-
-    out = StringIO()                 # memory buffer
-
-
-    while True:
-        job = jobs_queue.get()  # job is (id, title, page, page_num)
-        if job:
-            id, revid, title, page, page_num = job
-            try:
-                e = Extractor(*job[:4]) # (id, revid, title, page)
-                page = None              # free memory
-                e.extract(out)
-                text = out.getvalue()
-            except:
-                text = ''
-                logging.exception('Processing page: %s %s', id, title)
-
-            output_queue.put((page_num, text))
-            out.truncate(0)
-            out.seek(0)
-        else:
-            logging.debug('Quit extractor')
-            break
-    out.close()
-
-
-report_period = 10000           # progress report period
-def reduce_process(opts, output_queue, spool_length,
-                   out_file=None, file_size=0, file_compress=True):
-    """Pull finished article text, write series of files (or stdout)
-    :param opts: global parameters.
-    :param output_queue: text to be output.
-    :param spool_length: spool length.
-    :param out_file: filename where to print.
-    :param file_size: max file size.
-    :param file_compress: whether to compress output.
-    """
-
-    global options
-    options = opts
-
-    createLogger(options.quiet, options.debug)
-
-    if out_file:
-        nextFile = NextFile(out_file)
-        output = OutputSplitter(nextFile, file_size, file_compress)
-    else:
-        output = sys.stdout if PY2 else sys.stdout.buffer
-        if file_compress:
-            logging.warn("writing to stdout, so no output compression (use an external tool)")
-
-    interval_start = default_timer()
-    # FIXME: use a heap
-    spool = {}        # collected pages
-    next_page = 0     # sequence numbering of page
-    while True:
-        if next_page in spool:
-            output.write(spool.pop(next_page).encode('utf-8'))
-            next_page += 1
-            # tell mapper our load:
-            spool_length.value = len(spool)
-            # progress report
-            if next_page % report_period == 0:
-                interval_rate = report_period / (default_timer() - interval_start)
-                logging.info("Extracted %d articles (%.1f art/s)",
-                             next_page, interval_rate)
-                interval_start = default_timer()
-        else:
-            # mapper puts None to signal finish
-            pair = output_queue.get()
-            if not pair:
-                break
-            page_num, text = pair
-            spool[page_num] = text
-            # tell mapper our load:
-            spool_length.value = len(spool)
-            # FIXME: if an extractor dies, process stalls; the other processes
-            # continue to produce pairs, filling up memory.
-            if len(spool) > 200:
-                logging.debug('Collected %d, waiting: %d, %d', len(spool),
-                              next_page, next_page == page_num)
-    if output != sys.stdout:
-        output.close()
-
-
-# ----------------------------------------------------------------------
-
-# Minimum size of output files
-minFileSize = 200 * 1024
-
-def main():
-
-    parser = argparse.ArgumentParser(prog=os.path.basename(sys.argv[0]),
-                                     formatter_class=argparse.RawDescriptionHelpFormatter,
-                                     description=__doc__)
-    parser.add_argument("input",
-                        help="XML wiki dump file")
-    groupO = parser.add_argument_group('Output')
-    groupO.add_argument("-o", "--output", default="text",
-                        help="directory for extracted files (or '-' for dumping to stdout)")
-    groupO.add_argument("-b", "--bytes", default="1M",
-                        help="maximum bytes per output file (default %(default)s)",
-                        metavar="n[KMG]")
-    groupO.add_argument("-c", "--compress", action="store_true",
-                        help="compress output files using bzip")
-    groupO.add_argument("--json", action="store_true",
-                        help="write output in json format instead of the default one")
-
-
-    groupP = parser.add_argument_group('Processing')
-    groupP.add_argument("--html", action="store_true",
-                        help="produce HTML output, subsumes --links")
-    groupP.add_argument("-l", "--links", action="store_true",
-                        help="preserve links")
-    groupP.add_argument("-s", "--sections", action="store_true",
-                        help="preserve sections")
-    groupP.add_argument("--lists", action="store_true",
-                        help="preserve lists")
-    groupP.add_argument("-ns", "--namespaces", default="", metavar="ns1,ns2",
-                        help="accepted namespaces in links")
-    groupP.add_argument("--templates",
-                        help="use or create file containing templates")
-    groupP.add_argument("--no-templates", action="store_false",
-                        help="Do not expand templates")
-    groupP.add_argument("-r", "--revision", action="store_true", default=options.print_revision,
-                        help="Include the document revision id (default=%(default)s)")
-    groupP.add_argument("--min_text_length", type=int, default=options.min_text_length,
-                        help="Minimum expanded text length required to write document (default=%(default)s)")
-    groupP.add_argument("--filter_disambig_pages", action="store_true", default=options.filter_disambig_pages,
-                        help="Remove pages from output that contain disabmiguation markup (default=%(default)s)")
-    groupP.add_argument("-it", "--ignored_tags", default="", metavar="abbr,b,big",
-                        help="comma separated list of tags that will be dropped, keeping their content")
-    groupP.add_argument("-de", "--discard_elements", default="", metavar="gallery,timeline,noinclude",
-                        help="comma separated list of elements that will be removed from the article text")
-    groupP.add_argument("--keep_tables", action="store_true", default=options.keep_tables,
-                        help="Preserve tables in the output article text (default=%(default)s)")
-    default_process_count = max(1, cpu_count() - 1)
-    parser.add_argument("--processes", type=int, default=default_process_count,
-                        help="Number of processes to use (default %(default)s)")
-
-    groupS = parser.add_argument_group('Special')
-    groupS.add_argument("-q", "--quiet", action="store_true",
-                        help="suppress reporting progress info")
-    groupS.add_argument("--debug", action="store_true",
-                        help="print debug info")
-    groupS.add_argument("-a", "--article", action="store_true",
-                        help="analyze a file containing a single article (debug option)")
-    groupS.add_argument("-v", "--version", action="version",
-                        version='%(prog)s ' + version,
-                        help="print program version")
-
-    args = parser.parse_args()
-
-    options.keepLinks = args.links
-    options.keepSections = args.sections
-    options.keepLists = args.lists
-    options.toHTML = args.html
-    options.write_json = args.json
-    options.print_revision = args.revision
-    options.min_text_length = args.min_text_length
-    if args.html:
-        options.keepLinks = True
-
-    options.expand_templates = args.no_templates
-    options.filter_disambig_pages = args.filter_disambig_pages
-    options.keep_tables = args.keep_tables
-
-    try:
-        power = 'kmg'.find(args.bytes[-1].lower()) + 1
-        file_size = int(args.bytes[:-1]) * 1024 ** power
-        if file_size < minFileSize:
-            raise ValueError()
-    except ValueError:
-        logging.error('Insufficient or invalid size: %s', args.bytes)
-        return
-
-    if args.namespaces:
-        options.acceptedNamespaces = set(args.namespaces.split(','))
-
-    # ignoredTags and discardElemets have default values already supplied, if passed in the defaults are overwritten
-    if args.ignored_tags:
-        ignoredTags = set(args.ignored_tags.split(','))
-    else:
-        ignoredTags = [
-            'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'em',
-            'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd',
-            'p', 'plaintext', 's', 'span', 'strike', 'strong',
-            'tt', 'u', 'var',  'a', 'br', 'small', 'div', 'td',
-            'nowiki', 'ref', 'sup'
-        ]
-
-    # 'a' tag is handled separately
-    for tag in ignoredTags:
-        ignoreTag(tag)
-
-    if args.discard_elements:
-        options.discardElements = set(args.discard_elements.split(','))
-
-    FORMAT = '%(levelname)s: %(message)s'
-    logging.basicConfig(format=FORMAT)
-
-    options.quiet = args.quiet
-    options.debug = args.debug
-
-    createLogger(options.quiet, options.debug)
-
-    input_file = args.input
-
-    if not options.keepLinks:
-        ignoreTag('a')
-
-    # sharing cache of parser templates is too slow:
-    # manager = Manager()
-    # templateCache = manager.dict()
-
-    if args.article:
-        if args.templates:
-            if os.path.exists(args.templates):
-                with open(args.templates) as file:
-                    load_templates(file)
-
-        file = fileinput.FileInput(input_file, openhook=fileinput.hook_compressed)
-        for page_data in pages_from(file):
-            id, revid, title, ns, page = page_data
-            Extractor(id, revid, title, page).extract(sys.stdout)
-        file.close()
-        return
-
-    output_path = args.output
-    if output_path != '-' and not os.path.isdir(output_path):
-        try:
-            os.makedirs(output_path)
-        except:
-            logging.error('Could not create: %s', output_path)
-            return
-
-    process_dump(input_file, args.templates, output_path, file_size,
-                 args.compress, args.processes)
-
-def createLogger(quiet, debug):
-    logger = logging.getLogger()
-    if not quiet:
-        logger.setLevel(logging.INFO)
-    if debug:
-        logger.setLevel(logging.DEBUG)
-
-if __name__ == '__main__':
-    main()
+        templates[title] = text
```

### Comparing `hazm-0.7.0/hazm/data/stopwords.dat` & `hazm-0.9.0/hazm/data/stopwords.dat`

 * *Files identical despite different names*

