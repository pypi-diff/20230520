# Comparing `tmp/new-component-0.4.2.tar.gz` & `tmp/new-component-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.4.2.tar", last modified: Fri May 19 21:35:18 2023, max compression
+gzip compressed data, was "new-component-0.4.3.tar", last modified: Fri May 19 23:23:35 2023, max compression
```

## Comparing `new-component-0.4.2.tar` & `new-component-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-19 21:34:56.459287 new-component-0.4.2/LICENSE
--rw-r--r--   0        0        0     4798 2023-05-19 21:34:56.459287 new-component-0.4.2/README.md
--rw-r--r--   0        0        0     1660 2023-05-19 21:34:56.463287 new-component-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6187 2023-05-19 21:34:56.463287 new-component-0.4.2/tests/test_new_component.py
--rw-r--r--   0        0        0      491 2023-05-19 21:34:56.463287 new-component-0.4.2/tests/test_version.py
--rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 new-component-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 23:23:09.543231 new-component-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4798 2023-05-19 23:23:09.543231 new-component-0.4.3/README.md
+-rw-r--r--   0        0        0     2085 2023-05-19 23:23:09.543231 new-component-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/__init__.py
+-rw-r--r--   0        0        0      496 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/__version__.py
+-rw-r--r--   0        0        0     1961 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_config.py
+-rw-r--r--   0        0        0      708 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_confirms.py
+-rw-r--r--   0        0        0      566 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_constants.py
+-rw-r--r--   0        0        0     2088 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_echos.py
+-rw-r--r--   0        0        0      360 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_jinja.py
+-rw-r--r--   0        0        0      249 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_utils.py
+-rw-r--r--   0        0        0      206 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_version.py
+-rw-r--r--   0        0        0     4121 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/cli.py
+-rw-r--r--   0        0        0      142 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/py.typed
+-rw-r--r--   0        0        0      269 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/templates/component.js.j2
+-rw-r--r--   0        0        0       48 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/templates/index.js.j2
+-rw-r--r--   0        0        0        0 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     6177 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/test_new_component.py
+-rw-r--r--   0        0        0      285 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/test_version.py
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 new-component-0.4.3/PKG-INFO
```

### Comparing `new-component-0.4.2/LICENSE` & `new-component-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.4.2/README.md` & `new-component-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `new-component-0.4.2/pyproject.toml` & `new-component-0.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 [project]
-name = "new-component"
-version = "0.4.2"
+name = "new_component"
+version = "0.4.3"
 description = "Quickly create opinionated Styled Components for React Projects"
 authors = [
     { name = "Ian Cleary", email = "github@iancleary.me" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "typer==0.9.0",
     "colorama==0.4.6",
     "shellingham==1.5.0.post1",
     "rich==13.3.5",
     "Jinja2==3.1.2",
 ]
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+Homepage = "https://new-component.iancleary.me"
+Repository = "https://github.com/iancleary/new-component"
+Documentation = "https://new-component.iancleary.me"
+
 [project.scripts]
-new-component = "new_component.__main__:main"
+new-component = "new_component.main:main"
+
+[tool.pdm.version]
+source = "scm"
+write_to = "new_component/VERSION"
+write_template = "__version__ = '{}'"
+
+[tool.pdm.build]
+package-dir = "src"
+includes = [
+    "src/new_component",
+]
+source-includes = [
+    "tests",
+    "LICENSE",
+    "README.md",
+]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest==7.2.0",
     "black==22.10.0",
     "mypy==0.990",
     "ruff==0.0.225",
```

### Comparing `new-component-0.4.2/tests/test_new_component.py` & `new-component-0.4.3/tests/test_new_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,38 @@
     os.remove(GLOBAL_CONFIG_FILE)
 
 # create typer runner for testing
 runner = CliRunner()
 
 
 def test_version() -> None:
-
     result = runner.invoke(cli.app, ["--version"])
     assert result.exit_code == 0
     assert f"{__app_name__} v{__version__}\n" in result.stdout
 
 
 def test_prompt_to_create_components_directory() -> None:
-
     result = runner.invoke(
         cli.app, ["Button"], input="y\n"
     )  # y to create components directory
     assert result.exit_code == 0
     assert (
         "./src/components/ doesn't exist. Do you want to create it? [y/N]:"
         in result.stdout
     )
 
 
 def test_creating_component() -> None:
