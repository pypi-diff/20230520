# Comparing `tmp/cpp_linter-1.5.1-py3-none-any.whl.zip` & `tmp/cpp_linter-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 28169 bytes, number of entries: 14
--rw-r--r--  2.0 unx     6817 b- defN 23-Feb-18 07:57 cpp_linter/__init__.py
--rw-r--r--  2.0 unx     5449 b- defN 23-Feb-18 07:57 cpp_linter/clang_format_xml.py
--rw-r--r--  2.0 unx     4532 b- defN 23-Feb-18 07:57 cpp_linter/clang_tidy.py
--rw-r--r--  2.0 unx     4743 b- defN 23-Feb-18 07:57 cpp_linter/clang_tidy_yml.py
--rw-r--r--  2.0 unx     7351 b- defN 23-Feb-18 07:57 cpp_linter/cli.py
--rw-r--r--  2.0 unx     6376 b- defN 23-Feb-18 07:57 cpp_linter/git.py
--rw-r--r--  2.0 unx    31089 b- defN 23-Feb-18 07:57 cpp_linter/run.py
--rw-r--r--  2.0 unx    10849 b- defN 23-Feb-18 07:57 cpp_linter/thread_comments.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2811 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1141 b- defN 23-Feb-18 07:58 cpp_linter-1.5.1.dist-info/RECORD
-14 files, 82379 bytes uncompressed, 26281 bytes compressed:  68.1%
+Zip file size: 28444 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     6894 b- defN 23-May-20 09:38 cpp_linter/__init__.py
+-rw-r--r--  2.0 unx     5449 b- defN 23-May-20 09:38 cpp_linter/clang_format_xml.py
+-rw-r--r--  2.0 unx     4399 b- defN 23-May-20 09:38 cpp_linter/clang_tidy.py
+-rw-r--r--  2.0 unx     4743 b- defN 23-May-20 09:38 cpp_linter/clang_tidy_yml.py
+-rw-r--r--  2.0 unx     7646 b- defN 23-May-20 09:38 cpp_linter/cli.py
+-rw-r--r--  2.0 unx     6377 b- defN 23-May-20 09:38 cpp_linter/git.py
+-rw-r--r--  2.0 unx    31645 b- defN 23-May-20 09:38 cpp_linter/run.py
+-rw-r--r--  2.0 unx    10871 b- defN 23-May-20 09:38 cpp_linter/thread_comments.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2811 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1141 b- defN 23-May-20 09:38 cpp_linter-1.6.0.dist-info/RECORD
+14 files, 83197 bytes uncompressed, 26556 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: cpp_linter/run.py
 Comment: 
 
 Filename: cpp_linter/thread_comments.py
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/LICENSE
+Filename: cpp_linter-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/METADATA
+Filename: cpp_linter-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/WHEEL
+Filename: cpp_linter-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/entry_points.txt
+Filename: cpp_linter-1.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/top_level.txt
+Filename: cpp_linter-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cpp_linter-1.5.1.dist-info/RECORD
+Filename: cpp_linter-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cpp_linter/__init__.py

```diff
@@ -57,17 +57,18 @@
         headers["Authorization"] = f"token {GITHUB_TOKEN}"
     return headers
 
 
 class Globals:
     """Global variables for re-use (non-constant)."""
 
-    PAYLOAD_TIDY: str = ""
+    TIDY_COMMENT: str = ""
     """The accumulated output of clang-tidy (gets appended to OUTPUT)"""
-    OUTPUT: str = ""
+    FORMAT_COMMENT: str = ""
+    OUTPUT: str = "<!-- cpp linter action -->\n# Cpp-Linter Report "
     """The accumulated body of the resulting comment that gets posted."""
     FILES: List[Dict[str, Any]] = []
     """The responding payload containing info about changed files."""
     EVENT_PAYLOAD: Dict[str, Any] = {}
     """The parsed JSON of the event payload."""
     response_buffer: Response = Response()
     """A shared response object for `requests` module."""
```

## cpp_linter/clang_tidy.py

