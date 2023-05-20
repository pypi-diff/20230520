# Comparing `tmp/dbm-agent-8.33.5.tar.gz` & `tmp/dbm-agent-8.33.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.33.5.tar", last modified: Wed May  3 07:49:59 2023, max compression
+gzip compressed data, was "dbm-agent-8.33.8.tar", last modified: Sat May 20 14:38:38 2023, max compression
```

## Comparing `dbm-agent-8.33.5.tar` & `dbm-agent-8.33.8.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.895332 dbm-agent-8.33.5/bin/
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.5/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.5/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.5/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2242 2023-05-03 07:49:15.000000 dbm-agent-8.33.5/bin/dbma-cli-redis
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.5/bin/dbma-cli-single-instance
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.895332 dbm-agent-8.33.5/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.896332 dbm-agent-8.33.5/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.5/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.897332 dbm-agent-8.33.5/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.5/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.5/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.5/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     6820 2023-04-29 08:19:09.000000 dbm-agent-8.33.5/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.897332 dbm-agent-8.33.5/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.5/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.898332 dbm-agent-8.33.5/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.5/dbma/components/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.898332 dbm-agent-8.33.5/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.5/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.5/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.5/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    21072 2023-04-28 07:22:47.000000 dbm-agent-8.33.5/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-24 11:29:32.000000 dbm-agent-8.33.5/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15167 2023-04-28 07:25:52.000000 dbm-agent-8.33.5/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.5/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-28 09:01:15.000000 dbm-agent-8.33.5/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.899332 dbm-agent-8.33.5/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.5/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.5/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.5/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.899332 dbm-agent-8.33.5/dbma/components/orchestrator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:32:56.000000 dbm-agent-8.33.5/dbma/components/orchestrator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 11:31:39.000000 dbm-agent-8.33.5/dbma/components/orchestrator/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-25 10:26:23.000000 dbm-agent-8.33.5/dbma/components/orchestrator/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.900332 dbm-agent-8.33.5/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.5/dbma/components/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-28 09:33:50.000000 dbm-agent-8.33.5/dbma/components/redis/commons.py
--rw-r--r--   0 root         (0) root         (0)     2751 2023-05-03 07:49:55.000000 dbm-agent-8.33.5/dbma/components/redis/config.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-04-28 08:47:44.000000 dbm-agent-8.33.5/dbma/components/redis/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7288 2023-05-03 07:49:01.000000 dbm-agent-8.33.5/dbma/components/redis/install.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-04-29 08:09:50.000000 dbm-agent-8.33.5/dbma/components/redis/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.901332 dbm-agent-8.33.5/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.5/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.901332 dbm-agent-8.33.5/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.5/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-28 05:54:34.000000 dbm-agent-8.33.5/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-28 05:39:01.000000 dbm-agent-8.33.5/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-04-22 08:57:17.000000 dbm-agent-8.33.5/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.5/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.902332 dbm-agent-8.33.5/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.902332 dbm-agent-8.33.5/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.894332 dbm-agent-8.33.5/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.907332 dbm-agent-8.33.5/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-23 03:55:41.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10688 2023-04-30 15:53:02.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10850 2023-04-30 15:52:27.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18776 2023-04-28 07:24:00.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18774 2023-04-28 09:40:34.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-03 06:34:41.000000 dbm-agent-8.33.5/dbma/static/cnfs/redis.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      710 2023-04-29 07:42:18.000000 dbm-agent-8.33.5/dbma/static/cnfs/redisd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.907332 dbm-agent-8.33.5/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-03 06:53:15.000000 dbm-agent-8.33.5/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-28 09:25:35.000000 dbm-agent-8.33.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.497565 dbm-agent-8.33.8/bin/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-mysql
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/bin/dbma-cli-redis
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.499565 dbm-agent-8.33.8/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-20 14:38:38.000000 dbm-agent-8.33.8/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.499565 dbm-agent-8.33.8/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.501565 dbm-agent-8.33.8/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.502565 dbm-agent-8.33.8/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.504565 dbm-agent-8.33.8/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.505565 dbm-agent-8.33.8/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    21072 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15167 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.506565 dbm-agent-8.33.8/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13670 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.506565 dbm-agent-8.33.8/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.509565 dbm-agent-8.33.8/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7308 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/systemd.py
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/components/redis/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.512565 dbm-agent-8.33.8/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.512565 dbm-agent-8.33.8/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      739 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.513565 dbm-agent-8.33.8/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.513565 dbm-agent-8.33.8/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.495565 dbm-agent-8.33.8/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.521565 dbm-agent-8.33.8/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18776 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/redisd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 14:38:38.521565 dbm-agent-8.33.8/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-20 14:37:15.000000 dbm-agent-8.33.8/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 14:38:38.522565 dbm-agent-8.33.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-20 14:15:43.000000 dbm-agent-8.33.8/setup.py
```

### Comparing `dbm-agent-8.33.5/PKG-INFO` & `dbm-agent-8.33.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.5
+Version: 8.33.8
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.5/README.md` & `dbm-agent-8.33.8/README.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/bin/dbm-agent` & `dbm-agent-8.33.8/bin/dbm-agent`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/bin/dbma-cli-init` & `dbm-agent-8.33.8/bin/dbma-cli-init`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/bin/dbma-cli-redis` & `dbm-agent-8.33.8/bin/dbma-cli-redis`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# -*- encoding: utf8 -*-
 
 """
 dbm-agent Redis 的命令行接口
 """
 
 import re
 import time
```

