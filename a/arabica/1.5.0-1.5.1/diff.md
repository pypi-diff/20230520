# Comparing `tmp/arabica-1.5.0.tar.gz` & `tmp/arabica-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.5.0.tar", last modified: Thu May 18 21:25:51 2023, max compression
+gzip compressed data, was "arabica-1.5.1.tar", last modified: Sat May 20 11:04:13 2023, max compression
```

## Comparing `arabica-1.5.0.tar` & `arabica-1.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:25:51.834072 arabica-1.5.0/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     7527 2023-05-18 21:25:51.834072 arabica-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 21:25:51.829773 arabica-1.5.0/arabica/
--rw-rw-rw-   0        0        0      105 2023-05-18 21:01:56.000000 arabica-1.5.0/arabica/__init__.py
--rw-rw-rw-   0        0        0    12373 2023-04-29 22:20:26.000000 arabica-1.5.0/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.5.0/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.5.0/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.5.0/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.5.0/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.5.0/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.5.0/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.5.0/arabica/sentiment.py
--rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.5.0/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:25:51.834072 arabica-1.5.0/arabica.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-05-18 21:25:51.000000 arabica-1.5.0/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-18 21:25:51.000000 arabica-1.5.0/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:25:51.000000 arabica-1.5.0/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-18 21:25:51.000000 arabica-1.5.0/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 21:25:51.000000 arabica-1.5.0/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-05-18 21:25:24.000000 arabica-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 21:25:51.834072 arabica-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-18 21:25:24.000000 arabica-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:04:13.261922 arabica-1.5.1/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     7527 2023-05-20 11:04:13.261922 arabica-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 11:04:13.261922 arabica-1.5.1/arabica/
+-rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.5.1/arabica/__init__.py
+-rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.5.1/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.5.1/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.5.1/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.5.1/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7819 2023-05-20 10:56:18.000000 arabica-1.5.1/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.5.1/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.5.1/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.5.1/arabica/sentiment.py
+-rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.5.1/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:04:13.261922 arabica-1.5.1/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7527 2023-05-20 11:04:13.000000 arabica-1.5.1/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-05-20 11:04:13.000000 arabica-1.5.1/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:04:13.000000 arabica-1.5.1/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-20 11:04:13.000000 arabica-1.5.1/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 11:04:13.000000 arabica-1.5.1/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-05-20 11:03:03.000000 arabica-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 11:04:13.261922 arabica-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-20 11:03:03.000000 arabica-1.5.1/setup.py
```

### Comparing `arabica-1.5.0/PKG-INFO` & `arabica-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.5.0/README.md` & `arabica-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.5.0/arabica/arabica_freq.py` & `arabica-1.5.1/arabica/arabica_freq.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nltk.util import trigrams as tri
 
 from .preprocess import *
 from .clean_numbers import *
 from .stopwords import *
 from .group import grouper
 from .clean_ngram import *
