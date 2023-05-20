# Comparing `tmp/absplit-0.1.4.tar.gz` & `tmp/absplit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-0.1.4.tar", last modified: Thu Feb 16 15:16:57 2023, max compression
+gzip compressed data, was "absplit-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-0.1.4.tar` & `absplit-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4705 2023-02-16 15:05:20.274372 absplit-0.1.4/.gitignore
--rw-r--r--   0        0        0       47 2023-02-16 15:05:20.276086 absplit-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      657 2023-02-16 15:05:20.277785 absplit-0.1.4/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      174 2022-10-17 07:17:04.582000 absplit-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      191 2023-02-16 15:05:20.279114 absplit-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      286 2023-02-16 15:05:20.282421 absplit-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2023-02-16 15:05:20.283927 absplit-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0     1022 2023-02-16 15:05:20.285595 absplit-0.1.4/LICENSE
--rw-r--r--   0        0        0      147 2023-02-16 15:05:20.300520 absplit-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0     3897 2023-02-16 15:16:07.815260 absplit-0.1.4/README.md
--rw-r--r--   0        0        0       60 2023-02-16 15:16:07.820869 absplit-0.1.4/absplit/__init__.py
--rw-r--r--   0        0        0     8001 2023-02-16 15:05:20.305310 absplit-0.1.4/absplit/data.py
--rw-r--r--   0        0        0    19158 2023-02-16 15:05:20.306679 absplit-0.1.4/absplit/ga.py
--rw-r--r--   0        0        0     1808 2023-02-16 15:05:20.307962 absplit-0.1.4/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-05 15:15:17.012000 absplit-0.1.4/images/logo.jpeg
--rw-r--r--   0        0        0     1429 2023-02-16 15:16:07.818409 absplit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-02-16 15:05:20.310458 absplit-0.1.4/requirements.txt
--rw-r--r--   0        0        0        0 2023-01-10 22:15:38.957000 absplit-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     5787 2023-02-16 15:05:20.313522 absplit-0.1.4/tests/test_data.py
--rw-r--r--   0        0        0     2027 2023-02-16 15:05:20.319365 absplit-0.1.4/tests/test_ga.py
--rw-r--r--   0        0        0     5074 1970-01-01 00:00:00.000000 absplit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-05-20 17:44:37.211000 absplit-0.1.5/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-02-18 09:50:13.578000 absplit-0.1.5/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      193 2023-02-18 09:50:13.614000 absplit-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-0.1.5/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0     6030 2023-05-20 17:38:11.538000 absplit-0.1.5/README.md
+-rw-r--r--   0        0        0       62 2023-05-20 17:44:37.289000 absplit-0.1.5/absplit/__init__.py
+-rw-r--r--   0        0        0     8213 2023-05-20 17:32:17.963000 absplit-0.1.5/absplit/data.py
+-rw-r--r--   0        0        0    19949 2023-05-20 16:53:44.320000 absplit-0.1.5/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-0.1.5/absplit/param.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-0.1.5/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-05-20 17:47:05.965000 absplit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-20 08:12:29.431000 absplit-0.1.5/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-0.1.5/tests/test_data.py
+-rw-r--r--   0        0        0     2105 2023-02-18 09:46:26.249000 absplit-0.1.5/tests/test_ga.py
+-rw-r--r--   0        0        0     7095 1970-01-01 00:00:00.000000 absplit-0.1.5/PKG-INFO
```

### Comparing `absplit-0.1.4/.gitignore` & `absplit-0.1.5/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -1,243 +1,244 @@
-archive/
-data/
-notebooks/
-.pypirc
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
-# Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
-# Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
-
-# User-specific stuff
-.idea/**/workspace.xml
-.idea/**/tasks.xml
-.idea/**/usage.statistics.xml
-.idea/**/dictionaries
-.idea/**/shelf
-
-# AWS User-specific
-.idea/**/aws.xml
-
-# Generated files
-.idea/**/contentModel.xml
-
-# Sensitive or high-churn files
-.idea/**/dataSources/
-.idea/**/dataSources.ids
-.idea/**/dataSources.local.xml
-.idea/**/sqlDataSources.xml
-.idea/**/dynamic.xml
-.idea/**/uiDesigner.xml
-.idea/**/dbnavigator.xml
-
-# Gradle
-.idea/**/gradle.xml
-.idea/**/libraries
-
-# Gradle and Maven with auto-import
-# When using Gradle or Maven with auto-import, you should exclude module files,
-# since they will be recreated, and may cause churn.  Uncomment if using
-# auto-import.
-# .idea/artifacts
-# .idea/compiler.xml
-# .idea/jarRepositories.xml
-# .idea/modules.xml
-# .idea/*.iml
-# .idea/modules
-# *.iml
-# *.ipr
-
-# CMake
-cmake-build-*/
-
-# Mongo Explorer plugin
-.idea/**/mongoSettings.xml
-
-# File-based project format
-*.iws
-
-# IntelliJ
-out/
-
-# mpeltonen/sbt-idea plugin
-.idea_modules/
-
-# JIRA plugin
-atlassian-ide-plugin.xml
-
-# Cursive Clojure plugin
-.idea/replstate.xml
-
-# SonarLint plugin
-.idea/sonarlint/
-
-# Crashlytics plugin (for Android Studio and IntelliJ)
-com_crashlytics_export_strings.xml
-crashlytics.properties
-crashlytics-build.properties
-fabric.properties
-
-# Editor-based Rest Client
-.idea/httpRequests
-
-# Android studio 3.1+ serialized cache file
+archive/
+data/
+notebooks/
+.pypirc
+notes.txt
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+
+# Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
+# Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
+
+# User-specific stuff
+.idea/**/workspace.xml
+.idea/**/tasks.xml
+.idea/**/usage.statistics.xml
+.idea/**/dictionaries
+.idea/**/shelf
+
+# AWS User-specific
+.idea/**/aws.xml
+
+# Generated files
+.idea/**/contentModel.xml
+
+# Sensitive or high-churn files
+.idea/**/dataSources/
+.idea/**/dataSources.ids
+.idea/**/dataSources.local.xml
+.idea/**/sqlDataSources.xml
+.idea/**/dynamic.xml
+.idea/**/uiDesigner.xml
+.idea/**/dbnavigator.xml
+
+# Gradle
+.idea/**/gradle.xml
+.idea/**/libraries
+
+# Gradle and Maven with auto-import
+# When using Gradle or Maven with auto-import, you should exclude module files,
+# since they will be recreated, and may cause churn.  Uncomment if using
+# auto-import.
+# .idea/artifacts
+# .idea/compiler.xml
+# .idea/jarRepositories.xml
+# .idea/modules.xml
+# .idea/*.iml
+# .idea/modules
+# *.iml
+# *.ipr
+
+# CMake
+cmake-build-*/
+
+# Mongo Explorer plugin
+.idea/**/mongoSettings.xml
+
+# File-based project format
+*.iws
+
+# IntelliJ
+out/
+
+# mpeltonen/sbt-idea plugin
+.idea_modules/
+
+# JIRA plugin
+atlassian-ide-plugin.xml
+
+# Cursive Clojure plugin
+.idea/replstate.xml
+
+# SonarLint plugin
+.idea/sonarlint/
+
+# Crashlytics plugin (for Android Studio and IntelliJ)
+com_crashlytics_export_strings.xml
+crashlytics.properties
+crashlytics-build.properties
+fabric.properties
+
+# Editor-based Rest Client
+.idea/httpRequests
+
+# Android studio 3.1+ serialized cache file
 .idea/caches/build_file_checksums.ser
