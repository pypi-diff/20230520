# Comparing `tmp/references_parser-1.1.2.tar.gz` & `tmp/references_parser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "references_parser-1.1.2.tar", last modified: Fri May 19 04:17:01 2023, max compression
+gzip compressed data, was "references_parser-1.2.0.tar", last modified: Fri May 19 19:31:42 2023, max compression
```

## Comparing `references_parser-1.1.2.tar` & `references_parser-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 04:17:01.795235 references_parser-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-19 04:16:39.000000 references_parser-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 04:16:39.000000 references_parser-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.791235 references_parser-1.1.2/references_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/converters/url_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/IeeeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/SsauParser.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 04:17:01.795235 references_parser-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-19 04:16:39.000000 references_parser-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.435807 references_parser-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 19:31:42.435807 references_parser-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-19 19:31:27.000000 references_parser-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 19:31:27.000000 references_parser-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.431807 references_parser-1.2.0/references_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.435807 references_parser-1.2.0/references_parser/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/converters/url_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.435807 references_parser-1.2.0/references_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/models/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/models/bibtex_ssau.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.435807 references_parser-1.2.0/references_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/parsers/ieee_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-19 19:31:27.000000 references_parser-1.2.0/references_parser/parsers/ssau_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:31:42.435807 references_parser-1.2.0/references_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 19:31:42.000000 references_parser-1.2.0/references_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:31:42.435807 references_parser-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 19:31:27.000000 references_parser-1.2.0/setup.py
```

### Comparing `references_parser-1.1.2/PKG-INFO` & `references_parser-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references_parser
-Version: 1.1.2
+Version: 1.2.0
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-1.1.2/README.md` & `references_parser-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `references_parser-1.1.2/references_parser/cli.py` & `references_parser-1.2.0/references_parser/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,103 @@
 import click
-from .converters.url_converter import convert_urls_to_bibtex
-from .parsers import SsauParser
-from .parsers import IEEEParser
 
+from .converters.url_converter import convert_urls_to_bibtex
+from .parsers import IEEEParser, SsauParser
 
 PARSER_MAPPING = {
-    'ssau': SsauParser(),
-    'ieee': IEEEParser(),
-
+    "ssau": SsauParser(),
+    "ieee": IEEEParser(),
+    # 'ieee': IEEEParser(),
 }
 
 
+def log_errors(errors):
+    if errors is not None and len(errors.keys()) > 0:
+        print("Some errors was occured during parsing:")
+        for bibtex_title, error in errors.items():
+            for k, v in error.items():
+                print(f"ERROR | {bibtex_title}: {k} - {v}")
+
+
 @click.group()
 def cli():
     pass
 
 
 @cli.command()
-@click.argument('path', type=str)
-@click.option('-s', '--save', type=str, help='Path to file where to save the result of parsing.', default='')
-@click.option('-p', '--parser', type=str, help='Parser to use. Available parsers: ieee, ssau. Default: ssau.', default='ssau')
-@click.option('-v', '--verbose', is_flag=True, help='Whether to print output to stdout or not', default=False)
-@click.option('-b', '--beautify', type=int, help='Number of line wraps between references. Default: 1', default=1)
+@click.argument("path", type=str)
+@click.option(
+    "-s",
+    "--save",
+    type=str,
+    help="Path to file where to save the result of parsing.",
+    default="",
+)
+@click.option(
+    "-p",
+    "--parser",
+    type=str,
+    help="Parser to use. Available parsers: ieee, ssau. Default: ssau.",
+    default="ssau",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="Whether to print output to stdout or not",
+    default=False,
+)
+@click.option(
+    "-b",
+    "--beautify",
+    type=int,
+    help="Number of line wraps between references. Default: 1",
+    default=1,
+)
 def parse(path: str, save: str, parser: str, verbose: bool, beautify: int):
-    with open(path, 'r', encoding='utf-8') as f:
+    with open(path, "r", encoding="utf-8") as f:
         citations = f.read()
 
     parser_type = parser.lower()
     parser = PARSER_MAPPING.get(parser_type)
     if parser is None:
-        raise ValueError(f"Unknown parser type. Expect one of {list(PARSER_MAPPING.keys())}, but received"
-                         f"{parser_type}")
+        raise ValueError(
+            "Unknown parser type. Expect one of " +
+            f"{list(PARSER_MAPPING.keys())}, but received"
+            f"{parser_type}"
+        )
+
+    result, errors = parser(citations)
 
-    result = parser(citations)
-    
     end = "".join(["\n" for _ in range(beautify)])
-    
+
     if verbose:
         for entry in result:
-            print(entry, end=end)
+            if entry is not None:
+                print(entry, end=end)
 
     if save:
-        with open(save, 'w', encoding='utf-8') as f:
+        with open(save, "w", encoding="utf-8") as f:
             for entry in result:
-                f.write(entry + end)
-        print(f'Saved result to {save}.')
+                if entry is not None:
+                    f.write(entry + end)
+        print(f"Saved result to {save}.")
+
+    log_errors(errors)
 
 
 @cli.command()
-@click.argument('path', type=str)
+@click.argument("path", type=str)
 def prepare_urls(path: str):
-    with open(path, 'r', encoding='utf-8') as f:
+    with open(path, "r", encoding="utf-8") as f:
         citations = f.read()
-        
-    citations = convert_urls_to_bibtex(citations)
-    
-    with open(path, 'w', encoding='utf-8') as f:
+
+    citations, errors = convert_urls_to_bibtex(citations)
+
+    with open(path, "w", encoding="utf-8") as f:
         f.write(citations)
-        
-        
-if __name__ == '__main__':
-    cli()  
+
+    log_errors(errors)
+
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `references_parser-1.1.2/references_parser/converters/url_converter.py` & `references_parser-1.2.0/references_parser/converters/url_converter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-import bibtexparser as p
-import requests
 import re