```diff
@@ -1,14 +1,15 @@
 """Parse output from clang-tidy's stdout"""
 from pathlib import Path, PurePath
+from textwrap import indent
 import re
 from typing import Tuple, Union, List, cast
 from . import GlobalParser, CLANG_TIDY_STDOUT
 
-NOTE_HEADER = re.compile(r"^(.*):(\d+):(\d+):\s(\w+):(.*)\[(.*)\]$")
+NOTE_HEADER = re.compile(r"^(.+):(\d+):(\d+):\s(\w+):(.*)\[(.*)\]$")
 
 
 class TidyNotification:
     """Create a object that decodes info from the clang-tidy output's initial line that
     details a specific notification.
 
     :param notification_line: The first line in the notification parsed into a
@@ -52,25 +53,19 @@
             if not self.fixit_lines[-1].endswith("\n"):
                 # some notifications' code-blocks don't end in a LF
                 self.fixit_lines[-1] += "\n"  # and they should for us
             concerned_code = "```{}\n{}```\n".format(
                 PurePath(self.filename).suffix.lstrip("."),
                 "\n".join(self.fixit_lines),
             )
-        return (
-            "<details open>\n<summary><strong>{}:{}:{}:</strong> {}: [{}]"
-            "\n\n> {}\n</summary><p>\n\n{}</p>\n</details>\n\n".format(
-                self.filename,
-                self.line,
-                self.cols,
-                self.note_type,
-                self.diagnostic,
-                self.note_info,
-                concerned_code,
-            )
+        return indent(
+            f"<strong>{self.filename}:{self.line}:{self.cols}:</strong> "
+            + f"{self.note_type}: [{self.diagnostic}]\n> {self.note_info}"
+            + f"\n\n{concerned_code}\n",
+            "   "
         )
 
     def log_command(self) -> str:
         """Output the notification as a github log command.
 
         .. seealso::
```

## cpp_linter/cli.py

```diff
@@ -179,14 +179,24 @@
     If run on a private repository, then this feature is
     disabled because the GitHub REST API behaves
     differently for thread comments on a private repository.
 
 Defaults to ``%(default)s``.""",
 )
 cli_arg_parser.add_argument(
+    "-w",
+    "--step-summary",
+    default="false",
+    type=lambda input: input.lower() == "true",
+    help="""Set this option to true or false to enable or disable the use of
+a workflow step summary when the run has concluded.
+
+Defaults to ``%(default)s``.""",
+)
+cli_arg_parser.add_argument(
     "-a",
     "--file-annotations",
     default="true",
     type=lambda input: input.lower() == "true",
     help="""Set this option to false to disable the use of
 file annotations as feedback.
```

## cpp_linter/git.py

```diff
@@ -108,22 +108,22 @@
         first_hunk = HUNK_INFO.search(diff)
         hunk_start = -1 if first_hunk is None else first_hunk.start()
         diff_front_matter = diff[:hunk_start]
         filename_match = _get_filename_from_diff(diff_front_matter)
         if filename_match is None:
             continue
         filename = filename_match.groups(0)[0]
-        file_objects.append(dict(filename=filename))
+        file_objects.append({"filename": filename})
         if first_hunk is None:
             continue
         ranges, additions = parse_patch(diff[first_hunk.start() :])
-        file_objects[-1]["line_filter"] = dict(
-            diff_chunks=ranges,
-            lines_added=consolidate_list_to_ranges(additions),
-        )
+        file_objects[-1]["line_filter"] = {
+            "diff_chunks": ranges,
+            "lines_added": consolidate_list_to_ranges(additions),
+        }
     return file_objects
 
 
 def parse_patch(full_patch: str) -> Tuple[List[List[int]], List[int]]:
     """Parse a diff's patch accordingly.
 
     :param full_patch: The entire patch of hunks for 1 file.
```

## cpp_linter/run.py

