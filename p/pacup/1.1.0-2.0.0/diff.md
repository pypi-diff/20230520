# Comparing `tmp/pacup-1.1.0.tar.gz` & `tmp/pacup-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacup-1.1.0.tar", max compression
+gzip compressed data, was "pacup-2.0.0.tar", max compression
```

## Comparing `pacup-1.1.0.tar` & `pacup-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-09 18:28:38.038072 pacup-1.1.0/LICENSE
--rw-r--r--   0        0        0      829 2023-04-09 18:28:38.038072 pacup-1.1.0/LICENSE_BOILERPLATE
--rw-r--r--   0        0        0     7904 2023-04-09 18:28:38.038072 pacup-1.1.0/README.md
--rw-r--r--   0        0        0      870 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/__init__.py
--rw-r--r--   0        0        0    33430 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/__main__.py
--rw-r--r--   0        0        0    10404 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/parser.py
--rw-r--r--   0        0        0     6617 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/release_notes.py
--rw-r--r--   0        0        0     1207 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/utils.py
--rw-r--r--   0        0        0     7683 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/version.py
--rw-r--r--   0        0        0     1951 2023-04-09 18:28:38.038072 pacup-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9480 1970-01-01 00:00:00.000000 pacup-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-20 17:02:04.741627 pacup-2.0.0/LICENSE
+-rw-r--r--   0        0        0      829 2023-05-20 17:02:04.741627 pacup-2.0.0/LICENSE_BOILERPLATE
+-rw-r--r--   0        0        0     7906 2023-05-20 17:02:04.741627 pacup-2.0.0/README.md
+-rw-r--r--   0        0        0      870 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/__init__.py
+-rw-r--r--   0        0        0    33849 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/__main__.py
+-rw-r--r--   0        0        0    10361 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/parser.py
+-rw-r--r--   0        0        0     6574 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/release_notes.py
+-rw-r--r--   0        0        0     1216 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/utils.py
+-rw-r--r--   0        0        0     7615 2023-05-20 17:02:04.741627 pacup-2.0.0/pacup/version.py
+-rw-r--r--   0        0        0     1953 2023-05-20 17:02:04.745627 pacup-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9282 1970-01-01 00:00:00.000000 pacup-2.0.0/PKG-INFO
```

### Comparing `pacup-1.1.0/LICENSE` & `pacup-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pacup-1.1.0/LICENSE_BOILERPLATE` & `pacup-2.0.0/LICENSE_BOILERPLATE`

 * *Files identical despite different names*

### Comparing `pacup-1.1.0/README.md` & `pacup-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center"><img alt="logo" src="https://raw.githubusercontent.com/pacstall/pacup/master/imgs/logo.png"></p>
 <h1 align="center">Pacup</h1>
 <p align="center">
-  <a href="https://www.python.org/"><img alt="Python: 3.8+" src="https://img.shields.io/badge/python-3.8%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>
+  <a href="https://www.python.org/"><img alt="Python: 3.10+" src="https://img.shields.io/badge/python-3.10%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black?style=for-the-badge"/></a>
   <a href="https://www.codacy.com/gh/pacstall/pacup/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pacstall/pacup&amp;utm_campaign=Badge_Grade"><img alt="Codacy: grade" src="https://img.shields.io/codacy/grade/4b1365e6f7d2474283243f62b2c5973d?label=Codacy&logo=codacy&style=for-the-badge"></a>
   <a href="https://pypi.org/project/pacup/"><img alt="PyPI: version" src="https://img.shields.io/pypi/v/pacup?color=%233775a9&logo=pypi&logoColor=white&style=for-the-badge"></a>
 <p/>
 <p align="center">
   <!-- Social -->
   <a href="https://discord.gg/yzrjXJV6K8"><img alt="join discord" src="https://img.shields.io/discord/839818021207801878?color=5865F2&label=Discord&logo=discord&logoColor=FFFFFF&style=for-the-badge"></a>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                                     [logo]
                               ****** Pacup ******
-      [Python:_3.8+] [Code_style:_black] [Codacy:_grade] [PyPI:_version]
+      [Python:_3.10+] [Code_style:_black] [Codacy:_grade] [PyPI:_version]
       [join_discord] [https://img.shields.io/reddit/subreddit-subscribers/
                pacstall?label=Reddit&color=FF4301&style=for-the-
       badge&logo=reddit&logoColor=FFFFFF] [Mastodon_Follow] [join_matrix]
 ## What is this? Pacup (**Pac**script **Up**dater) is a maintainer helper tool
 to help maintainers update their pacscripts. It semi-automates the tedious task
 of updating pacscripts, and aims to make it a fun process for the maintainer!
 ## Installation To install the latest release run: ```console $ pacstall -