-from bs4 import BeautifulSoup
 from datetime import datetime
 
+import bibtexparser as p
+import requests
+from bs4 import BeautifulSoup
+from tqdm import tqdm
 
 bibtex_format = """@online{{{title_key},
     title={{{title}}},
     date={{{date}}},
     year={{{year}}},
     origin={{TODO: Author or place or corp here}},
     base={{TODO: Base resource title here}},
     url={{{url}}}
 }}"""
 
 
 def make_title_key(title):
-    return re.sub(r'[^0-9a-z]', '', title, flags=re.IGNORECASE)
+    return re.sub(r"[^0-9a-z]", "", title, flags=re.IGNORECASE)
 
 
 def convert_urls_to_bibtex(file_content: str):
-    today = datetime.now().strftime('%d.%m.%Y')
-    this_year = datetime.now().strftime('%Y')
-    
-    bibtex_dict = p.loads(file_content, p.bparser.BibTexParser(ignore_nonstandard_types=False))
-
-    for commentary in bibtex_dict.comments:
-        for url in commentary.split('\n'):
-            print(url)
-            if 'http' in url:
+    errors = {}
+
+    today = datetime.now().strftime("%d.%m.%Y")
+    this_year = datetime.now().strftime("%Y")
+
+    bibtex_dict = p.loads(
+        file_content, p.bparser.BibTexParser(ignore_nonstandard_types=False)
+    )
+    urls = (url for comment in bibtex_dict.comments for url in comment.split("\n"))
+
+    for url in tqdm(urls):
+        if "http" in url:
+            try:
                 r = requests.get(url)
-                soup = BeautifulSoup(r.content, 'html.parser')
-                title = soup.title.string
-                bibtex = bibtex_format.format(
-                    title_key=make_title_key(title),
-                    title=title,
-                    date=today,
-                    year=this_year,
-                    url=url
-                )
-                
-                file_content = file_content.replace(url, bibtex)
-    
-    return file_content            
+                print(r.status_code)
+                if r.status_code != 200:
+                    raise Exception("Cannot perform request")
+            except Exception:
+                errors[url] = {"Cannot get the page": "Try to enable VPN?"}
+                continue
+
+            soup = BeautifulSoup(r.content, "html.parser")
+            title = soup.title.string
+            bibtex = bibtex_format.format(
+                title_key=make_title_key(title),
+                title=title,
+                date=today,
+                year=this_year,
+                url=url,
+            )
+
+            file_content = file_content.replace(url, bibtex)
+
+    return file_content, errors
```

### Comparing `references_parser-1.1.2/references_parser/parsers/IeeeParser.py` & `references_parser-1.2.0/references_parser/parsers/ieee_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,85 @@
-from .SsauParser import SsauParser
+from typing import List, Optional
+from .ssau_parser import SsauParser
 
