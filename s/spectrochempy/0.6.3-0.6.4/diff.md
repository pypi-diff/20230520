# Comparing `tmp/spectrochempy-0.6.3.tar.gz` & `tmp/spectrochempy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.3.tar", last modified: Mon May  1 07:46:29 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.4.tar", last modified: Sat May 20 17:55:20 2023, max compression
```

## Comparing `spectrochempy-0.6.3.tar` & `spectrochempy-0.6.4.tar`

### file list

```diff
@@ -1,229 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-01 07:46:29.536927 spectrochempy-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.508925 spectrochempy-0.6.3/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.508925 spectrochempy-0.6.3/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-01 07:46:29.536927 spectrochempy-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71352 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/kinetic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    49002 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/nmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/analysis/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9945 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   120664 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37871 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    54110 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.524926 spectrochempy-0.6.3/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.524926 spectrochempy-0.6.3/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    29909 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-20 17:55:20.719194 spectrochempy-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71573 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/kinetic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/nmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/analysis/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36669 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/_check_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/plot_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119937 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74644 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53899 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.699194 spectrochempy-0.6.4/spectrochempy/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28400 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.699194 spectrochempy-0.6.4/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29889 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39297 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45433 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa_keller_massart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_chrom1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_lstsq_single_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/nddataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_baseline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/examples/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/plot_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/examples/read/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_generic_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_nmr_from_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_raman_from_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/traittypes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/numutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.687193 spectrochempy-0.6.4/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.3/.codeclimate.yml` & `spectrochempy-0.6.4/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/.conda/meta.yaml` & `spectrochempy-0.6.4/.conda/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -52,28 +52,27 @@
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
-    - ipywidgets=8.0.4
-    - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
+
     # Jupyter lab
     - jupyterlab
     - nodejs
-
-
-#EOF
+    - ipywidgets=8.0.4
+    - widgetsnbextension=4.0.5
+    - jupyterlab_widgets=3.0.5
+    - ipympl
 
 
   test:
     - python  {{ python }}
 
 test:
   script_env:
```

### Comparing `spectrochempy-0.6.3/.pre-commit-config.yaml` & `spectrochempy-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/.pylintrc` & `spectrochempy-0.6.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/.zenodo.json` & `spectrochempy-0.6.4/.zenodo.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-05-20'", "'version'": "'0.6.4'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-05-01",
+    "publication_date": "2023-05-20",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.3"
+    "version": "0.6.4"
 }
```

### Comparing `spectrochempy-0.6.3/CITATION.cff` & `spectrochempy-0.6.4/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-05-01'
+date-released: '2023-05-20'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.3
+version: 0.6.4
```

### Comparing `spectrochempy-0.6.3/Dockerfile` & `spectrochempy-0.6.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSE` & `spectrochempy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.4/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.4/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.4/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.4/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.4/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/PKG-INFO` & `spectrochempy-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.3
+Version: 0.6.4
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.3/README.md` & `spectrochempy-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/environment.yml` & `spectrochempy-0.6.4/environment.yml`

 * *Files 11% similar despite different names*

```diff
@@ -41,21 +41,20 @@
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
-    - ipywidgets=8.0.4
-    - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
+
     # Jupyter lab
     - jupyterlab
     - nodejs
-
-
-#EOF
+    - ipywidgets=8.0.4
+    - widgetsnbextension=4.0.5
+    - jupyterlab_widgets=3.0.5
+    - ipympl
```

### Comparing `spectrochempy-0.6.3/environment_dev.yml` & `spectrochempy-0.6.4/environment_dev.yml`

 * *Files 7% similar despite different names*

```diff
@@ -41,37 +41,40 @@
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
-    - ipywidgets=8.0.4
-    - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
+
     # Jupyter lab
     - jupyterlab
     - nodejs
+    - ipywidgets=8.0.4
+    - widgetsnbextension=4.0.5
+    - jupyterlab_widgets=3.0.5
+    - ipympl
 
     # TEST dependencies
     # ----------------
     - coverage
     - pytest
     - pytest-doctestplus
     - pytest-flake8
     - pytest-mock
     - pyfakefs
     - pep8-naming
     - xarray
-# DEV dependencies
+
+    # DEV dependencies
     # ----------------
     # From here, the dependencies are essentially for development.
     # They should not be necessary for the user of  spectrochempy.
     - scikit-image
     - black
     - pre-commit
     - mamba
@@ -86,9 +89,7 @@
     - sphinx-copybutton
     - sphinxcontrib-bibtex
     - pandoc=2.19
     - conda-build
     - conda-verify
     - anaconda-client
     - numpydoc>=1.2
-
-#EOF
```

### Comparing `spectrochempy-0.6.3/environment_test.yml` & `spectrochempy-0.6.4/environment_test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -41,31 +41,31 @@
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
-    - ipywidgets=8.0.4
-    - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
+
     # Jupyter lab
     - jupyterlab
     - nodejs
+    - ipywidgets=8.0.4
+    - widgetsnbextension=4.0.5
+    - jupyterlab_widgets=3.0.5
+    - ipympl
 
     # TEST dependencies
     # ----------------
     - coverage
     - pytest
     - pytest-doctestplus
     - pytest-flake8
     - pytest-mock
     - pyfakefs
     - pep8-naming
     - xarray
-
-#EOF
```

### Comparing `spectrochempy-0.6.3/requirements/requirements.txt` & `spectrochempy-0.6.4/requirements/requirements.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
 xlrd
 pyyaml
-ipywidgets==8.0.4
-widgetsnbextension==4.0.5
-jupyterlab_widgets==3.0.5
-ipympl
 setuptools
 setuptools_scm
 gitpython
 jupyterlab
 nodejs
+ipywidgets==8.0.4
+widgetsnbextension==4.0.5
+jupyterlab_widgets==3.0.5
+ipympl
```

### Comparing `spectrochempy-0.6.3/requirements/requirements_dev.txt` & `spectrochempy-0.6.4/requirements/requirements_dev.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
 xlrd
 pyyaml
-ipywidgets==8.0.4
-widgetsnbextension==4.0.5
-jupyterlab_widgets==3.0.5
-ipympl
 setuptools
 setuptools_scm
 gitpython
 jupyterlab
 nodejs
+ipywidgets==8.0.4
+widgetsnbextension==4.0.5
+jupyterlab_widgets==3.0.5
+ipympl
 coverage
 pytest
 pytest-doctestplus
 pytest-flake8
 pytest-mock
 pyfakefs
 pep8-naming
```

### Comparing `spectrochempy-0.6.3/requirements/requirements_test.txt` & `spectrochempy-0.6.4/requirements/requirements_test.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
 xlrd
 pyyaml
-ipywidgets==8.0.4
-widgetsnbextension==4.0.5
-jupyterlab_widgets==3.0.5
-ipympl
 setuptools
 setuptools_scm
 gitpython
 jupyterlab
 nodejs
+ipywidgets==8.0.4
+widgetsnbextension==4.0.5
+jupyterlab_widgets==3.0.5
+ipympl
 coverage
 pytest
 pytest-doctestplus
 pytest-flake8
 pytest-mock
 pyfakefs
 pep8-naming
```

### Comparing `spectrochempy-0.6.3/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.4/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.4/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.4/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.4/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.4/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.4/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.4/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.4/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.4/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.4/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.4/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scripts/checkindex.py` & `spectrochempy-0.6.4/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/scripts/validate_docstrings.py` & `spectrochempy-0.6.4/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/setup.cfg` & `spectrochempy-0.6.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -51,44 +51,47 @@
 
 [tool:pytest]
 testpaths = 
 	"tests"
 addopts = 
 	--ignore="~*"
 	--doctest-plus
+	-p no:warnings
 doctest_plus = enabled
 doctest_optionflags = 
 	ELLIPSIS
 	NORMALIZE_WHITESPACE
 	IGNORE_EXCEPTION_DETAIL
 	ALLOW_UNICODE
 	ALLOW_BYTES
 
 [coverage:run]
 source = spectrochempy/
-branch = true
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	'# '
 	if self.debug:
 	raise AssertionError
 	raise NotImplementedError
 	if 0:
 	if __name__ == .__main__.:
 	def __repr__
 	if settings.DEBUG
 ignore_errors = true
 omit = 
