# Comparing `tmp/trogon-0.1.0.tar.gz` & `tmp/trogon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trogon-0.1.0.tar", max compression
+gzip compressed data, was "trogon-0.2.0.tar", max compression
```

## Comparing `trogon-0.1.0.tar` & `trogon-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      357 2023-05-19 18:24:38.897137 trogon-0.1.0/README.md
--rw-r--r--   0        0        0      526 2023-05-19 18:26:55.912319 trogon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-19 18:26:14.348738 trogon-0.1.0/trogon/__init__.py
--rw-r--r--   0        0        0      123 2023-05-18 13:56:09.446634 trogon-0.1.0/trogon/constants.py
--rw-r--r--   0        0        0     6304 2023-05-18 09:14:44.794229 trogon-0.1.0/trogon/introspect.py
--rw-r--r--   0        0        0    11418 2023-05-19 18:25:37.160154 trogon-0.1.0/trogon/run_command.py
--rw-r--r--   0        0        0    10565 2023-05-19 18:26:23.108159 trogon-0.1.0/trogon/trogon.py
--rw-r--r--   0        0        0     3478 2023-05-19 17:39:52.761095 trogon-0.1.0/trogon/trogon.scss
--rw-r--r--   0        0        0        0 2023-05-18 09:14:44.794618 trogon-0.1.0/trogon/widgets/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-18 13:56:58.104458 trogon-0.1.0/trogon/widgets/about.py
--rw-r--r--   0        0        0     3874 2023-05-19 18:25:37.005493 trogon-0.1.0/trogon/widgets/command_info.py
--rw-r--r--   0        0        0     1985 2023-05-19 18:25:37.089993 trogon-0.1.0/trogon/widgets/command_tree.py
--rw-r--r--   0        0        0     7846 2023-05-19 18:25:37.146181 trogon-0.1.0/trogon/widgets/form.py
--rw-r--r--   0        0        0     2861 2023-05-18 09:14:44.794969 trogon-0.1.0/trogon/widgets/multiple_choice.py
--rw-r--r--   0        0        0    14891 2023-05-19 18:25:36.988309 trogon-0.1.0/trogon/widgets/parameter_controls.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 trogon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3537 2023-05-20 16:10:57.055318 trogon-0.2.0/README.md
+-rw-r--r--   0        0        0     1379 2023-05-20 16:10:57.062741 trogon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.2.0/trogon/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.2.0/trogon/constants.py
+-rw-r--r--   0        0        0     6304 2023-05-20 10:29:22.256860 trogon-0.2.0/trogon/introspect.py
+-rw-r--r--   0        0        0    11626 2023-05-20 10:29:22.257195 trogon-0.2.0/trogon/run_command.py
+-rw-r--r--   0        0        0    10558 2023-05-20 10:29:22.257466 trogon-0.2.0/trogon/trogon.py
+-rw-r--r--   0        0        0     3476 2023-05-20 10:29:22.257670 trogon-0.2.0/trogon/trogon.scss
+-rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.2.0/trogon/widgets/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.2.0/trogon/widgets/about.py
+-rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.2.0/trogon/widgets/command_info.py
+-rw-r--r--   0        0        0     1985 2023-05-20 10:29:22.258561 trogon-0.2.0/trogon/widgets/command_tree.py
+-rw-r--r--   0        0        0     7846 2023-05-20 10:29:22.258801 trogon-0.2.0/trogon/widgets/form.py
+-rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.2.0/trogon/widgets/multiple_choice.py
+-rw-r--r--   0        0        0    14891 2023-05-20 10:29:22.259311 trogon-0.2.0/trogon/widgets/parameter_controls.py
+-rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 trogon-0.2.0/PKG-INFO
```

### Comparing `trogon-0.1.0/trogon/introspect.py` & `trogon-0.2.0/trogon/introspect.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/run_command.py` & `trogon-0.2.0/trogon/run_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,19 @@
                             # `--foo bar`.
                             args.append(option_name)
                             for subvalue_tuple in value_data:
                                 args.extend(subvalue_tuple)
                         else:
                             # Get the value of the counting option
                             count = next(itertools.chain.from_iterable(value_data), 1)
-                            count = int(count)
+                            try:
+                                count = int(count)
+                            except ValueError:
+                                # TODO: Not sure if this is the right thing to do
+                                count = 1
                             if option_name.startswith("--"):
                                 args.extend([option_name] * count)
                             else:
                                 clean_option_name = option_name.lstrip("-")
                                 args.append(f"-{clean_option_name * count}")
 
         for option_name, values in multiples.items():
```

### Comparing `trogon-0.1.0/trogon/trogon.py` & `trogon-0.2.0/trogon/trogon.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         )
         await parent.mount(command_form)
         if not self.is_grouped_cli:
             command_form.focus()
 
 
 class Trogon(App):
-    CSS_PATH = Path(__file__).parent / "textual_click.scss"
+    CSS_PATH = Path(__file__).parent / "trogon.scss"
 
     def __init__(
         self,
         cli: click.Group,
         app_name: str = None,
         click_context: click.Context = None,
     ) -> None:
```

### Comparing `trogon-0.1.0/trogon/trogon.scss` & `trogon-0.2.0/trogon/trogon.scss`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
   padding: 0 1;
   margin-bottom: 1;  /* why is this needed? */
   border: blank;
 }
 
 
 CommandTree:focus {
-  border: tall $secondary;
+  border: tall $success;
 }
 
 CommandTree > .tree--cursor {
   background: $primary-darken-1;
 }
 
 CommandTree:focus > .tree--cursor {
@@ -173,15 +173,15 @@
 }
 
 CommandInfo {
   align: center middle;
 }
 
 .command-info-header-text {
-  padding: 1 2 0 2;
+  padding: 1 1 0 2;
 }
 
 $command-info-header-bg: $primary-darken-1;
 
 .command-info-header {
   dock: top;
   background: $command-info-header-bg;
```

### Comparing `trogon-0.1.0/trogon/widgets/about.py` & `trogon-0.2.0/trogon/widgets/about.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/widgets/command_info.py` & `trogon-0.2.0/trogon/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/widgets/command_tree.py` & `trogon-0.2.0/trogon/widgets/command_tree.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/widgets/form.py` & `trogon-0.2.0/trogon/widgets/form.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/widgets/multiple_choice.py` & `trogon-0.2.0/trogon/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `trogon-0.1.0/trogon/widgets/parameter_controls.py` & `trogon-0.2.0/trogon/widgets/parameter_controls.py`

 * *Files identical despite different names*

