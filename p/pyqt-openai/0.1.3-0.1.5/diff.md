# Comparing `tmp/pyqt-openai-0.1.3.tar.gz` & `tmp/pyqt-openai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.3.tar", last modified: Sun May  7 05:05:13 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.5.tar", last modified: Sat May 20 07:20:12 2023, max compression
```

## Comparing `pyqt-openai-0.1.3.tar` & `pyqt-openai-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.863436 pyqt-openai-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5704 2023-05-07 05:05:13.862442 pyqt-openai-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5301 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.658283 pyqt-openai-0.1.3/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.3/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0    10282 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/circleProfileImage.py
--rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/clickableTooltip.py
--rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/convListWidget.py
--rw-rw-rw-   0        0        0     7627 2023-05-07 04:26:44.000000 pyqt-openai-0.1.3/pyqt_openai/customizeDialog.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.733666 pyqt-openai-0.1.3/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.3/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.3/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/ico/customize.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/download.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.3/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.3/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.3/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/ico/user.svg
--rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/ico/vertical_three_dots.svg
--rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    22457 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.747629 pyqt-openai-0.1.3/pyqt_openai/prompt/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     3775 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/propPage.py
--rw-rw-rw-   0        0        0     4819 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/templatePage.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.793373 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0    21685 2023-05-07 04:26:44.000000 pyqt-openai-0.1.3/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/svgLabel.py
--rw-rw-rw-   0        0        0     5935 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/svgToolButton.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.813564 pyqt-openai-0.1.3/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0     4417 2023-05-07 03:48:58.000000 pyqt-openai-0.1.3/pyqt_openai/test/prompt_autocomplete.py
--rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.3/pyqt_openai/test/rightSideBarTab.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.859468 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/
--rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/__init__.py
--rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/delete_model.py
--rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/make_model.py
--rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/using_model.py
-drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.697797 pyqt-openai-0.1.3/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     5704 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1765 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 05:05:13.863436 pyqt-openai-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.941831 pyqt-openai-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6540 2023-05-20 07:20:12.940833 pyqt-openai-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6119 2023-05-20 05:47:50.000000 pyqt-openai-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.804201 pyqt-openai-0.1.5/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6737 2023-05-13 01:46:18.000000 pyqt-openai-0.1.5/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2316 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/aboutDialog.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0    13069 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.5/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     5078 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7574 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.861052 pyqt-openai-0.1.5/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.5/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.5/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.5/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.5/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.5/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0     1542 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/ico/discord.svg
+-rw-rw-rw-   0        0        0     1552 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/ico/github.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.5/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0      712 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/ico/history.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.5/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0      654 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/ico/save.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.5/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.5/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.5/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.5/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.5/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.5/pyqt_openai/ico/vertical_three_dots.svg
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.890969 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/currentImageView.py
+-rw-rw-rw-   0        0        0     1735 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/explorerWidget.py
+-rw-rw-rw-   0        0        0     3171 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageDallEPage.py
+-rw-rw-rw-   0        0        0     4869 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py
+-rw-rw-rw-   0        0        0     5090 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageListWidget.py
+-rw-rw-rw-   0        0        0    18549 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageSqlite.py
+-rw-rw-rw-   0        0        0    10698 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
+-rw-rw-rw-   0        0        0     3867 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/leftSideBar.py
+-rw-rw-rw-   0        0        0     1077 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/rightSideBar.py
+-rw-rw-rw-   0        0        0     4044 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/thumbnailView.py
+-rw-rw-rw-   0        0        0     2229 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/viewWidget.py
+-rw-rw-rw-   0        0        0     1444 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3764 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    10956 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1787 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.5/pyqt_openai/notifier.py
+-rw-rw-rw-   0        0        0    11189 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/openAiChatBotWidget.py
+-rw-rw-rw-   0        0        0     3048 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/openAiThread.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.899946 pyqt-openai-0.1.5/pyqt_openai/prompt/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/prompt/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/prompt/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     8984 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/prompt/propPage.py
+-rw-rw-rw-   0        0        0     4384 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/prompt/templatePage.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.912911 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    10982 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-07 22:16:16.000000 pyqt-openai-0.1.5/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.5/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0    30652 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5918 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.5/pyqt_openai/svgLabel.py
+-rw-rw-rw-   0        0        0     5935 2023-05-07 05:04:02.000000 pyqt-openai-0.1.5/pyqt_openai/svgToolButton.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.925876 pyqt-openai-0.1.5/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.5/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0     5573 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/test/prompt.py
+-rw-rw-rw-   0        0        0     4414 2023-05-13 01:46:18.000000 pyqt-openai-0.1.5/pyqt_openai/test/prompt_autocomplete.py
+-rw-rw-rw-   0        0        0      908 2023-05-13 01:46:18.000000 pyqt-openai-0.1.5/pyqt_openai/test/rightSideBarTab.py
+-rw-rw-rw-   0        0        0      761 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/pyqt_openai/test/sqlalchemy_example.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.928867 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/
+-rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.938840 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/
+-rw-rw-rw-   0        0        0        0 2023-05-07 08:08:35.000000 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/delete_model.py
+-rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/make_model.py
+-rw-rw-rw-   0        0        0      816 2023-05-11 12:24:04.000000 pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/using_model.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:20:12.817166 pyqt-openai-0.1.5/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     6540 2023-05-20 07:20:12.000000 pyqt-openai-0.1.5/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2619 2023-05-20 07:20:12.000000 pyqt-openai-0.1.5/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:20:12.000000 pyqt-openai-0.1.5/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-20 07:20:12.000000 pyqt-openai-0.1.5/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 07:20:12.000000 pyqt-openai-0.1.5/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 07:20:12.941831 pyqt-openai-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-05-20 05:39:27.000000 pyqt-openai-0.1.5/setup.py
```

### Comparing `pyqt-openai-0.1.3/LICENSE` & `pyqt-openai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/PKG-INFO` & `pyqt-openai-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.3
+Version: 0.1.5
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,113 +13,131 @@
 # pyqt-openai
 <p align="center">
   <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
 </p>
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
-This shows an example of using OpenAI with PyQt as a chatbot.
+This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
-Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
+Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
+
+<b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
+
+But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
 
 You can select the model at the right side bar.
 
 An internet connection is required.
 
