# Comparing `tmp/mac_cleanup-3.0.1.tar.gz` & `tmp/mac_cleanup-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mac_cleanup-3.0.1.tar", max compression
+gzip compressed data, was "mac_cleanup-3.0.2.tar", max compression
```

## Comparing `mac_cleanup-3.0.1.tar` & `mac_cleanup-3.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-08-09 13:15:49.497915 mac_cleanup-3.0.1/LICENSE
--rw-r--r--   0        0        0     3795 2023-04-25 11:33:45.460404 mac_cleanup-3.0.1/README.md
--rw-r--r--   0        0        0      425 2023-04-14 12:16:23.955827 mac_cleanup-3.0.1/mac_cleanup/__init__.py
--rw-r--r--   0        0        0      181 2023-03-26 22:15:29.161722 mac_cleanup-3.0.1/mac_cleanup/__version__.py
--rw-r--r--   0        0        0     8333 2023-04-14 12:16:23.956897 mac_cleanup-3.0.1/mac_cleanup/config.py
--rw-r--r--   0        0        0      653 2023-04-14 12:16:23.957364 mac_cleanup-3.0.1/mac_cleanup/console.py
--rw-r--r--   0        0        0     7743 2023-04-25 11:33:45.272323 mac_cleanup-3.0.1/mac_cleanup/core.py
--rw-r--r--   0        0        0     4257 2023-04-14 12:16:23.958176 mac_cleanup-3.0.1/mac_cleanup/core_modules.py
--rw-r--r--   0        0        0    14351 2023-04-14 12:16:23.958627 mac_cleanup-3.0.1/mac_cleanup/default_modules.py
--rw-r--r--   0        0        0     3791 2023-04-14 12:16:23.958905 mac_cleanup-3.0.1/mac_cleanup/error_handling.py
--rw-r--r--   0        0        0     2918 2023-04-14 12:16:23.959175 mac_cleanup-3.0.1/mac_cleanup/main.py
--rw-r--r--   0        0        0     1181 2023-04-14 12:16:23.959495 mac_cleanup-3.0.1/mac_cleanup/parser.py
--rw-r--r--   0        0        0     3380 2023-04-14 12:16:23.960159 mac_cleanup-3.0.1/mac_cleanup/progress.py
--rwxr-xr-x   0        0        0     3181 2023-04-14 12:16:23.960392 mac_cleanup-3.0.1/mac_cleanup/utils.py
--rw-r--r--   0        0        0     2959 2023-04-25 11:33:45.461381 mac_cleanup-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 22:17:44.340035 mac_cleanup-3.0.2/LICENSE
+-rw-r--r--   0        0        0     3795 2023-05-20 16:36:29.591790 mac_cleanup-3.0.2/README.md
+-rw-r--r--   0        0        0      425 2023-05-11 22:17:44.340449 mac_cleanup-3.0.2/mac_cleanup/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-11 22:17:44.340660 mac_cleanup-3.0.2/mac_cleanup/__version__.py
+-rw-r--r--   0        0        0     8289 2023-05-20 16:28:42.279287 mac_cleanup-3.0.2/mac_cleanup/config.py
+-rw-r--r--   0        0        0      652 2023-05-20 16:28:42.280426 mac_cleanup-3.0.2/mac_cleanup/console.py
+-rw-r--r--   0        0        0     7720 2023-05-20 16:28:42.286177 mac_cleanup-3.0.2/mac_cleanup/core.py
+-rw-r--r--   0        0        0     4185 2023-05-20 16:29:57.350961 mac_cleanup-3.0.2/mac_cleanup/core_modules.py
+-rw-r--r--   0        0        0    14634 2023-05-20 16:06:49.038722 mac_cleanup-3.0.2/mac_cleanup/default_modules.py
+-rw-r--r--   0        0        0     3790 2023-05-20 16:28:42.307709 mac_cleanup-3.0.2/mac_cleanup/error_handling.py
+-rw-r--r--   0        0        0     2918 2023-05-11 22:17:44.341805 mac_cleanup-3.0.2/mac_cleanup/main.py
+-rw-r--r--   0        0        0     1181 2023-05-11 22:17:44.341922 mac_cleanup-3.0.2/mac_cleanup/parser.py
+-rw-r--r--   0        0        0     3378 2023-05-20 16:28:42.315352 mac_cleanup-3.0.2/mac_cleanup/progress.py
+-rwxr-xr-x   0        0        0     3176 2023-05-20 16:28:42.318896 mac_cleanup-3.0.2/mac_cleanup/utils.py
+-rw-r--r--   0        0        0     2946 2023-05-20 16:36:29.591839 mac_cleanup-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.2/PKG-INFO
```

### Comparing `mac_cleanup-3.0.1/LICENSE` & `mac_cleanup-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.1/README.md` & `mac_cleanup-3.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.1
+    3.0.2
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/config.py` & `mac_cleanup-3.0.2/mac_cleanup/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 @final
 class Config:
     """
     Class for config initialization and validation.
 
     :param config_path_: Path to config location
-
     """
 
     def __init__(self, config_path_: Path):
         # Set config path
         self.__path: Final = config_path_
 
         # Set modules in the class
