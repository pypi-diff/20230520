# Comparing `tmp/channel2pdf-0.0.8.tar.gz` & `tmp/channel2pdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/channel2pdf-0.0.8.tar", last modified: Thu Mar 12 19:06:24 2020, max compression
+gzip compressed data, was "dist/channel2pdf-0.0.9.tar", last modified: Tue Mar 24 00:37:04 2020, max compression
```

## Comparing `channel2pdf-0.0.8.tar` & `channel2pdf-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      836 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      266 2020-01-18 14:57:46.000000 channel2pdf-0.0.8/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1622 2020-03-12 18:54:01.000000 channel2pdf-0.0.8/channel2pdf/__init__.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      746 2020-01-18 06:00:34.000000 channel2pdf-0.0.8/channel2pdf/article.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1461 2020-01-18 05:57:47.000000 channel2pdf-0.0.8/channel2pdf/find_resource.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1188 2020-02-29 14:16:47.000000 channel2pdf-0.0.8/channel2pdf/index.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      836 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      289 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       66 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       12 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/channel2pdf.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-03-12 19:06:24.000000 channel2pdf-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      797 2020-03-12 18:55:18.000000 channel2pdf-0.0.8/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-24 00:37:04.000000 channel2pdf-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      836 2020-03-24 00:37:04.000000 channel2pdf-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      266 2020-01-18 14:57:46.000000 channel2pdf-0.0.9/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-24 00:37:04.000000 channel2pdf-0.0.9/channel2pdf/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1622 2020-03-12 18:54:01.000000 channel2pdf-0.0.9/channel2pdf/__init__.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      746 2020-01-18 06:00:34.000000 channel2pdf-0.0.9/channel2pdf/article.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1502 2020-03-24 00:36:25.000000 channel2pdf-0.0.9/channel2pdf/find_resource.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1188 2020-02-29 14:16:47.000000 channel2pdf-0.0.9/channel2pdf/index.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-24 00:37:04.000000 channel2pdf-0.0.9/channel2pdf.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      836 2020-03-24 00:37:03.000000 channel2pdf-0.0.9/channel2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      289 2020-03-24 00:37:03.000000 channel2pdf-0.0.9/channel2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-03-24 00:37:03.000000 channel2pdf-0.0.9/channel2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       66 2020-03-24 00:37:03.000000 channel2pdf-0.0.9/channel2pdf.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       12 2020-03-24 00:37:03.000000 channel2pdf-0.0.9/channel2pdf.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-03-24 00:37:04.000000 channel2pdf-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      797 2020-03-24 00:30:04.000000 channel2pdf-0.0.9/setup.py
```

### Comparing `channel2pdf-0.0.8/PKG-INFO` & `channel2pdf-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channel2pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Export Telegram Channel to PDF
 Home-page: https://github.com/gaoyunzhi/channel2pdf
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # channel2pdf
```

### Comparing `channel2pdf-0.0.8/channel2pdf/__init__.py` & `channel2pdf-0.0.9/channel2pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `channel2pdf-0.0.8/channel2pdf/article.py` & `channel2pdf-0.0.9/channel2pdf/article.py`

 * *Files identical despite different names*

### Comparing `channel2pdf-0.0.8/channel2pdf/find_resource.py` & `channel2pdf-0.0.9/channel2pdf/find_resource.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,27 +22,26 @@
 	links = {}
 	for item in soup.find_all('a', class_='tgme_widget_message_link_preview'):
 		if 'telegra.ph' not in item['href']:
 			continue
 		title = item.find('div', class_='link_preview_title').text
 		links[item['href']] = title
 	pics = []
-	for item in soup.find_all('a', class_='tgme_widget_message_photo_wrap'):
-		text = item.parent.find('div', class_='tgme_widget_message_text')
-		src = findSrc(item['style'])
-		img = '<figure><img src="%s"/></figure>' % src
-		pics.append((img, text or ''))
+	for item in soup.find_all('div', class_='tgme_widget_message_bubble'):
+		imgs = []
+		for pic in item.find_all('a', class_='tgme_widget_message_photo_wrap'):
+			imgs.append('<figure><img src="%s"/></figure>' % findSrc(pic['style']))
+		text = item.find('div', class_='tgme_widget_message_text')
+		if imgs:
+			pics.append((''.join(imgs), text or ''))
 	texts = []
 	for item in soup.find_all('div', class_='tgme_widget_message_wrap'):
-		if 'telegra.ph' in item.text:
-			continue
 		if item.find('a', class_='tgme_widget_message_photo_wrap'):
 			continue
 		preview = item.find('a', class_='tgme_widget_message_link_preview')
-		if not preview:
-			continue
-		preview.name = 'div'
+		if preview:
+			preview.name = 'div'
 		text = item.find('div', class_='tgme_widget_message_text')
-		texts.append((text, preview))
+		texts.append((text, preview or ''))
 	return name, links, pics, texts
```

### Comparing `channel2pdf-0.0.8/channel2pdf/index.py` & `channel2pdf-0.0.9/channel2pdf/index.py`

 * *Files identical despite different names*

### Comparing `channel2pdf-0.0.8/channel2pdf.egg-info/PKG-INFO` & `channel2pdf-0.0.9/channel2pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channel2pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Export Telegram Channel to PDF
 Home-page: https://github.com/gaoyunzhi/channel2pdf
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # channel2pdf
```

### Comparing `channel2pdf-0.0.8/setup.py` & `channel2pdf-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="channel2pdf",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Export Telegram Channel to PDF",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/channel2pdf",
     packages=setuptools.find_packages(),
```

