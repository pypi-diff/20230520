# Comparing `tmp/pyhtools-2.2.3.tar.gz` & `tmp/pyhtools-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.2.3.tar", max compression
+gzip compressed data, was "pyhtools-2.2.4.tar", max compression
```

## Comparing `pyhtools-2.2.3.tar` & `pyhtools-2.2.4.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0     1076 2023-05-20 06:53:14.382185 pyhtools-2.2.3/LICENSE
--rw-r--r--   0        0        0     6823 2023-05-20 06:53:14.386185 pyhtools-2.2.3/README.md
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      283 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     6409 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/UI/functions.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/__init__.py
--rw-r--r--   0        0        0      201 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0     2728 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/forensics/data_harvestor.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     4887 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      406 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     6629 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4867 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3726 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     5075 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     4580 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2552 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     2177 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2831 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     7372 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0     4669 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     6643 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     3012 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     2141 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1357 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     3403 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     4529 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__main__.py
--rw-r--r--   0        0        0     7036 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2132 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-20 06:53:14.386185 pyhtools-2.2.3/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     4132 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3352 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2272 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1850 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1632 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     4868 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2230 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2599 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1338 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1147 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5247 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5727 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5015 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     4349 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2242 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0        0 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3857 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0      528 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyhtools/utils.py
--rw-r--r--   0        0        0     1822 2023-05-20 06:53:14.390185 pyhtools-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 pyhtools-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-20 13:10:37.960043 pyhtools-2.2.4/LICENSE
+-rw-r--r--   0        0        0     6823 2023-05-20 13:10:37.960043 pyhtools-2.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     6464 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/forensics/__init__.py
+-rw-r--r--   0        0        0     2876 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/forensics/data_harvester.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     6596 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      563 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     6629 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4868 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3726 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     5075 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     4580 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2552 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     2177 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2831 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     7372 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0     4669 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     6643 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     3012 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     2141 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1357 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     3403 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     4529 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__main__.py
+-rw-r--r--   0        0        0     7036 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2132 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     2254 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     1757 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/win_block_usb.py
+-rw-r--r--   0        0        0     4132 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/exec_generator.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/__init__.py
+-rw-r--r--   0        0        0     3352 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     2272 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
+-rw-r--r--   0        0        0     1850 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
+-rw-r--r--   0        0        0     1632 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
+-rw-r--r--   0        0        0     4868 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
+-rw-r--r--   0        0        0     2230 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/installer/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/installer/cert.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/keylogger/__init__.py
+-rw-r--r--   0        0        0     2599 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/keylogger/keylogger.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
+-rw-r--r--   0        0        0     1338 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
+-rw-r--r--   0        0        0     1147 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
+-rw-r--r--   0        0        0     5247 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
+-rw-r--r--   0        0        0     5727 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
+-rw-r--r--   0        0        0     5015 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     4349 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
+-rw-r--r--   0        0        0     2242 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/worms/__init__.py
+-rw-r--r--   0        0        0     3857 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/worms/dir_cloner.py
+-rw-r--r--   0        0        0      710 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/utils.py
+-rw-r--r--   0        0        0     1822 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 pyhtools-2.2.4/PKG-INFO
```

### Comparing `pyhtools-2.2.3/LICENSE` & `pyhtools-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/README.md` & `pyhtools-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/UI/functions.py` & `pyhtools-2.2.4/pyhtools/UI/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     print(BRIGHT_WHITE + f'| written by dmdhrumilmistry               |')
     print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
 
 
 def print_help():
     '''
     prints commands with their brief description.
+
+    Args:
+        None
+    
+    Returns:
+        None
     '''
     print(BRIGHT_WHITE + 'Python Hacking Tools (PyHTools) (pht)')
 
     help = PrettyTable(['Command', 'Description'])
     help.align['Command'] = 'c'
     help.align['Description'] = 'l'
     # help.add_row(['',''])