-	.ci/*
-	tests/*
-	docs/*
-	build/*
-	scripts/*
-	scp_data/*
-	~sandbox/*
+	*/.ci/**/*
+	*/tests/**/
+	*/docs/**/*
+	*/build/**/*
+	*/.eggs/**/*
+	*/scripts/**/*
+	*/scp_data/**/*
+	*/~sandbox/**/*
+	*/~tools/**/*
+	*/spectrochempy/extern/**/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `spectrochempy-0.6.3/setup.py` & `spectrochempy-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/__init__.py` & `spectrochempy-0.6.4/spectrochempy/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/_base.py` & `spectrochempy-0.6.4/spectrochempy/analysis/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,33 +154,43 @@
                 if self.typey == "components":
                     X_transf.set_coordset(
                         y=Coord(
                             None,
                             labels=["#%d" % (i) for i in range(X_transf.shape[0])],
                             title="components",
                         ),
-                        x=X.coord(-1),
+                        x=X.coord(-1).copy() if X.coord(-1) is not None else None,
                     )
                 if self.typex == "components":
                     X_transf.set_coordset(
-                        y=X.coord(0),  # cannot use X.y in case of transposed X
+                        y=X.coord(0).copy() if X.coord(0) is not None else None,
+                        # cannot use X.y in case of transposed X
                         x=Coord(
                             None,
                             labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
                             title="components",
                         ),
                     )
                 if self.typex == "features":
                     X_transf.set_coordset(
                         y=Coord(
                             None,
                             labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
                             title="components",
                         ),
-                        x=X.coord(1),
+                        x=X.coord(1).copy() if X.coord(1) is not None else None,
+                    )
+                if self.typey == "features":
+                    X_transf.set_coordset(
+                        y=X.coord(1).copy() if X.coord(1) is not None else None,
+                        x=Coord(
+                            None,
+                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
+                            title="components",
+                        ),
                     )
                 if self.typesingle == "components":
                     # occurs when the data are 1D such as ev_ratio...
                     X_transf.set_coordset(
                         x=Coord(
                             None,
                             labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
@@ -362,14 +372,26 @@
             d = [self._make_dataset(item) for item in d]
         elif not isinstance(d, NDDataset):
             d = NDDataset(d, copy=True)
         else:
             d = d.copy()
         return d
 
+    def _make_unsqueezed_dataset(self, d):
+        # add a dimension to 1D Dataset
+        if d.ndim == 1:
+            coordset = d.coordset
+            d._data = d._data[np.newaxis]
+            if np.any(d.mask):
+                d._mask = d._mask[np.newaxis]
+            d.dims = ["y", "x"]  # "y" is the new dimension
+            coordx = coordset[0] if coordset is not None else None
+            d.set_coordset(x=coordx, y=None)
+        return d
+
     def _get_masked_rc(self, mask):
         # Get the mask by row and columns.
         # -------------------------------
         # When a single element in the array is
         # masked, the whole row and columns for this element is masked as well as the
         # corresponding columns.
         if np.any(mask):
@@ -386,15 +408,14 @@
         # unfortunately, the implementation of linalg library
         # doesn't support numpy masked arrays as input. So we will have to
         # remove the masked values ourselves
 
         # the following however assumes that entire rows or columns are masked,
         # not only some individual data (if this is what you wanted, this
         # will fail)
-
         if not hasattr(X, "mask") or not np.any(X._mask):
             return X
 
         # remove masked rows and columns
         masked_rows, masked_columns = self._get_masked_rc(X._mask)
 
         Xc = X[:, ~masked_columns]
@@ -495,33 +516,29 @@
     def _X_default(self):
         raise NotFittedError
 
     @tr.validate("_X")
     def _X_validate(self, proposal):
         # validation fired when self._X is assigned
         X = proposal.value
+
         # for the following we need X with two dimensions
         # So let's generate the un-squeezed X
-        if X.ndim == 1:
-            coordset = X.coordset
-            X._data = X._data[np.newaxis]
-            if np.any(X.mask):
-                X._mask = X._mask[np.newaxis]
-            X.dims = ["y", "x"]  # "y" is the new dimension
-            coordx = coordset[0] if coordset is not None else None
-            X.set_coordset(x=coordx, y=None)
+        X = self._make_unsqueezed_dataset(X)
 
         # as in fit methods we often use np.linalg library, we cannot handle directly
         # masked data (so we remove them here and they will be restored at the end of
         # the process during transform or inverse transform methods
         # store the original shape as it will be eventually modified as welle- as the
         # original coordset
         self._X_shape = X.shape
+
         # store the mask because it may be destroyed
         self._X_mask = X._mask.copy()
+
         # and the original coordset
         self._X_coordset = copy(X._coordset)
 
         # remove masked data and return modified dataset
         X = self._remove_masked_data(X)
         return X
 
@@ -616,17 +633,17 @@
     _docstring.keep_params("analysis_fit.parameters", "X")
 
     @property
     def log(self):
         """
         Return ``log`` output.
         """
-        # A string handler (#2) is defined for the Spectrochempy logger,
+        # A string handler (#1) is defined for the Spectrochempy logger,
         # thus we will return it's content
-        return app.log.handlers[2].stream.getvalue().rstrip()
+        return app.log.handlers[1].stream.getvalue().rstrip()
 
     @property
     def X(self):
         """
         Return the X input dataset (eventually modified by the model).
         """
         if self._X_is_missing:
@@ -651,14 +668,15 @@
     Abstract class to write analysis decomposition models such as `PCA`, ...
 
     Subclass this to get a minimal structure
 
     See Also
     --------
     EFA : Perform an Evolving Factor Analysis (forward and reverse).
+    FastICA : Perform Independent Component Analysis with a fast algorithm.
     IRIS : Integral inversion solver for spectroscopic data.
     MCRALS : Perform MCR-ALS of a dataset knowing the initial :math:`C` or :math:`S^T` matrix.
     NMF : Non-Negative Matrix Factorization.
     PCA : Perform Principal Components Analysis.
     SIMPLISMA : SIMPLe to use Interactive Self-modeling Mixture Analysis.
     SVD : Perform a Singular Value Decomposition.
     """
@@ -1038,29 +1056,14 @@
         mao = ma * offset / 100
         mad = ma * offset / 100 + ma / 10
         _ = (X - X.min()).plot(color=colX, **kwargs)
         _ = (X_hat - X_hat.min() - mao).plot(
             clear=False, ls="dashed", cmap=None, color=colXhat
         )
         ax = (res - res.min() - mad).plot(clear=False, cmap=None, color=colRes)
-
-        #             color=colXhat)
-        #     ax.plot(res.T.masked_data - 1.2 * ma,
-        #             color=colRes)
-
-        # if X.x is not None and X.x.data is not None:
-        #     ax.plot(X.x.data, X_hat.T.masked_data - ma, '-',
-        #             color=colXhat)
-        #     ax.plot(X.x.data, res.T.masked_data - 1.2 * ma, '-',
-        #             color=colRes)
-        # else:
-        #     ax.plot(X_hat.T.masked_data - ma,
-        #             color=colXhat)
-        #     ax.plot(res.T.masked_data - 1.2 * ma,
-        #             color=colRes)
         ax.autoscale(enable=True, axis="y")
         ax.set_title(f"{self.name} plot of merit")
         ax.yaxis.set_visible(False)
         return ax
 
     _docstring.get_sections(_docstring.dedent(plotmerit.__doc__), base="plotmerit")
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/api.py` & `spectrochempy-0.6.4/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/efa.py` & `spectrochempy-0.6.4/spectrochempy/analysis/efa.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.4/spectrochempy/analysis/iris.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         default_value=None,
         allow_none=True,
         help="Target/profiles taken into account to fit a model",
     )
     _Y_preprocessed = Array(help="preprocessed Y")
     _q = CoordType()
     _channels = CoordType()
-    _lambdas = CoordType()
+    _lambdas = CoordType().tag(rounding=False)
     _regularization = tr.Bool(False)
     _search_reg = tr.Bool(False)
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # ----------------------------------------------------------------------------------
     reg_par = tr.List(
@@ -388,15 +388,15 @@
             log_level=log_level,
             warm_start=warm_start,
             **kwargs,
         )
         # no validation of reg_par triggred when it is None
         # so we need to init self._lambdas manually else itt will not be inited
         if self.reg_par is None:
-            self._lambdas = Coord([0], title="lambda")
+            self._lambdas = Coord([0], title="lambda", rounding=False)
 
     # ----------------------------------------------------------------------------------
     # Private validation and default getter methods
     # ----------------------------------------------------------------------------------
     @tr.validate("reg_par")
     def _reg_par_validate(self, proposal):
         reg_par = proposal.value
@@ -414,15 +414,15 @@
             _lambdas = np.logspace(reg_par[0], reg_par[1], reg_par[2])
         else:
             raise ValueError(
                 "reg_par should be either None or a set of 2 or 3 integers"
             )
 
         # create the lambdas coordinate
-        self._lambdas = Coord(_lambdas, title="lambda")
+        self._lambdas = Coord(_lambdas, title="lambda", rounding=False)
 
         # return the validated reg_par with no transformation
         return reg_par
 
     @tr.validate("_Y")
     def _Y_validate(self, proposal):
         # validation of the _Y attribute: fired when self._Y is assigned
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/kinetic_utilities.py` & `spectrochempy-0.6.4/spectrochempy/analysis/kinetic_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,246 +11,462 @@
 """
 
 import datetime
 import logging
 import re
 import warnings
 from collections.abc import Iterable
+from functools import partial
 
 import numpy as np
 import traitlets as tr
 from scipy.integrate import solve_ivp
 from scipy.optimize import differential_evolution, least_squares, minimize
 
-from spectrochempy.core import debug_, error_
+from spectrochempy.core import error_
 from spectrochempy.core.dataset.nddataset import Coord, NDDataset
 from spectrochempy.core.units import Quantity
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.exceptions import SpectroChemPyError
 from spectrochempy.utils.optional import import_optional_dependency
 
 __all__ = [
     "ActionMassKinetics",
     "PFR",
 ]
 
 R = 8.314462618153241
+SCIPY_MINIMIZE_METHODS = [
+    "NELDER-MEAD",
+    "POWELL",
+    "CG",
+    "BFGS",
+    "NEWTON-CG",
+    "L-BFGS-B",
+    "TNC",
+    "COBYLA",
+    "SLSQP",
+    "TRUST-CONSTR",
+    "DOGLEG",
+    "TRUST-NCG",
+    "TRUST-KRYLOV",
+    "TRUST-EXACT",
+]
 
 
 # exception used in this module
 class SolverError(SpectroChemPyError):
     """Error raised if solve_ivp (integrate) return a status < 0"""
 
 
+# ------------------------------------------------------------------------------------
+# ACTION MASS KINETICS
+# ------------------------------------------------------------------------------------
+
 # Utility
 # --------
 def _interpret_equation(eq, species):
-    # transform an equation given as a string to a dictionary of species with
-    # integer stoechiometric coefficients.
+    # transform an equation given as a string to dictionaries of species with
+    # integer stoechiometric coefficients for the left (reactants) and right (products)
+    # side of the equation.
 
     regex = r"(((([\.,0-9]*)((?=[a-zA-Z])[a-zA-Z, 1-9]+))(?=\+?))?(?=(->|→)?))"
 
     matches = re.finditer(regex, eq.replace(" ", ""))
-    equation = {}
-    mult = -1  # reactants
+    left, right = {}, {}
+    is_reactant = True
     for match in matches:
         if not match.group(5):
             # no species
             continue
         s = match.group(5)
         if s not in species:
             raise ValueError(
                 f'Species "{s}" in equation "{eq}" is not listed in species\n'
                 f"Available species : {species}"
             )
         coef = match.group(4) if match.group(4) else 1
-        equation[s] = float(coef) * mult
+        try:
+            coef = int(coef)
+        except ValueError:
+            raise ValueError(
+                f"Stoichiometric coeffcients must be integers. Could not "
+                f"convert {coef} in int"
+            )
+        if is_reactant:
+            left[s] = coef
+        else:
+            right[s] = coef
+
         if match.group(6) in ["->", "→"]:
             # shift to products
-            mult = 1
-
-    # normalize the coefficients (for float we assume that they have at the maximum
-    # 2 decimals
-    y = (np.array(list(equation.values())) * 100).astype(int)
-    div = np.gcd.reduce(np.abs(y))
-    equation = {k: int(v * 100 / div) for k, v in equation.items()}
-
-    return equation
+            is_reactant = False
+    return left, right
 
 
 @tr.signature_has_traits
 class ActionMassKinetics(tr.HasTraits):
     """
     An object which stores a reaction network of elementary reactions.
 
     It stores its rate parameterization, initial concentrations, temperature profile,
     with methods for evaluating production rates and concentration profiles assuming
     action mass kinetic and closed reactor.
 
     Parameters
     ----------
-    equations : `list` or `tuple` of `str`
-        Strings giving the ``n_equations`` chemical equation of the network.
+    reactions : 'dict' or `list` or `tuple` of `str`
+        Strings giving the ``n_reactions`` chemical equation of the network.
         Reactants and products must be separated by a ``"->"`` or "→" symbol,
         The name of each species should match a key of the `species` dictionary.
-        Examples: ``"A + B -> C"`` or ``"2A -> 0.5 D"``\
+        Examples: ``"A + B -> C"`` or ``"2A -> D"``\
     species : `dict`, optional
         Dictionary of initial concentrations for the `n_species` species.
-    k : :term:`array-like`
-        Iterable of shape `n_equations` x 2 with the Arrhenius rate parameters
-        ((:math:`A_1`\ , :math:`Ea_1`\ ), ... (:math:`A_n`\ , :math:`Ea_n`\ )).
-    T : `float`, `Quantity` or `callable`\ , optional, default: 298.0
-        Temperature. If it is not a temperature quantity, the unit is assumed to be
-        in Kelvin. A function can also be provided which output a temperature `T`
+    arrhenius : :term:`array-like`
+        Iterable of shape `n_reactions` x 1, `n_reactions` x 2  or `n_reactions` x 3
+        with either the isothermal rate constants (:math:`k_1`\ , ..., :math:`k_n`\ ) or
+        the Arrhenius rate parameters ((:math:`A_1`\ , :math:`b_1`\ , :math:`Ea_1`\ ),
+        ... (:math:`A_n`\ , :math:`b_n`\ , :math:`Ea_n`\ )) or  ((:math:`A_1`\ ,
+        :math:`Ea_1`\ ), ...)).  If a 2-column iterable is provided the temperature
+        exponents are set to 0.
+    T : `float`\ , `Quantity`\ , `callable` or None, optional, default: None
+        Temperature. If None, the system is considered isothermal and T = 298.0
+        If it is not a temperature quantity, the unit is assumed to be
+        in Kelvin. A function can also be provided which output a temperature `T` in K
         vs. time `t`\ .
     """
 
     # internal parameters
-    _equations = tr.List(tr.Unicode(), help="List of model equations")
-    _concentrations = tr.Dict(help="A dictionary of model's species:concentrations")
+    _reactions = tr.Union(
+        (tr.List(tr.Unicode()), tr.Dict()), help="List or dict of model reactions"
+    )
+    _reactions_names = tr.List(tr.Unicode(), help="List of model reactions names")
+    _init_concentrations = tr.Dict(
+        help="A dictionary of model's species: initial " "concentrations"
+    )
     _species = tr.List(help="a list of species in this model")
-    _M = Array(help="Stoichiometric matrix M = A+B")
-    _k = Array(help="Arrhenius rate")
-    _T = tr.Union((tr.Float(), tr.Callable()), default_value=298.0, help="Temperature")
-
-    def __init__(self, equations, species, k, T=298.0, **kwargs):
+    _A = Array(help="Stoichiometric matrix A (reactants)")
+    _B = Array(help="Stoichiometric matrix B (products)")
+    _arrhenius = Array(help="Arrhenius-like rate constant parameters")
+    _T = tr.Union(
+        (tr.Float(), tr.Callable()),
+        allow_none=False,
+        default_value=298.0,
+        help="Temperature",
+    )
+
+    def __init__(self, reactions, species_concentrations, arrhenius, T=298.0, **kwargs):
+
+        # initialise concentrations, species, reactions, arrhenius, T
+        self._init_concentrations = species_concentrations
+        self._species = list(self._init_concentrations.keys())
+
+        if isinstance(reactions, (list, tuple)):
+            self._reactions = reactions
+            self._reactions_names = [f"equation {i}" for i in range(len(reactions))]
+        if isinstance(reactions, dict):
+            self._reactions = list(reactions.values())
+            self._reactions_names = list(reactions.keys())
 
-        self._k = k
+        self._arrhenius = arrhenius
         self._T = T
 
-        # initialise concentrations, species and equations
-        self._concentrations = species
-        self._species = list(self._concentrations.keys())
-        self._equations = equations
+        self._reaction_rates = self._write_reaction_rates()
+        self._production_rates = self._write_production_rates()
+        self._jacobian = self._write_jacobian()
 
     # ----------------------------------------------------------------------------------
     # Private methods
     # ----------------------------------------------------------------------------------
-    @tr.validate("_k")
-    def _k_validate(self, proposal):
-        # k must be an iterable of pairs (A_1, Ea_1)
-        k = proposal.value
-        # k is an array (even if a list or tuple has been initialy provided (Array)
-        if k.shape[-1] != 2:
-            raise ValueError("k must be an iterable of pairs: shape=(n_reactions, 2)")
-        # Add more validation?
-        # ...
-        return k
+    @tr.validate("_arrhenius")
+    def _arrhenius_validate(self, proposal):
+        # arrhenius can be an iterable of:
+        # - single k values (k_1, ... k_n)
+        # - pairs of arrhenius parameters ((A_1, Ea_1), ... (A_n, E_a_n))
+        # - triplets of arrhenius parameters  ((A_1, b_1, Ea_1), ... (A_n, b_n, E_a_n))
+        arrhenius = proposal.value
+        # k is an array (even if a list or tuple has been initially provided (Array)
+        if len(arrhenius.shape) == 1:
+            # this id a 1D array
+            if arrhenius.shape[-1] != self.n_reactions:
+                raise ValueError(
+                    f"arrhenius should contain {self.n_reactions} rate "
+                    f"constants, {arrhenius.shape[-1]} have been provided"
+                )
+            if any(arrhenius < 0):
+                warnings.warn(
+                    "at least a rate constant is negative... are you sure of " "that ?!"
+                )
+        elif arrhenius.shape[-1] == 2:
+            # this is a 2D array with lines == [A, Ea]
+            if arrhenius.shape[0] != self.n_reactions:
+                raise ValueError(
+                    f"arrhenius should contain {self.n_reactions} rate "
+                    f"constants, {arrhenius.shape[0]} have been provided"
+                )
+            if (arrhenius < 0).any():
+                warnings.warn(
+                    "a least a pre-exp factor or activation energy is "
+                    "negative... ae you sure of that ?!"
+                )
+            # now add temperature exponents = 0
+            arrhenius = np.array(
+                [arrhenius[:, 0].T, np.zeros(arrhenius.shape[0]).T, arrhenius[:, 1].T]
+            ).T
+        elif arrhenius.shape[-1] == 3:
+            # this is a 2D array with lines == [A, b, Ea]
+            if arrhenius.shape[0] != self.n_reactions:
+                raise ValueError(
+                    f"arrhenius should contain {self.n_reactions} rate "
+                    f"constants, {arrhenius.shape[0]} have been provided"
+                )
+            if (arrhenius[:, [0, 2]] < 0).any():
+                warnings.warn(
+                    "a least a pre-exp factor or activation energy is "
+                    "negative... are you sure of that ?!"
+                )
+        return arrhenius
 
     @tr.validate("_T")
     def _T_validate(self, proposal):
         Tp = proposal.value
-
         if isinstance(Tp, Quantity):
-            Tp = Tp.to("K").magnitude
-
-        if isinstance(Tp, float):
-            # if T float, transform it to a callable
-            T = lambda t: Tp
+            T = Tp.to("K").magnitude
         else:
             T = Tp
         return T
 
-    @tr.observe("_equations")
+    @tr.observe("_reactions")
     def _stoichio_matrix(self, change):
         # generate stoichio matrix
-        equations = change.new
-        M = np.zeros((self.n_equations, self.n_species))
-        for i, eq in enumerate(equations):
-            equation = _interpret_equation(eq, self._species)
-            # fill M matrix in the order of the species list
-            M[i] = [equation[k] if k in equation else 0 for k in self._species]
-        self._M = M
+        reactions = change.new
+        A = np.zeros((self.n_reactions, self.n_species))
+        B = np.zeros((self.n_reactions, self.n_species))
+        for i, eq in enumerate(reactions):
+            left, right = _interpret_equation(eq, self._species)
+            A[i] = [left[k] if k in left else 0 for k in self._species]
+            B[i] = [right[k] if k in right else 0 for k in self._species]
+        self._A = A
+        self._B = B
+        self._BmAt = (B - A).T
 
     # ----------------------------------------------------------------------------------
     # Public properties
     # ----------------------------------------------------------------------------------
     @property
     def A(self):
         """
         Stoichiometry matrix A
 
         Stoichiometry matrices `A` and `B` are defined in :cite:t:`chellaboina:2009`\ .
         """
-        return (-self._M).clip(0)
+        return self._A
 
     @property
     def B(self):
         """
         Stoichiometry matrix B
 
         Stoichiometry matrices `A` and `B` are defined in :cite:t:`chellaboina:2009`\ .
         """
-        return self._M.clip(0)
+        return self._B
 
     @property
-    def n_equations(self):
-        """Number of reaction equations"""
-        return len(self._equations)
+    def n_reactions(self):
+        """Number of reaction reactions"""
+        return len(self._reactions)
 
     @property
     def n_species(self):
         """Number of species"""
         return len(self._species)
 
     @property
     def species(self):
         """Components names."""
-        return list(self._concentrations.keys())
+        return list(self._init_concentrations.keys())
 
     @property
-    def concentrations(self):
+    def init_concentrations(self):
         """Concentrations."""
-        return list(self._concentrations.values())
+        return list(self._init_concentrations.values())
 
-    def integrate(self, t, method="RK45", **kwargs):
+    def _write_reaction_rates(self):
+        """Return the expressions of production rates as a string"""
+        block = "["
+        for j, line in enumerate(self._A):
+            reac_rate = f"k[{j}]"
+            for k, nu in enumerate(line):
+                if nu == 1:
+                    reac_rate += f" * C[{k}]"
+                elif nu > 1:
+                    reac_rate += f" * C[{k}]**{nu}"
+            reac_rate += ", "
+            block += reac_rate
+        block += "]"
+        return block
+
+    def _print_reaction_rates(self):
+        print(self._write_reaction_rates().replace(",", ",\n"))
+
+    def _write_production_rates(self):
+        """Return the expressions of production rates as a string"""
+        block = "["
+        for line in (self._B - self._A).T:
+            prod_rate = ""
+            if not line.any():
+                # only zeors => spectator species
+                prod_rate = "0"
+            else:
+                for j, n in enumerate(line):
+                    if n != 0:
+                        if n == 1:
+                            prod_rate += f" + k[{j}]"
+                        elif n == -1:
+                            prod_rate += f" - k[{j}]"
+                        elif n > 1:
+                            prod_rate += f" + {n} * k[{j}]"
+                        elif n < -1:
+                            prod_rate += f" {n} * k[{j}]"
+
+                        for k, nu in enumerate(self.A[j]):
+                            if nu == 1:
+                                prod_rate += f" * C[{k}]"
+                            elif nu > 1:
+                                prod_rate += f" * C[{k}]**{nu}"
+            prod_rate += ", "
+            block += prod_rate
+        block += "]"
+        return block
+
+    def _print_production_rates(self):
+        print(self._write_production_rates().replace(",", ",\n"))
+
+    def _write_jacobian(self):
+        """Return the expressions of the jacobian of the production rates as a string"""
+        block = "["
+        for i, line in enumerate((self._B - self._A).T):
+            jac = "["
+            for j in range(self.n_species):
+                # compute jac[i,j] = d(dCidt)/dCj
+                is_null = True
+                for k, n in enumerate(line):
+                    if self.A[k, j] > 0 and n != 0:
+                        # the stoichiometruc coef. of reactant j is non-null
+                        # and reactant i is involved
+                        is_null = False
+                        if n == 1:
+                            jac += f" + k[{k}]"
+                        elif n == -1:
+                            jac += f" - k[{k}]"
+                        elif n > 1:
+                            jac += f" + {n} * k[{j}]"
+                        elif n < -1:
+                            jac += f" {n} * k[{j}]"
+
+                        for jj, nu in enumerate(self.A[k]):
+                            if nu == 1:
+                                jac += f" * C[{jj}]" if jj != j else ""
+                            elif nu > 1:
+                                jac += (
+                                    f" * C[{jj}]**{nu}"
+                                    if jj != j
+                                    else f" * {nu} * C[{jj}]**{nu-1}"
+                                )
+                if is_null:
+                    jac += "0,"
+                else:
+                    jac += ", "
+            block += jac + " ],"
+        block += "]"
+        return block
+
+    def _print_jacobian(self):
+        print(self._write_jacobian().replace(" ],", "],\n"))
+
+    def integrate(
+        self,
+        t,
+        k_dt=None,
+        method="LSODA",
+        left_op=None,
+        c_names=None,
+        use_jac=False,
+        atol=1e-6,
+        rtol=1e-3,
+        **kwargs,
+    ):
         """
         Integrate the kinetic equations at times `t`.
 
         This function computes and integrates the set of kinetic differential
-        equations given the initial concentration values:
-
-        .. math::
-            dC / dt =  (B - A).T  K C^A
-
-            C(t_0) = C_0
-
-        where :math:`A` and :math:`B` are the stoichiometry matrices,
-        :math:`K` is the diagonal matrix of rate constants and :math:`C^A` is the
-        vector-matrix exponentiation of :math:`C` by :math:`A`\ .
+        equations given the initial concentration values.
 
         Parameters
         ----------
         t : :term:`array-like` of shape (``t_points``\ ,)
             Iterable with time values at which the concentrations are computed.
-        method : `str` or `~scipy.integrate.OdeSolver`\ , optional, default: ``'RK45'``
+
+        k_dt : `float` or `None'
+            Resolution of the time grid used to compute `k(T(t))`\ . Used only for non
+            isothermal reaction.
+
+        method : `str` or `~scipy.integrate.OdeSolver`\ , optional, default: ``'LSODA'``
             Integration method to use:
 
+            * ``'LSODA'`` (default): Adams/BDF method with automatic stiffness detection and
+              switching.
             * ``'RK45'`` (default): Explicit Runge-Kutta method of order 5(4).
             * ``'RK23'`` : Explicit Runge-Kutta method of order 3(2).
             * ``'DOP853'``: Explicit Runge-Kutta method of order 8.
             * ``'Radau'`` : Implicit Runge-Kutta method of the Radau IIA family of
               order 5.
             * ``'BDF'`` : Implicit multi-step variable-order (1 to 5) method based
               on a backward differentiation formula for the derivative
               approximation.
-            * ``'LSODA'`` : Adams/BDF method with automatic stiffness detection and
-              switching.
 
-            Explicit Runge-Kutta methods ('RK23', 'RK45', 'DOP853') should be used
+            'LSODA' is generally faster and seems a good choice for the systems
+            treated in scpy so far.
+            Explicit Runge-Kutta methods ('RK23', 'RK45', 'DOP853') can be used
             for non-stiff problems and implicit methods ('Radau', 'BDF') for
             stiff problems. Among Runge-Kutta methods, 'DOP853' is recommended
             for solving with high precision (low values of `rtol` and `atol` ).
             If not sure, first try to run 'RK45'. If it makes unusually many
             iterations, diverges, or fails, your problem is likely to be stiff and
-            you should use 'Radau' or 'BDF'. 'LSODA' can also be a good universal
-            choice, but it might be somewhat less convenient to work with as it
-            wraps old Fortran code.
+            you should use 'Radau' or 'BDF'.
             You can also pass an arbitrary class derived from
             `~scipy.integrate.OdeSolver` which implements the solver.
+
+        left_op : array_like, optional
+            A (m x n_species) array to left multiply the (n_species, n_times) array
+            obtained after integration:
+            `C.T = left_op @ C.T`\ . Can be used to pool and/or remove some
+            concentration profiles in/from the output matrix of concentrations
+
+        c_names : list of str
+            List of names for each concentration profile. Used if `left_op` is not None
+            to name/rename the output concentration profiles.
+
+        use_jac : `Bool`
+            Whether to use the jacobian. Useful for stiff problems, can slightly
+            increase the execution time for non-stiff problems.
+
+        atol, rtol : `float` or `array_like`, optional
+            Relative and absolute tolerances. The solver keeps the local error estimates
+            less than `atol + rtol * abs(y)`. Here `rtol` controls a relative accuracy
+            (number of correct digits), while `atol` controls absolute accuracy
+            (number of correct decimal places). To achieve the desired `rtol`, set
+            `atol < min(rtol * C)` so that `rtol` dominates the allowable error.
+            If `atol > rtol * C` the number of correct digits is not guaranteed.
+            Conversely, to achieve the desired `atol` set `rtol` such that
+            `max(rtol * C) < atol` is always smaller than atol. If components of C have
+            different scales, it might be beneficial to set different atol values for
+            different components by passing array_like with shape (n_species,) for
+            atol. Default values are `rtol=1e-3` and `atol=1e-6`\ .
+
         **kwargs
             Additional keyword parameters. See Other Parameters.
 
         Other Parameters
         ----------------
         return_NDDataset : `bool`\ , optional, default: `True`
             Whether to return a NDDataset
