# Comparing `tmp/PySimpleInput-0.0.4.post1.tar.gz` & `tmp/PySimpleInput-0.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySimpleInput-0.0.4.post1.tar", last modified: Tue Dec 13 05:13:05 2022, max compression
+gzip compressed data, was "PySimpleInput-0.0.5.post1.tar", last modified: Sat May 20 05:24:30 2023, max compression
```

## Comparing `PySimpleInput-0.0.4.post1.tar` & `PySimpleInput-0.0.5.post1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwx------   0 u0_a524  (10524) u0_a524  (10524)        0 2022-12-13 05:13:05.892829 PySimpleInput-0.0.4.post1/
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     1066 2022-11-27 15:26:28.000000 PySimpleInput-0.0.4.post1/LICENSE
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     7161 2022-12-13 05:13:05.892829 PySimpleInput-0.0.4.post1/PKG-INFO
-drwx------   0 u0_a524  (10524) u0_a524  (10524)        0 2022-12-13 05:13:05.892829 PySimpleInput-0.0.4.post1/PySimpleInput/
--rw-------   0 u0_a524  (10524) u0_a524  (10524)       52 2022-12-01 16:20:45.000000 PySimpleInput-0.0.4.post1/PySimpleInput/__init__.py
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     6038 2022-12-13 05:01:03.000000 PySimpleInput-0.0.4.post1/PySimpleInput/inputter.py
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     4979 2022-12-02 12:46:41.000000 PySimpleInput-0.0.4.post1/PySimpleInput/inputter_old.py
--rw-------   0 u0_a524  (10524) u0_a524  (10524)       62 2022-12-01 08:35:12.000000 PySimpleInput-0.0.4.post1/PySimpleInput/wiki.py
-drwx------   0 u0_a524  (10524) u0_a524  (10524)        0 2022-12-13 05:13:05.892829 PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     7161 2022-12-13 05:13:05.000000 PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/PKG-INFO
--rw-------   0 u0_a524  (10524) u0_a524  (10524)      293 2022-12-13 05:13:05.000000 PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/SOURCES.txt
--rw-------   0 u0_a524  (10524) u0_a524  (10524)        1 2022-12-13 05:13:05.000000 PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/dependency_links.txt
--rw-------   0 u0_a524  (10524) u0_a524  (10524)       14 2022-12-13 05:13:05.000000 PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/top_level.txt
--rw-------   0 u0_a524  (10524) u0_a524  (10524)     6486 2022-12-13 05:09:40.000000 PySimpleInput-0.0.4.post1/README.md
--rw-------   0 u0_a524  (10524) u0_a524  (10524)      627 2022-12-13 05:12:35.000000 PySimpleInput-0.0.4.post1/pyproject.toml
--rw-------   0 u0_a524  (10524) u0_a524  (10524)       38 2022-12-13 05:13:05.892829 PySimpleInput-0.0.4.post1/setup.cfg
--rw-------   0 u0_a524  (10524) u0_a524  (10524)      909 2022-12-13 05:12:43.000000 PySimpleInput-0.0.4.post1/setup.py
+drwxrwxr-x   0 turtleion  (1000) turtleion  (1000)        0 2023-05-20 05:24:30.425293 PySimpleInput-0.0.5.post1/
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)     1066 2023-05-19 00:42:34.000000 PySimpleInput-0.0.5.post1/LICENSE
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)     5404 2023-05-20 05:24:30.425293 PySimpleInput-0.0.5.post1/PKG-INFO
+drwxrwxr-x   0 turtleion  (1000) turtleion  (1000)        0 2023-05-20 05:24:30.425293 PySimpleInput-0.0.5.post1/PySimpleInput/
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)       24 2023-05-20 04:01:38.000000 PySimpleInput-0.0.5.post1/PySimpleInput/__init__.py
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)     2466 2023-05-20 05:20:12.000000 PySimpleInput-0.0.5.post1/PySimpleInput/inputter.py
+drwxrwxr-x   0 turtleion  (1000) turtleion  (1000)        0 2023-05-20 05:24:30.425293 PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)     5404 2023-05-20 05:24:30.000000 PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/PKG-INFO
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)      241 2023-05-20 05:24:30.000000 PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/SOURCES.txt
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)        1 2023-05-20 05:24:30.000000 PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/dependency_links.txt
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)       14 2023-05-20 05:24:30.000000 PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/top_level.txt
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)     4779 2023-05-20 05:24:08.000000 PySimpleInput-0.0.5.post1/README.md
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)      589 2023-05-20 05:24:19.000000 PySimpleInput-0.0.5.post1/pyproject.toml
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)       38 2023-05-20 05:24:30.429293 PySimpleInput-0.0.5.post1/setup.cfg
+-rw-rw-r--   0 turtleion  (1000) turtleion  (1000)      860 2023-05-20 05:24:11.000000 PySimpleInput-0.0.5.post1/setup.py
```

### Comparing `PySimpleInput-0.0.4.post1/LICENSE` & `PySimpleInput-0.0.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySimpleInput-0.0.4.post1/PKG-INFO` & `PySimpleInput-0.0.5.post1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,117 @@
 Metadata-Version: 2.1
 Name: PySimpleInput