```

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Android/forensics/data_harvestor.py` & `pyhtools-2.2.4/pyhtools/attackers/Android/forensics/data_harvester.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,59 @@
 from ppadb.device import Device
 from subprocess import Popen, PIPE, STDOUT
 
 import logging
 import shutil
 import threading
 import os
+
+logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.DEBUG,
                     format='[%(asctime)s] [%(levelname)s] - %(message)s')
 
 
 class DataHarvestorExceptions:
     '''
-    Exceptions for DataHarvestor class
+    Exceptions for DataHarvester class
     '''
     class ServerNotRunning(Exception):
+        '''Server Not Running Exception'''
         pass
 
     class NoDevicesFound(Exception):
+        '''No Devices Found Exception'''
         pass
 
 
-class DataHarvestor:
+class DataHarvester:
+    '''Class to harvest data'''
     def __init__(self, dest_path: str, device_name: str, host: str = '127.0.0.1', port: int = 5037) -> None:
         assert type(dest_path) == str
         assert type(device_name) == str
         assert type(host) == str
         assert type(port) == int
 
         self.__device_name = device_name
         self.__dest_path = dest_path
 
         self._adb = Client(
             host=host,
             port=port
         )
         self.device: Device = self.get_device()
-        logging.info(f'Using {self.__device_name}')
+        logger.info(f'Using {self.__device_name}')
 
         # check paths, if present remove all files present
         if os.path.isdir(dest_path):
-            logging.warning(
+            logger.warning(
                 'Destination Path is already present, complete directory data will be overwritten')
             shutil.rmtree(dest_path)
 
         # Create Paths
-        logging.info('Creating Destination Path')
+        logger.info('Creating Destination Path')
         os.makedirs(dest_path)
 
     def get_device(self):
         _ = self.get_adb_devices()
         device: Device = self._adb.device(self.__device_name)
         return device
 
@@ -72,17 +77,17 @@
             shell=True,
             stdout=PIPE,
             stderr=STDOUT,
         )
 
     def start(self):
         # get package paths
-        logging.info('Getting packages list')
+        logger.info('Getting packages list')
         package_paths = [os.path.join('/data/data/', package_path)
                          for package_path in str(self.device.shell('ls -a /data/data')).splitlines()]
 
-        logging.info('Harvesting Data')
+        logger.info('Harvesting Data')
         for package_path in package_paths:
             threading.Thread(target=self.__clone_dir,
                              args=(package_path,)).start()
 
-        logging.info('Data Harvesting Completed')
+        logger.info('Data Harvesting Completed')
```

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.2.4/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,38 @@
 import logging
 import threading
 logging.basicConfig(level=logging.DEBUG,
                     format='[%(asctime)s] [%(levelname)s] - %(message)s')
 
 
 class PinCertificateExceptions:
-    '''
-    Pin Certificate Exception Class
-    '''
+    '''Pin Certificate Exception Class'''
     class ServerNotRunning(Exception):
-        pass
-
+        '''Server Not Running Exception Class'''
     class NoDevicesFound(Exception):
-        pass
+        '''No Devices Found Exception Class'''
 
 
 class PinCertificate:
     def __init__(self, apk_path: str,  package_name: str, cert_path: str, frida_binary_path: str, frida_script_path: str, device_name: str, host: str = '127.0.0.1', port: int = 5037,):
+        '''Pin Certificate class
+        
+        Args:
+            apk_path (str): apk file path
+            package_name (str): package name of apk file
+            cert_path (str): file path of certificate to be installed
+            frida_binary_path (str): file path of frida binary file
+            frida_script_file (str): file path of cert installer script to be executed in frida after frida installation
+            device_name (str): name of device for adb connection
+            host (str): adb host ip
+            port (int): adb host port
+
+        Returns:
+            None (None): None
+        '''
         # check data types
         assert type(apk_path) == str
         assert type(package_name) == str
         assert type(cert_path) == str
         assert type(device_name) == str
         assert type(frida_binary_path) == str
         assert type(frida_script_path) == str
@@ -64,60 +76,109 @@
             port=port
         )
 
         # set initial values
         self.device = self.get_device()
 
     def get_device(self):
+        '''Get adb device
+        
+        Args:
+            None
+
+        Returns:
+            ppadb.device.Device: returns specified adb device
+        '''
         _ = self.get_adb_devices()
         device: Device = self._adb.device(self.__device_name)
         return device
 
     def get_adb_devices(self):