+import sys
 
 
 def arabica_freq(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  stopwords: [],             # Languages for stop words
                  skip: [],                  # Remove additional strings
@@ -38,14 +39,17 @@
         data['time']=data['time'].astype(str)
         data['time'] = pd.to_datetime(data['time'], dayfirst=True)
 
     elif date_format == 'us':
         data['time']=data['time'].astype(str)
         data['time'] = pd.to_datetime(data['time'], dayfirst=False)
 
+    else:
+        sys.exit('Incorrect value for date_format parameter. Allowed: "us", "eur"')
+
     # cleaning - blank rows
     data=data.set_index(data['time'])
     data.replace("", float("NaN"), inplace=True)
     data.dropna(subset = ["text"], inplace=True)
 
     # cleaning - unwanted strings
     if skip is not None:
```

### Comparing `arabica-1.5.0/arabica/cappuccino.py` & `arabica-1.5.1/arabica/cappuccino.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from plotnine import *
 from arabica import arabica_freq
 from wordcloud import WordCloud
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import figure
 import pandas as pd
 import numpy as np
+import sys
 
 import nltk
 nltk.download('stopwords')
 
 
 def cappuccino(text: str,                  # Text
                time: str,                  # Time
@@ -31,15 +32,14 @@
                           time_freq = time_freq,
                           max_words = max_words,
                           stopwords = stopwords,
                           skip = skip,
                           numbers = numbers,
                           lower_case = lower_case)
 
-
     if ngram == 1:
         if time_freq == 'ungroup':
             if plot == 'wordcloud':
                 unigrams_df = result[['unigram','unigram_freq']]
                 unigrams_df = unigrams_df.dropna()
                 unigrams_df['unigram_freq'] = unigrams_df['unigram_freq'].astype(int)
                 unigrams_dict = dict(unigrams_df.values)
@@ -52,14 +52,17 @@
                                               margin=10).generate_from_frequencies(unigrams_dict)
                 plt.figure(dpi=1200)
                 plt.imshow(wordcloud_unigram,interpolation="bilinear")
                 fig.set_size_inches(10, 6, forward=True)
                 plt.axis('off')
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "wordcloud"')
+
 
         elif time_freq == 'M':
             period = result['period']
             subset = result['unigram']
             subset = subset.dropna()
             subset_expand = subset.str.split(pat=",", expand=True)
             subset_expand.columns = ['unigram' + str(i + 1) for i in range(len(subset_expand.columns))]
@@ -144,14 +147,17 @@
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "heatmap", "line"')
+
 
         elif time_freq == 'Y':
             period = result['period']
             subset = result['unigram']
             subset = subset.dropna()
             subset_expand = subset.str.split(pat=",", expand=True)
             subset_expand.columns = ['unigram' + str(i + 1) for i in range(len(subset_expand.columns))]
@@ -234,14 +240,20 @@
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "heatmap", "line"')
+
+        else:
+            sys.exit('Incorrect value for time_freq parameter. Allowed: "ungroup", "Y", "M"')
+
     elif ngram == 2:
         if time_freq == 'ungroup':
             if plot == 'wordcloud':
                 bigram_df = result[['bigram','bigram_freq']]
                 bigram_df = bigram_df.dropna()
                 bigram_df['bigram'] = bigram_df['bigram'].str.replace(",", " ")
                 bigram_df['bigram_freq'] = bigram_df['bigram_freq'].astype(int)
@@ -255,14 +267,17 @@
                                              ).generate_from_frequencies(bigrams_dict)
                 plt.figure(dpi=1200)
                 plt.imshow(wordcloud_bigram,interpolation="bilinear")
                 fig.set_size_inches(10, 6, forward=True)
                 plt.axis('off')
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "wordcloud"')
+
         elif time_freq == 'M':
             period = result['period']
             subset = result['bigram']
             subset = subset.dropna()
             subset_expand = subset.str.split(pat=",", expand=True)
 
             cols = (' '.join(w) for w in zip(subset_expand.columns[::2].astype(str), subset_expand.columns[1::2].astype(str)))
@@ -345,14 +360,18 @@
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "heatmap", "line"')
+
+
         elif time_freq == 'Y':
             period = result['period']
             subset = result['bigram']
             subset = subset.dropna()
             subset_expand = subset.str.split(pat=",", expand=True)
 
             cols = (' '.join(w) for w in zip(subset_expand.columns[::2].astype(str), subset_expand.columns[1::2].astype(str)))
@@ -436,14 +455,20 @@
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "heatmap", "line"')
+
+        else:
+            sys.exit('Incorrect value for time_freq parameter. Allowed: "ungroup", "Y", "M"')
+
     elif ngram == 3:
         if time_freq == 'ungroup':
             if plot == 'wordcloud':
                 trigram_df = result[['trigram','trigram_freq']]
                 trigram_df = trigram_df.dropna()
                 trigram_df['trigram'] = trigram_df['trigram'].str.replace(",", " ")
                 trigram_df['trigram_freq'] = trigram_df['trigram_freq'].astype(int)