```

### Comparing `absplit-0.1.4/LICENSE` & `absplit-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `absplit-0.1.4/absplit/data.py` & `absplit-0.1.5/absplit/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-from absplit.param import ParamMixin
-import pandas as pd
-import numpy as np
-from sklearn import preprocessing
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-class Data(ParamMixin):
-    """Takes population data and manages all the transformations necessary to use it in the genetic algorithm.
-
-    Processes:
-        1) Set indexes as all non-metric columns
-        2) Scale data (if required)
-            So that metrics are weighted more fairly against each other if they're of different scales
-        3) Unstack data by time periods (if required)
-        4) Extract metadata needed for 3D transformation
-            Final output shape needed of dimensions (number of metrics, size of population, number of time periods)
-
-    Attributes:
-        _df_stacked (pd.DataFrame): Data input from user, indexed on non-metric columns
-        _pre_fit_scaler (object): Scaling object
-        remainder_cols (list): Identifies any columns not specified by the user
-        _df_unstacked (pd.DataFrame): Data input from user, unstacked by time periods
-        _df_index (pd.DataFrame): Empty index from _df_unstacked
-        num_metrics (int): Number of metrics specified
-        time_periods (int): Number of time periods in data
-        pop_size (int): Size of population that is getting split/matched
-        splitting_values (np.array): IDs of each member of the population being split
-        reshape_tup (tuple): Tuple of ints, representing 3D array dimensions
-
-    Properties:
-        stacked (pd.DataFrame): Data as entered, but indexed
-        unstacked (pd.DataFrame): Data scaled (if required) and unstacked by time period (if required)
-        index (pd.DataFrame): Empty index from unstacked dataframe
-        matrix (np.array): 3D matrix of transformed data
-
-    Methods:
-        _check_columns_object(): Prints warning if any remainder columns are of type object
-        _extract_metadata(): Extracts metadata of dataframe dimensions
-        _set_indexes(): Sets indexes for data passed
-        _unstack(): Unstacks data by time periods (if applicable)
-        _scale(): Scales the metrics
-        filter(index): Uses index to filter dataframe
-        assign(solution): Maps solution (binary numpy array) to unstacked dataframe index
-    """
-
-    def __init__(self, df, scaler=None, scale=True, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            df (pd.DataFrame): Dataframe to process
-            scaler (object, optional): Scaling function object. Default None
-            scale (bool, optional): To apply scaling to data or not. Default True
-            **kwargs: Additional keyword arguments
-        """
-
-        super().__init__(**kwargs)
-        self._df_stacked = df
-        self._pre_fit_scaler = scaler
-        self._scaler_flag = scale
-        self.remainder_cols = [x for x in self._df_stacked.columns if x not in self.all_spec_columns]
-        self._df_unstacked = None
-        self._df_index = None
-        self.num_metrics = None
-        self.time_periods = None
-        self.pop_size = None
-        self.splitting_values = None
-        self.reshape_tup = None
-
-        logger.debug(f'Remainder: {self.remainder_cols}, dim_spec: {self.dim_spec_columns}, metric:{self.metrics}')
-
-        self._check_columns_object()
-
-        # Transformations
-        self._df_stacked = self._set_indexes()
-        self._df_unstacked = self._df_stacked.copy()
-        self._df_unstacked = self._scale()
-        self._df_unstacked = self._unstack()
-
-        # Extract unstacked index
-        self._df_index = pd.DataFrame(index=self._df_unstacked.index)
-
-        self._extract_metadata()
-
-        logger.debug(f'shape: {self._df_unstacked.shape}, reshape dims: {self.reshape_tup}, num_genes: {self.pop_size}')
-
-    def _check_columns_object(self):
-        """Prints warning if any remainder columns are not of type object
-
-        Returns:
-            None
-        """
-        for col in self.remainder_cols:
-            dtype = self._df_stacked[col].dtype
-            if not dtype == 'object':
-                print(f'Column \'{col}\' will be treated as a variable to split on. Normally additional splitting'
-                      f'columns are of type object, this is type {dtype}, this could cause problems in splitting. '
-                      'Please check your kwargs are correct and remove any metrics you dont intend on splitting on.')
-
-    def _extract_metadata(self):
-        """Extracts metadata used for 3D transformation from unstacked dataframe, builds transformation tuple
-
-        Returns:
-            None
-        """
-
-        # Extract metadata
-        self.num_metrics = len(self.metrics)
-        self.time_periods = int(self._df_unstacked.shape[1] / self.num_metrics)
-        self.pop_size = self._df_unstacked.shape[0]
-        self.splitting_values = self._df_unstacked.index.get_level_values(self.splitting).to_numpy()
-        self.reshape_tup = (self.pop_size, self.num_metrics, self.time_periods)
-
-    def _set_indexes(self):
-        """Sets indexes for the dataframe passed.
-
-        If user passes dataframe with a column which is not specified by one of the input
-        args (date_col, split_by etc) then it is considered a remainder col.
-
-        This is indexed because it is assumed this is important for unique identification.
-        For example if users wants to split all counties in the US, they will also need to pass
-        the state name as some county names will be duplicates. Even though this column isn't
-        specified as an argument, it is still relevant.
-
-        Return:
-            pd.DataFrame
-        """
-
-        columns = self.remainder_cols + self.dim_spec_columns  # Specifies order of columns
-        logger.debug(f'Indexes set: {columns}')
-        return self._df_stacked.set_index(columns).sort_index()
-
-    def _unstack(self):
-        """Unstack date column if date columns is passed
-
-        Returns:
-            pd.DataFrame
-        """
-
-        return self._df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col else self._df_stacked
-
-    def _scale(self):
-        """Standardise all metrics so all metrics weighted as equally as possible
-
-        Returns:
-            pd.DataFrame
-        """
-
-        if self._pre_fit_scaler:
-            scaler = self._pre_fit_scaler
-        else:
-            scaler = preprocessing.MinMaxScaler()
-            scaler.fit(self._df_stacked[self.metrics])
-
-        df = self._df_stacked.copy()
-        if self._scaler_flag:
-            df[self.metrics] = scaler.transform(self._df_stacked[self.metrics])
-        return df
-
-    def filter(self, index):
-        """Takes empty dataframe index 'index' and inner joins on unstacked data to return a filtered version.
-
-        Used when splitting out sample and population dataframes from concatenated dataframe when using
-        Match class
-
-        Args:
-            index (pd.DataFame): Indexes to filter for
-
-        Returns:
-            pd.DataFrame
-        """
-        return self._df_unstacked.stack(self.date_col).join(index, how='inner')
-
-    @property
-    def unstacked(self):
-        return self._df_unstacked
-
-    @property
-    def stacked(self):
-        return self._df_stacked
-
-    @property
-    def index(self):
-        return self._df_index
-
-    @property
-    def matrix(self):
-        """Returns 3D matrix of shape (no_metrics, no_splitting, no_days)
-
-        Returns:
-            np.array
-        """
-
-        return self._df_unstacked.values.reshape(self.reshape_tup).transpose(1, 0, 2)
-
-    def assign(self, solution):
-        """Assigns genetic algorithm solution (binary numpy array) to dataframe index.
-
-        Returned dataframe is the labelled (with index) solution to the splitting problem.
-
-        Returns:
-            pd.DataFrame
-        """
-
-        if solution is None:
-            solution = np.array([None])
-        df_assigned = self.index.copy()
-        df_assigned.insert(loc=0, column='bin', value=solution.reshape(-1, 1))
-        return df_assigned
+from absplit.param import ParamMixin
+import pandas as pd
+import numpy as np
+from sklearn import preprocessing
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+class Data(ParamMixin):
+    """Takes population data and manages all the transformations necessary to use it in the genetic algorithm.
+
+    Processes:
+        1) Set indexes as all non-metric columns
+        2) Scale data (if required)
+            So that metrics are weighted more fairly against each other if they're of different scales
+        3) Unstack data by time periods (if required)
+        4) Extract metadata needed for 3D transformation
+            Final output shape needed of dimensions (number of metrics, size of population, number of time periods)
+
+    Attributes:
+        _df_stacked (pd.DataFrame): Data input from user, indexed on non-metric columns
+        _pre_fit_scaler (object): Scaling object
+        remainder_cols (list): Identifies any columns not specified by the user
+        _df_unstacked (pd.DataFrame): Data input from user, unstacked by time periods
+        _df_index (pd.DataFrame): Empty index from _df_unstacked
+        num_metrics (int): Number of metrics specified
+        time_periods (int): Number of time periods in data
+        pop_size (int): Size of population that is getting split/matched
+        splitting_values (np.array): IDs of each member of the population being split
+        reshape_tup (tuple): Tuple of ints, representing 3D array dimensions
+
+    Properties:
+        stacked (pd.DataFrame): Data as entered, but indexed
+        unstacked (pd.DataFrame): Data scaled (if required) and unstacked by time period (if required)
+        index (pd.DataFrame): Empty index from unstacked dataframe
+        matrix (np.array): 3D matrix of transformed data
+
+    Methods:
+        _check_columns_object(): Prints warning if any remainder columns are of type object
+        _extract_metadata(): Extracts metadata of dataframe dimensions
+        _set_indexes(): Sets indexes for data passed
+        _unstack(): Unstacks data by time periods (if applicable)
+        _scale(): Scales the metrics
+        filter(index): Uses index to filter dataframe
+        assign(solution): Maps solution (binary numpy array) to unstacked dataframe index
+    """
+
+    def __init__(self, df, scaler=None, scale=True, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            df (pd.DataFrame): Dataframe to process
+            scaler (object, optional): Scaling function object. Default None
+            scale (bool, optional): To apply scaling to data or not. Default True
+            **kwargs: Additional keyword arguments
+        """
+
+        super().__init__(**kwargs)
+        self._df_stacked = df
+        self._pre_fit_scaler = scaler
+        self._scaler_flag = scale
+        self.remainder_cols = [x for x in self._df_stacked.columns if x not in self.all_spec_columns]
+        self._df_unstacked = None
+        self._df_index = None
+        self.num_metrics = None
+        self.time_periods = None
+        self.pop_size = None
+        self.splitting_values = None
+        self.reshape_tup = None
+
+        logger.debug(f'Remainder: {self.remainder_cols}, dim_spec: {self.dim_spec_columns}, metric:{self.metrics}')
+
+        self._check_columns_object()
+
+        # Transformations
+        self._df_stacked = self._set_indexes()
+        self._df_unstacked = self._df_stacked.copy()
+        self._scale()
+        self._unstack()
+
+        # Extract unstacked index
+        self._df_index = pd.DataFrame(index=self._df_unstacked.index)
+
+        self._extract_metadata()
+
+        logger.debug(f'shape: {self._df_unstacked.shape}, reshape dims: {self.reshape_tup}, num_genes: {self.pop_size}')
+
+    def _check_columns_object(self):
+        """Prints warning if any remainder columns are not of type object
+
+        Returns:
+            None
+        """
+        for col in self.remainder_cols:
+            dtype = self._df_stacked[col].dtype
+            if not dtype == 'object':
+                print(f'Column \'{col}\' will be treated as a variable to split on. Normally additional splitting'
+                      f'columns are of type object, this is type {dtype}, this could cause problems in splitting. '
+                      'Please check your kwargs are correct and remove any metrics you dont intend on splitting on.')
+
+    def _extract_metadata(self):
+        """Extracts metadata used for 3D transformation from unstacked dataframe, builds transformation tuple
+
+        Returns:
+            None
+        """
+
+        # Extract metadata
+        self.num_metrics = len(self.metrics)
+        self.time_periods = int(self._df_unstacked.shape[1] / self.num_metrics)
+        self.pop_size = self._df_unstacked.shape[0]
+        self.splitting_values = self._df_unstacked.index.get_level_values(self.splitting).to_numpy()
+        self.reshape_tup = (self.pop_size, self.num_metrics, self.time_periods)
+
+    def _set_indexes(self):
+        """Sets indexes for the dataframe passed.
+
+        If user passes dataframe with a column which is not specified by one of the input
+        args (date_col, split_by etc) then it is considered a remainder col.
+
+        This is indexed because it is assumed this is important for unique identification.
+        For example if users wants to split all counties in the US, they will also need to pass
+        the state name as some county names will be duplicates. Even though this column isn't
+        specified as an argument, it is still relevant.
+
+        Return:
+            pd.DataFrame
+        """
+
+        columns = self.remainder_cols + self.dim_spec_columns  # Specifies order of columns
+        logger.debug(f'Indexes set: {columns}')
+        return self._df_stacked.set_index(columns).sort_index()
+
+    def _unstack(self):
+        """Unstack date column if date columns is passed
+
+        Returns:
+            pd.DataFrame
+        """
+
+        self._df_unstacked = self._df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col \
+            else self._df_stacked
+
+    def _scale(self):
+        """Standardise all metrics so all metrics weighted as equally as possible
+
+        Returns:
+            pd.DataFrame
+        """
+
+        if self._pre_fit_scaler:
+            scaler = self._pre_fit_scaler
+        else:
+            scaler = preprocessing.MinMaxScaler()
+            scaler.fit(self._df_stacked[self.metrics])
+
+        self._df_unstacked = self._df_stacked.copy()
+        if self._scaler_flag:
+            self._df_unstacked [self.metrics] = scaler.transform(self._df_stacked[self.metrics])
+
+    def filter(self, index):
+        """Takes empty dataframe index 'index' and inner joins on unstacked data to return a filtered version.
+
+        Used when splitting out sample and population dataframes from concatenated dataframe when using
+        Match class
+
+        Args:
+            index (pd.DataFame): Indexes to filter for
+
+        Returns:
+            pd.DataFrame
+        """
+        return self._df_unstacked.stack(self.date_col).join(index, how='inner')
+
+    @property
+    def unstacked(self):
+        return self._df_unstacked
+
+    @property
+    def stacked(self):
+        return self._df_stacked
+
+    @property
+    def index(self):
+        return self._df_index
+
+    @property
+    def matrix(self):
+        """Returns 3D matrix of shape (no_metrics, no_splitting, no_days)
+
+        Returns:
+            np.array
+        """
+
+        return self._df_unstacked.values.reshape(self.reshape_tup).transpose(1, 0, 2)
+
+    def assign(self, solution):
+        """Assigns genetic algorithm solution (binary numpy array) to dataframe index.
+
+        Returned dataframe is the labelled (with index) solution to the splitting problem.
+
+        Returns:
+            pd.DataFrame
+        """
+
+        if solution is None:
+            solution = np.array([None])
+        df_assigned = self.index.copy()
+        df_assigned.insert(loc=0, column='bin', value=solution.reshape(-1, 1))
+        return df_assigned
```