### Comparing `dbm-agent-8.33.5/bin/dbma-cli-single-instance` & `dbm-agent-8.33.8/bin/dbma-cli-mysql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.33.8/dbm_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.5
+Version: 8.33.8
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.5/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.33.8/dbm_agent.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 README.md
 setup.py
 bin/dbm-agent
 bin/dbm-bt-conn-stack
 bin/dbma-cli-init
+bin/dbma-cli-mysql
 bin/dbma-cli-redis
-bin/dbma-cli-single-instance
 dbm_agent.egg-info/PKG-INFO
 dbm_agent.egg-info/SOURCES.txt
 dbm_agent.egg-info/dependency_links.txt
 dbm_agent.egg-info/requires.txt
 dbm_agent.egg-info/top_level.txt
 dbma/__init__.py
 dbma/version.py
@@ -39,14 +39,15 @@
 dbma/components/orchestrator/install.py
 dbma/components/redis/__init__.py
 dbma/components/redis/commons.py
 dbma/components/redis/config.py
 dbma/components/redis/exceptions.py
 dbma/components/redis/install.py
 dbma/components/redis/systemd.py
+dbma/components/redis/uninstall.py
 dbma/core/__init__.py
 dbma/core/configs.py
 dbma/core/exception.py
 dbma/core/httpserver.py
 dbma/core/messages.py
 dbma/core/router.py
 dbma/core/agent/__init__.py
```

### Comparing `dbm-agent-8.33.5/dbma/bil/daemon.py` & `dbm-agent-8.33.8/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/bil/fs.py` & `dbm-agent-8.33.8/dbma/bil/fs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,48 @@
 
 """
 实现文件系统的相关操作
 """
 
 import os
 import tarfile
+from pathlib import Path
 
 
-def is_file_exists(file_path):
+def is_file_exists(file_path: Path = None):
     """
     判断文件是否存在
+
+    Parameters:
+    -----------
+    file_path: Path
+        文件|目录 的路径
+
+    Return:
+    --------
+    bool
+
+    Exceptions:
+    -----------
+    ValueError
+        file_path 为 None 时抛出
+    TypeError
+        file_path 的类型不为 str | Path 时抛出
     """
-    return os.path.exists(file_path)
+    if file_path is None:
+        raise ValueError("file_path is None , not a valid value .")
+
+    if type(file_path) not in (str, Path):
+        raise TypeError("file_path must be a str, or an Path object .")
+
+    # 如果是 str 的话要传成 Path 对象
+    if isinstance(file_path, str):
+        file_path = Path(file_path)
+
+    return file_path.exists()
 
 
 def extract_tar_file(tar_file_path, extract_dir):
     """
     解压tar文件
 
     Parameters:
```

### Comparing `dbm-agent-8.33.5/dbma/bil/net.py` & `dbm-agent-8.33.8/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/bil/osuser.py` & `dbm-agent-8.33.8/dbma/bil/osuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,21 +182,20 @@
         在创建用户的时候如果组不存在，要去创建组
         """
         if (self.group is not None) and (not self.group.is_exists()):
             self.group.create()
         Identify.create(self)
 
     def chown(self, path, recursive=True):
