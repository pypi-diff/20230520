# Comparing `tmp/furo-2023.3.27.tar.gz` & `tmp/furo-2023.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furo-2023.3.27.tar", last modified: Mon Mar 27 10:01:17 2023, max compression
+gzip compressed data, was "furo-2023.5.20.tar", last modified: Sat May 20 08:55:19 2023, max compression
```

## Comparing `furo-2023.3.27.tar` & `furo-2023.5.20.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-03-27 10:01:17.528320 furo-2023.3.27/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2023.3.27/CODE_OF_CONDUCT.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2023.3.27/LICENSE
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2022-12-07 02:13:05.993369 furo-2023.3.27/README.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-03-27 09:59:45.158311 furo-2023.3.27/docs/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2023.3.27/docs/_static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2023.3.27/docs/_static/demo-dark.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2023.3.27/docs/_static/demo-light.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2023.3.27/docs/_static/demo.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2023.3.27/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2023.3.27/docs/_static/readthedocs-dummy.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    18660 2023-03-27 10:00:32.858167 furo-2023.3.27/docs/changelog.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2023-03-27 09:59:45.158525 furo-2023.3.27/docs/conf.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2023.3.27/docs/contributing/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2023.3.27/docs/contributing/design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2023.3.27/docs/contributing/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2023.3.27/docs/contributing/internals.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2023.3.27/docs/contributing/workflow.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-03-27 09:59:45.158698 furo-2023.3.27/docs/customisation/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2023.3.27/docs/customisation/announcement.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2023.3.27/docs/customisation/colors.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2023.3.27/docs/customisation/edit-button.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2023.3.27/docs/customisation/fonts.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5214 2023-03-27 09:59:45.158893 furo-2023.3.27/docs/customisation/footer.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3587 2022-12-07 02:12:20.994955 furo-2023.3.27/docs/customisation/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2023.3.27/docs/customisation/injecting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      971 2022-12-07 02:12:20.995118 furo-2023.3.27/docs/customisation/landing-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1822 2022-12-07 02:12:20.995197 furo-2023.3.27/docs/customisation/logo.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2023.3.27/docs/customisation/sidebar-title.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2023.3.27/docs/customisation/sidebar.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2023.3.27/docs/customisation/toc.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2023.3.27/docs/index.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-26 12:21:17.346555 furo-2023.3.27/docs/kitchen-sink/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2022-12-07 02:12:20.995648 furo-2023.3.27/docs/kitchen-sink/admonitions.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2023.3.27/docs/kitchen-sink/api.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8110 2023-02-25 11:34:51.779610 furo-2023.3.27/docs/kitchen-sink/blocks.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2022-12-26 12:21:17.346902 furo-2023.3.27/docs/kitchen-sink/generic.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2023.3.27/docs/kitchen-sink/images.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2023.3.27/docs/kitchen-sink/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2023.3.27/docs/kitchen-sink/lists.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12983 2023-03-23 23:04:54.882119 furo-2023.3.27/docs/kitchen-sink/really-long.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2023.3.27/docs/kitchen-sink/sphinx-design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2023.3.27/docs/kitchen-sink/structure.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5068 2022-12-07 02:12:20.996744 furo-2023.3.27/docs/kitchen-sink/tables.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2023.3.27/docs/kitchen-sink/typography.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2022-12-07 02:12:20.996914 furo-2023.3.27/docs/license.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2023.3.27/docs/quickstart.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2023.3.27/docs/recommendations.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-03 20:59:07.302559 furo-2023.3.27/docs/reference/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2023.3.27/docs/reference/admonitions.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-02-03 20:59:07.303276 furo-2023.3.27/docs/reference/api.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2023.3.27/docs/reference/code-blocks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2023.3.27/docs/reference/hyperlinks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1922 2022-12-07 02:12:20.997623 furo-2023.3.27/docs/reference/images.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2023.3.27/docs/reference/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2023.3.27/docs/reference/lists.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2023.3.27/docs/reference/tables.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2023.3.27/docs/reference/tabs.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2023.3.27/docs/reference/text-formatting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2023.3.27/docs/requirements.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2022-12-07 02:12:20.998207 furo-2023.3.27/docs/stability.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4588 2022-12-07 02:12:20.999297 furo-2023.3.27/noxfile.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)   102153 2022-12-26 12:20:59.239393 furo-2023.3.27/package-lock.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)      420 2022-12-07 02:12:21.001928 furo-2023.3.27/package.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2023.3.27/postcss.config.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1342 2023-03-11 09:30:27.931063 furo-2023.3.27/pyproject.toml
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2023.3.27/src/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:45:29.513868 furo-2023.3.27/src/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)    13988 2023-03-27 10:01:10.001838 furo-2023.3.27/src/furo/__init__.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1448 2022-12-07 02:12:21.002879 furo-2023.3.27/src/furo/_demo_module.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2023.3.27/src/furo/assets/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003142 furo-2023.3.27/src/furo/assets/scripts/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2022-12-07 02:12:21.003092 furo-2023.3.27/src/furo/assets/scripts/furo.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12991 2022-12-07 02:12:21.003228 furo-2023.3.27/src/furo/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919042 furo-2023.3.27/src/furo/assets/styles/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     9649 2023-02-25 11:33:38.919397 furo-2023.3.27/src/furo/assets/styles/_scaffold.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2023.3.27/src/furo/assets/styles/_shame.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2023.3.27/src/furo/assets/styles/base/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2023.3.27/src/furo/assets/styles/base/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2023.3.27/src/furo/assets/styles/base/_print.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      300 2022-12-07 02:12:21.003967 furo-2023.3.27/src/furo/assets/styles/base/_screen-readers.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2023.3.27/src/furo/assets/styles/base/_theme.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-07 02:12:21.004155 furo-2023.3.27/src/furo/assets/styles/base/_typography.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919529 furo-2023.3.27/src/furo/assets/styles/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2023.3.27/src/furo/assets/styles/components/_footer.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2023.3.27/src/furo/assets/styles/components/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2023.3.27/src/furo/assets/styles/components/_search.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6094 2022-12-07 02:12:21.005360 furo-2023.3.27/src/furo/assets/styles/components/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1832 2022-12-07 02:12:21.005453 furo-2023.3.27/src/furo/assets/styles/components/_table_of_contents.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-03 20:59:07.303520 furo-2023.3.27/src/furo/assets/styles/content/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1933 2022-12-07 02:12:21.005588 furo-2023.3.27/src/furo/assets/styles/content/_admonitions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2360 2023-02-03 20:59:07.304033 furo-2023.3.27/src/furo/assets/styles/content/_api.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2023.3.27/src/furo/assets/styles/content/_blocks.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2023.3.27/src/furo/assets/styles/content/_captions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3199 2023-03-23 22:59:33.724162 furo-2023.3.27/src/furo/assets/styles/content/_code.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      846 2022-12-07 02:12:21.006385 furo-2023.3.27/src/furo/assets/styles/content/_footnotes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2023.3.27/src/furo/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2023.3.27/src/furo/assets/styles/content/_images.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2023.3.27/src/furo/assets/styles/content/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2023.3.27/src/furo/assets/styles/content/_indexes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2023.3.27/src/furo/assets/styles/content/_lists.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2022-12-07 02:12:21.006878 furo-2023.3.27/src/furo/assets/styles/content/_math.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2023.3.27/src/furo/assets/styles/content/_misc.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2023.3.27/src/furo/assets/styles/content/_rubrics.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2023.3.27/src/furo/assets/styles/content/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2023.3.27/src/furo/assets/styles/content/_tables.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2022-12-07 02:12:21.007844 furo-2023.3.27/src/furo/assets/styles/content/_target.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2023.3.27/src/furo/assets/styles/extensions/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2023.3.27/src/furo/assets/styles/extensions/_copybutton.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2023.3.27/src/furo/assets/styles/extensions/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2023.3.27/src/furo/assets/styles/extensions/_readthedocs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-design.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-panels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2023.3.27/src/furo/assets/styles/furo-extensions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2023.3.27/src/furo/assets/styles/furo.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.920180 furo-2023.3.27/src/furo/assets/styles/variables/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2023.3.27/src/furo/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6355 2022-12-26 19:15:34.355902 furo-2023.3.27/src/furo/assets/styles/variables/_colors.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1366 2022-12-07 02:12:21.008944 furo-2023.3.27/src/furo/assets/styles/variables/_fonts.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2023.3.27/src/furo/assets/styles/variables/_icons.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2023.3.27/src/furo/assets/styles/variables/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2023.3.27/src/furo/assets/styles/variables/_layout.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2023.3.27/src/furo/assets/styles/variables/_spacing.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2817 2022-12-07 02:12:21.009414 furo-2023.3.27/src/furo/navigation.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2395 2022-12-07 02:12:21.009536 furo-2023.3.27/src/furo/sphinxext.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2023.3.27/src/furo/theme/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013802 furo-2023.3.27/src/furo/theme/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3206 2022-12-07 02:12:21.009927 furo-2023.3.27/src/furo/theme/furo/base.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2023.3.27/src/furo/theme/furo/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2023.3.27/src/furo/theme/furo/components/edit-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2023.3.27/src/furo/theme/furo/domainindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2023.3.27/src/furo/theme/furo/genindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2023.3.27/src/furo/theme/furo/globaltoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2023.3.27/src/furo/theme/furo/layout.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2023.3.27/src/furo/theme/furo/localtoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)    11025 2023-02-19 17:22:59.452178 furo-2023.3.27/src/furo/theme/furo/page.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2023.3.27/src/furo/theme/furo/partials/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2023.3.27/src/furo/theme/furo/partials/_head_css_variables.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2023.3.27/src/furo/theme/furo/partials/icons.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2022-12-07 02:12:21.012606 furo-2023.3.27/src/furo/theme/furo/search.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2023.3.27/src/furo/theme/furo/sidebar/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2023.3.27/src/furo/theme/furo/sidebar/brand.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2023.3.27/src/furo/theme/furo/sidebar/ethical-ads.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2023.3.27/src/furo/theme/furo/sidebar/navigation.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2023.3.27/src/furo/theme/furo/sidebar/rtd-versions.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2023.3.27/src/furo/theme/furo/sidebar/scroll-end.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2023.3.27/src/furo/theme/furo/sidebar/scroll-start.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2023.3.27/src/furo/theme/furo/sidebar/search.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2023.3.27/src/furo/theme/furo/sidebar/variant-selector.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2023.3.27/src/furo/theme/furo/static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2023.3.27/src/furo/theme/furo/static/.gitignore
--rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2023.3.27/src/furo/theme/furo/theme.conf
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2023.3.27/webpack.config.js
--rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 furo-2023.3.27/PKG-INFO
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 08:55:19.653102 furo-2023.5.20/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2023.5.20/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2023.5.20/LICENSE
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2023.5.20/README.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 16:46:08.985680 furo-2023.5.20/docs/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2023.5.20/docs/_static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2023.5.20/docs/_static/demo-dark.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2023.5.20/docs/_static/demo-light.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2023.5.20/docs/_static/demo.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2023.5.20/docs/_static/pied-piper-admonition.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2023.5.20/docs/_static/readthedocs-dummy.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    18926 2023-05-20 08:54:08.268498 furo-2023.5.20/docs/changelog.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2023-03-27 09:59:45.158525 furo-2023.5.20/docs/conf.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2023.5.20/docs/contributing/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2023.5.20/docs/contributing/design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2023.5.20/docs/contributing/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2023.5.20/docs/contributing/internals.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2023.5.20/docs/contributing/workflow.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 06:29:53.184727 furo-2023.5.20/docs/customisation/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2023.5.20/docs/customisation/announcement.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2023.5.20/docs/customisation/colors.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2023.5.20/docs/customisation/edit-button.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2023.5.20/docs/customisation/fonts.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5214 2023-03-27 09:59:45.158893 furo-2023.5.20/docs/customisation/footer.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2023.5.20/docs/customisation/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2023.5.20/docs/customisation/injecting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      971 2022-12-07 02:12:20.995118 furo-2023.5.20/docs/customisation/landing-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2023.5.20/docs/customisation/logo.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2023.5.20/docs/customisation/sidebar-title.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2023.5.20/docs/customisation/sidebar.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2023.5.20/docs/customisation/toc.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2023.5.20/docs/index.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:39.133954 furo-2023.5.20/docs/kitchen-sink/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2022-12-07 02:12:20.995648 furo-2023.5.20/docs/kitchen-sink/admonitions.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2023.5.20/docs/kitchen-sink/api.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8110 2023-02-25 11:34:51.779610 furo-2023.5.20/docs/kitchen-sink/blocks.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2023.5.20/docs/kitchen-sink/generic.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2023.5.20/docs/kitchen-sink/images.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2023.5.20/docs/kitchen-sink/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2023.5.20/docs/kitchen-sink/lists.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12983 2023-03-23 23:04:54.882119 furo-2023.5.20/docs/kitchen-sink/really-long.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2023.5.20/docs/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2023.5.20/docs/kitchen-sink/structure.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5068 2022-12-07 02:12:20.996744 furo-2023.5.20/docs/kitchen-sink/tables.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2023.5.20/docs/kitchen-sink/typography.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2022-12-07 02:12:20.996914 furo-2023.5.20/docs/license.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2023.5.20/docs/quickstart.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2023.5.20/docs/recommendations.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2023.5.20/docs/reference/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2023.5.20/docs/reference/admonitions.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2023.5.20/docs/reference/api.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2023.5.20/docs/reference/code-blocks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2023.5.20/docs/reference/hyperlinks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1922 2022-12-07 02:12:20.997623 furo-2023.5.20/docs/reference/images.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2023.5.20/docs/reference/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2023.5.20/docs/reference/lists.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2023.5.20/docs/reference/tables.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2023.5.20/docs/reference/tabs.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2023.5.20/docs/reference/text-formatting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2023.5.20/docs/requirements.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2023.5.20/docs/stability.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4588 2023-05-20 06:29:59.350803 furo-2023.5.20/noxfile.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   120224 2023-05-20 06:36:37.700979 furo-2023.5.20/package-lock.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      421 2023-03-27 12:04:35.297935 furo-2023.5.20/package.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2023.5.20/postcss.config.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1342 2023-05-20 06:34:19.599411 furo-2023.5.20/pyproject.toml
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2023.5.20/src/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-05-20 06:29:53.185006 furo-2023.5.20/src/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    14114 2023-05-20 08:55:13.356395 furo-2023.5.20/src/furo/__init__.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1448 2022-12-07 02:12:21.002879 furo-2023.5.20/src/furo/_demo_module.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2023.5.20/src/furo/assets/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003142 furo-2023.5.20/src/furo/assets/scripts/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2022-12-07 02:12:21.003092 furo-2023.5.20/src/furo/assets/scripts/furo.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12991 2022-12-07 02:12:21.003228 furo-2023.5.20/src/furo/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919042 furo-2023.5.20/src/furo/assets/styles/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     9649 2023-02-25 11:33:38.919397 furo-2023.5.20/src/furo/assets/styles/_scaffold.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2023.5.20/src/furo/assets/styles/_shame.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2023.5.20/src/furo/assets/styles/base/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2023.5.20/src/furo/assets/styles/base/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2023.5.20/src/furo/assets/styles/base/_print.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      300 2022-12-07 02:12:21.003967 furo-2023.5.20/src/furo/assets/styles/base/_screen-readers.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2023.5.20/src/furo/assets/styles/base/_theme.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-07 02:12:21.004155 furo-2023.5.20/src/furo/assets/styles/base/_typography.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919529 furo-2023.5.20/src/furo/assets/styles/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2023.5.20/src/furo/assets/styles/components/_footer.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2023.5.20/src/furo/assets/styles/components/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2023.5.20/src/furo/assets/styles/components/_search.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6094 2022-12-07 02:12:21.005360 furo-2023.5.20/src/furo/assets/styles/components/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1832 2022-12-07 02:12:21.005453 furo-2023.5.20/src/furo/assets/styles/components/_table_of_contents.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:43.172691 furo-2023.5.20/src/furo/assets/styles/content/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1933 2022-12-07 02:12:21.005588 furo-2023.5.20/src/furo/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2360 2023-02-03 20:59:07.304033 furo-2023.5.20/src/furo/assets/styles/content/_api.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2023.5.20/src/furo/assets/styles/content/_blocks.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2023.5.20/src/furo/assets/styles/content/_captions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3199 2023-03-23 22:59:33.724162 furo-2023.5.20/src/furo/assets/styles/content/_code.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      846 2022-12-07 02:12:21.006385 furo-2023.5.20/src/furo/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2023.5.20/src/furo/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2023.5.20/src/furo/assets/styles/content/_images.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2023.5.20/src/furo/assets/styles/content/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2023.5.20/src/furo/assets/styles/content/_indexes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2023.5.20/src/furo/assets/styles/content/_lists.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2023.5.20/src/furo/assets/styles/content/_math.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2023.5.20/src/furo/assets/styles/content/_misc.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2023.5.20/src/furo/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2023.5.20/src/furo/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2023.5.20/src/furo/assets/styles/content/_tables.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2022-12-07 02:12:21.007844 furo-2023.5.20/src/furo/assets/styles/content/_target.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2023.5.20/src/furo/assets/styles/extensions/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2023.5.20/src/furo/assets/styles/extensions/_copybutton.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2023.5.20/src/furo/assets/styles/extensions/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2023.5.20/src/furo/assets/styles/extensions/_readthedocs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-design.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-panels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2023.5.20/src/furo/assets/styles/furo-extensions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2023.5.20/src/furo/assets/styles/furo.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.920180 furo-2023.5.20/src/furo/assets/styles/variables/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2023.5.20/src/furo/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6355 2022-12-26 19:15:34.355902 furo-2023.5.20/src/furo/assets/styles/variables/_colors.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1366 2022-12-07 02:12:21.008944 furo-2023.5.20/src/furo/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2023.5.20/src/furo/assets/styles/variables/_icons.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2023.5.20/src/furo/assets/styles/variables/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2023.5.20/src/furo/assets/styles/variables/_layout.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2023.5.20/src/furo/assets/styles/variables/_spacing.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2023.5.20/src/furo/navigation.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2395 2022-12-07 02:12:21.009536 furo-2023.5.20/src/furo/sphinxext.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2023.5.20/src/furo/theme/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013802 furo-2023.5.20/src/furo/theme/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3206 2022-12-07 02:12:21.009927 furo-2023.5.20/src/furo/theme/furo/base.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2023.5.20/src/furo/theme/furo/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2023.5.20/src/furo/theme/furo/components/edit-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2023.5.20/src/furo/theme/furo/domainindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2023.5.20/src/furo/theme/furo/genindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2023.5.20/src/furo/theme/furo/globaltoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2023.5.20/src/furo/theme/furo/layout.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2023.5.20/src/furo/theme/furo/localtoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    11025 2023-02-19 17:22:59.452178 furo-2023.5.20/src/furo/theme/furo/page.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2023.5.20/src/furo/theme/furo/partials/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2023.5.20/src/furo/theme/furo/partials/_head_css_variables.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2023.5.20/src/furo/theme/furo/partials/icons.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2022-12-07 02:12:21.012606 furo-2023.5.20/src/furo/theme/furo/search.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2023.5.20/src/furo/theme/furo/sidebar/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2023.5.20/src/furo/theme/furo/sidebar/brand.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2023.5.20/src/furo/theme/furo/sidebar/ethical-ads.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2023.5.20/src/furo/theme/furo/sidebar/navigation.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2023.5.20/src/furo/theme/furo/sidebar/rtd-versions.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2023.5.20/src/furo/theme/furo/sidebar/scroll-end.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2023.5.20/src/furo/theme/furo/sidebar/scroll-start.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2023.5.20/src/furo/theme/furo/sidebar/search.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2023.5.20/src/furo/theme/furo/sidebar/variant-selector.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2023.5.20/src/furo/theme/furo/static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2023.5.20/src/furo/theme/furo/static/.gitignore
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2023.5.20/src/furo/theme/furo/theme.conf
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2023.5.20/webpack.config.js
+-rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 furo-2023.5.20/PKG-INFO
```

### Comparing `furo-2023.3.27/CODE_OF_CONDUCT.md` & `furo-2023.5.20/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/LICENSE` & `furo-2023.5.20/LICENSE`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/README.md` & `furo-2023.5.20/README.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/_static/demo-dark.png` & `furo-2023.5.20/docs/_static/demo-dark.png`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/_static/demo-light.png` & `furo-2023.5.20/docs/_static/demo-light.png`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/_static/demo.png` & `furo-2023.5.20/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/_static/pied-piper-admonition.css` & `furo-2023.5.20/docs/_static/pied-piper-admonition.css`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/changelog.md` & `furo-2023.5.20/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 date "+## %Y.%m.%d -- {adjective} {colorname}" | pbcopy
 
 https://patternbasedwriting.com/elementary_writing_success/list-4800-adjectives/
 https://en.wikipedia.org/wiki/Lists_of_colors
 
 -->
 
