# Comparing `tmp/mkdocs-toc-md-0.0.5.tar.gz` & `tmp/mkdocs-toc-md-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-toc-md-0.0.5.tar", last modified: Sat Apr  1 06:22:46 2023, max compression
+gzip compressed data, was "mkdocs-toc-md-0.0.6.tar", last modified: Sat May 20 11:55:37 2023, max compression
```

## Comparing `mkdocs-toc-md-0.0.5.tar` & `mkdocs-toc-md-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-01 06:22:46.759535 mkdocs-toc-md-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.5/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     3885 2023-04-01 06:22:46.755539 mkdocs-toc-md-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3287 2023-04-01 06:08:30.000000 mkdocs-toc-md-0.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-01 06:22:46.552213 mkdocs-toc-md-0.0.5/mkdocs_toc_md/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9367 2023-04-01 05:43:53.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md/plugin.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-01 06:22:46.726427 mkdocs-toc-md-0.0.5/mkdocs_toc_md/template/
--rwxrwxrwx   0 root         (0) root         (0)      382 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md/template/toc.md.j2
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-01 06:22:46.696431 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3885 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      345 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-01 06:22:46.000000 mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-01 06:22:46.760535 mkdocs-toc-md-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1300 2023-04-01 05:24:32.000000 mkdocs-toc-md-0.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.583474 mkdocs-toc-md-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     4353 2023-05-20 11:55:37.579475 mkdocs-toc-md-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3772 2023-05-20 11:30:58.000000 mkdocs-toc-md-0.0.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.365503 mkdocs-toc-md-0.0.6/mkdocs_toc_md/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11355 2023-05-20 10:34:12.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/plugin.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.552470 mkdocs-toc-md-0.0.6/mkdocs_toc_md/template/
+-rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-09 12:50:24.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/template/toc.md.j2
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.524472 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4353 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      345 2023-05-20 11:55:37.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-20 11:55:37.585476 mkdocs-toc-md-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1300 2023-05-20 10:34:12.000000 mkdocs-toc-md-0.0.6/setup.py
```

### Comparing `mkdocs-toc-md-0.0.5/LICENSE` & `mkdocs-toc-md-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-toc-md-0.0.5/PKG-INFO` & `mkdocs-toc-md-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-toc-md
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate a table of contents markdown file
 Home-page: https://github.com/try0/mkdocs-toc-md
 Author: Ryo Tsunoda
 Author-email: try0.development@gmail.com
 License: MIT
 Keywords: mkdocs plugin toc generator
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 
 ![](https://user-images.githubusercontent.com/17096601/199638378-892ddec9-b7af-4eb8-8ca8-a57c02980f53.png)
 
 
 
 ## Sample
 
-[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.md?plain=1)  
+[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.en.md?plain=1)  
 [Site](https://try0.github.io/mkdocs-toc-md/sample/site/)
 
 
 
 
 ## Usage
 
@@ -131,8 +131,25 @@
 Path of template dir.
 Put `toc.md.j2` in your custom template dir.
 
 ### beautiful_soup_parser: str
 Parser used in BeautifulSoup. Default is html.parser.  
 If using html5lib or lxml, you need to install additional dependencies.
 
+### integrate_mkdocs_static_i18n: bool
+With [mkdocs-static-i18n](https://github.com/ultrabug/mkdocs-static-i18n)
+
+### languages: dict
+Use with integrate_mkdocs_static_i18n option.
+Set toc_page_title, toc_page_description for each language.
+
+```yml
+languages:
+    en:
+        toc_page_title: Contents
+        toc_page_description: Usage mkdocs-toc-md
+    ja:
+        toc_page_title: 目次
+        toc_page_description: mkdocs-toc-mdプラグインの使い方
+```
+
```

### Comparing `mkdocs-toc-md-0.0.5/README.md` & `mkdocs-toc-md-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ![](https://user-images.githubusercontent.com/17096601/199638378-892ddec9-b7af-4eb8-8ca8-a57c02980f53.png)
 
 
 
 ## Sample
 
-[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.md?plain=1)  
+[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.en.md?plain=1)  
 [Site](https://try0.github.io/mkdocs-toc-md/sample/site/)
 
 
 
 
 ## Usage
 
@@ -109,7 +109,24 @@
 ### template_dir_path: str
 Path of template dir.
 Put `toc.md.j2` in your custom template dir.
 
 ### beautiful_soup_parser: str
 Parser used in BeautifulSoup. Default is html.parser.  
 If using html5lib or lxml, you need to install additional dependencies.
+
+### integrate_mkdocs_static_i18n: bool
+With [mkdocs-static-i18n](https://github.com/ultrabug/mkdocs-static-i18n)
+
+### languages: dict
+Use with integrate_mkdocs_static_i18n option.
+Set toc_page_title, toc_page_description for each language.
+
+```yml
+languages:
+    en:
+        toc_page_title: Contents
+        toc_page_description: Usage mkdocs-toc-md
+    ja:
+        toc_page_title: 目次
+        toc_page_description: mkdocs-toc-mdプラグインの使い方
+```
```

### Comparing `mkdocs-toc-md-0.0.5/mkdocs_toc_md/plugin.py` & `mkdocs-toc-md-0.0.6/mkdocs_toc_md/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import sys
 import logging
 import os
 import re
+from mkdocs import plugins
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from bs4 import BeautifulSoup
 from jinja2 import Environment, FileSystemLoader
+try:
+    from mkdocs.plugins import event_priority
+except ImportError:
+    event_priority = lambda priority: lambda f: f  # No-op fallback
 
 logging.getLogger(__name__)
 
 
 class TocPageData:
     """ Page params """
     toc_output_comment = None
@@ -79,14 +84,16 @@
         ('ignore_page_pattern', config_options.Type(str, default='')),
         ('remove_navigation_page_pattern', config_options.Type(str, default='')),
         ('toc_page_title', config_options.Type(str, default='Contents')),
         ('toc_page_description', config_options.Type(str, default=None)),
         ('header_level', config_options.Type(int, default=3)),
         ('template_dir_path', config_options.Type(str, default=None)),
         ('beautiful_soup_parser', config_options.Type(str, default='html.parser')),
+        ('languages', config_options.Type(dict, default=dict())),
+        ('integrate_mkdocs_static_i18n', config_options.Type(bool, default=False)),
     )
 
 
     def __init__(self):
         self.logger = logging.getLogger('mkdocs.toc-md')
         self.logger.setLevel(logging.INFO)
         
@@ -104,18 +111,22 @@
     def on_pre_build(self, config):
         self.logger.info("Enabled toc-md plugin")
 
 
     def on_nav(self, nav, config, files):
         # keep navigations
         self.nav = nav
+      
+        # mkdocs-static-i18n
+        self.i18n_plugin = None
+        if self.config['integrate_mkdocs_static_i18n'] and 'i18n' in config['plugins']:
+            self.i18n_plugin = config['plugins']['i18n']
 
 
     def on_post_page(self, output_content, page, config):
-        
         # remove navigation items
         pattern = self.config['remove_navigation_page_pattern']
         if pattern:
             remove_navigation_page_re = re.compile(pattern)
             if remove_navigation_page_re.match(page.file.src_path):
                 self.logger.info("toc-md: Remove toc")
 
@@ -123,39 +134,60 @@
                 for nav_elm in soup.find_all("nav", {"class": "md-nav md-nav--secondary"}):
                     nav_elm.decompose()
         
                 souped_html = soup.prettify(soup.original_encoding)
                 return souped_html 
 
         return output_content
-        
+    
 
+    @plugins.event_priority(-100) 
     def on_post_build(self, config):
 
         ignore_file_pattern = self.config['ignore_page_pattern']
-        ignore_re = None
+        self.ignore_re = None
         if ignore_file_pattern:
-            ignore_re = re.compile(ignore_file_pattern)
+            self.ignore_re = re.compile(ignore_file_pattern)
 
-        header_names = []
+        self.header_names = []
         for level in range(self.config['header_level']):
-            header_names.append('h' + str(level + 1))
+            self.header_names.append('h' + str(level + 1))
+
+        self.logger.info('toc-md: Lookup ' + ', '.join(self.header_names))
+
+
+        if self.i18n_plugin:
+            # mkdocs-static-i18n
+            # https://github.com/ultrabug/mkdocs-static-i18n
+
+            for lang in self.i18n_plugin.i18n_navs:
+                use_folder = 'folder' == self.i18n_plugin.config['docs_structure']
+                nav = self.i18n_plugin.i18n_navs[lang]
+                if use_folder:
+                    self.output(config, nav, "", lang)
+                else:
+                    self.output(config, nav, lang, "")
+
+        else:
+            # default
+
+            self.output(config, self.nav, "", "")
+
 
-        self.logger.info('toc-md: Lookup ' + ', '.join(header_names))
+    def output(self, config, nav, lang, folder):
 
         # Pickup headers
         toc_headers = []
-        for page in self.nav.pages:
-
+        for page in nav.pages:
             if 'output_path' in self.config:
                 output_path = self.config['output_path']
                 if page.file.src_path == output_path:
                     continue
 
-            ignore = ignore_re and ignore_re.match(page.file.src_path)
+            ignore = self.ignore_re and self.ignore_re.match(page.file.src_path)
             if ignore:
                 continue
 
             soup = BeautifulSoup(page.content, self.config['beautiful_soup_parser'])
 
             # extract page description
             toc_description = ''
@@ -171,15 +203,15 @@
                     if description_elm is not None:
                         toc_description += description_elm.text
 
             if 'toc_md_description' in page.meta:
                 toc_description += page.meta['toc_md_description']
 
             # create TocItem
-            article_headers = soup.find_all(header_names)
+            article_headers = soup.find_all(self.header_names)
             for h in article_headers:
 
                 toc_header = TocItem()
                 if h.find('a', attrs={'class', 'headerlink'}):
                      h.a.extract()
 
                 toc_header.text = h.text
@@ -198,33 +230,44 @@
                 elif h.name == 'h5' :
                     toc_header.src_level = 5
                 elif h.name == 'h6' :
                     toc_header.src_level = 6
 
                 toc_headers.append(toc_header)
 
+        # create template arg
+        template_param = TocPageData()
+        template_param.page_title = self.config['toc_page_title']
+        if lang in self.config['languages']:
+            if 'toc_page_title' in self.config['languages'][lang]:
+                template_param.page_title = self.config['languages'][lang]['toc_page_title']
+
+        template_param.page_description = self.config['toc_page_description']
+        if lang in self.config['languages']:
+            if 'toc_page_description' in self.config['languages'][lang]:
+                template_param.page_description = self.config['languages'][lang]['toc_page_description']
 
+        template_param.toc_headers = toc_headers
+        template_param.toc_output_comment = self.toc_output_comment
 
+        self.output_md_file(config, template_param, lang, folder)
+
+
+    def output_md_file(self, config, template_param, file_suffix, append_folder):
+        """ Outputs markdown file. """
+        
         base_path = os.path.abspath(os.path.dirname(__file__))
         template_path = [os.path.join(base_path, 'template')]
 
         # using custom template
         if 'template_dir_path' in self.config:
             if self.config['template_dir_path'] and os.path.exists(self.config['template_dir_path']):
                 template_path = self.config['template_dir_path']
                 self.logger.info("toc-md: Use custom template")
 
-
-        # create template arg
-        template_param = TocPageData()
-        template_param.page_title = self.config['toc_page_title']
-        template_param.page_description = self.config['toc_page_description']
-        template_param.toc_headers = toc_headers
-        template_param.toc_output_comment = self.toc_output_comment
-
         # render contents
         jinja_env = Environment(
             loader = FileSystemLoader(template_path),
             trim_blocks = True
         )
         template = jinja_env.get_template('toc.md.j2')
         toc_output = template.render(data = template_param)
@@ -233,16 +276,19 @@
         if 'output_log' in self.config:
             if self.config['output_log']:
                 print(toc_output)
 
         # save file
         if 'output_path' in self.config:
             output_path = self.config['output_path']
+            if file_suffix:
+                output_path = re.sub('md$', file_suffix + '.md', output_path)
+
             if output_path:
-                abs_md_path = os.path.join(config['docs_dir'], output_path)
+                abs_md_path = os.path.join(config['docs_dir'], append_folder, output_path)
                 os.makedirs(os.path.dirname(abs_md_path), exist_ok=True)
 
                  # avoid infinite loop
                 if os.path.isfile(abs_md_path):
                      with open(abs_md_path, 'r', encoding='utf-8') as file:
                         old_content = file.read()
                         if old_content == toc_output:
@@ -257,11 +303,7 @@
                     file.write(toc_output)
                 
                 self.logger.info(f'toc-md: Output a toc markdown file to "{abs_md_path}".')
 
                 if self.is_build_command:
                     self.logger.warning('toc-md: Command line contains [build]. You may need to build again to render toc md as html.')
 
-
-
-
-
```

### Comparing `mkdocs-toc-md-0.0.5/mkdocs_toc_md.egg-info/PKG-INFO` & `mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-toc-md
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate a table of contents markdown file
 Home-page: https://github.com/try0/mkdocs-toc-md
 Author: Ryo Tsunoda
 Author-email: try0.development@gmail.com
 License: MIT
 Keywords: mkdocs plugin toc generator
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 
 ![](https://user-images.githubusercontent.com/17096601/199638378-892ddec9-b7af-4eb8-8ca8-a57c02980f53.png)
 
 
 
 ## Sample
 
-[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.md?plain=1)  
+[File](https://github.com/try0/mkdocs-toc-md/blob/main/sample/docs/index.en.md?plain=1)  
 [Site](https://try0.github.io/mkdocs-toc-md/sample/site/)
 
 
 
 
 ## Usage
 
@@ -131,8 +131,25 @@
 Path of template dir.
 Put `toc.md.j2` in your custom template dir.
 
 ### beautiful_soup_parser: str
 Parser used in BeautifulSoup. Default is html.parser.  
 If using html5lib or lxml, you need to install additional dependencies.
 
+### integrate_mkdocs_static_i18n: bool
+With [mkdocs-static-i18n](https://github.com/ultrabug/mkdocs-static-i18n)
+
+### languages: dict
+Use with integrate_mkdocs_static_i18n option.
+Set toc_page_title, toc_page_description for each language.
+
+```yml
+languages:
+    en:
+        toc_page_title: Contents
+        toc_page_description: Usage mkdocs-toc-md
+    ja:
+        toc_page_title: 目次
+        toc_page_description: mkdocs-toc-mdプラグインの使い方
+```
+
```

### Comparing `mkdocs-toc-md-0.0.5/setup.py` & `mkdocs-toc-md-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # python setup.py develop
 # python setup.py sdist bdist_wheel
 # twine check dist/mkdocs-toc-md-x.x.x.tar.gz
 # twine upload --repository pypi dist/*
 setup(
     name='mkdocs-toc-md',
-    version='0.0.5',
+    version='0.0.6',
     description='Generate a table of contents markdown file',
     long_description=io.open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs plugin toc generator',
     author='Ryo Tsunoda',
     author_email='try0.development@gmail.com',
     url='https://github.com/try0/mkdocs-toc-md',
```