-        """ """
-        logging.info("execute User.chown.")
+        """调用 chown 命令"""
         if recursive == True:
             cmd = f"chown -R {str(self)} {path}"
         else:
             cmd = f"chown {str(self)} {path}"
-        logging.info(cmd)
+        logging.debug(cmd)
         with sudo():
             exe_shell_cmd(cmd)
 
     def __str__(self):
         """
         返回 user:group 的形式
         """
```

### Comparing `dbm-agent-8.33.5/dbma/bil/sudos.py` & `dbm-agent-8.33.8/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.33.8/dbma/components/mysql/backups/cloneplugin.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/commons.py` & `dbm-agent-8.33.8/dbma/components/mysql/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/config.py` & `dbm-agent-8.33.8/dbma/components/mysql/config.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/exceptions.py` & `dbm-agent-8.33.8/dbma/components/mysql/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/install.py` & `dbm-agent-8.33.8/dbma/components/mysql/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/instance.py` & `dbm-agent-8.33.8/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/replica.py` & `dbm-agent-8.33.8/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/source.py` & `dbm-agent-8.33.8/dbma/components/mysql/source.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.33.8/dbma/components/mysql/views/defaultsview.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.33.8/dbma/components/mysql/views/handlers.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/orchestrator/install.py` & `dbm-agent-8.33.8/dbma/components/orchestrator/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/redis/config.py` & `dbm-agent-8.33.8/dbma/components/redis/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,16 @@
         Redis 要监控的端口
     """
 
     port: int = 6379
     dbfilename: str = "dump.rdb"
     loglevel: str = "notice"
     daemonize: str = "yes"
-    bind: str = "127.0.0.1 ::1"
+    # bind: str = "127.0.0.1 ::1"
+    bind: str = "* -::*"
     redis_dir: str = "/database/redis/{}".format(port)
     protected_mode: str = "yes"
     tcp_backlog: int = 511
     unixsocketperm: str = "700"
     tcp_keepalive: int = 300
     now: str = datetime.now().isoformat()
```

### Comparing `dbm-agent-8.33.5/dbma/components/redis/exceptions.py` & `dbm-agent-8.33.8/dbma/components/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/components/redis/install.py` & `dbm-agent-8.33.8/dbma/components/redis/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- encoding: utf-8 -*-
 
-"""Resdis 单机环境的安装"""
+"""Redis 环境的安装"""
 
 
 import os
 import tarfile
 import logging
 from pathlib import Path
 from dbma.core import messages
@@ -96,15 +96,15 @@
     """
     logging.info(messages.FUN_STARTS.format(fname()))
 
     # 1. 确认当前 redis 的版本号
     m = redis_pkg_re_pattern.match(pkg.name)
     if m is None:
         logging.error(messages.FUN_ENDS.format(fname()))
-        raise ValueError("redis pkg name error .")
+        raise ValueError("redis pkg name error pkg-name = '{}'.".format(pkg))
     version = m.group("redis_version")
 
     # 2. 返回 redis 版本应该对应的 basedir
     logging.info(messages.FUN_ENDS.format(fname()))
     return Path("/usr/local/redis-{}".format(version))
```

### Comparing `dbm-agent-8.33.5/dbma/components/redis/systemd.py` & `dbm-agent-8.33.8/dbma/components/redis/systemd.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/core/agent/init.py` & `dbm-agent-8.33.8/dbma/core/agent/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,61 +9,113 @@
 import shutil
 import logging
 import atexit
 from pathlib import Path
 from dbma.bil.osuser import DBMAUser
 from dbma.core.configs import DBM_AGENT_BASE_DIR, DBMAgentConfig
 from dbma.bil.net import get_ip_by_card_name
+from dbma.core.exception import NetCardNotExistsException
 
 
-def init(net_card_name: str, dbm_center_url_prefix: str):
-    """安装 dbm-agent"""
-    # 配置日志
-    logging.basicConfig(
-        level=logging.INFO,
-        format="[%(asctime)s %(levelname)s] - [%(threadName)s] - [%(pathname)s %(lineno)d line]  ~  %(message)s",
-    )
-    logging.info("start install dbm-agent .")
-
-    # 检查给定的网卡是否存在
+def has_net_card_exists(net_card_name: str):
+    """
+    检查给定的网卡是否存在
+    返回 True 说明给定的网卡存在，如果网卡不存在那么就会报异常 NetCardNotExistsException
+
+    Parameters:
+    -----------
+    net_card_name: str
+
+    Returns:
+    --------
+    bool
+
+    Exceptions:
+    -----------
+    NetCardNotExistsException
+    """
     ip = get_ip_by_card_name(net_card_name)
     if ip is None:
         logging.error("not find any ip on {}".format(net_card_name))