```diff
@@ -245,15 +245,15 @@
                     break
             else:
                 file_path = rel_path.as_posix()
                 logger.debug('"./%s" is a source code file', file_path)
                 if not is_file_in_list(
                     ignored_paths, file_path, "ignored"
                 ) or is_file_in_list(not_ignored, file_path, "not ignored"):
-                    Globals.FILES.append(dict(filename=file_path))
+                    Globals.FILES.append({"filename": file_path})
 
     if Globals.FILES:
         logger.info(
             "Giving attention to the following files:\n\t%s",
             "\n\t".join([f["filename"] for f in Globals.FILES]),
         )
     else:
@@ -314,17 +314,18 @@
     if checks:
         cmds.append(f"-checks={checks}")
     if database:
         cmds.append("-p")
         if not PurePath(database).is_absolute():
             database = str(Path(RUNNER_WORKSPACE, repo_root, database).resolve())
         cmds.append(database)
-    line_ranges = dict(
-        name=filename, lines=range_of_changed_lines(file_obj, lines_changed_only, True)
-    )
+    line_ranges = {
+        "name": filename,
+        "lines": range_of_changed_lines(file_obj, lines_changed_only, True),
+    }
     if line_ranges["lines"]:
         # logger.info("line_filter = %s", json.dumps([line_ranges]))
         cmds.append(f"--line-filter={json.dumps([line_ranges])}")
     if len(extra_args) == 1 and " " in extra_args[0]:
         extra_args = extra_args[0].split()
     for extra_arg in extra_args:
         cmds.append(f"--extra-arg={extra_arg}")
@@ -401,24 +402,21 @@
         avoid duplicated content in comment, and it is later used again by
         `make_annotations()` after `capture_clang_tools_output()` is finished.
     """
     ranges = range_of_changed_lines(file_obj, lines_changed_only)
     if CLANG_TIDY_STDOUT.exists() and CLANG_TIDY_STDOUT.stat().st_size:
         parse_tidy_output()  # get clang-tidy fixes from stdout
         comment_output = ""
-        if Globals.PAYLOAD_TIDY:
-            Globals.PAYLOAD_TIDY += "<hr></details>"
         for fix in GlobalParser.tidy_notes:
             if lines_changed_only and fix.line not in ranges:
                 continue
             comment_output += repr(fix)
             tidy_notes.append(fix)
         if comment_output:
-            Globals.PAYLOAD_TIDY += f"<details><summary>{filename}</summary><br>\n"
-            Globals.PAYLOAD_TIDY += comment_output
+            Globals.TIDY_COMMENT += f"- {filename}\n\n{comment_output}"
         GlobalParser.tidy_notes.clear()  # empty list to avoid duplicated output
 
     if CLANG_FORMAT_XML.exists() and CLANG_FORMAT_XML.stat().st_size:
         parse_format_replacements_xml(PurePath(filename).as_posix())
         if GlobalParser.format_advice and GlobalParser.format_advice[-1].replaced_lines:
             should_comment = lines_changed_only == 0
             if not should_comment:
@@ -426,18 +424,15 @@
                     replacement.line
                     for replacement in GlobalParser.format_advice[-1].replaced_lines
                 ]:
                     if line in ranges:
                         should_comment = True
                         break
             if should_comment:
-                if not Globals.OUTPUT:
-                    Globals.OUTPUT = "<!-- cpp linter action -->\n## :scroll: "
-                    Globals.OUTPUT += "Run `clang-format` on the following files\n"
-                Globals.OUTPUT += f"- [ ] {file_obj['filename']}\n"
+                Globals.FORMAT_COMMENT += f"- {file_obj['filename']}\n"
 
 
 def capture_clang_tools_output(
     version: str,
     checks: str,
     style: str,
     lines_changed_only: int,
@@ -476,21 +471,33 @@
             extra_args,
         )
         run_clang_format(filename, file, version, style, lines_changed_only)
         end_log_group()
 
         create_comment_body(filename, file, lines_changed_only, tidy_notes)
 
-    if Globals.PAYLOAD_TIDY:
-        if not Globals.OUTPUT:
-            Globals.OUTPUT = "<!-- cpp linter action -->\n"
-        else:
-            Globals.OUTPUT += "\n---\n"
-        Globals.OUTPUT += "## :speech_balloon: Output from `clang-tidy`\n"
-        Globals.OUTPUT += Globals.PAYLOAD_TIDY
+    if Globals.FORMAT_COMMENT or Globals.TIDY_COMMENT:
+        Globals.OUTPUT += ":warning:\nSome files did not pass the configured checks!\n"
+        if Globals.FORMAT_COMMENT:
+            Globals.OUTPUT += (
+                "\n<details><summary>clang-format reports: <strong>"
+                + f"{len(GlobalParser.format_advice)} file(s) not formatted</strong>"
+                + f"</summary>\n\n{Globals.FORMAT_COMMENT}\n\n</details>"
+            )
+        if Globals.TIDY_COMMENT:
+            Globals.OUTPUT += (
+                f"\n<details><summary>clang-tidy reports: <strong>{len(tidy_notes)} "
+                + f"concern(s)</strong></summary>\n\n{Globals.TIDY_COMMENT}\n\n"
+                + "</details>"
+            )
+    else:
+        Globals.OUTPUT += ":heavy_check_mark:\nNo problems need attention."
+    Globals.OUTPUT += "\n\nHave any feedback or feature suggestions? [Share it here.]"
+    Globals.OUTPUT += "(https://github.com/cpp-linter/cpp-linter-action/issues)"
+
     GlobalParser.tidy_notes = tidy_notes[:]  # restore cache of notifications
 
 
 def post_push_comment(base_url: str, user_id: int) -> bool:
     """POST action's results for a push event.
 
     :param base_url: The root of the url used to interact with the REST API via
@@ -810,14 +817,17 @@
     thread_comments_allowed = True
     if GITHUB_EVENT_PATH and "private" in Globals.EVENT_PAYLOAD["repository"]:
         thread_comments_allowed = (
             Globals.EVENT_PAYLOAD["repository"]["private"] is not True
         )
     if args.thread_comments and thread_comments_allowed:
         post_results(False)  # False is hard-coded to disable diff comments.
+    if args.step_summary and "GITHUB_STEP_SUMMARY" in os.environ:
+        with open(os.environ["GITHUB_STEP_SUMMARY"], "a", encoding="utf-8") as summary:
+            summary.write(f"\n{Globals.OUTPUT}\n")
     set_exit_code(
         int(
             make_annotations(args.style, args.file_annotations, args.lines_changed_only)
         )
     )
     end_log_group()
```