```

### Comparing `pacup-1.1.0/pacup/__init__.py` & `pacup-2.0.0/pacup/__init__.py`

 * *Files identical despite different names*

### Comparing `pacup-1.1.0/pacup/__main__.py` & `pacup-2.0.0/pacup/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 """The main Pacup launcher file."""
 
 
 import hashlib
 import subprocess
 import sys
 from asyncio import Semaphore, gather, get_event_loop_policy
+from collections.abc import Generator
 from difflib import unified_diff
 from logging import basicConfig, getLogger
 from os import get_terminal_size, makedirs
 from pathlib import Path
 from shutil import rmtree
-from typing import Dict, Generator, List, NoReturn, Optional
+from typing import Annotated, NoReturn, Optional
 
 import typer
 from httpx import AsyncClient, HTTPStatusError, RequestError, Response
 from rich import print as rprint
 from rich import traceback
 from rich.logging import RichHandler
 from rich.markdown import Markdown
@@ -59,17 +60,19 @@
 from rich.syntax import Syntax
 from rich.table import Table
 
 from pacup.parser import Pacscript
 from pacup.utils import level
 from pacup.version import VersionStatuses
 
-__version__ = "1.1.0 Io"
+__version__ = "2.0.0 Sirius"
 
-app = typer.Typer(name="pacup")
+app = typer.Typer(
+    name="pacup", context_settings={"help_option_names": ["-h", "--help"]}
+)
 
 
 basicConfig(level="CRITICAL", format="%(message)s", handlers=[RichHandler(markup=True)])
 log = getLogger("rich")
 
 
 async def download(url: str, progress: Progress, task: TaskID) -> str:
@@ -129,19 +132,19 @@
                     if "content-length" in response.headers:
                         return await _process_response(response)
 
         return await _process_response(response)
 
 
 async def get_parsed_pacscripts(
-    pacscripts: List[Path],
+    pacscripts: list[Path],
     task: TaskID,
     progress: Progress,
-    show_repology: Optional[bool],
-) -> List[Pacscript]:
+    show_repology: bool | None,
+) -> list[Pacscript]:
     """
     Get the parsed pacscripts from a list of pacscript paths.
 
     Parameters
     ----------
     pacscripts
         The list of pacscripts to parse.
@@ -174,15 +177,15 @@
                 )
                 for pacscript in pacscripts
             ],
             return_exceptions=True,
         )
 
 
-def validate_parameters(ctx: typer.Context, pacscripts: List[Path]) -> List[Path]:
+def validate_parameters(ctx: typer.Context, pacscripts: list[Path]) -> list[Path]:
     """
     Validate command parameters.
 
     Parameters
     ----------
     ctx
         The typer context.
@@ -262,45 +265,57 @@
     """
 
     if value:
         rprint(f"PacUp {__version__}")
         raise typer.Exit()
 
 
+# HACK: This uses `Optional` due to a typer bug: https://github.com/tiangolo/typer/issues/533
 @app.command()
 def command(
-    show_repology: Optional[bool] = typer.Option(
-        None,
-        "-r",
-        "--show-repology",
-        help="Show the parsed repology data and exit.",
-    ),
-    debug: Optional[bool] = typer.Option(
-        None, "-d", "--debug", help="Turn on debugging mode."
-    ),
-    _: Optional[bool] = typer.Option(
-        None,
-        "-v",
-        "--version",
-        help="Show the version and exit.",
-        callback=version_callback,
-        is_eager=True,
-    ),
-    ship: Optional[bool] = typer.Option(
-        None, "-s", "--ship", help="Prepare the pacscript for shipping to upstream."
-    ),
-    pacscripts: List[Path] = typer.Argument(
-        ...,
-        help="The pacscripts to update.",
-        exists=True,
-        writable=True,
-        dir_okay=False,
-        callback=validate_parameters,
-        autocompletion=autocomplete_command,
-    ),
+    pacscripts: Annotated[
+        list[Path],
+        typer.Argument(
+            show_default=False,
+            exists=True,
+            writable=True,
+            dir_okay=False,
+            callback=validate_parameters,
+            autocompletion=autocomplete_command,
+            help="The pacscripts to update.",
+        ),
+    ],
+    show_repology: Annotated[
+        Optional[bool],
+        typer.Option(
+            "-r",
+            "--show-repology",
+            help="Show the parsed repology data and exit.",
+        ),
+    ] = None,
+    debug: Annotated[
+        Optional[bool],
+        typer.Option("-d", "--debug", help="Turn on debugging mode."),
+    ] = None,
+    _: Annotated[
+        Optional[bool],
+        typer.Option(
+            "-v",
+            "--version",
+            help="Show the version and exit.",
+            callback=version_callback,
+            is_eager=True,
+        ),
+    ] = None,
+    ship: Annotated[
+        Optional[bool],
+        typer.Option(
+            "-s", "--ship", help="Prepare the pacscript for shipping to upstream."
+        ),
+    ] = None,
 ) -> NoReturn:
     """
     Updates specified pacscripts.
 
     If ship flag is passed, the pacscript will be prepared for shipping to
     upstream. After the pacscript is prepared, it will be committed and pushed
     to the origin remote. This requires you to be present in your cloned fork.