-Version: 0.0.4.post1
-Summary: Package that help you to fix general python input() problems
+Version: 0.0.5.post1
+Summary: Advanced Input System
 Home-page: https://github.com/turtleion/PySimpleInput
 Author: Turtleion
 Author-email: Turtleion <remastred89@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/turtleion/PySimpleInput
 Project-URL: Bug Tracker, https://github.com/turtleion/PySimpleInput/issues
-Keywords: Simple ways to use Input
+Keywords: Python3 Input
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PySimpleInput | v0.0.4
+# PySimpleInput | v0.0.5 Rev. 1
 
-Hi! Let me introduce *PySimpleInput* Library.
-
-This library help you to fix problems with Python Input Built-in Function.
+Hi! Let me introduce *PySimpleInput*
 
 This library still on development progress.
     if you found a bugs, report it to me at [PySimpleInput Github Issues](https://github.com/turtleion/PySimpleInput/issues) 
     
 # Installation
-You can install PySimpleInput with pip or using .whl or manually with .tar.gz
+You can install PySimpleInput with pip or using .whl
 ### Using PIP
 `pip3 install --upgrade PySimpleInput`
 ### Using wheel
 - First, you need to get the wheel file from PyPi or Github
 - And, you can install it
 `pip3 install (PySimpleInput Wheel File).whl`
-### Using .tar.gz
-- Same as using wheel, you need to get the .tar.gz file from PyPi or Github
-- Extract the .tar.gz file using `tar -xvf (PySimpleInput TAR GZ File).tar.gz`
-- Cd into PySimpleInput directory : `cd PySimpleInput-(VERSION)/`
-- Then you can install it : `python3 setup.py install`
-
 
 # Docs
-*if you want the latest update, choose the devel branch, if you want stable then choose main branch, if you want to try the newest and earlier features choose testing branch*
-
-First of all we need to know all class in PySimpleInput modules
+*if you want the latest update, choose the devel branch, if you want stable then choose main branch*
 
-- PySimpleInput -> PySimpleInput (PySimpleInput.PySimpleInput)
-                    Modern PySimpleInput, got more updates, more bugs have been fixed than the previous version
-## How to Initialize PySimpleInput modules in a new ways
+## How to Initialize PySimpleInput modules
 ```
 import PySimpleInput
 
 pysim = PySimpleInput.PySimpleInput()
 ```
 
-*The difference between new PySimpleInput and old PySimpleInput is in the changelog*
+
 ### Method 
 - input()  
   - label: Give a question to the user
   - options: set additional settings to the input
-  - extra_options: extra arguments for the input options
 
 #### ARGUMENTS on the input method
-LABEL (REQUIRED) : This argument will ask questions to the user, without this argument the user will not be able to answer
+LABEL (REQUIRED) : This argument will ask questions to the user
 
 OPTIONS (OPTIONAL) : this argument provides additional settings to the input 
                        `ex. filtering user input to return only numbers`
 
-EXTRA_OPTIONS (OPTIONAL/SOMETIMES REQUIRED) : Either option requires additional arguments for it to work properly
 
 ### OPTIONS on the input method
 
 this section contains all options available in PySimpleInput (Modern)
 
-- remove_whitespace : this option will remove all white space in user input string
-
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["remove_whitespace"])`
+- rmwhtspc_* : this option will remove all white space in user input string
+    - rmwhtspc_arr : Will return array/list instead of str
+        > ex. `o = pysimpleinput.input("What's your name?", ["rmwhtspc_arr"])
 
