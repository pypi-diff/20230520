# Comparing `tmp/bosch-control-panel-cc880p-3.0.0.tar.gz` & `tmp/bosch-control-panel-cc880p-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-3.0.0.tar", last modified: Sun May  7 15:18:32 2023, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-3.1.0.tar", last modified: Sat May 20 09:51:26 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-3.0.0.tar` & `bosch-control-panel-cc880p-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21606 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 09:51:26.182753 bosch-control-panel-cc880p-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.174753 bosch-control-panel-cc880p-3.1.0/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.174753 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 09:51:15.000000 bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:51:26.178753 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 09:51:26.000000 bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-3.0.0/LICENSE` & `bosch-control-panel-cc880p-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.0.0/PKG-INFO` & `bosch-control-panel-cc880p-3.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
@@ -186,119 +186,101 @@
 C0 <k1> <k2> <k3> <k4> <k5> <k6> <k7> <area> <nKeys> <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
 1       C0          Hexadecimal representation of the 'Send Key' command
 2-8     k<n>        Each byte is represents the key of the keypad. Can be sent
                         from 1 up to 7 keys in a single command
-                        Note: Because it was not possible to determine the
-                        checksum algorithm, the keys can only be sent one at a
-                        time. Below is the list of the frames corresponding to
-                        all the keys available:
-                            '0': 0C 00 00 00 00 00 00 00 00 01 16
-                            '1': 0C 01 00 00 00 00 00 00 00 01 16
-                            '2': 0C 02 00 00 00 00 00 00 00 01 17
-                            '3': 0C 03 00 00 00 00 00 00 00 01 19
-                            '4': 0C 04 00 00 00 00 00 00 00 01 19
-                            '5': 0C 05 00 00 00 00 00 00 00 01 1B
-                            '6': 0C 06 00 00 00 00 00 00 00 01 1C
-                            '7': 0C 07 00 00 00 00 00 00 00 01 1C
-                            '8': 0C 08 00 00 00 00 00 00 00 01 1D
-                            '9': 0C 09 00 00 00 00 00 00 00 01 1F
-                            '#': 0C 1A 00 00 00 00 00 00 00 01 2F
-                            '*': 0C 1B 00 00 00 00 00 00 00 01 31
 9       area        If the alarm is configured to have multiple areas, then
                         this byte identifies the target area that the key(s)
                         will be sent to. Otherwise set it to '00'.
 10      nKeys       Number of keys being sent in this command
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Siren Command
+###### Set Siren Command (Special Command)
 
 Command used to enable/disable the siren
 
 ```
-'Set Siren On ' Command
-0E 05 00 00 00 00 00 00 00 00 1C
+'Set Siren' Command
 
-'Set Siren Off' Command
-0E 06 00 00 00 00 00 00 00 00 1D
+0E <on> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Sets the siren on or off:
+                      - 0x05 if is to set siren on
+                      - 0x06 if is to set siren off
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Arm Command
+###### Set Arm Command (Special Command)
 
 Command used to arm/disarm the alarm
 
 ```
-'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17
+'Arm/Disarm' Command
 
-'Disarm' Command
-0E 02 00 00 00 00 00 00 00 00 18
+0E <arm> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Arm/Disarm the alarm:
+                      - 0x01 if is to arm the alarm
+                      - 0x02 if is to disarm the alarm
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
+
 ###### Set Output Command
 
 Command used to set (enable/disable) outputs of the control panel.
 
 ```
 'Set Output' Command
 
 0E <on> <out> 00 00 00 00 00 00 00 <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
-1       0E          Hexadecimal representation of special functions
+1       0E          Hexadecimal representation of special commands
 2       on          Special function to be executed:
-                        Set Output On: Set this byte to 03
-                        Set Output Off: Set this byte to 04
+                        Set Output On: Set this byte to 0x03
+                        Set Output Off: Set this byte to 0x04
 3       out         This byte represents the index of the target output.
                       Supports setting the outputs 1-5, which values in this
                       byte are 0-4 respectively.
-                      Here is the list of commands for each single output:
-
-                            '1 On':   0E 03 00 00 00 00 00 00 00 00 1A
-                            '1 Off':  0E 04 00 00 00 00 00 00 00 00 1A
-                            '2 On':   0C 03 01 00 00 00 00 00 00 00 1A
-                            '2 Off':  0C 04 01 00 00 00 00 00 00 00 1A
-                            '3 On':   0C 03 02 00 00 00 00 00 00 00 1B
-                            '3 Off':  0C 04 02 00 00 00 00 00 00 00 1B
-                            '4 On':   0C 03 03 00 00 00 00 00 00 00 1D
-                            '4 Off':  0C 04 03 00 00 00 00 00 00 00 1D
-                            '5 On':   0C 03 04 00 00 00 00 00 00 00 1D
-                            '5 Off':  0C 04 04 00 00 00 00 00 00 00 1D
-4-10    XX          All those bytes should be settled to 00.
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+4-10    XX          All those bytes should be set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Command
 
 Command used to request the overall status of the control panel.
 After sending this command is expected the control panel to answer with the [`Get Status Response`](#get-status-response).
 
 ```
 'Get Status' Command
 
-01 00 00 00 91 30 19 0F 00 00 F1
+01 00 00 00 <c2c1> <c4c3> <c6c5> <c7> 00 00 <crc>
 
 Byte   Identifier   Comments
 ----------------------------
 1       01          Hexadecimal representation of the 'Get Status' command.