@@ -94,18 +93,15 @@
             self.__config_data["enabled"].remove(faulty_module)
 
         # Write updated config if faulty modules were found
         if remove_list:
             self.__write()
 
     def __read(self) -> ConfigFile:
-        """
-        Gets the config or creates it if it doesn't exist
-            :return: Config as a dict
-        """
+        """Gets the config or creates it if it doesn't exist :return: Config as a dict."""
 
         from toml import TomlDecodeError, load
 
         # Creates config if it's not already created
         self.__path.parent.mkdir(exist_ok=True, parents=True)
         self.__path.touch(exist_ok=True)
 
@@ -127,15 +123,14 @@
 
     @staticmethod
     def full_exit(failed: bool) -> None:
         """
         Gracefully exits from cleaner.
 
         :param failed: Status code of exit
-
         """
 
         console.print("Config saved, exiting...")
         exit(failed)
 
     def set_custom_path(self) -> None:
         """Sets path for custom modules in config."""
@@ -163,15 +158,14 @@
     def __configure(self, *, all_modules: list[str], enabled_modules: list[str]) -> None:
         """
         Opens modules configuration screen.
 
         :param all_modules: List w/ all modules
         :param enabled_modules: List w/ all enabled modules
         :return: List w/ all modules user enabled
-
         """
 
         import inquirer  # pyright: ignore [reportMissingTypeStubs]
 
         from mac_cleanup.console import print_panel
 
         # Prints the legend
@@ -182,22 +176,22 @@
         )
 
         questions = inquirer.Checkbox(  # pyright: ignore [reportUnknownVariableType, reportUnknownMemberType]
             "modules", message="Active modules", choices=all_modules, default=enabled_modules, carousel=True
         )
 
         # Get user answers