-## Contact
-You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
-
-## Note
-Some of the features are still being tested.
-
-I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+## Table of Contents
+* [Feature](#feature)
+* [Requirements](#requirements)
+* [Preview & Usage](#preview-usage)
+* [How to Install](#how-to-install)
+* [Troubleshooting](#troubleshooting)
+* [Contact](#contact)
+* [Note](#note)
+* [See Also](#see-also)
 
 ## Feature
-* basically this is <b>desktop application version of ChatGPT</b>
+* basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable)
+* support prompt generator (manageable, autosaved in database)
+* support slash commands
 * support beginning and ending part of the prompt
-* support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
+* image generation (DALL-E, Stable Diffusion with DreamStudio API)
+* you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
+* pyperclip - to copy prompt template from prompt generator
+* stability_sdk - for Stable Diffusion
 
-## Preview
-This is using GPT-3.5 turbo model by default. 
-
-### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
-<b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
-
+## Preview & Usage
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
+#### Note: Some of these previews are not the latest.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
+<b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
+
+You can change screen between text chatbot and image generating tool screen.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
-### Conversation preview
-#### Preview Image
-![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
-#### Preview Video
+### Conversation
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
-#### Preview 1 (v0.1.22)
-https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
-#### Preview 2 (v0.1.3)
-https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
-
-So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
-
-## How to play
-1. git clone ~
-2. from the root directory, type "cd pyqt_openai"
-3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
+https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+
+You can use the additional prompt feature by "prompt menu" right next to input field.
+
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+
+### Image Generation
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
+
+## How to Install
+1. open command propmt of your OS.
+2. git clone ~
+3. from the root directory, type "cd pyqt_openai"
+4. pip install -r requirements.txt
+5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
-4. python main.py
+6. python main.py
 
-If installation doesn't work, check the troubleshooting below.
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
-you can shout a curse word and just download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
+download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
+Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
+
+## Contact
+You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
+
+## Note
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## TODO list
-* support Stable Diffusion
+* DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
```

#### html2text {}

```diff
@@ -1,64 +1,76 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.3 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.5 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
-shows an example of using OpenAI with PyQt as a chatbot. Even though this
-project has become too huge to be called an 'example'. The major advantage of
-this package is that you don't need to know other language aside from Python.
-If you want to study openai with Python-only good old desktop software, this is
-for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
-generation feature available since v0.0.16. You can see the detail in official
-OpenAI site. Currently this feature is very basic now. This is using sqlite as
-a database. You can select the model at the right side bar. An internet
-connection is required. ## Contact You can join pyqt-openai's Discord_Server to
-have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. I recommend to install sqlite management
-software. It's not necessary to run this app (obviously), but it's good
-practice to manage database about conversation history with AI and to know how
-this works. ## Feature * basically this is desktop application version of
-ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
-past conversation * conversation management * add & delete conversations * save
+shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
+Stable Diffusion as a image generation tool. Even though this project has
+become too huge to be called an 'example'. The major advantage of this package
+is that you don't need to know other language aside from Python. If you want to
+study openai with Python-only good old desktop software, this is for you. The
+OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
+functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
+feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
+used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
+stable-diffusion-webgui. But this is very lightweight and more accessible.
+don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
+database. You can select the model at the right side bar. An internet
+connection is required. ## Table of Contents * [Feature](#feature) *
+[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
+Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
+(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
+is desktop application version of ChatGPT with image generation tool. * text
+streaming (enable by default, you can disable it) * AI remembers past
+conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable) * support beginning and ending part of
-the prompt * support image generation with DALL-E * you can run this in
-background application * notification will pop up when response is generated *
-you can make window stack on top or control its transparency ## Requirements *
-qtpy - the package allowing you to write code that works with both PyQt and
-PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
-turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
-b45401f8bb7c.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
-4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
-user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
-7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+* support prompt generator (manageable, autosaved in database) * support slash
+commands * support beginning and ending part of the prompt * you can run this
+in background application * notification will pop up when response is generated
+* you can make window stack on top or control its transparency * image
+generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
+download the image if you want. just hover the mouse cursor over the image. ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
+prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
+Preview & Usage ### Overview #### Note: Some of these previews are not the
+latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
+inside the red box. see [How to install](#how-to-install) You can change screen
+between text chatbot and image generating tool screen. ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
+07655cab2061) ### Conversation https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
-55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
-(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
-99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
-idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
-from the root directory, type "cd pyqt_openai" 3. You should put your api key
-in the line edit. You can get it in official_site of openai. Sign up and log in
-before you get it. By the way, this is free trial, not permanently free. See
-this after you have logged in. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 4. python
-main.py If installation doesn't work, check the troubleshooting below. ##
+Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
+1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
+"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
+pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
+Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
+of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
+pip install -r requirements.txt 5. You should put your api key in the line
+edit. You can get it in official_site of openai. Sign up and log in before you
+get it. Be sure, this is a very important API key that belongs to you only, so
+you should remember it and keep it secure. 6. python main.py If installation
+doesn't work, you can contact me with bring up new issue in issue tab or check
+the troubleshooting below even it is only about very specific error. ##
 Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` you can shout a curse word and just download
-the package itself from pypi. Unzip it, access the package directory, type ```
-python setup.py install ``` That will install the openai. ## TODO list *
-support Stable Diffusion * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+subprocess-exited-with-error ``` download the package itself from pypi. Unzip
+it, access the package directory, type ``` python setup.py install ``` That
+will install the openai. Note: I don't know this can happen in newer version of
+openai as well, so tell me if you know about something ## Contact You can join
+pyqt-openai's Discord_Server to have a conversation about it or AI-related
+stuff ð ## Note I recommend to install sqlite management software. It's not
+necessary to run this app (obviously), but it's good practice to manage
+database about conversation history with AI and to know how this works. ## TODO
+list * DB for images (to further experiement of both DALL-E and Stable
+Diffusion or other image generation engine) * show the explanation of every
+model and terms related to AI (e.g. temperature, topp..) * save conversation
+history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
+(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
+* show reason when the chat input is disabled for some reasons * add the basic
+example sources of making deep learning model with PyTorch (eventually) ## See
+Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
+from it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.3/README.md` & `pyqt-openai-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,113 +1,131 @@
 # pyqt-openai
 <p align="center">
   <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
 </p>
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
-This shows an example of using OpenAI with PyQt as a chatbot.
+This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
-Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
+Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
+
+<b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
+
+But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
 
 You can select the model at the right side bar.
 
 An internet connection is required.
 
-## Contact
-You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
-
-## Note
-Some of the features are still being tested.
-
-I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+## Table of Contents
+* [Feature](#feature)
+* [Requirements](#requirements)
+* [Preview & Usage](#preview-usage)
+* [How to Install](#how-to-install)
+* [Troubleshooting](#troubleshooting)
+* [Contact](#contact)
+* [Note](#note)
+* [See Also](#see-also)
 
 ## Feature
-* basically this is <b>desktop application version of ChatGPT</b>
+* basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable)
+* support prompt generator (manageable, autosaved in database)
+* support slash commands
 * support beginning and ending part of the prompt
-* support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
+* image generation (DALL-E, Stable Diffusion with DreamStudio API)
+* you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
+* pyperclip - to copy prompt template from prompt generator
+* stability_sdk - for Stable Diffusion
 
-## Preview
-This is using GPT-3.5 turbo model by default. 
-
-### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
-<b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
-
+## Preview & Usage
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
+#### Note: Some of these previews are not the latest.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
+<b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
+
+You can change screen between text chatbot and image generating tool screen.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
-### Conversation preview
-#### Preview Image
-![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
-#### Preview Video
+### Conversation
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
-#### Preview 1 (v0.1.22)
-https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
-#### Preview 2 (v0.1.3)
-https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
-
-So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
-
-## How to play
-1. git clone ~
-2. from the root directory, type "cd pyqt_openai"
-3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
+https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+
+You can use the additional prompt feature by "prompt menu" right next to input field.
+
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+
+### Image Generation
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
+
+## How to Install
+1. open command propmt of your OS.
+2. git clone ~
+3. from the root directory, type "cd pyqt_openai"
+4. pip install -r requirements.txt
+5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
-4. python main.py
+6. python main.py
 
-If installation doesn't work, check the troubleshooting below.
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
-you can shout a curse word and just download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
+download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
+Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
+
+## Contact
+You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
+
+## Note
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## TODO list
-* support Stable Diffusion
+* DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
```

#### html2text {}

```diff
@@ -1,61 +1,73 @@
 # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
-shows an example of using OpenAI with PyQt as a chatbot. Even though this
-project has become too huge to be called an 'example'. The major advantage of
-this package is that you don't need to know other language aside from Python.
-If you want to study openai with Python-only good old desktop software, this is
-for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
-generation feature available since v0.0.16. You can see the detail in official
-OpenAI site. Currently this feature is very basic now. This is using sqlite as
-a database. You can select the model at the right side bar. An internet
-connection is required. ## Contact You can join pyqt-openai's Discord_Server to
-have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. I recommend to install sqlite management
-software. It's not necessary to run this app (obviously), but it's good
-practice to manage database about conversation history with AI and to know how
-this works. ## Feature * basically this is desktop application version of
-ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
-past conversation * conversation management * add & delete conversations * save
+shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
+Stable Diffusion as a image generation tool. Even though this project has
+become too huge to be called an 'example'. The major advantage of this package
+is that you don't need to know other language aside from Python. If you want to
+study openai with Python-only good old desktop software, this is for you. The
+OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
+functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
+feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
+used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
+stable-diffusion-webgui. But this is very lightweight and more accessible.
+don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
+database. You can select the model at the right side bar. An internet
+connection is required. ## Table of Contents * [Feature](#feature) *
+[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
+Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
+(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
+is desktop application version of ChatGPT with image generation tool. * text
+streaming (enable by default, you can disable it) * AI remembers past
+conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable) * support beginning and ending part of
-the prompt * support image generation with DALL-E * you can run this in
-background application * notification will pop up when response is generated *
-you can make window stack on top or control its transparency ## Requirements *
-qtpy - the package allowing you to write code that works with both PyQt and
-PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
-turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
-b45401f8bb7c.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
-4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
-user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
-7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+* support prompt generator (manageable, autosaved in database) * support slash
+commands * support beginning and ending part of the prompt * you can run this
+in background application * notification will pop up when response is generated
+* you can make window stack on top or control its transparency * image
+generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
+download the image if you want. just hover the mouse cursor over the image. ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
+prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
+Preview & Usage ### Overview #### Note: Some of these previews are not the
+latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
+inside the red box. see [How to install](#how-to-install) You can change screen
+between text chatbot and image generating tool screen. ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
+07655cab2061) ### Conversation https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
-55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
-(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
-99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
-idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
-from the root directory, type "cd pyqt_openai" 3. You should put your api key
-in the line edit. You can get it in official_site of openai. Sign up and log in
-before you get it. By the way, this is free trial, not permanently free. See
-this after you have logged in. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 4. python
-main.py If installation doesn't work, check the troubleshooting below. ##
+Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
+1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
+"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
+pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
+Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
+of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
+pip install -r requirements.txt 5. You should put your api key in the line
+edit. You can get it in official_site of openai. Sign up and log in before you
+get it. Be sure, this is a very important API key that belongs to you only, so
+you should remember it and keep it secure. 6. python main.py If installation
+doesn't work, you can contact me with bring up new issue in issue tab or check
+the troubleshooting below even it is only about very specific error. ##
 Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` you can shout a curse word and just download
-the package itself from pypi. Unzip it, access the package directory, type ```
-python setup.py install ``` That will install the openai. ## TODO list *
-support Stable Diffusion * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+subprocess-exited-with-error ``` download the package itself from pypi. Unzip
+it, access the package directory, type ``` python setup.py install ``` That
+will install the openai. Note: I don't know this can happen in newer version of
+openai as well, so tell me if you know about something ## Contact You can join
+pyqt-openai's Discord_Server to have a conversation about it or AI-related
+stuff ð ## Note I recommend to install sqlite management software. It's not
+necessary to run this app (obviously), but it's good practice to manage
+database about conversation history with AI and to know how this works. ## TODO
+list * DB for images (to further experiement of both DALL-E and Stable
+Diffusion or other image generation engine) * show the explanation of every
+model and terms related to AI (e.g. temperature, topp..) * save conversation
+history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
+(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
+* show reason when the chat input is disabled for some reasons * add the basic
+example sources of making deep learning model with PyTorch (eventually) ## See
+Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
+from it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/a.py` & `pyqt-openai-0.1.5/pyqt_openai/a.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from PyQt5.QtWidgets import QLabel, QApplication, QWidget, QVBoxLayout
+from qtpy.QtWidgets import QLabel, QApplication, QWidget, QVBoxLayout
 
 
 def create_hyperlink_label(text, link):
     label = QLabel()
     label.setText(
         '''
         <html>
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/apiData.py` & `pyqt-openai-0.1.5/pyqt_openai/apiData.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.5/pyqt_openai/prompt/propPage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,314 +1,259 @@
-import json
-import os
+from qtpy.QtCore import Signal, Qt
+from qtpy.QtWidgets import QTableWidget, QSizePolicy, QPushButton, QSpacerItem, QStackedWidget, QLabel, \
+    QAbstractItemView, QTableWidgetItem, QHeaderView, QHBoxLayout, \
+    QVBoxLayout, QWidget, QDialog, QListWidget, QListWidgetItem, QApplication, QSplitter
+
+from pyqt_openai.inputDialog import InputDialog
+from pyqt_openai.sqlite import SqliteDatabase
+from pyqt_openai.svgButton import SvgButton
+
+
+class PropGroupList(QWidget):
+    added = Signal(int)
+    deleted = Signal(int)
+    currentRowChanged = Signal(int)
 
-import requests
-
-from qtpy.QtCore import Qt, Signal
-from qtpy.QtGui import QPixmap, QFont
-from qtpy.QtWidgets import QScrollArea, QVBoxLayout, QToolButton, QMenu, QAction, QWidget, QLabel, QHBoxLayout, QTextEdit, QStackedWidget
-
-from pyqt_openai.svgToolButton import SvgToolButton
-
-
-class ChatBrowser(QScrollArea):
-    convUnitUpdated = Signal(int, int, str)
-
-    def __init__(self):
+    def __init__(self, db: SqliteDatabase):
         super().__init__()
-        self.__initVal()
+        self.__initVal(db)
         self.__initUi()
 
-    def __initVal(self):
-        self.__cur_id = 0
+    def __initVal(self, db):
+        self.__db = db
 
     def __initUi(self):
-        self.__homeWidget = QLabel('Home')
-        self.__homeWidget.setAlignment(Qt.AlignCenter)
-        self.__homeWidget.setFont(QFont('Arial', 32))
+        self.__addBtn = SvgButton()
+        self.__delBtn = SvgButton()
 
-        lay = QVBoxLayout()
-        lay.setAlignment(Qt.AlignTop)
-        lay.setSpacing(0)
+        self.__addBtn.setIcon('ico/add.svg')
+        self.__delBtn.setIcon('ico/delete.svg')
+
+        self.__addBtn.clicked.connect(self.__addGroup)
+        self.__delBtn.clicked.connect(self.__deleteGroup)
+
+        lay = QHBoxLayout()
+        lay.addWidget(QLabel('Property Group'))
+        lay.addSpacerItem(QSpacerItem(10, 10, QSizePolicy.MinimumExpanding))
+        lay.addWidget(self.__addBtn)
+        lay.addWidget(self.__delBtn)
+        lay.setAlignment(Qt.AlignRight)
         lay.setContentsMargins(0, 0, 0, 0)
 
-        self.__chatWidget = QWidget()
-        self.__chatWidget.setLayout(lay)
+        topWidget = QWidget()
+        topWidget.setLayout(lay)
 
-        widget = QStackedWidget()
-        widget.addWidget(self.__homeWidget)
-        widget.addWidget(self.__chatWidget)
-        self.setWidget(widget)
-        self.setWidgetResizable(True)
-
-    def getChatWidget(self):
-        return self.__chatWidget
-
-    def showLabel(self, text, user_f, stream_f, image_f):
-        if image_f:
-            self.showImage(text, user_f)
-        else:
-            self.showText(text, stream_f, user_f)
-        if not stream_f:
-            # change user_f type from bool to int to insert in db
-            self.convUnitUpdated.emit(self.__cur_id, int(user_f), text)
-
-    def streamFinished(self):
-        self.convUnitUpdated.emit(self.__cur_id, 0, self.getLastResponse())
-
-    def showImage(self, image_url, user_f):
-        chatLbl = QLabel()
-        response = requests.get(image_url)
-        pixmap = QPixmap()
-        pixmap.loadFromData(response.content)
-        pixmap = pixmap.scaled(chatLbl.width(), chatLbl.height())
-        chatLbl.setPixmap(pixmap)
-        chatLbl.setStyleSheet('QLabel { background-color: #DDD; padding: 1em }')
-        self.getChatWidget().layout().addWidget(chatLbl)
-
-    def showText(self, text, stream_f, user_f):
-        if self.widget().currentWidget() == self.__chatWidget:
-            pass
-        else:
-            self.widget().setCurrentIndex(1)
-        self.__setLabel(text, stream_f, user_f)
-
-    def __setLabel(self, text, stream_f, user_f):
-        chatLbl = QLabel(text)
-        chatLbl.setWordWrap(True)
-        chatLbl.setTextInteractionFlags(Qt.TextSelectableByMouse)
-        if user_f:
-            chatLbl.setStyleSheet('QLabel { padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignRight)
-        else:
-            if stream_f:
-                lbl = self.getChatWidget().layout().itemAt(self.getChatWidget().layout().count()-1).widget()
-                if isinstance(lbl, QLabel) and lbl.alignment() == Qt.AlignLeft:
-                    lbl.setText(lbl.text()+text)
-                    return
-            chatLbl.setStyleSheet('QLabel { background-color: #DDD; padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignLeft)
-            chatLbl.setOpenExternalLinks(True)
-        self.getChatWidget().layout().addWidget(chatLbl)
-
-    def event(self, e):
-        if e.type() == 43:
-            self.verticalScrollBar().setSliderPosition(self.verticalScrollBar().maximum())
-        return super().event(e)
-
-    # TODO distinguish the image response
-    def getAllText(self):
-        all_text_lst = []
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()):
-                if lay.itemAt(i) and lay.itemAt(i).widget():
-                    widget = lay.itemAt(i).widget()
-                    if isinstance(widget, QLabel):
-                        all_text_lst.append(widget.text())
-
-        return '\n'.join(all_text_lst)
-
-    def getLastResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            i = lay.count()-1
-            if lay.itemAt(i) and lay.itemAt(i).widget():
-                widget = lay.itemAt(i).widget()
-                if isinstance(widget, QLabel):
-                    return widget.text()
-        return ''
-
-    def getEveryResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            text_lst = []
-            for i in range(lay.count()):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    widget = item.widget()
-                    if isinstance(widget, QLabel) and i % 2 == 1:
-                        text_lst.append(widget.text())
-            return '\n'.join(text_lst)
-        else:
-            return ''
-
-    def clear(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()-1, -1, -1):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    lay.removeWidget(item.widget())
-        self.widget().setCurrentIndex(0)
-
-    def isNew(self):
-        return self.widget().currentIndex() == 0
-
-    def setCurId(self, id):
-        self.__cur_id = id
-
-    def resetChatWidget(self, id):
-        self.clear()
-        self.setCurId(id)
-
-    def replaceConv(self, id, conv_data):
-        self.clear()
-        self.setCurId(id)
-        self.widget().setCurrentIndex(1)
-        for i in range(len(conv_data)):
-            self.__setLabel(conv_data[i], False, not bool(i % 2))
+        defaultPropPromptGroupArr = self.__db.selectPropPromptGroup()
 
+        self.__propList = QListWidget()
 
-class TextEditPrompt(QTextEdit):
-    returnPressed = Signal()
+        # TODO abcd
+        for group in defaultPropPromptGroupArr:
+            id = group[0]
+            name = group[1]
+            self.__addGroupItem(id, name)
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.__initUi()
+        self.__propList.currentRowChanged.connect(self.currentRowChanged)
 
-    def __initUi(self):
-        self.setStyleSheet('QTextEdit { border: 1px solid #AAA; } ')
+        lay = QVBoxLayout()
+        lay.addWidget(topWidget)
+        lay.addWidget(self.__propList)
+        lay.setContentsMargins(0, 0, 5, 0)
 
-    def keyPressEvent(self, e):
-        if e.key() == Qt.Key_Return or e.key() == Qt.Key_Enter:
-            if e.modifiers() == Qt.ShiftModifier:
-                return super().keyPressEvent(e)
-            else:
-                self.returnPressed.emit()
-        else:
-            return super().keyPressEvent(e)
+        self.setLayout(lay)
 
+        self.__propList.setCurrentRow(0)
 
-class TextEditPropmtGroup(QWidget):
-    textChanged = Signal()
+    def __addGroupItem(self, id, name):
+        item = QListWidgetItem()
+        item.setData(Qt.UserRole, id)
+        item.setText(name)
+        self.__propList.addItem(item)
+        self.__propList.setCurrentItem(item)
+        self.added.emit(id)
+
+    def __addGroup(self):
+        dialog = InputDialog('Add', '', self)
+        reply = dialog.exec()
+        if reply == QDialog.Accepted:
+            name = dialog.getText()
+            id = self.__db.insertPropPromptGroup(name)
+            self.__addGroupItem(id, name)
+
+    def __deleteGroup(self):
+        i = self.__propList.currentRow()
+        item = self.__propList.takeItem(i)
+        id = item.data(Qt.UserRole)
+        self.__db.deletePropPromptGroup(id)
+        self.deleted.emit(i)
+
+
+class PropTable(QWidget):
+    """
+    benchmarked https://gptforwork.com/tools/prompt-generator
+    """
+    updated = Signal(str)
 
-    def __init__(self):
+    def __init__(self, db: SqliteDatabase, id):
         super().__init__()
+        self.__initVal(db, id)
         self.__initUi()
 
+    def __initVal(self, db, id):
+        self.__db = db
+        self.__id = id
+
+        self.__title = self.__db.selectPropPromptGroupId(self.__id)[1]
+        self.__previousPromptPropArr = self.__db.selectPropPromptAttribute(self.__id)
+
     def __initUi(self):
-        self.__beginningTextEdit = TextEditPrompt()
-        self.__beginningTextEdit.textChanged.connect(self.textChanged)
-        self.__beginningTextEdit.setPlaceholderText('Beginning')
-
-        self.__textEdit = TextEditPrompt()
-        self.__textEdit.textChanged.connect(self.textChanged)
-        self.__textEdit.setPlaceholderText('Write some text...')
-
-        self.__endingTextEdit = TextEditPrompt()
-        self.__endingTextEdit.textChanged.connect(self.textChanged)
-        self.__endingTextEdit.setPlaceholderText('Ending')
+        self.__addBtn = SvgButton()
+        self.__delBtn = SvgButton()
 
-        self.__beginningTextEdit.setVisible(False)
-        self.__endingTextEdit.setVisible(False)
+        self.__addBtn.setIcon('ico/add.svg')
+        self.__delBtn.setIcon('ico/delete.svg')
 
-        self.__textGroup = [self.__beginningTextEdit, self.__textEdit, self.__endingTextEdit]
+        self.__addBtn.clicked.connect(self.__add)
+        self.__delBtn.clicked.connect(self.__delete)
 
-        lay = QVBoxLayout()
-        for w in self.__textGroup:
-            lay.addWidget(w)
+        lay = QHBoxLayout()
+        lay.addWidget(QLabel(self.__title))
+        lay.addSpacerItem(QSpacerItem(10, 10, QSizePolicy.MinimumExpanding))
+        lay.addWidget(self.__addBtn)
+        lay.addWidget(self.__delBtn)
+        lay.setAlignment(Qt.AlignRight)
         lay.setContentsMargins(0, 0, 0, 0)
-        lay.setSpacing(0)
-
-        self.setLayout(lay)
 
-    def adjustHeight(self) -> int:
-        """
-        adjust overall height of text edit group based on their contents and return adjusted height
-        :return:
-        """
-        groupHeight = 0
-        for w in self.__textGroup:
-            document = w.document()
-            height = document.size().height()
-            overallHeight = int(height+document.documentMargin())
-            w.setMaximumHeight(overallHeight)
-            groupHeight += overallHeight
-        return groupHeight
-
-    def getGroup(self):
-        return self.__textGroup
-
-    def getContent(self):
-        b = self.__textGroup[0].toPlainText().strip()
-        m = self.__textGroup[1].toPlainText().strip()
-        e = self.__textGroup[2].toPlainText().strip()
-
-        content = ''
-        if b:
-            content = b + '\n'
-        content += m
-        if e:
-            content += '\n' + e
+        topWidget = QWidget()
+        topWidget.setLayout(lay)
 
-        return content
+        self.__table = QTableWidget()
+        self.__table.setColumnCount(2)
+        self.__table.setRowCount(len(self.__previousPromptPropArr))
+        self.__table.horizontalHeader().setSectionResizeMode(1, QHeaderView.Stretch)
+        self.__table.setSelectionBehavior(QAbstractItemView.SelectRows)
+        self.__table.setHorizontalHeaderLabels(['Name', 'Value'])
+
+        for i in range(len(self.__previousPromptPropArr)):
+            name = self.__previousPromptPropArr[i][2]
+            value = self.__previousPromptPropArr[i][3]
+
+            item1 = QTableWidgetItem(name)
+            item1.setData(Qt.UserRole, self.__previousPromptPropArr[i][0])
+            item1.setTextAlignment(Qt.AlignCenter)
 
-class Prompt(QWidget):
-    def __init__(self):
-        super().__init__()
-        self.__initUi()
+            item2 = QTableWidgetItem(value)
+            item2.setTextAlignment(Qt.AlignCenter)
 
-    def __initUi(self):
-        self.__textEditGroup = TextEditPropmtGroup()
-        self.__textEditGroup.textChanged.connect(self.updateHeight)
+            self.__table.setItem(i, 0, item1)
+            self.__table.setItem(i, 1, item2)
 
-        settingsBtn = SvgToolButton()
-        settingsBtn.setIcon('ico/vertical_three_dots.svg')
-        settingsBtn.setToolTip('Prompt Settings')
-
-        # Create the menu
-        menu = QMenu(self)
-
-        # Create the actions
-        beginningAction = QAction("Show Beginning", self)
-        beginningAction.setShortcut('Ctrl+B')
-        beginningAction.setCheckable(True)
-        beginningAction.toggled.connect(self.__showBeginning)
-
-        endingAction = QAction("Show Ending", self)
-        endingAction.setShortcut('Ctrl+E')
-        endingAction.setCheckable(True)
-        endingAction.toggled.connect(self.__showEnding)
-
-        # Add the actions to the menu
-        menu.addAction(beginningAction)
-        menu.addAction(endingAction)
-
-        # Connect the button to the menu
-        settingsBtn.setMenu(menu)
-        settingsBtn.setPopupMode(QToolButton.InstantPopup)
+        self.__table.itemChanged.connect(self.__generatePropPrompt)
+        self.__table.itemChanged.connect(self.__saveChangedPropPrompt)
 
         lay = QVBoxLayout()
-        lay.addWidget(settingsBtn)
-        lay.setContentsMargins(1, 1, 1, 1)
-        lay.setAlignment(Qt.AlignBottom)
+        lay.addWidget(topWidget)
+        lay.addWidget(self.__table)
+        lay.setContentsMargins(5, 0, 0, 0)
 
-        rightWidget = QWidget()
-        rightWidget.setLayout(lay)
-
-        lay = QHBoxLayout()
-        lay.addWidget(self.__textEditGroup)
-        lay.addWidget(rightWidget)
-        lay.setContentsMargins(0, 0, 0, 0)
-        lay.setSpacing(0)
         self.setLayout(lay)
-        self.updateHeight()
 
-    def updateHeight(self):
-        overallHeight = self.__textEditGroup.adjustHeight()
-        self.setMaximumHeight(overallHeight)
+    def getPromptText(self):
+        prompt_text = ''
+        for i in range(self.__table.rowCount()):
+            name = self.__table.item(i, 0).text() if self.__table.item(i, 0) else ''
+            value = self.__table.item(i, 1).text() if self.__table.item(i, 1) else ''
+            if value.strip():
+                prompt_text += f'{name}: {value}\n'
+        return prompt_text
+
+    def __generatePropPrompt(self, item: QTableWidgetItem):
+        prompt_text = self.getPromptText()
+        self.updated.emit(prompt_text)
+
+    def __saveChangedPropPrompt(self, item: QTableWidgetItem):
+        name = self.__table.item(item.row(), 0)
+        id = name.data(Qt.UserRole)
+        name = name.text()
+        value = self.__table.item(item.row(), 1).text()
+        self.__db.updatePropPromptAttribute(self.__id, id, name, value)
+
+    def __add(self):
+        dialog = InputDialog('Name', '', self)
+        reply = dialog.exec()
+        if reply == QDialog.Accepted:
+            self.__table.itemChanged.disconnect(self.__saveChangedPropPrompt)
+
+            name = dialog.getText()
+            self.__table.setRowCount(self.__table.rowCount()+1)
+
+            item1 = QTableWidgetItem(name)
+            item1.setTextAlignment(Qt.AlignCenter)
+            self.__table.setItem(self.__table.rowCount()-1, 0, item1)
+
+            item2 = QTableWidgetItem('')
+            item2.setTextAlignment(Qt.AlignCenter)
+            self.__table.setItem(self.__table.rowCount()-1, 1, item2)
+
+            id = self.__db.insertPropPromptAttribute(self.__id, name)
+            item1.setData(Qt.UserRole, id)
+
+            self.__table.itemChanged.connect(self.__saveChangedPropPrompt)
+
+    def __delete(self):
+        for i in sorted(set([i.row() for i in self.__table.selectedIndexes()]), reverse=True):
+            id = self.__table.item(i, 0).data(Qt.UserRole)
+            self.__table.removeRow(i)
+            self.__db.deletePropPromptAttribute(self.__id, id)
 
-    def getTextEdit(self):
-        return self.__textEditGroup.getGroup()[1]
 
-    def getContent(self):
-        return self.__textEditGroup.getContent()
+class PropPage(QWidget):
+    updated = Signal(str)
 
-    def __showBeginning(self, f):
-        self.__textEditGroup.getGroup()[0].setVisible(f)
+    def __init__(self, db: SqliteDatabase):
+        super().__init__()
+        self.__initVal(db)
+        self.__initUi()
 
-    def __showEnding(self, f):
-        self.__textEditGroup.getGroup()[-1].setVisible(f)
+    def __initVal(self, db):
+        self.__db = db
+        self.__previousPropGroups = self.__db.selectPropPromptGroup()
 
+    def __initUi(self):
+        leftWidget = PropGroupList(self.__db)
+        leftWidget.added.connect(self.__propGroupAdded)
+        leftWidget.deleted.connect(self.__propGroupDeleted)
+        leftWidget.currentRowChanged.connect(self.__showProp)
+
+        self.__rightWidget = QStackedWidget()
+
+        for group in self.__previousPropGroups:
+            propTable = PropTable(self.__db, id=group[0])
+            propTable.updated.connect(self.updated)
+            self.__rightWidget.addWidget(propTable)
+
+        mainWidget = QSplitter()
+        mainWidget.addWidget(leftWidget)
+        mainWidget.addWidget(self.__rightWidget)
+        mainWidget.setChildrenCollapsible(False)
+        mainWidget.setSizes([300, 700])
 
+        lay = QVBoxLayout()
+        lay.addWidget(mainWidget)
+
+        self.setLayout(lay)
 
+    def __propGroupAdded(self, id):
+        propTable = PropTable(self.__db, id)
+        propTable.updated.connect(self.updated)
+        self.__rightWidget.addWidget(propTable)
+        self.__rightWidget.setCurrentWidget(propTable)
+
+    def __propGroupDeleted(self, n):
+        w = self.__rightWidget.widget(n)
+        self.__rightWidget.removeWidget(w)
+
+    def __showProp(self, n):
+        self.__rightWidget.setCurrentIndex(n)
+        w = self.__rightWidget.currentWidget()
+        if w and isinstance(w, PropTable):
+            self.updated.emit(w.getPromptText())
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/circleProfileImage.py` & `pyqt-openai-0.1.5/pyqt_openai/circleProfileImage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.5/pyqt_openai/convListWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         return super().enterEvent(e)
 
     def leaveEvent(self, e):
         self.__btnWidget.setVisible(False)
         return super().leaveEvent(e)
 
     def __btnClicked(self):
-        dialog = InputDialog('Rename', self.__topicLbl.text())
+        dialog = InputDialog('Rename', self.__topicLbl.text(), self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
             text = dialog.getText()
             self.__topicLbl.setText(text)
             self.convUpdated.emit(self.__id, text)
 
 class ConvListWidget(QListWidget):
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/customizeDialog.py` & `pyqt-openai-0.1.5/pyqt_openai/customizeDialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         self.__initUi()
 
     def __initVal(self):
         pass
 
     def __initUi(self):
         self.setWindowTitle('Customize (working)')
-        self.setWindowIcon(QIcon('ico/openai.svg'))
         self.setWindowFlags(Qt.Window | Qt.WindowCloseButtonHint)
 
         homePageGraphicsView = SingleImageGraphicsView()
 
         userImage = RoundedImage()
         userImage.setMaximumSize(24, 24)
         userImage.setImage('ico/user.svg')
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/customize.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/customize.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/download.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/save.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/ico/user.svg` & `pyqt-openai-0.1.5/pyqt_openai/ico/user.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.5/pyqt_openai/inputDialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from qtpy.QtWidgets import QDialog, QVBoxLayout, QLineEdit, QFrame, QPushButton, QHBoxLayout, QWidget
 from qtpy.QtCore import Qt
+from qtpy.QtGui import QIcon
 
 
 class InputDialog(QDialog):
-    def __init__(self, title, text):
-        super().__init__()
+    def __init__(self, title, text, parent=None):
+        super().__init__(parent)
         self.__initUi(title, text)
 
     def __initUi(self, title, text):
         self.setWindowTitle(title)
-        self.setWindowFlags(Qt.WindowCloseButtonHint)
+        self.setWindowFlags(Qt.Window | Qt.WindowCloseButtonHint)
 
         self.__newName = QLineEdit(text)
         self.__newName.textChanged.connect(self.__setAccept)
 
         sep = QFrame()
         sep.setFrameShape(QFrame.HLine)
         sep.setFrameShadow(QFrame.Sunken)
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.5/pyqt_openai/leftSideBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         self.__addBtn = SvgButton()
         self.__delBtn = SvgButton()
         self.__saveBtn = SvgButton()
 
         self.__addBtn.setIcon('ico/add.svg')
         self.__delBtn.setIcon('ico/delete.svg')
-        self.__saveBtn.setIcon('ico/download.svg')
+        self.__saveBtn.setIcon('ico/save.svg')
 
         self.__addBtn.setToolTip('Add')
         self.__delBtn.setToolTip('Delete')
         self.__saveBtn.setToolTip('Save')
 
         self.__addBtn.clicked.connect(self.__addClicked)
         self.__delBtn.clicked.connect(self.__deleteClicked)
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.5/pyqt_openai/modelTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtGui import QBrush, QColor
+from qtpy.QtGui import QBrush, QColor
 from qtpy.QtWidgets import QTableWidget, QHeaderView, QTableWidgetItem, QAbstractItemView
 from qtpy.QtCore import Qt
 
 
 class ModelTable(QTableWidget):
     def __init__(self):
         super().__init__()
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/notifier.py` & `pyqt-openai-0.1.5/pyqt_openai/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/prompt/promptGeneratorWidget.py` & `pyqt-openai-0.1.5/pyqt_openai/prompt/promptGeneratorWidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pyperclip
-
-from qtpy.QtWidgets import QApplication, QTextBrowser, QWidget, QTextEdit, QLabel, QVBoxLayout, QLineEdit, \
-    QFormLayout, QTableWidget, QPushButton, QTabWidget, QScrollArea
-
-from qtpy.QtGui import QTextCursor
+from qtpy.QtWidgets import QTextBrowser, QWidget, QLabel, QVBoxLayout, QPushButton, QTabWidget, QScrollArea
 
 from pyqt_openai.prompt.propPage import PropPage
 from pyqt_openai.prompt.templatePage import TemplatePage
+from pyqt_openai.sqlite import SqliteDatabase
 
 
 class PromptGeneratorWidget(QScrollArea):
-    def __init__(self):
+    def __init__(self, db: SqliteDatabase):
         super().__init__()
+        self.__initVal(db)
         self.__initUi()
 
+    def __initVal(self, db):
+        self.__db = db
+
     def __initUi(self):
         propmtLbl = QLabel('Prompt')
 
-        propPage = PropPage()
+        propPage = PropPage(self.__db)
         propPage.updated.connect(self.__textChanged)
 
-        templatePage = TemplatePage()
+        templatePage = TemplatePage(self.__db)
         templatePage.updated.connect(self.__textChanged)
 
         self.__prompt = QTextBrowser()
         self.__prompt.setPlaceholderText('Generated Prompt')
 
         promptTabWidget = QTabWidget()
         promptTabWidget.addTab(propPage, 'Property')
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/prompt/propPage.py` & `pyqt-openai-0.1.5/pyqt_openai/prompt/templatePage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-from qtpy.QtWidgets import QTableWidget, QAbstractItemView, QTableWidgetItem, QHeaderView, QHBoxLayout, \
-    QVBoxLayout, QWidget, QDialog
+from qtpy.QtWidgets import QWidget, QDialog, QTableWidget, QVBoxLayout, QHBoxLayout, QHeaderView, QTableWidgetItem, QAbstractItemView
 from qtpy.QtCore import Signal, Qt
 
 from pyqt_openai.inputDialog import InputDialog
+from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgButton import SvgButton
 
 
-class PropPage(QWidget):
-    """
-    benchmarked https://gptforwork.com/tools/prompt-generator
-    """
-    updated = Signal(str)
+class TemplatePage(QWidget):
+    updated = Signal(str, str)
 
-    def __init__(self):
+    def __init__(self, db: SqliteDatabase):
         super().__init__()
-        self.__initVal()
+        self.__initVal(db)
         self.__initUi()
 
-    def __initVal(self):
-        self.__defaultPromptPropArr = [{'name': 'Task', 'value': ''},
-                                       {'name': 'Topic', 'value': ''},
-                                       {'name': 'Style', 'value': ''},
-                                       {'name': 'Tone', 'value': ''},
-                                       {'name': 'Audience', 'value': ''},
-                                       {'name': 'Length', 'value': ''},
-                                       {'name': 'Form', 'value': ''}]
+    def __initVal(self, db):
+        self.__db = db
+        self.__previousTemplateArr = self.__db.selectTemplatePrompt()
 
     def __initUi(self):
         self.__addBtn = SvgButton()
         self.__delBtn = SvgButton()
 
         self.__addBtn.setIcon('ico/add.svg')
         self.__delBtn.setIcon('ico/delete.svg')
@@ -41,59 +33,78 @@
         lay.addWidget(self.__delBtn)
         lay.setAlignment(Qt.AlignRight)
         lay.setContentsMargins(0, 0, 0, 0)
 
         topWidget = QWidget()
         topWidget.setLayout(lay)
 
-        self.__table = QTableWidget()
-        self.__table.setColumnCount(2)
-        self.__table.setRowCount(len(self.__defaultPromptPropArr))
-        self.__table.horizontalHeader().setSectionResizeMode(1, QHeaderView.Stretch)
-        self.__table.setSelectionBehavior(QAbstractItemView.SelectRows)
-        self.__table.setHorizontalHeaderLabels(['Name', 'Value'])
-
-        for i in range(len(self.__defaultPromptPropArr)):
-            name = self.__defaultPromptPropArr[i]['name']
-            value = self.__defaultPromptPropArr[i]['value']
-            item1 = QTableWidgetItem(name)
-            item2 = QTableWidgetItem(value)
+        # this template has to be connected with db
+        # QSqlTableModel
+        self.__templateTable = QTableWidget()
+        self.__templateTable.setColumnCount(2)
+        self.__templateTable.setHorizontalHeaderLabels(['Name', 'Content'])
+        self.__templateTable.horizontalHeader().setSectionResizeMode(1, QHeaderView.Stretch)
+        self.__templateTable.setSelectionBehavior(QAbstractItemView.SelectRows)
+        self.__templateTable.currentItemChanged.connect(self.__rowChanged)
+
+        self.__templateTable.setRowCount(len(self.__previousTemplateArr))
+
+        for i in range(len(self.__previousTemplateArr)):
+            id = self.__previousTemplateArr[i][0]
+            name = self.__previousTemplateArr[i][1]
+            value = self.__previousTemplateArr[i][2]
+
+            content_item = QTableWidgetItem(name)
+            content_item.setTextAlignment(Qt.AlignCenter)
+            content_item.setData(Qt.UserRole, id)
 
-            item1.setTextAlignment(Qt.AlignCenter)
-            item2.setTextAlignment(Qt.AlignCenter)
+            self.__templateTable.setItem(i, 0, content_item)
+            self.__templateTable.setItem(i, 1, QTableWidgetItem(value))
 
-            self.__table.setItem(i, 0, item1)
-            self.__table.setItem(i, 1, item2)
-
-        self.__table.itemChanged.connect(self.__itemChanged)
+        self.__templateTable.itemChanged.connect(self.__saveUpdatedTemplate)
 
         lay = QVBoxLayout()
         lay.addWidget(topWidget)
-        lay.addWidget(self.__table)
+        lay.addWidget(self.__templateTable)
 
         self.setLayout(lay)
 
-    def __itemChanged(self, item: QTableWidgetItem):
-        if item.column() == 1:
-            prompt_text = ''
-            for i in range(self.__table.rowCount()):
-                if self.__table.item(i, 1).text().strip():
-                    prompt_text += f'{self.__table.item(i, 0).text()}: {self.__table.item(i, 1).text()}\n'
-            self.updated.emit(prompt_text)
+    def __rowChanged(self, new_item: QTableWidgetItem, old_item: QTableWidgetItem):
+        name_item = self.__templateTable.item(new_item.row(), 0)
+        name = name_item.text()
+        content = self.__templateTable.item(new_item.row(), 1).text() if new_item.column() == 0 else new_item.text()
+        self.updated.emit(content, name)
+
+    def __saveUpdatedTemplate(self, item: QTableWidgetItem):
+        name_item = self.__templateTable.item(item.row(), 0)
+        id = name_item.data(Qt.UserRole)
+        name = name_item.text()
+        content = self.__templateTable.item(item.row(), 1).text()
+        self.__db.updateTemplatePrompt(id, name, content)
 
     def __add(self):
-        dialog = InputDialog('Name', '')
+        dialog = InputDialog('Name', '', self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
+            self.__templateTable.itemChanged.disconnect(self.__saveUpdatedTemplate)
+
             text = dialog.getText()
-            self.__table.setRowCount(self.__table.rowCount()+1)
+            self.__templateTable.setRowCount(self.__templateTable.rowCount()+1)
+
             item1 = QTableWidgetItem(text)
             item1.setTextAlignment(Qt.AlignCenter)
-            self.__table.setItem(self.__table.rowCount()-1, 0, item1)
+            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 0, item1)
 
             item2 = QTableWidgetItem('')
             item2.setTextAlignment(Qt.AlignCenter)
-            self.__table.setItem(self.__table.rowCount()-1, 1, item2)
+            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 1, item2)
+
+            id = self.__db.insertTemplatePrompt(text)
+            item1.setData(Qt.UserRole, id)
+
+            self.__templateTable.itemChanged.connect(self.__saveUpdatedTemplate)
 
     def __delete(self):
-        for i in sorted(set([i.row() for i in self.__table.selectedIndexes()]), reverse=True):
-            self.__table.removeRow(i)
+        for i in sorted(set([i.row() for i in self.__templateTable.selectedIndexes()]), reverse=True):
+            id = self.__templateTable.item(i, 0).data(Qt.UserRole)
+            self.__db.deleteTemplatePrompt(id)
+            self.__templateTable.removeRow(i)
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/prompt/templatePage.py` & `pyqt-openai-0.1.5/pyqt_openai/image_gen_widget/imageListWidget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,149 @@
-from qtpy.QtWidgets import QWidget, QDialog, QTableWidget, QVBoxLayout, QHBoxLayout, QHeaderView, QTableWidgetItem, QAbstractItemView
-from qtpy.QtCore import Signal, Qt
+from datetime import datetime
+
+from qtpy.QtGui import QFont
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtWidgets import QListWidget, QDialog, QListWidgetItem, QLabel, QHBoxLayout, QWidget, QApplication, QVBoxLayout
 
 from pyqt_openai.inputDialog import InputDialog
 from pyqt_openai.svgButton import SvgButton
 
 
-class TemplatePage(QWidget):
-    updated = Signal(str, str)
+class ImageItemWidget(QWidget):
+    btnClicked = Signal(QListWidgetItem)
+    imageUpdated = Signal(int, str)
 
-    def __init__(self):
+    def __init__(self, text: str, item: QListWidgetItem, id):
         super().__init__()
-        self.__initUi()
+        self.__item = item
+        self.__id = id
+        self.__initUi(text)
 
-    def __initUi(self):
-        self.__addBtn = SvgButton()
-        self.__delBtn = SvgButton()
+    def __initUi(self, text):
+        self.__topicLbl = QLabel(text)
 
-        self.__addBtn.setIcon('ico/add.svg')
-        self.__delBtn.setIcon('ico/delete.svg')
+        lay = QVBoxLayout()
+        lay.addWidget(self.__topicLbl)
+        lay.setContentsMargins(0, 0, 0, 0)
 
-        self.__addBtn.clicked.connect(self.__add)
-        self.__delBtn.clicked.connect(self.__delete)
+        leftWidget = QWidget()
+        leftWidget.setLayout(lay)
+
+        editButton = SvgButton()
+        editButton.setIcon('ico/edit.svg')
+        editButton.setToolTip('Rename')
+        editButton.clicked.connect(self.__btnClicked)
 
         lay = QHBoxLayout()
-        lay.addWidget(self.__addBtn)
-        lay.addWidget(self.__delBtn)
-        lay.setAlignment(Qt.AlignRight)
         lay.setContentsMargins(0, 0, 0, 0)
+        lay.addWidget(editButton)
+        self.__btnWidget = QWidget()
+        self.__btnWidget.setLayout(lay)
+        self.__btnWidget.setVisible(False)
 
-        topWidget = QWidget()
-        topWidget.setLayout(lay)
+        lay = QVBoxLayout()
+        lay.addWidget(self.__btnWidget)
+        lay.setAlignment(Qt.AlignCenter | Qt.AlignRight)
+        lay.setContentsMargins(0, 0, 0, 0)
 
-        # this template has to be connected with db
-        # QSqlTableModel
-        self.__templateTable = QTableWidget()
-        self.__templateTable.setColumnCount(2)
-        self.__templateTable.setHorizontalHeaderLabels(['Content', 'Variables'])
-        self.__templateTable.horizontalHeader().setSectionResizeMode(0, QHeaderView.Stretch)
-        self.__templateTable.setSelectionBehavior(QAbstractItemView.SelectRows)
-        self.__templateTable.currentItemChanged.connect(self.__rowChanged)
-
-        # sample
-        # Alex Brogan's prompt example
-        sampleTemplateItems = [
-            'Identify the 20% of [topic or skill] that will yield 80% of the desired results and provide a focused learning plan to master it.',
-            'Explain [topic or skill] in the simplest terms possible as if teaching it to a complete beginner. Identify gaps in my understanding and suggest resources to fill them.',
-            'Create a study plan that mixes different topics or skills within [subject area] to help me develop a more robust understanding and facilitate connections between them.',
-            'Design a spaced repetition schedule for me to effectively review [topic or skill] over time, ensuring better retention and recall.',
-            'Help me create mental models or analogies to better understand and remember key concepts in [topic or skill].',
-            'Suggest various learning resources (e.g., videos, books, podcasts, interactive exercises) for [topic or skill] that cater to different learning styles.',
-            'Provide me with a series of challenging questions or problems related to [topic or skill] to test my understanding and improve long-term retention.',
-            'Transform key concepts or lessons from [topic or skill] into engaging stories or narratives to help me better remember and understand the material.',
-            'Design a deliberate practice routine for [topic or skill], focusing on my weaknesses and providing regular feedback for improvement.',
-            'Guide me through a visualization exercise to help me internalize [topic or skill] and imagine myself succesfully applying it in real-life situations.'
-        ]
-
-        self.__templateTable.setRowCount(len(sampleTemplateItems))
-        for i in range(len(sampleTemplateItems)):
-            content = sampleTemplateItems[i]
-            self.__templateTable.setItem(i, 0, QTableWidgetItem(content))
-            # variable = content.find()
-            self.__templateTable.setItem(i, 1, QTableWidgetItem('topic or skill'))
+        rightWidget = QWidget()
+        rightWidget.setLayout(lay)
 
-        lay = QVBoxLayout()
-        lay.addWidget(topWidget)
-        lay.addWidget(self.__templateTable)
+        lay = QHBoxLayout()
+        lay.addWidget(leftWidget)
+        lay.addWidget(rightWidget)
 
         self.setLayout(lay)
 
-    def __rowChanged(self, new_item: QTableWidgetItem, old_item: QTableWidgetItem):
-        content = self.__templateTable.item(new_item.row(), 0).text() if new_item.column() == 1 else new_item.text()
-        variable = self.__templateTable.item(new_item.row(), 1).text()
-        self.updated.emit(content, variable)
+        # Qt bug - not following by app's font size, update the font on its own after setItemWidget being called
+        # to avoid BUG (if there is nothing in qt bug report, i'll report by myself)
+        # i don't know this was fixed or not in PySide6 so i will check it out FIXME
+        self.__topicLbl.setFont(QApplication.font())
+
+        self.setAutoFillBackground(True)
+
+    def text(self):
+        return self.__topicLbl.text()
+
+    def enterEvent(self, e):
+        self.__btnWidget.setVisible(True)
+        return super().enterEvent(e)
+
+    def leaveEvent(self, e):
+        self.__btnWidget.setVisible(False)
+        return super().leaveEvent(e)
 
-    def __add(self):
-        dialog = InputDialog('Content', '')
+    def __btnClicked(self):
+        dialog = InputDialog('Rename', self.__topicLbl.text(), self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
             text = dialog.getText()
-            self.__templateTable.setRowCount(self.__templateTable.rowCount()+1)
-            item1 = QTableWidgetItem(text)
-            item1.setTextAlignment(Qt.AlignCenter)
-            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 0, item1)
-
-            item2 = QTableWidgetItem('')
-            item2.setTextAlignment(Qt.AlignCenter)
-            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 1, item2)
-
-    def __delete(self):
-        for i in sorted(set([i.row() for i in self.__templateTable.selectedIndexes()]), reverse=True):
-            self.__templateTable.removeRow(i)
+            self.__topicLbl.setText(text)
+            self.imageUpdated.emit(self.__id, text)
+
+
+class ImageListWidget(QListWidget):
+    changed = Signal(QListWidgetItem)
+    imageUpdated = Signal(int, str)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__initUi()
+
+    def __initUi(self):
+        self.itemClicked.connect(self.__clicked)
+        self.currentItemChanged.connect(self.changed)
+
+    def addImage(self, text: str, id: int):
+        item = QListWidgetItem()
+        item.setFlags(item.flags() | Qt.ItemIsUserCheckable)
+        item.setCheckState(Qt.Unchecked)
+        widget = ImageItemWidget(text, item, id)
+        widget.imageUpdated.connect(self.imageUpdated)
+        item.setSizeHint(widget.sizeHint())
+        item.setData(Qt.UserRole, id)
+        self.insertItem(0, item)
+        self.setItemWidget(item, widget)
+
+    def __clicked(self, item):
+        potentialChkBoxWidgetInItem = QApplication.widgetAt(self.cursor().pos())
+        if isinstance(potentialChkBoxWidgetInItem, QWidget) and potentialChkBoxWidgetInItem.children():
+            if isinstance(potentialChkBoxWidgetInItem.children()[0], ImageItemWidget):
+                if item.listWidget().itemWidget(item) != None:
+                    if item.checkState() == Qt.Checked:
+                        item.setCheckState(Qt.Unchecked)
+                    else:
+                        item.setCheckState(Qt.Checked)
+
+    def toggleState(self, state):
+        for i in range(self.count()):
+            item = self.item(i)
+            if item.checkState() != state:
+                item.setCheckState(state)
+
+    def getCheckedRowsIds(self):
+        return self.__getFlagRows(Qt.Checked, is_id=True)
+
+    def getUncheckedRowsIds(self):
+        return self.__getFlagRows(Qt.Unchecked, is_id=True)
+
+    def __getFlagRows(self, flag: Qt.CheckState, is_id: bool = False):
+        flag_lst = []
+        for i in range(self.count()):
+            item = self.item(i)
+            if item.checkState() == flag:
+                token = item.data(Qt.UserRole) if is_id else i
+                flag_lst.append(token)
+
+        return flag_lst
+
+    def removeCheckedRows(self):
+        self.__removeFlagRows(Qt.Checked)
+
+    def removeUncheckedRows(self):
+        self.__removeFlagRows(Qt.Unchecked)
+
+    def __removeFlagRows(self, flag):
+        flag_lst = self.__getFlagRows(flag)
+        flag_lst = reversed(flag_lst)
+        for i in flag_lst:
+            self.takeItem(i)
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.5/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from PyQt5.QtCore import QSettings
+from qtpy.QtCore import QSettings
 from qtpy.QtWidgets import QScrollArea, QWidget, QTabWidget, QGridLayout
 
 from pyqt_openai.right_sidebar.chatPage import ChatPage
 from pyqt_openai.right_sidebar.completionPage import CompletionPage
-from pyqt_openai.right_sidebar.imagePage import ImagePage
 from pyqt_openai.sqlite import SqliteDatabase
 
 
 class AIPlaygroundWidget(QScrollArea):
     def __init__(self, db: SqliteDatabase, ini_etc_dict, model_data):
         super().__init__()
         self.__initVal(db, ini_etc_dict, model_data)
@@ -29,19 +28,17 @@
         self.__db.setModelType(self.__cur_idx+1)
 
     def __initUi(self):
         tabWidget = QTabWidget()
 
         chatPage = ChatPage(self.__db, self.__ini_etc_dict)
         self.__completionPage = CompletionPage(self.__db, self.__ini_etc_dict, self.__modelData)
-        imagePage = ImagePage(self.__db)
 
         tabWidget.addTab(chatPage, 'Chat', )
         tabWidget.addTab(self.__completionPage, 'Completion', )
-        tabWidget.addTab(imagePage, 'Image (testing)', )
         tabWidget.currentChanged.connect(self.__tabChanged)
         tabWidget.setCurrentIndex(self.__cur_idx)
 
         lay = QGridLayout()
         lay.addWidget(tabWidget)
 
         mainWidget = QWidget()
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.5/pyqt_openai/right_sidebar/chatPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.5/pyqt_openai/right_sidebar/completionPage.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         self.__findDataLineEdit = QLineEdit()
 
         seeEveryModelCheckBox = QCheckBox('View every model (not all models may work)')
         seeEveryModelCheckBox.toggled.connect(self.__seeEveryModelToggled)
         seeEveryModelCheckBoxLbl = SvgLabel()
         seeEveryModelCheckBoxLbl.setSvgFile('ico/help.svg')
         seeEveryModelCheckBoxLbl.setToolTip(
-            '''Check this box to show all models, including obsolete ones. If you don\'t check this, combobox lists <a href="https://platform.openai.com/docs/models/gpt-3-5">latest models.</a>''')
-        seeEveryModelCheckBoxLbl.installEventFilter(self)
+            '''Check this box to show all models, including obsolete ones. \nIf you don\'t check this, combobox lists latest models.''')
 
         lay = QHBoxLayout()
         lay.addWidget(seeEveryModelCheckBox)
         lay.addWidget(seeEveryModelCheckBoxLbl)
         lay.setContentsMargins(0, 0, 0, 0)
         lay.setAlignment(Qt.AlignLeft)
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.5/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.5/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/sqlite.py` & `pyqt-openai-0.1.5/pyqt_openai/sqlite.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,17 +21,22 @@
         self.__conv_tb_nm = 'conv_tb'
         self.__conv_tb_tr_nm = 'conv_tr'
         self.__conv_unit_tb_nm = 'conv_unit_tb'
 
         # info table names
         self.__info_tb_nm = 'info_tb'
         self.__completion_info_tb_nm = 'info_completion_tb'
-        self.__image_info_tb_nm = 'image_info_tb'
 
-        # model type (chat, image, etc.)
+        # prompt table
+        self.__prop_prompt_group_tb_nm = 'prop_prompt_grp_tb'
+        self.__prop_prompt_unit_tb_nm = 'prop_prompt_unit_tb'
+
+        self.__template_prompt_tb_nm = 'template_prompt_tb'
+
+        # model type (chat, etc.)
         self.__model_type = 1
 
         # default value of each properties based on https://platform.openai.com/docs/api-reference/chat/create
         # GPT-3.5(ChatGPT), GPT-4
         self.__chat_default_value = {
             'engine': "gpt-3.5-turbo",
             'system': "You are a helpful assistant.",
@@ -50,26 +55,57 @@
             'temperature': 0.7,
             'max_tokens': 4096,
             'top_p': 1,
             'frequency_penalty': 0,
             'presence_penalty': 0,
         }
 
-        # DALL-E, Midjourney, Stable Diffusion
+        # DALL-E
         self.__image_default_value = {
             'engine': "DALL-E",
             'n': 1,
             'width': 1024,
             'height': 1024,
             # 'response_format':
         }
 
         self.__each_info_dict = {1: [self.__info_tb_nm, self.__chat_default_value],
-                                 2: [self.__completion_info_tb_nm, self.__completion_default_value],
-                                 3: [self.__image_info_tb_nm, self.__image_default_value], }
+                                 2: [self.__completion_info_tb_nm, self.__completion_default_value], }
+
+        self.__prop_prompt_unit_default_value = [{'name': 'Task', 'text': ''},
+                                                 {'name': 'Topic', 'text': ''},
+                                                 {'name': 'Style', 'text': ''},
+                                                 {'name': 'Tone', 'text': ''},
+                                                 {'name': 'Audience', 'text': ''},
+                                                 {'name': 'Length', 'text': ''},
+                                                 {'name': 'Form', 'text': ''}]
+
+        # based on Alex Brogan's prompt example
+        self.__template_prompt_default_value = [
+            {'name': 'Sample 1',
+             'text': 'Identify the 20% of [topic or skill] that will yield 80% of the desired results and provide a focused learning plan to master it.'},
+             {'name': 'Sample 2',
+              'text': 'Explain [topic or skill] in the simplest terms possible as if teaching it to a complete beginner. Identify gaps in my understanding and suggest resources to fill them.'},
+              {'name': 'Sample 3',
+               'text': 'Create a study plan that mixes different topics or skills within [subject area] to help me develop a more robust understanding and facilitate connections between them.'},
+               {'name': 'Sample 4',
+                'text': 'Design a spaced repetition schedule for me to effectively review [topic or skill] over time, ensuring better retention and recall.'},
+                {'name': 'Sample 5',
+                 'text': 'Help me create mental models or analogies to better understand and remember key concepts in [topic or skill].'},
+                 {'name': 'Sample 6',
+                  'text': 'Suggest various learning resources (e.g., videos, books, podcasts, interactive exercises) for [topic or skill] that cater to different learning styles.'},
+                  {'name': 'Sample 7',
+                   'text': 'Provide me with a series of challenging questions or problems related to [topic or skill] to test my understanding and improve long-term retention.'},
+                   {'name': 'Sample 8',
+                    'text': 'Transform key concepts or lessons from [topic or skill] into engaging stories or narratives to help me better remember and understand the material.'},
+                    {'name': 'Sample 9',
+                     'text': 'Design a deliberate practice routine for [topic or skill], focusing on my weaknesses and providing regular feedback for improvement.'},
+                     {'name': 'Sample 10',
+                      'text': 'Guide me through a visualization exercise to help me internalize [topic or skill] and imagine myself succesfully applying it in real-life situations.'}
+        ]
 
     def __initDb(self):
         try:
             # Connect to the database (create a new file if it doesn't exist)
             self.__conn = sqlite3.connect(self.__db_filename)
             self.__conn.execute('PRAGMA foreign_keys = ON;')
             self.__conn.commit()
@@ -161,51 +197,206 @@
                                                         presence_penalty
                                                     ) VALUES
                                                     (
                                                         {','.join(['?' for _ in range(len(self.__completion_default_value))])}
                                                     )
                                                  ''', tuple(self.__completion_default_value.values()))
 
-    def __createImage(self):
-        # Check if the table exists
-        self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__image_info_tb_nm}'")
+    def __createPropPromptGroup(self):
+        self.__c.execute(
+            f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__prop_prompt_group_tb_nm}'")
         if self.__c.fetchone()[0] == 1:
             pass
         else:
-            self.__c.execute(f'''CREATE TABLE {self.__image_info_tb_nm}
-                                             (id INTEGER PRIMARY KEY,
-                                              engine VARCHAR(50) DEFAULT '{self.__image_default_value['engine']}',
-                                              n INTEGER DEFAULT {self.__image_default_value['n']},
-                                              width INTEGER DEFAULT {self.__image_default_value['width']},
-                                              height INTEGER DEFAULT {self.__image_default_value['height']},  
+            self.__c.execute(f'''CREATE TABLE {self.__prop_prompt_group_tb_nm}
+                                                 (id INTEGER PRIMARY KEY,
+                                                  name VARCHAR(50),
+                                                  
+                                                  update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                                  insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
 
-                                              update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
-                                              insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
+            # Commit the transaction
+            self.__conn.commit()
+
+            self.insertPropPromptGroup('Default')
+
+    def createDefaultPropPromptAttributes(self, id_fk):
+        self.__c.execute(
+            f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__prop_prompt_unit_tb_nm}{id_fk}'")
+        if self.__c.fetchone()[0] == 1:
+            pass
+        else:
+            self.__c.execute(f'''CREATE TABLE {self.__prop_prompt_unit_tb_nm}{id_fk}
+                                                             (id INTEGER PRIMARY KEY,
+                                                              id_fk INTEGER,
+                                                              name VARCHAR(50),
+                                                              text TEXT,
+                                                              update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                                              insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                                              FOREIGN KEY (id_fk) REFERENCES {self.__prop_prompt_group_tb_nm}(id)
+                                                              ON DELETE CASCADE)''')
+
+        # insert default property group
+        for obj in self.__prop_prompt_unit_default_value:
+            lst = [id_fk] + list(tuple(obj.values()))
+            self.__c.execute(f"INSERT INTO {self.__prop_prompt_unit_tb_nm}{id_fk} (id_fk, name, text) VALUES (?, ?, ?)", tuple(lst))
+
+        # Commit the transaction
+        self.__conn.commit()
 
+    def selectPropPromptAttribute(self, id):
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__prop_prompt_unit_tb_nm}{id}')
+            return self.__c.fetchall()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def insertPropPromptAttribute(self, id, name):
+        try:
+            # Insert a row into the table
+            self.__c.execute(f'INSERT INTO {self.__prop_prompt_unit_tb_nm}{id} (id_fk, name) VALUES (?, ?)', (id, name,))
+            new_id = self.__c.lastrowid
             # Commit the transaction
             self.__conn.commit()
+            return new_id
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
 
-            # insert default record
-            self.__c.execute(f'''INSERT INTO {self.__image_info_tb_nm}
-                                                    (
-                                                        engine,
-                                                        n,
-                                                        width,
-                                                        height
-                                                    ) VALUES
-                                                    (
-                                                        {','.join(['?' for _ in range(len(self.__image_default_value))])}
-                                                    )
-                                                 ''', tuple(self.__image_default_value.values()))
+    def updatePropPromptAttribute(self, p_id, id, name, text):
+        try:
+            self.__c.execute(f'UPDATE {self.__prop_prompt_unit_tb_nm}{p_id} SET name=?, text=? WHERE id={id}', (name, text))
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def deletePropPromptAttribute(self, p_id, id):
+        try:
+            self.__c.execute(f'DELETE FROM {self.__prop_prompt_unit_tb_nm}{p_id} WHERE id={id}')
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def selectPropPromptGroup(self):
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__prop_prompt_group_tb_nm}')
+            return self.__c.fetchall()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def selectPropPromptGroupId(self, id):
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__prop_prompt_group_tb_nm} WHERE id={id}')
+            return self.__c.fetchone()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def insertPropPromptGroup(self, name):
+        try:
+            # Insert a row into the table
+            self.__c.execute(f'INSERT INTO {self.__prop_prompt_group_tb_nm} (name) VALUES (?)', (name,))
+            new_id = self.__c.lastrowid
+            # Commit the transaction
+            self.__conn.commit()
+            # insert default attributes
+            self.createDefaultPropPromptAttributes(new_id)
+            # TODO abcd make others insert statement return like this
+            return new_id
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def updatePropPromptGroup(self, id, name):
+        try:
+            self.__c.execute(f'UPDATE {self.__prop_prompt_group_tb_nm} SET name=(?) WHERE id={id}', (name,))
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def deletePropPromptGroup(self, id):
+        try:
+            self.__c.execute(f'DELETE FROM {self.__prop_prompt_group_tb_nm} WHERE id={id}')
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def __createTemplatePrompt(self):
+        self.__c.execute(
+            f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__template_prompt_tb_nm}'")
+        if self.__c.fetchone()[0] == 1:
+            pass
+        else:
+            self.__c.execute(f'''CREATE TABLE {self.__template_prompt_tb_nm}
+                                                 (id INTEGER PRIMARY KEY,
+                                                  name VARCHAR(50),
+                                                  text TEXT,
+                                                  update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                                  insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
+
+            # Commit the transaction
+            self.__conn.commit()
+
+            # insert default template set
+            for obj in self.__template_prompt_default_value:
+                self.__c.execute(f"INSERT INTO {self.__template_prompt_tb_nm} (name, text) VALUES (?, ?)", tuple(obj.values()))
+
+    def selectTemplatePrompt(self):
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__template_prompt_tb_nm}')
+            return self.__c.fetchall()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def insertTemplatePrompt(self, name):
+        try:
+            # Insert a row into the table
+            self.__c.execute(f"INSERT INTO {self.__template_prompt_tb_nm} (name, text) VALUES (?, ?)",
+                             (name, ''))
+            new_id = self.__c.lastrowid
+            # Commit the transaction
+            self.__conn.commit()
+            return new_id
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def updateTemplatePrompt(self, id, name, text):
+        try:
+            self.__c.execute(f'UPDATE {self.__template_prompt_tb_nm} SET name=(?), text=(?) WHERE id={id}', (name, text))
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def deleteTemplatePrompt(self, id):
+        try:
+            self.__c.execute(f'DELETE FROM {self.__template_prompt_tb_nm} WHERE id={id}')
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
 
     def __createInfo(self):
         try:
+            # chat and completion information
             self.__createChat()
             self.__createCompletion()
-            self.__createImage()
+
+            # prompt information
+            self.__createPropPromptGroup()
+            self.__createTemplatePrompt()
+
             # Commit the transaction
             self.__conn.commit()
         except sqlite3.Error as e:
             print(f"An error occurred while creating the table: {e}")
             raise
 
     def __createConv(self):
@@ -480,12 +671,8 @@
         self.__conn.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         # Close the connection
-        self.__conn.close()
-
-
-with SqliteDatabase() as f:
-    pass
+        self.__conn.close()
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.5/pyqt_openai/svgToolButton.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path, posixpath
 
 from qtpy.QtGui import QColor, QPalette, qGray
-from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QPushButton
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QToolButton
 
 
-class SvgButton(QPushButton):
+class SvgToolButton(QToolButton):
     def __init__(self, base_widget: QWidget = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__baseWidget = base_widget
         self.__initVal()
         self.__styleInit()
 
     def __initVal(self):
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.5/pyqt_openai/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/svgToolButton.py` & `pyqt-openai-0.1.5/pyqt_openai/svgButton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os.path, posixpath
 
 from qtpy.QtGui import QColor, QPalette, qGray
-from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QToolButton
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QPushButton
 
 
-class SvgToolButton(QToolButton):
-    def __init__(self, base_widget: QWidget = None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+class SvgButton(QPushButton):
+    def __init__(self, base_widget: QWidget = None, parent=None):
+        super().__init__(parent)
         self.__baseWidget = base_widget
         self.__initVal()
         self.__styleInit()
 
     def __initVal(self):
         # to set size accordance with scale
         sc = qApp.screens()[0]
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/test/htmlformat.py` & `pyqt-openai-0.1.5/pyqt_openai/test/htmlformat.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/test/prompt_autocomplete.py` & `pyqt-openai-0.1.5/pyqt_openai/test/prompt_autocomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-from PyQt5.QtWidgets import QApplication, QMainWindow, QTextEdit, QVBoxLayout, QWidget, QCompleter
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QTextCursor
+from qtpy.QtWidgets import QApplication, QMainWindow, QTextEdit, QVBoxLayout, QWidget, QCompleter
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QTextCursor
 
 class AutoCompleteTextEdit(QTextEdit):
     def __init__(self, parent=None):
         super(AutoCompleteTextEdit, self).__init__(parent)
         self.completer = None
 
     def set_completer(self, completer):
```

### Comparing `pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/delete_model.py` & `pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/delete_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/make_model.py` & `pyqt-openai-0.1.5/pyqt_openai/test/stable_diffusion/in_model/make_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.3/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.5/pyqt_openai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.3
+Version: 0.1.5
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,113 +13,131 @@
 # pyqt-openai
 <p align="center">
   <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
 </p>
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
-This shows an example of using OpenAI with PyQt as a chatbot.
+This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
-Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
+Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
+
+<b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
+
+But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
 
 You can select the model at the right side bar.
 
 An internet connection is required.
 
-## Contact
-You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
-
-## Note
-Some of the features are still being tested.
-
-I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+## Table of Contents
+* [Feature](#feature)
+* [Requirements](#requirements)
+* [Preview & Usage](#preview-usage)
+* [How to Install](#how-to-install)
+* [Troubleshooting](#troubleshooting)
+* [Contact](#contact)
+* [Note](#note)
+* [See Also](#see-also)
 
 ## Feature
-* basically this is <b>desktop application version of ChatGPT</b>
+* basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable)
+* support prompt generator (manageable, autosaved in database)
+* support slash commands
 * support beginning and ending part of the prompt
-* support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
+* image generation (DALL-E, Stable Diffusion with DreamStudio API)
+* you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
+* pyperclip - to copy prompt template from prompt generator
+* stability_sdk - for Stable Diffusion
 
-## Preview
-This is using GPT-3.5 turbo model by default. 
-
-### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
-<b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
-
+## Preview & Usage
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
+#### Note: Some of these previews are not the latest.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
+<b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
+
+You can change screen between text chatbot and image generating tool screen.
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
-### Conversation preview
-#### Preview Image
-![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
-#### Preview Video
+### Conversation
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
-#### Preview 1 (v0.1.22)
-https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
-#### Preview 2 (v0.1.3)
-https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
-
-So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
-
-## How to play
-1. git clone ~
-2. from the root directory, type "cd pyqt_openai"
-3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
+https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+
+You can use the additional prompt feature by "prompt menu" right next to input field.
+
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+
+### Image Generation
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
+
+## How to Install
+1. open command propmt of your OS.
+2. git clone ~
+3. from the root directory, type "cd pyqt_openai"
+4. pip install -r requirements.txt
+5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
-4. python main.py
+6. python main.py
 
-If installation doesn't work, check the troubleshooting below.
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
-you can shout a curse word and just download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
+download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
+Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
+
+## Contact
+You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
+
+## Note
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## TODO list
-* support Stable Diffusion
+* DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
```

#### html2text {}

```diff
@@ -1,64 +1,76 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.3 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.5 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
-shows an example of using OpenAI with PyQt as a chatbot. Even though this
-project has become too huge to be called an 'example'. The major advantage of
-this package is that you don't need to know other language aside from Python.
-If you want to study openai with Python-only good old desktop software, this is
-for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
-generation feature available since v0.0.16. You can see the detail in official
-OpenAI site. Currently this feature is very basic now. This is using sqlite as
-a database. You can select the model at the right side bar. An internet
-connection is required. ## Contact You can join pyqt-openai's Discord_Server to
-have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. I recommend to install sqlite management
-software. It's not necessary to run this app (obviously), but it's good
-practice to manage database about conversation history with AI and to know how
-this works. ## Feature * basically this is desktop application version of
-ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
-past conversation * conversation management * add & delete conversations * save
+shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
+Stable Diffusion as a image generation tool. Even though this project has
+become too huge to be called an 'example'. The major advantage of this package
+is that you don't need to know other language aside from Python. If you want to
+study openai with Python-only good old desktop software, this is for you. The
+OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
+functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
+feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
+used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
+stable-diffusion-webgui. But this is very lightweight and more accessible.
+don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
+database. You can select the model at the right side bar. An internet
+connection is required. ## Table of Contents * [Feature](#feature) *
+[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
+Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
+(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
+is desktop application version of ChatGPT with image generation tool. * text
+streaming (enable by default, you can disable it) * AI remembers past
+conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable) * support beginning and ending part of
-the prompt * support image generation with DALL-E * you can run this in
-background application * notification will pop up when response is generated *
-you can make window stack on top or control its transparency ## Requirements *
-qtpy - the package allowing you to write code that works with both PyQt and
-PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
-turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
-b45401f8bb7c.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
-4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
-user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
-7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+* support prompt generator (manageable, autosaved in database) * support slash
+commands * support beginning and ending part of the prompt * you can run this
+in background application * notification will pop up when response is generated
+* you can make window stack on top or control its transparency * image
+generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
+download the image if you want. just hover the mouse cursor over the image. ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
+prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
+Preview & Usage ### Overview #### Note: Some of these previews are not the
+latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
+inside the red box. see [How to install](#how-to-install) You can change screen
+between text chatbot and image generating tool screen. ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
+07655cab2061) ### Conversation https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
-55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
-(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
-99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
-idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
-from the root directory, type "cd pyqt_openai" 3. You should put your api key
-in the line edit. You can get it in official_site of openai. Sign up and log in
-before you get it. By the way, this is free trial, not permanently free. See
-this after you have logged in. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 4. python
-main.py If installation doesn't work, check the troubleshooting below. ##
+Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
+1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
+"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
+pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
+Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
+of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
+pip install -r requirements.txt 5. You should put your api key in the line
+edit. You can get it in official_site of openai. Sign up and log in before you
+get it. Be sure, this is a very important API key that belongs to you only, so
+you should remember it and keep it secure. 6. python main.py If installation
+doesn't work, you can contact me with bring up new issue in issue tab or check
+the troubleshooting below even it is only about very specific error. ##
 Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` you can shout a curse word and just download
-the package itself from pypi. Unzip it, access the package directory, type ```
-python setup.py install ``` That will install the openai. ## TODO list *
-support Stable Diffusion * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+subprocess-exited-with-error ``` download the package itself from pypi. Unzip
+it, access the package directory, type ``` python setup.py install ``` That
+will install the openai. Note: I don't know this can happen in newer version of
+openai as well, so tell me if you know about something ## Contact You can join
+pyqt-openai's Discord_Server to have a conversation about it or AI-related
+stuff ð ## Note I recommend to install sqlite management software. It's not
+necessary to run this app (obviously), but it's good practice to manage
+database about conversation history with AI and to know how this works. ## TODO
+list * DB for images (to further experiement of both DALL-E and Stable
+Diffusion or other image generation engine) * show the explanation of every
+model and terms related to AI (e.g. temperature, topp..) * save conversation
+history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
+(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
+* show reason when the chat input is disabled for some reasons * add the basic
+example sources of making deep learning model with PyTorch (eventually) ## See
+Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
+from it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.3/setup.py` & `pyqt-openai-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.3',
+    version='0.1.5',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'customize.svg', 'user.svg',
-                                      'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg',
+    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'discord.svg', 'github.svg', 'help.svg', 'customize.svg', 'history.svg',
+                                      'user.svg', 'sidebar.svg', 'prompt.svg', 'save.svg', 'stackontop.svg',
                                       'add.svg', 'delete.svg', 'setting.svg', 'search.svg',
                                       'vertical_three_dots.svg']},
     description='PyQt OpenAI example',
     url='https://github.com/yjg30737/pyqt-openai.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
         'qtpy',
         'aiohttp',
         'openai',
-        'pyperclip'
+        'pyperclip',
+        'stability_sdk'
     ]
 )
```