-SEP = ', '
+SEP = ", "
 
 
 class IEEEParser(SsauParser):
+    def __init__(self):
+        super().__init__()
+
     """
     Parses Bibtext into IEEE citation format.
     Official citation guideline:
     https://ieee-dataport.org/sites/default/files/analysis/27/IEEE%20Citation%20Guidelines.pdf
     """
+
     def parse_article(self, bibtex_entry: dict):
         """
         Parse bibtex annotated with @article
         """
-        authors = self._parse_authors(bibtex_entry['author'])
-        title = bibtex_entry['title']
-        year = bibtex_entry['year']
+        authors = self._parse_authors(bibtex_entry["author"])
+        title = bibtex_entry["title"]
+        year = bibtex_entry["year"]
 
-        journal = bibtex_entry['journal']
+        journal = bibtex_entry["journal"]
 
-        result = authors + SEP + "\"" + title + ",\" " + journal
+        result = authors + SEP + '"' + title + '," ' + journal
 
-        if 'arXiv' in journal:
+        if "arXiv" in journal:
             result += SEP + f"{year}."
             return result
 
-        number = "" if 'number' not in bibtex_entry else f"no. {bibtex_entry['number']}"
-        volume = "" if 'volume' not in bibtex_entry else f"vol. {bibtex_entry['volume']}"
+        number = "" if "number" not in bibtex_entry else f"no. {bibtex_entry['number']}"
+        volume = (
+            "" if "volume" not in bibtex_entry else f"vol. {bibtex_entry['volume']}"
+        )
         if len(volume) != 0:
             result += SEP + volume
             result += SEP + number
 
-        pages = bibtex_entry['pages'].split("--")
+        pages = bibtex_entry["pages"].split("--")
         if len(pages) == 1:
             result += SEP + f"p. {pages[0]}"
         elif len(pages) == 2:
             result += SEP + f"pp. {pages[0]}-{pages[1]}"
 
         result += SEP + f"{year}."
         return result
 
     def parse_proceedings(self, bibtex_entry: dict):
         """
         Parse bibtex annotated with @inproceedings
         """
-        authors = self._parse_authors(bibtex_entry['author'])
-        title = bibtex_entry['title']
-        booktitle = bibtex_entry['booktitle']
-        year = bibtex_entry['year']
-        pages = [] if 'pages' not in bibtex_entry else bibtex_entry['pages'].split("--")
+        authors = self._parse_authors(bibtex_entry["author"])
+        title = bibtex_entry["title"]
+        booktitle = bibtex_entry["booktitle"]
+        year = bibtex_entry["year"]
+        pages = [] if "pages" not in bibtex_entry else bibtex_entry["pages"].split("--")
 
-        result = authors + SEP + "\"" + title + ",\" In " + booktitle + SEP + year
+        result = authors + SEP + '"' + title + '," In ' + booktitle + SEP + year
         if len(pages) == 1:
             result += SEP + f"p. {pages[0]}"
         elif len(pages) == 2:
             result += SEP + f"pp. {pages[0]}-{pages[1]}"
 
         return result + "."
 
     def _parse_authors(self, authors):
         first_author, authors = super()._parse_authors(authors, return_all=True)
 
-        authors_list = authors.split(', ')
+        authors_list = authors.split(", ")
         if len(authors_list) == 1:
             return authors
         if len(authors_list) == 2:
-            return authors_list[0] + ' and ' + authors_list[1]
+            return authors_list[0] + " and " + authors_list[1]
         # Add `and` before the last author
-        authors_upd = ''
+        authors_upd = ""
         for author in authors_list[:-1]:
-            authors_upd += author + ', '
-        authors_upd += 'and ' + authors_list[-1]
+            authors_upd += author + ", "
+        authors_upd += "and " + authors_list[-1]
         return authors_upd
+
+    def __call__(self, bibtex: str):
+        raise Exception("Hasn't been tested yet")
+        return super().__call__(bibtex)
```

### Comparing `references_parser-1.1.2/references_parser/parsers/SsauParser.py` & `references_parser-1.2.0/references_parser/parsers/ssau_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,221 +1,172 @@
 from datetime import datetime