@@ -288,85 +504,197 @@
 
                     *  0 : The solver successfully reached the end of `tspan` .
                     *  1 : A termination event occurred.
 
             * message : `str`
               Human-readable description of the termination reason.
         """
+        # uncomment for debugging and optimization
+        # import time
+        # t0 = time.time()
+
+        global_env = {}
+        locals_env = {}
+
+        if callable(self._T):
+            # non-isothermal: a grid of k_i values spaced by k_dt time intervals
+            # is computed
+            t_grid = np.arange(0, t[-1] + k_dt, k_dt)
+            T_grid = np.expand_dims(self._T(t_grid), axis=1)
+            k_grid = (
+                self._arrhenius[:, 0]
+                * np.power(T_grid, self._arrhenius[:, 1])
+                * np.exp(-self._arrhenius[:, 2] / 8.314 / T_grid)
+            )
 
-        def production_rates(ti, Ci):
-            """
-            Compute the production rates :math:`\frac{dC,dt}`.
-
-            Compute the n_s production rates at time :math:`t_i` according to:
-
-            .. math::
-                dC / dt =  (B - A).T  K C_i^A
-                C_i = C(t_i)
-
-            where :math:`A` and :math:`B` are the stoichiometry matrices, :math:`K` is
-            the diagonal matrix of rate constants and :math:`C_i^A` is the vector-matrix
-            exponentiation of :math:`C_i` by :math:`A`.
-
-            Parameters
-            ----------
-            ti: `float`
-                Time.
-            Ci: `~numpy.ndarray`
-                1D vector of the concentrations at time `ti`\ .
-            """
-            beta = 1 / R / self._T(ti)
-            K = np.diag(self._k[:, 0] * np.exp(-beta * self._k[:, 1]))
-            A, B = self.A, self.B
-            BmAt = (B - A).T
-            return np.dot(np.dot(BmAt, K), _vm_exp(Ci, A))
-
-        bunch = solve_ivp(
-            production_rates,
-            (t[0], t[-1]),
-            self.concentrations,
-            t_eval=t,
-            method=method,
-        )
+            # uncomment for debugging and optimization
+            # t1 = time.time()
+
+            exec(
+                f"def f_(self, k_grid, k_dt, t, C): k = k_grid[int(t/k_dt)] ; return self._BmAt @ {self._reaction_rates}",
+                global_env,
+                locals_env,
+            )
+
+            if use_jac:
+                # define jac_ = d[dC/dt]/dCi
+                exec(
+                    f"def jac_(self, k_grid, k_dt, t, C): k = k_grid[int(t/k_dt)] ; return{self._jacobian}",
+                    global_env,
+                    locals_env,
+                )
+                jac = partial(locals_env["jac_"], self, k_grid, k_dt)
+            else:
+                jac = None
+
+            # uncomment for debugging and optimization
+            # t2 = time.time()
+
+            bunch = solve_ivp(
+                partial(locals_env["f_"], self, k_grid, k_dt),
+                (t[0], t[-1]),
+                self.init_concentrations,
+                t_eval=t,
+                method=method,
+                atol=atol,
+                rtol=rtol,
+                jac=jac,
+            )
+
+            # uncomment for debugging and optimization
+            # t3 = time.time()
+
+        else:
+            if len(self._arrhenius.shape) == 1:
+                # _arrhenius is 1D array of rate constants
+                k = self._arrhenius
+
+                # uncomment for debugging and optimization
+                # t1 = time.time()
+
+            else:
+                # isothermal, the k_i are computed once
+                k = (
+                    self._arrhenius[:, 0]
+                    * self._T ** self._arrhenius[:, 1]
+                    * np.exp(-self._arrhenius[:, 2] / R / self._T)
+                )
+
+            # uncomment for debugging and optimization
+            # t1 = time.time()
+
+            exec(
+                f"def f_(self, k, t, C): return{self._production_rates}",
+                global_env,
+                locals_env,
+            )
+            if use_jac:
+                # define jac_ = d[dC/dt]/dCi
+                exec(
+                    f"def jac_(self, k, t, C): return{self._jacobian}",
+                    global_env,
+                    locals_env,
+                )
+                jac = partial(locals_env["jac_"], self, k)
+            else:
+                jac = None
+
+            # uncomment for debugging and optimization
+            # t2 = time.time()
+
+            bunch = solve_ivp(
+                partial(locals_env["f_"], self, k),
+                (t[0], t[-1]),
+                self.init_concentrations,
+                t_eval=t,
+                method=method,
+                atol=atol,
+                rtol=rtol,
+                jac=jac,
+            )
+
+            # uncomment for debugging and optimization
+            # t2 = time.time()
+
+        # uncomment for debugging (warning: debug_() multiply the exec time by 4...)
+        # from from spectrochempy.core import debug_
+        # debug_(bunch.message)
+        # t4 = time.time()
 
-        debug_(bunch.message)
         if bunch.status != 0:
             raise SolverError(bunch.message)
 
-        C = bunch.y.T
+        C = (left_op @ bunch.y).T if left_op is not None else bunch.y.T
         t = bunch.t
 
-        # remove some keys from bunch
-        del bunch.y
-        del bunch.success
+        # uncomment for debugging and optimization
+        # t5 = time.time()
 
         return_dataset = kwargs.get("return_NDDataset", True)
         if return_dataset:
             C = NDDataset(C, name="Concentrations")
             C.y = Coord(t, title="time")
-            C.x = Coord(range(self.n_species), labels=self.species, title="species")
+            if left_op is None:
+                C.x = Coord(range(self.n_species), labels=self.species, title="species")
+            elif c_names is not None:
+                C.x = Coord(range(left_op.shape[0]), labels=c_names, title="species")
+            else:
+                C.x = Coord(
+                    range(left_op.shape[0]),
+                    labels=[f"species #{i}" for i in range(left_op.shape[0])],
+                    title="species",
+                )
             C.history = "Created using ActionMassKinetics.integrate"
             C.meta.update(bunch)
 
+        # uncomment for debugging and optimization
+        # t6 = time.time()
+        # print(f"time compute k       : {t1 - t0:f}, {100*(t1 - t0)/(t6-t0):f}%")
+        # print(f"time load f (and jac): {t2 - t1:f}, {100*(t2 - t1)/(t6-t0):f}%")
+        # print(f"time integration     : {t3 - t2:f}, {100*(t3 - t2)/(t6-t0):f}%")
+        # print(f"time debug           : {t4 - t3:f}, {100*(t4 - t3)/(t6-t0):f}%")
+        # print(f"time C,t             : {t5 - t4:f}, {100*(t5 - t4)/(t6-t0):f}%")
+        # print(f"time to NDDataset    : {t6 - t5:f}, {100*(t6 - t5)/(t6-t0):f}%")
+
         if kwargs.get("return_meta", False) and not return_dataset:
             return (C, bunch)
-        return C
+        else:
+            return C
 
-    def _modify_kinetics(self, dict_param):
-        for item in dict_param:
-            i_r, p = item.split("[")[-1].split("].")
-            if p == "A":
-                self._k[int(i_r), 0] = dict_param[item]
-            elif p == "Ea":
-                self._k[int(i_r), 1] = dict_param[item]
-            else:
-                raise ValueError("something went wrong in parsing the dict of params")
+    def _modify_kinetics(self, dict_param, left_op=None):
+
+        if len(self._arrhenius.shape) == 2:
+            for item in dict_param:
+                i_r, p = item.split("[")[-1].split("].")
+                if p == "A":
+                    self._arrhenius[int(i_r), 0] = dict_param[item]
+                elif p == "b":
+                    self._arrhenius[int(i_r), 1] = dict_param[item]
+                elif p == "Ea":
+                    self._arrhenius[int(i_r), 2] = dict_param[item]
+                else:
+                    raise ValueError(
+                        "something went wrong in parsing the dict of params"
+                    )
+        else:
+            for item in dict_param:
+                i_r = item.split("[")[-1].split("]")[0]
+                self._arrhenius[int(i_r)] = dict_param[item]
+
+        if left_op is not None:
+            self._arrhenius = left_op @ self._arrhenius
 
     def fit_to_concentrations(
-        self, Cexp, iexp, i2iexp, dict_param_to_optimize, **kwargs
+        self,
+        Cexp,
+        iexp,
+        i2iexp,
+        dict_param_to_optimize,
+        ivp_solver_kwargs={},
+        optimizer_kwargs={},
     ):
         """
         Fit rate parameters and concentrations to a concentration profile.
 
         Parameters
         ------------
         Cexp : `NDDataset`
@@ -374,112 +702,136 @@
             `Cexp` can contain more concentration profiles than those to fit.
         iexp : `int`
             Indexes of experimental concentration profiles on which the model will be
             fitted.
         i2iexp : `int`
             Correspondence between optimized (external) concentration profile and
             experimental concentration profile.
-        dict_param_to_optimize : `dict`
+        dict_param_to_optimize : `dict` or None
             rate parameters to optimize. Keys should be 'k[i].A' and 'k[i].Ea' for
             pre-exponential factor.