-
     result = runner.invoke(cli.app, ["AwesomeComponent"])
     assert result.exit_code == 0
     assert "AwesomeComponent" in result.stdout
     assert "✨ Creating a new AwesomeComponent Component ✨!" in result.stdout
 
 
 def test_creating_component_with_directory_first_time() -> None:
-
     # ensure ./component directory is empty
     SPECIFIED_COMPONENTS_DIR_PATH = Path("./components")
     if SPECIFIED_COMPONENTS_DIR_PATH.exists():
         shutil.rmtree(path=SPECIFIED_COMPONENTS_DIR_PATH)
 
     result = runner.invoke(
         cli.app, ["DirectoryComponent", "--directory", "components"], input="y\n"
@@ -71,47 +67,43 @@
         "./components/ doesn't exist. Do you want to create it? [y/N]:" in result.stdout
     )
     assert "DirectoryComponent" in result.stdout
     assert "✨ Creating a new DirectoryComponent Component ✨!" in result.stdout
 
 
 def test_creating_component_with_directory_that_exists() -> None:
-
     result = runner.invoke(
         cli.app, ["DirectoryComponent2", "--directory", "components"]
     )
     assert result.exit_code == 0
     assert "DirectoryComponent2" in result.stdout
     assert "✨ Creating a new DirectoryComponent2 Component ✨!" in result.stdout
 
 
 def test_creating_component_files() -> None:
-
     result = runner.invoke(cli.app, ["File"])
     assert result.exit_code == 0
     assert "File" in result.stdout
     assert "✨ Creating a new File Component ✨!" in result.stdout
     assert (
         Path(f"./src/components/File/index.{DEFAULT_FILE_EXTENSION}").exists() is True
     )
     assert Path(f"./src/components/File/File.{DEFAULT_FILE_EXTENSION}").exists() is True
 
 
 def test_creating_component_with_extension() -> None:
-
     result = runner.invoke(cli.app, ["Extension", "--extension", "jsx"])
     assert result.exit_code == 0
     assert "Extension" in result.stdout
     assert "✨ Creating a new Extension Component ✨!" in result.stdout
     assert Path("./src/components/Extension/index.jsx").exists() is True
     assert Path("./src/components/Extension/Extension.jsx").exists() is True
 
 
 def test_local_config_file() -> None:
-
     if LOCAL_CONFIG_FILE.exists():
         os.remove(LOCAL_CONFIG_FILE)
 
     if GLOBAL_CONFIG_FILE.exists():
         os.remove(GLOBAL_CONFIG_FILE)
 
     # Data to be written to LOCAL_CONFIG_FILE
@@ -126,15 +118,14 @@
     assert "LocalConfig" in result.stdout
     assert "✨ Creating a new LocalConfig Component ✨!" in result.stdout
     assert Path("./components/LocalConfig/index.jsx").exists() is True
     assert Path("./components/LocalConfig/LocalConfig.jsx").exists() is True
 
 
 def test_global_config_file() -> None:
-
     if LOCAL_CONFIG_FILE.exists():
         os.remove(LOCAL_CONFIG_FILE)
 
     if GLOBAL_CONFIG_FILE.exists():
         os.remove(GLOBAL_CONFIG_FILE)
 
     if GLOBAL_CONFIG_PATH.exists() is False:
@@ -154,15 +145,14 @@
     assert Path("./src/global/components/GlobalConfig/index.jsx").exists() is True
     assert (
         Path("./src/global/components/GlobalConfig/GlobalConfig.jsx").exists() is True
     )
 
 
 def test_local_and_global_config_file() -> None:
-
     if LOCAL_CONFIG_FILE.exists():
         os.remove(LOCAL_CONFIG_FILE)
 
     if GLOBAL_CONFIG_FILE.exists():
         os.remove(GLOBAL_CONFIG_FILE)
 
     if GLOBAL_CONFIG_PATH.exists() is False:
```

### Comparing `new-component-0.4.2/PKG-INFO` & `new-component-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: new-component
-Version: 0.4.2
+Name: new_component
+Version: 0.4.3
 Summary: Quickly create opinionated Styled Components for React Projects
 License: MIT
 Author-email: Ian Cleary <github@iancleary.me>
-Requires-Python: >=3.8
+Requires-Python: >=3.11
+Project-URL: Documentation, https://new-component.iancleary.me
+Project-URL: Homepage, https://new-component.iancleary.me
+Project-URL: Repository, https://github.com/iancleary/new-component
 Description-Content-Type: text/markdown
 
 # new-component
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
```