-2-10    XX          The meaning of those bytes are unknown, and thus should be
-                        always sent shown above.
-11      F1          Frame Checksum. Since the checksum algorithm is unknown and
-                        this bytes of this command have always the same value,
-                        the checksum value should always be 'F1'
+2-4     XX          This bytes are not used and thus set to 0.
+5-8     c1..c7      Corresponds to the installer code needed to have permissions
+                      to get the alarm status. Each digit occupies a nibble.
+                      Not used digits should be set to 0xF.
+9..10   XX          This bytes are not used and thus set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Response
 
 Response of [`Get Status Command`](#get-status-command). This frame contains all the relevant information about the status of the control panel.
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.0.0 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
@@ -90,58 +90,51 @@
 ##### Frames Below are presented the decoded frames that are used by this
 library so far: ###### Send Keys Command Command used to send keys to the
 control panel simulating the pressing of the keypad keys. ``` 'Send Keys'
 Command C0
    Byte Identifier Comments ---------------------------------------------------
 ---------------------------- 1 C0 Hexadecimal representation of the 'Send Key'
 command 2-8 k Each byte is represents the key of the keypad. Can be sent from 1
-up to 7 keys in a single command Note: Because it was not possible to determine
-the checksum algorithm, the keys can only be sent one at a time. Below is the
-list of the frames corresponding to all the keys available: '0': 0C 00 00 00 00
-00 00 00 00 01 16 '1': 0C 01 00 00 00 00 00 00 00 01 16 '2': 0C 02 00 00 00 00
-00 00 00 01 17 '3': 0C 03 00 00 00 00 00 00 00 01 19 '4': 0C 04 00 00 00 00 00
-00 00 01 19 '5': 0C 05 00 00 00 00 00 00 00 01 1B '6': 0C 06 00 00 00 00 00 00
-00 01 1C '7': 0C 07 00 00 00 00 00 00 00 01 1C '8': 0C 08 00 00 00 00 00 00 00
-01 1D '9': 0C 09 00 00 00 00 00 00 00 01 1F '#': 0C 1A 00 00 00 00 00 00 00 01
-2F '*': 0C 1B 00 00 00 00 00 00 00 01 31 9 area If the alarm is configured to
-have multiple areas, then this byte identifies the target area that the key(s)
-will be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent
-in this command 11 crc Frame checksum Note: The checksum is not recognized so
-far, and thus it should be manually set ``` ###### Set Siren Command Command
-used to enable/disable the siren ``` 'Set Siren On ' Command 0E 05 00 00 00 00
-00 00 00 00 1C 'Set Siren Off' Command 0E 06 00 00 00 00 00 00 00 00 1D ```
-###### Set Arm Command Command used to arm/disarm the alarm ``` 'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17 'Disarm' Command 0E 02 00 00 00 00 00 00 00 00
-18 ``` ###### Set Output Command Command used to set (enable/disable) outputs
-of the control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
+up to 7 keys in a single command 9 area If the alarm is configured to have
+multiple areas, then this byte identifies the target area that the key(s) will
+be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent in
+this command 11 crc Frame checksum (excluding the 1st byte) ``` ###### Set
+Siren Command (Special Command) Command used to enable/disable the siren ```
+'Set Siren' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments -----
+-------------------------------------------------------------------------- 1 0E
+Hexadecimal representation of the special commands 2 on Sets the siren on or
+off: - 0x05 if is to set siren on - 0x06 if is to set siren off 3-10 XX Not
+used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Arm Command (Special Command) Command used to arm/disarm the alarm
+``` 'Arm/Disarm' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments
+------------------------------------------------------------------------------
+- 1 0E Hexadecimal representation of the special commands 2 on Arm/Disarm the
+alarm: - 0x01 if is to arm the alarm - 0x02 if is to disarm the alarm 3-10 XX
+Not used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Output Command Command used to set (enable/disable) outputs of the
+control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
 Identifier Comments -----------------------------------------------------------
--------------------- 1 0E Hexadecimal representation of special functions 2 on
-Special function to be executed: Set Output On: Set this byte to 03 Set Output
-Off: Set this byte to 04 3 out This byte represents the index of the target
-output. Supports setting the outputs 1-5, which values in this byte are 0-
-4 respectively. Here is the list of commands for each single output: '1 On': 0E
-03 00 00 00 00 00 00 00 00 1A '1 Off': 0E 04 00 00 00 00 00 00 00 00 1A '2 On':
-0C 03 01 00 00 00 00 00 00 00 1A '2 Off': 0C 04 01 00 00 00 00 00 00 00 1A '3
-On': 0C 03 02 00 00 00 00 00 00 00 1B '3 Off': 0C 04 02 00 00 00 00 00 00 00 1B
-'4 On': 0C 03 03 00 00 00 00 00 00 00 1D '4 Off': 0C 04 03 00 00 00 00 00 00 00
-1D '5 On': 0C 03 04 00 00 00 00 00 00 00 1D '5 Off': 0C 04 04 00 00 00 00 00 00
-00 1D 4-10 XX All those bytes should be settled to 00. 11 crc Frame checksum
-Note: The checksum is not recognized so far, and thus it should be manually set
-``` ###### Get Status Command Command used to request the overall status of the
-control panel. After sending this command is expected the control panel to
-answer with the [`Get Status Response`](#get-status-response). ``` 'Get Status'
-Command 01 00 00 00 91 30 19 0F 00 00 F1 Byte Identifier Comments -------------
---------------- 1 01 Hexadecimal representation of the 'Get Status' command. 2-
-10 XX The meaning of those bytes are unknown, and thus should be always sent
-shown above. 11 F1 Frame Checksum. Since the checksum algorithm is unknown and
-this bytes of this command have always the same value, the checksum value
-should always be 'F1' ``` ###### Get Status Response Response of [`Get Status
-Command`](#get-status-command). This frame contains all the relevant
-information about the status of the control panel. ``` 'Get Status' Response 04
-XX XX
+-------------------- 1 0E Hexadecimal representation of special commands 2 on
+Special function to be executed: Set Output On: Set this byte to 0x03 Set
+Output Off: Set this byte to 0x04 3 out This byte represents the index of the
+target output. Supports setting the outputs 1-5, which values in this byte are
+0-4 respectively. 4-10 XX All those bytes should be set to 0. 11 crc Frame
+checksum (excluding the 1st byte) ``` ###### Get Status Command Command used to
+request the overall status of the control panel. After sending this command is
+expected the control panel to answer with the [`Get Status Response`](#get-
+status-response). ``` 'Get Status' Command 01 00 00 00     00 00  Byte
+Identifier Comments ---------------------------- 1 01 Hexadecimal
+representation of the 'Get Status' command. 2-4 XX This bytes are not used and
+thus set to 0. 5-8 c1..c7 Corresponds to the installer code needed to have
+permissions to get the alarm status. Each digit occupies a nibble. Not used
+digits should be set to 0xF. 9..10 XX This bytes are not used and thus set to
+0. 11 crc Frame checksum (excluding the 1st byte) ``` ###### Get Status
+Response Response of [`Get Status Command`](#get-status-command). This frame
+contains all the relevant information about the status of the control panel.
+``` 'Get Status' Response 04       XX XX
 
 >  Byte Identifier Comments ---------------------------- 1 04 : Hexadecimal
 representation of the 'Get Status' response 2-3 out : Each bit set indicates
 whether an output is on. Maximum number of outputs is 14. Bits 1-8 of byte 3
 correspond to the outputs 1-8 of the control panel. Bits 1-6 of byte 2
 correspond to the outputs 9-14 of the control panel. Bits 7-8 of byte 2 are not
 used. 4-5 zone : Each bit set indicates whether a zone is triggered. Maximum
```

### Comparing `bosch-control-panel-cc880p-3.0.0/README.md` & `bosch-control-panel-cc880p-3.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -169,119 +169,101 @@
 C0 <k1> <k2> <k3> <k4> <k5> <k6> <k7> <area> <nKeys> <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
 1       C0          Hexadecimal representation of the 'Send Key' command
 2-8     k<n>        Each byte is represents the key of the keypad. Can be sent
                         from 1 up to 7 keys in a single command
-                        Note: Because it was not possible to determine the
-                        checksum algorithm, the keys can only be sent one at a
-                        time. Below is the list of the frames corresponding to
-                        all the keys available:
-                            '0': 0C 00 00 00 00 00 00 00 00 01 16
-                            '1': 0C 01 00 00 00 00 00 00 00 01 16
-                            '2': 0C 02 00 00 00 00 00 00 00 01 17
-                            '3': 0C 03 00 00 00 00 00 00 00 01 19
-                            '4': 0C 04 00 00 00 00 00 00 00 01 19
-                            '5': 0C 05 00 00 00 00 00 00 00 01 1B
-                            '6': 0C 06 00 00 00 00 00 00 00 01 1C
-                            '7': 0C 07 00 00 00 00 00 00 00 01 1C
-                            '8': 0C 08 00 00 00 00 00 00 00 01 1D
-                            '9': 0C 09 00 00 00 00 00 00 00 01 1F
-                            '#': 0C 1A 00 00 00 00 00 00 00 01 2F
-                            '*': 0C 1B 00 00 00 00 00 00 00 01 31
 9       area        If the alarm is configured to have multiple areas, then
                         this byte identifies the target area that the key(s)
                         will be sent to. Otherwise set it to '00'.
 10      nKeys       Number of keys being sent in this command
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Siren Command
+###### Set Siren Command (Special Command)
 
 Command used to enable/disable the siren
 
 ```
-'Set Siren On ' Command
-0E 05 00 00 00 00 00 00 00 00 1C
+'Set Siren' Command
 
-'Set Siren Off' Command
-0E 06 00 00 00 00 00 00 00 00 1D
+0E <on> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Sets the siren on or off:
+                      - 0x05 if is to set siren on
+                      - 0x06 if is to set siren off
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Arm Command
+###### Set Arm Command (Special Command)
 
 Command used to arm/disarm the alarm
 
 ```
-'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17
+'Arm/Disarm' Command
 
-'Disarm' Command
-0E 02 00 00 00 00 00 00 00 00 18
+0E <arm> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Arm/Disarm the alarm:
+                      - 0x01 if is to arm the alarm
+                      - 0x02 if is to disarm the alarm
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
+
 ###### Set Output Command
 
 Command used to set (enable/disable) outputs of the control panel.
 
 ```
 'Set Output' Command
 
 0E <on> <out> 00 00 00 00 00 00 00 <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
-1       0E          Hexadecimal representation of special functions
+1       0E          Hexadecimal representation of special commands
 2       on          Special function to be executed:
-                        Set Output On: Set this byte to 03
-                        Set Output Off: Set this byte to 04
+                        Set Output On: Set this byte to 0x03
+                        Set Output Off: Set this byte to 0x04
 3       out         This byte represents the index of the target output.
                       Supports setting the outputs 1-5, which values in this
                       byte are 0-4 respectively.
-                      Here is the list of commands for each single output:
-
-                            '1 On':   0E 03 00 00 00 00 00 00 00 00 1A
-                            '1 Off':  0E 04 00 00 00 00 00 00 00 00 1A
-                            '2 On':   0C 03 01 00 00 00 00 00 00 00 1A
-                            '2 Off':  0C 04 01 00 00 00 00 00 00 00 1A
-                            '3 On':   0C 03 02 00 00 00 00 00 00 00 1B
-                            '3 Off':  0C 04 02 00 00 00 00 00 00 00 1B
-                            '4 On':   0C 03 03 00 00 00 00 00 00 00 1D
-                            '4 Off':  0C 04 03 00 00 00 00 00 00 00 1D
-                            '5 On':   0C 03 04 00 00 00 00 00 00 00 1D
-                            '5 Off':  0C 04 04 00 00 00 00 00 00 00 1D
-4-10    XX          All those bytes should be settled to 00.
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+4-10    XX          All those bytes should be set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Command
 
 Command used to request the overall status of the control panel.
 After sending this command is expected the control panel to answer with the [`Get Status Response`](#get-status-response).
 
 ```
 'Get Status' Command
 
-01 00 00 00 91 30 19 0F 00 00 F1
+01 00 00 00 <c2c1> <c4c3> <c6c5> <c7> 00 00 <crc>
 
 Byte   Identifier   Comments
 ----------------------------
 1       01          Hexadecimal representation of the 'Get Status' command.
-2-10    XX          The meaning of those bytes are unknown, and thus should be
-                        always sent shown above.
-11      F1          Frame Checksum. Since the checksum algorithm is unknown and
-                        this bytes of this command have always the same value,
-                        the checksum value should always be 'F1'
+2-4     XX          This bytes are not used and thus set to 0.
+5-8     c1..c7      Corresponds to the installer code needed to have permissions
+                      to get the alarm status. Each digit occupies a nibble.
+                      Not used digits should be set to 0xF.
+9..10   XX          This bytes are not used and thus set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Response
 
 Response of [`Get Status Command`](#get-status-command). This frame contains all the relevant information about the status of the control panel.
 
 ```
```

#### html2text {}

```diff
@@ -81,58 +81,51 @@
 ##### Frames Below are presented the decoded frames that are used by this
 library so far: ###### Send Keys Command Command used to send keys to the
 control panel simulating the pressing of the keypad keys. ``` 'Send Keys'
 Command C0
    Byte Identifier Comments ---------------------------------------------------
 ---------------------------- 1 C0 Hexadecimal representation of the 'Send Key'
 command 2-8 k Each byte is represents the key of the keypad. Can be sent from 1
-up to 7 keys in a single command Note: Because it was not possible to determine
-the checksum algorithm, the keys can only be sent one at a time. Below is the
-list of the frames corresponding to all the keys available: '0': 0C 00 00 00 00
-00 00 00 00 01 16 '1': 0C 01 00 00 00 00 00 00 00 01 16 '2': 0C 02 00 00 00 00
-00 00 00 01 17 '3': 0C 03 00 00 00 00 00 00 00 01 19 '4': 0C 04 00 00 00 00 00
-00 00 01 19 '5': 0C 05 00 00 00 00 00 00 00 01 1B '6': 0C 06 00 00 00 00 00 00
-00 01 1C '7': 0C 07 00 00 00 00 00 00 00 01 1C '8': 0C 08 00 00 00 00 00 00 00
-01 1D '9': 0C 09 00 00 00 00 00 00 00 01 1F '#': 0C 1A 00 00 00 00 00 00 00 01
-2F '*': 0C 1B 00 00 00 00 00 00 00 01 31 9 area If the alarm is configured to
-have multiple areas, then this byte identifies the target area that the key(s)
-will be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent
-in this command 11 crc Frame checksum Note: The checksum is not recognized so
-far, and thus it should be manually set ``` ###### Set Siren Command Command
-used to enable/disable the siren ``` 'Set Siren On ' Command 0E 05 00 00 00 00
-00 00 00 00 1C 'Set Siren Off' Command 0E 06 00 00 00 00 00 00 00 00 1D ```
-###### Set Arm Command Command used to arm/disarm the alarm ``` 'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17 'Disarm' Command 0E 02 00 00 00 00 00 00 00 00
-18 ``` ###### Set Output Command Command used to set (enable/disable) outputs
-of the control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
+up to 7 keys in a single command 9 area If the alarm is configured to have
+multiple areas, then this byte identifies the target area that the key(s) will
+be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent in
+this command 11 crc Frame checksum (excluding the 1st byte) ``` ###### Set
+Siren Command (Special Command) Command used to enable/disable the siren ```
+'Set Siren' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments -----
+-------------------------------------------------------------------------- 1 0E
+Hexadecimal representation of the special commands 2 on Sets the siren on or
+off: - 0x05 if is to set siren on - 0x06 if is to set siren off 3-10 XX Not
+used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Arm Command (Special Command) Command used to arm/disarm the alarm
+``` 'Arm/Disarm' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments
+------------------------------------------------------------------------------
+- 1 0E Hexadecimal representation of the special commands 2 on Arm/Disarm the
+alarm: - 0x01 if is to arm the alarm - 0x02 if is to disarm the alarm 3-10 XX
+Not used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Output Command Command used to set (enable/disable) outputs of the
+control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
 Identifier Comments -----------------------------------------------------------
--------------------- 1 0E Hexadecimal representation of special functions 2 on
-Special function to be executed: Set Output On: Set this byte to 03 Set Output
-Off: Set this byte to 04 3 out This byte represents the index of the target
-output. Supports setting the outputs 1-5, which values in this byte are 0-
-4 respectively. Here is the list of commands for each single output: '1 On': 0E
-03 00 00 00 00 00 00 00 00 1A '1 Off': 0E 04 00 00 00 00 00 00 00 00 1A '2 On':
-0C 03 01 00 00 00 00 00 00 00 1A '2 Off': 0C 04 01 00 00 00 00 00 00 00 1A '3
-On': 0C 03 02 00 00 00 00 00 00 00 1B '3 Off': 0C 04 02 00 00 00 00 00 00 00 1B
-'4 On': 0C 03 03 00 00 00 00 00 00 00 1D '4 Off': 0C 04 03 00 00 00 00 00 00 00
-1D '5 On': 0C 03 04 00 00 00 00 00 00 00 1D '5 Off': 0C 04 04 00 00 00 00 00 00
-00 1D 4-10 XX All those bytes should be settled to 00. 11 crc Frame checksum
-Note: The checksum is not recognized so far, and thus it should be manually set
-``` ###### Get Status Command Command used to request the overall status of the
-control panel. After sending this command is expected the control panel to
-answer with the [`Get Status Response`](#get-status-response). ``` 'Get Status'
-Command 01 00 00 00 91 30 19 0F 00 00 F1 Byte Identifier Comments -------------
---------------- 1 01 Hexadecimal representation of the 'Get Status' command. 2-
-10 XX The meaning of those bytes are unknown, and thus should be always sent
-shown above. 11 F1 Frame Checksum. Since the checksum algorithm is unknown and
-this bytes of this command have always the same value, the checksum value
-should always be 'F1' ``` ###### Get Status Response Response of [`Get Status
-Command`](#get-status-command). This frame contains all the relevant
-information about the status of the control panel. ``` 'Get Status' Response 04
-XX XX
+-------------------- 1 0E Hexadecimal representation of special commands 2 on
+Special function to be executed: Set Output On: Set this byte to 0x03 Set
+Output Off: Set this byte to 0x04 3 out This byte represents the index of the
+target output. Supports setting the outputs 1-5, which values in this byte are
+0-4 respectively. 4-10 XX All those bytes should be set to 0. 11 crc Frame
+checksum (excluding the 1st byte) ``` ###### Get Status Command Command used to
+request the overall status of the control panel. After sending this command is
+expected the control panel to answer with the [`Get Status Response`](#get-
+status-response). ``` 'Get Status' Command 01 00 00 00     00 00  Byte
+Identifier Comments ---------------------------- 1 01 Hexadecimal
+representation of the 'Get Status' command. 2-4 XX This bytes are not used and
+thus set to 0. 5-8 c1..c7 Corresponds to the installer code needed to have
+permissions to get the alarm status. Each digit occupies a nibble. Not used
+digits should be set to 0xF. 9..10 XX This bytes are not used and thus set to
+0. 11 crc Frame checksum (excluding the 1st byte) ``` ###### Get Status
+Response Response of [`Get Status Command`](#get-status-command). This frame
+contains all the relevant information about the status of the control panel.
+``` 'Get Status' Response 04       XX XX
 
 >  Byte Identifier Comments ---------------------------- 1 04 : Hexadecimal
 representation of the 'Get Status' response 2-3 out : Each bit set indicates
 whether an output is on. Maximum number of outputs is 14. Bits 1-8 of byte 3
 correspond to the outputs 1-8 of the control panel. Bits 1-6 of byte 2
 correspond to the outputs 9-14 of the control panel. Bits 7-8 of byte 2 are not
 used. 4-5 zone : Each bit set indicates whether a zone is triggered. Maximum
```

### Comparing `bosch-control-panel-cc880p-3.0.0/setup.cfg` & `bosch-control-panel-cc880p-3.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = bosch-control-panel-cc880p
-version = attr: bosch.control_panel.cc880p.version.__version__
 author = Hugo Gomes
 author_email = hgomes88@gmail.com
 description = Library to interface with the old CC880p Bosch COntrol Panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hgomes88/bosch-control-panel-cc880p
 project_urls = 
 	Tracker = https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 	Download = https://pypi.org/project/bosch-control-panel-cc880p/
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
+dynamic = ["version"]
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >=3.8
 include_package_data = True
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from bosch.control_panel.cc880p.models.cp import Area
 from bosch.control_panel.cc880p.models.cp import Availability
 from bosch.control_panel.cc880p.models.cp import ControlPanelEntity
 from bosch.control_panel.cc880p.models.cp import CpVersion
 from bosch.control_panel.cc880p.models.cp import Id
 from bosch.control_panel.cc880p.models.cp import Output
 from bosch.control_panel.cc880p.models.cp import Siren
+from bosch.control_panel.cc880p.models.cp import Time
 from bosch.control_panel.cc880p.models.cp import Zone
 from bosch.control_panel.cc880p.utils import to_hex
 
 logging.basicConfig(level=logging.WARNING)
 
 prev_data = None
 
@@ -43,14 +44,16 @@
         print(f'Output {id} updated: {cp}')
     elif isinstance(cp, Siren):
         print(f'Siren updated: {cp}')
     elif isinstance(cp, Area):
         print(f'Area {id} updated: {cp}')
     elif isinstance(cp, Availability):
         print(f'Control Panel availability is: {cp}')
+    elif isinstance(cp, Time):
+        print(f'Control Panel time is: {cp}')
 
     return True
 
 
 async def run_listen_mode(cp: CP):
     """Run the control panel in listen mode."""
     cp.add_data_listener(data_listener)
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cmds.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/cmds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command Line Commands Management."""
+from datetime import datetime
 from typing import Any
 from typing import List
 
 from bosch.control_panel.cc880p.cli.parser import Args
 from bosch.control_panel.cc880p.cli.parser import Commands
 from bosch.control_panel.cc880p.cp import CP
 from bosch.control_panel.cc880p.utils import checksum
@@ -45,14 +46,19 @@
     """Handle outputs command."""
     await cmd(cp, cp.control_panel.outputs[out])(cp.set_output)(
         id=out,
         on=status
     )
 
 
+async def handle_time_command(cp: CP, time: datetime):
+    """Handle the set time command."""
+    await cmd(cp, cp.control_panel.time)(cp.set_time)(time=time)
+
+
 async def handle_keys_command(cp: CP, keys: List[str]):
     """Handle the keys sending."""
     keys = [i for ele in keys for i in ele]
     await cmd(cp)(cp.send_keys)(keys=keys)
     await cmd(cp, cp.control_panel.areas)(cp.get_status)()
 
 
@@ -86,13 +92,15 @@
 
 async def handle_command(cp: CP, args: Args):
     """Handle the control panel commands."""
     if args.cmd == Commands.SetMode:
         await handle_mode_command(cp, args.mode)
     if args.cmd == Commands.SetSiren:
         await handle_siren_command(cp, args.status)
+    if args.cmd == Commands.SetTime:
+        await handle_time_command(cp, args.time)
     if args.cmd == Commands.SetOutput:
         await handle_out_command(cp, args.out, args.status)
     if args.cmd == Commands.SendKeys:
         await handle_keys_command(cp, args.keys)
     if args.cmd == Commands.SendRaw:
         await handle_raw_command(cp, args.raw)
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/parser.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cli/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Control panel command line parser."""
 from argparse import ArgumentParser
+from datetime import datetime
 from enum import Enum
 from typing import List
 from typing import Optional
 
 from bosch.control_panel.cc880p.version import __version__ as version
 from distutils.util import strtobool
 
 
 class Commands(Enum):
     """Supported Commands."""
 
     SetSiren = 0
     SetMode = 1
     SetOutput = 2
-    SendKeys = 3
-    SendRaw = 4
+    SetTime = 3
+    SendKeys = 4
+    SendRaw = 5
 
 
 class Args:
     """Parser arguments."""
 
     connect: str
     port: int
     cmd: Optional[Commands]
     keys: List[str]
     mode: str
     status: bool
     out: int
+    time: datetime
 
 
 args = Args()
 
 
 def get_parser():
     """Get the argument parser."""
@@ -85,14 +88,15 @@
     subparsers = cmds_parser.add_subparsers()
 
     get_cmd_send_keys_parser(subparsers)
     get_cmd_send_raw_parser(subparsers)
     get_cmd_set_mode_parser(subparsers)
     get_cmd_set_siren_parser(subparsers)
     get_cmd_set_output_parser(subparsers)
+    get_cmd_set_time_parser(subparsers)
 
 
 def get_cmd_send_keys_parser(subparsers):
     """Send keys command parser."""
     # SEND KEYS command
     cmd_send_keys_parser = subparsers.add_parser(
         'sendKeys',
@@ -192,10 +196,35 @@
     cmd_set_out_parser.add_argument(
         'status',
         type=lambda x: bool(strtobool(x)),
         help='Changes the output'
     )
 
 
+def get_cmd_set_time_parser(subparsers):
+    """Set output parser."""
+    # SET OUTPUT command
+    cmd_set_time_parser = subparsers.add_parser(
+        'setTime',
+        help='Set the time of the control panel'
+    )
+    cmd_set_time_parser.add_argument(
+        'cmd',
+        action='store_const',
+        const=Commands.SetTime
+    )
+    cmd_set_time_parser.add_argument(
+        '-t', '--time',
+        required=False,
+        metavar='TIME',
+        type=datetime.fromisoformat,
+        help=(
+            'Datetime to be set on the control panel. It should be in iso '
+            'format (e.g.: "2023-12-31 23:59:59"). If not used, the current '
+            'time will be applied.'
+        )
+    )
+
+
 def get_args():
     """Parse and get the arguments."""
     return get_parser().parse_args(namespace=args)
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cp.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Control Panel."""
 import asyncio
 import dataclasses
+import datetime
 import logging
 from asyncio import AbstractEventLoop
 from enum import Enum
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
@@ -12,20 +13,20 @@
 from bosch.control_panel.cc880p.models.callbacks import ControlPanelListener
 from bosch.control_panel.cc880p.models.callbacks import DataListener
 from bosch.control_panel.cc880p.models.constants import Id
 from bosch.control_panel.cc880p.models.constants import MAX_KEYS
 from bosch.control_panel.cc880p.models.cp import ArmingMode
 from bosch.control_panel.cc880p.models.cp import ControlPanel
 from bosch.control_panel.cc880p.models.cp import CpModel
-from bosch.control_panel.cc880p.models.cp import Time
 from bosch.control_panel.cc880p.models.requests import KeysRequest
 from bosch.control_panel.cc880p.models.requests import Request
 from bosch.control_panel.cc880p.models.requests import SetArmingRequest
 from bosch.control_panel.cc880p.models.requests import SetOutRequest
 from bosch.control_panel.cc880p.models.requests import SetSirenRequest
+from bosch.control_panel.cc880p.models.requests import SetTimeRequest
 from bosch.control_panel.cc880p.models.requests import StatusRequest
 from bosch.control_panel.cc880p.models.responses import Response
 from bosch.control_panel.cc880p.models.responses import StatusResponse
 from bosch.control_panel.cc880p.utils import checksum
 from bosch.control_panel.cc880p.utils import to_hex
 
 _LOGGER = logging.getLogger(__name__)
@@ -174,14 +175,19 @@
         if on and self._control_panel.siren.on != on:
             # Switch on the siren
             await self.send_request(SetSirenRequest(on), StatusResponse)
         elif not on and self._control_panel.siren.on != on:
             # Switch of the siren
             await self.send_request(SetSirenRequest(on), StatusResponse)
 
+    async def set_time(self, time: datetime.datetime = None):
+        """Set time."""
+        # Set the time in the alarm
+        await self.send_request(SetTimeRequest(time), StatusResponse)
+
     async def get_status(self):
         """Command to request the status of the alarm."""
         request = StatusRequest(installer_code=self._installer_code)
         await self.send_request(request, StatusResponse)
 
     async def send_request(
             self,
@@ -469,17 +475,16 @@
                 for listener in self._control_panel_listeners:
                     asyncio.create_task(listener(area_number, area))
 
                 _LOGGER.info(
                     'Status of Area %d changed to %s', area_number, area.mode
                 )
 
-    def _update_time(self, time: Time):
-        if self._control_panel.time_utc != time:
-            self._control_panel.time_utc = Time(
-                hour=time.hour, minute=time.minute
-            )
+    def _update_time(self, time: datetime.time):
+
+        if self._control_panel.time.time != time:
+            self._control_panel.time.time = time
 
             for listener in self._control_panel_listeners:
-                asyncio.create_task(listener(0, self._control_panel.time_utc))
+                asyncio.create_task(listener(0, self._control_panel.time))
 
-            _LOGGER.info('Time updated %s', self._control_panel.time_utc)
+            _LOGGER.info('Time updated %s', self._control_panel.time)
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/cp.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,33 +79,44 @@
 @dataclass
 class Area(ControlPanelEntity):
     """Dataclass representing the alarm area."""
 
     mode: ArmingMode = ArmingMode.DISARMED
 
 
-class Time(datetime.time):
+@dataclass
+class Time(ControlPanelEntity):
     """Datetime."""
 
+    time: datetime.time = datetime.time(hour=0, minute=0)
+
+    def __str__(self) -> str:
+        """Convert the object hours and minutes into a string."""
+        return f'{self.time.hour}:{self.time.minute}'
+
+    def __repr__(self) -> str:
+        """Convert the Time object into its string representation."""
+        return f'Time(time={str(self)})'
+
 
 @dataclass
 class ControlPanel(ControlPanelEntity):
     """Dataclass representing the control panel object."""
 
     siren: Siren
     areas: Dict[Id, Area]
     zones: Dict[Id, Zone]
     outputs: Dict[Id, Output]
-    time_utc: Time
+    time: Time
     availability: Availability
 
     @staticmethod
     def build(model: CpModel) -> 'ControlPanel':
         """Build a control panel object."""
         return ControlPanel(
             siren=Siren(),
             outputs={i + 1: Output() for i in range(model.n_outputs)},
             areas={i + 1: Area() for i in range(model.n_areas)},
             zones={i + 1: Zone() for i in range(model.n_zones)},
-            time_utc=Time(),
+            time=Time(),
             availability=Availability()
         )
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/requests.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Requests related data models."""
 from dataclasses import dataclass
 from dataclasses import field
+from datetime import datetime
 from enum import Enum
 
 from bosch.control_panel.cc880p.utils import checksum
 from bosch.control_panel.cc880p.utils import swap_nibbles
 
 
 class RequestsProps(Enum):
@@ -16,14 +17,16 @@
     KeysRequestSize = 11
     SetOutRequestCode = '0E'
     SetOutRequestSize = 11
     SetArmingRequestCode = '0E'
     SetArmingRequestSize = 11
     SetSirenRequestCode = '0E'
     SetSirenRequestSize = 11
+    SetTimeRequestCode = '0E'
+    SetTimeRequestSize = 11
 
 
 @dataclass
 class Request:
     """Base Request Class."""
 
     code: str
@@ -138,7 +141,39 @@
     on: bool
 
     def encode(self):
         """Encode the request to set the siren on/off."""
         empty8 = [0x00] * 8
         status = 0x05 if self.on else 0x06
         return self._encode(bytes([status, *empty8]))
+
+
+@dataclass
+class SetTimeRequest(Request):
+    """Set TIme Request."""
+
+    code: str = field(
+        init=False,
+        default=RequestsProps.SetSirenRequestCode.value)
+    size: int = field(
+        init=False,
+        default=RequestsProps.SetSirenRequestSize.value)
+    time: datetime
+
+    def encode(self):
+        """Encode the request to set the siren on/off."""
+        empty3 = [0x00] * 3
+        set_time = 0x0C
+
+        if self.time is None:
+            self.time = datetime.now()
+
+        year = int(self.time.strftime('%y'))
+        return self._encode(bytes([
+            set_time,
+            self.time.hour,
+            self.time.minute,
+            year,
+            self.time.month,
+            self.time.day,
+            *empty3
+        ]))
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/responses.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/models/responses.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/utils.py` & `bosch-control-panel-cc880p-3.1.0/src/bosch/control_panel/cc880p/utils.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
@@ -186,119 +186,101 @@
 C0 <k1> <k2> <k3> <k4> <k5> <k6> <k7> <area> <nKeys> <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
 1       C0          Hexadecimal representation of the 'Send Key' command
 2-8     k<n>        Each byte is represents the key of the keypad. Can be sent
                         from 1 up to 7 keys in a single command
-                        Note: Because it was not possible to determine the
-                        checksum algorithm, the keys can only be sent one at a
-                        time. Below is the list of the frames corresponding to
-                        all the keys available:
-                            '0': 0C 00 00 00 00 00 00 00 00 01 16
-                            '1': 0C 01 00 00 00 00 00 00 00 01 16
-                            '2': 0C 02 00 00 00 00 00 00 00 01 17
-                            '3': 0C 03 00 00 00 00 00 00 00 01 19
-                            '4': 0C 04 00 00 00 00 00 00 00 01 19
-                            '5': 0C 05 00 00 00 00 00 00 00 01 1B
-                            '6': 0C 06 00 00 00 00 00 00 00 01 1C
-                            '7': 0C 07 00 00 00 00 00 00 00 01 1C
-                            '8': 0C 08 00 00 00 00 00 00 00 01 1D
-                            '9': 0C 09 00 00 00 00 00 00 00 01 1F
-                            '#': 0C 1A 00 00 00 00 00 00 00 01 2F
-                            '*': 0C 1B 00 00 00 00 00 00 00 01 31
 9       area        If the alarm is configured to have multiple areas, then
                         this byte identifies the target area that the key(s)
                         will be sent to. Otherwise set it to '00'.
 10      nKeys       Number of keys being sent in this command
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Siren Command
+###### Set Siren Command (Special Command)
 
 Command used to enable/disable the siren
 
 ```
-'Set Siren On ' Command
-0E 05 00 00 00 00 00 00 00 00 1C
+'Set Siren' Command
 
-'Set Siren Off' Command
-0E 06 00 00 00 00 00 00 00 00 1D
+0E <on> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Sets the siren on or off:
+                      - 0x05 if is to set siren on
+                      - 0x06 if is to set siren off
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
-###### Set Arm Command
+###### Set Arm Command (Special Command)
 
 Command used to arm/disarm the alarm
 
 ```
-'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17
+'Arm/Disarm' Command
 
-'Disarm' Command
-0E 02 00 00 00 00 00 00 00 00 18
+0E <arm> 00 00 00 00 00 00 00 00 <crc>
 
+Byte    Identifier  Comments
+-------------------------------------------------------------------------------
+1       0E          Hexadecimal representation of the special commands
+2       on          Arm/Disarm the alarm:
+                      - 0x01 if is to arm the alarm
+                      - 0x02 if is to disarm the alarm
+3-10    XX          Not used and thus, set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
+
 ###### Set Output Command
 
 Command used to set (enable/disable) outputs of the control panel.
 
 ```
 'Set Output' Command
 
 0E <on> <out> 00 00 00 00 00 00 00 <crc>
 
 Byte    Identifier  Comments
 -------------------------------------------------------------------------------
-1       0E          Hexadecimal representation of special functions
+1       0E          Hexadecimal representation of special commands
 2       on          Special function to be executed:
-                        Set Output On: Set this byte to 03
-                        Set Output Off: Set this byte to 04
+                        Set Output On: Set this byte to 0x03
+                        Set Output Off: Set this byte to 0x04
 3       out         This byte represents the index of the target output.
                       Supports setting the outputs 1-5, which values in this
                       byte are 0-4 respectively.
-                      Here is the list of commands for each single output:
-
-                            '1 On':   0E 03 00 00 00 00 00 00 00 00 1A
-                            '1 Off':  0E 04 00 00 00 00 00 00 00 00 1A
-                            '2 On':   0C 03 01 00 00 00 00 00 00 00 1A
-                            '2 Off':  0C 04 01 00 00 00 00 00 00 00 1A
-                            '3 On':   0C 03 02 00 00 00 00 00 00 00 1B
-                            '3 Off':  0C 04 02 00 00 00 00 00 00 00 1B
-                            '4 On':   0C 03 03 00 00 00 00 00 00 00 1D
-                            '4 Off':  0C 04 03 00 00 00 00 00 00 00 1D
-                            '5 On':   0C 03 04 00 00 00 00 00 00 00 1D
-                            '5 Off':  0C 04 04 00 00 00 00 00 00 00 1D
-4-10    XX          All those bytes should be settled to 00.
-11      crc         Frame checksum
-                        Note: The checksum is not recognized so far, and thus
-                        it should be manually set
+4-10    XX          All those bytes should be set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Command
 
 Command used to request the overall status of the control panel.
 After sending this command is expected the control panel to answer with the [`Get Status Response`](#get-status-response).
 
 ```
 'Get Status' Command
 
-01 00 00 00 91 30 19 0F 00 00 F1
+01 00 00 00 <c2c1> <c4c3> <c6c5> <c7> 00 00 <crc>
 
 Byte   Identifier   Comments
 ----------------------------
 1       01          Hexadecimal representation of the 'Get Status' command.
-2-10    XX          The meaning of those bytes are unknown, and thus should be
-                        always sent shown above.
-11      F1          Frame Checksum. Since the checksum algorithm is unknown and
-                        this bytes of this command have always the same value,
-                        the checksum value should always be 'F1'
+2-4     XX          This bytes are not used and thus set to 0.
+5-8     c1..c7      Corresponds to the installer code needed to have permissions
+                      to get the alarm status. Each digit occupies a nibble.
+                      Not used digits should be set to 0xF.
+9..10   XX          This bytes are not used and thus set to 0.
+11      crc         Frame checksum (excluding the 1st byte)
 ```
 
 ###### Get Status Response
 
 Response of [`Get Status Command`](#get-status-command). This frame contains all the relevant information about the status of the control panel.
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.0.0 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
@@ -90,58 +90,51 @@
 ##### Frames Below are presented the decoded frames that are used by this
 library so far: ###### Send Keys Command Command used to send keys to the
 control panel simulating the pressing of the keypad keys. ``` 'Send Keys'
 Command C0
    Byte Identifier Comments ---------------------------------------------------
 ---------------------------- 1 C0 Hexadecimal representation of the 'Send Key'
 command 2-8 k Each byte is represents the key of the keypad. Can be sent from 1
-up to 7 keys in a single command Note: Because it was not possible to determine
-the checksum algorithm, the keys can only be sent one at a time. Below is the
-list of the frames corresponding to all the keys available: '0': 0C 00 00 00 00
-00 00 00 00 01 16 '1': 0C 01 00 00 00 00 00 00 00 01 16 '2': 0C 02 00 00 00 00
-00 00 00 01 17 '3': 0C 03 00 00 00 00 00 00 00 01 19 '4': 0C 04 00 00 00 00 00
-00 00 01 19 '5': 0C 05 00 00 00 00 00 00 00 01 1B '6': 0C 06 00 00 00 00 00 00
-00 01 1C '7': 0C 07 00 00 00 00 00 00 00 01 1C '8': 0C 08 00 00 00 00 00 00 00
-01 1D '9': 0C 09 00 00 00 00 00 00 00 01 1F '#': 0C 1A 00 00 00 00 00 00 00 01
-2F '*': 0C 1B 00 00 00 00 00 00 00 01 31 9 area If the alarm is configured to
-have multiple areas, then this byte identifies the target area that the key(s)
-will be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent
-in this command 11 crc Frame checksum Note: The checksum is not recognized so
-far, and thus it should be manually set ``` ###### Set Siren Command Command
-used to enable/disable the siren ``` 'Set Siren On ' Command 0E 05 00 00 00 00
-00 00 00 00 1C 'Set Siren Off' Command 0E 06 00 00 00 00 00 00 00 00 1D ```
-###### Set Arm Command Command used to arm/disarm the alarm ``` 'Arm' Command
-0E 01 00 00 00 00 00 00 00 00 17 'Disarm' Command 0E 02 00 00 00 00 00 00 00 00
-18 ``` ###### Set Output Command Command used to set (enable/disable) outputs
-of the control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
+up to 7 keys in a single command 9 area If the alarm is configured to have
+multiple areas, then this byte identifies the target area that the key(s) will
+be sent to. Otherwise set it to '00'. 10 nKeys Number of keys being sent in
+this command 11 crc Frame checksum (excluding the 1st byte) ``` ###### Set
+Siren Command (Special Command) Command used to enable/disable the siren ```
+'Set Siren' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments -----
+-------------------------------------------------------------------------- 1 0E
+Hexadecimal representation of the special commands 2 on Sets the siren on or
+off: - 0x05 if is to set siren on - 0x06 if is to set siren off 3-10 XX Not
+used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Arm Command (Special Command) Command used to arm/disarm the alarm
+``` 'Arm/Disarm' Command 0E  00 00 00 00 00 00 00 00  Byte Identifier Comments
+------------------------------------------------------------------------------
+- 1 0E Hexadecimal representation of the special commands 2 on Arm/Disarm the
+alarm: - 0x01 if is to arm the alarm - 0x02 if is to disarm the alarm 3-10 XX
+Not used and thus, set to 0. 11 crc Frame checksum (excluding the 1st byte) ```
+###### Set Output Command Command used to set (enable/disable) outputs of the
+control panel. ``` 'Set Output' Command 0E   00 00 00 00 00 00 00  Byte
 Identifier Comments -----------------------------------------------------------
--------------------- 1 0E Hexadecimal representation of special functions 2 on
-Special function to be executed: Set Output On: Set this byte to 03 Set Output
-Off: Set this byte to 04 3 out This byte represents the index of the target
-output. Supports setting the outputs 1-5, which values in this byte are 0-
-4 respectively. Here is the list of commands for each single output: '1 On': 0E
-03 00 00 00 00 00 00 00 00 1A '1 Off': 0E 04 00 00 00 00 00 00 00 00 1A '2 On':
-0C 03 01 00 00 00 00 00 00 00 1A '2 Off': 0C 04 01 00 00 00 00 00 00 00 1A '3
-On': 0C 03 02 00 00 00 00 00 00 00 1B '3 Off': 0C 04 02 00 00 00 00 00 00 00 1B
-'4 On': 0C 03 03 00 00 00 00 00 00 00 1D '4 Off': 0C 04 03 00 00 00 00 00 00 00
-1D '5 On': 0C 03 04 00 00 00 00 00 00 00 1D '5 Off': 0C 04 04 00 00 00 00 00 00
-00 1D 4-10 XX All those bytes should be settled to 00. 11 crc Frame checksum
-Note: The checksum is not recognized so far, and thus it should be manually set
-``` ###### Get Status Command Command used to request the overall status of the
-control panel. After sending this command is expected the control panel to
-answer with the [`Get Status Response`](#get-status-response). ``` 'Get Status'
-Command 01 00 00 00 91 30 19 0F 00 00 F1 Byte Identifier Comments -------------
---------------- 1 01 Hexadecimal representation of the 'Get Status' command. 2-
-10 XX The meaning of those bytes are unknown, and thus should be always sent
-shown above. 11 F1 Frame Checksum. Since the checksum algorithm is unknown and
-this bytes of this command have always the same value, the checksum value
-should always be 'F1' ``` ###### Get Status Response Response of [`Get Status
-Command`](#get-status-command). This frame contains all the relevant
-information about the status of the control panel. ``` 'Get Status' Response 04
-XX XX
+-------------------- 1 0E Hexadecimal representation of special commands 2 on
+Special function to be executed: Set Output On: Set this byte to 0x03 Set
+Output Off: Set this byte to 0x04 3 out This byte represents the index of the
+target output. Supports setting the outputs 1-5, which values in this byte are
+0-4 respectively. 4-10 XX All those bytes should be set to 0. 11 crc Frame
+checksum (excluding the 1st byte) ``` ###### Get Status Command Command used to
+request the overall status of the control panel. After sending this command is
+expected the control panel to answer with the [`Get Status Response`](#get-
+status-response). ``` 'Get Status' Command 01 00 00 00     00 00  Byte
+Identifier Comments ---------------------------- 1 01 Hexadecimal
+representation of the 'Get Status' command. 2-4 XX This bytes are not used and
+thus set to 0. 5-8 c1..c7 Corresponds to the installer code needed to have
+permissions to get the alarm status. Each digit occupies a nibble. Not used
+digits should be set to 0xF. 9..10 XX This bytes are not used and thus set to
+0. 11 crc Frame checksum (excluding the 1st byte) ``` ###### Get Status
+Response Response of [`Get Status Command`](#get-status-command). This frame
+contains all the relevant information about the status of the control panel.
+``` 'Get Status' Response 04       XX XX
 
 >  Byte Identifier Comments ---------------------------- 1 04 : Hexadecimal
 representation of the 'Get Status' response 2-3 out : Each bit set indicates
 whether an output is on. Maximum number of outputs is 14. Bits 1-8 of byte 3
 correspond to the outputs 1-8 of the control panel. Bits 1-6 of byte 2
 correspond to the outputs 9-14 of the control panel. Bits 7-8 of byte 2 are not
 used. 4-5 zone : Each bit set indicates whether a zone is triggered. Maximum
```

### Comparing `bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-3.1.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

