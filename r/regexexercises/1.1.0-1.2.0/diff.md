# Comparing `tmp/regexexercises-1.1.0.tar.gz` & `tmp/regexexercises-1.2.0.tar.gz`

## Comparing `regexexercises-1.1.0.tar` & `regexexercises-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/__init__.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/app_guide.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/pyregex_exercises.css
--rw-r--r--   0        0        0    13324 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/pyregex_exercises.py
--rw-r--r--   0        0        0    60241 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/questions.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 regexexercises-1.1.0/src/regexexercises/user_progress.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 regexexercises-1.1.0/LICENSE
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 regexexercises-1.1.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 regexexercises-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 regexexercises-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/__init__.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/app_guide.md
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/pyregex_exercises.css
+-rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/pyregex_exercises.py
+-rw-r--r--   0        0        0    60241 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/questions.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 regexexercises-1.2.0/src/regexexercises/user_progress.json
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 regexexercises-1.2.0/LICENSE
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 regexexercises-1.2.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 regexexercises-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 regexexercises-1.2.0/PKG-INFO
```

### Comparing `regexexercises-1.1.0/src/regexexercises/app_guide.md` & `regexexercises-1.2.0/src/regexexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `regexexercises-1.1.0/src/regexexercises/pyregex_exercises.css` & `regexexercises-1.2.0/src/regexexercises/pyregex_exercises.css`

 * *Files 26% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     border: none;
     background: silver;
 }
 
 .radio {
     layout: horizontal;
     border: none;
-    width: 50%;
+    width: 1fr;
     margin: 0 2 0 2;
 }
 
 #question {
     width: 100%;
     margin: 0 1 1 1;
 }
 
 #solution {
     width: 100%;
-    margin: 0 1 1 1;
+    padding: 0 1 0 1;
+    border: round gray;
+    border-title-align: center;
 }
 
 #columns {
     height: auto;
     align: center middle;
     border: solid brown;
 }
@@ -47,27 +49,29 @@
     border-top: solid gray;
     padding: 0 1 0 1;
 }
 
 .list {
     height: auto;
     margin: 0 1 0 1;
-    width: 50%;
+    width: 1fr;
     color: black;
 }
 
 .error {
     min-height: 0;
     height: auto;
     width: 100%;
     color: red;
+    padding: 0 1 0 1;
+    border: round red;
 }
 
 Button:focus {
     text-style: bold;
 }
 
 .buttons {
     max-height: 1;
     border: none;
-    width: 50%;
+    width: 1fr;
 }
```

### Comparing `regexexercises-1.1.0/src/regexexercises/pyregex_exercises.py` & `regexexercises-1.2.0/src/regexexercises/pyregex_exercises.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from textual.app import App
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical, VerticalScroll
 from textual.widgets import Footer, Label, Input, MarkdownViewer, Button
 from textual.widgets import RadioButton, RadioSet, ContentSwitcher
-from rich.panel import Panel
 from rich.markdown import Markdown
 
 import json
 import re
 import regex
 import os
 from pathlib import Path
@@ -46,22 +45,23 @@
                     break
             self.q_idx = idx
 
         self.l_question = Label('', id='question')
         placeholder = 'Add your solution here. Use ip to represent the input.'
         self.i_user_code = Input(placeholder=placeholder, id='input')
         self.v_code = Vertical(self.l_question, self.i_user_code, id='code')
-        self.l_code_error = Label('')
+        self.l_code_error = Label()
 
         self.v_left_col = Vertical(classes='list')
         self.v_right_col = Vertical(classes='list')
         self.h_columns = Horizontal(self.v_left_col, self.v_right_col,
                                     id='columns')
 
-        self.l_ref_solution = Label('', id='solution')
+        self.l_ref_solution = Label(id='solution', markup=False)
+        self.l_ref_solution.border_title = 'Reference Solution'
 
         self.error_types = (SyntaxError, TypeError, ValueError,
                             NameError, AttributeError, IndexError,
                             re.error, regex._regex_core.error)
         self.input_bg_color = 'gray'
         self.input_error_color = 'ansi_red'
         self.item_color = 'gray'
@@ -119,15 +119,15 @@
         self.cs_tabs.current = name
 
     def on_input_submitted(self, event):
         self.process_user_code()
         self.save_progress()
 
     def process_user_code(self):