-        return
+        raise NetCardNotExistsException(
+            "net card '{}' not exists".format(net_card_name)
+        )
+    return True
 
-    # 创建用户
+
+def create_dbma_user():
+    """
+    创建 dbma 用户
+    """
     logging.info("prepare create user dbma .")
     dbma_user = DBMAUser()
     dbma_user.create()
     logging.info("create user dbma done .")
+    return dbma_user
 
-    # 创建目录和子目录
+
+def create_dbm_agent_and_database_directorys():
+    """
+    创建 /usr/local/dbm-agent/*
+        /database/mysql/*
+        /database/redis/*
+    这三个目录和它的子目标
+    """
     logging.info("prepare create directions .")
     if not DBM_AGENT_BASE_DIR.exists():
         DBM_AGENT_BASE_DIR.mkdir()
 
     for subdir in ("etc", "pkgs", "logs", "etc/templates"):
         item = DBM_AGENT_BASE_DIR / subdir
         if not item.exists():
+            logging.info("go to create dir {} .".format(item))
+            item.mkdir()
+
+    # 创建 MySQL+Redis 会用的的一些公共目录
+    DATABASE_DIR = Path("/database")
+    for subdir in ("mysql", "mysql/data", "mysql/binlog", "redis"):
+        item = DATABASE_DIR / subdir
+        if not item.exists():
+            logging.info("go to create dir {} .".format(item))
             item.mkdir()
+
     logging.info("create directions done .")
 
-    # 复制模板文件
-    logging.info("prepare copy template files .")
-    import dbma
-
-    basedir = Path(dbma.__file__).parent
-    src = basedir / "static/cnfs/"
-    dest = DBM_AGENT_BASE_DIR / "etc/templates"
-    shutil.copytree(src, dest, dirs_exist_ok=True)
-    logging.info("copy template files done .")
+
+def init(net_card_name: str, dbm_center_url_prefix: str):
+    """安装 dbm-agent"""
+    # 配置日志
+    logging.basicConfig(
+        level=logging.INFO,
+        format="[%(asctime)s %(levelname)s] - [%(threadName)s] - [%(pathname)s %(lineno)d line]  ~  %(message)s",
+    )
+    logging.info("start install dbm-agent .")
+
+    # 检查给定的网卡是否存在
+    has_net_card_exists(net_card_name)
+
+    # 创建用户
+    dbma_user = create_dbma_user()
+
+    # 创建目录和子目录
+    create_dbm_agent_and_database_directorys()
+
+    # # 复制模板文件
+    # logging.info("prepare copy template files .")
+    # import dbma
+
+    # basedir = Path(dbma.__file__).parent
+    # src = basedir / "static/cnfs/"
+    # dest = DBM_AGENT_BASE_DIR / "etc/templates"
+    # shutil.copytree(src, dest, dirs_exist_ok=True)
+    # logging.info("copy template files done .")
 
     # 更新配置并保存到磁盘
     dbm_agent_config = DBMAgentConfig()
-    dbm_agent_config.host = ip
+    dbm_agent_config.host = get_ip_by_card_name(net_card_name)
     dbm_agent_config.dbmcenter_url_prefix = dbm_center_url_prefix
     dbm_agent_config.sync_to_disk()
 
     ## 权限调整
     dbma_user.chown(DBM_AGENT_BASE_DIR)
 
     # 给到启动 dbm-agent 的命令提示
```

### Comparing `dbm-agent-8.33.5/dbma/core/configs.py` & `dbm-agent-8.33.8/dbma/core/configs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/core/exception.py` & `dbm-agent-8.33.8/dbma/core/exception.py`

 * *Files 23% similar despite different names*

```diff
@@ -39,7 +39,17 @@
 class DirectoryNotExistsException(DBMAgentException):
     """目录不存在的异常"""
 
     pass
 
 
 # endregion directorys