@@ -320,31 +335,31 @@
         transient=True,
     ) as parsing_pacscripts_progress:
         log.info(f"Parsing {len(pacscripts)} pacscripts")
         task = parsing_pacscripts_progress.add_task(
             "Parsing pacscripts", total=len(pacscripts)
         )
         loop = get_event_loop_policy().get_event_loop()
-        parsed_pacscripts: List[Pacscript] = loop.run_until_complete(
+        parsed_pacscripts: list[Pacscript] = loop.run_until_complete(
             get_parsed_pacscripts(
                 pacscripts, task, parsing_pacscripts_progress, show_repology
             )
         )
         log.debug(f"{parsed_pacscripts = }")
         parsing_pacscripts_progress.advance(task)
 
     # Display the summary to the user
     log.info("Sorting parsed pacscripts by version statsuses...")
     version_statuses_table = Table.grid()
     version_statuses_table.add_column()
 
-    outdated_pacscripts: List[Pacscript] = []
-    updated_pacscripts: List[Pacscript] = []
-    newer_pacscripts: List[Pacscript] = []
-    unknown_pacscripts: List[Pacscript] = []
+    outdated_pacscripts: list[Pacscript] = []
+    updated_pacscripts: list[Pacscript] = []
+    newer_pacscripts: list[Pacscript] = []
+    unknown_pacscripts: list[Pacscript] = []
     for pacscript in parsed_pacscripts:
         if pacscript.version.status == VersionStatuses.OUTDATED:
             outdated_pacscripts.append(pacscript)
         elif pacscript.version.status == VersionStatuses.UPDATED:
             updated_pacscripts.append(pacscript)
         elif pacscript.version.status == VersionStatuses.NEWER:
             newer_pacscripts.append(pacscript)
@@ -458,16 +473,16 @@
 
     if show_repology:
         log.info("Exiting early due to [code]show_repology[/code] flag")
         sys.exit()
 
     # Loop through the parsed pacscripts and update them
     log.info("Updating pacscripts...")
-    successfully_updated_pacscripts: List[Pacscript] = []
-    failed_to_update_pacscripts: Dict[Pacscript, str] = {}
+    successfully_updated_pacscripts: list[Pacscript] = []
+    failed_to_update_pacscripts: dict[Pacscript, str] = {}
     for pacscript in outdated_pacscripts:
         path = pacscript.path
         pkgname = pacscript.pkgname
         version = pacscript.version
         url = pacscript.url
         hash_line = pacscript.hash_line
         release_notes = pacscript.release_notes
```

### Comparing `pacup-1.1.0/pacup/parser.py` & `pacup-2.0.0/pacup/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 """ The pacscript parser module."""
 
 
 from asyncio.locks import Semaphore
 from asyncio.subprocess import PIPE, Process, create_subprocess_shell
 from logging import getLogger
 from pathlib import Path
-from typing import Dict, List, Optional
 
 from httpx import AsyncClient, HTTPStatusError, RequestError
 from rich.progress import Progress, TaskID
 
 from pacup.release_notes import Github, Gitlab
 from pacup.version import Version
 
@@ -137,17 +136,17 @@
         self,
         path: Path,
         pkgname: str,
         version: Version,
         url: Url,
         hash_line: int,
         maintainer: str,
-        repology_filters: Dict[str, str],
-        release_notes: Dict[str, str],
-        lines: List[str],
+        repology_filters: dict[str, str],
+        release_notes: dict[str, str],
+        lines: list[str],
     ):
         """
         Parameters
         ----------
         path
             The path to the pacscript.
         pkgname
@@ -182,15 +181,15 @@
     async def parse(
         cls,
         path: Path,
         client: AsyncClient,
         semaphore: Semaphore,
         task: TaskID,
         progress: Progress,
-        show_repology: Optional[bool],
+        show_repology: bool | None,
     ) -> "Pacscript":
         """
         Parses a pacscript file.
 
         Parameters
         ----------
         path