-    > Result. `"Joseph Madriguo Terafora" -> "JosephMadrigioTerafora"`
+        > Result. `"Joseph Arauro" > "["Joseph", "Arauro"]"`
 
-- prevent_enterkeypress : this option will prevent the user from pressing the enter key
+    - rmwhtspc_str : Will return str
+        > ex. `o = pysimpleinput.input("What is your name?", ["rmwhtspc_str"])`
 
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["prevent_enterkeypress"])`
+        > Result. `"Joseph Arauro" -> "JosephArauro"`
 
-- convert_datatype : this option will change the user input data type from string to ... (str, int, float)
-
-    > ex. `pysimOut = pysimpleinput.input("How old are you?", options=["filter_num", "convert_datatype"], options_arg={"convert_datatype": "(int, float, str)"})`
-
-    > Result. --> `"29 (STR)" -> 29 (Int)`
 
 - filter_num : this option will filter user input to return only numbers
 
-    > ex. `pysimOut = pysimpleinput.input("How old are you?", options=["filter_num"])`
+    > ex. `pysimOut = pysimpleinput.input("How old are you?", ["filternum"])`
 
     > Result. --> `"oejnzo299kwjo02" -> "29902"`
 
-- to_upper and to_lower : This option will change the user input letters to uppercase or vice versa
+- filteralph : This option will filter user input to return alphabet characters only
 
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["to_upper/to_lower"])`
-
-    > Result. --> `"gerardo martinuez firatzi" <(OR)> "GERARDO MARTINUEZ FIRATZI"`
+    > ex. `pysimOut = pysimpleinput.input("Type random string!", ["filteralph"])`
 
-- yesno_prompt : This option will make the question yes or no (All OS is now supported) (EXPERIMENTAL)
-    > NO EXAMPLES
+    > Result. --> `"hello219282839my282872name283739191is8287399turtleion" -> "hellomynameisturtleion"`
 
-- redirect_output : this option will write the output to a file (EXPERIMENTAL)
-    > NO EXAMPLES
+- upcase and lowcase : This option will change the user input letters to uppercase or vice versa
 