+        '''returns lis of all adb devices
+        
+        Args:
+            None
+
+        Returns:
+            list: list of connected adb devices
+        '''
         try:
             devices: list[Device] = self._adb.devices()
             if len(devices) == 0:
                 raise PinCertificateExceptions.NoDevicesFound(
                     "No ADB Devices Attached")
 
             return devices
         except RuntimeError:
             raise PinCertificateExceptions.ServerNotRunning(
                 "ADB Server is not running, start using `adb start-server`")
 
     def get_frida_devices(self):
+        '''Get list of devices running frida
+
+        Args:
+            None:
+
+        Returns:
+            list: list of adb connected devices running frida server
+        '''
         devices = frida.enumerate_devices()
         if len(devices) == 0:
             raise PinCertificateExceptions.NoDevicesFound(
                 "No Frida Devices Found")
 
         return devices
 
     def install_apk(self, force_install: bool = True):
+        '''Installs apk on device
+        
+        Args:
+            force_install (bool): if True then uninstalls apk if already installed then installs apk again
+
+        Returns:
+            bool: True if installed successfully else False
+        '''
         if self.device.is_installed(self.__package_name) and force_install:
             self.device.uninstall(self.__package_name)
 
         self.device.install(self.__apk_path)
 
         if self.device.is_installed(self.__package_name):
             return True
+        
         return False
 
     def start_frida(self):
-        asyncio.run(utils.run(f'adb shell /data/local/tmp/frida-server &'))
+        '''Starts Frida server on target device
+        
+        Args:
+            None
+        
+        Returns:
+            None
+        '''
+        asyncio.run(utils.run('adb shell /data/local/tmp/frida-server &'))
 
     def pin_certificate(self):
+        '''Starts certificate pinning procedure to the apk
+
+        Args:
+            None
+
+        Returns:
+            None
+        '''
         logging.info("Starting Certificate Pinning Procedure..")
 
         # get device
         self.device: Device = self.get_device()
         logging.info(f'Connected to {self.__device_name} device')
 
         # install apk
-        logging.info(f'Installing package')
+        logging.info('Installing package')
         if self.install_apk():
             logging.info(
                 f'{basename(self.__apk_path)} APK installation completed successfully')
         else:
             logging.error(
                 f'{basename(self.__apk_path)} APK installation failed!')
```

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/arpspoofer.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/code_injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #########################################################################
 # If you encounter Import error after installing netfilter use command 
 # sudo apt install libnfnetlink-dev libnetfilter-queue-dev
 # sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
 #########################################################################
 
 from subprocess import call
-import netfilterqueue
-import scapy.all as scapy
 from re import search, sub
 from pyhtools.UI.colors import *
 
+import scapy.all as scapy
+import netfilterqueue
 
 ############################### Functions ############################### 
 def forward_packets():
     '''configures the mitm for incoming request packets
     into a queue.
 
     Args:
@@ -96,15 +96,15 @@
             load = load.replace('</BODY>', '</body>')
             if '</body>' in load:
                 print('\n[+] Script/Code Injected!!\n')
                 tampered_load = load.replace('</body>', inj_code+'</body>')
                 tampered_load = tampered_load.encode('utf-8', 'ignore')
                 print(tampered_load)
 
-                content_len_search = search("(?:Content-Length:\s)(\d*)", load)
+                content_len_search = search(r"(?:Content-Length:\s)(\d*)", load)
                 if content_len_search and b'text/html' in load:
                     content_len = content_len_search.group(1)
                     new_content_len = int(content_len) + len(inj_code)
 
                     tampered_load = sub(b'(?:Content-Length:\s)(\d*)', bytes(new_content_len), tampered_load)
                 print(tampered_load)
```

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/dnsspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/downloads_replacer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/machngr.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/machngr.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/network_jammer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/nwscan.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/Network/tcp_proxy.py` & `pyhtools-2.2.4/pyhtools/attackers/Network/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/attackers.py` & `pyhtools-2.2.4/pyhtools/attackers/attackers.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/api/discover.py` & `pyhtools-2.2.4/pyhtools/attackers/web/api/discover.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.2.4/pyhtools/attackers/web/enumerate.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.2.4/pyhtools/attackers/web/get_forms.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.2.4/pyhtools/attackers/web/login_guesser.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/spider.py` & `pyhtools-2.2.4/pyhtools/attackers/web/spider.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/utils.py` & `pyhtools-2.2.4/pyhtools/attackers/web/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/__main__.py` & `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.2.4/pyhtools/detectors/arp_spoof_detector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 import scapy.all as sp
 from argparse import ArgumentParser
 
 
 class SpoofDetector:
     '''
-    ARP spoofer to perform Local MITM attacks
+    SpoofDetector class to detect Local MITM attacks
     '''
 
     def __init__(self, interface: str) -> None:
+        '''SpoofDetector class constructor
+        
+        Args:
+            interface (str): network interface on which spoofing needs to be detected
+
+        Returns:
+            None
+        '''
         self.interface = interface
 
+
     def get_mac(self, ip: str):
-        '''
-        returns mac address of the ip
+        '''returns mac address of the ip
+
+        Args:
+            ip (str): ip address of the string
+
+        Returns:
+            str: Mac address of the ip in the network
         '''
         arp_req = sp.ARP(pdst=ip)
         brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
 
         packet = brdcst / arp_req
         responded_list = sp.srp(packet, timeout=1, verbose=False)[0]
+        
+        return str(responded_list[0][1].hwsrc)
 
-        return responded_list[0][1].hwsrc
 
     def check_spoof(self, packet) -> bool:
-        '''
-        checks if machine is under ARP/MITM attack.
+        '''checks if machine is under ARP/MITM attack
+
+        Args:
+            packet (scapy.Packet): sniffed scapy packet from the interface
+
+        Returns:
+            bool: True if ARP spoofing/poisoning detected else False
         '''
         if packet.haslayer(sp.ARP) and packet[sp.ARP].op == 2:
             try:
                 real_mac = self.get_mac(packet[sp.ARP].psrc)
                 response_mac = packet[sp.ARP].hwsrc
                 if real_mac != response_mac:
                     print(
                         f"[!] ARP Spoof Detected! {response_mac} is imposter. {response_mac} is spoofing as {real_mac}")
             except IndexError:
                 pass
 
+
     def start(self):
-        '''
-        captures and processes packets to check whether network is being attacked or not
+        '''captures and processes packets to check whether network is being attacked or not
+
+        Args:
+            None:
+
+        Returns:
+            None
         '''
         sp.sniff(iface=self.interface, store=False, prn=self.check_spoof)
 
 
 if __name__ == '__main__':
     parser = ArgumentParser()
     parser.add_argument('-i', '--interface', dest='interface',
```

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/exec_generator.py` & `pyhtools-2.2.4/pyhtools/evil_files/exec_generator.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/backdoor/ssh/handler.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/handler.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/installer/cert.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/installer/cert.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/keylogger/keylogger.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/keylogger/keylogger.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/malwares/utils.py` & `pyhtools-2.2.4/pyhtools/evil_files/malwares/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/decrypter.py` & `pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/ransomwares/dmsec/encrypter.py` & `pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/encrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/evil_files/worms/dir_cloner.py` & `pyhtools-2.2.4/pyhtools/evil_files/worms/dir_cloner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.3/pyhtools/utils.py` & `pyhtools-2.2.4/pyhtools/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO,
                     format='[%(asctime)s] [%(levelname)s] - %(message)s')
 
 
 def read_file_lines(file_path: str) -> list[str]:
+    '''reads file and returns as list of str
+    
+    Args:
+        file_path (str): path of file to be read
+
+    Returns:
+        list: lines read from file as list of str 
+    '''
     lines = []
 
     if isfile(file_path):
         with open(file_path, 'r') as f:
             lines = [line.strip() for line in f.readlines()]
             logging.debug(f"File Read: {file_path}")
```

### Comparing `pyhtools-2.2.3/pyproject.toml` & `pyhtools-2.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhtools"
-version = "2.2.3"
+version = "2.2.4"
 description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
 authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `pyhtools-2.2.3/PKG-INFO` & `pyhtools-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtools
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
 License: MIT
 Author: Dhrumil Mistry
 Author-email: contact@dmdhrumilmistry.tech
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