@@ -220,15 +219,15 @@
         pkgname = path.stem.replace("-bin", "").replace("-deb", "").replace("-app", "")
 
         # Instantiate placeholder variables
         version = Version()
         url = Url()
         hash_line = -1  # Which line contains the hash
         maintainer = ""
-        repology_filters: Dict[str, str] = {}
+        repology_filters: dict[str, str] = {}
         release_notes = {}
 
         pacscript_reader_process = await create_subprocess_shell(
             "/usr/bin/env bash", stdin=PIPE, stdout=PIPE
         )
 
         assert pacscript_reader_process.stdin is not None
```

### Comparing `pacup-1.1.0/pacup/release_notes.py` & `pacup-2.0.0/pacup/release_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 """The release notes processor module."""
 
 # WARNING: Shit code ahead, feel free to improve.
 
 from abc import ABC, abstractmethod
 from logging import getLogger
-from typing import Dict, List, Optional
 
 from httpx import AsyncClient
 
 log = getLogger("rich")
 
 
 class Repository(ABC):
@@ -62,30 +61,30 @@
         log.info(f"Processing {self.__class__.__name__} release notes...")
         self.current_release = current_release
         self.url = url
         self.client = client
 
     @property
     @abstractmethod
-    async def release_notes(self) -> Optional[Dict[str, str]]:
+    async def release_notes(self) -> dict[str, str] | None:
         """
         Returns the release notes of the releases from the latest to the
         current release.
 
         Returns
         -------
         Optional[Dict[str, str]]
             The release notes of the releases from the latest to the current
             release.
         """
         ...
 
     def _back_calculate_current_release_index(
         self,
-        releases: List[Dict[str, str]],
+        releases: list[dict[str, str]],
     ) -> int:
         """
         Back calculates the index of the current release in the list of releases.
 
         Parameters
         ----------
         releases
@@ -108,16 +107,16 @@
 
         log.error("Could not find current release in release notes")
         return -1
 
     def _get_release_notes(
         self,
         current_release_index: int,
-        response: List[Dict[str, str]],
-    ) -> Dict[str, str]:
+        response: list[dict[str, str]],
+    ) -> dict[str, str]:
         """
         Returns the release notes of the releases from the latest to the
         current release.
 
         Parameters
         ----------
         current_release_index
@@ -129,15 +128,15 @@
         Returns
         -------
         Dict[str, str]
             The release notes of the releases from the latest to the current
             release.
         """
 
-        release_notes: Dict[str, str] = {}
+        release_notes: dict[str, str] = {}
         for index, release in enumerate(response):
             if index == current_release_index:
                 break
 
             release_notes[release[self.tag_name]] = release[self.description]
 
             log.debug(f"{release_notes = }")
@@ -150,15 +149,15 @@
     The Github class is a concrete implementation of the Repository class that
     fetches the release notes from the Github repository.
     """
 
     description = "body"
 
     @property
-    async def release_notes(self) -> Dict[str, str]:
+    async def release_notes(self) -> dict[str, str]:
         """Get the release notes of the releases from the latest to the current."""
 
         owner = self.url.split("/")[3]
         repo = self.url.split("/")[4]
 
         log.debug(f"{owner = }")
         log.debug(f"{repo = }")
@@ -186,15 +185,15 @@
 class Gitlab(Repository):
     """
     The Gitlab class is a concrete implementation of the Repository class that
     fetches the release notes from the Gitlab repository.
     """
 
     @property
-    async def release_notes(self) -> Dict[str, str]:
+    async def release_notes(self) -> dict[str, str]:
         """Get the release notes of the releases from the latest to the current."""
 
         if "projects" in self.url:
             # NOTE: https://gitlab.com/api/v4/projects/24386000/...
             log.info("ID type URL detected.")
             identifier = self.url.split("/")[6]
             log.debug(f"{identifier = }")
```

### Comparing `pacup-1.1.0/pacup/utils.py` & `pacup-2.0.0/pacup/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PacUp.  If not, see <https://www.gnu.org/licenses/>.
 
 """Utility functions."""
 