-- filter_alpha : This option will filter user input to return alphabet characters only
+    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["upcase/lowcase"])`
 
-    > ex. `pysimOut = pysimpleinput.input("Type random string!", options=["filter_alpha"])`
+    > Result. --> `"gerardo martinuez firatzi" <(OR)> "GERARDO MARTINUEZ FIRATZI"`
 
-    > Result. --> `"hello219282839my282872name283739191is8287399turtleion" -> "hellomynameisturtleion"`
 
-- validate_email : This option will validate an email from the user
+- valemail : This option will validate an email from the user
 
-    > ex. `pysimOut = pysimpleinput.input("Type an email!",options=["validate_email"]
+    > ex. `pysimOut = pysimpleinput.input("Type an email!",["valemail"])
 
-    > Result. --> True | False (If the string is an email it will return True otherwise False
+    > Result. --> `True | False (If the string is an email it will return True otherwise False)`
 
 - validate_phonenumber : This option will validate an phone number from the user
 
-    > ex. `pysimOut = pysimpleinput.input("Type your phone numbers!",options=["validate_phonenumber"]
-
-    > Result. --> PhoneNumber | Warning (If the string is a valid number it will return the number back otherwise an warnimg
+    > ex. `pysimOut = pysimpleinput.input("Type your phone numbers!", ["valphnum])
 
-- validate_url : This option will validate an URL from the user
+    > Result. --> `PhoneNumber | Warning (If the string is a valid number it will return the number back otherwise a warning`
 
-    > ex. `pysimOut = pysimpleinput.input("Show me Famous Artist in YouTube!", options=["validate_url"])
 
-    > Result. --> True | False (If the string is a valid url, it will eeturn True otherwise False
-
-### And Also, You can combine options
-like this
-`pysim = pysimpleinput.input("What is your name?", options=["remove_whitespace","prevent_enterkeypress")`
-
-Do not combine "validate" options!
+### And Also, You can combine options like this
+`pysim = pysimpleinput.input("What is your name?", ["rmwhtspc_str","filteralph")`
 
+Do not combine "valemail, valphnum" options!
+and also if you use "rmwhtspc_arr" options.. you will cannot use "valemail, valphnum, filteralph, filternum" options!
 --------------
 
 # Contribution
 I Appreciate you for contributing on this modules
 ### How To Contribute
 You can Contribute by forking this repo and start adding more features, optimizing code and fixing bugs
 Then you can make a pull request to this repo and wait your pull request merged
@@ -172,21 +143,27 @@
 - Changed the contents of README.md to make it easier to understand
 - Added More Features:
     - "validate_email",
     - "validate_phonenumber"
     - "validate_url"
 - Recombining modern & old PySimpleInput
 - Create Makefile to simplify the development process
+--------
 
-# You need to READ this
-I'm not recommended you to download PySimpleInput below this version (0.0.3.1)
-
-And I will focus to fixing bugs over adding features
+--> Changelog | 0.0.5
+- Changed the contents of README.md
+- Less features to make it lightweighter and simplier
+  - Removed features
+    - Filter URL
+    - Redirect output to a file
+    - Prevent User KEY_ENTER press
+- Renamed features
+- Removed some files
 
 # About
 This project was made 100% by Me (Turtleion) 
 This project was licensed by MIT License
 Visit my GitHub
 https://github.com/turtleion
 
 
-*Sorry for bad English, I"am Indonesian. so it's normal for me*
+*Sorry for bad English, I"am Indonesian.*
```

### Comparing `PySimpleInput-0.0.4.post1/PySimpleInput.egg-info/PKG-INFO` & `PySimpleInput-0.0.5.post1/PySimpleInput.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,117 @@
 Metadata-Version: 2.1
 Name: PySimpleInput
-Version: 0.0.4.post1
-Summary: Package that help you to fix general python input() problems
+Version: 0.0.5.post1
+Summary: Advanced Input System
 Home-page: https://github.com/turtleion/PySimpleInput
 Author: Turtleion
 Author-email: Turtleion <remastred89@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/turtleion/PySimpleInput
 Project-URL: Bug Tracker, https://github.com/turtleion/PySimpleInput/issues
-Keywords: Simple ways to use Input
+Keywords: Python3 Input
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PySimpleInput | v0.0.4
+# PySimpleInput | v0.0.5 Rev. 1
 
-Hi! Let me introduce *PySimpleInput* Library.
-
-This library help you to fix problems with Python Input Built-in Function.
+Hi! Let me introduce *PySimpleInput*
 
 This library still on development progress.
     if you found a bugs, report it to me at [PySimpleInput Github Issues](https://github.com/turtleion/PySimpleInput/issues) 
     
 # Installation
-You can install PySimpleInput with pip or using .whl or manually with .tar.gz
+You can install PySimpleInput with pip or using .whl
 ### Using PIP
 `pip3 install --upgrade PySimpleInput`
 ### Using wheel
 - First, you need to get the wheel file from PyPi or Github
 - And, you can install it
 `pip3 install (PySimpleInput Wheel File).whl`
-### Using .tar.gz
-- Same as using wheel, you need to get the .tar.gz file from PyPi or Github
-- Extract the .tar.gz file using `tar -xvf (PySimpleInput TAR GZ File).tar.gz`
-- Cd into PySimpleInput directory : `cd PySimpleInput-(VERSION)/`
-- Then you can install it : `python3 setup.py install`
-
 
 # Docs
-*if you want the latest update, choose the devel branch, if you want stable then choose main branch, if you want to try the newest and earlier features choose testing branch*
-
-First of all we need to know all class in PySimpleInput modules
+*if you want the latest update, choose the devel branch, if you want stable then choose main branch*
 
-- PySimpleInput -> PySimpleInput (PySimpleInput.PySimpleInput)
-                    Modern PySimpleInput, got more updates, more bugs have been fixed than the previous version
-## How to Initialize PySimpleInput modules in a new ways
+## How to Initialize PySimpleInput modules
 ```
 import PySimpleInput
 
 pysim = PySimpleInput.PySimpleInput()
 ```
 
-*The difference between new PySimpleInput and old PySimpleInput is in the changelog*
+
 ### Method 
 - input()  
   - label: Give a question to the user
   - options: set additional settings to the input
-  - extra_options: extra arguments for the input options
 
 #### ARGUMENTS on the input method
-LABEL (REQUIRED) : This argument will ask questions to the user, without this argument the user will not be able to answer
+LABEL (REQUIRED) : This argument will ask questions to the user
 
 OPTIONS (OPTIONAL) : this argument provides additional settings to the input 
                        `ex. filtering user input to return only numbers`
 
-EXTRA_OPTIONS (OPTIONAL/SOMETIMES REQUIRED) : Either option requires additional arguments for it to work properly
 
 ### OPTIONS on the input method
 
 this section contains all options available in PySimpleInput (Modern)
 
-- remove_whitespace : this option will remove all white space in user input string
-
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["remove_whitespace"])`
+- rmwhtspc_* : this option will remove all white space in user input string
+    - rmwhtspc_arr : Will return array/list instead of str
+        > ex. `o = pysimpleinput.input("What's your name?", ["rmwhtspc_arr"])
 
-    > Result. `"Joseph Madriguo Terafora" -> "JosephMadrigioTerafora"`
+        > Result. `"Joseph Arauro" > "["Joseph", "Arauro"]"`
 
-- prevent_enterkeypress : this option will prevent the user from pressing the enter key
+    - rmwhtspc_str : Will return str
+        > ex. `o = pysimpleinput.input("What is your name?", ["rmwhtspc_str"])`
 
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["prevent_enterkeypress"])`
+        > Result. `"Joseph Arauro" -> "JosephArauro"`
 
-- convert_datatype : this option will change the user input data type from string to ... (str, int, float)
-
-    > ex. `pysimOut = pysimpleinput.input("How old are you?", options=["filter_num", "convert_datatype"], options_arg={"convert_datatype": "(int, float, str)"})`
-
-    > Result. --> `"29 (STR)" -> 29 (Int)`
 
 - filter_num : this option will filter user input to return only numbers
 
-    > ex. `pysimOut = pysimpleinput.input("How old are you?", options=["filter_num"])`
+    > ex. `pysimOut = pysimpleinput.input("How old are you?", ["filternum"])`
 
     > Result. --> `"oejnzo299kwjo02" -> "29902"`
 
-- to_upper and to_lower : This option will change the user input letters to uppercase or vice versa
+- filteralph : This option will filter user input to return alphabet characters only
 
-    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["to_upper/to_lower"])`
-
-    > Result. --> `"gerardo martinuez firatzi" <(OR)> "GERARDO MARTINUEZ FIRATZI"`
+    > ex. `pysimOut = pysimpleinput.input("Type random string!", ["filteralph"])`
 
-- yesno_prompt : This option will make the question yes or no (All OS is now supported) (EXPERIMENTAL)
-    > NO EXAMPLES
+    > Result. --> `"hello219282839my282872name283739191is8287399turtleion" -> "hellomynameisturtleion"`
 
-- redirect_output : this option will write the output to a file (EXPERIMENTAL)
-    > NO EXAMPLES
+- upcase and lowcase : This option will change the user input letters to uppercase or vice versa
 
-- filter_alpha : This option will filter user input to return alphabet characters only
+    > ex. `pysimOut = pysimpleinput.input("What is your name?", options=["upcase/lowcase"])`
 
-    > ex. `pysimOut = pysimpleinput.input("Type random string!", options=["filter_alpha"])`
+    > Result. --> `"gerardo martinuez firatzi" <(OR)> "GERARDO MARTINUEZ FIRATZI"`
 
-    > Result. --> `"hello219282839my282872name283739191is8287399turtleion" -> "hellomynameisturtleion"`
 
-- validate_email : This option will validate an email from the user
+- valemail : This option will validate an email from the user
 
-    > ex. `pysimOut = pysimpleinput.input("Type an email!",options=["validate_email"]
+    > ex. `pysimOut = pysimpleinput.input("Type an email!",["valemail"])
 
-    > Result. --> True | False (If the string is an email it will return True otherwise False
+    > Result. --> `True | False (If the string is an email it will return True otherwise False)`
 
 - validate_phonenumber : This option will validate an phone number from the user
 
-    > ex. `pysimOut = pysimpleinput.input("Type your phone numbers!",options=["validate_phonenumber"]
-
-    > Result. --> PhoneNumber | Warning (If the string is a valid number it will return the number back otherwise an warnimg
+    > ex. `pysimOut = pysimpleinput.input("Type your phone numbers!", ["valphnum])
 
-- validate_url : This option will validate an URL from the user
+    > Result. --> `PhoneNumber | Warning (If the string is a valid number it will return the number back otherwise a warning`
 
-    > ex. `pysimOut = pysimpleinput.input("Show me Famous Artist in YouTube!", options=["validate_url"])
 
-    > Result. --> True | False (If the string is a valid url, it will eeturn True otherwise False
-
-### And Also, You can combine options
-like this
-`pysim = pysimpleinput.input("What is your name?", options=["remove_whitespace","prevent_enterkeypress")`
-
-Do not combine "validate" options!
+### And Also, You can combine options like this
+`pysim = pysimpleinput.input("What is your name?", ["rmwhtspc_str","filteralph")`
 
+Do not combine "valemail, valphnum" options!
+and also if you use "rmwhtspc_arr" options.. you will cannot use "valemail, valphnum, filteralph, filternum" options!
 --------------
 
 # Contribution
 I Appreciate you for contributing on this modules
 ### How To Contribute
 You can Contribute by forking this repo and start adding more features, optimizing code and fixing bugs
 Then you can make a pull request to this repo and wait your pull request merged
@@ -172,21 +143,27 @@
 - Changed the contents of README.md to make it easier to understand
 - Added More Features:
     - "validate_email",
     - "validate_phonenumber"
     - "validate_url"
 - Recombining modern & old PySimpleInput
 - Create Makefile to simplify the development process
+--------
 
-# You need to READ this
-I'm not recommended you to download PySimpleInput below this version (0.0.3.1)
-
-And I will focus to fixing bugs over adding features
+--> Changelog | 0.0.5
+- Changed the contents of README.md
+- Less features to make it lightweighter and simplier
+  - Removed features
+    - Filter URL
+    - Redirect output to a file
+    - Prevent User KEY_ENTER press
+- Renamed features
+- Removed some files
 
 # About
 This project was made 100% by Me (Turtleion) 
 This project was licensed by MIT License
 Visit my GitHub
 https://github.com/turtleion
 
 
-*Sorry for bad English, I"am Indonesian. so it's normal for me*
+*Sorry for bad English, I"am Indonesian.*
```

