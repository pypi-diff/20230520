# Comparing `tmp/pyloobins-0.1.5.tar.gz` & `tmp/pyloobins-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.5.tar", max compression
+gzip compressed data, was "pyloobins-0.1.6.tar", max compression
```

## Comparing `pyloobins-0.1.5.tar` & `pyloobins-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.5/LICENSE
--rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.5/LOOBins/GetFileInfo.yml
--rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.5/LOOBins/SetFile.yml
--rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.5/LOOBins/dscl.yml
--rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.5/LOOBins/ioreg.yml
--rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.5/LOOBins/last.yml
--rw-r--r--   0        0        0     1224 2023-05-01 23:30:07.410602 pyloobins-0.1.5/LOOBins/mdfind.yml
--rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.5/LOOBins/networksetup.yml
--rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.5/LOOBins/osascript.yml
--rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.5/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.5/LOOBins/screencapture.yml
--rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.5/LOOBins/security.yml
--rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.5/LOOBins/softwareupdate.yml
--rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.5/LOOBins/sysctl.yml
--rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.5/LOOBins/xattr.yml
--rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.5/README.md
--rw-r--r--   0        0        0      877 2023-05-02 22:58:45.096617 pyloobins-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.5/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     1538 2023-04-19 23:44:40.581452 pyloobins-0.1.5/src/pyloobins/cli.py
--rw-r--r--   0        0        0     3776 2023-05-02 22:58:45.096968 pyloobins-0.1.5/src/pyloobins/models.py
--rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.5/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2729 2023-04-23 17:34:43.219963 pyloobins-0.1.5/src/pyloobins/util.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.6/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.6/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.6/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.6/LOOBins/csrutil.yml
+-rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.6/LOOBins/ditto.yml
+-rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.6/LOOBins/dns-sd.yml
+-rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.6/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.6/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.6/LOOBins/last.yml
+-rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.6/LOOBins/lsregister.yml
+-rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.6/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.6/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.6/LOOBins/open.yml
+-rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.6/LOOBins/osacompile.yml
+-rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.6/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.6/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.6/LOOBins/plutil.yml
+-rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.6/LOOBins/profiles.yml
+-rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.6/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.6/LOOBins/security.yml
+-rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.6/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.6/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.6/LOOBins/tclsh.yml
+-rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.6/LOOBins/textutil.yml
+-rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.6/LOOBins/tmutil.yml
+-rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.6/LOOBins/xattr.yml
+-rw-r--r--   0        0        0      559 2023-05-09 23:38:24.844556 pyloobins-0.1.6/README.md
+-rw-r--r--   0        0        0     1212 2023-05-20 14:54:20.754666 pyloobins-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.6/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-20 14:54:20.754917 pyloobins-0.1.6/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.6/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.6/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2761 2023-05-20 14:54:20.755132 pyloobins-0.1.6/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pyloobins-0.1.6/PKG-INFO
```

### Comparing `pyloobins-0.1.5/LICENSE` & `pyloobins-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/GetFileInfo.yml` & `pyloobins-0.1.6/LOOBins/GetFileInfo.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/SetFile.yml` & `pyloobins-0.1.6/LOOBins/SetFile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/dscl.yml` & `pyloobins-0.1.6/LOOBins/dscl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/ioreg.yml` & `pyloobins-0.1.6/LOOBins/ioreg.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/last.yml` & `pyloobins-0.1.6/LOOBins/last.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/mdfind.yml` & `pyloobins-0.1.6/LOOBins/mdfind.yml`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,27 @@
     tactics:
       - Reconnaissance
       - Discovery
     tags:
       - bash
       - zsh
       - oneliner
+  - name: Use mdfind to search for apps to infect
+    description: Allows an attacker to determine if specific applications are installed and can be leveraged
+    code: set appId to do shell script "mdfind kMDItemCFBundleIdentifier = '" & bundleId & "'"
+    tactics:
+      - Reconnaissance
+      - Discovery
+      - Defense Evasion
+    tags:
+      - osascript
+      - XCSSET
 paths:
   - /usr/bin/mdfind
 detections:
   - name: No detections at time of publishing
     url: N/A
 resources:
   - name: '"Farming The Apple Orchards: Living off the Land Techniques" - Chris Ross & Cedric Owens'
     url: https://youtu.be/Snwh4mMe-Cg?t=45
+  - name: '"Zero-Day TCC bypass discovered in XCSSET malware" - Jaron Bradley'
+    url: https://www.jamf.com/blog/zero-day-tcc-bypass-discovered-in-xcsset-malware/
```

### Comparing `pyloobins-0.1.5/LOOBins/networksetup.yml` & `pyloobins-0.1.6/LOOBins/networksetup.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/osascript.yml` & `pyloobins-0.1.6/LOOBins/osascript.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/pbpaste.yml` & `pyloobins-0.1.6/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/screencapture.yml` & `pyloobins-0.1.6/LOOBins/screencapture.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/security.yml` & `pyloobins-0.1.6/LOOBins/security.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/softwareupdate.yml` & `pyloobins-0.1.6/LOOBins/softwareupdate.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/sysctl.yml` & `pyloobins-0.1.6/LOOBins/sysctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/LOOBins/xattr.yml` & `pyloobins-0.1.6/LOOBins/xattr.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/src/pyloobins/cli.py` & `pyloobins-0.1.6/src/pyloobins/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Model for CLI functions"""
 import os
 import sys
 
 import click
 
-from .util import make_template, normalize_file_name, validate_loobin
+from .util import get_loobins, make_template, normalize_file_name, validate_loobin
 
 
 @click.group()
 def cli():
