# Comparing `tmp/paracrine-0.0.6.tar.gz` & `tmp/paracrine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracrine-0.0.6.tar", last modified: Thu May 18 21:04:32 2023, max compression
+gzip compressed data, was "paracrine-0.0.7.tar", last modified: Sat May 20 21:46:38 2023, max compression
```

## Comparing `paracrine-0.0.6.tar` & `paracrine-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,64 @@
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.6/LICENSE
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.6/MANIFEST.in
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 21:04:32.432836 paracrine-0.0.6/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3062 2023-01-29 20:33:16.000000 paracrine-0.0.6/README.md
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4762 2023-01-29 17:58:35.000000 paracrine-0.0.6/paracrine/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      820 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/aws.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3817 2023-05-18 09:57:23.000000 paracrine-0.0.6/paracrine/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5795 2023-05-15 10:59:07.000000 paracrine-0.0.6/paracrine/config.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2362 2023-05-12 12:30:29.000000 paracrine-0.0.6/paracrine/core.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1171 2023-05-17 22:09:32.000000 paracrine-0.0.6/paracrine/cron.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3341 2023-05-14 10:12:09.000000 paracrine-0.0.6/paracrine/debian.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1856 2023-05-12 12:21:05.000000 paracrine-0.0.6/paracrine/deps.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10055 2023-05-18 21:00:30.000000 paracrine-0.0.6/paracrine/fs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      960 2023-02-04 16:56:52.000000 paracrine-0.0.6/paracrine/login.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      896 2023-05-15 10:59:42.000000 paracrine-0.0.6/paracrine/network.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-01-22 00:10:48.000000 paracrine-0.0.6/paracrine/python.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/reboot.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3576 2023-05-12 12:35:38.000000 paracrine-0.0.6/paracrine/runner.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/services/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.6/paracrine/services/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4961 2023-05-18 21:00:30.000000 paracrine-0.0.6/paracrine/services/cockroachdb.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      177 2023-05-09 13:05:32.000000 paracrine-0.0.6/paracrine/services/ntp.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4136 2023-05-14 10:11:08.000000 paracrine-0.0.6/paracrine/services/pleroma.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1247 2023-05-14 10:14:42.000000 paracrine-0.0.6/paracrine/services/postgresql.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4434 2023-05-15 10:24:12.000000 paracrine-0.0.6/paracrine/services/wireguard.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-02-04 16:56:52.000000 paracrine-0.0.6/paracrine/setup.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-14 10:17:17.000000 paracrine-0.0.6/paracrine/systemd.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/templates/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.6/paracrine/templates/certbot_requirements.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-17 22:16:40.000000 paracrine-0.0.6/paracrine/templates/cockroach.service.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1774 2023-02-04 15:56:26.000000 paracrine-0.0.6/paracrine/templates/config.exs.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.6/paracrine/templates/cron.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.6/paracrine/templates/pleroma.nginx.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.6/paracrine/templates/robots.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.6/paracrine/templates/setup_db.psql.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/templates/wg.conf.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1180 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/users.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine.egg-info/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1023 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/SOURCES.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/dependency_links.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       36 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/requires.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/top_level.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      741 2023-05-18 21:04:06.000000 paracrine-0.0.6/pyproject.toml
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-18 21:04:32.432836 paracrine-0.0.6/setup.cfg
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/tests/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.6/tests/test_ssh.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.7/LICENSE
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.7/MANIFEST.in
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-05-20 21:46:38.135034 paracrine-0.0.7/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3071 2023-05-20 20:51:52.000000 paracrine-0.0.7/README.md
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4661 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/commands/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      969 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/login.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/reboot.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/setup.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1864 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/deps.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/helpers/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5862 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/helpers/config.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1161 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/cron.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3492 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/debian.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10091 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/fs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      896 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/network.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/python.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/systemd.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1232 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/users.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3478 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runner.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/runners/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/runners/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      828 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/runners/aws.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3855 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runners/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2314 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runners/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/services/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.7/paracrine/services/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/services/cockroachdb/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1067 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2688 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/services/cockroachdb/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      699 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      670 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/init.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2441 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/node.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      172 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/ntp.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4091 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/pleroma.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1242 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/postgresql.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/services/wireguard/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       62 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3493 2023-05-20 21:43:24.000000 paracrine-0.0.7/paracrine/services/wireguard/bootstrap.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      248 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1147 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/templates/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.7/paracrine/templates/certbot_requirements.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-20 19:57:25.000000 paracrine-0.0.7/paracrine/templates/cockroach.service.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1774 2023-02-04 15:56:26.000000 paracrine-0.0.7/paracrine/templates/config.exs.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.7/paracrine/templates/cron.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.7/paracrine/templates/pleroma.nginx.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.7/paracrine/templates/robots.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.7/paracrine/templates/setup_db.psql.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.7/paracrine/templates/wg.conf.j2
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine.egg-info/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1524 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/SOURCES.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/dependency_links.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       36 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/requires.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/top_level.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      871 2023-05-20 21:46:17.000000 paracrine-0.0.7/pyproject.toml
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-20 21:46:38.135034 paracrine-0.0.7/setup.cfg
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/tests/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.7/tests/test_ssh.py
```

### Comparing `paracrine-0.0.6/LICENSE` & `paracrine-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.6/PKG-INFO` & `paracrine-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.6
+Version: 0.0.7
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 -----
 
 1. Setup Python. Tested against 3.8+
 2. `pip install paracrine`
 3. Write a main file describing what you want to setup. [integration_test/main.py](https://github.com/palfrey/paracrine/blob/main/integration_test/main.py) is a reasonable example. It must call the `run` function, which takes arguments for the inventory file, and list of modules to run.
 4. Write an inventory file for the machines this is managing. Current setup assumes they're all the same. [integration_test/docker/inventory.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/docker/inventory.yaml) is a reasonable example file, but I suggest generating it from whatever you're using to create the servers (e.g. Terraform).
 5. Write a `config.yaml`. This has a main top-level key of `environments` with keys below that for each inventory file you've got ([integration_test/config.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/config.yaml) just has one, but in most scenarios you'll have at least a dev and prod setup). What you do below that is up to you, but typically it'll be environment variables and secrets to feed into the main file.