-        self.l_ref_solution.update('')
+        self.l_ref_solution_clear()
         self.solved = self.eval_func[self.func_search]()
         if self.solved:
             self.i_user_code.styles.background = self.item_solved_color
             self.show_solution()
 
     def search(self):
         self.l_code_error.remove()
@@ -145,16 +145,16 @@
                 ip = self.right_col[idx]
                 if not eval(self.i_user_code.value):
                     label.styles.color = self.item_solved_color
                 else:
                     label.styles.color = self.item_failed_color
                     solved = False
         except self.error_types as e:
-            t = Panel(f'{e}', title=f'{type(e).__name__}', title_align='left')
-            self.l_code_error = Label(t, classes='error')
+            self.l_code_error = Label(str(e), classes='error', markup=False)
+            self.l_code_error.border_title = str(type(e).__name__)
             self.v_code.mount(self.l_code_error)
             self.i_user_code.styles.background = self.input_error_color
             solved = False
         return solved
 
     def ip_op(self):
         self.l_code_error.remove()
@@ -177,24 +177,24 @@
                     solved = False
                     if self.debug_on:
                         self.l_right_col[idx].update(f(op))
                         self.l_right_col[idx].styles.color = self.debug_color
                     else:
                         self.l_right_col[idx].update(f(self.right_col[idx]))
         except self.error_types as e:
-            t = Panel(f'{e}', title=f'{type(e).__name__}', title_align='left')
-            self.l_code_error = Label(t, classes='error')
+            self.l_code_error = Label(str(e), classes='error', markup=False)
+            self.l_code_error.border_title = str(type(e).__name__)
             self.v_code.mount(self.l_code_error)
             self.i_user_code.styles.background = self.input_error_color
             solved = False
         return solved
 
     def set_question(self):
         self.v_exercises.scroll_home(animate=False)
-        self.l_ref_solution.update('')
+        self.l_ref_solution_clear()
 
         self.l_code_error.remove()
         self.v_left_col.remove()
         self.v_right_col.remove()
         self.v_left_col = Vertical(classes='list')
         self.v_right_col = Vertical(classes='list')
         self.h_columns.mount(self.v_left_col)
@@ -272,17 +272,21 @@
             self.set_question()
 
     def action_next(self):
         if self.q_idx < self.q_max_idx:
             self.q_idx += 1
             self.set_question()
 
+    def l_ref_solution_clear(self):
+        self.l_ref_solution.update('')
+        self.l_ref_solution.styles.border = ('none', 'gray')
+
     def show_solution(self):
-        self.l_ref_solution.update(
-            Panel(self.ref_solution, title='Reference Solution'))
+        self.l_ref_solution.update(self.ref_solution)
+        self.l_ref_solution.styles.border = ('round', 'gray')
 
     def action_solution(self):
         self.show_solution()
         self.v_exercises.scroll_end(animate=False)
 
     def left_fmt_func(self):
         f = self.fmt_func[self.fmt_idx]
```

### Comparing `regexexercises-1.1.0/src/regexexercises/questions.json` & `regexexercises-1.2.0/src/regexexercises/questions.json`

 * *Files identical despite different names*

### Comparing `regexexercises-1.1.0/LICENSE` & `regexexercises-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regexexercises-1.1.0/README.md` & `regexexercises-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `regexexercises-1.1.0/pyproject.toml` & `regexexercises-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "regexexercises"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "100+ exercises for Python Regular Expressions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.16.0",
+  "textual>=0.24.1",
   "regex",
 ]
 
 [project.scripts]
 regexexercises = "regexexercises.pyregex_exercises:main"
 
 [project.urls]
```

### Comparing `regexexercises-1.1.0/PKG-INFO` & `regexexercises-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: regexexercises
-Version: 1.1.0
+Version: 1.2.0
 Summary: 100+ exercises for Python Regular Expressions
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/PyRegexExercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: regex
-Requires-Dist: textual>=0.16.0
+Requires-Dist: textual>=0.24.1
 Description-Content-Type: text/markdown
 
 # Python re(gex)? exercises
 
 This TUI application is intended to help you practice Python regular expressions. There are more than 100 exercises covering both the builtin `re` and third-party `regex` module.
 
 # Screenshot
```