+from collections.abc import Generator
 from contextlib import contextmanager
-from typing import Generator
 
 current_level = 0
 
 
 @contextmanager
 def level() -> Generator[str, None, None]:
     """Context manager for printing with indentation."""
```

### Comparing `pacup-1.1.0/pacup/version.py` & `pacup-2.0.0/pacup/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 # You should have received a copy of the GNU General Public License
 # along with PacUp.  If not, see <https://www.gnu.org/licenses/>.
 
 """The version processor module."""
 
 
 from asyncio.locks import Semaphore
+from collections import Counter
 from enum import Enum, auto
 from logging import getLogger
-from typing import Any, Counter, Dict, List, Literal, Optional, Union
+from typing import Any, Literal
 
 from httpx import AsyncClient, HTTPStatusError, RequestError
 from packaging import version as pkg_version
 from rich import print as rprint
 from rich.panel import Panel
 from rich.pretty import Pretty
 from rich.table import Table
@@ -73,37 +74,35 @@
         The latest version of the package.
     status
         The status of the version.
     """
 
     line_number: int = -1
     current: str = ""
-    __latest: str = ""
+    latest: str = ""
 
     def __init__(self, line_number: int = -1, version: str = "", latest: str = ""):
         self.line_number = line_number
         self.current = version
         self.latest = latest
 
     @staticmethod
     async def get_latest_version(
-        filters: Dict[str, str],
+        filters: dict[str, str],
         client: AsyncClient,
         semaphore: Semaphore,
-        show_repology: Optional[bool],
+        show_repology: bool | None,
     ) -> (
-        Union[
-            str,
-            Literal[
-                RepologyErrors.NOT_FOUND,
-                RepologyErrors.NO_PROJECT_FILTER,
-                RepologyErrors.NO_FILTERS,
-                RepologyErrors.HTTP_STATUS_ERROR,
-                RepologyErrors.REQUEST_ERROR,
-            ],
+        str
+        | Literal[
+            RepologyErrors.NOT_FOUND,
+            RepologyErrors.NO_PROJECT_FILTER,
+            RepologyErrors.NO_FILTERS,
+            RepologyErrors.HTTP_STATUS_ERROR,
+            RepologyErrors.REQUEST_ERROR,
         ]
     ):
         """
         Gets the latest version of a package from repology.
 
         Parameters
         ----------
@@ -152,28 +151,28 @@
 
             try:
                 response.raise_for_status()
             except HTTPStatusError:
                 return RepologyErrors.HTTP_STATUS_ERROR
 
             else:
-                filtered: List[Dict[str, Any]] = response.json()
+                filtered: list[dict[str, Any]] = response.json()
 
                 log.info("Filtering...")
                 for key, value in filters.items():
                     if new_filtered := [
                         packages
                         for packages in filtered
                         if key in packages and packages[key] == value
                     ]:
                         filtered = new_filtered
 
                 # Map the versions to their list of packages
                 log.info("Mapping the versions to their filtered packages...")
-                versions: List[str] = [package["version"] for package in filtered]
+                versions: list[str] = [package["version"] for package in filtered]
 
                 log.debug(f"{filtered = }")
                 log.debug(f"{versions = }")
 
                 log.info("Selecting most common version...")
                 selected_version = Counter(versions).most_common(1)[0][0]
                 log.debug(f"{selected_version = }")
