# Comparing `tmp/vmware-cloud-foundation-health-monitoring-1.0.0.tar.gz` & `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.0.0.tar", last modified: Fri Apr 21 22:48:27 2023, max compression
+gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.tar", last modified: Wed May 17 00:05:06 2023, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-1.0.0.tar` & `vmware-cloud-foundation-health-monitoring-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.538074 vmware-cloud-foundation-health-monitoring-1.0.0/
--rw-rw-rw-   0        0        0    10974 2023-04-21 22:48:27.538074 vmware-cloud-foundation-health-monitoring-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10172 2023-04-20 21:24:20.000000 vmware-cloud-foundation-health-monitoring-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-18 00:06:38.000000 vmware-cloud-foundation-health-monitoring-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1041 2023-04-21 22:48:27.584952 vmware-cloud-foundation-health-monitoring-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.475584 vmware-cloud-foundation-health-monitoring-1.0.0/source/
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.491198 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-02-28 19:45:01.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.491198 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Notifications.json
--rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    10154 2023-03-02 19:11:15.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-02-28 19:45:01.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.506823 vmware-cloud-foundation-health-monitoring-1.0.0/source/examples/
--rw-rw-rw-   0        0        0        0 2023-02-28 19:45:01.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-04-21 22:34:42.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.506823 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/
--rw-rw-rw-   0        0        0        0 2023-02-28 19:45:01.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/__init__.py
--rw-rw-rw-   0        0        0     3127 2023-04-14 21:40:15.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.506823 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-02-16 16:27:50.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-04-14 21:40:15.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/env.json
--rw-rw-rw-   0        0        0    68946 2023-04-14 21:40:15.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.506823 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/
--rw-rw-rw-   0        0        0     5862 2023-02-28 00:30:14.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     4336 2023-02-27 23:50:56.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     3042 2023-03-02 00:09:32.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     7160 2023-02-16 16:27:50.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-02-16 16:27:50.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 22:48:27.538074 vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    10974 2023-04-21 22:48:27.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2023-04-21 22:48:27.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 22:48:27.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 22:48:27.000000 vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/
+-rw-rw-rw-   0        0        0    10974 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10172 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1041 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.776855 vmware-cloud-foundation-health-monitoring-1.1.0/source/
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.792477 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.839357 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Notifications.json
+-rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    10147 2023-05-16 19:30:01.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.839357 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.870606 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.870606 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1456 2023-05-16 23:55:35.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/env.json
+-rw-rw-rw-   0        0        0    70917 2023-05-16 23:58:10.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.901856 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/
+-rw-rw-rw-   0        0        0     5862 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     4438 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     3042 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     7362 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    10974 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/README.md` & `vmware-cloud-foundation-health-monitoring-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/setup.cfg` & `vmware-cloud-foundation-health-monitoring-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
-00000040: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
+00000040: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
 00000050: 7574 686f 7220 3d20 4268 756d 6974 7261  uthor = Bhumitra
 00000060: 204e 6167 6172 0d0a 6175 7468 6f72 5f65   Nagar..author_e
 00000070: 6d61 696c 203d 2062 6e61 6761 7240 766d  mail = bnagar@vm
 00000080: 7761 7265 2e63 6f6d 0d0a 6465 7363 7269  ware.com..descri
 00000090: 7074 696f 6e20 3d20 5079 7468 6f6e 204d  ption = Python M
 000000a0: 6f64 756c 6520 666f 7220 564d 7761 7265  odule for VMware
 000000b0: 2043 6c6f 7564 2046 6f75 6e64 6174 696f   Cloud Foundatio
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Dashboards.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Dashboards.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Notifications.json` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Notifications.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Supermetrics.json` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Supermetrics.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/artifacts/vSAN/Views.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Views.zip`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
-Zip file size: 10154 bytes, number of entries: 1
--rw-a--     2.0 fat   234927 t- defN 23-Mar-02 19:10 content.xml
-1 file, 234927 bytes uncompressed, 10034 bytes compressed:  95.7%
+Zip file size: 10147 bytes, number of entries: 1
+-rw-a--     2.0 fat   234937 t- defN 23-May-16 20:29 content.xml
+1 file, 234937 bytes uncompressed, 10027 bytes compressed:  95.7%
```

#### content.xml

##### content.xml

```diff
@@ -3885,15 +3885,15 @@
                   <Property name="addTimestampAsColumn" value="false"/>
                   <Property name="isShowRelativeTimestamp" value="false"/>
                 </Value>
               </Item>
               <Item>
                 <Value>
                   <Property name="objectType" value="RESOURCE"/>
-                  <Property name="attributeKey" value="HRM Snapshot Status|latest"/>
+                  <Property name="attributeKey" value="HRM Snapshot Status|date_taken"/>
                   <Property name="isStringAttribute" value="false"/>
                   <Property name="adapterKind" value="VMWARE"/>
                   <Property name="resourceKind" value="VirtualMachine"/>
                   <Property name="rollUpType" value="NONE"/>
                   <Property name="rollUpCount" value="0"/>
                   <Property name="transformations">
                     <List>
@@ -4101,15 +4101,15 @@
                   <Property name="addTimestampAsColumn" value="false"/>
                   <Property name="isShowRelativeTimestamp" value="false"/>
                 </Value>
               </Item>
               <Item>
                 <Value>
                   <Property name="objectType" value="RESOURCE"/>
-                  <Property name="attributeKey" value="HRM Backup Status|date"/>
+                  <Property name="attributeKey" value="HRM Backup Status|date_taken"/>
                   <Property name="isStringAttribute" value="false"/>
                   <Property name="adapterKind" value="VMWARE"/>
                   <Property name="resourceKind" value="VirtualMachine"/>
                   <Property name="rollUpType" value="NONE"/>
                   <Property name="rollUpCount" value="0"/>
                   <Property name="transformations">
                     <List>
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/encrypt-passwords.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypt-passwords.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar
-# Date:   2023-02-01
-# Version: 1.0.0.1001
+# Date:   2023-04-01
+# Version: 1.1.0.1001
 # ===================================================================================================================
 #
 # Description:
 # Script to encrypt passwords for SDDC Manager and vRealize Operations credentials. Passwords are encrypted and saved
 # in an encrypted_pwds file and a key file in encrypted_files directory.
 #
 # Example:
@@ -35,41 +35,41 @@
             data = json.load(df)
         return data
 
     def generate_encrypted_pwds(self):
         env_info = self.read_data('env.json')
         vrops_user = env_info["vrops"]["user"]
         sddc_manager_user = env_info["sddc_manager"]["user"]
-        sddc_manager_root = 'root'
+        sddc_manager_local_user = env_info["sddc_manager"]["local_user"]
         vrops_pwd = maskpass.askpass(prompt=f"Enter password for vRealize Operations user - {vrops_user}: ", mask="*")
         sddc_manager_user_pwd = maskpass.askpass(prompt=f"Enter password for SDDC Manager user - {sddc_manager_user}: ",
                                                  mask="*")
-        sddc_manager_root_pwd = maskpass.askpass(prompt=f"Enter password for SDDC Manager user - "
-                                                        f"{sddc_manager_root}: ", mask="*")
+        sddc_manager_vcf_pwd = maskpass.askpass(prompt=f"Enter password for SDDC Manager local user - "
+                                                        f"{sddc_manager_local_user}: ", mask="*")
 
         # generate key and write to file
         key = Fernet.generate_key()
         with open(os.path.join('encrypted_files', 'key'), "wb") as f:
             f.write(key)
 
         # encrypt and write to file
         rKey = Fernet(key)
         bvrops_pwd = bytes(vrops_pwd, 'utf-8')
         enc_vrops_pwd = rKey.encrypt(bvrops_pwd)
 
         bsddc_user = bytes(sddc_manager_user_pwd, 'utf-8')
         enc_sddc_user = rKey.encrypt(bsddc_user)
 
-        bsddc_root = bytes(sddc_manager_root_pwd, 'utf-8')
-        env_sddc_root = rKey.encrypt(bsddc_root)
+        bsddc_local_user = bytes(sddc_manager_vcf_pwd, 'utf-8')
+        env_sddc_local_user = rKey.encrypt(bsddc_local_user)
 
         with open(os.path.join('encrypted_files', 'encrypted_pwds'), "wb") as ep:
             ep.write(enc_vrops_pwd + b'\n')
             ep.write(enc_sddc_user + b'\n')
-            ep.write(env_sddc_root)
+            ep.write(env_sddc_local_user)
 
         print(f'Encrypted Password files saved to {os.path.abspath("encrypted_files")}')
 
 
 if __name__ == "__main__":
     ep = EncryptPasswords()
     ep.generate_encrypted_pwds()
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/env.json` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/env.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888888888888889%*

 * *Differences: {"'sddc_manager'": "{'local_user': 'vcf'}"}*