-        answers = inquirer.prompt(  # pyright: ignore [reportUnknownVariableType, reportUnknownMemberType]
+        answers = inquirer.prompt(  # pyright: ignore [reportUnknownMemberType]
             questions=[questions], raise_keyboard_interrupt=True
         )
 
         # Clear console after checkbox
         console.clear()
 
-        if not answers["modules"]:
+        if not answers or not answers["modules"]:
             console.print("Config cannot be empty. Enable some modules")
 
             return self.__configure(all_modules=all_modules, enabled_modules=enabled_modules)
 
         # Update config
         self.__config_data["enabled"] = answers["modules"]
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/console.py` & `mac_cleanup-3.0.2/mac_cleanup/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,13 +12,12 @@
 def print_panel(text: str, title: Optional[str] = None) -> None:
     """
     Prints a rich panel with the given text.
 
     Args:
         text: Text to print in the panel
         title: Title of the panel
-
     """
     from rich.panel import Panel
     from rich.text import Text
 
     console.print(Panel(Text.from_markup(text, justify="center"), subtitle=title, subtitle_align="right"))
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/core.py` & `mac_cleanup-3.0.2/mac_cleanup/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,38 +86,36 @@
 
     @beartype
     def message(self, message_: str) -> None:
         """
         Add message to instance of :class:`Unit`
 
         :param message_: Message to be printed in progress bar
-
         """
 
         self.__temp_message = message_
 
     @beartype
     def add(self, module_: BaseModule) -> None:
         """
         Add module to the list of modules to instance of :class:`Unit`
 
-        :param module_: Module based on :class:`BaseModule`
-
+        :param module_: Module based on
+        :class: `BaseModule`
         """
 
         self.__temp_modules_list.append(module_)
 
     @staticmethod
     def _get_size(path_: Path_) -> float:
         """
         Counts size of directory.
 
         :param path_: Path to the directory
         :return: Size of specified directory
-
         """
 
         # Get path posix
         path_posix = path_.as_posix()
 
         # Set list of globs
         globs = ["*", "[", "]"]
@@ -190,18 +188,15 @@
     @staticmethod
     def __filter_modules(module_: BaseModule, filter_type: Type[T]) -> TypeGuard[T]:
         """Filter instances of specified class based on :class:`BaseModule`"""
 
         return isinstance(module_, filter_type)
 
     def _count_dry(self) -> float:
-        """
-        Counts free space for dry run
-            :return: Approx amount of bytes to be removed
-        """
+        """Counts free space for dry run :return: Approx amount of bytes to be removed."""
 
         from concurrent.futures import ThreadPoolExecutor, as_completed
 
         from mac_cleanup.progress import ProgressBar
 
         # Extract all modules
         all_modules = list(chain.from_iterable([unit.modules for unit in self._execute_list]))
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/core_modules.py` & `mac_cleanup-3.0.2/mac_cleanup/core_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,33 +19,30 @@
 
     @beartype
     def with_prompt(self: T, message_: Optional[str] = None) -> T:
         """
         Execute command with user prompt.
 
         :param message_: Message to be shown on prompt
-        :return: :class:`BaseModule`
-
+        :return: Instance of self from
+        :class: `BaseModule`
         """
 
         # Can't be solved without typing.Self
         self.__prompt = True  # pyright: ignore [reportGeneralTypeIssues]
 
         if message_:
             # Can't be solved without typing.Self
             self.__prompt_message = message_  # pyright: ignore [reportGeneralTypeIssues]
 
         return self
 
     @abstractmethod
     def _execute(self) -> bool:
-        """
-        Base exec with check for prompt
-            :return: True on successful prompt
-        """
+        """Base exec with check for prompt :return: True on successful prompt."""
 
         # Call prompt if needed
         if self.__prompt:
             # Skip on negative prompt
             return ProgressBar.prompt(prompt_text=self.__prompt_message, prompt_title="Module requires attention")
 
         return True
@@ -78,15 +75,14 @@
     @abstractmethod
     def _execute(self, **kwargs: bool) -> Optional[str]:
         """
         Execute the command specified.
 
         :param ignore_errors_: Ignore errors during execution
         :return: Command execution results based on specified parameters
-
         """
 
         # Skip if there is no command
         if not self.__command:
             return
 
         # Skip on negative prompt
@@ -100,18 +96,15 @@
 @final
 class Command(_BaseCommand):
     """Collector list unit for command execution."""
 
     __ignore_errors: bool = True
 
     def with_errors(self) -> "Command":
-        """
-        Return errors in exec output
-            :return: :class:`Command`
-        """
+        """Return errors in exec output :return: :class:`Command`"""
 
         self.__ignore_errors = False
 
         return self
 
     def _execute(self) -> Optional[str]:
         return super()._execute(ignore_errors=self.__ignore_errors)
@@ -134,27 +127,23 @@
     @property
     def get_path(self) -> Path_:
         """Get path specified to the module."""
 
         return self.__path
 
     def dry_run_only(self) -> "Path":
-        """
-        Set module to only count size in dry runs
-            :return: :class:`Path`
-        """
+        """Set module to only count size in dry runs :return: :class:`Path`"""
 
         self.__dry_run_only = True
 
         return self
 
     def _execute(self) -> Optional[str]:
-        """
-        Delete specified path
-            :return: Command execution results based on specified parameters
+        """Delete specified path :return: Command execution results based on specified
+        parameters.
         """
 
         if self.__dry_run_only:
             return
 
         # Skip if path is not deletable or undefined
         if not all([check_deletable(path=self.__path), check_exists(path=self.__path, expand_user=False)]):
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/default_modules.py` & `mac_cleanup-3.0.2/mac_cleanup/default_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,24 @@
     if cmd("type 'npm'"):
         with clc as unit:
             unit.message("Cleaning up npm cache")
             unit.add(Command("npm cache clean --force"))
             unit.add(Path("~/.npm/*").dry_run_only())
 
 
+def pnpn():
+    from mac_cleanup.utils import cmd
+
+    if cmd("type 'pnpm'"):
+        with clc as unit:
+            unit.message("Cleaning up pnpm Cache...")
+            unit.add(Command("pnpm store prune &>/dev/null"))
+            unit.add(Path("~/.pnpm-store/*").dry_run_only())
+
+
 def yarn():
     from mac_cleanup.utils import cmd
 
     if cmd("type 'yarn'"):
         with clc as unit:
             unit.message("Cleaning up Yarn Cache")
             unit.add(Command("yarn cache clean --force"))
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/error_handling.py` & `mac_cleanup-3.0.2/mac_cleanup/error_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     """
     Decorator for catching exceptions and printing logs.
 
     :param func: Function to be decorated
     :param exception: Expected exception(s)
     :param exit_on_exception: If True, exit after unexpected exception was handled
     :return: Decorated function
-
     """
 
     err_handler_instance: ErrorHandler = ErrorHandler(exception=exception, exit_on_exception=exit_on_exception)
 
     if func:
         err_handler_call: Callable[..., Optional[T]] = err_handler_instance(func)
         return err_handler_call
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/main.py` & `mac_cleanup-3.0.2/mac_cleanup/main.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.1/mac_cleanup/parser.py` & `mac_cleanup-3.0.2/mac_cleanup/parser.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.1/mac_cleanup/progress.py` & `mac_cleanup-3.0.2/mac_cleanup/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         :param prompt_text: Text to be shown in panel
         :param prompt_title: Title of panel to be shown
         :param password: Enable password input. Defaults to False.
         :param choices: A list of valid choices. Defaults to None.
         :param show_default: Show default in prompt. Defaults to True.
         :param show_choices: Show choices in prompt. Defaults to True.
         :return: True on successful prompt
-
         """
 
         # Stop refreshing progress bar
         self.current_progress.stop()
 
         # Print prompt to user
         print_panel(text=prompt_text, title=prompt_title)
@@ -89,15 +88,14 @@
         """
         Wrapper other :func:`rich.progress.track`
 
         :param sequence: Sequence (must support "len") you wish to iterate over.
         :param total: Total number of steps. Default is len(sequence).
         :param description: Description of task show next to progress bar. Defaults to "Working".
         :return: An iterable of the values in the sequence
-
         """
 
         # Clear previous Live instance
         self.current_progress.console.clear_live()
 
         # Get new progress instance with default stuff
         self.__init__()
```

### Comparing `mac_cleanup-3.0.1/mac_cleanup/utils.py` & `mac_cleanup-3.0.2/mac_cleanup/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 def cmd(command: str, *, ignore_errors: bool = True) -> str:
     """
     Executes command in Popen.
 
     :param command: Bash command
     :param ignore_errors: If True, no stderr in return
     :return: stdout of executed command
-
     """
 
     from subprocess import DEVNULL, PIPE, Popen
 
     # Get stdout and stderr from PIPE
     out_tuple = Popen(command, shell=True, stdout=PIPE, stderr=(DEVNULL if ignore_errors else PIPE)).communicate()
 
@@ -32,15 +31,14 @@
 @beartype
 def expanduser(str_path: str) -> str:
     """
     Expands user.
 
     :param str_path: Path to be expanded
     :return: Path with extended user path as a posix
-
     """
 
     from pathlib import Path
 
     return Path(str_path).expanduser().as_posix()
 
 
@@ -48,15 +46,14 @@
 def check_exists(path: Path | str, *, expand_user: bool = True) -> bool:
     """
     Checks if path exists.
 
     :param path: Path to be checked
     :param expand_user: True if path needs to be expanded
     :return: True if specified path exists
-
     """
 
     if not isinstance(path, Path):
         path = Path(path)
 
     if expand_user:
         path = path.expanduser()
@@ -71,15 +68,14 @@
 @beartype
 def check_deletable(path: Path | str) -> bool:
     """
     Checks if path is deletable.
 
     :param path: Path to be deleted
     :return: True if specified path is deletable
-
     """
 
     # Convert path to correct type
     if not isinstance(path, Path):
         path_: Path = Path(path)
     else:
         path_ = path
@@ -105,15 +101,14 @@
 @beartype
 def bytes_to_human(size_bytes: int | float) -> str:
     """
     Converts bytes to human-readable format.
 
     :param size_bytes: Bytes
     :return: Human readable size
-
     """
 
     from math import floor, log, pow
 
     if size_bytes <= 0:
         return "0B"
```

### Comparing `mac_cleanup-3.0.1/pyproject.toml` & `mac_cleanup-3.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mac_cleanup"
-version = "3.0.1"
+version = "3.0.2"
 description = "Python cleanup script for macOS"
 license = "Apache-2.0"
 authors = [ "Drugsosos" ]
 readme = "README.md"
 homepage = "https://github.com/mac-cleanup/mac-cleanup-py"
 repository = "https://github.com/mac-cleanup/mac-cleanup-py"
 keywords = [
@@ -26,38 +26,38 @@
 [tool.poetry.urls]
 "Documentation" = "https://github.com/mac-cleanup/mac-cleanup-py#install-automatically"
 "Issue Tracker" = "https://github.com/mac-cleanup/mac-cleanup-py/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-rich = "^13.3.4"
+rich = "^13.3.5"
 attrs = "^23.1.0"
 inquirer = "^3.1.3"
 toml = "^0.10.2"
-beartype = "^0.13.1"
+beartype = "^0.14.0"
 
 [tool.poetry.scripts]
 mac-cleanup = "mac_cleanup:main"
 
 [tool.poetry.group.test.dependencies]
-tox = "^4.5.0"
+tox = "^4.5.1"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-pyright = "^1.1.304"
-ruff = "^0.0.263"
+pyright = "^1.1.309"
+ruff = "^0.0.269"
 
 [tool.poetry.group.dev.dependencies]
-commitizen = "^3.0.1"
-pre-commit = "^3.2.2"
+commitizen = "^3.2.2"
+pre-commit = "^3.3.2"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
-docformatter = "^1.6.3"
+docformatter = "^1.7.1"
 
 [build-system]
 requires = [ "poetry-core>=1.0.0" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -76,15 +76,14 @@
 
 [tool.docformatter]
 wrap-summaries = 100
 wrap-descriptions = 100
 tab-width = 4
 pre-summary-newline = true
 close-quotes-on-newline = true
-blank = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version_files = [ "pyproject.toml:version" ]
 tag_format = "v$version"
 
 [tool.coverage.run]
```

### Comparing `mac_cleanup-3.0.1/PKG-INFO` & `mac_cleanup-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mac-cleanup
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python cleanup script for macOS
 Home-page: https://github.com/mac-cleanup/mac-cleanup-py
 License: Apache-2.0
 Keywords: macos,script,cleanup,cleaner
 Author: Drugsosos
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
@@ -12,17 +12,17 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: beartype (>=0.13.1,<0.14.0)
+Requires-Dist: beartype (>=0.14.0,<0.15.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/mac-cleanup/mac-cleanup-py#install-automatically
 Project-URL: Issue Tracker, https://github.com/mac-cleanup/mac-cleanup-py/issues
 Project-URL: Repository, https://github.com/mac-cleanup/mac-cleanup-py
 Description-Content-Type: text/markdown
 
 # mac-cleanup-py
@@ -129,15 +129,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.1
+    3.0.2
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