## cpp_linter/thread_comments.py

```diff
@@ -101,21 +101,21 @@
             if not is_multiline_fix and diag.replacements:
                 # complete suggestion with original src code and closing md fence
                 last_fix = diag.replacements[len(diag.replacements) - 1]
                 suggestion += line[last_fix.cols + last_fix.null_len - 1 : -1] + "\n```"
                 body += suggestion
 
             results.append(
-                dict(
-                    body=body,
-                    commit_id=GITHUB_SHA,
-                    line=diag.line,
-                    path=fixit.filename,
-                    side="RIGHT",
-                )
+                {
+                    "body": body,
+                    "commit_id": GITHUB_SHA,
+                    "line": diag.line,
+                    "path": fixit.filename,
+                    "side": "RIGHT",
+                }
             )
     return results
 
 
 def aggregate_format_advice(lines_changed_only: int) -> List[Dict[str, Any]]:
     """Aggregate a list of json contents representing advice from clang-format
     suggestions.
@@ -158,21 +158,21 @@
             # complete suggestion with original src code and closing md fence
             last_fix = fixed_line.replacements[-1]
             body += line[last_fix.cols + last_fix.null_len - 1 : -1] + "\n```"
             # logger.debug("body <<< %s", body)
 
             # create a suggestion from clang-format advice
             results.append(
-                dict(
-                    body=body,
-                    commit_id=GITHUB_SHA,
-                    line=fixed_line.line,
-                    path=fmt_advice.filename,
-                    side="RIGHT",
-                )
+                {
+                    "body": body,
+                    "commit_id": GITHUB_SHA,
+                    "line": fixed_line.line,
+                    "path": fmt_advice.filename,
+                    "side": "RIGHT",
+                }
             )
     return results
 
 
 def concatenate_comments(
     tidy_advice: list, format_advice: list
 ) -> List[Dict[str, Union[str, int]]]:
```

## Comparing `cpp_linter-1.5.1.dist-info/LICENSE` & `cpp_linter-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpp_linter-1.5.1.dist-info/METADATA` & `cpp_linter-1.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-linter
-Version: 1.5.1
+Version: 1.6.0
 Summary: Run clang-format and clang-tidy on a batch of files.
 Author-email: Brendan Doherty <2bndy5@gmail.com>, Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/cpp-linter/cpp-linter
 Project-URL: tracker, https://github.com/cpp-linter/cpp-linter/issues
 Keywords: clang,clang-tools,linter,clang-tidy,clang-format
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `cpp_linter-1.5.1.dist-info/RECORD` & `cpp_linter-1.6.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-cpp_linter/__init__.py,sha256=f4HCHmkFpTkj7ZaMnzy1PRbVRr0P3hU9OKX-LwuqxHQ,6817
+cpp_linter/__init__.py,sha256=Vyz8LxCP4CSyoMEDT1o903J4Cm7Yh6uXIuPHSyoTMm8,6894
 cpp_linter/clang_format_xml.py,sha256=F_mECZgDceTQfgD3x-bPhPx58wU2oJEcp-dfmNyGUss,5449
-cpp_linter/clang_tidy.py,sha256=_SN81xXLDp6kH8l2SE6a_i-XUY1vuasTTspF6TmlNYc,4532
+cpp_linter/clang_tidy.py,sha256=8DEUdMNfDbhhMfT9I4RFfpbcA-KE2I0YWPC75pZhyKA,4399
 cpp_linter/clang_tidy_yml.py,sha256=fAcF8zV4RiBY-bkW3SFy4c4HR6h2mlf46DmzPfdxQ30,4743
-cpp_linter/cli.py,sha256=t-l9voOTqssUrIh3Y5qcRdKD61Jx2on-UQvrBUVDw7g,7351
-cpp_linter/git.py,sha256=aI5wTDrgmyK6nwihULt6taQ9mRPrm4yz7PnHQIb6fIk,6376
-cpp_linter/run.py,sha256=n-fjEdivfP11j8rNE6LD7HVVQubL0guzI2ZkFW5EkIA,31089
-cpp_linter/thread_comments.py,sha256=kvFWj0-b0ODVahnnOMSOGV-CzhXX7EaIgECDG-USNwU,10849
-cpp_linter-1.5.1.dist-info/LICENSE,sha256=jQ9ovcGO-7MCWam1lJKfGtUY7nKa7nEc9aIGN7wk6Lw,1067
-cpp_linter-1.5.1.dist-info/METADATA,sha256=56n7TCRKGgMDXOBqOYj9vhIL97fackryzDUTqXvT3E8,2811
-cpp_linter-1.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cpp_linter-1.5.1.dist-info/entry_points.txt,sha256=qO6GQsENVyy7-eQ-FfAju-q2SeaNVEBa_Ij4nJdgNJQ,51
-cpp_linter-1.5.1.dist-info/top_level.txt,sha256=9revY4HSck6TvN-QcFh8296Gffnp80dHARWnRzUHmVE,11
-cpp_linter-1.5.1.dist-info/RECORD,,
+cpp_linter/cli.py,sha256=HX_4ImPaPd-Z0m4EuPwRDSwFfXPPSqD6K-C0ssvdA9Q,7646
+cpp_linter/git.py,sha256=Z9-Wsqdd6EHhOf61DGBtJIqkFhgmr34WaTQRYIz13Lc,6377
+cpp_linter/run.py,sha256=SHat2dnTllR-Y1akxgbz3OD4LmSlXGYafyWnlXLkDRM,31645
+cpp_linter/thread_comments.py,sha256=Z0NIDlfR22KNwmiZyUcA3D-5eSTU9KMxUd8Voj0Yw5M,10871
+cpp_linter-1.6.0.dist-info/LICENSE,sha256=jQ9ovcGO-7MCWam1lJKfGtUY7nKa7nEc9aIGN7wk6Lw,1067
+cpp_linter-1.6.0.dist-info/METADATA,sha256=sqETU7ErGXjjDk1GMR2pogNdwUE0-8KzxXajfyYYBDA,2811
+cpp_linter-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cpp_linter-1.6.0.dist-info/entry_points.txt,sha256=qO6GQsENVyy7-eQ-FfAju-q2SeaNVEBa_Ij4nJdgNJQ,51
+cpp_linter-1.6.0.dist-info/top_level.txt,sha256=9revY4HSck6TvN-QcFh8296Gffnp80dHARWnRzUHmVE,11
+cpp_linter-1.6.0.dist-info/RECORD,,
```