```diff
@@ -21,14 +21,15 @@
     "log_level": "INFO",
     "log_retention_in_days": 30,
     "nsx_adapterKind": "NSXTAdapter",
     "nsx_resourceKind": "NSXTAdapterInstance",
     "pod_resourceKind": "Pod",
     "sddc_manager": {
         "fqdn": "sfo-vcf01.sfo.rainpole.io",
+        "local_user": "vcf",
         "user": "svc-hrm-vcf@sfo.rainpole.io"
     },
     "vm_resourceKind": "VirtualMachine",
     "vrops": {
         "fqdn": "xint-vrops01.rainpole.io",
         "user": "svc-hrm-vrops@sfo.rainpole.io@vIDMAuthSource"
     }
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/send-data-to-vrops.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/send-data-to-vrops.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,40 @@
 # WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar, Sowjanya V
-# Date:   2023-01-01
-# Version: 1.0.0.1001
+# Date:   2023-05-04
+# Version: 1.1.0.1001
 # ===================================================================================================================
 #
 # Description:
 # The send-data-to-vrops.py script receives the operational health data as JSON from SOS utility and supporting
 # Powershell modules and then sends it to objects in vRealize Operations as custom metrics for use in dashboards
 # to monitor the platform's health.
 #
-# Example:
-# python send-data-to-vrops.py
+# Change Log:
+# ---------------------------------------------------------------------------------------
+#    Version - Description
+# 1.1.0.1002 - chore: code cleanup
+# 1.1.0.1001 - bug: [HRM] Date on Backups and Snapshot dashboard shown incorrectly #50
+# 1.1.0.1001 - artifacts_update: Updated views for backup and snapshots to address issue #50
+# 1.1.0.1001 - feat: [HRM] Remove SDDC Manager root password from Python module #38
+# 1.1.0.1000 - feat: [HRM] Update project structure to host module on PyPI
+# ---------------------------------------------------------------------------------------
+# 1.0.0.1002 - bug: [HRM] Exception while sending Backup status data to vROps #48
 #
 # Example:
 # python send-data-to-vrops.py [-options]
 #
-# Options:
-# -np : Gets the data and saves it JSON files but will not send the data to vrops
+# [Options]:
+# -np : Retrieves the health data from SOS Utility and Powershell cmdlets and saves it JSON files.
+# It will not send the data to vRealize Operations
 
 
 import argparse
 import nagini
 import requests
 import json
 import os
@@ -42,19 +51,18 @@
 from cryptography.fernet import Fernet
 
 
 def push_handler(func):
     def inner_function(*args, **kwargs):
         try:
             func(*args, **kwargs)
-            args[0].logger.info("############################################################################")
+            args[0].logger.info('############################################################################')
         except Exception as e:
-            args[0].logger.info('Exception occurred. Details - ')
-            args[0].logger.info(e)
-
+            args[0].logger.error('Exception occurred. Details - ')
+            args[0].logger.error(e)
     return inner_function
 
 
 class PushDataVrops:
 
     def __init__(self, args):
         os.chdir(os.path.dirname(os.path.abspath(__file__)))
@@ -65,15 +73,15 @@
         log_level = env_info["log_level"]
         self.logger = LogUtility.get_logger(log_level)
 
         # set env
         requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
         self.logger.info('Gathering environment info..')
         self.logger.info(f'script started in path - {os.getcwd()}')
-        self.logger.info(f"change current working directory to - {os.path.dirname(__file__)}")
+        self.logger.info(f'change current working directory to - {os.path.dirname(__file__)}')
         self.logger.info(os.getcwd())
         self.logger.info(f'Log files located at - {self.logger.test_log_folder}')
 
         # set script options
         self.push_to_vrops = args.push_data
 
         # read env.json info
@@ -99,47 +107,48 @@
 
         self.vrops_fqdn = env_info["vrops"]["fqdn"]
         self.vrops_passwd = None
         self.vrops_user = env_info["vrops"]["user"]
         self.sddc_manager_fqdn = env_info["sddc_manager"]["fqdn"]
         self.sddc_manager_pwd = None
         self.sddc_manager_user = env_info["sddc_manager"]["user"]
-        self.sddc_manager_root_pwd = None
+        self.sddc_manager_local_user = env_info["sddc_manager"]["local_user"]
+        self.sddc_manager_local_pwd = None
 
         # set status codes
         self.codes = {'green': 0, 'yellow': 1, 'red': 2, 'NA': 1, 'skipped': 0}
 
         # resource inventory object
         self.resource_inventory = {}
 
         try:
             self.log_retention = int(env_info["log_retention_in_days"])
-            self.logger.info(f'Performing older logs cleanup from location '
+            self.logger.info(f'Cleaning up older logs from location: '
                              f'{os.path.dirname(self.logger.test_log_folder)}')
-            self.logger.info(f'deleting logs older than {self.log_retention} days')
+            self.logger.info(f'Deleting logs older than {self.log_retention} days')
             FolderUtility.delete_logs_older_than_days(self.log_retention, self.logger)
         except Exception as e:
-            self.logger.info('Exception occurred while deleting older logs')
-            self.logger.info(e)
+            self.logger.error('Exception occurred while deleting older logs')
+            self.logger.error(e)
 
         self.decrypt_pwds()
 
         # get vrops nagini client
         self.vrops = nagini.Nagini(host=self.vrops_fqdn, user_pass=(self.vrops_user, self.vrops_passwd))
 
-        self.logger.info('Fetching data from VMware.Cloudfoundation.Reporting cmdlets...')
+        self.logger.info('Fetching data from VMware.CloudFoundation.Reporting cmdlets...')
         self.get_data_from_reporting_module()
 
-        self.logger.info('Fetching data from SOS tool which runs on SDDC Manager...')
-        self.logger.info('This can take between 15 to 90 min depending on the size of your environment. '
+        self.logger.info('Fetching data from SOS Utility on SDDC Manager...')
+        self.logger.info('This can take 15~90 min (or even more) depending on the size of your environment. '
                          'Please wait....')
         self.data = self.get_sos_data_from_sddc_manager()
 
         if not self.data:
-            self.logger.info("Unable to get SOS data from SDDC Manager")
+            self.logger.error("Unable to get data from SOS Utility on SDDC Manager")
 
     def decrypt_pwds(self):
         # read encrypted pwd and convert into byte
         with open(os.path.join('encrypted_files', 'encrypted_pwds')) as f:
             pwds = []
             for line in f:
                 pwds.append(bytes(line, 'utf-8'))
@@ -147,45 +156,45 @@
         with open(os.path.join('encrypted_files', 'key')) as f:
             key = ''.join(f.readlines())
             keybyt = bytes(key, 'utf-8')
 
         fkey = Fernet(keybyt)
         self.vrops_passwd = fkey.decrypt(pwds[0]).decode()
         self.sddc_manager_pwd = fkey.decrypt(pwds[1]).decode()
-        self.sddc_manager_root_pwd = fkey.decrypt(pwds[2]).decode()
+        self.sddc_manager_local_pwd = fkey.decrypt(pwds[2]).decode()
 
     def get_resource_mapping_info(self):
         esx_res = self.match_resources(self.esx_resource_kind, self.esx_adapter_kind)
-        self.logger.info(f"ESX Resource mapping info - {esx_res}, size {len(esx_res)}")
+        self.logger.info(f'ESX Resource mapping info - {esx_res}, size {len(esx_res)}')
 
         nsx_res = self.match_resources(self.nsx_resource_kind, self.nsx_adapter_kind)
-        self.logger.info(f"NSX Resource mapping info - {nsx_res},  size {len(nsx_res)}")
+        self.logger.info(f'NSX Resource mapping info - {nsx_res},  size {len(nsx_res)}')
 
         vm_res = self.match_resources(self.vm_resource_kind, self.adapter_kind)
-        self.logger.info(f"VM Resource mapping info - {vm_res},  size {len(vm_res)}")
+        self.logger.info(f'VM Resource mapping info - {vm_res},  size {len(vm_res)}')
 
         pod_res = self.match_resources(self.pod_resource_kind, self.adapter_kind)
-        self.logger.info(f"Pod Resource mapping info - {pod_res},  size {len(pod_res)}")
+        self.logger.info(f'Pod Resource mapping info - {pod_res},  size {len(pod_res)}')
 
         cluster_res = self.match_resources(self.cluster_resource_kind, self.adapter_kind)
-        self.logger.info(f"Cluster Resource mapping info - {cluster_res},  size {len(cluster_res)}")
+        self.logger.info(f'Cluster Resource mapping info - {cluster_res},  size {len(cluster_res)}')
 
         self.resource_inventory = {**esx_res, **nsx_res, **vm_res, **cluster_res, **pod_res}
-        self.logger.info(f'Total number of resources in inventory = {len(self.resource_inventory)}')
-        self.logger.info(f'Number of esx resources - {len(esx_res)} ')
-        self.logger.info(f'Number of nsx resources - {len(nsx_res)} ')
-        self.logger.info(f'Number of vm resources - {len(vm_res)} ')
-        self.logger.info(f'Number of cluster resources  - {len(cluster_res)} ')
-        self.logger.info(f'Number of pod resources  - {len(pod_res)} ')
+        self.logger.info(f'Total number of resources in inventory: {len(self.resource_inventory)}')
+        self.logger.info(f'Number of esx resources: {len(esx_res)} ')
+        self.logger.info(f'Number of nsx resources: {len(nsx_res)} ')
+        self.logger.info(f'Number of vm resources: {len(vm_res)} ')
+        self.logger.info(f'Number of cluster resources: {len(cluster_res)} ')
+        self.logger.info(f'Number of pod resources: {len(pod_res)} ')
 
         total_len = len(esx_res) + len(nsx_res) + len(vm_res) + len(cluster_res) + len(pod_res)
 
-        self.logger.info(f'TOTAL resources (adding 5 categories above) = {total_len}')
+        self.logger.info(f'Total resources (adding all categories above): {total_len}')
         if total_len != len(self.resource_inventory):
-            self.logger.warn(f'It seems there is a possibility of duplicate entries in the inventory, please check')
+            self.logger.warn(f'There are duplicate resources in the inventory, please check.')
         return
 
     def backup_existing_file(self, data_file):
         backup_name = datetime.datetime.now().strftime('health-results_%H_%M_%d_%m_%Y.json')
         # remove existing file health_data_file
         if not os.path.exists('backup'):
             self.logger.info('creating backup directory')
@@ -198,47 +207,49 @@
         modules_without_root = ['Publish-BackupStatus',
                                 'Publish-NsxtTransportNodeStatus',
                                 'Publish-NsxtTransportNodeTunnelStatus',
                                 'Publish-NsxtTier0BgpStatus',
                                 'Publish-SnapshotStatus',
                                 'Publish-ComponentConnectivityHealthNonSOS']
 
-        without_root_cmd = f'-server {self.sddc_manager_fqdn} -user {self.sddc_manager_user} ' \
-                           f'-pass {self.sddc_manager_pwd} -allDomains -outputJson {self.logger.test_log_folder}'
+        without_local_user_cmd = f'-server {self.sddc_manager_fqdn} -user {self.sddc_manager_user} ' \
+                                 f'-pass {self.sddc_manager_pwd} -allDomains -outputJson {self.logger.test_log_folder}'
         request_token_cmd = f'Request-VCFToken -fqdn {self.sddc_manager_fqdn} -username {self.sddc_manager_user} ' \
                             f'-password {self.sddc_manager_pwd}'
-        publish_nsx_cmd = 'Publish-NsxtHealthNonSOS ' + without_root_cmd
+        publish_nsx_cmd = 'Publish-NsxtHealthNonSOS ' + without_local_user_cmd
 
         combined_cmd = request_token_cmd + ' ; ' + publish_nsx_cmd
         psu.execute_ps_cmd(combined_cmd)
 
-        # module requiring sddc root user
-        psu.execute_ps_cmd(f'Publish-StorageCapacityHealth {without_root_cmd} -rootPass {self.sddc_manager_pwd}')
+        # module requiring sddc local user
+        psu.execute_ps_cmd(f'Publish-StorageCapacityHealth {without_local_user_cmd} '
+                           f' -localUser {self.sddc_manager_local_user}'
+                           f' -localPass {self.sddc_manager_local_pwd}')
 
         for module in modules_without_root:
-            psu.execute_ps_cmd(f'{module} {without_root_cmd}')
+            psu.execute_ps_cmd(f'{module} {without_local_user_cmd}')
 
         self.logger.info(f'Generated JSON files for Publish-* cmdlets in location {self.logger.test_log_folder}')
 
     # TODO: change this function
     def get_sos_data_from_sddc_manager(self):
         data = None
         dest = os.path.join(self.logger.test_log_folder, self.data_file)
 
         sosrest = SosRest(host=self.sddc_manager_fqdn, user=self.sddc_manager_user,
                           password=self.sddc_manager_pwd, logger=self.logger)
         sosrest.get_auth_token()
-        id = sosrest.start_health_checks_op()
-        sosrest.get_health_checks_status(id)
-        sosrest.get_health_check_bundle(id, path=self.logger.test_log_folder)
+        request_id = sosrest.start_health_checks_op()
+        sosrest.get_health_checks_status(request_id)
+        sosrest.get_health_check_bundle(request_id, path=self.logger.test_log_folder)
 
         if os.path.exists(dest):
             data = self.read_data(os.path.join(dest))
         else:
-            self.logger.info(f'Unable to find {self.data_file} in {dest}')
+            self.logger.error(f'Unable to find {self.data_file} in {dest}')
         return data
 
     def match_resources(self, resource_kind, adapter_kind):
         try:
             resource_data = {}
             page = 0
             page_size = 1000
@@ -255,22 +266,22 @@
                 total_pages = total_pages - 1
                 page = page + 1
                 data = self.vrops.get_resources(resourceKind=resource_kind, adapterKindKey=adapter_kind,
                                                 pageSize=page_size, page=page)
                 for resource in data['resourceList']:
                     resource_data[resource['resourceKey']['name']] = resource['identifier']
 
-            self.logger.info(f'Resource inventory data from vrops for ResourceKind - {resource_kind} '
-                             f'and AdapterKind - {adapter_kind}')
+            self.logger.info(f'Resource inventory data from vROps for ResourceKind: {resource_kind} '
+                             f'and AdapterKind: {adapter_kind}')
             self.logger.info(resource_data)
 
             return resource_data
         except Exception as e:
-            self.logger.info(e)
-            self.logger.info("Unable to connect to vrops using given credentials")
+            self.logger.error(e)
+            self.logger.error('Unable to connect to vROps using given credentials')
             raise e
 
     def read_data(self, data_file):
         with open(data_file) as df:
             data = json.load(df)
         return data
 
@@ -278,20 +289,19 @@
         path = None
         for file in os.listdir(self.logger.test_log_folder):
             if file.endswith(file_name):
                 path = os.path.join(self.logger.test_log_folder, file)
                 break
         if not path:
             self.logger.info(f'Unable to find file ending with {file_name} in {self.logger.test_log_folder}')
-
         return path
 
     def push_data(self):
         self.get_resource_mapping_info()
-        self.logger.info("############################################################################")
+        self.logger.info('############################################################################')
 
         file_name = self.get_complete_json_file_name(self.backup_status_json)
         self.push_backup_status(file_name)
 
         file_name = self.get_complete_json_file_name(self.storagecapacityhealth_status_json)
         self.push_storagecapacityhealth_status(file_name)
 
@@ -301,15 +311,15 @@
         file_name = self.get_complete_json_file_name(self.component_connectivity_json)
         self.push_componentconnectivityhealth_status(file_name)
 
         file_name = self.get_complete_json_file_name(self.snapshot_status_json)
         self.push_snapshot_status(file_name)
 
         file_name = self.get_complete_json_file_name(self.nsxttier0bgp_status_json)
-        self.push_nsxttier0_backup_status(file_name)
+        self.push_nsxttier0_status(file_name)
 
         file_name = self.get_complete_json_file_name(self.nsxttransportnode_status_json)
         self.push_nsxt_transportnode_status(file_name)
 
         file_name = self.get_complete_json_file_name(self.nsxttntunnel_status_json)
         self.push_nsxt_tunnel_status(file_name)
 
@@ -323,46 +333,46 @@
             self.push_services()
             self.push_compute()
             self.push_vsan()
             self.push_connectivity()
             self.push_hw_compatibility()
             self.push_general()
         else:
-            self.logger.info('Skipping pushing SOS data to vrops. No data received')
+            self.logger.info('Skipping pushing SOS data to vROps. No data received.')
 
-        self.logger.info("###############################Script Complete############################################")
+        self.logger.info("############################### Script Complete ############################################")
         self.logger.info(f'Log files located at - {self.logger.test_log_folder}')
 
     def get_most_nested_dict(self, dictionary, parent_key=None, prev_keys=[]):
         for key, value in dictionary.items():
             if type(value) is dict:
                 parent_key = key
                 prev_keys.append(key)
                 yield from self.get_most_nested_dict(value, parent_key, prev_keys)
             else:
                 yield dictionary, parent_key, prev_keys
                 break
 
     def push_data_to_vrops(self, category, resource_id, hostname, metrics_payload_json):
         if category.lstrip().startswith("HRM"):
-            suc_log_msg = f"**********************Pushed '{category}' to vrops**********************"
-            fail_log_msg = f"**********************Unable to Push '{category}' to vrops**********************"
+            suc_log_msg = f'********************** Pushed "{category}" to vROps **********************'
+            fail_log_msg = f'********************** Unable to Push "{category}" to vROps**********************'
         else:
-            suc_log_msg = f"**********************Pushed 'SOS {category}' to vrops**********************"
-            fail_log_msg = f"**********************Unable to Push 'SOS {category}' to vrops**********************"
+            suc_log_msg = f'********************** Pushed "SOS {category}" to vROps **********************'
+            fail_log_msg = f'********************** Unable to Push "SOS {category}" to vROps **********************'
 
         if not resource_id:
-            self.logger.info(f'Cannot add data for {hostname}, resource id is {resource_id}')
-            self.logger.info(fail_log_msg)
+            self.logger.error(f'Unable to add data for Hostname: {hostname} | Resource id: {resource_id}')
+            self.logger.error(fail_log_msg)
         else:
             if self.push_to_vrops:
                 self.vrops.add_stats(metrics_payload_json, id=resource_id)
                 self.logger.info(suc_log_msg)
             else:
-                self.logger.info(f"********************** will not push '{category}' data to vrops******************")
+                self.logger.info(f"********************** Will not push '{category}' data to vROps ******************")
 
     @push_handler
     def push_general(self):
         category = "General"
         update_count = 0
         for d, parent_key, prev_keys in self.get_most_nested_dict(self.data[category]):
             if parent_key == "":
@@ -375,15 +385,15 @@
                     component, hostname = d['area'].split(':')
                 else:
                     hostname = d['area']
                     component = 'NA'
                 hostname = hostname.lstrip('*').lstrip().rstrip()
                 component = component.lstrip('*').rstrip().lstrip()
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
 
             resource_id = self.get_resource_id(hostname, resource_name)
 
             metrics_payload = {"stat-content": []}
             timestamp_raw = d['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
 
@@ -429,15 +439,15 @@
         update_count = 0
         for d, parent_key, prev_keys in self.get_most_nested_dict(self.data[category]):
             if parent_key == "":
                 continue
             component, hostname = d['area'].split(':')
             hostname = hostname.lstrip().rstrip()
             component = component.rstrip().lstrip()
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
 
             resource_id = self.get_resource_id(hostname, None)
 
             metrics_payload = {"stat-content": []}
             timestamp_raw = d['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
 
@@ -484,15 +494,15 @@
                 hostname = self.sddc_manager_fqdn
                 component = 'SDDCMANAGER'
             else:
                 component, hostname = d['area'].split(':')
                 hostname = hostname.lstrip().rstrip()
                 component = component.rstrip().lstrip()
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
 
             resource_id = self.get_resource_id(hostname, resource_name)
 
             metrics_payload = {"stat-content": []}
             timestamp_raw = d['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
 
@@ -634,15 +644,15 @@
         update_count = 0
         for key, value in self.data[category].items():
             for host, val in value.items():
                 component, hostname = val['area'].split(':')
                 hostname = hostname.lstrip().rstrip()
                 component = component.rstrip().lstrip()
                 resource_name = hostname.split(".")[0]
-                self.logger.info(f"hostname = {hostname}, component = {component}")
+                self.logger.info(f'Hostname: {hostname}, Component: {component}')
 
                 metrics_payload = {"stat-content": []}
 
                 timestamp_raw = val['timestamp']
                 timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
 
                 resource_id = self.get_resource_id(hostname, resource_name)
@@ -677,15 +687,15 @@
         update_count = 0
         for element in self.data[category]:
             for key, value in element.items():
                 component, hostname = value['area'].split(':')
                 hostname = hostname.lstrip().rstrip()
                 component = component.rstrip().lstrip()
                 resource_name = hostname.split(".")[0]
-                self.logger.info(f"hostname = {hostname}, component = {component}")
+                self.logger.info(f'Hostname: {hostname}, Component: {component}')
 
                 metrics_payload = {"stat-content": []}
 
                 timestamp_raw = value['timestamp']
                 timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
 
                 resource_id = self.get_resource_id(hostname, resource_name)
@@ -730,15 +740,15 @@
                     except Exception:
                         self.push_ntp_iterator(key, value)
                         category_orig = category
                         continue
                 else:
                     continue
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}")
+            self.logger.info(f'Hostname: {hostname}')
             metrics_payload = {"stat-content": []}
 
             timestamp_raw = value['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, val in value.items():
@@ -773,15 +783,15 @@
     @push_handler
     def push_dns_lookup(self, dns_type):
         category = "DNS lookup Status"
         update_count = 0
         for key, value in self.data[category][dns_type].items():
             hostname = key.rstrip()
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}")
+            self.logger.info(f'Hostname = {hostname}')
             metrics_payload = {"stat-content": []}
 
             timestamp_raw = value['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, val in value.items():
@@ -819,29 +829,29 @@
                     resource_id = res_id
                     break
         return resource_id
 
     def push_flat_struct(self, data_type, data_arr, key_var):
         update_count = 0
         category = f"HRM {data_type} Status"
-        self.logger.info(f"Pushing {data_type} status data to vrops")
+        self.logger.info(f'Pushing {data_type} status data to vROps')
         for arr_val in data_arr:
             data = arr_val
             user = None
             component = None
             if arr_val.get("User"):
                 user = arr_val["User"]
             if arr_val.get("Component"):
                 component = arr_val["Component"]
             if key_var:
                 hostname = data[key_var]
             else:
                 hostname = data["Resource"]
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
             metrics_payload = {"stat-content": []}
 
             timestamp = time.mktime(datetime.datetime.now().timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, v in arr_val.items():
                 if user:
@@ -870,15 +880,15 @@
             self.push_data_to_vrops(category, resource_id, hostname, metrics_payload_json)
             update_count = update_count + 1
         return update_count
 
     @push_handler
     def push_data_password(self):
         category = "Password Expiry Status"
-        self.logger.info('Pushing SOS password data to vrops')
+        self.logger.info('Pushing SOS password data to vROps')
         update_count = 0
         for key, value in self.data[category].items():
             hostname, user = key.split(':')
             hostname = hostname.rstrip()
             user = user.rstrip().lstrip()
             resource_name = hostname.split(".")[0]
             component = value['area'].split(":")[0].rstrip()
@@ -927,39 +937,49 @@
 
     @push_handler
     def push_backup_status(self, file_name):
         data_arr = self.read_data(file_name)
         update_count = 0
         category = "HRM Backup Status"
         data_type = "Backup"
-        self.logger.info(f"Pushing {data_type} status data to vrops")
+        self.logger.info(f'Pushing {data_type} status data to vROps')
 
-        for arr_val in data_arr:
-            data = arr_val
+        for data in data_arr:
             component = data["Component"]
             index_val = data["Resource"]
             hostname = data["Element"]
             if component == "NSX Manager":
                 statkey = f"HRM {data_type} Status:{index_val}"
             else:
                 statkey = f"HRM {data_type} Status"
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
             metrics_payload = {"stat-content": []}
             timestamp = time.mktime(datetime.datetime.now().timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
-            for k, v in arr_val.items():
+            for k, v in data.items():
                 if k.lower() == 'date':
+                    k = "date_taken"
                     if v:
-                        val = re.search(r"\d{10}", v)
-                        timestamp_raw = int(val.group())
-                        date_time = datetime.datetime.fromtimestamp(timestamp_raw)
-                        datetime_str = date_time.strftime("%b %d %H:%M:%S %Y GMT")
-                        v = datetime_str
+                        match = re.search(r"\d{10}", v)
+                        if match:
+                            timestamp_raw = int(match.group())
+                            parsed_date = datetime.datetime.fromtimestamp(timestamp_raw)
+                            datetime_str = parsed_date.strftime("%b %d %H:%M:%S %Y GMT")
+                            v = datetime_str
+                        else:
+                            match = re.search("\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}", v)
+                            if match:
+                                date_format = "%Y-%m-%dT%H:%M:%S"
+                                parsed_date = datetime.datetime.strptime(match.group(), date_format)
+                                datetime_str = parsed_date.strftime("%b %d %H:%M:%S %Y GMT")
+                                v = datetime_str
+                    else:
+                        v = ""
                 details = {
                     "statKey": f"{statkey}|{k.lower()}",
                     "timestamps": [int(timestamp * 1000)],
                     "values": [v]
                 }
                 metrics_payload["stat-content"].append(details)
                 if k.lower() == 'alert':
@@ -980,35 +1000,45 @@
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
     def push_snapshot_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM Snapshot Status"
         data_type = "Snapshot"
-        self.logger.info(f"Pushing {data_type} status data to vrops")
+        self.logger.info(f'Pushing {data_type} status data to vROps')
         update_count = 0
-        for arr_val in data_arr:
-            data = arr_val
+        for data in data_arr:
             component = data["Component"]
             hostname = data["Element"]
             resource_name = hostname.split(".")[0]
-            self.logger.info(f"hostname = {hostname}, component = {component}")
+            self.logger.info(f'Hostname: {hostname}, Component: {component}')
             metrics_payload = {"stat-content": []}
 
             timestamp = time.mktime(datetime.datetime.now().timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
-            for k, v in arr_val.items():
+            for k, v in data.items():
                 if k.lower() == 'latest':
+                    k = "date_taken"
                     if v:
-                        val = re.search(r"\d{10}", v)
-                        timestamp_raw = int(val.group())
-                        date_time = datetime.datetime.fromtimestamp(timestamp_raw)
-                        datetime_str = date_time.strftime("%b %d %H:%M:%S %Y GMT")
-                        v = datetime_str
+                        match = re.search(r"\d{10}", v)
+                        if match:
+                            timestamp_raw = int(match.group())
+                            parsed_date = datetime.datetime.fromtimestamp(timestamp_raw)
+                            datetime_str = parsed_date.strftime("%b %d %H:%M:%S %Y GMT")
+                            v = datetime_str
+                        else:
+                            match = re.search("\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}", v)
+                            if match:
+                                date_format = "%Y-%m-%dT%H:%M:%S"
+                                parsed_date = datetime.datetime.strptime(match.group(), date_format)
+                                datetime_str = parsed_date.strftime("%b %d %H:%M:%S %Y GMT")
+                                v = datetime_str
+                    else:
+                        v = ""
                 details = {
                     "statKey": f"HRM {data_type} Status|{k.lower()}",
                     "timestamps": [int(timestamp * 1000)],
                     "values": [v]
                 }
                 metrics_payload["stat-content"].append(details)
                 if k.lower() == 'alert':
@@ -1095,15 +1125,14 @@
                 for arr_val in data_arr:
                     data = arr_val
                     hostname = data[key_var]
                     resource_name = hostname.split(".")[0]
                     self.logger.info(f"hostname = {hostname}")
                     metrics_payload = {"stat-content": []}
 
-                    # timestamp_raw = value['timestamp']
                     timestamp = time.mktime(datetime.datetime.now().timetuple())
                     resource_id = self.get_resource_id(hostname, resource_name)
 
                     for k, v in arr_val.items():
                         index_val = arr_val["Datastore Name"]
                         statkey = f"HRM {data_type} Status:{index_val}"
                         details = {
@@ -1162,46 +1191,44 @@
                     self.logger.info(metrics_payload_json)
                     self.push_data_to_vrops(category, resource_id, hostname, metrics_payload_json)
 
                     update_count = update_count + 1
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
-    def push_nsxttier0_backup_status(self, file_name):
+    def push_nsxttier0_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM NSXT TIER0 BGP Backup Status"
-        self.logger.info('Pushing nsxt tier0 bgp backup status data to vrops')
+        self.logger.info('Pushing nsxt tier0 bgp status data to vROps')
         update_count = 0
         instance_hash = {}
 
         for arr_val in data_arr:
             instance_name = arr_val["NSX Manager"]
             instance_hash[instance_name] = 0
 
         for arr_val in data_arr:
             data = arr_val
             hostname = data["NSX Manager"]
             resource_name = hostname.split(".")[0]
             self.logger.info(f"hostname = {hostname}")
             metrics_payload = {"stat-content": []}
-
-            # timestamp_raw = value['timestamp']
             timestamp = time.mktime(datetime.datetime.now().timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, v in arr_val.items():
                 details = {
-                    "statKey": f"HRM NSXT TIER0 BGP Backup Status:{instance_hash[hostname]}|{k.lower()}",
+                    "statKey": f"{category}:{instance_hash[hostname]}|{k.lower()}",
                     "timestamps": [int(timestamp * 1000)],
                     "values": [v]
                 }
                 metrics_payload["stat-content"].append(details)
                 if k.lower() == 'alert':
                     details = {
-                        "statKey": f"HRM NSXT TIER0 BGP Backup Status:{instance_hash[hostname]}|alert_code",
+                        "statKey": f"{category}:{instance_hash[hostname]}|alert_code",
                         "timestamps": [int(timestamp * 1000)],
                         "data": [self.codes[v.lower()]] if v.lower() in self.codes else [self.codes['NA']]
                     }
                     metrics_payload["stat-content"].append(details)
 
             metrics_payload_json = json.dumps(metrics_payload)
 
@@ -1213,15 +1240,15 @@
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
     def push_nsxt_transportnode_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM NSXT Transport Node Status"
-        self.logger.info('Pushing nsxt transport node status data to vrops')
+        self.logger.info('Pushing nsxt transport node status data to vROps')
         update_count = 0
         instance_hash = {}
 
         for arr_val in data_arr:
             instance_name = arr_val["Resource"]
             instance_hash[instance_name] = 0
 
@@ -1261,15 +1288,15 @@
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
     def push_nsxt_tunnel_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM NSXT Tunnel Status"
-        self.logger.info('Pushing nsxt tunnel status data to vrops')
+        self.logger.info('Pushing nsxt tunnel status data to vROps')
         update_count = 0
         instance_hash = {}
 
         for arr_val in data_arr:
             instance_name = arr_val["Resource"]
             instance_hash[instance_name] = 0
 
@@ -1309,15 +1336,15 @@
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
     def push_nsxtcombinedhealthnonsos_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM NSXTCombinedHealth Status"
-        self.logger.info('Pushing NSXT Combined Health Status data to vrops')
+        self.logger.info('Pushing NSXT Combined Health Status data to vROps')
         update_count = 0
         instance_hash = {}
 
         for arr_val in data_arr:
             instance_name = arr_val["Resource"]
             instance_hash[instance_name] = 0
 
@@ -1356,15 +1383,15 @@
             instance_hash[hostname] += 1
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
     def push_data_certificates(self):
         category = "Certificates"
-        self.logger.info('Pushing SOS Certificate Health data to vrops')
+        self.logger.info('Pushing SOS Certificate Health data to vROps')
         update_count = 0
         for key, value in self.data[category]['Certificate Status'].items():
             for hostname, cert_data in value.items():
                 resource_name = hostname.split(".")[0]
                 self.logger.info(f"hostname = {hostname}")
 
                 resource_id = self.get_resource_id(hostname, resource_name)
@@ -1447,17 +1474,17 @@
         self.logger.info(f'Total object update requests = {update_count}')
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument("-e", "--env-json", default='env.json',
-                        help="path of env.json file. Default is in same folder as env.json")
+                        help="path of env.json file. Default is in same directory as this file")
     parser.add_argument('-p', '--push-data', dest='push_data', action='store_true',
-                        help="This is default option to push data to vrops")
+                        help="This is default option to send the data to vROps")
     parser.add_argument('-np', '--no-push-data', dest='push_data', action='store_false',
-                        help="Use this option if you do not want to push data to vrops")
+                        help="Use this option if you do not want to send the data to vROps")
     parser.set_defaults(push_data=True)
 
     args = parser.parse_args()
     pd = PushDataVrops(args)
     pd.push_data()
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/FolderUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/LogUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/LogUtility.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# Copyright 2022-2023 VMware, Inc.
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-# ===================================================================================================================
-# Created by:  Bhumitra Nagar - Senior Member of Technical Staff
-# Authors: Bhumitra Nagar
-# Date:   2023-02-01
-# Version: 1.0.0.1001
-# ===================================================================================================================
-#
-# Description:
-# Script implementing Logger class. Used for logging output to a file.
-
-import os
-import logging
-import traceback
-import inspect
-
-from utils.FolderUtility import FolderUtility
-
-"""Singleton class which wraps around python logger to log to file """
-
-class LogUtility(object):
-    __test_logger = None  # test logger which is object of this class
-    __logger = None  # python logger
-    test_log_folder = None
-
-    @staticmethod
-    def __get_call_info():
-        stack = inspect.stack()
-
-        # stack[1] gives previous function ('info' in this case)
-        # stack[2] gives before previous function and so on
-
-        fname = stack[2][1]  # filename
-        line_num = stack[2][2]  # line num
-
-        return os.path.basename(fname), line_num
-
-    def __init__(self, level='INFO'):
-        if LogUtility.__test_logger:
-            raise Exception('This is singleton class. Cannot instantiate again.')
-        else:
-            self.__logger = self._get_logger(level)
-            self.__logger.info("python logger ready")
-        LogUtility.__test_logger = self
-
-    def info(self, msg):
-        fname, line_num = self.__get_call_info()
-        msg = "[{}:{}] - {}".format(fname, line_num, msg)
-        self.__logger.info(msg)
-
-    def warn(self, msg):
-        fname, line_num = self.__get_call_info()
-        msg = "[{}:{}] - {}".format(fname, line_num, msg)
-        self.__logger.warn(msg)
-        self.__logger.warn(traceback.format_exc())
-
-    def error(self, msg, trace=True):
-        fname, line_num = self.__get_call_info()
-        msg = "[{}:{}] - {}".format(fname, line_num, msg)
-        self.__logger.error(f"Error - {msg}")
-        if trace and (traceback.format_exc() != 'NoneType: None\n'):
-            self.__logger.error(traceback.format_exc())
-
-    def debug(self, msg, trace=True):
-        fname, line_num = self.__get_call_info()
-        msg = "[{}:{}] - {}".format(fname, line_num, msg)
-        self.__logger.debug(f"Debug - {msg}")
-        if trace and (traceback.format_exc() != 'NoneType: None\n'):
-            self.__logger.debug(traceback.format_exc())
-
-    @staticmethod
-    def get_logger(log_level='INFO'):
-        if not LogUtility.__test_logger:
-            return LogUtility(level=log_level)
-        else:
-            return LogUtility.__test_logger
-
-    def _get_logger(self, level='INFO'):
-        """default python logger"""
-        accepted_levels = {'INFO': logging.INFO, 'DEBUG': logging.DEBUG}
-        if level.upper() not in accepted_levels:
-            raise Exception('INVALID LOG LEVEL SPECIFIED')
-        logging_format = '[%(asctime)s] %(levelname)s - %(message)s'
-        date_format = '%Y-%m-%d %H:%M:%S'
-        test_log_directory = FolderUtility.get_log_directory()
-        FolderUtility.make_directory(test_log_directory)
-        tmp_log_file_folder = os.path.join(test_log_directory, "send-data_")
-        self.test_log_folder = FolderUtility.make_director_with_timestamp(tmp_log_file_folder)
-        log_file_path = os.path.join(self.test_log_folder, "send-data-to-vrops.log")
-        logging.basicConfig(level=logging.NOTSET, format=logging_format, datefmt=date_format)
-        formatter = logging.Formatter(fmt=logging_format, datefmt=date_format)
-        handler = logging.FileHandler(log_file_path)
-        handler.setLevel(accepted_levels[level])
-        handler.setFormatter(formatter)
-        logger = logging.getLogger("HRM")
-        logger.addHandler(handler)
-        return logger
+# Copyright 2022-2023 VMware, Inc.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+# ===================================================================================================================
+# Created by:  Bhumitra Nagar - Senior Member of Technical Staff
+# Authors: Bhumitra Nagar
+# Date:   2023-02-01
+# Version: 1.0.0.1001
+# ===================================================================================================================
+#
+# Description:
+# Script implementing Logger class. Used for logging output to a file.
+
+import os
+import logging
+import traceback
+import inspect
+
+from utils.FolderUtility import FolderUtility
+
+"""Singleton class which wraps around python logger to log to file """
+
+class LogUtility(object):
+    __test_logger = None  # test logger which is object of this class
+    __logger = None  # python logger
+    test_log_folder = None
+
+    @staticmethod
+    def __get_call_info():
+        stack = inspect.stack()
+
+        # stack[1] gives previous function ('info' in this case)
+        # stack[2] gives before previous function and so on
+
+        fname = stack[2][1]  # filename
+        line_num = stack[2][2]  # line num
+
+        return os.path.basename(fname), line_num
+
+    def __init__(self, level='INFO'):
+        if LogUtility.__test_logger:
+            raise Exception('This is singleton class. Cannot instantiate again.')
+        else:
+            self.__logger = self._get_logger(level)
+            self.__logger.info("python logger ready")
+        LogUtility.__test_logger = self
+
+    def info(self, msg):
+        fname, line_num = self.__get_call_info()
+        msg = "[{}:{}] - {}".format(fname, line_num, msg)
+        self.__logger.info(msg)
+
+    def warn(self, msg):
+        fname, line_num = self.__get_call_info()
+        msg = "[{}:{}] - {}".format(fname, line_num, msg)
+        self.__logger.warn(msg)
+        self.__logger.warn(traceback.format_exc())
+
+    def error(self, msg, trace=True):
+        fname, line_num = self.__get_call_info()
+        msg = "[{}:{}] - {}".format(fname, line_num, msg)
+        self.__logger.error(f"Error - {msg}")
+        if trace and (traceback.format_exc() != 'NoneType: None\n'):
+            self.__logger.error(traceback.format_exc())
+
+    def debug(self, msg, trace=True):
+        fname, line_num = self.__get_call_info()
+        msg = "[{}:{}] - {}".format(fname, line_num, msg)
+        self.__logger.debug(f"Debug - {msg}")
+        if trace and (traceback.format_exc() != 'NoneType: None\n'):
+            self.__logger.debug(traceback.format_exc())
+
+    @staticmethod
+    def get_logger(log_level='INFO'):
+        if not LogUtility.__test_logger:
+            return LogUtility(level=log_level)
+        else:
+            return LogUtility.__test_logger
+
+    def _get_logger(self, level='INFO'):
+        """default python logger"""
+        accepted_levels = {'INFO': logging.INFO, 'DEBUG': logging.DEBUG}
+        if level.upper() not in accepted_levels:
+            raise Exception('INVALID LOG LEVEL SPECIFIED')
+        logging_format = '[%(asctime)s] %(levelname)s - %(message)s'
+        date_format = '%Y-%m-%d %H:%M:%S'
+        test_log_directory = FolderUtility.get_log_directory()
+        FolderUtility.make_directory(test_log_directory)
+        tmp_log_file_folder = os.path.join(test_log_directory, "send-data_")
+        self.test_log_folder = FolderUtility.make_director_with_timestamp(tmp_log_file_folder)
+        log_file_path = os.path.join(self.test_log_folder, "send-data-to-vrops.log")
+        logging.basicConfig(level=logging.NOTSET, format=logging_format, datefmt=date_format)
+        formatter = logging.Formatter(fmt=logging_format, datefmt=date_format)
+        handler = logging.FileHandler(log_file_path)
+        handler.setLevel(accepted_levels[level])
+        handler.setFormatter(formatter)
+        logger = logging.getLogger("HRM")
+        logger.addHandler(handler)
+        return logger
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/PSUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/main/utils/SosRest.py` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/SosRest.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-# Copyright 2022-2023 VMware, Inc.
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-# ===================================================================================================================
-# Created by:  Bhumitra Nagar - Senior Member of Technical Staff
-# Authors: Bhumitra Nagar
-# Date:   2023-02-01
-# Version: 1.0.0.1001
-# ===================================================================================================================
-#
-# Description:
-# Helper script to run health checks on SDDC Manager using SOS Utility and get the data. It saves it as
-# health-results.json in test log directory.
-
-
-import requests
-import time
-import os
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
-from pathlib import Path
-import tarfile
-import shutil
-import glob
-
-
-class SosRest(object):
-
-    def __init__(self, host, user, password, logger=None):
-        self.host = host
-        self.user = user
-        self.password = password
-        self.logger = logger
-        requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-        self.token = self.get_auth_token()
-
-        if not self.token:
-            raise Exception('Unable to get Authorization token from SDDC manager')
-
-    def get_auth_token(self):
-        headers = {
-            'Content-Type': 'application/json',
-        }
-
-        json_data = {
-            'username': self.user,
-            'password': self.password,
-        }
-
-        response = requests.post(f'https://{self.host}/v1/tokens', headers=headers, json=json_data, verify=False)
-        token = None
-        res = response.json()
-        # self.log_msg(res)
-        if response.status_code == 200:
-            token = res['accessToken']
-        return token
-
-    def start_health_checks_op(self):
-
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {self.token}'
-        }
-
-        json_data = {
-            "healthChecks": {
-                "certificateHealth": True,
-                "composabilityHealth": True,
-                "computeHealth": True,
-                "connectivityHealth": True,
-                "dnsHealth": True,
-                "generalHealth": True,
-                "hardwareCompatibilityHealth": True,
-                "ntpHealth": True,
-                "passwordHealth": True,
-                "servicesHealth": True,
-                "storageHealth": True
-            },
-            "options": {
-                "config": {
-                    "force": True,
-                    "skipKnownHostCheck": True
-                },
-                "include": {
-                    "summaryReport": True
-                }
-            },
-            "scope": {
-                "domains": [{
-                    "clusterNames": [""],
-                    "domainName": ""
-                }],
-                "includeAllDomains": True,
-                "includeFreeHosts": True
-            }
-        }
-
-        response = requests.post(f'https://{self.host}/v1/system/health-summary', headers=headers, json=json_data,
-                                 verify=False)
-        id = None
-        res = response.json()
-        self.log_msg(res)
-        self.log_msg(f'status code {response.status_code}')
-        if response.status_code == 202:
-            id = res['id']
-        if response.status_code == 409:
-            raise Exception(f'SOS Utility operation in progress - {res}')
-        return id
-
-    def log_msg(self, msg):
-        if self.logger:
-            self.logger.info(msg)
-        else:
-            print(msg)
-
-    def get_health_checks_status(self, id):
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {self.token}'
-        }
-
-        while True:
-            time.sleep(30)
-            response = requests.get(f'https://{self.host}/v1/system/health-summary/{id}', headers=headers, verify=False)
-            res = response.json()
-
-            self.log_msg(response)
-            if res['status'] == 'IN_PROGRESS':
-                self.log_msg('Health check bundle creation in progress...')
-                self.log_msg('Please wait for it to complete')
-                self.log_msg('Polling again in 30 seconds')
-                continue
-            elif res['status'] == 'COMPLETED_WITH_SUCCESS':
-                self.log_msg(f'Bundle created successfully - {res}')
-                break
-            else:
-                self.log_msg(f'Unexpected status code - response is - {res}')
-                break
-        return res
-
-    def get_health_check_bundle(self, id, path=None):
-        headers = {
-            'Content-Type': 'application/octet-stream',
-            'Authorization': f'Bearer {self.token}'
-        }
-
-        response = requests.get(f'https://{self.host}/v1/system/health-summary/{id}/data', headers=headers,
-                                verify=False)
-
-        self.logger.info(f'bundle response code - {response.status_code}')
-
-        if path:
-            if os.path.exists(path):
-                file_path = os.path.join(path, f'health-data-{id}.tar')
-            else:
-                raise Exception(f'Invalid location - {path} or folder doesnt exist')
-        else:
-            file_path = f'health-data-{id}.tar'
-
-        with open(file_path, 'wb') as f:
-            for chunk in response.iter_content(chunk_size=1024):
-                if chunk:
-                    f.write(chunk)
-
-        if os.path.exists(file_path):
-            self.log_msg('Extracting contents of bundle')
-            self.get_health_check_json_from_tar(file_path, path)
-
-    def get_health_check_json_from_tar(self, absfname, path=None):
-        fname = Path(absfname).name
-        foldername = fname.rstrip(".tar")
-        dst = path
-        if path is None:
-            path = os.getcwd()
-        path = os.path.join(path, foldername)
-        filepath = os.path.join(path, '**')
-        filepath = os.path.join(filepath, 'health-results.json')
-        tar = tarfile.open(absfname, "r:*")
-        tar.extractall(path)
-        tar.close()
-
-        for file in glob.glob(filepath, recursive=True):
-            if file:
-                self.log_msg(f"health-results.json file exists in the path {file}")
-                shutil.copy(file, dst)
-            else:
-                self.log_msg(f"health-results.json file doesn't exist in {fname}")
-
-
-if __name__ == "__main__":
-    host = 'sfo-vcf01.sfo.rainpole.io'
-    user = 'svc-hrm-vcf@sfo.rainpole.io'
-    password = '********'
-    sosrest = SosRest(host=host, user=user, password=password)
-    sosrest.get_auth_token()
-    time.sleep(5)
-    id = sosrest.start_health_checks_op()
-    if id:
-        sosrest.get_health_checks_status(id)
-        sosrest.get_health_check_bundle(id)
+# Copyright 2022-2023 VMware, Inc.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+# ===================================================================================================================
+# Created by:  Bhumitra Nagar - Senior Member of Technical Staff
+# Authors: Bhumitra Nagar
+# Date:   2023-02-01
+# Version: 1.0.0.1001
+# ===================================================================================================================
+#
+# Description:
+# Helper script to run health checks on SDDC Manager using SOS Utility and get the data. It saves it as
+# health-results.json in test log directory.
+
+
+import requests
+import time
+import os
+from requests.packages.urllib3.exceptions import InsecureRequestWarning
+from pathlib import Path
+import tarfile
+import shutil
+import glob
+
+
+class SosRest(object):
+
+    def __init__(self, host, user, password, logger=None):
+        self.host = host
+        self.user = user
+        self.password = password
+        self.logger = logger
+        requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
+        self.token = self.get_auth_token()
+
+        if not self.token:
+            raise Exception('Unable to get Authorization token from SDDC manager')
+
+    def get_auth_token(self):
+        headers = {
+            'Content-Type': 'application/json',
+        }
+
+        json_data = {
+            'username': self.user,
+            'password': self.password,
+        }
+
+        response = requests.post(f'https://{self.host}/v1/tokens', headers=headers, json=json_data, verify=False)
+        token = None
+        res = response.json()
+        # self.log_msg(res)
+        if response.status_code == 200:
+            token = res['accessToken']
+        return token
+
+    def start_health_checks_op(self):
+
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.token}'
+        }
+
+        json_data = {
+            "healthChecks": {
+                "certificateHealth": True,
+                "composabilityHealth": True,
+                "computeHealth": True,
+                "connectivityHealth": True,
+                "dnsHealth": True,
+                "generalHealth": True,
+                "hardwareCompatibilityHealth": True,
+                "ntpHealth": True,
+                "passwordHealth": True,
+                "servicesHealth": True,
+                "storageHealth": True
+            },
+            "options": {
+                "config": {
+                    "force": True,
+                    "skipKnownHostCheck": True
+                },
+                "include": {
+                    "summaryReport": True
+                }
+            },
+            "scope": {
+                "domains": [{
+                    "clusterNames": [""],
+                    "domainName": ""
+                }],
+                "includeAllDomains": True,
+                "includeFreeHosts": True
+            }
+        }
+
+        response = requests.post(f'https://{self.host}/v1/system/health-summary', headers=headers, json=json_data,
+                                 verify=False)
+        id = None
+        res = response.json()
+        self.log_msg(res)
+        self.log_msg(f'status code {response.status_code}')
+        if response.status_code == 202:
+            id = res['id']
+        if response.status_code == 409:
+            raise Exception(f'SOS Utility operation in progress - {res}')
+        return id
+
+    def log_msg(self, msg):
+        if self.logger:
+            self.logger.info(msg)
+        else:
+            print(msg)
+
+    def get_health_checks_status(self, id):
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.token}'
+        }
+
+        while True:
+            time.sleep(30)
+            response = requests.get(f'https://{self.host}/v1/system/health-summary/{id}', headers=headers, verify=False)
+            res = response.json()
+
+            self.log_msg(response)
+            if res['status'] == 'IN_PROGRESS':
+                self.log_msg('Health check bundle creation in progress...')
+                self.log_msg('Please wait for it to complete')
+                self.log_msg('Polling again in 30 seconds')
+                continue
+            elif res['status'] == 'COMPLETED_WITH_SUCCESS':
+                self.log_msg(f'Bundle created successfully - {res}')
+                break
+            else:
+                self.log_msg(f'Unexpected status code - response is - {res}')
+                break
+        return res
+
+    def get_health_check_bundle(self, id, path=None):
+        headers = {
+            'Content-Type': 'application/octet-stream',
+            'Authorization': f'Bearer {self.token}'
+        }
+
+        response = requests.get(f'https://{self.host}/v1/system/health-summary/{id}/data', headers=headers,
+                                verify=False)
+
+        self.logger.info(f'bundle response code - {response.status_code}')
+
+        if path:
+            if os.path.exists(path):
+                file_path = os.path.join(path, f'health-data-{id}.tar')
+            else:
+                raise Exception(f'Invalid location - {path} or folder doesnt exist')
+        else:
+            file_path = f'health-data-{id}.tar'
+
+        with open(file_path, 'wb') as f:
+            for chunk in response.iter_content(chunk_size=1024):
+                if chunk:
+                    f.write(chunk)
+
+        if os.path.exists(file_path):
+            self.log_msg('Extracting contents of bundle')
+            self.get_health_check_json_from_tar(file_path, path)
+
+    def get_health_check_json_from_tar(self, absfname, path=None):
+        fname = Path(absfname).name
+        foldername = fname.rstrip(".tar")
+        dst = path
+        if path is None:
+            path = os.getcwd()
+        path = os.path.join(path, foldername)
+        filepath = os.path.join(path, '**')
+        filepath = os.path.join(filepath, 'health-results.json')
+        tar = tarfile.open(absfname, "r:*")
+        tar.extractall(path)
+        tar.close()
+
+        for file in glob.glob(filepath, recursive=True):
+            if file:
+                self.log_msg(f"health-results.json file exists in the path {file}")
+                shutil.copy(file, dst)
+            else:
+                self.log_msg(f"health-results.json file doesn't exist in {fname}")
+
+
+if __name__ == "__main__":
+    host = 'sfo-vcf01.sfo.rainpole.io'
+    user = 'svc-hrm-vcf@sfo.rainpole.io'
+    password = '********'
+    sosrest = SosRest(host=host, user=user, password=password)
+    sosrest.get_auth_token()
+    time.sleep(5)
+    id = sosrest.start_health_checks_op()
+    if id:
+        sosrest.get_health_checks_status(id)
+        sosrest.get_health_check_bundle(id)
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.0.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