-6. Run `python -m paracrine.setup <inventory file>` - this will install the minimum python bits so that everything else works.
+6. Run `python -m paracrine.commands.setup <inventory file>` - this will install the minimum python bits so that everything else works.
 7. Run the main file (e.g. `python main.py ./docker/inventory.yaml`)
 
 Limitations
 -----------
 * All the servers are assumed to be Debian Linux boxes (although Debian-derivatives like Ubuntu _should_ work)
 * Direct SSH access is assumed possible (Mitogen supports jump boxes, but there's no setup for that yet here) with keys, not passwords
 * There's no "dry run" mode yet, which would be useful for GitOps
```

### Comparing `paracrine-0.0.6/README.md` & `paracrine-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 -----
 
 1. Setup Python. Tested against 3.8+
 2. `pip install paracrine`
 3. Write a main file describing what you want to setup. [integration_test/main.py](https://github.com/palfrey/paracrine/blob/main/integration_test/main.py) is a reasonable example. It must call the `run` function, which takes arguments for the inventory file, and list of modules to run.
 4. Write an inventory file for the machines this is managing. Current setup assumes they're all the same. [integration_test/docker/inventory.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/docker/inventory.yaml) is a reasonable example file, but I suggest generating it from whatever you're using to create the servers (e.g. Terraform).
 5. Write a `config.yaml`. This has a main top-level key of `environments` with keys below that for each inventory file you've got ([integration_test/config.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/config.yaml) just has one, but in most scenarios you'll have at least a dev and prod setup). What you do below that is up to you, but typically it'll be environment variables and secrets to feed into the main file.
-6. Run `python -m paracrine.setup <inventory file>` - this will install the minimum python bits so that everything else works.
+6. Run `python -m paracrine.commands.setup <inventory file>` - this will install the minimum python bits so that everything else works.
 7. Run the main file (e.g. `python main.py ./docker/inventory.yaml`)
 
 Limitations
 -----------
 * All the servers are assumed to be Debian Linux boxes (although Debian-derivatives like Ubuntu _should_ work)
 * Direct SSH access is assumed possible (Mitogen supports jump boxes, but there's no setup for that yet here) with keys, not passwords
 * There's no "dry run" mode yet, which would be useful for GitOps
```

### Comparing `paracrine-0.0.6/paracrine/__init__.py` & `paracrine-0.0.7/paracrine/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 -----
 
 1. Setup Python. Tested against 3.8+
 2. `pip install paracrine`
 3. Write a main file describing what you want to setup. [integration_test/main.py](https://github.com/palfrey/paracrine/blob/main/integration_test/main.py) is a reasonable example. It must call the `run` function, which takes arguments for the inventory file, and list of modules to run.
 4. Write an inventory file for the machines this is managing. Current setup assumes they're all the same. [integration_test/docker/inventory.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/docker/inventory.yaml) is a reasonable example file, but I suggest generating it from whatever you're using to create the servers (e.g. Terraform).
 5. Write a <code>config.yaml</code>. This has a main top-level key of `environments` with keys below that for each inventory file you've got ([integration_test/config.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/config.yaml) just has one, but in most scenarios you'll have at least a dev and prod setup). What you do below that is up to you, but typically it'll be environment variables and secrets to feed into the main file.
-6. Run `python -m paracrine.setup <inventory file>` - this will install the minimum python bits so that everything else works.
+6. Run `python -m paracrine.commands.setup <inventory file>` - this will install the minimum python bits so that everything else works.
 7. Run the main file (e.g. `python main.py ./docker/inventory.yaml`)
 
 Utilities
 ---
-All the utilities are callable as `python -m paracrine.<utility> <inventory file>` and sometimes some extra args
+All the utilities are callable as `python -m paracrine.commands.<utility> <inventory file>` and sometimes some extra args
 
-* `paracrine.login` - login to a specific server in the inventory. Index of which one is an additional arg
-* `paracrine.setup` - this will install the minimum python bits so that everything else works.
+* `paracrine.commands.login` - login to a specific server in the inventory. Index of which one is an additional arg
+* `paracrine.commands.setup` - this will install the minimum python bits so that everything else works.
 
 Built-in modules
 ---
-* `paracrine.aws` - Runs locally, gets the AWS access/secret keys of the current user during bootstrap for access later. Has a function `set_aws_creds` for setting them in a run step.
-* `paracrine.certs` - Creates SSL certificates via LetsEncrypt. Takes two args "hostname" and "email".
+* `paracrine.runners.aws` - Runs locally, gets the AWS access/secret keys of the current user during bootstrap for access later. Has a function `set_aws_creds` for setting them in a run step.
+* `paracrine.runners.certs` - Creates SSL certificates via LetsEncrypt. Takes two args "hostname" and "email".
+* `paracrine.services.cockroachdb` - Sets up a [CockroachDB server](https://www.cockroachlabs.com/)
 * `paracrine.services.pleroma` - Sets up a [Pleroma server](https://pleroma.social/). Uses the PostgreSQL and certs modules.
 * `paracrine.services.postgresql` - Sets up a [PostgresSQL server](https://www.postgresql.org/)
 * `paracrine.services.wireguard` - Sets up [Wireguard](https://www.wireguard.com/). Assumes your inventory template has a unique `wireguard_ip` line per server.
 
 Writing a module file
 ---
 
 "modules" are just Python files (or packages containing them). They should have one or more specially named functions - all of these are optional, but a module with none of these won't do anything.
 
 * `dependencies` - Returns a list of modules this module requires (e.g. a database setup). Return type is `paracrine.deps.Modules` i.e. a list of either `ModuleType` or a Tuple of `ModuleType` and a value to be inserted as the `options` dictionary into the module.
-* `core_local` - Function to be run locally i.e. on the running host before connecting to the destination machine
-* `core_run` - Main function to run on the destination machine
-* `core_parse_return` - Function to run locally with an argument of the result of running `core_run`
-* `bootstrap_local`/`bootstrap_run`/`bootstrap_parse_return` - Like the `core` ones, but we do all the bootstrap functions first, then run all the core functions. This could be expanded into a n-stage setup, but nothing has needed that yet.
+* `local` - Function to be run locally i.e. on the running host before connecting to the destination machine
+* `run` - Main function to run on the destination machine
+* `parse_return` - Function to run locally with an argument of the result of running `run`
 
-You can just use plain Python code, but `paracrine.fs/config/debian/network/python/systemd/users` have lots of useful functions you should preferably use instead.
+You can just use plain Python code, but `paracrine.helpers.fs/config/debian/network/python/systemd/users` have lots of useful functions you should preferably use instead.
 """
```

### Comparing `paracrine-0.0.6/paracrine/aws.py` & `paracrine-0.0.7/paracrine/runners/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 import pathlib
 
-from .config import config_path, get_config_file
-from .fs import run_command
+from ..helpers.config import config_path, get_config_file
+from ..helpers.fs import run_command
 
 
-def bootstrap_local():
+def local():
     aws_path = pathlib.Path(config_path()).joinpath("other-aws")
     if not aws_path.exists():
         json.dump(
             {
                 "access_key": run_command(
                     "aws configure get aws_access_key_id"
                 ).strip(),
```

### Comparing `paracrine-0.0.6/paracrine/certs.py` & `paracrine-0.0.7/paracrine/runners/certs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from datetime import timedelta
 from pathlib import Path
 from typing import Dict, List, Union
 
-from . import aws, cron
-from .config import core_config, other_config_file
-from .core import use_this_host
-from .debian import apt_install
-from .deps import Modules
-from .fs import (
+from ..deps import Modules
+from ..helpers import cron
+from ..helpers.config import core_config, other_config_file
+from ..helpers.debian import apt_install
+from ..helpers.fs import (
     make_directory,
     run_command,
     run_with_marker,
     set_file_contents_from_template,
 )
-from .python import setup_venv
+from ..helpers.python import setup_venv
+from . import aws
+from .core import use_this_host
 
 options = {}
 
 
 # Are we in a test config where we should just not get the cert
 def get_dummy_certs():
     config = core_config()
@@ -102,17 +103,17 @@
         return {}
 
 
 def dependencies() -> Modules:
     return [aws, cron]
 
 
-def bootstrap_run() -> Dict:
+def run() -> Dict:
     return certbot_for_host(options["hostname"], options["email"])
 
 
-def bootstrap_parse_return(
+def parse_return(
     infos: List[Dict],
 ) -> None:
     for info in infos:
         for key in info:
             open(other_config_file(key), "w").write(info[key])
```

### Comparing `paracrine-0.0.6/paracrine/config.py` & `paracrine-0.0.7/paracrine/helpers/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 
 def create_data(server: Optional[Dict] = None):
     config = get_config()
     templates = {}
     template_paths = [
         pathlib.Path("templates"),
-        pathlib.Path(__file__).parent.joinpath("templates"),
+        pathlib.Path(__file__).parent.parent.joinpath("templates"),
     ]
     for template_path in template_paths:
         if not template_path.exists():
             continue
         for path in walk(template_path):
             templates[path.name] = path.open("r").read()
 
@@ -230,7 +230,11 @@
     local_hostname = host()["name"]
     for server in servers():
         name = server["name"]
         if name == local_hostname:
             return server
 
     raise Exception(f"Cannot find {local_hostname}")
+
+
+def in_docker():
+    return os.path.exists("/.dockerenv")
```

### Comparing `paracrine-0.0.6/paracrine/core.py` & `paracrine-0.0.7/paracrine/runners/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import json
 import os
 import socket
 from pathlib import Path
 from typing import Dict, List
 
-from .config import config, host, network_config_file, other_config_file
-from .debian import apt_install
-from .fs import run_command
-from .users import users
+from ..helpers.config import (
+    config,
+    host,
+    in_docker,
+    network_config_file,
+    other_config_file,
+)
+from ..helpers.debian import apt_install
+from ..helpers.fs import run_command
+from ..helpers.users import in_vagrant, users
 
 
 def is_wireguard():
     return os.path.exists("/etc/wireguard")
 
 
 def hash_fn(key: str, count: int) -> int:
@@ -22,15 +28,15 @@
 # Intended for "run on one machine" things
 def use_this_host(name: str) -> bool:
     hosts = [h["name"] for h in config()["servers"]]
     index = hash_fn(name, len(hosts))
     return host()["name"] == hosts[index]
 
 
-def bootstrap_run():
+def run():
     apt_install(["iproute2"])
 
     data = {
         "hostname": socket.gethostname(),
         "network_devices": run_command("ip -j address"),
         "users": users(force_load=True),
         "groups": run_command("getent group"),
@@ -53,28 +59,20 @@
             apt_install(["curl", "ca-certificates"])
             data["external_ip"] = run_command("curl https://api.ipify.org?format=json")
         json.dump(data["external_ip"], ip_file.open("w"))
 
     return data
 
 
-def bootstrap_parse_return(infos: List[Dict]) -> None:
+def parse_return(infos: List[Dict]) -> None:
     info = infos[0]
     networks = json.loads(info["network_devices"])
     name = info["server_name"]
     json.dump(networks, open(network_config_file(name), "w"), indent=2)
 
     other = {
         "external_ip": json.loads(info["external_ip"])["ip"],
         "users": info["users"],
         "groups": info["groups"],
         "hostname": info["hostname"],
     }
     json.dump(other, open(other_config_file(name), "w"), indent=2)
-
-
-def in_vagrant():
-    return "vagrant" in users()
-
-
-def in_docker():
-    return os.path.exists("/.dockerenv")
```

### Comparing `paracrine-0.0.6/paracrine/cron.py` & `paracrine-0.0.7/paracrine/helpers/cron.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .config import config_path, get_config_file
 from .fs import set_file_contents, set_file_contents_from_template
 
 mailto: Optional[str] = None
 mailfrom: Optional[str] = None
 
 
-def bootstrap_local():
+def local():
     global mailto, mailfrom
     cron_path = pathlib.Path(config_path()).joinpath("cron-info")
     set_file_contents(
         cron_path,
         json.dumps(
             {"mailto": mailto, "mailfrom": mailfrom},
             indent=2,
```

### Comparing `paracrine-0.0.6/paracrine/debian.py` & `paracrine-0.0.7/paracrine/helpers/debian.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 import os
 import re
+from glob import glob
 from typing import Dict, List, Optional, Union
 
 from debian.debian_support import version_compare
 
-from .fs import build_with_command, download, run_command, set_file_contents
+from .fs import (
+    build_with_command,
+    download,
+    run_command,
+    run_with_marker,
+    set_file_contents,
+)
 
 host_arch: Optional[str] = None
 
 _version_pattern = re.compile(r"Version: (\S+)")
 
 
 def apt_update():
-    run_command("apt-get update --allow-releaseinfo-change")
+    run_with_marker(
+        "/opt/apt-update",
+        "apt-get update --allow-releaseinfo-change",
+        deps=glob("/etc/apt/sources.list.d/*")
+        + glob("/etc/apt/trusted.gpg.d/*")
+        + ["/etc/apt/sources.list"],
+    )
 
 
 def add_trusted_key(url: str, name: str, hash: str):
     download(
         url,
         f"/etc/apt/trusted.gpg.d/{name}.gpg.asc",
         hash,
@@ -32,14 +45,15 @@
 
 # List is just "any version", Dict is a "name => min version" requirement
 def apt_install(
     packages: Union[List[str], Dict[str, Optional[str]]],
     always_install: bool = False,
     target_release: Optional[str] = None,
 ) -> bool:
+    apt_update()
     global host_arch
     if host_arch is None and packages != ["dpkg-dev"]:
         apt_install(["dpkg-dev"])
         host_arch = run_command("dpkg-architecture -q DEB_HOST_ARCH").strip()
     if isinstance(packages, List):
         packages = dict([(p, None) for p in packages])
     if always_install:
@@ -63,18 +77,14 @@
                     break
             else:
                 to_install.append(package)
 
         if to_install == []:
             return False
 
-    # Because it's probably the first run
-    if packages == {"dpkg-dev": None}:
-        apt_update()
-
     # Confdef is to fix https://unix.stackexchange.com/a/416816/73838
     os.environ["DEBIAN_FRONTEND"] = "noninteractive"
     cmd = (
         "apt-get install %s --no-install-recommends --yes -o DPkg::Options::=--force-confdef"
         % " ".join(to_install)
     )
     if target_release is not None:
```

### Comparing `paracrine-0.0.6/paracrine/deps.py` & `paracrine-0.0.7/paracrine/deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from .config import set_data
+from .helpers.config import set_data
 
 Modules = List[Union[ModuleType, Tuple[ModuleType, Dict]]]
 """Type of modules handed to `paracrine.runner.run`"""
 
 TransmitModules = List[Union[str, Tuple[str, Dict]]]
```

### Comparing `paracrine-0.0.6/paracrine/fs.py` & `paracrine-0.0.7/paracrine/helpers/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,14 +272,15 @@
         display = display.replace("  ", " ")
     changed = set_file_contents("%s.command" % fname, display) or force_build
     target_modified = last_modified(fname)
     for dep in deps:
         if last_modified(dep) > target_modified:
             logging.info("%s is younger than %s" % (dep, fname))
             changed = True
+            break
     if not os.path.exists(fname) or changed:
         logging.info("Building %s" % fname)
         if command.find("|") != -1:
             out = ""
             commands = command.split("|")
             for command in commands:
                 try:
@@ -304,14 +305,15 @@
         if age > max_age:
             changed = True
     for dep in deps:
         dep_modified = last_modified(dep)
         if dep_modified > target_modified:
             logging.info("%s is younger than %s" % (dep, fname))
             changed = True
+            break
 
     if changed:
         run_command(command, directory=directory)
         open(fname, "w").write(command)
 
     return changed
```

### Comparing `paracrine-0.0.6/paracrine/login.py` & `paracrine-0.0.7/paracrine/commands/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 import sys
 
-from .config import get_config, path_to_config_file, set_config
+from ..helpers.config import get_config, path_to_config_file, set_config
 
 
 def ssh_server(server, run="", as_root=False):
     if run != "" and as_root and server["ssh_user"] != "root":
         run = f"sudo {run}"
     command = f"ssh {server['ssh_user']}@{server['ssh_hostname']} \
         -i {path_to_config_file(server['ssh_key'])} \
```

### Comparing `paracrine-0.0.6/paracrine/network.py` & `paracrine-0.0.7/paracrine/helpers/network.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.6/paracrine/runner.py` & `paracrine-0.0.7/paracrine/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 import os
 from typing import Any, Callable, Dict
 
 from mitogen.core import Error, StreamError
 from mitogen.parent import Router
 from mitogen.utils import run_with_router
 
-from . import core
-from .config import create_data, get_config, path_to_config_file, set_config, set_data
 from .deps import Modules, TransmitModules, makereal, maketransmit, runfunc
+from .helpers.config import (
+    create_data,
+    get_config,
+    path_to_config_file,
+    set_config,
+    set_data,
+)
+from .runners import core
 
 
 def decode(info):
     for k in list(info.keys()):
         if type(k) == bytes:
             info[k.decode()] = info[k].decode()
             del info[k]
@@ -73,45 +79,37 @@
     modules = makereal(transmitmodules)
     return runfunc(modules, name)
 
 
 def internal_runner(
     router: Router, modules: Modules, local_func: str, run_func: str, parse_func: str
 ) -> None:
-    runfunc(modules, local_func)
-    infos = main(router, do, maketransmit(modules), run_func)
-    for info in infos["infos"]:
-        runfunc(modules, parse_func, info, infos["data"])
+    for module in modules:
+        runfunc([module], local_func)
+        infos = main(router, do, maketransmit([module]), run_func)
+        for info in infos["infos"]:
+            runfunc([module], parse_func, info, infos["data"])
 
 
 def run(inventory_path: str, modules: Modules):
     logging.basicConfig()
     logging.root.setLevel(logging.INFO)
     set_config(inventory_path)
 
-    modules.insert(0, core)
     needs_dependencies = list(modules)
     while len(needs_dependencies) > 0:
         new_dependencies = runfunc(needs_dependencies, "dependencies")
         needs_dependencies = []
         for item in new_dependencies.values():
             for new_dependency in item[0]:
                 if new_dependency in modules:
                     continue
                 modules.insert(0, new_dependency)
                 needs_dependencies.append(new_dependency)
+    modules.insert(0, core)
 
     print("Running:")
     for module in maketransmit(modules):
         print(f"* {module}")
     print("")
 
-    run_with_router(
-        internal_runner,
-        modules,
-        "bootstrap_local",
-        "bootstrap_run",
-        "bootstrap_parse_return",
-    )
-    run_with_router(
-        internal_runner, modules, "core_local", "core_run", "core_parse_return"
-    )
+    run_with_router(internal_runner, modules, "local", "run", "parse_return")
```

### Comparing `paracrine-0.0.6/paracrine/services/pleroma.py` & `paracrine-0.0.7/paracrine/services/pleroma.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from pathlib import Path
 
-import paracrine.certs
-from paracrine.config import build_config, core_config, get_config_file, local_config
-from paracrine.debian import apt_install
-from paracrine.deps import Modules
-from paracrine.fs import (
+from ..deps import Modules
+from ..helpers.config import build_config, core_config, get_config_file, local_config
+from ..helpers.debian import apt_install
+from ..helpers.fs import (
     download_and_unpack,
     link,
     make_directory,
     run_command,
     run_with_marker,
     set_file_contents,
     set_file_contents_from_template,
 )
-from paracrine.services import postgresql
-from paracrine.systemd import link_service, systemd_set
-from paracrine.users import adduser
+from ..helpers.systemd import link_service, systemd_set
+from ..helpers.users import adduser
+from ..runners import certs
+from . import postgresql
 
 # FIXME: Do soapbox from https://gitlab.com/soapbox-pub/soapbox/-/jobs/3371276281/artifacts/download
 # Unzipped with "unzip soapbox.zip -d instance" and then moved instance/static to /var/lib/pleroma
 # https://docs.soapbox.pub/frontend/installing/#install-soapbox
 
 
 def dependencies() -> Modules:
     LOCAL = build_config(local_config())
     return [
         postgresql,
         (
-            paracrine.certs,
+            certs,
             {"hostname": LOCAL["PLEROMA_HOST"], "email": LOCAL["PLEROMA_EMAIL"]},
         ),
     ]
 
 
-def core_run():
+def run():
     LOCAL = build_config(core_config())
     adduser("pleroma", home_dir="/opt/pleroma")
     make_directory("/opt/pleroma", owner="pleroma")
     # Taken from https://git.pleroma.social/pleroma/pleroma/-/pipelines?page=1&scope=branches&ref=stable
     res = download_and_unpack(
         "https://git.pleroma.social/pleroma/pleroma/-/jobs/220705/artifacts/download?file_type=archive",
         "8b4e2ab17362c7b0ed3ca685e19d578ad842ac00cde2db7d8c54dfd5a4e05891",
@@ -105,15 +105,15 @@
 
     apt_install(["nginx"])
 
     nginx_changes = set_file_contents_from_template(
         "/etc/nginx/sites-available/pleroma.conf",
         "pleroma.nginx.j2",
         PLEROMA_HOST=LOCAL["PLEROMA_HOST"],
-        DUMMY_CERTS=paracrine.certs.get_dummy_certs(),
+        DUMMY_CERTS=certs.get_dummy_certs(),
     )
     nginx_changes = (
         link(
             "/etc/nginx/sites-enabled/pleroma.conf",
             "/etc/nginx/sites-available/pleroma.conf",
         )
         or nginx_changes
```

### Comparing `paracrine-0.0.6/paracrine/services/postgresql.py` & `paracrine-0.0.7/paracrine/services/postgresql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
-from paracrine.debian import add_trusted_key, apt_install, debian_repo
-from paracrine.fs import make_directory, run_with_marker
-from paracrine.systemd import systemd_set
+from ..helpers.debian import add_trusted_key, apt_install, debian_repo
+from ..helpers.fs import make_directory, run_with_marker
+from ..helpers.systemd import systemd_set
 
 
-def core_run():
+def run():
     add_trusted_key(
         "https://www.postgresql.org/media/keys/ACCC4CF8.asc",
         "postgresql",
         "0144068502a1eddd2a0280ede10ef607d1ec592ce819940991203941564e8e76",
     )
     debian_repo(
         "postgresql_org_repository",
```

### Comparing `paracrine-0.0.6/paracrine/services/wireguard.py` & `paracrine-0.0.7/paracrine/services/wireguard/bootstrap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,22 @@
 import json
 import os
 import sys
 from distutils.version import LooseVersion
 
-from ..config import (
-    config,
-    config_path,
+from ...helpers.config import (
     get_config,
-    get_config_file,
     host,
+    in_docker,
     network_config,
     other_config_file,
 )
-from ..core import in_docker
-from ..debian import apt_install, apt_update
-from ..fs import make_directory, run_command, set_file_contents_from_template
-from ..network import external_ip, wireguard_ip
-from ..systemd import systemd_set
-
-wg_config = "/etc/wireguard"
-private_key_file = "{wg_config}/privatekey".format(wg_config=wg_config)
-public_key_file = "{wg_config}/publickey".format(wg_config=wg_config)
-
-
-def public_key_path(name):
-    return config_path() + "/wireguard-public-{name}.key".format(name=name)
+from ...helpers.debian import apt_install
+from ...helpers.fs import make_directory, run_command, set_file_contents
+from .common import private_key_file, public_key_file, public_key_path, wg_config
 
 
 def get_output(host, command):
     status, stdout, stderr = host.run_shell_command(command=command)
     stdout = "".join(stdout)
     assert status is True, (stdout, stderr)
     return stdout
@@ -47,28 +35,34 @@
         except ValueError:
             raise Exception("'%s'" % line)
         if status == "install ok installed":
             versions[name] = version
     return versions
 
 
-def bootstrap_run():
+def run():
     apt_install(["kmod", "wireguard"])
     modules = sorted([line.split(" ")[0] for line in run_command("lsmod").splitlines()])
-    if "wireguard" not in modules:
+    if "wireguard" not in modules and not in_docker():
         print("modules", modules)
-        apt_update()
         apt_install(["linux-image-amd64"])
         versions = get_all_kernel_versions()
+        version_keys = [
+            x.replace("linux-image-", "")
+            for x in versions.keys()
+            if x
+            not in [
+                "linux-image-amd64",
+                "linux-image-cloud-amd64",
+                "linux-image-rt-amd64",
+            ]
+        ]
+        print("kernel version keys", version_keys)
         ordered = sorted(
-            [
-                x.replace("linux-image-", "")
-                for x in versions.keys()
-                if x not in ["linux-image-amd64", "linux-image-cloud-amd64"]
-            ],
+            version_keys,
             key=LooseVersion,
             reverse=True,
         )
         highest = ordered[0]
         current = run_command("uname -r").strip()
         if current != highest:
             print(ordered)
@@ -89,55 +83,28 @@
 
     make_directory(wg_config)
     if not os.path.exists(private_key_file):
         run_command("wg genkey > %s" % private_key_file)
     if not os.path.exists(public_key_file):
         run_command("cat %s | wg pubkey > %s" % (private_key_file, public_key_file))
 
-    return {"wg_publickey": open(public_key_file).read().strip()}
+    return {
+        "wg_publickey": open(public_key_file).read().strip(),
+        "host": host()["name"],
+    }
 
 
-def bootstrap_parse_return(infos):
+def parse_return(infos):
+    assert len(infos) == 1, infos
     info = infos[0]
-    open(public_key_path(host()["name"]), "w").write(info["wg_publickey"])
+    set_file_contents(public_key_path(info["host"]), info["wg_publickey"])
 
     wg_ips = []
 
     for server in get_config()["servers"]:
         networks = network_config(server["name"])
         wireguard_networks = [
             network for network in networks if network["ifname"] == "wg0"
         ]
         if len(wireguard_networks) == 1:
             wg_ips.append(wireguard_networks[0]["addr_info"][0]["local"])
-    json.dump(wg_ips, open(other_config_file("wireguard-ips"), "w"), indent=2)
-
-
-def setup(name="wg0", ip="192.168.2.1", netmask=24, peers=[]):
-    peers = {}
-    for h in config()["servers"]:
-        if h["name"] == host()["name"]:
-            continue
-        public_key = get_config_file(public_key_path(h["name"]))
-        peers[h["name"]] = {
-            "public_key": public_key,
-            "endpoint": "%s:51820" % external_ip(h),
-            "peer_addr": h["wireguard_ip"],
-        }
-
-    conf_change = set_file_contents_from_template(
-        f"/etc/wireguard/{name}.conf",
-        "wg.conf.j2",
-        PRIVATE_KEY=open(private_key_file).read().strip(),
-        PEERS=peers,
-        IP=ip,
-        NETMASK=netmask,
-    )
-
-    systemd_set(f"wg-quick@{name}", enabled=True, restart=conf_change)
-
-
-def core_run():
-    setup(ip=wireguard_ip())
-
-
-__all__ = ["core_run", "bootstrap_run", "bootstrap_parse_return"]
+    set_file_contents(other_config_file("wireguard-ips"), json.dumps(wg_ips, indent=2))
```

### Comparing `paracrine-0.0.6/paracrine/systemd.py` & `paracrine-0.0.7/paracrine/helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.6/paracrine/templates/config.exs.j2` & `paracrine-0.0.7/paracrine/templates/config.exs.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.6/paracrine/templates/pleroma.nginx.j2` & `paracrine-0.0.7/paracrine/templates/pleroma.nginx.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.6/paracrine/users.py` & `paracrine-0.0.7/paracrine/helpers/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,11 @@
     existing_groups = groups()
     existing_group = existing_groups[group]
     if user not in existing_group:
         run_command("usermod -aG %s %s" % (group, user))
         return True
     else:
         return False
+
+
+def in_vagrant():
+    return "vagrant" in users()
```

### Comparing `paracrine-0.0.6/paracrine.egg-info/PKG-INFO` & `paracrine-0.0.7/paracrine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.6
+Version: 0.0.7
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 -----
 
 1. Setup Python. Tested against 3.8+
 2. `pip install paracrine`
 3. Write a main file describing what you want to setup. [integration_test/main.py](https://github.com/palfrey/paracrine/blob/main/integration_test/main.py) is a reasonable example. It must call the `run` function, which takes arguments for the inventory file, and list of modules to run.
 4. Write an inventory file for the machines this is managing. Current setup assumes they're all the same. [integration_test/docker/inventory.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/docker/inventory.yaml) is a reasonable example file, but I suggest generating it from whatever you're using to create the servers (e.g. Terraform).
 5. Write a `config.yaml`. This has a main top-level key of `environments` with keys below that for each inventory file you've got ([integration_test/config.yaml](https://github.com/palfrey/paracrine/blob/main/integration_test/config.yaml) just has one, but in most scenarios you'll have at least a dev and prod setup). What you do below that is up to you, but typically it'll be environment variables and secrets to feed into the main file.
-6. Run `python -m paracrine.setup <inventory file>` - this will install the minimum python bits so that everything else works.
+6. Run `python -m paracrine.commands.setup <inventory file>` - this will install the minimum python bits so that everything else works.
 7. Run the main file (e.g. `python main.py ./docker/inventory.yaml`)
 
 Limitations
 -----------
 * All the servers are assumed to be Debian Linux boxes (although Debian-derivatives like Ubuntu _should_ work)
 * Direct SSH access is assumed possible (Mitogen supports jump boxes, but there's no setup for that yet here) with keys, not passwords
 * There's no "dry run" mode yet, which would be useful for GitOps
```

### Comparing `paracrine-0.0.6/paracrine.egg-info/SOURCES.txt` & `paracrine-0.0.7/paracrine.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 paracrine/__init__.py
-paracrine/aws.py
-paracrine/certs.py
-paracrine/config.py
-paracrine/core.py
-paracrine/cron.py
-paracrine/debian.py
 paracrine/deps.py
-paracrine/fs.py
-paracrine/login.py
-paracrine/network.py
-paracrine/python.py
-paracrine/reboot.py
 paracrine/runner.py
-paracrine/setup.py
-paracrine/systemd.py
-paracrine/users.py
 paracrine.egg-info/PKG-INFO
 paracrine.egg-info/SOURCES.txt
 paracrine.egg-info/dependency_links.txt
 paracrine.egg-info/requires.txt
 paracrine.egg-info/top_level.txt
+paracrine/commands/__init__.py
+paracrine/commands/login.py
+paracrine/commands/reboot.py
+paracrine/commands/setup.py
+paracrine/helpers/__init__.py
+paracrine/helpers/config.py
+paracrine/helpers/cron.py
+paracrine/helpers/debian.py
+paracrine/helpers/fs.py
+paracrine/helpers/network.py
+paracrine/helpers/python.py
+paracrine/helpers/systemd.py
+paracrine/helpers/users.py
+paracrine/runners/__init__.py
+paracrine/runners/aws.py
+paracrine/runners/certs.py
+paracrine/runners/core.py
 paracrine/services/__init__.py
-paracrine/services/cockroachdb.py
 paracrine/services/ntp.py
 paracrine/services/pleroma.py
 paracrine/services/postgresql.py
-paracrine/services/wireguard.py
+paracrine/services/cockroachdb/__init__.py
+paracrine/services/cockroachdb/certs.py
+paracrine/services/cockroachdb/common.py
+paracrine/services/cockroachdb/init.py
+paracrine/services/cockroachdb/node.py
+paracrine/services/wireguard/__init__.py
+paracrine/services/wireguard/bootstrap.py
+paracrine/services/wireguard/common.py
+paracrine/services/wireguard/core.py
 paracrine/templates/certbot_requirements.txt
 paracrine/templates/cockroach.service.j2
 paracrine/templates/config.exs.j2
 paracrine/templates/cron.j2
 paracrine/templates/pleroma.nginx.j2
 paracrine/templates/robots.txt
 paracrine/templates/setup_db.psql.j2
```

### Comparing `paracrine-0.0.6/pyproject.toml` & `paracrine-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paracrine"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Tom Parker-Shemilt", email="palfrey@tevp.net" },
 ]
 description = "A system deployment tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,8 +19,8 @@
 "Bug Tracker" = "https://github.com/palfrey/paracrine/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["paracrine", "paracrine.services"]
+include = ["paracrine", "paracrine.services", "paracrine.services.wireguard", "paracrine.services.cockroachdb", "paracrine.commands", "paracrine.helpers", "paracrine.runners"]
```

### Comparing `paracrine-0.0.6/tests/test_ssh.py` & `paracrine-0.0.7/tests/test_ssh.py`

 * *Files identical despite different names*