-from duckpy import Client
+from typing import List, Optional
 
 import bibtexparser as p
+from duckpy import Client
+from tqdm import tqdm
+
+from references_parser.models import Bibtex, BibtexSsau
 
 # Constant which stands for the following template: ". (long dash) " or ". -- "
 SEP_DASH = ". \u2012 "
 
 
 class SsauParser:
-    
     def __init__(self):
         self.search_client = Client()
-    
-    def parse_website(self, bibtex_entry: dict):
-        result = bibtex_entry["title"]
-        
-        base = bibtex_entry.get("base")
-        year = bibtex_entry["year"]
-        origin = bibtex_entry["origin"]
-        url = bibtex_entry["url"]
-        date = bibtex_entry["date"]
-        address = bibtex_entry.get("address")
-        
-        if base and len(base) > 0:
-            result += " // " + base
-        result += " / " + origin
-        if address is None:
-            result += SEP_DASH + "[Б.м.], " + year
+        self.errors = {}
+
+    def parse_website(self, bibtex: BibtexSsau):
+        result = bibtex.title
+
+        if bibtex.base is not None and len(bibtex.base) > 0:
+            result += " // " + bibtex.base
+        result += " / " + bibtex.origin
+        if bibtex.address is None:
+            result += SEP_DASH + "[Б.м.], " + bibtex.year
         else:
-            result += SEP_DASH + f"{address}, " + year
+            result += SEP_DASH + f"{bibtex.address}, " + bibtex.year
         result += SEP_DASH + "URL: "
-        result += url
-        result += f" (дата обращения: {date})"
+        result += bibtex.url
+        result += f" (дата обращения: {bibtex.date})."
         return result
-    
-    def parse_arxiv(self, bibtex_entry: dict):
+
+    def parse_arxiv(self, bibtex: BibtexSsau):
         """
         In case of reference on arxiv.org
         Le, Q. Distributed Representations of Sentences and Documents / Q. Le,
-        T. Mikolov // ArXiv / Cornell University. – 2014. – URL: https://arxiv.org/abs/1405.4053 (дата обращения: 03.11.2020)
+        T. Mikolov // ArXiv / Cornell University. – 2014.
+        – URL: https://arxiv.org/abs/1405.4053 (дата обращения: 03.11.2020)
         """
-        first_author, authors = self._parse_authors(bibtex_entry["author"])
-        title = bibtex_entry["title"]
-        year = bibtex_entry["year"]
-        
-        url = bibtex_entry.get("url")
-        today = datetime.now().strftime('%d.%m.%Y')
-        
-        if url is None:
-            results = self.search_client.search(f"arxiv {title}")
-            url = results[0]['url']
-            
+        first_author, authors = bibtex.get_parsed_authors()
+        today = datetime.now().strftime("%d.%m.%Y")
+
+        if bibtex.url is None:
+            try:
+                results = self.search_client.search(f"arxiv {bibtex.title}")
+                url = results[0]["url"]
+            except Exception as e:
+                self.errors[bibtex.title] = {"Error occured while searching": str(e)}
+                return None
+
         result = ""
         if first_author is not None:
             result += first_author + " "
-        
+
         return (
             result
-            + title
+            + bibtex.title
             + " / "
             + authors
             + " // ArXiv / Cornell University"
             + SEP_DASH
-            + year
+            + bibtex.year
             + SEP_DASH
-            + f"URL: {url} (дата обращения: {today})"
-            )
+            + f"URL: {url} (дата обращения: {today})."
+        )
 
-    def parse_article(self, bibtex_entry: dict):
+    def parse_article(self, bibtex: BibtexSsau):
         """
         Parse bibtex annotated with @article
         """
-        try:
-            journal = bibtex_entry["journal"]
-            if "arXiv" in journal:
-                raise Exception("Reference from ARXIV")
-        except:
-            return self.parse_arxiv(bibtex_entry)
-        
-        first_author, authors = self._parse_authors(bibtex_entry["author"])
-        title = bibtex_entry["title"]
-        year = bibtex_entry["year"]
-        
+        if bibtex.journal is not None and "arXiv" in bibtex.journal:
+            return self.parse_arxiv(bibtex)
+
+        first_author, authors = bibtex.get_parsed_authors()
+
         result = ""
         if first_author is not None:
             result += first_author + " "
 
         result = (
             result
-            + title
+            + bibtex.title
             + " / "
             + authors
             + " // "
-            + journal
+            + bibtex.journal
             + SEP_DASH
-            + year
+            + bibtex.year
         )
 
