# Comparing `tmp/iphack-1.3.6.tar.gz` & `tmp/iphack-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphack-1.3.6.tar", last modified: Thu May 18 19:18:01 2023, max compression
+gzip compressed data, was "iphack-1.3.7.tar", last modified: Sat May 20 12:31:16 2023, max compression
```

## Comparing `iphack-1.3.6.tar` & `iphack-1.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:18:01.183580 iphack-1.3.6/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     5795 2023-05-18 18:56:47.000000 iphack-1.3.6/README.md
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/iphack/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.6/iphack/__init__.py
--rw-------   0 u0_a314  (10314) u0_a314  (10314)    44289 2023-05-18 19:17:41.000000 iphack-1.3.6/iphack/iphack.py
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/iphack.egg-info/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/SOURCES.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/dependency_links.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/requires.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/top_level.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-18 19:18:01.183580 iphack-1.3.6/setup.cfg
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-18 19:17:51.000000 iphack-1.3.6/setup.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.953552 iphack-1.3.7/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 12:31:16.953552 iphack-1.3.7/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     5913 2023-05-20 12:30:35.000000 iphack-1.3.7/README.md
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.949552 iphack-1.3.7/iphack/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.7/iphack/__init__.py
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)    44383 2023-05-20 12:30:53.000000 iphack-1.3.7/iphack/iphack.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.953552 iphack-1.3.7/iphack.egg-info/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/SOURCES.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/dependency_links.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/requires.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/top_level.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-20 12:31:16.953552 iphack-1.3.7/setup.cfg
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-20 12:30:46.000000 iphack-1.3.7/setup.py
```

### Comparing `iphack-1.3.6/PKG-INFO` & `iphack-1.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.6
+Version: 1.3.7
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -111,17 +111,18 @@
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
 
-# get domain IP behind CF
+# search IP
 >>> from iphack import *
->>> iphack.domain.ip("google.com")
+>>> iphack.search.ip("google.com")
+1.0.126.229 / 1.0.158.92 / 1.0.160.34 / 1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 / 1.0.247.243
 >>> 
 
 ```
 
 **Check Proxy**
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.6 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.7 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -43,29 +43,31 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> # get domain IP behind CF >>> from iphack import *
->>> iphack.domain.ip("google.com") >>> ``` **Check Proxy** ```python # check
-proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
-Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
-City : Los Angeles Country : United States Region : California Network :
-130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # search IP >>> from iphack import * >>>
+iphack.search.ip("google.com") 1.0.126.229 / 1.0.158.92 / 1.0.160.34 /
+1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 /
+1.0.247.243 >>> ``` **Check Proxy** ```python # check proxy >>> from iphack
+import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online #Online or
+Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los Angeles Country :
+United States Region : California Network : 130.41.52.0/22 Version : IPv4 >>>
+``` **Websites** ```python # Check amazon subdomains from iphack import ip
+ip.subdomains("amazon.com") # Check amazon directories from iphack import ip
+ip.directory("amazon.com") ``` **Inquiry** ```python # anonymous request from
+iphack import inquiry # request from url, using tor & fake user-agent >>> get =
+inquiry.get("https://api.ipify.org/") #method get >>> print(get.text)
+199.249.230.102 >>> post = inquiry.post("https://example.com") #method post put
+= inquiry.put("https://example.com") #method put delete = inquiry.delete
+("https://example.com") #method delete head = inquiry.head("https://
+example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.6/README.md` & `iphack-1.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -79,17 +79,18 @@
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
 
-# get domain IP behind CF
+# search IP
 >>> from iphack import *
->>> iphack.domain.ip("google.com")
+>>> iphack.search.ip("google.com")
+1.0.126.229 / 1.0.158.92 / 1.0.160.34 / 1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 / 1.0.247.243
 >>> 
 
 ```
 
 **Check Proxy**
 
 ```python
```

#### html2text {}