-        **kwargs
-            Parameters for the optimization (see `~scipy.optimize.minimize`\ ).
+        ivp_solver_kwargs : `dict`
+            keyword arguments for the ode solver. Defaults are the same as for
+            `~scipy.integrate.solve_ivp`\ , except for `method=LSDOA`
+        optimizer_kwargs: `dict`
+            keyword arguments the optimization (see `~scipy.optimize.minimize`\ ).
 
         Returns
         --------
         `dict`
             A result dictionary.
         """
 
-        def objective(params, Cexp, iexp, i2iexp, dict_param_to_optimize):
+        def objective(
+            params,
+            Cexp,
+            iexp,
+            i2iexp,
+            dict_param_to_optimize,
+            optimizer_left_op,
+            ivp_solver_method,
+            k_dt,
+            C_op,
+        ):
+            """returns the SSE on concentrationb profiles"""
+
             for param, item in zip(params, dict_param_to_optimize):
                 dict_param_to_optimize[item] = param
-            self._modify_kinetics(dict_param_to_optimize)
-            Chat = self.integrate(Cexp.y.data, return_NDDataset=False)
+
+            self._modify_kinetics(dict_param_to_optimize, optimizer_left_op)
+
+            Chat = self.integrate(
+                Cexp.y.data,
+                return_NDDataset=False,
+                method=ivp_solver_method,
+                k_dt=k_dt,
+                left_op=C_op,
+            )
             return np.sum(np.square(Cexp.data[:, iexp] - Chat[:, i2iexp]))
 
-        method = kwargs.get("method", "Nelder-Mead")
-        bounds = kwargs.get("bounds", None)
-        tol = kwargs.get("tol", None)
-        options = kwargs.get("options", {"disp": True})
+        # optimizer (kw)arguments:
+        # ... parameters for scipy.minimize
+        optimizer_method = optimizer_kwargs.get("Method", "Nelder-Mead")
+        optimizer_bounds = optimizer_kwargs.get("bounds", None)
+        optimizer_tol = optimizer_kwargs.get("tol", None)
+        optimizer_options = optimizer_kwargs.get("options", {"disp": True})
+        # optimizer_callback = optimizer_kwargs.get("callback", None)
+        # ... other parameters
+        optimizer_left_op = optimizer_kwargs.get("left_op", None)
+
+        # ivp solver (kw)arguments:
+        # ... parameters for integrate.ivp_solve
+        ivp_solver_method = ivp_solver_kwargs.get("method", "LSODA")
+        # ... other parameters
+        ivp_solver_k_dt = ivp_solver_kwargs.get("k_dt", None)
+        ivp_solver_left_op = ivp_solver_kwargs.get("left_op", None)
 
-        guess_param = np.zeros((len(dict_param_to_optimize)))
+        # get x0
+        x0 = np.zeros(len(dict_param_to_optimize))
         for i, param in enumerate(dict_param_to_optimize):
-            guess_param[i] = dict_param_to_optimize[param]
+            x0[i] = dict_param_to_optimize[param]
 
-        if options["disp"]:
-            print("Optimization of the parameters.")
-            print(f"         Initial parameters: {guess_param}")
-            print(
-                f"         Initial function value: "
-                f"{objective(guess_param, Cexp, iexp, i2iexp, dict_param_to_optimize)}"
+        if optimizer_options["disp"]:
+            init_val = objective(
+                x0,
+                Cexp,
+                iexp,
+                i2iexp,
+                dict_param_to_optimize,
+                optimizer_left_op,
+                ivp_solver_method,
+                ivp_solver_k_dt,
+                ivp_solver_left_op,
             )
+            print("Optimization of the parameters.")
+            print(f"         Initial parameters: {x0}")
+            print(f"         Initial function value: {init_val:f}")
         tic = datetime.datetime.now(datetime.timezone.utc)
+
         optim_res = minimize(
             objective,
-            guess_param,
-            args=(Cexp, iexp, i2iexp, dict_param_to_optimize),
-            method=method,
-            bounds=bounds,
-            tol=tol,
-            options=options,
+            x0,
+            args=(
+                Cexp,
+                iexp,
+                i2iexp,
+                dict_param_to_optimize,
+                optimizer_left_op,
+                ivp_solver_method,
+                ivp_solver_k_dt,
+                ivp_solver_left_op,
+            ),
+            method=optimizer_method,
+            bounds=optimizer_bounds,
+            tol=optimizer_tol,
+            options=optimizer_options,
         )
         toc = datetime.datetime.now(datetime.timezone.utc)
-        opt_param = optim_res.x
-        if options["disp"]:
+
+        if optimizer_options["disp"]:
             print(f"         Optimization time: {toc - tic}")
-            print(f"         Final parameters: {opt_param}")
+            print(f"         Final parameters: {optim_res['x']}")
 
-        Ckin = self.integrate(Cexp.y.data, return_NDDataset=False)
+        Ckin = self.integrate(
+            Cexp.y.data,
+            return_NDDataset=False,
+            method=ivp_solver_method,
+            k_dt=ivp_solver_k_dt,
+            left_op=ivp_solver_left_op,
+        )
 
         for i, param in enumerate(dict_param_to_optimize):
-            dict_param_to_optimize[param] = opt_param[i]
+            dict_param_to_optimize[param] = optim_res["x"][i]
 
         return Ckin, (iexp, i2iexp, dict_param_to_optimize), optim_res
 
 
-def _vm_exp(x: Iterable, A: Iterable):
-    """
-    Vector matrix exponentiation
-
-    The vector-matrix exponentiation is the operation that maps x
-    and A to its vector-matrix power $x^A$ which given by:
-    $$ \left[ x_1^{A_{11}}x_2^{A_{21}} ... x_n^{A_{n1}} \;\; x_1^{A_{1n}}x_2^{A_{2n}}
-    ... x_n^{A_{nn}} \right]$$
-
-
-    Parameters
-    ----------
-    x: (px1) iterable of float
-         Columns vector
-    A: (pxq) iterable of int
-         Matrix
-
-    Returns
-    -------
-    Vm_exp: (px1) iterable
-         x^A vector
-
-    References
-    ----------
-    [1] Chellaboina et al., "Modeling and analysis of mass-action kinetics", IEEE
-        control systems (2009),DOI: 10.1109/MCS.2009.932926
-    [2] Gjerrit Meinsma, "Dimensional and Scaling Analysis" SIAM review, Vol. 61, No. 1,
-        pp. 159–184 (2009), DOI: 10.1137/16M1107127
-    """
-    out = [1] * len(A)
-    for i, A_i in enumerate(A):
-        for x_j, A_ij in zip(x, A_i):
-            out[i] *= x_j**A_ij
-    return out
-
-
-# --------
+# ------------------------------------------------------------------------------------
 # CANTERA UTILITIES
-# -------
+# ------------------------------------------------------------------------------------
 ct = import_optional_dependency("cantera", errors="ignore")
 
 
 def _cantera_is_not_available():
     if ct is None:
         error_(
             ImportError,
@@ -989,30 +1341,15 @@
                 return se
 
         method = kwargs.get("method", "Nelder-Mead")
         bounds = kwargs.get("bounds", None)
         tol = kwargs.get("tol", None)
         options = kwargs.get("options", {"disp": True})
 
-        if method in [
-            "Nelder-Mead",
-            "Powell",
-            "CG",
-            "BFGS",
-            "Newton-CG",
-            "L-BFGS-B",
-            "TNC",
-            "COBYLA",
-            "SLSQP",
-            "trust-constr",
-            "dogleg",
-            "trust-ncg",
-            "trust-krylov",
-            "trust-exact",
-        ]:
+        if method.upper() in SCIPY_MINIMIZE_METHODS:
             optimizer = "minimize"
 
         elif method in ["trf", "dogbox", "lm"]:
             optimizer = "least_squares"
             if bounds is None:
                 bounds = (-np.inf, np.inf)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/linearregression.py` & `spectrochempy-0.6.4/spectrochempy/analysis/linearregression.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.4/spectrochempy/analysis/mcrals.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 - ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc``
 - ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc,
   extraOutputGetConc``
 
 with:
 
 - ``Ccurr`` is the current `C` dataset,
-- ``\*argsGetConc`` are the parameters needed to completely specify the function.
+- ``argsGetConc`` are the parameters needed to completely specify the function.
 - ``hardC`` is a `~numpy.ndarray` or `NDDataset` of shape
   (:term:`n_observations` , len(``hardConc``\ ),
 - ``newArgsGetConc`` are the updated parameters for the next iteration (can be `None`),
 - ``extraOutputGetConc`` can be any other relevant output to be kept in
   ``extraOutputGetConc`` attribute, a list of ``extraOutputGetConc`` at each MCR ALS
   iteration.
 
@@ -318,22 +318,23 @@
         help="Supplementary keyword arguments passed to the external function.",
     ).tag(config=True)
 
     getC_to_C_idx = tr.Union(
         (tr.Enum(["default"]), tr.List()),
         default_value="default",
         help=(
-            r"""Correspondence of the profiles returned by `getConc` and `C`.
+            r"""Correspondence of the profiles returned by `getConc`
+and `C[:,hardConc]`\ .
 
-- ``'default'``: the profiles correspond to those of `C`. This is equivalent to
-  ``range(len(hardConc))``
-- `list` of indexes or of `None`. For instance ``[2, None, 0]`` indicates that the
-  first returned profile corresponds to the 3rd profile of `C`  (index ``2``\ ), the 2nd
-  returned profile does not correspond to any profile in `C`, the 3rd returned profile
-  corresponds to the first `C` profile (index ``0`` )."""
+- ``'default'``: the profiles correspond to those of `C[:,hardConc]`. This is equivalent
+  to ``range(len(hardConc))``
+- `list` of indexes or of `None`. For instance ``[2, 1, 0]`` indicates that the
+  third profile returned by `getC` (index ``2``\ ) corresponds to the 1st profile of
+  `C[:, hardConc]`\ , the 2nd returned profile (index ``1``\ ) corresponds to
+  second profile of `C[:, hardConc]`, etc..."""
         ),
     ).tag(config=True)
 
     solverSpec = tr.Enum(
         ["lstsq", "nnls", "pnnls"],
         default_value="lstsq",
         help=(
@@ -717,16 +718,17 @@
             return proposal.value
         getC_to_C_idx = proposal.value
         if not self._n_components:  # not initialized or 0
             return getC_to_C_idx
         if getC_to_C_idx == "default":
             getC_to_C_idx = np.arange(self._n_components).tolist()
         elif (
-            len(getC_to_C_idx) > self._n_components
-            or max(getC_to_C_idx) + 1 > self._n_components
+            len(getC_to_C_idx)
+            > self._n_components
+            #   or max(getC_to_C_idx) + 1 > self._n_components
         ):
             raise ValueError(
                 f"The profile has only {self._n_components} species, please check "
                 f"the `getC_to_C_idx`  configuration (value:{getC_to_C_idx})"
             )
         return getC_to_C_idx
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/nmf.py` & `spectrochempy-0.6.4/spectrochempy/analysis/nmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     )
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # ----------------------------------------------------------------------------------
 
     n_components = tr.Integer(
-        default_value=None,
+        default_value=2,
         allow_none=True,
-        help="Number of components to use. If None is passed, all are used.",
+        help="Number of components to use.",
     ).tag(config=True)
 
     init = tr.Enum(
         ["random", "nndsvd", "nndsvda", "nndsvdar", "custom"],
         default_value=None,
         allow_none=True,
         help=(
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/optimize/__init__.py` & `spectrochempy-0.6.4/spectrochempy/analysis/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/optimize/_models.py` & `spectrochempy-0.6.4/spectrochempy/analysis/optimize/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 This module holds the definitions all the various models.
 """
 from functools import wraps
 
 import numpy as np
 
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.units import Quantity
 
 __all__ = [
     "polynomialbaseline",
     "gaussianmodel",
     "lorentzianmodel",
@@ -75,15 +75,15 @@
             ampl_units = newargs[0].units
             newargs[0] = newargs[0].m
 
         _data = func(cls, x, *newargs)
 
         if returntype == "NDDataset":
             res = NDDataset(_data, units=ampl_units)
-            res.x = LinearCoord(xinput)
+            res.x = Coord(xinput)
             res.name = cls.__class__.__name__.split("model")[0]
             res.title = "intensity"
 
         else:
             res = _data
             if ampl_units:
                 res = res * ampl_units
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/optimize/_parameters.py` & `spectrochempy-0.6.4/spectrochempy/analysis/optimize/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/optimize/optimize.py` & `spectrochempy-0.6.4/spectrochempy/analysis/optimize/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 
-__all__ = ["Optimize"]
-__configurables__ = __all__
-
 import re
 import sys
 
 import numpy as np
 import scipy.optimize
 import traitlets as tr
 from IPython import display
@@ -38,17 +35,14 @@
 
     Parameters
     ----------
     %(AnalysisConfigurable.parameters)s
     """
     )
 
-    name = "Optimize"
-    description = "Non-linear Least-Squares Optimization"
-
     # ----------------------------------------------------------------------------------
     # Configuration parameters (mostly defined in subclass
     # as they depend on the model estimator)
     # ----------------------------------------------------------------------------------
     max_iter = tr.Integer(
         default_value=500, help="Maximum number of fitting iteration."
     ).tag(config=True)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.4/spectrochempy/analysis/pca.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.4/spectrochempy/analysis/peakfinding.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from datetime import datetime, timezone
 
 import numpy as np
 import scipy
 
 from spectrochempy.core.dataset.coord import Coord
+from spectrochempy.core.units import Quantity
 
 # Todo:
 # find_peaks_cwt(vector, widths[, wavelet, ...]) Attempt to find the peaks in a 1-D array.
 # argrelmin(data[, axis, order, mode]) 	Calculate the relative minima of data.
 # argrelmax(data[, axis, order, mode]) 	Calculate the relative maxima of data.
 # argrelextrema(data, comparator[, axis, ...]) 	Calculate the relative extrema of data.
 
@@ -186,25 +187,25 @@
     * Use `wlen` to reduce the time it takes to evaluate the conditions for
       `prominence` or `width` if `dataset` is large or has many local maxima
       (see `scipy.signal.peak_prominences`\ ).
 
     Examples
     --------
 
-    >>> dataset = scp.NDDataset.read("irdata/nh4y-activation.spg")
+    >>> dataset = scp.read("irdata/nh4y-activation.spg")
     >>> X = dataset[0, 1800.0:1300.0]
     >>> peaks, properties = X.find_peaks(height=1.5, distance=50.0, width=0.0)
     >>> len(peaks.x)
     2
     >>> peaks.x.values
     <Quantity([    1644     1455], 'centimeter^-1')>
     >>> properties["peak_heights"][0]
     <Quantity(2.26663446, 'absorbance')>
     >>> properties["widths"][0]
-    <Quantity(38.7309614, 'centimeter^-1')>
+    <Quantity(38.729003, 'centimeter^-1')>
     """
 
     X = dataset.squeeze()
 
     if X.ndim > 1:
         raise ValueError(
             "Works only for 1D NDDataset or a 2D NDdataset with `len(X.y) <= 1`"
@@ -218,17 +219,22 @@
     use_coord = use_coord and X.coordset is not None
 
     # units
     xunits = X.x.units if use_coord else 1
     dunits = X.units if use_coord else 1
 
     # assume linear x coordinates when use_coord is True!
-    step = np.abs(X.x.increment) if use_coord else 1
+    # TODO: what if the coordinates are not linear?
+    spacing = X.x.spacing
+    if isinstance(spacing, Quantity):
+        spacing = spacing.magnitude
+    step = np.abs(spacing) if use_coord else 1
 
     # transform coord (if exists) to index
+    # TODO: allow units for distance, width, wlen, plateau_size
     distance = int(round(distance / step)) if distance is not None else None
     width = int(round(width / step)) if width is not None else None
     wlen = int(round(wlen / step)) if wlen is not None else None
     plateau_size = int(round(plateau_size / step)) if plateau_size is not None else None
 
     # now the distance, width ... parameters are given in data points
     peaks, properties = scipy.signal.find_peaks(
```

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/pls.py` & `spectrochempy-0.6.4/spectrochempy/analysis/pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.4/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.4/spectrochempy/analysis/simplisma.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.4/spectrochempy/analysis/svd.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/api.py` & `spectrochempy-0.6.4/spectrochempy/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.4/spectrochempy/application/general_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/application/metaconfigurable.py` & `spectrochempy-0.6.4/spectrochempy/application/metaconfigurable.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.4/spectrochempy/application/plot_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/__init__.py` & `spectrochempy-0.6.4/spectrochempy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.4/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
+# flake8: noqa
 
-__all__ = ["Coord", "LinearCoord", "CoordSet", "NDDataset"]
-
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
-from spectrochempy.core.dataset.coordset import CoordSet
-from spectrochempy.core.dataset.nddataset import NDDataset
+# This is necessary for a correct generation of the core API
+# from spectrochempy.core.dataset.arraymixins.ndmath import *
+# from spectrochempy.core.dataset.arraymixins.ndmath import __all__
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 from warnings import warn
 
 import numpy as np
 from numpy.lib.npyio import zipfile_factory
 from traitlets import HasTraits, Instance, Unicode, Union
 
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.utils import exceptions
 from spectrochempy.utils.file import check_filename_to_save, pathclean
 from spectrochempy.utils.jsonutils import json_serialiser
 from spectrochempy.utils.misc import TYPE_BOOL
 from spectrochempy.utils.zip import ScpFile
 
@@ -368,29 +368,20 @@
                                 # coords
                                 _coords.append(item_to_attr(Coord(), v))
                             elif "coords" in v:
                                 # likely a coordset (multicoordinates)
                                 if v["is_same_dim"]:
                                     _mcoords = []
                                     for mv in v["coords"]:
-                                        if "data" in mv:
-                                            # coords
-                                            _mcoords.append(item_to_attr(Coord(), mv))
-                                        else:
-                                            # likely a linearcoord
-                                            _mcoords.append(
-                                                item_to_attr(LinearCoord(), mv)
-                                            )
+                                        _mcoords.append(item_to_attr(Coord(), mv))
+
                                     cs = CoordSet(*_mcoords[::-1], name=v["name"])
                                     _coords.append(cs)
                                 else:
                                     raise ValueError("Invalid : not a multicoordinate")
-                            else:
-                                # likely a linearcoord
-                                _coords.append(item_to_attr(LinearCoord(), v))
 
                         coords = dict((c.name, c) for c in _coords)
                         obj.set_coordset(coords)
                         obj._name = val["name"]
                         obj._references = val["references"]
 
                     elif key in ["_datasets"]:
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1108,15 +1108,15 @@
         NDDataset: [float64] a.u. (shape: (y:55, x:5549))
         >>> scp.average(nd)
         <Quantity(1.25085858, 'absorbance')>
         >>> m = scp.average(nd, dim='y')
         >>> m
         NDDataset: [float64] a.u. (size: 5549)
         >>> m.x
-        LinearCoord: [float64] cm⁻¹ (size: 5549)
+        Coord: [float64] cm⁻¹ (size: 5549)
         >>> m = scp.average(nd, dim='y', weights=np.arange(55))
         >>> m.data
         array([   1.789,    1.789, ...,    1.222,     1.22])
         """
 
         axis, dim = cls.get_axis(dim, allows_none=True)
         m, sumweight = np.ma.average(dataset, axis=axis, weights=weights, returned=True)
@@ -1632,15 +1632,15 @@
         fromiter : Make a dataset from an iterable.
 
         Examples
         --------
         Create a 1D NDDataset from a function
 
         >>> func1 = lambda t, v: v * t
-        >>> time = scp.LinearCoord.arange(0, 60, 10, units='min')
+        >>> time = scp.Coord.arange(0, 60, 10, units='min')
         >>> d = scp.fromfunction(func1, v=scp.Quantity(134, 'km/hour'), coordset=scp.CoordSet(t=time))
         >>> d.dims
         ['t']
         >>> d
         NDDataset: [float64] km (size: 6)
         """
 
@@ -2073,15 +2073,15 @@
         <Quantity(1.25085858, 'absorbance')>
         >>> scp.mean(nd, keepdims=True)
         NDDataset: [float64] a.u. (shape: (y:1, x:1))
         >>> m = scp.mean(nd, dim='y')
         >>> m
         NDDataset: [float64] a.u. (size: 5549)
         >>> m.x
-        LinearCoord: [float64] cm⁻¹ (size: 5549)
+        Coord: [float64] cm⁻¹ (size: 5549)
         """
 
         axis, dim = cls.get_axis(dim, allows_none=True)
         m = np.ma.mean(dataset, axis=axis, dtype=dtype, keepdims=keepdims)
 
         if np.isscalar(m):
             return Quantity(m, cls.units) if cls.units is not None else m
@@ -2747,16 +2747,14 @@
                     )
 
             # returntype
             if objtype == "NDDataset":
                 returntype = "NDDataset"
             elif objtype == "Coord" and returntype != "NDDataset":
                 returntype = "Coord"
-            elif objtype == "LinearCoord" and returntype != "NDDataset":
-                returntype = "LinearCoord"
             else:
                 # only the three above type have math capabilities in spectrochempy.
                 pass
 
             # Do we have to deal with mask?
             if hasattr(obj, "mask") and np.any(obj.mask):
                 is_masked = True
@@ -2765,18 +2763,15 @@
             is_quaternion = (
                 is_quaternion or False
                 if not hasattr(obj, "is_quaternion")
                 else obj.is_quaternion
             )
 
         # it may be necessary to change the object order regarding the types
-        if (
-            returntype in ["NDDataset", "Coord", "LinearCoord"]
-            and objtypes[0] != returntype
-        ):
+        if returntype in ["NDDataset", "Coord"] and objtypes[0] != returntype:
             inputs.reverse()
             objtypes.reverse()
 
             if fname in ["mul", "multiply", "add", "iadd"]:
                 pass
             elif fname in ["truediv", "divide", "true_divide"]:
                 fname = "multiply"
@@ -2849,16 +2844,17 @@
         # ---------------------------------------------------------------------------
         args = []
         otherqs = []
 
         # If other is None, then it is a unary operation we can pass the following
 
         if other is not None:
-            # First the units may require to be compatible, and if thet are sometimes they may need to be rescales
-            if othertype in ["NDDataset", "Coord", "LinearCoord", "Quantity"]:
+            # First the units may require to be compatible, and if thet are sometimes
+            # they may need to be rescales
+            if othertype in ["NDDataset", "Coord", "Quantity"]:
                 # rescale according to units
                 if not other.unitless:
                     if hasattr(obj, "units"):
                         # obj is a Quantity
                         if compatible_units:
                             # adapt the other units to that of object
                             other.ito(obj.units)
@@ -2927,15 +2923,15 @@
                                 data_only=True,
                             )  # we compare only data for this operation
                         except AssertionError:
                             raise CoordinatesMismatchError(
                                 obc[obj.dims[idx]].data, otc[other.dims[idx]].data
                             )
 
-            if othertype in ["NDDataset", "Coord", "LinearCoord"]:
+            if othertype in ["NDDataset", "Coord"]:
                 # mask?
                 if is_masked:
                     arg = other._umasked(other.data, other.mask)
                 else:
                     arg = other.data
 
             else:
@@ -3130,25 +3126,20 @@
             # type
             objtype = type(obj).__name__
             objtypes.append(objtype)
             if objtype == "NDDataset":
                 returntype = "NDDataset"
             elif objtype == "Coord" and returntype != "NDDataset":
                 returntype = "Coord"
-            elif objtype == "LinearCoord" and returntype != "NDDataset":
-                returntype = "LinearCoord"
             else:
                 # only the three above type have math capabilities in spectrochempy.
                 pass
 
         # it may be necessary to change the object order regarding the types
-        if (
-            returntype in ["NDDataset", "Coord", "LinearCoord"]
-            and objtypes[0] != returntype
-        ):
+        if returntype in ["NDDataset", "Coord"] and objtypes[0] != returntype:
             inputs.reverse()
             objtypes.reverse()
 
             if fname in ["mul", "add", "iadd"]:
                 pass
             elif fname in ["truediv", "divide", "true_divide"]:
                 fname = "mul"
@@ -3203,20 +3194,15 @@
                 self.history = f"Inplace binary op: {fname}  with `{_get_name(other)}` "
             # else:
             #    history = None
             objs = [self, other]
             fm, objs = self._check_order(fname, objs)
 
             data, units, mask, returntype = self._op(fm, objs)
-            if returntype != "LinearCoord":
-                self._data = data
-            else:
-                from spectrochempy.core.dataset.coord import LinearCoord
-
-                self = LinearCoord(data)
+            self._data = data
             self._units = units
             self._mask = mask
 
             return self
 
         return func
 
@@ -3225,20 +3211,15 @@
 
         new = self.copy()
         if returntype == "NDDataset" and not new._implements("NDDataset"):
             from spectrochempy.core.dataset.nddataset import NDDataset
 
             new = NDDataset(new)
 
-        if returntype != "LinearCoord":
-            new._data = cpy.deepcopy(data)
-        else:
-            from spectrochempy.core.dataset.coord import LinearCoord
-
-            new = LinearCoord(cpy.deepcopy(data))
+        new._data = cpy.deepcopy(data)
 
         # update the attributes
         new._units = cpy.copy(units)
         if mask is not None and np.any(mask != NOMASK):
             new._mask = cpy.copy(mask)
         if history is not None and hasattr(new, "history"):
             new.history = history.strip()
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/npy.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     Quantity,
     Unit,
     set_nmr_context,
     ur,
 )
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.constants import INPLACE, MASKED, NOMASK, MaskedConstant
+from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.file import pathclean
 from spectrochempy.utils.misc import (
     TYPE_FLOAT,
     TYPE_INTEGER,
     is_number,
     is_sequence,
     make_new_object,
@@ -158,15 +159,14 @@
     copy : bool, optional, Default:False
         If True, a deep copy of the passed object is performed.
 
     See Also
     --------
     NDDataset : Object which subclass  `NDArray` with the addition of coordinates.
     Coord : Object which subclass  `NDArray` (coordinates object).
-    LinearCoord : Object which subclass  `NDArray` (Linear coordinates object).
 
     Examples
     --------
 
     >>> myarray = scp.NDArray([1., 2., 3.], name='myarray')
     >>> assert myarray.name == 'myarray'
     """
@@ -285,15 +285,15 @@
             else:  # pragma: no cover
                 return False
             return eq
 
         if attrs is None:
             attrs = self.__dir__()
 
-        for attr in ["name"]:
+        for attr in ["name", "linear"]:
             if attr in attrs:
                 attrs.remove(attr)
 
         for attr in attrs:
             if attr != "units":
                 sattr = getattr(self, f"_{attr}")
                 if hasattr(other, f"_{attr}"):
@@ -375,15 +375,15 @@
         # init returned object
         if inplace:
             new = self
         else:
             new = self.copy()
 
         # slicing by index of all internal array
-        if new.data is not None:
+        if new._data is not None:
             udata = new.masked_data[keys]
             new._data = np.asarray(udata)
 
         if self.is_labeled:
             # case only of 1D dataset such as Coord
             new._labels = np.array(self._labels[keys])
 
@@ -657,15 +657,16 @@
                 start = self._loc2index(key, dim, units=units)
                 if isinstance(start, tuple):
                     start, info = start
                 if start is None:
                     return slice(None)
             else:
                 if key < 0:  # reverse indexing
-                    axis, dim = self.get_axis(dim)
+                    axis, dim = self.get_axis(dim) if self.ndim > 1 else (0, dim)
+                    # get axis is not defined for Coord for example
                     start = self.shape[axis] + key
             stop = start + 1  # in order to keep a non squeezed slice
             return slice(start, stop, 1)
         else:
             start, stop, step = key.start, key.stop, key.step
             if start is not None and not isinstance(start, TYPE_INTEGER):
                 start = self._loc2index(start, dim, units=units)
@@ -888,25 +889,26 @@
             if strunits == "":
                 strunits = "dimensionless"
         else:
             strunits = "unitless"
         return strunits
 
     def _repr_value(self):
+
         numpyprintoptions(precision=4, edgeitems=0, spc=1, linewidth=120)
 
         prefix = type(self).__name__ + ": "
         units = ""
 
         size = ""
         if not self.is_empty:
             if self.data is not None:
                 dtype = self.dtype
                 data = ""
-                if self._implements("Coord") or self._implements("LinearCoord"):
+                if self._implements("Coord"):
                     size = f" (size: {self.data.size})"
                 units = " " + self._repr_units()
             else:
                 # no data but labels
                 lab = self.get_labels()
                 data = f" {lab}"
                 size = f" (size: {len(lab)})"
@@ -1187,17 +1189,19 @@
         # name must be changed
         if not keepname:
             new.name = ""  # default
 
         return new
 
     @property
+    @_docstring.get_docstring(base="data")
+    @_docstring.dedent
     def data(self):
         """
-        The `data` array (`~numpy.ndarray`).
+        Data array (`~numpy.ndarray`).
 
         If there is no data but labels, then the labels are returned instead of data.
         """
         return self._data
 
     @data.setter
     def data(self, data):
@@ -1267,21 +1271,19 @@
                 )
 
         self._dims = tuple(values)
 
     @property
     def dtype(self):
         """
-        Data type (np.dtype).
+        Return the data type.
         """
         if self.is_empty:
-            self._dtype = None
-        else:
-            self._dtype = self.data.dtype
-        return self._dtype
+            return None
+        return self._data.dtype
 
     @property
     def filename(self):
         """
         Current filename for this dataset (`Pathlib` object).
         """
         if self._filename:
@@ -1381,19 +1383,17 @@
             return self.labels[level]
         else:
             return self._labels
 
     @property
     def has_data(self):
         """
-        True if the `data` array is not empty and size > 0.
-
-        (Readonly property).
+        True if the `data` array is not empty.
         """
-        if (self.data is None) or (self.data.size == 0):
+        if self._data is None or self._data.size == 0:
             return False
 
         return True
 
     @property
     def has_defined_name(self):
         """
@@ -1978,14 +1978,16 @@
             return "<untitled>"
 
     @title.setter
     def title(self, title):
         if title:
             self._title = title
 
+    @_docstring.get_docstring(base="to")
+    @_docstring.dedent
     def to(self, other, inplace=False, force=False):
         """
         Return the object with data rescaled to different units.
 
         Parameters
         ----------
         other : `Quantity` or str
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/coord.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implements the class  `Coord` .
 """
 
-__all__ = ["Coord", "LinearCoord"]
+__all__ = ["Coord"]
 
-import copy as cpy
 import textwrap
 
 import numpy as np
-from traitlets import All, Bool, CFloat, CInt, Instance, Integer, Unicode, Union
-from traitlets import default as traitdefault
-from traitlets import observe, signature_has_traits
+import traitlets as tr
 
 from spectrochempy.core import error_
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath, _set_operators
 from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
 from spectrochempy.core.units import Quantity, ur
+from spectrochempy.utils.compare import is_iterable, is_number
 from spectrochempy.utils.constants import INPLACE, NOMASK
-from spectrochempy.utils.misc import spacing_
+from spectrochempy.utils.decorators import deprecated
+from spectrochempy.utils.docstrings import _docstring
+from spectrochempy.utils.numutils import get_n_decimals, spacings
 from spectrochempy.utils.print import colored_output
 
 
 # ======================================================================================
 # Coord
 # ======================================================================================
-@signature_has_traits
+@tr.signature_has_traits
 class Coord(NDMath, NDArray):
     """
     Explicit coordinates for a dataset along a given axis.
 
     The coordinates of a `NDDataset` can be created using the  `Coord`
     object.
     This is a single dimension array with either numerical (float)
@@ -57,26 +57,26 @@
         desired behavior or set the `copy` argument to True.
     **kwargs
         Optional keywords parameters. See other parameters.
 
     Other Parameters
     ----------------
     dtype : str or dtype, optional, default=np.float64
-        If specified, the data will be casted to this dtype, else the
+        If specified, the data will be cast to this dtype, else the
         type of the data will be used.
     dims : list of chars, optional.
         if specified the list must have a length equal to the number od
         data dimensions (ndim) and the chars must be
-        taken among among x,y,z,u,v,w or t. If not specified,
+        taken among x,y,z,u,v,w or t. If not specified,
         the dimension names are automatically attributed in
         this order.
     name : str, optional
-        A user friendly name for this object. If not given,
+        A user-friendly name for this object. If not given,
         the automatic `id` given at the object creation will be
-        used as a name..
+        used as a name.
     labels : array of objects, optional
         Labels for the `data` . labels can be used only for 1D-datasets.
         The labels array may have an additional dimension, meaning
         several series of labels for the same data.
         The given array can be a list, a tuple, a `~numpy.ndarray` ,
         a ndarray-like, a  `NDArray` or any subclass of `NDArray` .
     units : `Unit` instance or str, optional
@@ -87,30 +87,38 @@
         package.
     title : str, optional
         The title of the dimension. It will later be used for instance
         for labelling plots of the data.
         It is optional but recommended to give a title to each ndarray.
     dlabel :  str, optional
         Alias of `title` .
-    copy : bool, optional
-        Perform a copy of the passed object. Default is False.
-    linear : bool, optional
-        If set to True, the coordinate is considered as a
-        `LinearCoord` object.
-    offset : float, optional
-        Only used is linear is True.
-        If omitted a value of 0.0 is taken for the coordinate offset.
-    increment : float, optional
-        Only used if linear is true.
-        If omitted a value of 1.0 is taken for the coordinate increment.
+    linearize_below : float, optional, default=0.1
+        variation of spacing in % below which the coordinate is linearized. Set it to
+    rounding : bool, optional, default=True
+        If True, the data will be rounded to the number of significant
+        digits given by `sigdigits`\ .
+    sigdigits : int, optional, default=4
+        Number of significant digits to be used for rounding and linearizing
+        the data.
+    larmor : `float` or `Quantity` instance, optional
+        The Larmor frequency of the nucleus. This is used only for NMR
+        data.
+    offset : `float` instance, optional
+        The offset of the axis. This is used to generate an evenly values spaced axis
+        together with `ìncrement` and `size`\ .
+    increment : `float` instance, optional
+        The increment between two consecutive values of the axis. This is used to
+        generate an evenly values spaced axis together with `offset` and `size`\ .
+    size : `int` instance, optional
+        The size of the axis. This is used to generate an evenly values spaced axis
+        together with `offset` and `increment`\ .
 
     See Also
     --------
     NDDataset : Main SpectroChemPy object: an array with masks, units and coordinates.
-    LinearCoord : linear coordinates.
 
     Examples
     --------
 
     We first import the object from the api :
 
     >>> from spectrochempy import Coord
@@ -118,203 +126,213 @@
     We then create a numpy `~numpy.ndarray` and use it as the numerical `data`
     axis of our new  `Coord` object :
 
     >>> c0 = Coord.arange(1., 12., 2., title='frequency', units='Hz')
     >>> c0
     Coord: [float64] Hz (size: 6)
 
-    We can take a series of str to create a non numerical but labelled
+    We can take a series of str to create a non-numerical but labelled
     axis :
 
     >>> tarr = list('abcdef')
     >>> tarr
     ['a', 'b', 'c', 'd', 'e', 'f']
 
     >>> c1 = Coord(labels=tarr, title='mylabels')
     >>> c1
     Coord: [labels] [  a   b   c   d   e   f] (size: 6)
     """
 
-    _copy = Bool()
+    _copy = tr.Bool()
 
-    _html_output = False
-    _parent_dim = Unicode(allow_none=True)
+    _html_output = tr.Bool(False)
+    _parent_dim = tr.Unicode(allow_none=True)
+    _parent = tr.Instance(
+        "spectrochempy.core.dataset.nddataset.NDDataset", allow_none=True
+    )
+    _use_time = tr.Bool(False)
+    _show_datapoints = tr.Bool(True)
+    _zpd = tr.Integer()
+
+    _linearize_below = tr.Float(0.1)
+    _linear = tr.Bool(False)
+    _sigdigits = tr.Int(4)
+    _rounding = tr.Bool(True)
 
-    # For linear data generation
-    _offset = Union((CFloat(), CInt(), Instance(Quantity)))
-    _increment = Union((CFloat(), CInt(), Instance(Quantity)))
-    _size = Integer(0)
-    _linear = Bool(False)
+    # specific to NMR
+    _larmor = tr.Instance(Quantity, allow_none=True)
 
     # ----------------------------------------------------------------------------------
     # initialization
     # ----------------------------------------------------------------------------------
     def __init__(self, data=None, **kwargs):
 
+        # check if data is iterable
+        if data is not None and not is_iterable(data):
+            raise ValueError("Data for coordinates must be an iterable or None")
+
+        # in case Coord replace old LinearCoord object
+        # without changing the arguments
+        _offset = kwargs.pop("offset", 0)
+        _increment = kwargs.pop("increment", None)
+        _size = kwargs.pop("size", None)
+
+        if data is None and _size is not None and _increment is not None:
+            data = np.arange(_size) * _increment + _offset
+
+        # specific case of NMR (initialize unit context NMR)
+        larmor = kwargs.pop("larmor", None)
+
+        self._linearize_below = kwargs.pop("linearize_below", 0.1)
+
+        # extract parameters for linearization and data rounding
+        self._sigdigits = kwargs.pop("sigdigits", 4)
+
+        # if data is a Coord, rounding may have been set already
+        if isinstance(data, Coord):
+            self._rounding = data._rounding
+        else:
+            self._rounding = kwargs.pop("rounding", True)  # rounding of data by default
+
+        # initialize the object
         super().__init__(data=data, **kwargs)
 
-        if len(self.shape) > 1:
-            raise ValueError("Only one 1D arrays can be used to define coordinates")
+        # set the larmor frequency if any
+        if larmor is not None:
+            self.larmor = larmor
 
-        self._linear = kwargs.pop("linear", False)
-        self._increment = kwargs.pop("increment", 1.0)
-        self._offset = kwargs.pop("offset", 0.0)
-        self._size = kwargs.pop("size", 0)
-        # self._accuracy = kwargs.pop('accuracy', None)
+    # ----------------------------------------------------------------------------------
+    # default values
+    # ----------------------------------------------------------------------------------
+    @tr.default("_larmor")
+    def _default_larmor(self):
+        return None
 
     # ----------------------------------------------------------------------------------
     # readonly property
     # ----------------------------------------------------------------------------------
     @property
     def reversed(self):
-        """bool - Whether the axis is reversed (readonly
-        property).
-        """
+        """Whether the axis is reversed."""
         if self.units == "ppm":
             return True
         elif self.units == "1 / centimeter" and "raman" not in self.title.lower():
             return True
         return False
 
         # Return a correct result only if the data are sorted  # return  # bool(self.data[0] > self.data[-1])
 
     @property
+    @_docstring.dedent
     def data(self):
-        """
-        The `data` array (`~numpy.ndarray`).
+        """%(data)s
 
-        If there is no data but labels, then the labels are returned instead of data.
+        Notes
+        -----
+        The data are always returned as a 1D array of float rounded to the number
+        of significant digits given by the `sigdigits` parameters.
+        If the spacing between the data is constant with the accuracy given by the
+        significant digits, the data are thus linearized
+        and the `linear` attribute is set to True.
         """
-        if self.linear:
-            data = np.arange(self.size) * self._increment + self._offset
-            # if hasattr(data, "units"):
-            #    data = data.m
-        else:
-            data = self._data
-
-        return data
+        return super().data
 
     @data.setter
     def data(self, data):
-
+        # set the data
         self._set_data(data)
 
+        # check if data is 1D
+        if self.has_data and len(self.shape) > 1:
+            raise ValueError("Only one 1D arrays can be used to define coordinates")
+
+        # linearize the data if possible or at least round it
+        # to the number of significant digits
+
+        if self.has_data and self.dtype.kind not in "M":
+
+            # First try to linearize the data if it is not a datetime
+            self._linear = False
+            self.linearize(self._sigdigits)
+            if self._linear:
+                return
+
+            # well, the data cannot be linearized with the given significant digits,
+            # now eventually round the data to the number of significant digits
+            # if self._data.size < 1:  # pragma: no cover
+            #     nd = self.sigdigits + 1
+            if self._rounding:
+                maxval = np.max(np.abs(self._data))
+                rounding = 2
+                nd = get_n_decimals(maxval, self.sigdigits) if maxval > 0 else rounding
+                self._data = np.around(self._data, max(nd, rounding))
+
     @property
     def default(self):
         # this is in case default is called on a coord, while it is a coordset property
         return self
 
     # ----------------------------------------------------------------------------------
     # hidden properties (for the documentation, only - we remove the docstring)
     # some of the property of NDArray has to be hidden because they
     # are not useful for this Coord class
     # ----------------------------------------------------------------------------------
     # NDarray methods
 
     @property
-    def is_complex(self):
-        return False  # always real
-
-    @property
-    def is_empty(self):
-        """
-        True if the `data` array is empty or size=0, and if no label are present
-        - Readonly property (bool).
-        """
-        if not self.linear:
-            return super().is_empty
-
-        return False
-
-    @property
     def ndim(self):
         if self.linear:
             return 1
         ndim = super().ndim
-        if ndim > 1:
+        if ndim > 1:  # pragma: no cover
             raise ValueError("Coordinate's array should be 1-dimensional!")
         return ndim
 
     @property
     def T(self):  # no transpose
         return self
 
     # @property
     # def values(self):
     #    return super().values
 
+    @_docstring.dedent
     def to(self, other, inplace=False, force=False):
-
+        """%(to)s"""
         new = super().to(other, force=force)
 
         if inplace:
+            # update the current object
+            self.data = new._data  # here we assign to the data attribute to fire
+            # the linearisation (eventually) and the rounding
+            # the _linear attribute is set to True if the data are linearized
             self._units = new._units
             self._title = new._title
             self._roi = new._roi
-            if not self.linear:
-                self._data = new._data
-            else:
-                self._offset = new._offset
-                self._increment = new._increment
-                self._linear = new._linear
-
         else:
+            new.data = new._data  # here we assign to the data attribute to fire
+            # the linearisation (eventually) and the rounding
             return new
 
-    to.__doc__ = NDArray.to.__doc__
-
     @property
     def masked_data(self):
         return super().masked_data
 
     @property
     def is_masked(self):
         return False
 
     @property
     def linear(self):
         """
-        Flag to specify if the data can be constructed using a linear variation (bool).
-        """
-        return self._linear
-
-    @linear.setter
-    def linear(self, val):
-
-        self._linear = (
-            val  # it val is true this provoque the linearization (  # see observe)
-        )
-
-        # if val and self._data is not None:  #     # linearisation of the data, if possible  #     self._linearize()
-
-    @property
-    def offset(self):
+        Whether the coordinates axis is linear (i.e. regularly spaced)
         """
-        Starting value for linear array
-        """
-        return self._offset
-
-    @offset.setter
-    def offset(self, val):
-        if isinstance(val, Quantity):
-            if self.has_units:
-                val.ito(self.units)
-                val = val.m
-            else:
-                self.units = val.units
-                val = val.m
-        self._offset = val
-
-    @property
-    def offset_value(self):
-        offset = self.offset
-        if self.units:
-            return Quantity(offset, self._units)
-        else:
-            return offset
+        if self.has_data and self.dtype.kind not in "M":
+            return self._linear
+        return False
 
     @property
     def mask(self):
         return NOMASK
 
     @mask.setter
     def mask(self, val):
@@ -331,56 +349,26 @@
 
     def pipe(self, func=None, *args, **kwargs):
         raise NotImplementedError
 
     def remove_masks(self, **kwargs):
         raise NotImplementedError
 
-    @property
-    def size(self):
-        """
-        Size of the underlying `data` array - Readonly property (int).
-        """
-
-        if self.linear:
-            # the provided size is returned i or its default
-            return self._size
-        else:
-            return super().size
-
-    @property
-    def shape(self):
-        if self.linear:
-            return (self._size,)
-        return super().shape
-
     def std(self, *args, **kwargs):
         raise NotImplementedError
 
     def sum(self, *args, **kwargs):
         raise NotImplementedError
 
     def swapdims(self, *args, **kwargs):
         raise NotImplementedError
 
     def swapaxes(self, *args, **kwargs):
         raise NotImplementedError
 
-    @property
-    def spacing(self):
-        """
-        Return coordinates spacing.
-
-        It will be a scalar if the coordinates are uniformly spaced,
-        else an array of the different spacings
-        """
-        if self.linear:
-            return self.increment * self.units
-        return spacing_(self.data) * self.units
-
     def squeeze(self, *args, **kwargs):
         raise NotImplementedError
 
     def random(self, *args, **kwargs):
         raise NotImplementedError
 
     def empty(self, *args, **kwargs):
@@ -451,62 +439,66 @@
 
     def argmin(self, *args, **kwargs):
         raise NotImplementedError
 
     def asfortranarray(self, *args, **kwargs):
         raise NotImplementedError
 
-    def astype(self, dtype=None, **kwargs):
-        """
-        Cast the data to a specified type.
-
-        Parameters
-        ----------
-        dtype : str or dtype
-            Typecode or data-type to which the array is cast.
-        """
-        if not self.linear:
-            self._data = self._data.astype(dtype, **kwargs)
-        else:
-            self._increment = np.array(self._increment).astype(dtype, **kwargs)[()]
-            self._offset = np.array(self._offset).astype(dtype, **kwargs)[()]
-        return self
+    # TODO: make it work
+    # def astype(self, dtype=None, **kwargs):
+    #     """
+    #     Cast the data to a specified type.
+    #
+    #     Parameters
+    #     ----------
+    #     dtype : str or dtype
+    #         Typecode or data-type to which the array is cast.
+    #     """
+    #     if dtype is None:
+    #         return self # no copy
+    #
+    #     if isinstance(dtype, str):
+    #         dtype = np.dtype(dtype) # convert to dtype
+    #
+    #     if kwargs.pop("copy", False) or not kwargs.pop("inplace", False):
+    #         new = self.copy()
+    #     else:
+    #         new = self  # no copy
+    #         kwargs["copy"] = False
+    #
+    #     data = self._data.astype(dtype, **kwargs)
+    #     new._data = data
+    #
+    #     return new
 
     def average(self, *args, **kwargs):
         raise NotImplementedError
 
     def clip(self, *args, **kwargs):
         raise NotImplementedError
 
     def get_axis(self, *args, **kwargs):
-        return super().get_axis(*args, **kwargs)
-
-    @property
-    def origin(self, *args, **kwargs):
         raise NotImplementedError
 
     @property
-    def author(self):
-        return None
+    def is_complex(self):
+        return False  # always real
 
     @property
-    def descendant(self):
-        return (self.data[-1] - self.data[0]) < 0
+    def is_descendant(self):
+        return (self._data[-1] - self._data[0]) < 0
 
     @property
     def dims(self):
         return ["x"]
 
     @property
     def is_1d(self):
         return True
 
-    def transpose(self, **kwargs):
-        return self
-
     # ----------------------------------------------------------------------------------
     # public methods
     # ----------------------------------------------------------------------------------
     def loc2index(self, loc):
         """
         Return the index corresponding to a given location.
 
@@ -519,20 +511,48 @@
         -------
         index : int.
             The corresponding index.
 
         Examples
         --------
 
-        >>> dataset = scp.NDDataset.read("irdata/nh4y-activation.spg")
+        >>> dataset = scp.read("irdata/nh4y-activation.spg")
         >>> dataset.x.loc2index(1644.0)
         4517
         """
         return self._loc2index(loc)
 
+    # TODO: new method to replace the old loc2index
+    # def loc2index(self, *loc):
+    #     """
+    #     Return the index(es) corresponding to given location(s).
+    #
+    #     Parameters
+    #     ----------
+    #     *loc : int, float, label or str
+    #         Value(s) corresponding to given location(s) on the coordinate's axis.
+    #
+    #     Returns
+    #     -------
+    #     int
+    #         The corresponding index.
+    #     """
+    #     if self.is_empty:
+    #         raise IndexError("Can not search location on an empty array")
+    #
+    #     # in case several location has been passed
+    #     if len(loc) > 1:
+    #         return [self.loc2index(loc_) for loc_ in loc]
+    #
+    #     res = self._interpret_key(*loc)
+    #     return res if not isinstance(res, tuple) else res[0]
+
+    def transpose(self, **kwargs):
+        return self
+
     # ----------------------------------------------------------------------------------
     # special methods
     # ----------------------------------------------------------------------------------
     def __copy__(self):
         res = self.copy(deep=False)  # we keep name of the coordinate by default
         res.name = self.name
         return res
@@ -545,24 +565,34 @@
     def __dir__(self):
         # remove some methods with respect to the full NDArray
         # as they are not useful for Coord.
         return [
             "data",
             "labels",
             "units",
+            "meta",
             "title",
             "name",
-            "offset",
-            "increment",
-            "linear",
             "roi",
+            "linear",
+            "sigdigits",
+            "larmor",
         ]
 
-    def __getitem__(self, items, **kwargs):
+    def __getattr__(self, attr):
+        if attr.startswith("_"):
+            # raise an error so that traits, ipython operation and more ...
+            # will be handled correctly
+            raise AttributeError
+        if attr in ("default", "coords"):
+            # this is in case these attributes are called while it is not a coordset.
+            return self
+        raise AttributeError
 
+    def __getitem__(self, items, **kwargs):
         if isinstance(items, list):
             # Special case of fancy indexing
             items = (items,)
 
         # choose, if we keep the same or create new object
         inplace = False
         if isinstance(items, tuple) and items[-1] == INPLACE:
@@ -576,69 +606,52 @@
         if inplace:
             new = self
         else:
             new = self.copy()
 
         # slicing by index of all internal array
         if new.data is not None:
-            udata = new.data[keys]
-
-            if new.linear:
-                # if self.increment > 0:
-                #     new._offset = udata.min()
-                # else:
-                #     new._offset = udata.max()
-                new._size = udata.size
-                if new._size > 1:
-                    inc = np.diff(udata)
-                    variation = (inc.max() - inc.min()) / udata.ptp()
-                    if variation < 1.0e-5:
-                        new._increment = np.mean(inc)  # np.round(np.mean(
-                        # inc), 5)
-                        new._offset = udata[0]
-                        new._data = None
-                        new._linear = True
-                    else:
-                        new._linear = False
-                else:
-                    new._linear = False
-
-            if not new.linear:
-                new._data = np.asarray(udata)
+            new._data = new.data[keys]
 
         if self.is_labeled:
             # case only of 1D dataset such as Coord
             new._labels = np.array(self._labels[keys])
 
         if new.is_empty:
             error_(
                 IndexError,
                 f"Empty array of shape {new._data.shape} resulted from slicing.\n"
                 f"Check the indexes and make sure to use floats for location slicing",
             )
-            new = None
+            return None
 
         new._mask = NOMASK
 
         # we need to keep the names when copying coordinates to avoid later
         # problems
         new.name = self.name
         return new
 
-    def __setitem__(self, items, value):
-
-        if self.linear:
-            error_(Exception, "Linearly defined array are readonly")
-            return
-
-        super().__setitem__(items, value)
-
     def __str__(self):
         return repr(self)
 
+    # ----------------------------------------------------------------------------------
+    # private methods and properties
+    # ----------------------------------------------------------------------------------
+    # @property
+    # def _axis_reversed(self):
+    #     # Whether the axis is usually _axis_reversed for plotting.
+    #     # This is usually the case of ppm and IR wavenumber.
+    #
+    #     if self.units == "ppm":
+    #         return True
+    #     if self.units == "1 / centimeter" and "raman" not in self.title.lower():
+    #         return True
+    #     return False
+
     def _cstr(self, header="  coordinates: ... \n", print_size=True, **kwargs):
 
         indent = kwargs.get("indent", 0)
 
         out = ""
         if not self.is_empty and print_size:
             out += f"{self._str_shape().rstrip()}\n"
@@ -672,383 +685,99 @@
         else:
             return out
 
     def __repr__(self):
         out = self._repr_value().rstrip()
         return out
 
-    # ----------------------------------------------------------------------------------
-    # Private properties and methods
-    # ----------------------------------------------------------------------------------
-    @traitdefault("_increment")
-    def _increment_default(self):
-        return 1.0
-
-    def _linearize(self):
-
-        if not self.linear or self._data is None:
-            return
-
-        self._linear = False  # to avoid action of the observer
-
-        if self._squeeze_ndim > 1:
-            error_(NotImplementedError, "Linearization is only implemented for 1D data")
-            return
-
-        data = self._data.squeeze()
-
-        # try to find an increment
-        if data.size > 1:
-            inc = np.diff(data)
-            variation = (inc.max() - inc.min()) / data.ptp()
-            if variation < 1.0e-5:
-                self._increment = (
-                    data.ptp() / (data.size - 1) * np.sign(inc[0])
-                )  # np.mean(inc)  # np.round(np.mean(inc), 5)
-                self._offset = data[0]
-                self._size = data.size
-                self._data = None
-                self._linear = True
-            else:
-                self._linear = False
-        else:
-            self._linear = False
-
-    @traitdefault("_offset")
-    def _offset_default(self):
-        return 0
-
-    def _set_data(self, data):
-
-        if data is None:
-            return
-
-        elif isinstance(data, Coord) and data.linear:
-            # Case of LinearCoord
-            for attr in self.__dir__():
-                try:
-                    if attr in ["linear", "offset", "increment"]:
-                        continue
-                    if attr == "data":
-                        val = data.data
-                    else:
-                        val = getattr(data, f"_{attr}")
-                    if self._copy:
-                        val = cpy.deepcopy(val)
-                    setattr(self, f"_{attr}", val)
-                except AttributeError:
-                    # some attribute of NDDataset are missing in NDArray
-                    pass
-
-        elif isinstance(data, NDArray):
-            # init data with data from another NDArray or NDArray's subclass
-            # No need to check the validity of the data
-            # because the data must have been already
-            # successfully initialized for the passed NDArray.data
-            for attr in self.__dir__():
-                try:
-                    val = getattr(data, f"_{attr}")
-                    if self._copy:
-                        val = cpy.deepcopy(val)
-                    setattr(self, f"_{attr}", val)
-                except AttributeError:
-                    # some attribute of NDDataset are missing in NDArray
-                    pass
-
-        elif isinstance(data, Quantity):
-            self._data = np.array(data.magnitude, subok=True, copy=self._copy)
-            self._units = data.units
-
-        elif hasattr(data, "mask"):
-            # an object with data and mask attributes
-            self._data = np.array(data.data, subok=True, copy=self._copy)
-            if isinstance(data.mask, np.ndarray) and data.mask.shape == data.data.shape:
-                self.mask = np.array(data.mask, dtype=np.bool_, copy=False)
-
-        elif (
-            not hasattr(data, "shape")
-            or not hasattr(data, "__getitem__")
-            or not hasattr(data, "__array_struct__")
-        ):
-            # Data doesn't look like a numpy array, try converting it to
-            # one. Non-numerical input are converted to an array of objects.
-            self._data = np.array(data, subok=True, copy=False)
-
-        else:
-            data = np.array(data, subok=True, copy=self._copy)
-            if data.dtype == np.object_:  # likely None value
-                data = data.astype(float)
-            self._data = data
-
-        if self.linear:
-            # we try to replace data by only an offset and an increment
-            self._linearize()
-
     @staticmethod
     def _unittransform(new, units):
         oldunits = new.units
-        if not new.linear:
-            udata = (new.data * oldunits).to(units)
-            new._data = udata.m
-            new._units = udata.units
-        else:
-            offset = (new.offset * oldunits).to(units)
-            increment = (new.increment * oldunits).to(units)
-            new._offset = offset.m
-            new._increment = increment.m
-            new._units = increment.units
-
+        udata = (new.data * oldunits).to(units)
+        new._data = udata.m
+        new._units = udata.units
         if new._roi is not None:
             roi = (np.array(new._roi) * oldunits).to(units)
             new._roi = list(roi)
-
-        # if new._linear:
-        #     # try to make it linear as well
-        #     new._linearize()
-        #     if not new._linear and new._implements("LinearCoord"):
-        #         # can't be linearized -> Coord
-        #         if inplace:
-        #             raise Exception(
-        #                     "A LinearCoord object cannot be transformed to a non linear coordinate "
-        #                     "`inplace` . "
-        #                     "Use to() instead of ito() and leave the `inplace` attribute to False"
-        #             )
-        #         else:
-        #             from spectrochempy import Coord
-        #
-        #             new = Coord(new)
         return new
 
     # ----------------------------------------------------------------------------------
     # Events
     # ----------------------------------------------------------------------------------
-    @observe(All)
+    @tr.observe(tr.All)
     def _anytrait_changed(self, change):
         # ex: change {
         #   'owner': object, # The HasTraits instance
         #   'new': 6, # The new value
         #   'old': 5, # The old value
         #   'name': "foo", # The name of the changed trait
         #   'type': 'change', # The event type of the notification, usually
         #   'change'
         # }
+        pass
 
-        if change.name in ["_linear", "_increment", "_offset", "_size"]:
-            if self._linear:
-                self._linearize()
-            return
-
-    @property
-    def increment(self):
-        return self._increment
-
-    @increment.setter
-    def increment(self, val):
-        if isinstance(val, Quantity):
-            if self.has_units:
-                val.ito(self.units)
-                val = val.m
-            else:
-                self.units = val.units
-                val = val.m
-        self._increment = val
-
-    @property
-    def increment_value(self):
-        increment = self.increment
-        if self.units:
-            return Quantity(increment, self._units)
-        else:
-            return increment
-
-
-@signature_has_traits
-class LinearCoord(Coord):
-    """
-    Linear coordinates.
-
-    Such coordinates correspond to a ascending or descending linear
-    sequence of values, fully determined by two parameters, i.e., an offset (off) and an increment (inc) :
-
-    .. math::
-
-        \\mathrm{data} = i*\\mathrm{inc} + \\mathrm{off}.
-
-    Parameters
-    ----------
-    data : a 1D array-like object, optional
-        WWen provided, the `size` parameters is adjusted to the size of
-        the array, and a linearization of the
-        array is performed (only if it is possible: regular spacing in
-        the 1.e5 relative accuracy).
-    offset : float, optional
-        If omitted a value of 0.0 is taken for the coordinate offset.
-    increment : float, optional
-        If omitted a value of 1.0 is taken for the coordinate increment.
-    **kwargs
-        Optional keywords parameters. See other parameters.
-
-    Other Parameters
-    ----------------
-    dtype : str or dtype, optional, default=np.float64
-        If specified, the data will be casted to this dtype, else the
-        type of the data will be used
-    dims : list of chars, optional.
-        if specified the list must have a length equal to the number od
-        data dimensions (ndim) and the chars must be
-        taken among x,y,z,u,v,w or t. If not specified,
-        the dimension names are automatically attributed in
-        this order.
-    name : str, optional
-        A user-friendly name for this object. If not given,
-        the automatic `id` given at the object creation will be
-        used as a name.
-    labels : array of objects, optional
-        Labels for the `data` . labels can be used only for 1D-datasets.
-        The labels array may have an additional dimension, meaning
-        several series of labels for the same data.
-        The given array can be a list, a tuple, a `~numpy.ndarray` ,
-        a ndarray-like, a  `NDArray` or any subclass of `NDArray` .
-    units : `Unit` instance or str, optional
-        Units of the data. If data is a `Quantity` then `units` is set
-        to the unit of the `data`; if a unit is also
-        explicitly provided an error is raised. Handling of units use
-        the `pint <https://pint.readthedocs.org/>`_
-        package.
-    title : str, optional
-        The title of the dimension. It will later be used for instance
-        for labelling plots of the data.
-        It is optional but recommended to give a title to each ndarray.
-    dlabel : str, optional.
-        Alias of `title` .
-    meta : dict-like object, optional.
-        Additional metadata for this object. Must be dict-like but no
-        further restriction is placed on meta.
-    copy : bool, optional
-        Perform a copy of the passed object. Default is False.
-    fill_missing : bool
-        Create a linear coordinate array where missing data are masked.
-
-    See Also
-    --------
-    NDDataset : Main SpectroChemPy object: an array with masks, units and
-    coordinates.
-    Coord : Explicit coordinates.
-
-    Examples
-    --------
-    >>> from spectrochempy import LinearCoord, Coord
-
-    To create a linear coordinate, we need to specify an offset,
-    an increment and
-    the size of the data
-
-    >>> c1 = LinearCoord(offset=2.0, increment=2.0, size=10)
-
-    Alternatively, linear coordinates can be created using the
-    `linear` keyword
-
-    >>> c2 = Coord(linear=True, offset=2.0, increment=2.0, size=10)
-    """
-
-    _use_time = Bool(False)
-    _show_datapoints = Bool(True)
-    _zpd = Integer()
-
-    def __init__(self, data=None, offset=0.0, increment=1.0, **kwargs):
-
-        if data is not None and isinstance(data, Coord) and not data.linear:
-            raise ValueError(
-                "Only linear Coord (with attribute linear set to True, can be transformed into "
-                "LinearCoord class"
-            )
-
-        super().__init__(data, **kwargs)
-
-        # when data is present, we don't need offset and increment, nor size,
-        # we just do linear=True and these parameters are ignored
-
-        if self._data is not None:
-            self._linear = True
-
-        elif not self.linear:
-            # in case it was not already a linear array
-            self.offset = offset
-            self.increment = increment
-            self._linear = True
-
-    @property  # read only
-    def linear(self):
-        return self._linear
-
-    def __dir__(self):
-        # remove some methods with respect to the full NDArray
-        # as they are not useful for Coord.
-
-        return [
-            "data",
-            "labels",
-            "units",
-            "meta",
-            "title",
-            "name",
-            "offset",
-            "increment",
-            "linear",
-            "size",
-            "roi",
-            "show_datapoints",
-        ]
+    # ----------------------------------------------------------------------------------
+    # Public methods and properties
+    # ----------------------------------------------------------------------------------
 
     def set_laser_frequency(self, frequency=15798.26 * ur("cm^-1")):
+        """
+        Set the laser frequency.
 
+        This method is used to set the laser frequency of the dataset.
+        The laser frequency is used to convert the x-axis from optical path
+        difference to time. The laser frequency is also used to calculate
+        the wavenumber axis.
+
+        Parameters
+        ----------
+        frequency : `float` or `Quantity`\ , optional, default=15798.26 * ur("cm^-1")
+            The laser frequency in cm^-1 or Hz. If the value is in cm^-1, the
+            frequency is converted to Hz using the current speed of light value.
+        """
         if not isinstance(frequency, Quantity):
             frequency = frequency * ur("cm^-1")
 
         frequency.ito("Hz")
         self.meta.laser_frequency = frequency
 
         if self._use_time:
             spacing = 1.0 / frequency
             spacing.ito("picoseconds")
-
-            self.increment = spacing.m
-            self.offset = 0
+            self._data = np.arange(self.shape[-1]) * spacing.m
             self._units = ur.picoseconds
             self.title = "time"
 
         else:
             frequency.ito("cm^-1")
             spacing = 1.0 / frequency
             spacing.ito("mm")
-
-            self.increment = spacing.m
-            self.offset = -self.increment * self._zpd
+            offset = -spacing.m * self._zpd
+            self._data = np.arange(self.shape[-1]) * spacing.m + offset
             self._units = ur.mm
             self.title = "optical path difference"
 
     @property
     def _use_time_axis(self):
         # private property
-        # True if time scale must be used for interferogram axis. Else it
+        # True if timescale must be used for interferogram axis. Else it
         # will be set to optical path difference.
         return self._use_time
 
     @_use_time_axis.setter
     def _use_time_axis(self, val):
 
         self._use_time = val
         if "laser_frequency" in self.meta:
             self.set_laser_frequency(self.meta.laser_frequency)
 
     @property
     def show_datapoints(self):
         """
         Bool : True if axis must discard values and show only datapoints.
-
         """
         if "laser_frequency" not in self.meta or self.units.dimensionality not in [
             "[time]",
             "[length]",
         ]:
             return False
 
@@ -1056,23 +785,133 @@
 
     @show_datapoints.setter
     def show_datapoints(self, val):
 
         self._show_datapoints = val
 
     @property
+    def larmor(self):
+        """
+        Return larmor frequency in NMR spectroscopy context.
+        """
+        return self._larmor
+
+    @larmor.setter
+    def larmor(self, val):
+        self._larmor = val
+
+    @property
     def laser_frequency(self):
         """
         Laser frequency if needed (Quantity).
         """
         return self.meta.laser_frequency
 
     @laser_frequency.setter
     def laser_frequency(self, val):
-        self.meta.aser_frequency = val
+        self.meta.laser_frequency = val
+
+    def linearize(self, sigdigits=4):
+        """
+        Linearize the coordinate's data.
+
+        Make coordinates with an equally distributed spacing, when possible, i.e.,
+        if the spacings are not too different when rounded to the number of
+        significant digits passed in parameters.
+        If the spacings are too different, the coordinates are not linearized.
+        In this case, the `linear` attribute is set to False.
+
+        Parameters
+        ----------
+        sigdigits :  Int, optional, default=4
+            The number of significant digit for coordinates values.
+        """
+        if not self.has_data or self.data.size < 3:
+            return
+
+        data = self._data.squeeze()
+
+        self._sigdigits = sigdigits
+
+        spacing = spacings(self._data, sigdigits)
+
+        makeitlinear = is_number(spacing)
+
+        if not makeitlinear and is_iterable(spacing):
+            # may be the variation in % are small enough (0.1%)
+            variation = (
+                (np.max(spacing) - np.min(spacing)) * 100.0 / np.max(spacing) / 2.0
+            )
+            if variation <= self._linearize_below:
+                makeitlinear = True
+
+        if makeitlinear:
+            # single spacing with this precision
+            # we set the number with their full precision
+            # rounding will be made if necessary when reading the data property
+            nd = get_n_decimals(np.diff(self._data).max(), self._sigdigits)
+            data = np.around(data, nd)
+            self._data = np.linspace(data[0], data[-1], data.size)
+            self._linear = True
+        else:
+            # from spectrochempy.core import debug_
+            # debug_(
+            #      "The coordinates spacing is not enough uniform to allow linearization."
+            #  )
+            self._linear = False
+
+    @property
+    def sigdigits(self):
+        """
+        Number of significant digits for rounding coordinate values.
+
+        Note
+        ----
+        The number of significant digits is used when linearizing the coordinates. It is
+        also used when setting the coordinates values at the Coord initialization
+        or everytime the data array is changed.
+        """
+        return self._sigdigits
+
+    @sigdigits.setter
+    def sigdigits(self, val):
+        self._sigdigits = val
+
+    @property
+    def spacing(self):
+        """
+        Coordinate spacing.
+
+        It will be a scalar if the coordinates are uniformly spaced, else
+        an array of the different spacings.
+
+        Note
+        ----
+        The spacing is returned in the units of the coordinate.
+        """
+        units = self.units if self.units is not None else 1
+        if self.has_data:
+            return spacings(self._data) * units
+        return None
+
+
+# ======================================================================================
+# LinearCoord (Deprecated)
+# TODO : should be removed in version 0.8
+# ======================================================================================
+@tr.signature_has_traits
+class LinearCoord(Coord):
+    @deprecated(
+        kind="object",
+        replace="Coord",
+        removed="0.8",
+    )
+    def __init__(self, **kwargs):
+        # TODO : remove in version 0.8
+        super().__init__(**kwargs)
 
 
 # ======================================================================================
 # Set the operators
 # ======================================================================================
 _set_operators(Coord, priority=50)
-_set_operators(LinearCoord, priority=50)
+_set_operators(LinearCoord, priority=50)  # Suppress 0.8
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/coordset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     default,
     observe,
     signature_has_traits,
     validate,
 )
 
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.utils.misc import is_sequence
 from spectrochempy.utils.print import colored_output, convert_to_html
 
 
 # ======================================================================================
 # CoordSet
 # ======================================================================================
@@ -71,15 +71,14 @@
         given, standard names are used: x, y, ...
     copy : bool, optional
         Perform a copy of the passed object. Default is True.
 
     See Also
     --------
     Coord : Explicit coordinates object.
-    LinearCoord : Implicit coordinates object.
     NDDataset: The main object of SpectroChempy which makes use of CoordSet.
 
     Examples
     --------
     >>> from spectrochempy import Coord, CoordSet
 
     Define 4 coordinates, with two for the same dimension
@@ -180,15 +179,15 @@
             for coord in coords[::-1]:  # we fill from the end of the list
                 # (in reverse order) because by convention when the
                 # names are not specified, the order of the
                 # coords follow the order of dims.
                 if not isinstance(coord, CoordSet):
                     if isinstance(coord, list):
                         coord = CoordSet(*coord[::-1], sorted=False)
-                    elif not isinstance(coord, LinearCoord):  # else
+                    else:
                         coord = Coord(coord, copy=True)
                 else:
                     coord = cpy.deepcopy(coord)
 
                 if not keepnames:
                     if dims is None:
                         # take the last available name of available names list
@@ -202,45 +201,47 @@
 
         # now evaluate keywords argument
         # ------------------------------
         for key, coord in list(kwargs.items())[:]:
             # remove the already used kwargs (Fix: deprecation warning in Traitlets - all args, kwargs must be used)
             del kwargs[key]
 
-            # prepare values to be either Coord, LinearCoord or CoordSet
+            # prepare values to be either Coord or CoordSet
             if isinstance(coord, (list, tuple)):
                 coord = CoordSet(
                     *coord, sorted=False
                 )  # make sure in this case it becomes a CoordSet instance
 
             elif isinstance(coord, np.ndarray) or coord is None:
                 coord = Coord(
                     coord, copy=True
                 )  # make sure it's a Coord  # (even if it is None -> Coord(None)
 
             elif isinstance(coord, str) and coord in DEFAULT_DIM_NAME:
-                # may be a reference to another coordinates (e.g. same coordinates for various dimensions)
+                # may be a reference to another coordinates (e.g. same coordinates for
+                # various dimensions)
                 self._references[key] = coord  # store this reference
                 continue
 
             # Populate the coords with coord and coord's name.
-            if isinstance(coord, (NDArray, Coord, LinearCoord, CoordSet)):  # NDArray,
+            if isinstance(coord, (NDArray, Coord, CoordSet)):
                 if key in self.available_names or (
                     len(key) == 2
                     and key.startswith("_")
                     and key[1] in list("123456789")
                 ):
                     # ok we can find it as a canonical name:
                     # this will overwrite any already defined coord value
                     # which means also that kwargs have priority over args
                     coord.name = key
                     self._append(coord)
 
                 elif not self.is_empty and key in self.names:
-                    # append when a coordinate with this name is already set in passed arg.
+                    # append when a coordinate with this name is already set in passed
+                    # arg.
                     # replace it
                     idx = self.names.index(key)
                     coord.name = key
                     self._coords[idx] = coord
 
                 else:
                     raise KeyError(
@@ -287,15 +288,15 @@
     @validate("_coords")
     def _coords_validate(self, proposal):
         coords = proposal["value"]
         if not coords:
             return None
 
         for id, coord in enumerate(coords):
-            if coord and not isinstance(coord, (Coord, LinearCoord, CoordSet)):
+            if coord and not isinstance(coord, (Coord, CoordSet)):
                 raise TypeError(
                     "At this point all passed coordinates should be of type Coord or CoordSet!"
                 )  # coord =  #
                 # Coord(coord)
             if self._copy:
                 coords[id] = coord.copy()
             else:
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.4/spectrochempy/core/dataset/nddataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from spectrochempy.core import error_, warning_
 from spectrochempy.core.dataset.arraymixins.ndio import NDIO
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath  # _set_ufuncs,
 from spectrochempy.core.dataset.arraymixins.ndmath import _set_operators
 from spectrochempy.core.dataset.arraymixins.ndplot import NDPlot
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
 from spectrochempy.core.dataset.baseobjects.ndcomplex import NDComplexArray
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.exceptions import SpectroChemPyError, UnknownTimeZoneError
 from spectrochempy.utils.optional import import_optional_dependency
 from spectrochempy.utils.print import colored_output
 from spectrochempy.utils.system import get_user_and_node
 
@@ -148,15 +148,14 @@
         A string to add to the object history.
     copy : `bool`\ , optional
         Perform a copy of the passed object. Default is False.
 
     See Also
     --------
     Coord : Explicit coordinates object.
-    LinearCoord : Implicit coordinates object.
     CoordSet : Set of coordinates.
 
     Notes
     -----
     The underlying array in a `NDDataset` object can be accessed through the
     `data` attribute, which will return a conventional `~numpy.ndarray`\ .
     """
@@ -252,18 +251,15 @@
 
             if coordtitles is None:
                 coordtitles = [None] * self.ndim
 
             _coordset = []
             for c, u, t in zip(coordset, coordunits, coordtitles):
                 if not isinstance(c, CoordSet):
-                    if isinstance(c, LinearCoord):
-                        coord = LinearCoord(c)
-                    else:
-                        coord = Coord(c)
+                    coord = Coord(c)
                     if u is not None:
                         coord.units = u
                     if t is not None:
                         coord.title = t
                 else:
                     if u:  # pragma: no cover
                         warning_(
@@ -479,15 +475,15 @@
                     _coordset[idx]._is_same_dim = True
                 elif isinstance(value, CoordSet):
                     if len(value) > 1:
                         value = CoordSet(value)
                     _coordset[idx] = list(value.to_dict().values())[0]
                     _coordset[idx].name = key
                     _coordset[idx]._is_same_dim = True
-                elif isinstance(value, (Coord, LinearCoord)):
+                elif isinstance(value, Coord):
                     value.name = key
                     _coordset[idx] = value
                 else:
                     _coordset[idx] = Coord(value, name=key)
                 _coordset = self._valid_coordset(_coordset)
                 self._coordset.set(_coordset)
             else:
@@ -504,15 +500,14 @@
             "name",
             "author",
             "description",
             "history",
             "created",
             "modified",
             "origin",
-            "show_datapoints",
             "roi",
             "modeldata",
             "processeddata",
             "baselinedata",
             "referencedata",
             "state",
             "ranges",
@@ -716,15 +711,15 @@
                 coord is not None
                 and not isinstance(coord, CoordSet)
                 and coord.data is None
             ):
                 continue
 
             # For coord to be acceptable, we require at least a NDArray, a NDArray subclass or a CoordSet
-            if not isinstance(coord, (LinearCoord, Coord, CoordSet)):
+            if not isinstance(coord, (Coord, CoordSet)):
                 if isinstance(coord, NDArray):
                     coord = coords[k] = Coord(coord)
                 else:
                     raise TypeError(
                         "Coordinates must be an instance or a subclass of Coord class or NDArray, or of "
                         f" CoordSet class, but an instance of {type(coord)} has been passed"
                     )
@@ -833,15 +828,15 @@
     @author.setter
     def author(self, value):
         self._author = value
 
     @property
     def history(self):
         """
-        Describes the history of actions made on this array (tr.List of strings).
+        Describes the history of actions made on this array (List of strings).
         """
 
         history = []
         for date, value in self._history:
             date = pytz.utc.localize(date)
             date = date.astimezone(self.timezone).isoformat(sep=" ", timespec="seconds")
             value = value[0].capitalize() + value[1:]
@@ -1451,15 +1446,17 @@
             Transposed NDDataset.
 
         See Also
         --------
         swapdims : Interchange two dimensions of a NDDataset.
         """
         new = super().transpose(*dims, inplace=inplace)
-        new.history = f"Data transposed between dims: {dims}" if dims else ""
+        new.history = (
+            f"Data transposed between dims: {dims}" if dims else "Data transposed"
+        )
 
         return new
 
     # # ----------------------------------------------------------------------------------
     # # DASH GUI options  (Work in Progress - not used for now)
     # # ----------------------------------------------------------------------------------
     # #
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.4/spectrochempy/core/plotters/multiplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.4/spectrochempy/core/plotters/plot1d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.4/spectrochempy/core/plotters/plot2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from copy import copy as cpy
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.ticker import MaxNLocator, ScalarFormatter
 
-from spectrochempy.core.dataset.coord import LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.utils.docstrings import add_docstring
 from spectrochempy.utils.plots import make_label, plot_method
 
 _PLOT2D_DOC = """
 ax : |Axes| instance. Optional
     The axe where to plot. The default is the current axe or to create a new one if is None.
 clear : bool, optional, default=`True`
@@ -224,15 +224,15 @@
         x = x.default
     xsize = new.shape[-1]
     show_x_points = False
     if x is not None and hasattr(x, "show_datapoints"):
         show_x_points = x.show_datapoints
     if show_x_points:
         # remove data and units for display
-        x = LinearCoord.arange(xsize)
+        x = Coord.arange(xsize)
 
     discrete_data = False
 
     if x is not None and (not x.is_empty or x.is_labeled):
         xdata = x.data
         if not np.any(xdata):
             if x.is_labeled:
@@ -277,15 +277,15 @@
     ysize = new.shape[-2]
 
     show_y_points = False
     if y is not None and hasattr(y, "show_datapoints"):
         show_y_points = y.show_datapoints
     if show_y_points:
         # remove data and units for display
-        y = LinearCoord.arange(ysize)
+        y = Coord.arange(ysize)
 
     if y is not None and (not y.is_empty or y.is_labeled):
         ydata = y.data
 
         if not np.any(ydata):
             if y.is_labeled:
                 ydata = range(1, len(y.labels) + 1)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.4/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.4/spectrochempy/core/plotters/plotly.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 __all__ = ["align"]
 __dataset_methods__ = __all__
 
 # import scipy.interpolate
 import numpy as np
 
 from spectrochempy.core import error_, warning_
-from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.utils import exceptions
 from spectrochempy.utils.constants import MASKED
 from spectrochempy.utils.misc import get_n_decimals
 
 
 def can_merge_or_align(coord1, coord2):
     """
@@ -113,32 +112,25 @@
 
     Raises
     ------
     ValueError
         Issued when the dimensions given in `dim` or `dims` argument are not
         compatibles (units, titles, etc.).
     """
-    # DEVELOPER NOTE
-    # There is probably better methods, but to simplify dealing with
-    # LinearCoord, we transform them in Coord before treatment (going back
-    # to linear if possible at the end of the process)
-
     # TODO: Perform an alignment along numeric labels
     # TODO: add example in docs
 
     # copy objects?
     copy = kwargs.pop("copy", True)
 
     # make a single list with dataset and the remaining object
     objects = [dataset] + list(others)
 
     # should we align on given external coordinates
     extern_coord = kwargs.pop("coord", None)
-    if extern_coord and extern_coord._implements("LinearCoord"):
-        extern_coord = Coord(extern_coord, linear=False, copy=True)
 
     # what's the method to use (by default='outer')
     method = kwargs.pop("method", "outer")
 
     # trivial cases where alignment is not possible or unnecessary
     if not objects:
         warning_("No object provided for alignment!")
@@ -207,33 +199,28 @@
         reversed = ref_coord.reversed
 
         # prepare a new Coord object to store the final new dimension
         new_coord = ref_coord.copy()
 
         ndec = get_n_decimals(new_coord.data.max(), 1.0e-5)
 
-        if new_coord._implements("LinearCoord"):
-            new_coord = Coord(new_coord, linear=False, copy=True)
-
         # loop on all object
         for index, object in _objects.items():
 
             obj = object["obj"]
 
             if obj is ref_obj:
                 # not necessary to compare with itself!
                 continue
 
             if reversed:
                 obj.sort(descend=False, dim=dim, inplace=True)
 
             # get the current object coordinates and check compatibility
             coord = obj.coordset[dim]
-            if coord._implements("LinearCoord") or coord.linear:
-                coord = Coord(coord, linear=False, copy=True)
 
             if not coord.is_units_compatible(ref_coord):
                 # not compatible, stop everything
                 raise exceptions.UnitsCompatibilityError(
                     "NDataset to align must have compatible units!"
                 )
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/apodization.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/autosub.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             new.swapdims(axis, -1, inplace=True)
             swapped = True
 
         lastcoord = new.coordset[dim]
 
         # most of the time we need sorted axis, so let's do it now
         is_descendant = False
-        if lastcoord.descendant:
+        if lastcoord.is_descendant:
             new.sort(dim=dim, inplace=True, descend=False)
             is_descendant = True
             lastcoord = new.coordset[dim]
 
         x = lastcoord.data
         self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
         self._extendranges(*ranges, **kwargs)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,21 +134,21 @@
         if not coords[dim].is_empty:
 
             labels = []
             if coords[dim].is_labeled:
                 for ds in datasets:
                     labels.append(ds.coordset[dim].labels)
 
-            if coords[dim]._implements() in ["Coord", "LinearCoord"]:
-                coords[dim] = Coord(coords[dim], linear=False)
+            if coords[dim]._implements() in ["Coord"]:
+                coords[dim] = Coord(coords[dim])
                 if labels != []:
                     coords[dim]._labels = np.concatenate(labels)
             elif coords[dim]._implements("CoordSet"):
                 if labels != []:
-                    labels = np.array(labels)
+                    labels = np.array(labels, dtype=object)
                     for i, coord in enumerate(coords[dim]):
                         if labels[:i].size != 0:
                             coord._labels = np.concatenate(
                                 [label for label in labels[:, i]]
                             )
             coord_data_tuple = tuple((ds.coordset[dim].data for ds in datasets))
             none_coord = len([x for x in coord_data_tuple if x is None])
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import re
 
 import numpy as np
 from quaternion import as_float_array
 from scipy.signal import hilbert
 
 from spectrochempy.core import error_
-from spectrochempy.core.dataset.coord import LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.processors.utils import _units_agnostic_method
 from spectrochempy.core.processors.zero_filling import zf_size
 from spectrochempy.core.units import ur
 from spectrochempy.utils.misc import (
     as_quaternion,
     get_component,
     largest_power_of_2,
@@ -252,14 +252,15 @@
     --------
     fft : Direct Fourier transform.
     """
     return fft(dataset, size=size, inv=True, **kwargs)
 
 
 def fft(dataset, size=None, sizeff=None, inv=False, ppm=True, **kwargs):
+
     """
     Apply a complex fast fourier transform.
 
     For multidimensional NDDataset,
     the apodization is by default performed on the last dimension.
 
     The data in the last dimension MUST be in time-domain (or without dimension)
@@ -336,58 +337,63 @@
     if (
         not inv
         and not x.unitless
         and not x.dimensionless
         and x.units.dimensionality != "[time]"
     ):
         error_(
+            Exception,
             "fft apply only to dimensions with [time] dimensionality or dimensionless coords\n"
-            "fft processing was thus cancelled"
+            "fft processing was thus cancelled",
         )
         error = True
 
     elif (
         inv
         and not x.unitless
         and x.units.dimensionality != "1/[time]"
         and not x.dimensionless
     ):
         error_(
+            Exception,
             "ifft apply only to dimensions with [frequency] dimensionality or with ppm units "
-            "or dimensionless coords.\n ifft processing was thus cancelled"
+            "or dimensionless coords.\n ifft processing was thus cancelled",
         )
         error = True
 
     # Should not be masked
     elif new.is_masked:
         error_(
-            "current fft or ifft processing does not support masked data as input.\n processing was thus cancelled"
+            Exception,
+            "current fft or ifft processing does not support masked data as input.\n processing was thus cancelled",
         )
         error = True
 
     # Coordinates should be uniformly spaced (linear coordinate)
     if not x.linear:
-        # try to linearize it
-        x.linear = True
-        if not x.linear:
-            # linearization failed
-            error = True
+        error_(
+            "fft or ifft processing only support linear coordinates.\n"
+            "Processing was thus cancelled"
+        )
+
+        error = True
 
     if hasattr(x, "_use_time_axis"):
-        x._use_time_axis = True  # we need to havze dimentionless or time units
+        x._use_time_axis = True  # we need to have dimentionless or time units
 
     if not error:
         # OK we can proceed
 
         # time domain size
         td = None
         if not inv:
             td = x.size
 
-        # if no size (or si) parameter then use the size of the data (size not used for inverse transform
+        # if no size (or si) parameter then use the size of the data
+        # (size not used for inverse transform
         if size is None or inv:
             size = kwargs.get("si", x.size)
 
         # we default to the closest power of two larger of the data size
         if is_nmr:
             size = largest_power_of_2(size)
 
@@ -498,15 +504,15 @@
         if not inv:
             # time to frequency
             sizem = max(size - 1, 1)
             deltaf = -sw / sizem
             first = sfo1 - sf - deltaf * sizem / 2.0
 
             # newcoord = type(x)(np.arange(size) * deltaf + first)
-            newcoord = LinearCoord.arange(size) * deltaf + first
+            newcoord = Coord.arange(size) * deltaf + first
             newcoord.show_datapoints = False
             newcoord.name = x.name
             new.title = "intensity"
             if is_nmr:
                 newcoord.title = f"${nucleus}$ frequency"
                 newcoord.ito("Hz")
             elif is_ir:
@@ -520,15 +526,15 @@
         else:
             # frequency or ppm to time
             sw = abs(x.data[-1] - x.data[0])
             if x.units == "ppm":
                 sw = bf1.to("Hz") * sw / 1.0e6
             deltat = (1.0 / sw).to("us")
 
-            newcoord = LinearCoord.arange(size) * deltat
+            newcoord = Coord.arange(size) * deltat
             newcoord.name = x.name
             newcoord.title = "time"
             newcoord.ito("us")
 
         if is_nmr and not inv:
             newcoord.meta.larmor = bf1  # needed for ppm transformation
             ppm = kwargs.get("ppm", True)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/filter.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/filter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/phasing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/shift.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/smooth.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/smooth.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/utils.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.4/spectrochempy/core/processors/zero_filling.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 __dataset_methods__ = __all__
 
 import functools
 
 import numpy as np
 
 from spectrochempy.core import error_
-from spectrochempy.core.dataset.coord import LinearCoord
 from spectrochempy.utils.misc import largest_power_of_2
 
 
 # ======================================================================================
 # Decorators
 # ======================================================================================
 def _zf_method(method):
@@ -35,43 +34,47 @@
 
         swapped = False
         if axis != -1:
             new.swapdims(axis, -1, inplace=True)  # must be done in  place
             swapped = True
 
         x = new.coordset[dim]
+
+        if not x.linear:
+            # this method is not valid for non-linear coordinates
+            error_(
+                "zero-filling apply only to linear coordinates\n"
+                "The processing was thus cancelled"
+            )
+            return dataset  # return the original dataset
+
         if hasattr(x, "_use_time_axis"):
-            x._use_time_axis = True  # we need to havze dimentionless or time units
+            x._use_time_axis = True  # we need to have dimensionless or time units
 
         # get the lastcoord
         if x.unitless or x.dimensionless or x.units.dimensionality == "[time]":
-
-            if not x.linear:
-                # This method apply only to linear coordinates.
-                # we try to linearize it
-                x = LinearCoord(x)
-
-            if not x.linear:
-                raise TypeError("Coordinate x is not linearisable")
-
+            # we can apply the method
             data = method(new.data, **kwargs)
             new._data = data
 
-            # we needs to increase the x coordinates array
-            x._size = new._data.shape[-1]
-
+            # we need to increase the x coordinates array to match the new data size
+            offset = x.data[0]
+            size = x.size
+            inc = x._data.ptp() / (size - 1)
+            x._data = np.arange(offset, offset + new._data.shape[-1] * inc, inc)
             # update with the new td
             new.meta.td[-1] = x.size
             new.history = f"`{method.__name__}` shift performed on dimension `{dim}` with parameters: {kwargs}"
 
         else:
             error_(
                 "zero-filling apply only to dimensions with [time] dimensionality or dimensionless coords\n"
                 "The processing was thus cancelled"
             )
+            return dataset  # return the original dataset
 
         # restore original data order if it was swapped
         if swapped:
             new.swapdims(axis, -1, inplace=True)  # must be done inplace
 
         return new
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.4/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/project/project.py` & `spectrochempy-0.6.4/spectrochempy/core/project/project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/download.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
     >>> scp.read('irdata\\\\OPUS\\\\test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Reading a single OPUS file  (providing a unix/python type filename relative
     to the default ``datadir`` )
     Note that here read_opus is called as a classmethod of the NDDataset class
 
-    >>> scp.NDDataset.read('irdata/OPUS/test.0000')
+    >>> scp.read('irdata/OPUS/test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Single file specified with pathlib.Path object
 
     >>> from pathlib import Path
     >>> folder = Path('irdata/OPUS')
     >>> p = folder / 'test.0000'
@@ -550,15 +550,15 @@
     --------
 
     >>> scp.preferences.csv_delimiter = ','
     >>> A = scp.read_dir('irdata')
     >>> len(A)
     4
 
-    >>> B = scp.NDDataset.read_dir()
+    >>> B = scp.read_dir()
     """
     kwargs["iterdir"] = True
     importer = Importer()
     return importer(directory, **kwargs)
 
 
 # _docstring.delete_params("Importer.see_also", "read_remote")
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_carroucell.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     if ";" in txt:
         # look like the delimiter is ;
         # if comma is also present, it could be that french writer was used.
         txt = txt.replace(",", ".")
         delimiter = ";"
 
     d = [row for row in csv.reader(txt.splitlines(), delimiter=delimiter)]
-    d = np.array(d).T
+    d = np.array(d, dtype=float).T
 
     # First column is the x coordinates
     coordx = Coord(d[0])
 
     # Create a second coordinate for dimension y of size 1
     coordy = Coord([0])
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_labspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __dataset_methods__ = __all__
 
 import datetime
 
 import numpy as np
 
 from spectrochempy.core.dataset.baseobjects.meta import Meta
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 _docstring.delete_params("Importer.see_also", "read_labspec")
@@ -125,21 +125,14 @@
 
     else:
         data = rawdata[1:, 1:]
         _x = Coord(rawdata[0, 1:], title="Raman shift", units="1/cm")
         _y = Coord(rawdata[1:, 0], title="Time", units="s")
         date_acq, _y = _transf_meta(_y, meta)
 
-    # try to transform to linear coord
-    _x.linear = True
-
-    # if success linear should still be True
-    if _x.linear:
-        _x = LinearCoord(_x)
-
     # set dataset metadata
     dataset.data = data
     dataset.set_coordset(y=_y, x=_x)
     dataset.title = "Counts"
     dataset.units = None
     dataset.name = filename.stem
     dataset.meta = meta
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_omnic.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re
 import struct
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 
 from spectrochempy.core import info_
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import ur
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
@@ -79,15 +79,15 @@
     >>> scp.read_omnic('irdata\\\\nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
 
     Reading a single OMNIC file  (providing a unix/python type filename
     relative to the default `datadir` )
     Note that here read_omnic is called as a classmethod of the NDDataset class
 
-    >>> scp.NDDataset.read_omnic('irdata/nh4y-activation.spg')
+    >>> scp.read_omnic('irdata/nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
 
     Single file specified with pathlib.Path object
 
     >>> from pathlib import Path
     >>> folder = Path('irdata')
     >>> p = folder / 'nh4y-activation.spg'
@@ -189,15 +189,15 @@
     read_spa : Read single Omnic spectra.
     read_srs : Read series Omnic spectra.
     %(Importer.see_also.no_read_omnic)s
 
     Notes
     -----
     This method is an alias of `read_omnic`\ , except that the type of file
-    is contrain to ``.spg``.
+    is constrained to ``.spg``.
 
     Examples
     ---------
 
     >>> scp.read_spg('irdata/nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
     """
@@ -476,31 +476,21 @@
     dataset.data = data
     dataset.units = units[0]
     dataset.title = titles[0]
     dataset.name = filename.stem
     dataset.filename = filename
 
     # now add coordinates
-    # _x = Coord(np.around(np.linspace(firstx[0], lastx[0], nx[0]), 3),
-    #           title=xtitles[0], units=xunits[0])
-    spacing = (lastx[0] - firstx[0]) / int(nx[0] - 1)
-    _x = LinearCoord(
-        offset=firstx[0],
-        increment=spacing,
-        size=int(nx[0]),
+    _x = Coord.linspace(
+        firstx[0],
+        lastx[0],
+        nx[0],
         title=xtitles[0],
         units=xunits[0],
     )
-    # _x = Coord.linspace(
-    #     firstx[0],
-    #     lastx[0],
-    #     int(nx[0]),
-    #     title=xtitles[0],
-    #     units=xunits[0],
-    # )
 
     _y = Coord(
         timestamps,
         title="acquisition timestamp (GMT)",
         units="s",
         labels=(acquisitiondates, spectitles),
     )
@@ -665,50 +655,38 @@
         # now add coordinates
         nx = info["nx"]
         firstx = info["firstx"]
         lastx = info["lastx"]
         xunit = info["xunits"]
         xtitle = info["xtitle"]
 
-        spacing = (lastx - firstx) / (nx - 1)
-
-        # _x = Coord.linspace(
-        #     firstx,
-        #     lastx,
-        #     int(nx),
-        #     title=xtitle,
-        #     units=xunit,
-        # )
-        _x = LinearCoord(
-            offset=firstx, increment=spacing, size=nx, title=xtitle, units=xunit
+        _x = Coord.linspace(
+            firstx,
+            lastx,
+            int(nx),
+            title=xtitle,
+            units=xunit,
         )
 
     else:  # interferogram
         if return_ifg == "sample":
             default_description = (
                 f"# Omnic name: {spa_name} : sample IFG\n # Filename: {filename.name}"
             )
         else:
             default_description = f"# Omnic name: {spa_name} : background IFG\n # Filename: {filename.name}"
         spa_name += ": Sample IFG"
         dataset.units = "V"
         dataset.title = "detector signal"
-        _x = LinearCoord(
-            offset=0,
-            increment=1,
-            size=len(intensities),
+
+        _x = Coord.arange(
+            len(intensities),
             title="data points",
             units=None,
         )
-        #
-        # _x = Coord.arange(
-        #     len(intensities),
-        #     title="data points",
-        #     units=None,
-        # )
 
     dataset.set_coordset(y=_y, x=_x)
     dataset.name = spa_name  # to be consistent with omnic behaviour
     dataset.filename = str(filename)
 
     # Set origin, description, history, date
     # Omnic spg file don't have specific "origin" field stating the oirigin of the data
@@ -860,26 +838,18 @@
     dataset.mask = np.isnan(dataset.data)
 
     dataset.units = info["units"]
     dataset.title = info["title"]
     dataset.origin = "omnic"
 
     # now add coordinates
-    spacing = (info["lastx"] - info["firstx"]) / (info["nx"] - 1)
-    # _x = Coord.linspace(
-    #     info["firstx"],
-    #     info["lastx"],
-    #     int(info["nx"]),
-    #     title=info["xtitle"],
-    #     units=info["xunits"],
-    # )
-    _x = LinearCoord(
-        offset=info["firstx"],
-        increment=spacing,
-        size=info["nx"],
+    _x = Coord.linspace(
+        info["firstx"],
+        info["lastx"],
+        int(info["nx"]),
         title=info["xtitle"],
         units=info["xunits"],
     )
 
     # specific infos for series data
     if not return_bg:
         dataset.name = info["name"]
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_opus.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 from brukeropusreader.opus_parser import parse_data, parse_meta
 
 from spectrochempy.core import debug_
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 _docstring.delete_params("Importer.see_also", "read_opus")
@@ -72,34 +72,38 @@
     >>> p = folder / 'test.0000'
     >>> scp.read_opus(p)
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Multiple files not merged (return a list of datasets). Note that a directory is
     specified
 
-    >>> le = scp.read_opus('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
+    >>> le = scp.read_opus('test.0000', 'test.0001', 'test.0002',
+    >>>                    directory='irdata/OPUS')
     >>> len(le)
     3
     >>> le[0]
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Multiple files merged as the `merge` keyword is set to true
 
-    >>> scp.read_opus('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
+    >>> scp.read_opus('test.0000', 'test.0001', 'test.0002',
+    directory='irdata/OPUS', merge=True)
     NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
     Multiple files to merge : they are passed as a list instead of using the keyword `
     merge`
 
-    >>> scp.read_opus(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
+    >>> scp.read_opus(['test.0000', 'test.0001', 'test.0002'],
+    >>>               directory='irdata/OPUS')
     NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
     Multiple files not merged : they are passed as a list but `merge` is set to false
 
-    >>> le = scp.read_opus(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
+    >>> le = scp.read_opus(['test.0000', 'test.0001', 'test.0002'],
+    >>>                    directory='irdata/OPUS', merge=False)
     >>> len(le)
     3
 
     Read without a filename. This has the effect of opening a dialog for file(s)
     selection
 
     >>> nd = scp.read_opus()
@@ -139,37 +143,39 @@
     # data
     try:
         npt = opus_data["AB Data Parameter"]["NPT"]
         data = opus_data["AB"][:npt]
         dataset.data = np.array(data[np.newaxis], dtype="float32")
     except KeyError:
         raise KeyError(
-            f"{filename} is not an Absorbance spectrum. It cannot be read with the `read_opus` import method"
+            f"{filename} is not an Absorbance spectrum. It cannot be read with the "
+            f"`read_opus` import method"
         )
     # todo: read background
 
     # xaxis
     fxv = opus_data["AB Data Parameter"]["FXV"]
     lxv = opus_data["AB Data Parameter"]["LXV"]
-    # xdata = linspace(fxv, lxv, npt)
-    xaxis = LinearCoord.linspace(fxv, lxv, npt, title="wavenumbers", units="cm^-1")
+    xaxis = Coord.linspace(fxv, lxv, npt)
 
     # yaxis
     name = opus_data["Sample"]["SNM"]
     acqdate = opus_data["AB Data Parameter"]["DAT"]
     acqtime = opus_data["AB Data Parameter"]["TIM"]
     gmt_offset_hour = float(acqtime.split("GMT")[1].split(")")[0])
     if len(acqdate.split("/")[0]) == 2:
         date_time = datetime.strptime(
             acqdate + "_" + acqtime.split()[0], "%d/%m/%Y_%H:%M:%S.%f"
         )
     elif len(acqdate.split("/")[0]) == 4:
         date_time = datetime.strptime(
             acqdate + "_" + acqtime.split()[0], "%Y/%m/%d_%H:%M:%S"
         )
+    else:  # pragma: no cover
+        raise ValueError("acqdate can not be interpreted.")
     utc_dt = date_time - timedelta(hours=gmt_offset_hour)
     utc_dt = utc_dt.replace(tzinfo=timezone.utc)
     timestamp = utc_dt.timestamp()
 
     yaxis = Coord(
         [timestamp],
         title="acquisition timestamp (GMT)",
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_quadera.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_soc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_spc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 import struct
 from datetime import datetime
 from warnings import warn
 
 import numpy as np
 
-from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import Quantity
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 _docstring.delete_params("Importer.see_also", "read_spc")
 
 
 @_docstring.dedent
 def read_spc(*paths, **kwargs):
+    # type: (*str, **kwargs) -> NDDataset
     """
     Read GRAMS/Thermo Scientific Galactic files or a list of files with extension :file:`.spc`\ .
 
     Parameters
     ----------
     %(Importer.parameters)s
 
@@ -425,22 +426,22 @@
     #         w_unit = x_or_z_unit[ixtype]
     #         w_title = x_or_z_title[ixtype]
     #     else:
     #         w_unit = None
     #         w_title = "Double interferogram"
 
     if not txvals:  # evenly spaced x data
-        spacing = (Flast - Ffirst) / (Fnpts - 1)
-        _x = LinearCoord(
-            offset=Ffirst,
-            increment=spacing,
-            size=Fnpts,
+        _x = Coord.linspace(
+            Ffirst,
+            Flast,
+            Fnpts,
             title=x_title,
             units=x_unit,
         )
+
     else:
         _x = Coord(
             data=np.frombuffer(content, offset=512, dtype=float32_dtype, count=Fnpts),
             title=x_title,
             units=x_unit,
         )
 
@@ -491,15 +492,22 @@
         dataset.description += "Instrumental Technique: " + technique + "\n"
     if Fres != b"\x00\x00\x00\x00\x00\x00\x00\x00\x00":
         dataset.description += "Resolution: " + sres + "\n"
     if Fsource != b"\x00\x00\x00\x00\x00\x00\x00\x00\x00":
         dataset.description += "Source Instrument: " + ssource + "\n"
     if (
         Fcmnt
-        != b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        != b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
+        b"\x00\x00\x00\x00"
     ):
         dataset.description += "Memo: " + scmnt + "\n"
     if Flogoff:
         if Logtxto:
             dataset.description += "Log Text: \n---------\n"
             dataset.description += logtxt
             dataset.description += "---------\n"
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_topspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re
 
 import numpy as np
 from quaternion import as_quat_array
 
 from spectrochempy.core import debug_
 from spectrochempy.core.dataset.baseobjects.meta import Meta
-from spectrochempy.core.dataset.coord import LinearCoord
+from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.core.units import ur
 from spectrochempy.extern.nmrglue import read_fid, read_pdata
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Constants
@@ -992,34 +992,29 @@
     coords = []
     axe_range = list(range(parmode + 1))
 
     for axis in axe_range:
         if not meta.isfreq[axis]:
             # the axis is in time units
             dw = (1.0 / meta.sw_h[axis]).to("us")
-            # coordpoints = np.arange(meta.td[axis])
-            # coord = Coord(coordpoints * dw,
-            #             title=f"F{axis + 1} acquisition time")  # TODO: use AQSEQ for >2D data
-            coord = LinearCoord(
-                offset=0.0,
-                increment=dw,
-                units="us",
-                size=meta.td[axis],
-                title=f"F{axis + 1} acquisition time",
-            )
+            coordpoints = np.arange(meta.td[axis])
+            coord = Coord(
+                coordpoints * dw, title=f"F{axis + 1} acquisition time"
+            )  # TODO: use AQSEQ for >2D data
+
             coord.meta.larmor = meta.sfo1[axis]
             coords.append(coord)
         else:
             size = meta.si[axis]
             sizem = max(size - 1, 1)
             deltaf = -meta.sw_h[axis] / sizem
             first = meta.sfo1[axis] - meta.sf[axis] - deltaf * sizem / 2.0
 
-            # coord = Coord(np.arange(size) * deltaf + first)
-            coord = LinearCoord(offset=first, increment=deltaf, size=size)
+            coordpoints = np.arange(size) * deltaf + first
+            coord = Coord(coordpoints)
             coord.meta.larmor = meta.sfo1[axis]  # needed for ppm transformation
             coord.ito("ppm")
             if meta.nuc1 is not None:
                 nuc1 = meta.nuc1[axis]
                 regex = r"([^a-zA-Z]+)([a-zA-Z]+)"
                 m = re.match(regex, nuc1)
                 mass = m[1]
```

### Comparing `spectrochempy-0.6.3/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.4/spectrochempy/core/readers/read_zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.4/spectrochempy/core/script/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.4/spectrochempy/core/units/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.4/spectrochempy/core/writers/exporter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.4/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.4/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.4/spectrochempy/core/writers/write_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.4/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.4/spectrochempy/extern/nmrglue.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.4/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.4/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.4/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.4/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/citation.py` & `spectrochempy-0.6.4/spectrochempy/utils/citation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/constants.py` & `spectrochempy-0.6.4/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.4/spectrochempy/utils/coordrange.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/decorators.py` & `spectrochempy-0.6.4/spectrochempy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.4/spectrochempy/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.4/spectrochempy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/fake.py` & `spectrochempy-0.6.4/spectrochempy/utils/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         data=st, units="absorbance", title="absorbance", coordset=[range(len(st)), x]
     )
 
     return st
 
 
 def _make_concentrations_matrix(*profiles):
-    from spectrochempy.core.dataset.coord import LinearCoord
+    from spectrochempy.core.dataset.coord import Coord
     from spectrochempy.core.dataset.nddataset import NDDataset
 
-    t = LinearCoord(np.linspace(0, 10, 50), units="hour", title="time")
+    t = Coord(np.linspace(0, 10, 50), units="hour", title="time")
     c = []
     for p in profiles:
         c.append(p(t.data))
     ct = np.vstack(c)
     ct = ct - np.min(ct)
     if ct.shape[0] > 1:
         ct = ct / np.sum(ct, axis=0)
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/file.py` & `spectrochempy-0.6.4/spectrochempy/utils/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,14 +553,26 @@
             else:
                 filenames_dict[extension] = [filename]
         return filenames_dict
     else:
         return filenames
 
 
+def find_or_create_spectrochempy_dir():
+    directory = Path.home() / ".spectrochempy"
+
+    directory.mkdir(exist_ok=True)  # Create directory only if it does not exist
+
+    if directory.is_file():  # pragma: no cover
+        msg = "Intended SpectroChemPy directory `{0}` is actually a file."
+        raise IOError(msg.format(directory))
+
+    return directory
+
+
 def get_directory_name(directory, **kwargs):
     """
     Return a valid directory name.
 
     Parameters
     ----------
     directory : `str` or `pathlib.Path` object, optional.
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.4/spectrochempy/utils/jsonutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,14 @@
     if byte_obj is None:
         return None
 
     elif hasattr(byte_obj, "_implements"):
 
         objnames = byte_obj.__dir__()
 
-        # particular case of Linear Coordinates
-        if byte_obj._implements("LinearCoord"):
-            objnames.remove("data")
-
         dic = {}
         for name in objnames:
 
             if (
                 name in ["readonly"]
                 or (name == "dims" and "datasets" in objnames)
                 or [name in ["parent", "name"] and isinstance(byte_obj, PreferencesSet)]
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/misc.py` & `spectrochempy-0.6.4/spectrochempy/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,31 +278,14 @@
             return response
 
         return wrapper
 
     return decorated
 
 
-def gt_eps(arr):
-    """
-    Lambda function to check that an array has at least some values greater than
-    epsilon.
-
-    Parameters
-    ----------
-    arr : array to check
-
-    Returns
-    --------
-    bool : results of checking
-        True means that at least some values are greater than epsilon.
-    """
-    return np.any(arr > EPSILON)
-
-
 def htmldoc(text):
     """
     Format docstring in html for a nice display in IPython.
 
     Parameters
     ----------
     text : str
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/objects.py` & `spectrochempy-0.6.4/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/optional.py` & `spectrochempy-0.6.4/spectrochempy/utils/optional.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.4/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/packages.py` & `spectrochempy-0.6.4/spectrochempy/utils/packages.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/plots.py` & `spectrochempy-0.6.4/spectrochempy/utils/plots.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/print.py` & `spectrochempy-0.6.4/spectrochempy/utils/print.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 def pstr(object, **kwargs):
     if hasattr(object, "_implements") and object._implements() in [
         "NDArray",
         "NDComplexArrray",
         "NDDataset",
-        "LinearCoord",
         "Coord",
         "CoordSet",
     ]:
         return object._cstr(**kwargs).strip()
     else:
         return str(object).strip()
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.4/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/system.py` & `spectrochempy-0.6.4/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/testing.py` & `spectrochempy-0.6.4/spectrochempy/utils/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,28 +221,19 @@
     elif data_only:
         attrs = ["data"]
     else:
         attrs = ["data", "labels", "units", "meta", "title"]
         # if 'title' in attrs:  #    attrs.remove('title')
         # #TODO: should we use title for comparison?
 
-    if other.linear == this.linear:
-        # To còmpare linear coordinates
-        attrs += ["offset", "increment", "linear", "size"]
-
     for attr in attrs:
         if attr != "units":
             sattr = getattr(this, f"_{attr}")
-            if this.linear and attr == "data":
-                # allow comparison of LinearCoord and Coord
-                sattr = this.data
             if hasattr(other, f"_{attr}"):
                 oattr = getattr(other, f"_{attr}")
-                if other.linear and attr == "data":
-                    oattr = other.data
                 # to avoid deprecation warning issue for unequal array
                 if sattr is None and oattr is not None:
                     raise AssertionError(f"`{attr}` of {this} is None.")
                 if oattr is None and sattr is not None:
                     raise AssertionError(f"{attr} of {other} is None.")
                 if (
                     hasattr(oattr, "size")
@@ -269,23 +260,14 @@
                             sattr,
                             oattr,
                             header=f"{thistype}.{attr} "
                             f"attributes are not "
                             f"equal",
                         )
 
-                elif attr in ["offset", "increment"] and approx:
-                    assert_approx_equal(
-                        sattr,
-                        oattr,
-                        significant=decimal,
-                        err_msg=f"{thistype}.{attr} attributes "
-                        f"are not almost equal to %d decimals" % decimal,
-                    )
-
                 else:
                     eq &= np.all(sattr == oattr)
 
                 if not eq:
                     raise AssertionError(
                         f"The {attr} attributes of {this} and {other} are "
                         f"different."
@@ -359,15 +341,14 @@
             "history",
             "created",
             "modified",
             "origin",
             "roi",
             "size",
             "name",
-            "show_datapoints",
             "modeldata",
             "processeddata",
             "baselinedata",
             "referencedata",
             "state",
         )
         for attr in exclude:
```

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/traits.py` & `spectrochempy-0.6.4/spectrochempy/utils/traits.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/version.py` & `spectrochempy-0.6.4/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.4/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/utils/zip.py` & `spectrochempy-0.6.4/spectrochempy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.4/spectrochempy/widgets/baselinecorrector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.4/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.3/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.4/spectrochempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.3
+Version: 0.6.4
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