```

### Comparing `pacup-1.1.0/pyproject.toml` & `pacup-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pacup"
-version = "1.1.0"
+version = "2.0.0"
 description = "Help maintainers update pacscripts"
 readme = "README.md"
 authors = ["Sourajyoti Basak <wiz28@protonmail.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/pacstall/pacup"
 documentation = "https://github.com/pacstall/pacup/wiki"
 keywords = [
@@ -32,19 +32,19 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: System",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-httpx = ">=0.22,<0.24"
+python = ">=3.10,<3.12"
+httpx = ">=0.24,<0.25"
 rich = "^13.0.0"
-typer = ">=0.4.1,<0.8.0"
-packaging = ">=23,<23.1"
+typer = ">=0.9.0,<0.10.0"
+packaging = ">=23,<23.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
 codespell = "^2.2.2"
 isort = "^5.11.2"
 mypy = "^1.0"
 pre-commit = "^3.0.0"
```

### Comparing `pacup-1.1.0/PKG-INFO` & `pacup-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 Metadata-Version: 2.1
 Name: pacup
-Version: 1.1.0
+Version: 2.0.0
 Summary: Help maintainers update pacscripts
 Home-page: https://github.com/pacstall/pacup
 License: GPL-3.0-or-later
 Keywords: aur,cli,command line,console,debian,pacscript,pacstall,ubuntu,repology
 Author: Sourajyoti Basak
 Author-email: wiz28@protonmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: httpx (>=0.22,<0.24)
-Requires-Dist: packaging (>=23,<23.1)
+Requires-Dist: httpx (>=0.24,<0.25)
+Requires-Dist: packaging (>=23,<23.2)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
-Requires-Dist: typer (>=0.4.1,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/pacstall/pacup/wiki
 Project-URL: Repository, https://github.com/pacstall/pacup
 Description-Content-Type: text/markdown
 
 <p align="center"><img alt="logo" src="https://raw.githubusercontent.com/pacstall/pacup/master/imgs/logo.png"></p>
 <h1 align="center">Pacup</h1>
 <p align="center">
-  <a href="https://www.python.org/"><img alt="Python: 3.8+" src="https://img.shields.io/badge/python-3.8%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>
+  <a href="https://www.python.org/"><img alt="Python: 3.10+" src="https://img.shields.io/badge/python-3.10%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black?style=for-the-badge"/></a>
   <a href="https://www.codacy.com/gh/pacstall/pacup/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pacstall/pacup&amp;utm_campaign=Badge_Grade"><img alt="Codacy: grade" src="https://img.shields.io/codacy/grade/4b1365e6f7d2474283243f62b2c5973d?label=Codacy&logo=codacy&style=for-the-badge"></a>
   <a href="https://pypi.org/project/pacup/"><img alt="PyPI: version" src="https://img.shields.io/pypi/v/pacup?color=%233775a9&logo=pypi&logoColor=white&style=for-the-badge"></a>
 <p/>
 <p align="center">
   <!-- Social -->
   <a href="https://discord.gg/yzrjXJV6K8"><img alt="join discord" src="https://img.shields.io/discord/839818021207801878?color=5865F2&label=Discord&logo=discord&logoColor=FFFFFF&style=for-the-badge"></a>
```

#### html2text {}

```diff
@@ -1,32 +1,29 @@
-Metadata-Version: 2.1 Name: pacup Version: 1.1.0 Summary: Help maintainers
+Metadata-Version: 2.1 Name: pacup Version: 2.0.0 Summary: Help maintainers
 update pacscripts Home-page: https://github.com/pacstall/pacup License: GPL-
 3.0-or-later Keywords: aur,cli,command
 line,console,debian,pacscript,pacstall,ubuntu,repology Author: Sourajyoti Basak
-Author-email: wiz28@protonmail.com Requires-Python: >=3.8,<3.12 Classifier:
+Author-email: wiz28@protonmail.com Requires-Python: >=3.10,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Operating System ::
 POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: System Classifier: Topic :: Utilities Classifier: Typing
-:: Typed Requires-Dist: httpx (>=0.22,<0.24) Requires-Dist: packaging
-(>=23,<23.1) Requires-Dist: rich (>=13.0.0,<14.0.0) Requires-Dist: typer
-(>=0.4.1,<0.8.0) Project-URL: Documentation, https://github.com/pacstall/pacup/
-wiki Project-URL: Repository, https://github.com/pacstall/pacup Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: System Classifier: Topic ::
+Utilities Classifier: Typing :: Typed Requires-Dist: httpx (>=0.24,<0.25)
+Requires-Dist: packaging (>=23,<23.2) Requires-Dist: rich (>=13.0.0,<14.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0) Project-URL: Documentation, https://
+github.com/pacstall/pacup/wiki Project-URL: Repository, https://github.com/
+pacstall/pacup Description-Content-Type: text/markdown
                                     [logo]
                               ****** Pacup ******
-      [Python:_3.8+] [Code_style:_black] [Codacy:_grade] [PyPI:_version]
+      [Python:_3.10+] [Code_style:_black] [Codacy:_grade] [PyPI:_version]
       [join_discord] [https://img.shields.io/reddit/subreddit-subscribers/
                pacstall?label=Reddit&color=FF4301&style=for-the-
       badge&logo=reddit&logoColor=FFFFFF] [Mastodon_Follow] [join_matrix]
 ## What is this? Pacup (**Pac**script **Up**dater) is a maintainer helper tool
 to help maintainers update their pacscripts. It semi-automates the tedious task
 of updating pacscripts, and aims to make it a fun process for the maintainer!
 ## Installation To install the latest release run: ```console $ pacstall -
```