### Comparing `absplit-0.1.4/absplit/ga.py` & `absplit-0.1.5/absplit/ga.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,566 +1,567 @@
-from absplit.param import ParamMixin
-from absplit.data import Data
-import pandas as pd
-import pygad
-import logging
-import numpy as np
-import matplotlib.pyplot as plt
-import seaborn as sns
-from sklearn import preprocessing
-
-logger = logging.getLogger(__name__)
-
-
-class GAInstance:
-    """Manages initialisation and running of pygad genetic algorithm instance
-
-    Attributes:
-        num_genes (int): Number of members in the population that is being searched
-        ga (pygad.GA): PyGAD GA module
-        solution (np.array): The best solution found in genetic algorith search
-        fitness (np.float): The fitness score of the best solution
-
-    Methods:
-        run(): Runs the genetic algorithm search
-    """
-
-    def __init__(self, num_genes, ga_params):
-        """Class init
-
-        Args:
-            num_genes (int): Number of solutions (genes) in chromosome
-            ga_params (GAParams): GA parameter object
-        """
-
-        self.num_genes = num_genes
-        self.ga = pygad.GA(
-            num_genes=self.num_genes,
-            **ga_params.params
-        )
-        self.solution = None
-        self.fitness = None
-
-    def run(self):
-        """Runs genetic algorithm and returns best solution
-
-        Returns:
-            np.array
-        """
-
-        if self.num_genes > 1:
-            self.ga.run()
-            self.solution, self.fitness, _ = self.ga.best_solution()
-        else:
-            logger.warning('Population size of < 2, skipping')
-            self.solution = None
-            self.fitness = None
-
-
-class GAParams:
-    """Manages PyGAD GA module parameters and any parameter updates
-
-    Attributes:
-        _default_ga_params (dict): Default parameters for genetic algorithm
-        params (dict): PyGAD GA module parameters to be implemented
-
-    """
-
-    def __init__(self, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            **kwargs: Genetic algorithm parameters
-        """
-        global fitness_func_absplit
-
-        # Default parameters
-        self._default_ga_params = dict(
-            # -- General Genetic Algorithm params --
-            num_generations=200,
-            sol_per_pop=100,
-            num_parents_mating=5,
-            mutation_type='swap',
-            mutation_probability=0.1,
-            fitness_func=fitness_func_absplit,
-            keep_elitism=1,
-
-            # -- Binary Genetic Algorithm specific parameters --
-            init_range_low=0,
-            init_range_high=2,
-            random_mutation_min_val=0,
-            random_mutation_max_val=2,
-            gene_type=int,
-        )
-
-        self._dont_touch = [
-            'init_range_low',
-            'init_range_high',
-            'random_mutation_min_val',
-            'random_mutation_max_val',
-            'gene_type'
-        ]
-
-        # Copy default, update
-        self.params = dict(self._default_ga_params)
-        self._update_params(**kwargs)
-
-    def _update_params(self, **kwargs):
-        """Update GA params if any passed
-
-        Returns:
-            None
-        """
-
-        # Update if args passed
-        if kwargs:
-            for key, value in kwargs.items():
-                if key in self._dont_touch:
-                    print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a'\
-                          f'binary genetic algorith, and so youre not allowed to modify this')
-                    continue
-                print(f'Updating {key} to {value}')
-                self.params[key] = value
-
-
-class SplitBase(ParamMixin):
-    """Base class for genetic algorithm orchestration.
-
-    Manages applying different weights to costs, using multiple runs, extracting and visualising results.
-
-    Attributes:
-        _runs (int): Number of runs of the genetic algorithm to try
-        _ga_params (object): GAParams object
-        _best_score (float): Stores best score when using multiple runs
-        _metric_weights (dict): Dictionary of {col_name: value} format for applying differing weights to columns
-        _df (pd.DataFrame): Input data
-        _population (object): Data object
-        _df_result (pd.DataFrame): Proposed solution dataframe
-        _ga (object): GAInstance object
-        _df_vis (pd.DataFrame): DataFrame with solutions used for visualisation
-        _best_ga (object): GAInstance object of the best solution
-        _solution (np.array): Best solution from search
-
-    Properties:
-        results (pd.DataFrame): Accessor for _df_result
-
-    Methods:
-        _cost_weighting(): Modifies cost weighting array
-        run(): Runs the genetic algorithm
-        fitness(): Plot generation fitness graph
-        visualise(): Plots metrics using results from genetic algorithm output
-    """
-
-    def __init__(self, ga_params={}, metric_weights={}, runs=1, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            ga_params (dict, optional): Genetic algorithm parameters to add/modify
-            metric_weights (dict, optional): Cost weightings to apply to metrics
-            runs (int, optional): How many runs to try
-            **kwargs: Additional keyword arguments
-        """
-        super().__init__(**kwargs)
-        if ga_params:
-            assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
-        self._runs = runs
-        self._ga_params = GAParams(**ga_params)
-        self._best_score = -1
-        self._metric_weights = metric_weights
-        self._df = None
-        self._population = None
-        self._df_result = None  # Final results dataframe
-        self._ga = None  # genetic algorithm instance
-        self._df_vis = None  # Visualisation dataframe
-        self._best_ga = None
-        self._solution = None
-
-        self._cost_weighting()
-
-    def _cost_weighting(self):
-        """Set relative cost weights for each metric. Defaults to 1 unless specified.
-
-        Used if you want the genetic algorithm to penalise the MSE cost of some metrics
-        over others. Particularly useful if one metric is quite volatile, as the MSE cost can
-        end up with it prioritising this over others.
-
-        Returns:
-            None
-        """
-        global metric_weights_global
-        metric_weights_global = np.ones(len(self.metrics))
-        if self._metric_weights:
-            for key, value in self._metric_weights.items():
-                try:
-                    i = self.metrics.index(key)
-                    metric_weights_global[i] = value
-                    print(f'{key} weight updated to {value}')
-                except ValueError:
-                    print(f'Cant find metric name {key}, weight {value} not applied, defaulting to 1')
-
-    def run(self):
-        """Runs genetic algorithm and returns bin splits into _df_result
-
-        Returns:
-            None
-        """
-
-        global all_metrics_global
-        logger.debug('Splitting..')
-        all_metrics_global = self._population.matrix
-
-        # Run multiple times, save the best solution
-        for i in range(self._runs):
-            if self._runs > 1:
-                print(f'Run {i+1}')
-
-            # Initialise and run GA, get solution
-            self._ga = GAInstance(
-                num_genes=self._population.pop_size,
-                ga_params=self._ga_params,
-            )
-            self._ga.run()
-
-            if self._ga.fitness > self._best_score:
-                print(f'Best fitness: {self._ga.fitness}')
-                self._solution = self._ga.solution
-                self._best_ga = self._ga
-                self._best_score = self._ga.fitness
-
-        if self._solution is None:
-            raise ValueError('Solution is None')
-
-        # Assign solution to index
-        self._df_result = self._population.assign(self._solution)
-
-        logger.debug('Split complete')
-
-    def fitness(self, title=None):
-        """Plots the fitness-generation graph
-
-        Returns:
-            None
-        """
-
-        if self._best_ga:
-            self._best_ga.ga.plot_fitness(title=title)
-        else:
-            print('No solution available, please use .run() first')
-
-    @property
-    def results(self):
-        """Returns compiled dataframe of solutions
-
-        Returns:
-            pd.DataFrame
-        """
-
-        return self._df_result
-
-    def visualise(self, column=None):
-        """Visualise metrics for both bins and there comparative performances
-
-        Returns:
-            None
-        """
-
-        # Default to all metric columns if no columns specified
-        if column:
-            if isinstance(column, str):
-                column = [column]
-            vis_metrics = column
-        else:
-            vis_metrics = self.metrics
-
-        if self.results is None:
-            print('Must use .run() before visualising')
-            return
-
-        # Aggregate by bin
-        group_cols = ['bin']
-        group_cols += [self.date_col] if self.date_col else []
-        df = self._df_vis.groupby(group_cols)[vis_metrics].sum().reset_index()
-
-        if not len(df):
-            logger.warning(f'Failed vis')
-            return
-
-        sns.set_style('darkgrid')
-
-        # Chart sizing
-        figsize = (min(20, len(vis_metrics)*8), 5) if self.date_col else (8, 5)
-        fig, ax = plt.subplots(1, len(vis_metrics), figsize=figsize)
-        if not hasattr(ax, '__iter__'):
-            ax = [ax]
-
-        # Plot each metric
-        for i, metric in enumerate(vis_metrics):
-
-            # If over time, plot line graph, else bar
-            if self.date_col:
-                sns.lineplot(data=df, x=self.date_col, y=metric, hue='bin', ax=ax[i])
-            else:
-                df['metric'] = metric
-                sns.barplot(data=df, x='metric', y=metric, hue='bin', ax=ax[i])
-
-            ax[i].set_title(f'{metric.title()}')
-            ax[i].tick_params(axis='x', labelrotation=45)
-
-        plt.show()
-
-
-class ABSplit(SplitBase):
-    """Splits data into A/B groups based on specified parameters. All members of the population will be in one bin or
-    the other.
-
-    Attributes:
-        _runs (int): Number of runs of the genetic algorithm to try
-        _ga_params (object): GAParams object
-        _best_score (float): Stores best score when using multiple runs
-        _metric_weights (dict): Dictionary of {col_name: value} format for applying differing weights to columns
-        _df (pd.DataFrame): Input data
-        _population (object): Data object
-        _df_result (pd.DataFrame): Proposed solution dataframe
-        _ga (object): GAInstance object
-        _df_vis (pd.DataFrame): DataFrame with solutions used for visualisation
-        _best_ga (object): GAInstance object of best solution
-        _solution (np.array): Best solution from search
-
-    Properties:
-        results (pd.DataFrame): Accessor for _df_result
-
-    Methods:
-        _cost_weighting(): Modifies cost weighting array
-        run(): Runs the genetic algorithm
-        fitness(): Plot generation fitness graph
-        visualise(): Plots metrics using results from genetic algorithm output
-    """
-
-    def __init__(self, df, ga_params={}, metric_weights={}, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            df (pd.DataFrame): Dataframe to be split
-            ga_params (dict): Parameters for the genetic algorithm (default: {})
-            metric_weights (dict): Weights for each metric in the data (default: {})
-            **kwargs: Additional keyword arguments
-        """
-        super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
-        self.df = df
-        self._population = Data(self.df.copy(), **kwargs)
-
-    def visualise(self, column=None):
-        """Visualizes the A/B split results.
-
-        Returns:
-            None
-        """
-
-        # Merge solution results (_df_results) onto input data (metrics) so that data can be visualised
-        self._df_vis = self._population.stacked.merge(
-            self._df_result,
-            left_index=True,
-            right_index=True
-        )
-        super().visualise(column=column)
-
-    def __repr__(self):
-        lst_str = [f"'{col}', " for col in self.all_spec_columns]
-        return f'ABSplit([{lst_str}])'
-
-
-class MatchDataProc:
-    """Ensures consistent number of dates between sample and population data
-
-    Achieves this by concatenating both dataframes, unstacking by date, then filtering
-    by the index of the sample and population data and restacking.
-
-    Without this, if there are date mismatches between sample and population (e.g.
-    100 distinct date in sample, and 110 in population) then the 2 matrices will be
-    different sizes.
-
-    Defaults missing date values to 0
-
-    Attributes:
-        df_pop (pd.DataFrame): Dataframe of population data
-        df_samp (pd.DataFrame): Dataframe of sample data
-        df_all (pd.DataFrame): Concatenation of df_pop and df_samp
-        all (Data): Instance of the Data class for all data
-        pop (Data): Instance of the Data class for population data
-        samp (Data): Instance of the Data class for sample data
-
-    Properties:
-        sample (pd.DataFrame): Sample data
-        population (pd.DataFrame): Population data
-    """
-
-    def __init__(self, df_pop, df_samp, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            df_pop (pd.DataFrame): Dataframe of population data
-            df_samp (pd.DataFrame): Dataframe of sample data
-            **kwargs: Additional keyword arguments
-        """
-        self.df_pop = df_pop
-        self.df_samp = df_samp
-        self.df_all = pd.concat([df_pop, df_samp], axis=0)
-        self.all = Data(self.df_all, scale=False, **kwargs)
-        self.pop = Data(self.df_pop, scale=False, **kwargs)
-        self.samp = Data(self.df_samp, scale=False, **kwargs)
-
-    @property
-    def sample(self):
-        """Returns the filtered dataframe of sample data
-
-        Returns:
-            pd.DataFrame: Filtered dataframe of sample data
-        """
-        return self.all.filter(self.samp.index)
-
-    @property
-    def population(self):
-        """Returns the filtered dataframe of population data
-
-        Returns:
-            pd.DataFrame: Filtered dataframe of population data
-        """
-        return self.all.filter(self.pop.index)
-
-
-class Match(SplitBase):
-    """Manages a genetic algorithm to find a group in a population with similar properties
-    as a specified sample group. Sample group must be removed from population prior to running
-    Match.
-
-    Attributes:
-        _df_pop (pd.DataFrame): Dataframe of population data
-        _df_samp (pd.DataFrame): Dataframe of sample data
-        _population (Data): Instance of the Data class for population data
-        _sample (Data): Instance of the Data class for sample data
-        _df_result (pd.DataFrame): Dataframe of population data that matches the sample group
-        _df_vis (pd.DataFrame): Dataframe of population data, sample data and matched population data for visualization
-
-    Methods:
-        _broadcast_match(): Makes the match matrix available globally
-        run(): Runs the genetic algorithm
-        fitness(): Plot generation fitness graph
-        visualise(): Plots metrics using results from genetic algorithm output
-    """
-
-    def __init__(self, population, sample, ga_params={}, metric_weights={}, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            population (pd.DataFrame): Dataframe of population data
-            sample (pd.DataFrame): Dataframe of sample data
-            ga_params (dict): Parameters for the genetic algorithm
-            metric_weights (dict): Weights for the metrics being compared
-            **kwargs: Additional keyword arguments
-        """
-
-        # Specify fitness function
-        global fitness_func_match
-        ga_params['fitness_func'] = fitness_func_match
-        ga_params['mutation_type'] = 'scramble'
-        super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
-
-        self._df_pop = population
-        self._df_samp = sample
-
-        # Ensure consistent dates between sample and population
-        if self.date_col:
-            mdp = MatchDataProc(df_pop=self._df_pop, df_samp=self._df_samp, **kwargs)
-            self._df_pop = mdp.population.reset_index()
-            self._df_samp = mdp.sample.reset_index()
-
-        # Fit scaler on combined data
-        scaler = preprocessing.MinMaxScaler()
-        scaler.fit(pd.concat([self._df_pop, self._df_samp], axis=0)[self.metrics])
-
-        self._population = Data(self._df_pop, scaler=scaler, **kwargs)
-        self._sample = Data(self._df_samp, scaler=scaler, **kwargs)
-        self._broadcast_match()
-
-    def _broadcast_match(self):
-        """Makes the match matrix available globally
-
-        Returns:
-            None
-        """
-        global match_metrics_global
-        match_metrics_global = self._sample.matrix
-
-    def run(self):
-        """Runs the genetic algorithm, filters out all except sample and result
-
-        Returns:
-            None
-        """
-        # Run genetic algorithm
-        super().run()
-
-        # Filter on only bin == 1
-        self._df_result = self._df_result[self._df_result['bin'] == 1]
-
-        # Get sample index, set as bin 0, concat to _df_results (which are all bin 1)
-        index_cols = self._sample.index.index.names
-        df_match = self._df_samp[index_cols].drop_duplicates().set_index(index_cols)
-        df_match['bin'] = 0
-        self._df_result = pd.concat([self._df_result, df_match], axis=0).sort_index()
-
-    def visualise(self, column=None):
-        """Visualizes sample and results side by side
-
-        Returns:
-            None
-        """
-
-        # Concat to form entire population
-        self._df_vis = pd.concat([self._population.stacked, self._sample.stacked], axis=0)
-
-        # Inner join to filter out all but sample and match
-        self._df_vis = self._df_vis.merge(
-            self._df_result,
-            left_index=True,
-            right_index=True,
-            how='inner'
-        )
-
-        super().visualise(column=column)
-
-    def __repr__(self):
-        lst_str = [f"'{col}', " for col in self.all_spec_columns]
-        return f'Match([{lst_str}])'
-
-
-def fitness_func_absplit(solution, solution_idx):
-    """Fitness function for ABSplit
-    """
-    global all_metrics_global
-    global metric_weights_global
-
-    cost1 = solution @ all_metrics_global
-    cost2 = (1 - solution) @ all_metrics_global
-    # Average over time axis, sum over metric axis
-    mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
-
-    # Fitness
-    fitness = 1.0 / np.abs(mse)
-    return fitness
-
-
-def fitness_func_match(solution, solution_idx):
-    """Fitness function for Match
-    """
-    global all_metrics_global
-    global match_metrics_global
-    global metric_weights_global
-
-    cost1 = match_metrics_global.sum(1)  # Sum along population axis
-    cost2 = solution @ all_metrics_global
-    # Average over time axis, sum over metric axis
-    mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
-
-    # Fitness
-    fitness = 1.0 / np.abs(mse)
-    return fitness
+from absplit.param import ParamMixin
+from absplit.data import Data
+import pandas as pd
+import pygad
+import logging
+import numpy as np
+import matplotlib.pyplot as plt
+import seaborn as sns
+from sklearn import preprocessing
+
+logger = logging.getLogger(__name__)
+
+
+class GAInstance:
+    """Manages initialisation and running of pygad genetic algorithm instance
+
+    Attributes:
+        num_genes (int): Number of members in the population that is being searched
+        ga (pygad.GA): PyGAD GA module
+        solution (np.array): The best solution found in genetic algorith search
+        fitness (np.float): The fitness score of the best solution
+
+    Methods:
+        run(): Runs the genetic algorithm search
+    """
+
+    def __init__(self, num_genes, ga_params):
+        """Class init
+
+        Args:
+            num_genes (int): Number of solutions (genes) in chromosome
+            ga_params (GAParams): GA parameter object
+        """
+
+        self.num_genes = num_genes
+        self.ga = pygad.GA(
+            num_genes=self.num_genes,
+            **ga_params.params
+        )
+        self.solution = None
+        self.fitness = None
+
+    def run(self):
+        """Runs genetic algorithm and returns best solution
+
+        Sets:
+            solution (np.array): Array of 0/1 splits
+            fitness (float): Fitness value
+        """
+
+        if self.num_genes > 1:
+            self.ga.run()
+            self.solution, self.fitness, _ = self.ga.best_solution()
+        else:
+            logger.warning('Population size of < 2, skipping')
+            self.solution = None
+            self.fitness = None
+
+
+class GAParams:
+    """Manages PyGAD GA module parameters and any parameter updates
+
+    Attributes:
+        _default_ga_params (dict): Default parameters for genetic algorithm
+        params (dict): PyGAD GA module parameters to be implemented
+
+    """
+
+    def __init__(self, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            **kwargs: Genetic algorithm parameters
+        """
+        global fitness_func_absplit
+
+        # Default parameters
+        self._default_ga_params = dict(
+            # -- General Genetic Algorithm params --
+            num_generations=200,
+            sol_per_pop=100,
+            num_parents_mating=5,
+            mutation_type='scramble',
+            mutation_probability=0.1,
+            fitness_func=fitness_func_absplit,
+            keep_elitism=1,
+
+            # -- Binary Genetic Algorithm specific parameters --
+            init_range_low=0,
+            init_range_high=2,
+            random_mutation_min_val=0,
+            random_mutation_max_val=2,
+            gene_type=int,
+        )
+
+        self._dont_touch = [
+            'init_range_low',
+            'init_range_high',
+            'random_mutation_min_val',
+            'random_mutation_max_val',
+            'gene_type'
+        ]
+
+        # Copy default, update
+        self.params = dict(self._default_ga_params)
+        self._update_params(**kwargs)
+
+    def _update_params(self, **kwargs):
+        """Update GA params if any passed
+
+        Returns:
+            None
+        """
+
+        # Update if args passed
+        if kwargs:
+            for key, value in kwargs.items():
+                if key in self._dont_touch:
+                    print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a'\
+                          f'binary genetic algorith, and so you\'re not allowed to modify this')
+                    continue
+                print(f'[Updating] {key} to {value}')
+                self.params[key] = value
+
+
+class SplitBase(ParamMixin):
+    """Base class for genetic algorithm orchestration.
+
+    Manages applying different weights to costs, using multiple runs, extracting and visualising results.
+
+    Attributes:
+        _runs (int): Number of runs of the genetic algorithm to try
+        _ga_params (object): GAParams object
+        _best_score (float): Stores best score when using multiple runs
+        _metric_weights (dict): Dictionary of {col_name: value} format for applying differing weights to columns
+        _df (pd.DataFrame): Input data
+        _population (object): Data object
+        _df_result (pd.DataFrame): Proposed solution dataframe
+        _ga (object): GAInstance object
+        _df_vis (pd.DataFrame): DataFrame with solutions used for visualisation
+        _best_ga (object): GAInstance object of the best solution
+        _solution (np.array): Best solution from search
+
+    Properties:
+        results (pd.DataFrame): Accessor for _df_result
+
+    Methods:
+        _cost_weighting(): Modifies cost weighting array
+        run(): Runs the genetic algorithm
+        fitness(): Plot generation fitness graph
+        visualise(): Plots metrics using results from genetic algorithm output
+    """
+
+    def __init__(self, ga_params={}, metric_weights={}, runs=1, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            ga_params (dict, optional): Genetic algorithm parameters to add/modify
+            metric_weights (dict, optional): Cost weightings to apply to metrics
+            runs (int, optional): How many runs to try
+            **kwargs: Additional keyword arguments
+        """
+        super().__init__(**kwargs)
+        if ga_params:
+            assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
+        self._runs = runs
+        self._ga_params = GAParams(**ga_params)
+        self._best_score = -1
+        self._metric_weights = metric_weights
+        self._df = None
+        self._population = None
+        self._df_result = None  # Final results dataframe
+        self._ga = None  # genetic algorithm instance
+        self._df_vis = None  # Visualisation dataframe
+        self._best_ga = None
+        self._solution = None
+
+        self._cost_weighting()
+
+    def _cost_weighting(self):
+        """Set relative cost weights for each metric. Defaults to 1 unless specified.
+
+        Used if you want the genetic algorithm to penalise the MSE cost of some metrics
+        over others. Particularly useful if one metric is quite volatile, as the MSE cost can
+        end up with it prioritising this over others.
+
+        Returns:
+            None
+        """
+        global metric_weights_global
+        metric_weights_global = np.ones(len(self.metrics))
+        if self._metric_weights:
+            for key, value in self._metric_weights.items():
+                try:
+                    i = self.metrics.index(key)
+                    metric_weights_global[i] = value
+                    print(f'[Updating] {key} weight updated to {value}')
+                except ValueError:
+                    print(f'Cant find metric name {key}, weight {value} not applied, defaulting to 1')
+
+    def run(self):
+        """Runs genetic algorithm and returns bin splits into _df_result
+
+        Returns:
+            None
+        """
+
+        global all_metrics_global
+        logger.debug('Splitting..')
+        all_metrics_global = self._population.matrix
+
+        # Run multiple times, save the best solution
+        for i in range(self._runs):
+            if self._runs > 1:
+                print(f'[Run {i+1}]')
+
+            # Initialise and run GA, get solution
+            self._ga = GAInstance(
+                num_genes=self._population.pop_size,
+                ga_params=self._ga_params,
+            )
+            self._ga.run()
+
+            if self._ga.fitness > self._best_score:
+                print(f'Best fitness: {self._ga.fitness:.4}')
+                self._solution = self._ga.solution
+                self._best_ga = self._ga
+                self._best_score = self._ga.fitness
+
+        if self._solution is None:
+            raise ValueError('Solution is None')
+
+        # Assign solution to index
+        self._df_result = self._population.assign(self._solution)
+
+        logger.debug('Split complete')
+
+    def fitness(self, title=None):
+        """Plots the fitness-generation graph
+
+        Returns:
+            None
+        """
+
+        if self._best_ga:
+            self._best_ga.ga.plot_fitness(title=title)
+        else:
+            print('No solution available, please use .run() first')
+
+    @property
+    def results(self):
+        """Returns compiled dataframe of solutions
+
+        Returns:
+            pd.DataFrame
+        """
+
+        return self._df_result
+
+    def visualise(self, column=None):
+        """Visualise metrics for both bins and there comparative performances
+
+        Returns:
+            None
+        """
+
+        # Default to all metric columns if no columns specified
+        if column:
+            if isinstance(column, str):
+                column = [column]
+            vis_metrics = column
+        else:
+            vis_metrics = self.metrics
+
+        if self.results is None:
+            print('Must use .run() before visualising')
+            return
+
+        # Aggregate by bin
+        group_cols = ['bin']
+        group_cols += [self.date_col] if self.date_col else []
+        df = self._df_vis.groupby(group_cols)[vis_metrics].sum().reset_index()
+
+        if not len(df):
+            logger.warning(f'Failed vis')
+            return
+
+        sns.set_style('darkgrid')
+
+        # Chart sizing
+        figsize = (min(20, len(vis_metrics)*8), 5) if self.date_col else (8, 5)
+        fig, ax = plt.subplots(1, len(vis_metrics), figsize=figsize)
+        if not hasattr(ax, '__iter__'):
+            ax = [ax]
+
+        # Plot each metric
+        for i, metric in enumerate(vis_metrics):
+
+            # If over time, plot line graph, else bar
+            if self.date_col:
+                sns.lineplot(data=df, x=self.date_col, y=metric, hue='bin', ax=ax[i])
+            else:
+                df['metric'] = metric
+                sns.barplot(data=df, x='metric', y=metric, hue='bin', ax=ax[i])
+
+            ax[i].set_title(f'{metric.title()}')
+            ax[i].tick_params(axis='x', labelrotation=45)
+
+        plt.show()
+
+
+class ABSplit(SplitBase):
+    """Splits data into A/B groups based on specified parameters. All members of the population will be in one bin or
+    the other.
+
+    Attributes:
+        _runs (int): Number of runs of the genetic algorithm to try
+        _ga_params (object): GAParams object
+        _best_score (float): Stores best score when using multiple runs
+        _metric_weights (dict): Dictionary of {col_name: value} format for applying differing weights to columns
+        _df (pd.DataFrame): Input data
+        _population (object): Data object
+        _df_result (pd.DataFrame): Proposed solution dataframe
+        _ga (object): GAInstance object
+        _df_vis (pd.DataFrame): DataFrame with solutions used for visualisation
+        _best_ga (object): GAInstance object of best solution
+        _solution (np.array): Best solution from search
+
+    Properties:
+        results (pd.DataFrame): Accessor for _df_result
+
+    Methods:
+        _cost_weighting(): Modifies cost weighting array
+        run(): Runs the genetic algorithm
+        fitness(): Plot generation fitness graph
+        visualise(): Plots metrics using results from genetic algorithm output
+    """
+
+    def __init__(self, df, ga_params={}, metric_weights={}, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            df (pd.DataFrame): Dataframe to be split
+            ga_params (dict): Parameters for the genetic algorithm (default: {})
+            metric_weights (dict): Weights for each metric in the data (default: {})
+            **kwargs: Additional keyword arguments
+        """
+        super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
+        self.df = df
+        self._population = Data(self.df.copy(), **kwargs)
+
+    def visualise(self, column=None):
+        """Visualizes the A/B split results.
+
+        Returns:
+            None
+        """
+
+        # Merge solution results (_df_results) onto input data (metrics) so that data can be visualised
+        self._df_vis = self._population.stacked.merge(
+            self._df_result,
+            left_index=True,
+            right_index=True
+        )
+        super().visualise(column=column)
+
+    def __repr__(self):
+        lst_str = [f"'{col}', " for col in self.all_spec_columns]
+        return f'ABSplit([{lst_str}])'
+
+
+class MatchDataProc:
+    """Ensures consistent number of dates between sample and population data
+
+    Achieves this by concatenating both dataframes, unstacking by date, then filtering
+    by the index of the sample and population data and restacking.
+
+    Without this, if there are date mismatches between sample and population (e.g.
+    100 distinct date in sample, and 110 in population) then the 2 matrices will be
+    different sizes.
+
+    Defaults missing date values to 0
+
+    Attributes:
+        df_pop (pd.DataFrame): Dataframe of population data
+        df_samp (pd.DataFrame): Dataframe of sample data
+        df_all (pd.DataFrame): Concatenation of df_pop and df_samp
+        all (Data): Instance of the Data class for all data
+        pop (Data): Instance of the Data class for population data
+        samp (Data): Instance of the Data class for sample data
+
+    Properties:
+        sample (pd.DataFrame): Sample data
+        population (pd.DataFrame): Population data
+    """
+
+    def __init__(self, df_pop, df_samp, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            df_pop (pd.DataFrame): Dataframe of population data
+            df_samp (pd.DataFrame): Dataframe of sample data
+            **kwargs: Additional keyword arguments
+        """
+        self.df_pop = df_pop
+        self.df_samp = df_samp
+        self.df_all = pd.concat([df_pop, df_samp], axis=0)
+        self.all = Data(self.df_all, scale=False, **kwargs)
+        self.pop = Data(self.df_pop, scale=False, **kwargs)
+        self.samp = Data(self.df_samp, scale=False, **kwargs)
+
+    @property
+    def sample(self):
+        """Returns the filtered dataframe of sample data
+
+        Returns:
+            pd.DataFrame: Filtered dataframe of sample data
+        """
+        return self.all.filter(self.samp.index)
+
+    @property
+    def population(self):
+        """Returns the filtered dataframe of population data
+
+        Returns:
+            pd.DataFrame: Filtered dataframe of population data
+        """
+        return self.all.filter(self.pop.index)
+
+
+class Match(SplitBase):
+    """Manages a genetic algorithm to find a group in a population with similar properties
+    as a specified sample group. Sample group must be removed from population prior to running
+    Match.
+
+    Attributes:
+        _df_pop (pd.DataFrame): Dataframe of population data
+        _df_samp (pd.DataFrame): Dataframe of sample data
+        _population (Data): Instance of the Data class for population data
+        _sample (Data): Instance of the Data class for sample data
+        _df_result (pd.DataFrame): Dataframe of population data that matches the sample group
+        _df_vis (pd.DataFrame): Dataframe of population data, sample data and matched population data for visualization
+
+    Methods:
+        _broadcast_match(): Makes the match matrix available globally
+        run(): Runs the genetic algorithm
+        fitness(): Plot generation fitness graph
+        visualise(): Plots metrics using results from genetic algorithm output
+    """
+
+    def __init__(self, population, sample, ga_params={}, metric_weights={}, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            population (pd.DataFrame): Dataframe of population data
+            sample (pd.DataFrame): Dataframe of sample data
+            ga_params (dict): Parameters for the genetic algorithm
+            metric_weights (dict): Weights for the metrics being compared
+            **kwargs: Additional keyword arguments
+        """
+
+        # Specify fitness function
+        global fitness_func_match
+        ga_params['fitness_func'] = fitness_func_match
+        ga_params['mutation_type'] = 'scramble'
+        super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
+
+        self._df_pop = population
+        self._df_samp = sample
+
+        # Ensure consistent dates between sample and population
+        if self.date_col:
+            mdp = MatchDataProc(df_pop=self._df_pop, df_samp=self._df_samp, **kwargs)
+            self._df_pop = mdp.population.reset_index()
+            self._df_samp = mdp.sample.reset_index()
+
+        # Fit scaler on combined data
+        scaler = preprocessing.MinMaxScaler()
+        scaler.fit(pd.concat([self._df_pop, self._df_samp], axis=0)[self.metrics])
+
+        self._population = Data(self._df_pop, scaler=scaler, **kwargs)
+        self._sample = Data(self._df_samp, scaler=scaler, **kwargs)
+        self._broadcast_match()
+
+    def _broadcast_match(self):
+        """Makes the match matrix available globally
+
+        Returns:
+            None
+        """
+        global match_metrics_global
+        match_metrics_global = self._sample.matrix
+
+    def run(self):
+        """Runs the genetic algorithm, filters out all except sample and result
+
+        Returns:
+            None
+        """
+        # Run genetic algorithm
+        super().run()
+
+        # Filter on only bin == 1
+        self._df_result = self._df_result[self._df_result['bin'] == 1]
+
+        # Get sample index, set as bin 0, concat to _df_results (which are all bin 1)
+        index_cols = self._sample.index.index.names
+        df_match = self._df_samp[index_cols].drop_duplicates().set_index(index_cols)
+        df_match['bin'] = 0
+        self._df_result = pd.concat([self._df_result, df_match], axis=0).sort_index()
+
+    def visualise(self, column=None):
+        """Visualizes sample and results side by side
+
+        Returns:
+            None
+        """
+
+        # Concat to form entire population
+        self._df_vis = pd.concat([self._population.stacked, self._sample.stacked], axis=0)
+
+        # Inner join to filter out all but sample and match
+        self._df_vis = self._df_vis.merge(
+            self._df_result,
+            left_index=True,
+            right_index=True,
+            how='inner'
+        )
+
+        super().visualise(column=column)
+
+    def __repr__(self):
+        lst_str = [f"'{col}', " for col in self.all_spec_columns]
+        return f'Match([{lst_str}])'
+
+
+def fitness_func_absplit(ga_instance, solution, solution_idx):
+    """Fitness function for ABSplit
+    """
+    global all_metrics_global
+    global metric_weights_global
+
+    cost1 = solution @ all_metrics_global
+    cost2 = (1 - solution) @ all_metrics_global
+    # Average over time axis, sum over metric axis
+    mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
+
+    # Fitness
+    fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
+    return fitness
+
+
+def fitness_func_match(ga_instance, solution, solution_idx):
+    """Fitness function for Match
+    """
+    global all_metrics_global
+    global match_metrics_global
+    global metric_weights_global
+
+    cost1 = match_metrics_global.sum(1)  # Sum along population axis
+    cost2 = solution @ all_metrics_global
+    # Average over time axis, sum over metric axis
+    mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
+
+    # Fitness
+    fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
+    return fitness
```

### Comparing `absplit-0.1.4/absplit/param.py` & `absplit-0.1.5/absplit/param.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from abc import ABC
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-class ParamMixin(ABC):
-    """Mixin class to store and process column names
-
-    Attributes:
-        metrics (list): Metric column names
-        date_col (str): Date column name, if applicable
-        splitting (str): Column to split on
-        all_spec_columns (list): All column names specified by user
-        dim_spec_columns (list): All dimension columns (non-metrics) specified by user
-
-    Methods:
-        get_columns(): Get all columns specified by user in specific order
-    """
-
-    def __init__(self, metrics, splitting, date_col=None, **kwargs):
-        """Initializes the class and sets the attributes
-
-        Args:
-            metrics (list): Metric column names
-            splitting (str): Column to split on
-            date_col (str): Date column name, if applicable
-            **kwargs: Additional keyword arguments
-        """
-        self.metrics = metrics if isinstance(metrics, list) else [metrics]
-        self.date_col = date_col
-        self.splitting = splitting
-        self.all_spec_columns = self.get_columns()
-        self.dim_spec_columns = [x for x in self.all_spec_columns if x not in self.metrics]
-
-    def get_columns(self):
-        """Gets list of all column names specified by user, in order of:
-            * splitting
-            * date_col
-            * metrics
-
-        Returns:
-            list
-        """
-
-        col_type_lst = [
-            self.splitting,
-            self.date_col,
-            self.metrics
-        ]
-        all_columns = []
-        for col in col_type_lst:
-            if col is not None:
-                if isinstance(col, list):
-                    all_columns += col
-                else:
-                    all_columns.append(col)
-        return all_columns
+from abc import ABC
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+class ParamMixin(ABC):
+    """Mixin class to store and process column names
+
+    Attributes:
+        metrics (list): Metric column names
+        date_col (str): Date column name, if applicable
+        splitting (str): Column to split on
+        all_spec_columns (list): All column names specified by user
+        dim_spec_columns (list): All dimension columns (non-metrics) specified by user
+
+    Methods:
+        get_columns(): Get all columns specified by user in specific order
+    """
+
+    def __init__(self, metrics, splitting, date_col=None, **kwargs):
+        """Initializes the class and sets the attributes
+
+        Args:
+            metrics (list): Metric column names
+            splitting (str): Column to split on
+            date_col (str): Date column name, if applicable
+            **kwargs: Additional keyword arguments
+        """
+        self.metrics = metrics if isinstance(metrics, list) else [metrics]
+        self.date_col = date_col
+        self.splitting = splitting
+        self.all_spec_columns = self.get_columns()
+        self.dim_spec_columns = [x for x in self.all_spec_columns if x not in self.metrics]
+
+    def get_columns(self):
+        """Gets list of all column names specified by user, in order of:
+            * splitting
+            * date_col
+            * metrics
+
+        Returns:
+            list
+        """
+
+        col_type_lst = [
+            self.splitting,
+            self.date_col,
+            self.metrics
+        ]
+        all_columns = []
+        for col in col_type_lst:
+            if col is not None:
+                if isinstance(col, list):
+                    all_columns += col
+                else:
+                    all_columns.append(col)
+        return all_columns
```

### Comparing `absplit-0.1.4/images/logo.jpeg` & `absplit-0.1.5/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-0.1.4/tests/test_ga.py` & `absplit-0.1.5/tests/test_ga.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from absplit import ABSplit, Match
-import pandas as pd
-import datetime as dt
-import numpy as np
-
-# Build test data
-data_dct = {
-    'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)]*5,
-    'country': ['UK'] * 15,
-    'region': [item for sublist in [[x]*6 for x in ['z', 'y']] for item in sublist] + ['x']*3,
-    'city': [item for sublist in [[x]*3 for x in ['a', 'b', 'c', 'd', 'e']] for item in sublist],
-    'metric1': np.arange(0, 15, 1),
-    'metric2': np.arange(0, 150, 10)
-}
-df = pd.DataFrame(data_dct)
-
-# Column kwargs
-kwargs = {
-    'metrics': ['metric1', 'metric2'],
-    'date_col': 'date',
-    'split_by': 'region',
-    'splitting': 'city'
-}
-
-# Initialise and run
-ab = ABSplit(
-    df=df,
-    **kwargs,
-)
-ab.run()
-
-# Results
-data_dct1 = {
-    'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
-    'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
-    'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
-    'bin': {0: 1, 1: 0, 2: 0, 3: 1, 4: 1}
-}
-data_dct2 = {
-    'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
-    'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
-    'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
-    'bin': {0: 0, 1: 1, 2: 1, 3: 0, 4: 0}
-}
-df_data1 = pd.DataFrame(data_dct1)
-df_data2 = pd.DataFrame(data_dct2)
-
-
-def test_ab_results():
-    """GA output ab.results"""
-    r1 = len(ab.results.reset_index().compare(df_data1)) == 0
-    r2 = len(ab.results.reset_index().compare(df_data2)) == 0
-    assert True in (r1, r2)
-
-
-# Generate sample dataframe
-data_dct = {
-    'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)],
-    'country': ['UK'] * 3,
-    'region': ['w'] * 3,
-    'city': ['f'] * 3,
-    'metric1': [3, 6, 7],
-    'metric2': [30, 45, 70]
-}
-df_sample = pd.DataFrame(data_dct)
-
-# Initialise match and run
-m = Match(
-    population=df,
-    sample=df_sample,
-    **kwargs
-)
-m.run()
-
-
-def test_match_results():
-    dct = {'bin': {('UK', 'w', 'f'): 0, ('UK', 'z', 'a'): 1, ('UK', 'z', 'b'): 1}}
-    assert m.results.to_dict() == dct
+from absplit import ABSplit, Match
+import pandas as pd
+import datetime as dt
+import numpy as np
+
+# Build test data
+data_dct = {
+    'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)]*5,
+    'country': ['UK'] * 15,
+    'region': [item for sublist in [[x]*6 for x in ['z', 'y']] for item in sublist] + ['x']*3,
+    'city': [item for sublist in [[x]*3 for x in ['a', 'b', 'c', 'd', 'e']] for item in sublist],
+    'metric1': np.arange(0, 15, 1),
+    'metric2': np.arange(0, 150, 10)
+}
+df = pd.DataFrame(data_dct)
+
+# Column kwargs
+kwargs = {
+    'metrics': ['metric1', 'metric2'],
+    'date_col': 'date',
+    'split_by': 'region',
+    'splitting': 'city'
+}
+
+# Initialise and run
+ab = ABSplit(
+    df=df,
+    **kwargs,
+)
+ab.run()
+
+# Results
+data_dct1 = {
+    'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
+    'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
+    'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
+    'bin': {0: 1, 1: 0, 2: 0, 3: 1, 4: 1}
+}
+data_dct2 = {
+    'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
+    'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
+    'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
+    'bin': {0: 0, 1: 1, 2: 1, 3: 0, 4: 0}
+}
+df_data1 = pd.DataFrame(data_dct1)
+df_data2 = pd.DataFrame(data_dct2)
+
+
+def test_ab_results():
+    """GA output ab.results"""
+    r1 = len(ab.results.reset_index().compare(df_data1)) == 0
+    r2 = len(ab.results.reset_index().compare(df_data2)) == 0
+    assert True in (r1, r2)
+
+
+# Generate sample dataframe
+data_dct = {
+    'date': [dt.date(2030,4,1) + dt.timedelta(days=x) for x in range(3)],
+    'country': ['UK'] * 3,
+    'region': ['w'] * 3,
+    'city': ['f'] * 3,
+    'metric1': [3, 6, 7],
+    'metric2': [30, 45, 70]
+}
+df_sample = pd.DataFrame(data_dct)
+
+# Initialise match and run
+m = Match(
+    population=df,
+    sample=df_sample,
+    **kwargs
+)
+m.run()
+
+
+def test_match_results():
+    dct = {'bin': {('UK', 'w', 'f'): 0, ('UK', 'z', 'a'): 1, ('UK', 'z', 'b'): 1}}
+    assert m.results.to_dict() == dct
```