```diff
@@ -22,29 +22,31 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> # get domain IP behind CF >>> from iphack import *
->>> iphack.domain.ip("google.com") >>> ``` **Check Proxy** ```python # check
-proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
-Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
-City : Los Angeles Country : United States Region : California Network :
-130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # search IP >>> from iphack import * >>>
+iphack.search.ip("google.com") 1.0.126.229 / 1.0.158.92 / 1.0.160.34 /
+1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 /
+1.0.247.243 >>> ``` **Check Proxy** ```python # check proxy >>> from iphack
+import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online #Online or
+Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los Angeles Country :
+United States Region : California Network : 130.41.52.0/22 Version : IPv4 >>>
+``` **Websites** ```python # Check amazon subdomains from iphack import ip
+ip.subdomains("amazon.com") # Check amazon directories from iphack import ip
+ip.directory("amazon.com") ``` **Inquiry** ```python # anonymous request from
+iphack import inquiry # request from url, using tor & fake user-agent >>> get =
+inquiry.get("https://api.ipify.org/") #method get >>> print(get.text)
+199.249.230.102 >>> post = inquiry.post("https://example.com") #method post put
+= inquiry.put("https://example.com") #method put delete = inquiry.delete
+("https://example.com") #method delete head = inquiry.head("https://
+example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.6/iphack/iphack.py` & `iphack-1.3.7/iphack/iphack.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 red = '\033[31m'
 yellow = '\033[93m'
 lgreen = '\033[92m'
 clear = '\033[0m'
 bold = '\033[01m'
 cyan = '\033[96m'
-version = "1.3.6"
+version = "1.3.7"
 referer_list = ["https://www.google.com/", "https://www.youtube.com/", "https://www.twitter.com/", "https://www.discord.com/", "https://www.tiktok.com/", "https://www.instagram.com/", "https://check-host.net/", "https://github.com", "https://gitlab.com", "https://he1zen.rf.gd"]
 
 major = str(sys.version_info.major)
 minor = str(sys.version_info.minor)
 path = str(sys.exec_prefix+"/lib/python"+major+"."+minor+"/site-packages/iphack/")
 
 global log
@@ -362,37 +362,40 @@
                print("Https      : False")
                print("Google     : True")
                print("Country    : "+c_name)
                print("Checked    : "+last)
                print("Anonymity  : "+anonymity)
                print(" ")
 
-class domain:
+class search:
     def ip(*text:str):
         import requests, socket
         find = " ".join([str(m) for m in text])
         find = find.replace("https://", "")
         find = find.replace("http://", "")
         find = find.replace("/", "")
         find = find.replace(" ", "")
         get = requests.get("https://raw.githubusercontent.com/mishakorzik/mishakorzik.menu.io/master/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80/https.json").json()
         ip = str(get["mailip"])
         port = int(get["mailport"])
         check = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         check.connect((ip, port))
-        check.settimeout(5)
         find = str(find)
         check.sendall(bytes("get|domain,ip|info|"+find,'UTF-8'))
-        code = check.recv(256)
-        get = code.decode('utf-8')
-        if get == "-":
-            print("not found")
-        else:
-            get = get.replace(",", " / ")
-            print(get)
+        try:
+            check.settimeout(10)
+            code = check.recv(2048)
+            get = code.decode('utf-8')
+            if get == "-":
+                print("no results")
+            else:
+                get = get.replace(",", "/")
+                print(get)
+        except:
+            print("no results")
 
 class check:
     def proxy(ip, port):
         import requests
         proxies = {"http":"http://"+ip+":"+port}
         headers = {"User-Agent": ua.windows()}
         info = requests.get("https://ipapi.co/"+ip+"/json/", headers=headers).json()
```

### Comparing `iphack-1.3.6/iphack.egg-info/PKG-INFO` & `iphack-1.3.7/iphack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.6
+Version: 1.3.7
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -111,17 +111,18 @@
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
 
-# get domain IP behind CF
+# search IP
 >>> from iphack import *
->>> iphack.domain.ip("google.com")
+>>> iphack.search.ip("google.com")
+1.0.126.229 / 1.0.158.92 / 1.0.160.34 / 1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 / 1.0.247.243
 >>> 
 
 ```
 
 **Check Proxy**
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.6 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.7 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -43,29 +43,31 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> # get domain IP behind CF >>> from iphack import *
->>> iphack.domain.ip("google.com") >>> ``` **Check Proxy** ```python # check
-proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
-Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
-City : Los Angeles Country : United States Region : California Network :
-130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # search IP >>> from iphack import * >>>
+iphack.search.ip("google.com") 1.0.126.229 / 1.0.158.92 / 1.0.160.34 /
+1.0.161.31 / 1.0.164.79 / 1.0.167.84 / 1.0.167.205 / 1.0.168.165 / 1.0.169.41 /
+1.0.247.243 >>> ``` **Check Proxy** ```python # check proxy >>> from iphack
+import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online #Online or
+Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los Angeles Country :
+United States Region : California Network : 130.41.52.0/22 Version : IPv4 >>>
+``` **Websites** ```python # Check amazon subdomains from iphack import ip
+ip.subdomains("amazon.com") # Check amazon directories from iphack import ip
+ip.directory("amazon.com") ``` **Inquiry** ```python # anonymous request from
+iphack import inquiry # request from url, using tor & fake user-agent >>> get =
+inquiry.get("https://api.ipify.org/") #method get >>> print(get.text)
+199.249.230.102 >>> post = inquiry.post("https://example.com") #method post put
+= inquiry.put("https://example.com") #method put delete = inquiry.delete
+("https://example.com") #method delete head = inquiry.head("https://
+example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.6/setup.py` & `iphack-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iphack',  # should match the package folder
     packages=['iphack'],  # should match the package folder
-    version='1.3.6',  # important for updates
+    version='1.3.7',  # important for updates
     python_requires=">=3.4",
     license='Apache 2.0',  # should match your chosen license
     description='the most ideal tool for finding out information about IP, etc.',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='MishaKorzhik_He1Zen',
     author_email='developer.mishakorzhik@gmail.com',
```

