# Comparing `tmp/r0c-1.4.0.tar.gz` & `tmp/r0c-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r0c-1.4.0.tar", last modified: Wed Oct 12 21:48:19 2022, max compression
+gzip compressed data, was "r0c-1.4.1.tar", last modified: Fri May 19 22:46:06 2023, max compression
```

## Comparing `r0c-1.4.0.tar` & `r0c-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2022-10-12 21:48:19.546720 r0c-1.4.0/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-19 15:14:09.000000 r0c-1.4.0/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)      224 2022-10-12 21:48:19.000000 r0c-1.4.0/MANIFEST.in
--rw-r--r--   0 ed        (1000) ed        (1000)     6586 2022-10-12 21:48:19.542720 r0c-1.4.0/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     4149 2022-10-12 07:59:00.000000 r0c-1.4.0/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2022-10-12 21:48:19.542720 r0c-1.4.0/clients/
--rwxr-xr-x   0 ed        (1000) ed        (1000)     1002 2021-09-19 15:14:09.000000 r0c-1.4.0/clients/bash.sh
--rw-r--r--   0 ed        (1000) ed        (1000)     4617 2021-09-19 15:14:09.000000 r0c-1.4.0/clients/powershell.ps1
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2022-10-12 21:48:19.542720 r0c-1.4.0/docs/
--rw-r--r--   0 ed        (1000) ed        (1000)      333 2021-09-19 15:14:09.000000 r0c-1.4.0/docs/help-about.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2285 2022-10-12 21:17:15.000000 r0c-1.4.0/docs/help-commands.md
--rw-r--r--   0 ed        (1000) ed        (1000)      741 2022-10-12 21:17:46.000000 r0c-1.4.0/docs/help-hotkeys.md
--rw-r--r--   0 ed        (1000) ed        (1000)      161 2021-09-19 15:14:09.000000 r0c-1.4.0/docs/help-topics.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2507 2021-09-19 15:14:09.000000 r0c-1.4.0/docs/todo.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2022-10-12 21:48:19.542720 r0c-1.4.0/r0c/
--rw-r--r--   0 ed        (1000) ed        (1000)     2543 2022-08-31 21:02:50.000000 r0c-1.4.0/r0c/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    19314 2022-10-04 20:46:59.000000 r0c-1.4.0/r0c/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      213 2022-10-12 20:41:12.000000 r0c-1.4.0/r0c/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7609 2022-09-01 21:07:01.000000 r0c-1.4.0/r0c/chat.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2227 2022-09-01 21:50:46.000000 r0c-1.4.0/r0c/diag.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3546 2022-09-01 17:10:00.000000 r0c-1.4.0/r0c/inetcat.py
--rw-r--r--   0 ed        (1000) ed        (1000)    13899 2022-10-12 19:51:30.000000 r0c-1.4.0/r0c/itelnet.py
--rw-r--r--   0 ed        (1000) ed        (1000)   103535 2022-10-12 21:27:59.000000 r0c-1.4.0/r0c/ivt100.py
--rw-r--r--   0 ed        (1000) ed        (1000)    33752 2022-10-12 19:52:55.000000 r0c-1.4.0/r0c/user.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16927 2022-10-12 18:32:24.000000 r0c-1.4.0/r0c/util.py
--rw-r--r--   0 ed        (1000) ed        (1000)    19144 2022-09-01 21:49:52.000000 r0c-1.4.0/r0c/world.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2022-10-12 21:48:19.542720 r0c-1.4.0/r0c.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)     6586 2022-10-12 21:48:19.000000 r0c-1.4.0/r0c.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)      466 2022-10-12 21:48:19.000000 r0c-1.4.0/r0c.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2022-10-12 21:48:19.000000 r0c-1.4.0/r0c.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       43 2022-10-12 21:48:19.000000 r0c-1.4.0/r0c.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        4 2022-10-12 21:48:19.000000 r0c-1.4.0/r0c.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2022-10-12 21:48:19.546720 r0c-1.4.0/setup.cfg
--rwxr-xr-x   0 ed        (1000) ed        (1000)     4568 2022-07-03 22:07:27.000000 r0c-1.4.0/setup.py
+drwxr-xr-x   0 ed         (501) staff       (20)        0 2023-05-19 22:46:06.297123 r0c-1.4.1/
+-rw-r--r--   0 ed         (501) staff       (20)     1059 2023-05-17 19:09:23.000000 r0c-1.4.1/LICENSE
+-rw-r--r--   0 ed         (501) staff       (20)      224 2023-05-19 22:46:06.000000 r0c-1.4.1/MANIFEST.in
+-rw-r--r--   0 ed         (501) staff       (20)     6829 2023-05-19 22:46:06.296997 r0c-1.4.1/PKG-INFO
+-rw-r--r--   0 ed         (501) staff       (20)     4989 2023-05-17 19:09:23.000000 r0c-1.4.1/README.md
+drwxr-xr-x   0 ed         (501) staff       (20)        0 2023-05-19 22:46:06.293249 r0c-1.4.1/clients/
+-rwxr-xr-x   0 ed         (501) staff       (20)     1002 2023-05-17 19:09:23.000000 r0c-1.4.1/clients/bash.sh
+-rw-r--r--   0 ed         (501) staff       (20)     4617 2023-05-17 19:09:23.000000 r0c-1.4.1/clients/powershell.ps1
+drwxr-xr-x   0 ed         (501) staff       (20)        0 2023-05-19 22:46:06.293998 r0c-1.4.1/docs/
+-rw-r--r--   0 ed         (501) staff       (20)      333 2023-05-17 19:09:23.000000 r0c-1.4.1/docs/help-about.md
+-rw-r--r--   0 ed         (501) staff       (20)     2285 2023-05-17 19:09:23.000000 r0c-1.4.1/docs/help-commands.md
+-rw-r--r--   0 ed         (501) staff       (20)      741 2023-05-17 19:09:23.000000 r0c-1.4.1/docs/help-hotkeys.md
+-rw-r--r--   0 ed         (501) staff       (20)      161 2023-05-17 19:09:23.000000 r0c-1.4.1/docs/help-topics.md
+-rw-r--r--   0 ed         (501) staff       (20)     2507 2023-05-17 19:09:23.000000 r0c-1.4.1/docs/todo.md
+drwxr-xr-x   0 ed         (501) staff       (20)        0 2023-05-19 22:46:06.296189 r0c-1.4.1/r0c/
+-rw-r--r--   0 ed         (501) staff       (20)     2543 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/__init__.py
+-rw-r--r--   0 ed         (501) staff       (20)    19314 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/__main__.py
+-rw-r--r--   0 ed         (501) staff       (20)      212 2023-05-19 14:48:11.000000 r0c-1.4.1/r0c/__version__.py
+-rw-r--r--   0 ed         (501) staff       (20)     7609 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/chat.py
+-rw-r--r--   0 ed         (501) staff       (20)     2227 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/diag.py
+-rw-r--r--   0 ed         (501) staff       (20)     3546 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/inetcat.py
+-rw-r--r--   0 ed         (501) staff       (20)    13899 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/itelnet.py
+-rw-r--r--   0 ed         (501) staff       (20)   103535 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/ivt100.py
+-rw-r--r--   0 ed         (501) staff       (20)    33752 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/user.py
+-rw-r--r--   0 ed         (501) staff       (20)    16927 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/util.py
+-rw-r--r--   0 ed         (501) staff       (20)    19144 2023-05-17 19:09:23.000000 r0c-1.4.1/r0c/world.py
+drwxr-xr-x   0 ed         (501) staff       (20)        0 2023-05-19 22:46:06.296780 r0c-1.4.1/r0c.egg-info/
+-rw-r--r--   0 ed         (501) staff       (20)     6829 2023-05-19 22:46:06.000000 r0c-1.4.1/r0c.egg-info/PKG-INFO
+-rw-r--r--   0 ed         (501) staff       (20)      466 2023-05-19 22:46:06.000000 r0c-1.4.1/r0c.egg-info/SOURCES.txt
+-rw-r--r--   0 ed         (501) staff       (20)        1 2023-05-19 22:46:06.000000 r0c-1.4.1/r0c.egg-info/dependency_links.txt
+-rw-r--r--   0 ed         (501) staff       (20)       42 2023-05-19 22:46:06.000000 r0c-1.4.1/r0c.egg-info/entry_points.txt
+-rw-r--r--   0 ed         (501) staff       (20)        4 2023-05-19 22:46:06.000000 r0c-1.4.1/r0c.egg-info/top_level.txt
+-rw-r--r--   0 ed         (501) staff       (20)       38 2023-05-19 22:46:06.297161 r0c-1.4.1/setup.cfg
+-rwxr-xr-x   0 ed         (501) staff       (20)     4658 2023-05-17 19:11:09.000000 r0c-1.4.1/setup.py
```

### Comparing `r0c-1.4.0/LICENSE` & `r0c-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/PKG-INFO` & `r0c-1.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,15 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.4.0
+Version: 1.4.1
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
-Description: # `r0c` telnet server
-        
-        * retr0chat, irc-like chat service for superthin clients [(on PyPI)](https://pypi.org/project/r0c/)
-        * MIT-Licensed, 2018-01-07, ed @ irc.rizon.net
-        * **[windows telnet 360 noscope](https://ocv.me/r0c.webm)** <- good video
-        
-        ![screenshot of telnet connected to a r0c server](https://raw.githubusercontent.com/9001/r0c/master/docs/r0c.png)
-        
-        * download the latest release (standalone): **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
-        
-        ## summary
-        
-        imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
-        
-        retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
-        
-        * tries to be irssi
-        * zero dependencies on python 2.6, 2.7, 3.x
-        * supports telnet, netcat, /dev/tcp, TLS clients
-        * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
-        * fallbacks for inhumane conditions
-          * linemode
-          * no vt100 / ansi escape codes
-        
-        ## endorsements
-        
-        * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
-        
-        ## features
-        
-        irc-like:
-        * public channels with persistent history (pgup/pgdn)
-        * private messages (`/msg acidburn hey`)
-        * nick completion with `Tab ↹`
-        * notifications (bell/visual) on hilights and PMs
-        * command subset (`/nick`, `/join`, `/part`, `/names`, `/topic`, `/me`)
-        * inline message coloring, see `/help`
-        
-        technical:
-        * client behavior detection (echo, colors, charset, newline)
-        * message input with readline-like editing (arrow-left/right, home/end, backspace)
-          * history of sent messages (arrow-up/down)
-        * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
-        * fast enough; 1'000 clients @ 200 msgs/sec
-        
-        ## windows clients
-        
-        * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
-        * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
-        * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
-        
-        putty is the best option;
-        * the powershell client is OK and no longer spammy as of windows 10.0.15063 (win10 1703 / LTSC)
-        * windows-telnet has a bug (since win7) where [non-ascii letters occasionally render but usually dont](https://ocv.me/stuff/win10-telnet.webm)
-          * this is due to a buffer overflow in `telnet.exe`, so r0c will apply a rate-limit to avoid it
-          * looks like messages larger than 512 bytes end up messing with the unicode glyphs area? or something
-        
-        ## linux clients
-        
-        most to least recommended
-        
-        | client | example |
-        | :---   | :---    |
-        | telnet | `telnet r0c.int` |
-        | socat  | `socat -,raw,echo=0 tcp:r0c.int:531` |
-        | bash   | [mostly internals](https://github.com/9001/r0c/blob/master/clients/bash.sh) |
-        | netcat | `nc r0c.int 531` |
-        
-        you can even `exec 147<>/dev/tcp/r0c.int/531;cat<&147&while IFS= read -rn1 x;do [ -z "$x" ]&&x=$'\n';printf %s "$x">&147;done` (disconnect using `exec 147<&-; killall cat #sorry`)
-        
-        ## tls clients
-        
-        if you enable TLS with `-tpt 2424` (telnet) and/or `-tpn 1515` (netcat) you can connect to r0c with TLS encryption using any of the following:
-        
-        * `telnet-ssl -zssl -zsecure -zcacert=r0c.crt r0c.int 2424`
-        * `socat -,raw,echo=0 openssl:r0c.int:1515,cafile=cert.crt`
-        * `stty -icanon; ncat --ssl --ssl-trustfile r0c.crt -v r0c.int 1515`
-        * `stty -icanon; openssl s_client -CAfile ~/.r0c/cert.crt -connect r0c.int:1515`
-        
-        ## firewall rules
-        
-        telnet uses port 23 by default, so on the server you'll want to port-forward `23` to `2323` (and `531` to `1531` for plaintext):
-        
-        ```bash
-        iptables -A INPUT -p tcp --dport 23 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 531 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 2323 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 1531 -m state --state NEW -j ACCEPT
-        iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 23 -j REDIRECT --to-port 2323
-        iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 531 -j REDIRECT --to-port 1531
-        ```
-        
-        ## documentation
-        
-        not really but there is a [list of commands](https://github.com/9001/r0c/blob/master/docs/help-commands.md) and a [list of hotkeys](https://github.com/9001/r0c/blob/master/docs/help-hotkeys.md)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -115,15 +18,137 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Terminals :: Telnet
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `r0c` telnet server
+
+* retr0chat, irc-like chat service for superthin clients [(on PyPI)](https://pypi.org/project/r0c/)
+* MIT-Licensed, 2018-01-07, ed @ irc.rizon.net
+* **[windows telnet 360 noscope](https://ocv.me/r0c.webm)** <- good video
+
+![screenshot of telnet connected to a r0c server](https://raw.githubusercontent.com/9001/r0c/master/docs/r0c.png)
+
+* see [installation](#installation) or grab the latest release: **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
+
+## summary
+
+imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
+
+retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
+
+* tries to be irssi
+* zero dependencies on python 2.6, 2.7, 3.x
+* supports telnet, netcat, /dev/tcp, TLS clients
+* [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
+* fallbacks for inhumane conditions
+  * linemode
+  * no vt100 / ansi escape codes
+
+## endorsements
+
+* the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
+
+## features
+
+irc-like:
+* public channels with persistent history (pgup/pgdn)
+* private messages (`/msg acidburn hey`)
+* nick completion with `Tab ↹`
+* notifications (bell/visual) on hilights and PMs
+* command subset (`/nick`, `/join`, `/part`, `/names`, `/topic`, `/me`)
+* inline message coloring, see `/help`
+
+technical:
+* client behavior detection (echo, colors, charset, newline)
+* message input with readline-like editing (arrow-left/right, home/end, backspace)
+  * history of sent messages (arrow-up/down)
+* bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
+* fast enough; 1'000 clients @ 200 msgs/sec
+
+## windows clients
+
+* use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
+* or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
+* or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
+
+putty is the best option;
+* the powershell client is OK and no longer spammy as of windows 10.0.15063 (win10 1703 / LTSC)
+* windows-telnet has a bug (since win7) where [non-ascii letters occasionally render but usually dont](https://ocv.me/stuff/win10-telnet.webm)
+  * this is due to a buffer overflow in `telnet.exe`, so r0c will apply a rate-limit to avoid it
+  * looks like messages larger than 512 bytes end up messing with the unicode glyphs area? or something
+
+## linux clients
+
+most to least recommended
+
+| client | example |
+| :---   | :---    |
+| telnet | `telnet r0c.int` |
+| socat  | `socat -,raw,echo=0 tcp:r0c.int:531` |
+| bash   | [mostly internals](https://github.com/9001/r0c/blob/master/clients/bash.sh) |
+| netcat | `nc r0c.int 531` |
+
+you can even `exec 147<>/dev/tcp/r0c.int/531;cat<&147&while IFS= read -rn1 x;do [ -z "$x" ]&&x=$'\n';printf %s "$x">&147;done` (disconnect using `exec 147<&-; killall cat #sorry`)
+
+## tls clients
+
+if you enable TLS with `-tpt 2424` (telnet) and/or `-tpn 1515` (netcat) you can connect to r0c with TLS encryption using any of the following:
+
+* `telnet-ssl -zssl -zsecure -zcacert=r0c.crt r0c.int 2424`
+* `socat -,raw,echo=0 openssl:r0c.int:1515,cafile=cert.crt`
+* `stty -icanon; ncat --ssl --ssl-trustfile r0c.crt -v r0c.int 1515`
+* `stty -icanon; openssl s_client -CAfile ~/.r0c/cert.crt -connect r0c.int:1515`
+
+
+
+# installation
+
+just run **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** and that's it (usually)
+
+* or install through pypi (python3 only): `python3 -m pip install --user -U r0c`
+
+you can run it as a service so it autostarts on boot:
+
+* on most linux distros: [systemd service](https://github.com/9001/r0c/blob/master/docs/systemd/r0c.service) (automatically does port-forwarding)
+* on alpine / gentoo: [openrc service](https://github.com/9001/r0c/blob/master/docs/openrc/r0c)
+* on windows: [nssm](https://nssm.cc/) probably
+
+## firewall rules
+
+skip this section if:
+* you are using the systemd service
+* or you are running as root and do not have a firewall
+* or you're on windows
+
+telnet uses port 23 by default, so on the server you'll want to port-forward `23` to `2323` (and `531` to `1531` for plaintext):
+
+```bash
+iptables -A INPUT -p tcp --dport 23 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 531 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 2323 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 1531 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 2424 -m state --state NEW -j ACCEPT  # tls telnet
+iptables -A INPUT -p tcp --dport 1515 -m state --state NEW -j ACCEPT  # tls netcat
+iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 23 -j REDIRECT --to-port 2323
+iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 531 -j REDIRECT --to-port 1531
+```
+
+(you'll have to do this on every reboot)
+
+## documentation
+
+not really but there is a [list of commands](https://github.com/9001/r0c/blob/master/docs/help-commands.md) and a [list of hotkeys](https://github.com/9001/r0c/blob/master/docs/help-hotkeys.md)
```

### Comparing `r0c-1.4.0/README.md` & `r0c-1.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 * retr0chat, irc-like chat service for superthin clients [(on PyPI)](https://pypi.org/project/r0c/)
 * MIT-Licensed, 2018-01-07, ed @ irc.rizon.net
 * **[windows telnet 360 noscope](https://ocv.me/r0c.webm)** <- good video
 
 ![screenshot of telnet connected to a r0c server](docs/r0c.png)
 
-* download the latest release (standalone): **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
+* see [installation](#installation) or grab the latest release: **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
 
 ## summary
 
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
@@ -73,23 +73,46 @@
 if you enable TLS with `-tpt 2424` (telnet) and/or `-tpn 1515` (netcat) you can connect to r0c with TLS encryption using any of the following:
 
 * `telnet-ssl -zssl -zsecure -zcacert=r0c.crt r0c.int 2424`
 * `socat -,raw,echo=0 openssl:r0c.int:1515,cafile=cert.crt`
 * `stty -icanon; ncat --ssl --ssl-trustfile r0c.crt -v r0c.int 1515`
 * `stty -icanon; openssl s_client -CAfile ~/.r0c/cert.crt -connect r0c.int:1515`
 
+
+
+# installation
+
+just run **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** and that's it (usually)
+
+* or install through pypi (python3 only): `python3 -m pip install --user -U r0c`
+
+you can run it as a service so it autostarts on boot:
+
+* on most linux distros: [systemd service](docs/systemd/r0c.service) (automatically does port-forwarding)
+* on alpine / gentoo: [openrc service](docs/openrc/r0c)
+* on windows: [nssm](https://nssm.cc/) probably
+
 ## firewall rules
 
+skip this section if:
+* you are using the systemd service
+* or you are running as root and do not have a firewall
+* or you're on windows
+
 telnet uses port 23 by default, so on the server you'll want to port-forward `23` to `2323` (and `531` to `1531` for plaintext):
 
 ```bash
 iptables -A INPUT -p tcp --dport 23 -m state --state NEW -j ACCEPT
 iptables -A INPUT -p tcp --dport 531 -m state --state NEW -j ACCEPT
 iptables -A INPUT -p tcp --dport 2323 -m state --state NEW -j ACCEPT
 iptables -A INPUT -p tcp --dport 1531 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 2424 -m state --state NEW -j ACCEPT  # tls telnet
+iptables -A INPUT -p tcp --dport 1515 -m state --state NEW -j ACCEPT  # tls netcat
 iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 23 -j REDIRECT --to-port 2323
 iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 531 -j REDIRECT --to-port 1531
 ```
 
+(you'll have to do this on every reboot)
+
 ## documentation
 
 not really but there is a [list of commands](docs/help-commands.md) and a [list of hotkeys](docs/help-hotkeys.md)
```

### Comparing `r0c-1.4.0/clients/bash.sh` & `r0c-1.4.1/clients/bash.sh`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/clients/powershell.ps1` & `r0c-1.4.1/clients/powershell.ps1`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/docs/help-commands.md` & `r0c-1.4.1/docs/help-commands.md`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/docs/help-hotkeys.md` & `r0c-1.4.1/docs/help-hotkeys.md`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/docs/todo.md` & `r0c-1.4.1/docs/todo.md`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/__init__.py` & `r0c-1.4.1/r0c/__init__.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/__main__.py` & `r0c-1.4.1/r0c/__main__.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/chat.py` & `r0c-1.4.1/r0c/chat.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/diag.py` & `r0c-1.4.1/r0c/diag.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/inetcat.py` & `r0c-1.4.1/r0c/inetcat.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/itelnet.py` & `r0c-1.4.1/r0c/itelnet.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/ivt100.py` & `r0c-1.4.1/r0c/ivt100.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/user.py` & `r0c-1.4.1/r0c/user.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/util.py` & `r0c-1.4.1/r0c/util.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c/world.py` & `r0c-1.4.1/r0c/world.py`

 * *Files identical despite different names*

### Comparing `r0c-1.4.0/r0c.egg-info/PKG-INFO` & `r0c-1.4.1/r0c.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,15 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.4.0
+Version: 1.4.1
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
-Description: # `r0c` telnet server
-        
-        * retr0chat, irc-like chat service for superthin clients [(on PyPI)](https://pypi.org/project/r0c/)
-        * MIT-Licensed, 2018-01-07, ed @ irc.rizon.net
-        * **[windows telnet 360 noscope](https://ocv.me/r0c.webm)** <- good video
-        
-        ![screenshot of telnet connected to a r0c server](https://raw.githubusercontent.com/9001/r0c/master/docs/r0c.png)
-        
-        * download the latest release (standalone): **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
-        
-        ## summary
-        
-        imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
-        
-        retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
-        
-        * tries to be irssi
-        * zero dependencies on python 2.6, 2.7, 3.x
-        * supports telnet, netcat, /dev/tcp, TLS clients
-        * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
-        * fallbacks for inhumane conditions
-          * linemode
-          * no vt100 / ansi escape codes
-        
-        ## endorsements
-        
-        * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
-        
-        ## features
-        
-        irc-like:
-        * public channels with persistent history (pgup/pgdn)
-        * private messages (`/msg acidburn hey`)
-        * nick completion with `Tab ↹`
-        * notifications (bell/visual) on hilights and PMs
-        * command subset (`/nick`, `/join`, `/part`, `/names`, `/topic`, `/me`)
-        * inline message coloring, see `/help`
-        
-        technical:
-        * client behavior detection (echo, colors, charset, newline)
-        * message input with readline-like editing (arrow-left/right, home/end, backspace)
-          * history of sent messages (arrow-up/down)
-        * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
-        * fast enough; 1'000 clients @ 200 msgs/sec
-        
-        ## windows clients
-        
-        * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
-        * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
-        * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
-        
-        putty is the best option;
-        * the powershell client is OK and no longer spammy as of windows 10.0.15063 (win10 1703 / LTSC)
-        * windows-telnet has a bug (since win7) where [non-ascii letters occasionally render but usually dont](https://ocv.me/stuff/win10-telnet.webm)
-          * this is due to a buffer overflow in `telnet.exe`, so r0c will apply a rate-limit to avoid it
-          * looks like messages larger than 512 bytes end up messing with the unicode glyphs area? or something
-        
-        ## linux clients
-        
-        most to least recommended
-        
-        | client | example |
-        | :---   | :---    |
-        | telnet | `telnet r0c.int` |
-        | socat  | `socat -,raw,echo=0 tcp:r0c.int:531` |
-        | bash   | [mostly internals](https://github.com/9001/r0c/blob/master/clients/bash.sh) |
-        | netcat | `nc r0c.int 531` |
-        
-        you can even `exec 147<>/dev/tcp/r0c.int/531;cat<&147&while IFS= read -rn1 x;do [ -z "$x" ]&&x=$'\n';printf %s "$x">&147;done` (disconnect using `exec 147<&-; killall cat #sorry`)
-        
-        ## tls clients
-        
-        if you enable TLS with `-tpt 2424` (telnet) and/or `-tpn 1515` (netcat) you can connect to r0c with TLS encryption using any of the following:
-        
-        * `telnet-ssl -zssl -zsecure -zcacert=r0c.crt r0c.int 2424`
-        * `socat -,raw,echo=0 openssl:r0c.int:1515,cafile=cert.crt`
-        * `stty -icanon; ncat --ssl --ssl-trustfile r0c.crt -v r0c.int 1515`
-        * `stty -icanon; openssl s_client -CAfile ~/.r0c/cert.crt -connect r0c.int:1515`
-        
-        ## firewall rules
-        
-        telnet uses port 23 by default, so on the server you'll want to port-forward `23` to `2323` (and `531` to `1531` for plaintext):
-        
-        ```bash
-        iptables -A INPUT -p tcp --dport 23 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 531 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 2323 -m state --state NEW -j ACCEPT
-        iptables -A INPUT -p tcp --dport 1531 -m state --state NEW -j ACCEPT
-        iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 23 -j REDIRECT --to-port 2323
-        iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 531 -j REDIRECT --to-port 1531
-        ```
-        
-        ## documentation
-        
-        not really but there is a [list of commands](https://github.com/9001/r0c/blob/master/docs/help-commands.md) and a [list of hotkeys](https://github.com/9001/r0c/blob/master/docs/help-hotkeys.md)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -115,15 +18,137 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Terminals :: Telnet
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `r0c` telnet server
+
+* retr0chat, irc-like chat service for superthin clients [(on PyPI)](https://pypi.org/project/r0c/)
+* MIT-Licensed, 2018-01-07, ed @ irc.rizon.net
+* **[windows telnet 360 noscope](https://ocv.me/r0c.webm)** <- good video
+
+![screenshot of telnet connected to a r0c server](https://raw.githubusercontent.com/9001/r0c/master/docs/r0c.png)
+
+* see [installation](#installation) or grab the latest release: **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)**
+
+## summary
+
+imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
+
+retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
+
+* tries to be irssi
+* zero dependencies on python 2.6, 2.7, 3.x
+* supports telnet, netcat, /dev/tcp, TLS clients
+* [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
+* fallbacks for inhumane conditions
+  * linemode
+  * no vt100 / ansi escape codes
+
+## endorsements
+
+* the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
+
+## features
+
+irc-like:
+* public channels with persistent history (pgup/pgdn)
+* private messages (`/msg acidburn hey`)
+* nick completion with `Tab ↹`
+* notifications (bell/visual) on hilights and PMs
+* command subset (`/nick`, `/join`, `/part`, `/names`, `/topic`, `/me`)
+* inline message coloring, see `/help`
+
+technical:
+* client behavior detection (echo, colors, charset, newline)
+* message input with readline-like editing (arrow-left/right, home/end, backspace)
+  * history of sent messages (arrow-up/down)
+* bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
+* fast enough; 1'000 clients @ 200 msgs/sec
+
+## windows clients
+
+* use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
+* or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
+* or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
+
+putty is the best option;
+* the powershell client is OK and no longer spammy as of windows 10.0.15063 (win10 1703 / LTSC)
+* windows-telnet has a bug (since win7) where [non-ascii letters occasionally render but usually dont](https://ocv.me/stuff/win10-telnet.webm)
+  * this is due to a buffer overflow in `telnet.exe`, so r0c will apply a rate-limit to avoid it
+  * looks like messages larger than 512 bytes end up messing with the unicode glyphs area? or something
+
+## linux clients
+
+most to least recommended
+
+| client | example |
+| :---   | :---    |
+| telnet | `telnet r0c.int` |
+| socat  | `socat -,raw,echo=0 tcp:r0c.int:531` |
+| bash   | [mostly internals](https://github.com/9001/r0c/blob/master/clients/bash.sh) |
+| netcat | `nc r0c.int 531` |
+
+you can even `exec 147<>/dev/tcp/r0c.int/531;cat<&147&while IFS= read -rn1 x;do [ -z "$x" ]&&x=$'\n';printf %s "$x">&147;done` (disconnect using `exec 147<&-; killall cat #sorry`)
+
+## tls clients
+
+if you enable TLS with `-tpt 2424` (telnet) and/or `-tpn 1515` (netcat) you can connect to r0c with TLS encryption using any of the following:
+
+* `telnet-ssl -zssl -zsecure -zcacert=r0c.crt r0c.int 2424`
+* `socat -,raw,echo=0 openssl:r0c.int:1515,cafile=cert.crt`
+* `stty -icanon; ncat --ssl --ssl-trustfile r0c.crt -v r0c.int 1515`
+* `stty -icanon; openssl s_client -CAfile ~/.r0c/cert.crt -connect r0c.int:1515`
+
+
+
+# installation
+
+just run **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** and that's it (usually)
+
+* or install through pypi (python3 only): `python3 -m pip install --user -U r0c`
+
+you can run it as a service so it autostarts on boot:
+
+* on most linux distros: [systemd service](https://github.com/9001/r0c/blob/master/docs/systemd/r0c.service) (automatically does port-forwarding)
+* on alpine / gentoo: [openrc service](https://github.com/9001/r0c/blob/master/docs/openrc/r0c)
+* on windows: [nssm](https://nssm.cc/) probably
+
+## firewall rules
+
+skip this section if:
+* you are using the systemd service
+* or you are running as root and do not have a firewall
+* or you're on windows
+
+telnet uses port 23 by default, so on the server you'll want to port-forward `23` to `2323` (and `531` to `1531` for plaintext):
+
+```bash
+iptables -A INPUT -p tcp --dport 23 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 531 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 2323 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 1531 -m state --state NEW -j ACCEPT
+iptables -A INPUT -p tcp --dport 2424 -m state --state NEW -j ACCEPT  # tls telnet
+iptables -A INPUT -p tcp --dport 1515 -m state --state NEW -j ACCEPT  # tls netcat
+iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 23 -j REDIRECT --to-port 2323
+iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 531 -j REDIRECT --to-port 1531
+```
+
+(you'll have to do this on every reboot)
+
+## documentation
+
+not really but there is a [list of commands](https://github.com/9001/r0c/blob/master/docs/help-commands.md) and a [list of hotkeys](https://github.com/9001/r0c/blob/master/docs/help-hotkeys.md)
```

### Comparing `r0c-1.4.0/setup.py` & `r0c-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,23 @@
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: IronPython",
         "Programming Language :: Python :: Implementation :: Jython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Environment :: Console",
         "Environment :: No Input/Output (Daemon)",
         "Topic :: Communications :: Chat",
+        "Topic :: Terminals :: Telnet",
     ],
     "cmdclass": {"clean2": clean2},
 }
 
 
 if setuptools_available:
     args.update(
```