-        number = "" if "number" not in bibtex_entry else f"({bibtex_entry['number']})"
-        volume = (
-            ""
-            if "volume" not in bibtex_entry
-            else f"Vol. {bibtex_entry['volume']}{number}"
-        )
+        number = f"({bibtex.number})" if bibtex.number is not None else ""
+        volume = f"Vol. {bibtex.volume}{number}" if bibtex.volume is not None else ""
         if len(volume) != 0:
             result += SEP_DASH + volume
 
-        pages = [] if "pages" not in bibtex_entry else bibtex_entry["pages"].split("--")
+        pages = bibtex.pages_list
         if len(pages) == 0:
             pass
         elif len(pages) == 1:
             result += SEP_DASH + f"P. {pages[0]}"
         elif len(pages) == 2:
             result += SEP_DASH + f"P. {pages[0]}-{pages[1]}"
         return result + "."
 
-    def parse_proceedings(self, bibtex_entry: dict):
+    def parse_proceedings(self, bibtex: BibtexSsau):
         """
         Parse bibtex annotated with @inproceedings
         """
-        first_author, authors = self._parse_authors(bibtex_entry["author"])
-        title = bibtex_entry["title"]
-        booktitle = bibtex_entry["booktitle"]
-        year = bibtex_entry["year"]
-        pages = [] if "pages" not in bibtex_entry else bibtex_entry["pages"].split("--")
+        first_author, authors = bibtex.get_parsed_authors()
         org_year = (
-            year
-            if "organization" not in bibtex_entry
-            else f"{bibtex_entry['organization']}, {year}"
+            f"{bibtex.organization}, {bibtex.year}"
+            if bibtex.organization is not None
+            else bibtex.year
         )
-        
+
         result = ""
         if first_author is not None:
             result += first_author + " "
 
         result = (
             result
-            + title
+            + bibtex.title
             + " / "
             + authors
             + " // "
-            + booktitle
+            + bibtex.booktitle
             + SEP_DASH
             + org_year
         )
-        if len(pages) == 1:
+
+        number = f"({bibtex.number})" if bibtex.number is not None else ""
+        volume = f"Vol. {bibtex.volume}{number}" if bibtex.volume is not None else ""
+        if len(volume) != 0:
+            result += SEP_DASH + volume
+
+        pages = bibtex.pages_list
+        if len(pages) == 0:
+            pass
+        elif len(pages) == 1:
             result += SEP_DASH + f"P. {pages[0]}"
         elif len(pages) == 2:
             result += SEP_DASH + f"P. {pages[0]}-{pages[1]}"
-
         return result + "."
 
-    def _parse_authors(self, author_string, return_all=False):
-        """
-        1. Авторов < 4
-        Фамилия, инициалы первого автора. Основное заглавие : 
-        добавочное заглавие / Инициалы и фамилии первого, 
-        второго, третьего автора
-        2. Авторов == 4
-        Основное заглавие : добавочное заглавие / Инициалы и 
-        фамилии всех четырех авторов ;
-        3. Авторов > 4
-        Основное заглавие : добавочное заглавие / Инициалы и 
-        фамилии первых трех авторов [и др.]
-        """
-        def parse_single_author(str_author):
-            result = ""
-            splitted_author = p.customization.splitname(str_author)
-            for initial in splitted_author["first"]:
-                result += initial[0] + "."
-            return result + " " + "".join(splitted_author["last"]) + ", "
-
-        authors = ""
-        first_author = ""
-
-        first_author_unparsed = author_string[0]
-        splitted_first_author = p.customization.splitname(first_author_unparsed)
-        first_author += "".join(splitted_first_author["last"]) + ", "
-        for initial in splitted_first_author["first"]:
-            first_author += initial[0]
-        first_author += "."
-
-        if len(author_string) < 4 or return_all:
-            for str_author in author_string:
-                authors += parse_single_author(str_author)
-            authors = authors[:-2]
-        elif len(author_string) == 4:
-            for str_author in author_string:
-                authors += parse_single_author(str_author)
-            authors = authors[:-2]
-            first_author = None
-        else:
-            for str_author in author_string[:3]:
-                authors += parse_single_author(str_author)
-            authors = authors[:-2]
-            first_author = None
-            authors = f"{authors} [и др.]"
-        return first_author, authors
-
-    def __call__(self, bibtex: str):
+    def __call__(self, bibtex: str) -> List[Optional[str]]:
         if bibtex.endswith(".txt"):
             with open(bibtex, "r") as f:
-                bibtex_dict = p.load(f, p.bparser.BibTexParser(ignore_nonstandard_types=False))
+                bibtex_dict = p.load(
+                    f, p.bparser.BibTexParser(ignore_nonstandard_types=False)
+                )
         else:
-            bibtex_dict = p.loads(bibtex, p.bparser.BibTexParser(ignore_nonstandard_types=False))
+            bibtex_dict = p.loads(
+                bibtex, p.bparser.BibTexParser(ignore_nonstandard_types=False)
+            )
         result = []
-        for bibtex_entry in bibtex_dict.entries:
+        for bibtex_entry in tqdm(bibtex_dict.entries):
             # The following line will parse string with authors in list of authors
             bibtex_entry = p.customization.author(bibtex_entry)
             bibtex_entry = p.customization.convert_to_unicode(bibtex_entry)
-            bibtex_type = bibtex_entry["ENTRYTYPE"]
-            if bibtex_type == "article":
-                result.append(self.parse_article(bibtex_entry))
-            elif bibtex_type == "inproceedings":
-                result.append(self.parse_proceedings(bibtex_entry))
-            elif bibtex_type == "online":
-                result.append(self.parse_website(bibtex_entry))
+
+            bibtex_model = BibtexSsau(**bibtex_entry)
+
+            if bibtex_model.ENTRYTYPE == Bibtex.Types.Article:
+                result.append(self.parse_article(bibtex_model))
+            elif bibtex_model.ENTRYTYPE == Bibtex.Types.Proceedings:
+                result.append(self.parse_proceedings(bibtex_model))
+            elif bibtex_model.ENTRYTYPE == Bibtex.Types.Website:
+                result.append(self.parse_website(bibtex_model))
             else:
-                raise Exception(f"Unsupported bibtex type: {bibtex_entry['ENTRYTYPE']}")
-        return result
+                raise Exception(f"Unsupported bibtex type: {bibtex_model.ENTRYTYPE}")
+        return result, self.errors
```

### Comparing `references_parser-1.1.2/references_parser.egg-info/PKG-INFO` & `references_parser-1.2.0/references_parser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references-parser
-Version: 1.1.2
+Version: 1.2.0
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-1.1.2/references_parser.egg-info/SOURCES.txt` & `references_parser-1.2.0/references_parser.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,10 +8,13 @@
 references_parser.egg-info/SOURCES.txt
 references_parser.egg-info/dependency_links.txt
 references_parser.egg-info/entry_points.txt
 references_parser.egg-info/requires.txt
 references_parser.egg-info/top_level.txt
 references_parser/converters/__init__.py
 references_parser/converters/url_converter.py
-references_parser/parsers/IeeeParser.py
-references_parser/parsers/SsauParser.py
-references_parser/parsers/__init__.py
+references_parser/models/__init__.py
+references_parser/models/bibtex.py
+references_parser/models/bibtex_ssau.py
+references_parser/parsers/__init__.py
+references_parser/parsers/ieee_parser.py
+references_parser/parsers/ssau_parser.py
```

### Comparing `references_parser-1.1.2/setup.py` & `references_parser-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='references_parser',
     packages=setuptools.find_packages(),
-    version='1.1.2',
+    version='1.2.0',
     description="Tool for parsing bibtex in ssau's format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mukhin Artem',
     author_email='artemmukhinssau@gmail.com',
     url='https://github.com/Banayaki/ReferencesParser',
     include_package_data=True,
@@ -21,14 +21,16 @@
     ], 
     install_requires=[
         "beautifulsoup4==4.12.2",
         "bibtexparser==1.4.0",
         "click==8.1.3",
         "duckpy==3.2.0",
         "Requests==2.30.0",
+        "pydantic==1.10.2",
+        "tqdm==4.64.1"
     ],
     entry_points={
         'console_scripts': [
             'references_parser=references_parser.cli:main'
         ]
     }
 )
```