+## 2023.05.20 -- Unassuming Ultramarine
+
+- ✨ Add support for Sphinx 7.
+- Drop support for Sphinx 5.
+- Improve the screen-reader label for sidebar collapse.
+- Make it easier to create derived themes from Furo.
+- Bump all JS dependencies (NodeJS and npm packages).
+
 ## 2023.03.27 -- Tasty Tangerine
 
 - Regenerate with newer version of sphinx-theme-builder, to fix RECORD hashes.
 - Add missing class to Font Awesome examples
 
 ## 2023.03.23 -- Sassy Saffron
```

### Comparing `furo-2023.3.27/docs/conf.py` & `furo-2023.5.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/contributing/design.md` & `furo-2023.5.20/docs/contributing/design.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/contributing/index.md` & `furo-2023.5.20/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/contributing/internals.md` & `furo-2023.5.20/docs/contributing/internals.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/contributing/workflow.md` & `furo-2023.5.20/docs/contributing/workflow.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/announcement.md` & `furo-2023.5.20/docs/customisation/announcement.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/colors.md` & `furo-2023.5.20/docs/customisation/colors.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/edit-button.md` & `furo-2023.5.20/docs/customisation/edit-button.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/fonts.md` & `furo-2023.5.20/docs/customisation/fonts.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/footer.md` & `furo-2023.5.20/docs/customisation/footer.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/index.md` & `furo-2023.5.20/docs/customisation/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 }
 ```
 
 ```{caution}
 Typos in the `*_css_variables` dictionary are silently ignored, and do not raise any errors or warnings. Double check that your spellings and values are correct and valid.
 ```
 
+(sidebar_hide_name)=
+
 ### `sidebar_hide_name`
 
 Controls whether you see the project's name in the sidebar of the documentation. This is useful when you only want to show your documentation's logo in the sidebar. The default is `False`.
 
 ```python
 html_theme_options = {
     "sidebar_hide_name": True,
@@ -96,12 +98,12 @@
 
 ### `hide-toc`
 
 The “Contents” sidebar is automatically hidden for any pages that don’t have any inner headings. It is possible to hide it even when a page has inner headings, by setting `hide-toc` at the page level. See {doc}`./toc` for an example.
 
 ## Custom CSS files
 
-If you want more control than what is provided by the above theme options, see {any}`customisation/injecting.md#injecting-code`.
+If you want more control than what is provided by the above theme options, see {doc}`injecting`.
 
 [css-variables]: https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties
 [sphinx-html_theme_options]: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_theme_options
 [sphinx-file-wide-metadata]: https://www.sphinx-doc.org/en/master/usage/restructuredtext/field-lists.html#metadata
```

### Comparing `furo-2023.3.27/docs/customisation/injecting.md` & `furo-2023.5.20/docs/customisation/injecting.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/landing-page.md` & `furo-2023.5.20/docs/customisation/landing-page.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/logo.md` & `furo-2023.5.20/docs/customisation/logo.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 The filenames must be relative to the [`html_static_path`][sphinx-html_static_path] folder. In the above example, that'd be `_static/logo-light-mode.png` and `_static/logo-dark-mode.png`.
 
 This is different from how `html_logo` works, which copies the given filename into the correct location automagically.
 ```
 
 ## Related Information
 
-It is also possible to [hide the name of the project in the sidebar](customisation/index.md#sidebar_hide_name), which might be desirable if the logo contains the project name.
+It is also possible to [hide the name of the project in the sidebar](sidebar_hide_name), which might be desirable if the logo contains the project name.
 
 [sphinx-html_logo]: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_logo
 [sphinx-html_theme_options]: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_theme_options
 [sphinx-html_static_path]: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_static_path
```

### Comparing `furo-2023.3.27/docs/customisation/sidebar.md` & `furo-2023.5.20/docs/customisation/sidebar.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/customisation/toc.md` & `furo-2023.5.20/docs/customisation/toc.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/admonitions.rst` & `furo-2023.5.20/docs/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/api.rst` & `furo-2023.5.20/docs/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/blocks.rst` & `furo-2023.5.20/docs/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/generic.rst` & `furo-2023.5.20/docs/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/images.rst` & `furo-2023.5.20/docs/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/index.md` & `furo-2023.5.20/docs/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/lists.rst` & `furo-2023.5.20/docs/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/really-long.md` & `furo-2023.5.20/docs/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/sphinx-design.md` & `furo-2023.5.20/docs/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/structure.rst` & `furo-2023.5.20/docs/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/tables.rst` & `furo-2023.5.20/docs/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/kitchen-sink/typography.rst` & `furo-2023.5.20/docs/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/recommendations.md` & `furo-2023.5.20/docs/recommendations.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/admonitions.md` & `furo-2023.5.20/docs/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/api.md` & `furo-2023.5.20/docs/reference/api.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/code-blocks.md` & `furo-2023.5.20/docs/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/hyperlinks.md` & `furo-2023.5.20/docs/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/images.md` & `furo-2023.5.20/docs/reference/images.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/index.md` & `furo-2023.5.20/docs/reference/index.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/lists.md` & `furo-2023.5.20/docs/reference/lists.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/tables.md` & `furo-2023.5.20/docs/reference/tables.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/tabs.md` & `furo-2023.5.20/docs/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/reference/text-formatting.md` & `furo-2023.5.20/docs/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/docs/stability.md` & `furo-2023.5.20/docs/stability.md`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/noxfile.py` & `furo-2023.5.20/noxfile.py`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/pyproject.toml` & `furo-2023.5.20/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["sphinx-theme-builder >= 0.2.0a10"]
 build-backend = "sphinx_theme_builder"
 
 [tool.sphinx-theme-builder]
-node-version = "16.15.1"
+node-version = "18.16.0"
 additional-compiled-static-assets = [
   "styles/furo-extensions.css",
 ]
 
 [project]
 name = "furo"
 description = "A clean customisable Sphinx documentation theme."
 dynamic = ["version"]
 readme = "README.md"
 
 requires-python = ">=3.7"
 dependencies = [
   "beautifulsoup4",
-  "sphinx >= 5.0,<7.0",
+  "sphinx >= 6.0,<8.0",
   "sphinx-basic-ng",
   "pygments >= 2.7",
 ]
 
 license = { file = "LICENSE"}
 authors = [
     {name = "Pradyun Gedam", email = "mail@pradyunsg.me"},
```

### Comparing `furo-2023.3.27/src/furo/__init__.py` & `furo-2023.5.20/src/furo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A clean customisable Sphinx documentation theme."""
 
-__version__ = "2023.03.27"
+__version__ = "2023.05.20"
 
 import hashlib
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional
@@ -164,18 +164,20 @@
 def _html_page_context(
     app: sphinx.application.Sphinx,
     pagename: str,
     templatename: str,
     context: Dict[str, Any],
     doctree: Any,
 ) -> None:
-    if app.config.html_theme != "furo":
-        return
-
-    assert isinstance(app.builder, StandaloneHTMLBuilder)
+    if not isinstance(app.builder, StandaloneHTMLBuilder):
+        raise Exception(
+            "Furo is being used with a non-HTML builder. "
+            "If you're seeing this error, it is a symptom of a mistake in your "
+            "configuration."
+        )
 
     if "css_files" in context:
         if "_static/styles/furo.css" not in context["css_files"]:
             raise Exception(
                 "This documentation is not using `furo.css` as the stylesheet. "
                 "If you have set `html_style` in your conf.py file, remove it."
             )
@@ -215,16 +217,14 @@
                 background="black",
             ),
         ),
     }
 
 
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
-    if app.config.html_theme != "furo":
-        return
     if "furo" in app.config.extensions:
         raise Exception(
             "Did you list 'furo' in the `extensions` in conf.py? "
             "If so, please remove it. Furo does not work with non-HTML builders "
             "and specifying it as an `html_theme` is sufficient."
         )
 
@@ -348,16 +348,16 @@
 
 
 def get_pygments_stylesheet() -> str:
     """Generate the theme-specific pygments.css.
 
     There is no way to tell Sphinx how the theme handles dark mode; at this time.
     """
-    light_formatter = HtmlFormatter(style=_KNOWN_STYLES_IN_USE["light"])
-    dark_formatter = HtmlFormatter(style=_KNOWN_STYLES_IN_USE["dark"])
+    light_formatter = PygmentsBridge.html_formatter(style=_KNOWN_STYLES_IN_USE["light"])
+    dark_formatter = PygmentsBridge.html_formatter(style=_KNOWN_STYLES_IN_USE["dark"])
 
     lines: List[str] = []
 
     lines.extend(_get_styles(light_formatter, prefix=".highlight"))
 
     lines.append("@media not print {")
```

### Comparing `furo-2023.3.27/src/furo/_demo_module.py` & `furo-2023.5.20/src/furo/_demo_module.py`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/scripts/furo.js` & `furo-2023.5.20/src/furo/assets/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/scripts/gumshoe-patched.js` & `furo-2023.5.20/src/furo/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/_scaffold.sass` & `furo-2023.5.20/src/furo/assets/styles/_scaffold.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/base/_print.sass` & `furo-2023.5.20/src/furo/assets/styles/base/_print.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/base/_theme.sass` & `furo-2023.5.20/src/furo/assets/styles/base/_theme.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/base/_typography.sass` & `furo-2023.5.20/src/furo/assets/styles/base/_typography.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/components/_footer.sass` & `furo-2023.5.20/src/furo/assets/styles/components/_footer.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/components/_sidebar.sass` & `furo-2023.5.20/src/furo/assets/styles/components/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/components/_table_of_contents.sass` & `furo-2023.5.20/src/furo/assets/styles/components/_table_of_contents.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_admonitions.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_api.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_code.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_footnotes.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_images.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_lists.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_misc.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_sidebar.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_tables.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/content/_target.sass` & `furo-2023.5.20/src/furo/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/extensions/_copybutton.sass` & `furo-2023.5.20/src/furo/assets/styles/extensions/_copybutton.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/extensions/_readthedocs.sass` & `furo-2023.5.20/src/furo/assets/styles/extensions/_readthedocs.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-design.sass` & `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-design.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass` & `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/extensions/_sphinx-panels.sass` & `furo-2023.5.20/src/furo/assets/styles/extensions/_sphinx-panels.sass`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/variables/_admonitions.scss` & `furo-2023.5.20/src/furo/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/variables/_colors.scss` & `furo-2023.5.20/src/furo/assets/styles/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/variables/_fonts.scss` & `furo-2023.5.20/src/furo/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/variables/_icons.scss` & `furo-2023.5.20/src/furo/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/assets/styles/variables/_spacing.scss` & `furo-2023.5.20/src/furo/assets/styles/variables/_spacing.scss`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/navigation.py` & `furo-2023.5.20/src/furo/navigation.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 "for": checkbox_name,
             },
         )
         screen_reader_label = soup.new_tag(
             "div",
             attrs={"class": "visually-hidden"},
         )
-        screen_reader_label.string = "Toggle child pages in navigation"
+        screen_reader_label.string = f"Toggle navigation of {element.find('a').text}"
         label.append(screen_reader_label)
         label.append(_get_navigation_expand_image(soup))
 
         element.insert(1, label)
 
         # Add the checkbox that's used to store expanded/collapsed state.
         checkbox = soup.new_tag(
```

### Comparing `furo-2023.3.27/src/furo/sphinxext.py` & `furo-2023.5.20/src/furo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/base.html` & `furo-2023.5.20/src/furo/theme/furo/base.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/components/edit-this-page.html` & `furo-2023.5.20/src/furo/theme/furo/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/domainindex.html` & `furo-2023.5.20/src/furo/theme/furo/domainindex.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/genindex.html` & `furo-2023.5.20/src/furo/theme/furo/genindex.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/page.html` & `furo-2023.5.20/src/furo/theme/furo/page.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/partials/_head_css_variables.html` & `furo-2023.5.20/src/furo/theme/furo/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/partials/icons.html` & `furo-2023.5.20/src/furo/theme/furo/partials/icons.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/search.html` & `furo-2023.5.20/src/furo/theme/furo/search.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/sidebar/brand.html` & `furo-2023.5.20/src/furo/theme/furo/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/sidebar/rtd-versions.html` & `furo-2023.5.20/src/furo/theme/furo/sidebar/rtd-versions.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/sidebar/variant-selector.html` & `furo-2023.5.20/src/furo/theme/furo/sidebar/variant-selector.html`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/src/furo/theme/furo/theme.conf` & `furo-2023.5.20/src/furo/theme/furo/theme.conf`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/webpack.config.js` & `furo-2023.5.20/webpack.config.js`

 * *Files identical despite different names*

### Comparing `furo-2023.3.27/PKG-INFO` & `furo-2023.5.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furo
-Version: 2023.3.27
+Version: 2023.5.20
 Summary: A clean customisable Sphinx documentation theme.
 Author-Email: Pradyun Gedam <mail@pradyunsg.me>
 License: Copyright (c) 2020 Pradyun Gedam <mail@pradyunsg.me>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
@@ -36,15 +36,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Project-URL: Github, https://github.com/pradyunsg/furo
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
-Requires-Dist: sphinx<7.0,>=5.0
+Requires-Dist: sphinx<8.0,>=6.0
 Requires-Dist: sphinx-basic-ng
 Requires-Dist: pygments>=2.7
 Description-Content-Type: text/markdown
 
 <h1 align="center">Furo</h1>
 <p align="center">
   A clean customisable <a href="https://www.sphinx-doc.org/">Sphinx</a> documentation theme.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: furo Version: 2023.3.27 Summary: A clean
+Metadata-Version: 2.1 Name: furo Version: 2023.5.20 Summary: A clean
 customisable Sphinx documentation theme. Author-Email: Pradyun Gedam
 pradyunsg.me> License: Copyright (c) 2020 Pradyun Gedam
 pradyunsg.me> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -21,15 +21,15 @@
 Developers Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Classifier: Topic
 :: Documentation Classifier: Topic :: Software Development :: Documentation
 Project-URL: Github, https://github.com/pradyunsg/furo Requires-Python: >=3.7
-Requires-Dist: beautifulsoup4 Requires-Dist: sphinx<7.0,>=5.0 Requires-Dist:
+Requires-Dist: beautifulsoup4 Requires-Dist: sphinx<8.0,>=6.0 Requires-Dist:
 sphinx-basic-ng Requires-Dist: pygments>=2.7 Description-Content-Type: text/
 markdown
                               ****** Furo ******
                A clean customisable Sphinx documentation theme.
 [Demo_image] ## Elevator pitch  - **Intentionally minimal** --- the most
 important thing is the content, not the scaffolding around it. - **Responsive**
 --- adapting perfectly to the available screen space, to work on all sorts of
```

