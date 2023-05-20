# Comparing `tmp/ScriptCollection-3.3.90-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.91-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57589 bytes, number of entries: 14
+Zip file size: 57600 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34139 b- defN 23-May-20 16:21 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6273 b- defN 22-Oct-16 19:55 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    86233 b- defN 23-May-20 16:22 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   128883 b- defN 23-May-20 16:21 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    86233 b- defN 23-May-20 18:20 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   129034 b- defN 23-May-20 18:20 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7864 b- defN 23-May-20 16:22 ScriptCollection-3.3.90.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 16:22 ScriptCollection-3.3.90.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-20 16:22 ScriptCollection-3.3.90.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-20 16:22 ScriptCollection-3.3.90.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-20 16:22 ScriptCollection-3.3.90.dist-info/RECORD
-14 files, 297706 bytes uncompressed, 55397 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7864 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/RECORD
+14 files, 297857 bytes uncompressed, 55408 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.90.dist-info/METADATA
+Filename: ScriptCollection-3.3.91.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.90.dist-info/WHEEL
+Filename: ScriptCollection-3.3.91.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.90.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.91.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.90.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.91.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.90.dist-info/RECORD
+Filename: ScriptCollection-3.3.91.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -21,15 +21,15 @@
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.90"
+version = "3.3.91"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -890,28 +890,31 @@
     @GeneralUtilities.check_arguments
     def __generate_entire_reference(self, projectname: str, project_version: str, reference_folder: str) -> None:
         all_available_version_identifier_folders_of_reference = list(
             folder for folder in GeneralUtilities.get_direct_folders_of_folder(reference_folder))
         all_available_version_identifier_folders_of_reference.reverse()  # move newer versions above
         all_available_version_identifier_folders_of_reference.insert(0, all_available_version_identifier_folders_of_reference.pop())  # move latest version to the top
         reference_versions_html_lines = []
+        reference_versions_html_lines.append('    <hr/>')
         for all_available_version_identifier_folder_of_reference in all_available_version_identifier_folders_of_reference:
             version_identifier_of_project = os.path.basename(all_available_version_identifier_folder_of_reference)
             if version_identifier_of_project == "Latest":
                 latest_version_hint = f" (v{project_version})"
             else:
                 latest_version_hint = ""
-            reference_versions_html_lines.append('    <hr/>')
-            reference_versions_html_lines.append(f'    <h2 class="display-2">{version_identifier_of_project}{latest_version_hint}</h2>')
+            reference_versions_html_lines.append(f'    <h2>{version_identifier_of_project}{latest_version_hint}</h2>')
             reference_versions_html_lines.append("    Contained codeunits:<br/>")
             reference_versions_html_lines.append("    <ul>")
             for codeunit_reference_folder in list(folder for folder in GeneralUtilities.get_direct_folders_of_folder(all_available_version_identifier_folder_of_reference)):
                 reference_versions_html_lines.append(f'      <li><a href="./{version_identifier_of_project}/{os.path.basename(codeunit_reference_folder)}/index.html">' +
                                                      f'{os.path.basename(codeunit_reference_folder)} {version_identifier_of_project}</a></li>')
             reference_versions_html_lines.append("    </ul>")
+            reference_versions_html_lines.append('    <hr/>')
+            if version_identifier_of_project == "Latest":
+                latest_version_hint = "    <h2>History</h2>"
 
         design_file = None
         design = "ModestDark"
         if design == "ModestDark":
             design_file = GeneralUtilities.get_modest_dark_url()
         # TODO make designs from customizable sources be available by a customizable name and outsource this to a class-property because this is duplicated code.
         if design_file is None:
@@ -929,15 +932,14 @@
     <meta charset="UTF-8">
     <title>{title}</title>
     {design_html}
   </head>
 
   <body>
     <h1>{title}</h1>
-    <hr/>
 {reference_versions_links_file_content}
   </body>
 
 </html>
 """  # see https://getbootstrap.com/docs/5.1/getting-started/introduction/
         GeneralUtilities.write_text_to_file(reference_index_file, reference_index_file_content)
```

## Comparing `ScriptCollection-3.3.90.dist-info/METADATA` & `ScriptCollection-3.3.91.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.90
+Version: 3.3.91
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.3.90.dist-info/entry_points.txt` & `ScriptCollection-3.3.91.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.90.dist-info/RECORD` & `ScriptCollection-3.3.91.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
 ScriptCollection/GeneralUtilities.py,sha256=7-KuXjS_S-oiMcMM9bEDGx8n4RlnGxGpqHdhXhN47I8,34139
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=ZiBZVMcsphmo49z2BwUwQYXo2uTKXPu33QW3IxCT46E,6273
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=6a0Iv8AadsvGOi-BYkNz8WNG9Aahl6xb3OxHwR2m_5I,86233
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=fxagwkr3wb9e8zF4J-IIdu3vQb1Vot46atuknu1aIbI,128883
+ScriptCollection/ScriptCollectionCore.py,sha256=IAMV4HvN-BBiMRgMerxDtsgIb-f3l8cGaVUv2shcnrM,86233
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=Zg_aBGA5K8oA06l79HYT_Tm7lERE1Ym3JLtqUVyT7ys,129034
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.90.dist-info/METADATA,sha256=6CwhvPJr267_V1E-nC27j0dK_eqNJ6F7z5XS-iO7G38,7864
-ScriptCollection-3.3.90.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.90.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.90.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.90.dist-info/RECORD,,
+ScriptCollection-3.3.91.dist-info/METADATA,sha256=F0pUTHib0IqOb5W6LgtS6ISu45kqfUyZagtf258sKTs,7864
+ScriptCollection-3.3.91.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.91.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.91.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.91.dist-info/RECORD,,
```