+
+
+# region netcards
+class NetCardNotExistsException(DBMAgentException):
+    """网卡不存在"""
+
+    pass
+
+
+# endregion netcards
```

### Comparing `dbm-agent-8.33.5/dbma/core/httpserver.py` & `dbm-agent-8.33.8/dbma/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/core/messages.py` & `dbm-agent-8.33.8/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/core/threads/backends.py` & `dbm-agent-8.33.8/dbma/core/threads/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from requests.exceptions import ConnectionError
 from concurrent.futures import ThreadPoolExecutor
 from dbma.core.configs import DBMAgentConfig, DBMCenterUrlConfig
 
 keep_threads_running = True
 dbm_center_url_config = DBMCenterUrlConfig()
 dbm_agent_config = DBMAgentConfig()
-threads = ThreadPoolExecutor(max_workers=2, thread_name_prefix="backends")
+threads = ThreadPoolExecutor(max_workers=8, thread_name_prefix="backends")
 
 
 def registor_agent_to_center():
     """注册 agent 的信息到 dbm-center"""
     while keep_threads_running:
         try:
             logging.info(
```

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.33.8/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.33.8/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.33.8/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -202,25 +202,25 @@
 innodb_fsync_threshold                   = {{innodb_fsync_threshold}}
 innodb_fill_factor                       = {{innodb_fill_factor}}
 innodb_file_per_table                    = {{innodb_file_per_table}}
 sql_generate_invisible_primary_key       = {{sql_generate_invisible_primary_key}} 
 innodb_autoextend_increment              = {{innodb_autoextend_increment}}
 innodb_open_files                        = {{innodb_open_files}}
 innodb_buffer_pool_chunk_size            = {{innodb_buffer_pool_chunk_size}}
-innodb_buffer_pool_instances             = {{innodb_buffer_pool_instances}}
+innodb_buffer_pool_instances             = 1
 #innodb_log_files_in_group               = {{innodb_log_files_in_group}}
 #innodb_log_file_size                    = {{innodb_log_file_size}}
 innodb_redo_log_capacity                 = {{innodb_redo_log_capacity}}
 innodb_flush_neighbors                   = {{innodb_flush_neighbors}}
 innodb_io_capacity                       = {{innodb_io_capacity}}
 innodb_io_capacity_max                   = {{innodb_io_capacity_max}}
 innodb_autoinc_lock_mode                 = {{innodb_autoinc_lock_mode}}
 innodb_change_buffer_max_size            = {{innodb_change_buffer_max_size}}
 innodb_flush_method                      = {{innodb_flush_method}}
-innodb_log_buffer_size                   = {{innodb_log_buffer_size}}
+innodb_log_buffer_size                   = 128MB
 innodb_flush_log_at_trx_commit           = {{innodb_flush_log_at_trx_commit}}
 innodb_buffer_pool_size                  = {{innodb_buffer_pool_size}}
 
 
 ####  for performance_schema
 performance_schema                                                      ={{performance_schema}}  
 performance_schema_consumer_global_instrumentation                      =ON
```

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.33.cnf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/redis.conf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/redis.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/redisd.service.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/redisd.service.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.33.8/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.33.8/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.5/setup.py` & `dbm-agent-8.33.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     description="dbm-agent 数据库管理中心客户端程序",
     author="Neeky",
     author_email="neeky@live.com",
     maintainer="Neeky",
     maintainer_email="neeky@live.com",
     scripts=[
         "bin/dbm-agent",
-        "bin/dbma-cli-single-instance",
         "bin/dbma-cli-init",
+        "bin/dbma-cli-mysql",
         "bin/dbma-cli-redis",
         "bin/dbm-bt-conn-stack",
     ],
     packages=[
         "dbma",
         "dbma/core",
         "dbma/core/views",
@@ -48,20 +48,21 @@
         "dbma/components/mysql/backups",
         "dbma/components/redis",
         "dbma/components/orchestrator",
     ],
     package_data={"dbma": ["static/cnfs/*", "static/sql-scripts/*"]},
     url="https://github.com/Neeky/dbm-agent",
     install_requires=[
-        "Jinja2>=2.10.1",
         "mysql-connector-python>=8.0.31",
-        "psutil>=5.6.6",
+        "redis>=4.5.4",
+        "aiohttp>=3.8.1",
         "requests>=2.22.0",
+        "Jinja2>=2.10.1",
+        "psutil>=5.6.6",
         "distro>=1.4.0",
-        "aiohttp>=3.8.1",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3.8",
```