-    """Create, manage, and validate LOOBin objects."""
+    """Create, validate, and view LOOBin objects."""
 
 
 @cli.command()
 @click.option(
     "--file",
     type=str,
     required=True,
     help="File location of the LOOBin YAML file to validate.",
 )
 def validate(file: str) -> None:
-    """Validate a LOOBin object."""
+    """Validate a LOOBin YAML file."""
     if validate_loobin(yml_path=file):
         print(f"LOOBin at {file} is valid.")
         sys.exit(0)
     else:
         print(f"LOOBin at {file} is NOT valid.")
         sys.exit(1)
 
@@ -33,26 +33,49 @@
 @click.option("--name", type=str, required=False, help="Enter the name of the binary")
 @click.option(
     "--path",
     type=str,
     required=False,
     help="Enter the path where you would like to create the template YAML file.",
 )
-def create_template(name: str, path: str) -> None:
-    """Create a new LOOBin template file."""
-    template = make_template().to_yaml()
+def create(name: str, path: str) -> None:
+    """Create a YAML template file for a new LOOBin."""
+    template = make_template(name=name).to_yaml()
     file_name = normalize_file_name(name) if name else "template"
     file_path = path if path and os.path.exists(path) else "./"
     if not os.path.exists(file_path):
         click.echo(
             f"The specified path did not exist. "
             f"Creating the {file_name}.yml file in the current directory."
         )
     with open(
         file=f"{file_path}{file_name}.yml", mode="w", encoding="utf-8"
     ) as out_file:
         out_file.write(template)
         out_file.close()
 
 
+@cli.command()
+@click.option("--name", type=str, required=True, help="Enter the name of the binary")
+@click.option(
+    "--path",
+    type=str,
+    required=False,
+    help="Enter the path where you would like to create the template YAML file.",
+)
+def get(name: str, path: str = "") -> None:
+    """Get a LOOBin object."""
+    if path:
+        loobins = get_loobins(path=path)
+    else:
+        loobins = get_loobins()
+
+    res = [loobin for loobin in loobins if loobin.name == name]
+
+    if len(res) == 0:
+        print(f"No LOOBin found for {name}.")
+    else:
+        print(res[0].json(indent=True, exclude_none=True))
+
+
 if __name__ == "__main__":
     sys.exit(cli())
```

### Comparing `pyloobins-0.1.5/src/pyloobins/models.py` & `pyloobins-0.1.6/src/pyloobins/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     """LOOBin base class"""
 
     name: str = Field(title="Name", description="Name of the LOOBin")
     author: str = Field(title="Author", description="Author of the LOOBin")
     short_description: str = Field(
         title="Short Description",
         description="A short description of the LOOBin."
-        "This will display in the LOOBin card list and the LOOBins website search results.",
+        "This will display in the LOOBin card list and the"
+        "LOOBins website search results.",
     )
     full_description: str = Field(
         title="Full Description",
         description="A full description of the LOOBin."
         "This will display on the LOOBin's single page.",
     )
     created: date = Field(title="Created", description="Date the LOOBin was created")
@@ -78,19 +79,33 @@
     )
     acknowledgements: Optional[List[str]] = Field(
         title="Acknowledgements", description="Acknowledgements for the LOOBin"
     )
 
     def combine_tactics(self) -> List[str]:
         """Returns a list of all tactics across all LOOBin example use cases"""
-        return list(dict.fromkeys([t for euc in self.example_use_cases for t in euc.tactics]))  # type: ignore
+        return list(
+            dict.fromkeys(
+                tactic
+                for euc in self.example_use_cases
+                if euc.tactics is not None
+                for tactic in euc.tactics
+            )
+        )
 
     def combine_tags(self) -> List[str]:
         """Returns a list of all tags across all LOOBin example use cases"""
-        return list(dict.fromkeys([t for euc in self.example_use_cases for t in euc.tags]))  # type: ignore
+        return list(
+            dict.fromkeys(
+                tag
+                for euc in self.example_use_cases
+                if euc.tags is not None
+                for tag in euc.tags
+            )
+        )
 
     def to_yaml(self, exclude_null: bool = True) -> str:
         """Convert a LOOBin object to a YAML string"""
         return yaml.dump(
             self.dict(exclude_none=exclude_null),
             Dumper=yaml.Dumper,
             sort_keys=False,
```

### Comparing `pyloobins-0.1.5/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.6/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.5/src/pyloobins/util.py` & `pyloobins-0.1.6/src/pyloobins/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         return True
     except Exception as exc:
         # TODO add more specific Exception handling
         print(exc)
         return False
 
 
-def make_template() -> LOOBin:
+def make_template(name: str = "") -> LOOBin:
     """Creates a template LOOBin object"""
     loobin_template = LOOBin(
-        name="Template",
+        name=name if name else "Template",
         short_description="A short description of the binary goes here.",
         full_description="A full length description of the binary goes here.",
         author="Enter your name or alias here.",
         created=date.today(),
         example_use_cases=[
             ExampleUseCase(
                 name="An Example Use Case",
```

### Comparing `pyloobins-0.1.5/PKG-INFO` & `pyloobins-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
@@ -18,10 +18,13 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/infosecB/LOOBins
 Description-Content-Type: text/markdown
 
 # LOOBins
+[https://loobins.io](https://loobins.io)
 
 **L**iving **O**ff the **O**rchard: macOS Binaries (LOOBins) is designed to provide detailed information on various built-in macOS binaries and how they can be used by threat actors for malicious purposes. This list does not include overlapping Unix binaries that are detailed in [GTFOBins](https://gtfobins.github.io).
 
+We are in active development and welcome contributions. Please see [our guidelines](https://github.com/infosecB/LOOBins/blob/main/CONTRIBUTING.md) if you are interesting in helping out!
+
```