@@ -457,9 +482,17 @@
                                               margin=10).generate_from_frequencies(trigram_dict)
                 plt.figure(dpi=1200)
                 plt.imshow(wordcloud_trigram,interpolation="bilinear")
                 fig.set_size_inches(10, 6, forward=True)
                 plt.axis('off')
                 picture = plt.show()
 
+            else:
+                sys.exit('Incorrect value for plot parameter. Allowed: "wordcloud"')
+
+        else:
+            sys.exit('Incorrect value for time_freq parameter. Allowed: "ungroup"')
+
+    else:
+        sys.exit("Incorrect value for ngram parameter. Allowed: 1,2,3.")
 
     return picture
```

### Comparing `arabica-1.5.0/arabica/clean_ngram.py` & `arabica-1.5.1/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.0/arabica/coffee_break.py` & `arabica-1.5.1/arabica/coffee_break.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,28 @@
                  time: str,                  # Time column
                  date_format: str,           # Date format: 'eur' - European, 'us' - American
                  skip: [ ],                  # Remove additional strings
                  preprocess: bool = False,   # Clean data from numbers and punctuation
                  time_freq: int = '',        # Aggregation period: 'Y'/'M'
                  n_breaks: int = ''):        # Number of breaks: min. 2
 
+    date_formats = ["eur", "us"]
+    frequencies = ["M", "Y"]
+
+    if date_format in date_formats:
+        pass
+    else:
+        sys.exit('Incorrect value for date_format parameter. Allowed: "eur", "us"')
+
+
+    if time_freq in frequencies:
+        pass
+    else:
+        sys.exit('Incorrect value for time_freq parameter. Allowed: "M", "Y"')
+
 
     if n_breaks is not None:
         if n_breaks < 2:
             sys.exit("N_breaks parameter is too low. Increase it!")
 
         else:
             pass
@@ -77,15 +91,15 @@
             plt.plot(ts, label='sentiment')
             plt.grid(linewidth=0.5)
             plt.xlabel('Period', size = 13, labelpad = 6)
             plt.ylabel('Sentiment', size = 13, labelpad = 6)
             plt.legend(loc = 'best', fontsize = 13)
             picture = plt.show()
 
-        else:
+        elif n_breaks is not None:
             sentiment_ts.reset_index(drop = True, inplace = True)
             sentiment_ts['period'] = pd.to_datetime(sentiment_ts['period'].astype('str'))
             sentiment_ts['period'] = sentiment_ts['period'].dt.strftime('%Y-%m')
 
             ts = sentiment_ts
             ts.set_index('period', inplace = True)
             ts.index = pd.to_datetime(ts.index, format='%Y-%m').to_period("m")
@@ -150,15 +164,15 @@
             plt.grid(linewidth=0.5)
             plt.xlabel('Period', size = 13, labelpad = 8)
             plt.xticks(ts.index, rotation = 45)
             plt.ylabel('Sentiment', size = 13, labelpad = 6)
             plt.legend(loc = 'best', fontsize = 13)
             picture = plt.show()
 
-        else:
+        elif n_breaks is not None:
             sentiment_ts.reset_index(drop = True, inplace = True)
             sentiment_ts['period'] = pd.to_datetime(sentiment_ts['period'].astype('str'))
             sentiment_ts['period'] = sentiment_ts['period'].dt.strftime('%Y')
 
             ts = sentiment_ts
             ts.set_index('period', inplace = True)
             ts.index = pd.to_datetime(ts.index, format='%Y').year
```

### Comparing `arabica-1.5.0/arabica/group.py` & `arabica-1.5.1/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.0/arabica/preprocess.py` & `arabica-1.5.1/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.0/arabica/stopwords.py` & `arabica-1.5.1/arabica/stopwords.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.0/arabica.egg-info/PKG-INFO` & `arabica-1.5.1/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.5.0/pyproject.toml` & `arabica-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.5.0/setup.py` & `arabica-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.5.0",
+        version="1.5.1",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

