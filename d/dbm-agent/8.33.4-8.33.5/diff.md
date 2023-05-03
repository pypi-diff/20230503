# Comparing `tmp/dbm-agent-8.33.4.tar.gz` & `tmp/dbm-agent-8.33.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.33.4.tar", last modified: Mon May  1 08:47:32 2023, max compression
+gzip compressed data, was "dbm-agent-8.33.5.tar", last modified: Wed May  3 07:49:59 2023, max compression
```

## Comparing `dbm-agent-8.33.4.tar` & `dbm-agent-8.33.5.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.281857 dbm-agent-8.33.4/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-01 08:47:32.281857 dbm-agent-8.33.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.268857 dbm-agent-8.33.4/bin/
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.4/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.4/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.4/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     1162 2023-04-29 08:15:51.000000 dbm-agent-8.33.4/bin/dbma-cli-redis
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.4/bin/dbma-cli-single-instance
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.269857 dbm-agent-8.33.4/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-01 08:47:32.000000 dbm-agent-8.33.4/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-01 08:47:32.000000 dbm-agent-8.33.4/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 08:47:32.000000 dbm-agent-8.33.4/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-01 08:47:32.000000 dbm-agent-8.33.4/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-01 08:47:32.000000 dbm-agent-8.33.4/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.269857 dbm-agent-8.33.4/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.4/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.270857 dbm-agent-8.33.4/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.4/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.4/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.4/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     6820 2023-04-29 08:19:09.000000 dbm-agent-8.33.4/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.270857 dbm-agent-8.33.4/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.4/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.271857 dbm-agent-8.33.4/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.4/dbma/components/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.272857 dbm-agent-8.33.4/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.4/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.4/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.4/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    21072 2023-04-28 07:22:47.000000 dbm-agent-8.33.4/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-24 11:29:32.000000 dbm-agent-8.33.4/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15167 2023-04-28 07:25:52.000000 dbm-agent-8.33.4/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.4/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-28 09:01:15.000000 dbm-agent-8.33.4/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.272857 dbm-agent-8.33.4/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.4/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.4/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.4/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.272857 dbm-agent-8.33.4/dbma/components/orchestrator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:32:56.000000 dbm-agent-8.33.4/dbma/components/orchestrator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 11:31:39.000000 dbm-agent-8.33.4/dbma/components/orchestrator/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-25 10:26:23.000000 dbm-agent-8.33.4/dbma/components/orchestrator/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.273857 dbm-agent-8.33.4/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.4/dbma/components/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-28 09:33:50.000000 dbm-agent-8.33.4/dbma/components/redis/commons.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-29 08:28:15.000000 dbm-agent-8.33.4/dbma/components/redis/config.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-04-28 08:47:44.000000 dbm-agent-8.33.4/dbma/components/redis/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5980 2023-04-29 08:32:41.000000 dbm-agent-8.33.4/dbma/components/redis/install.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-04-29 08:09:50.000000 dbm-agent-8.33.4/dbma/components/redis/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.274857 dbm-agent-8.33.4/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.4/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.275857 dbm-agent-8.33.4/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.4/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.4/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-28 05:54:34.000000 dbm-agent-8.33.4/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-28 05:39:01.000000 dbm-agent-8.33.4/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-04-22 08:57:17.000000 dbm-agent-8.33.4/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.4/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.4/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.275857 dbm-agent-8.33.4/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.4/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.4/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.275857 dbm-agent-8.33.4/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.4/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.4/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.267857 dbm-agent-8.33.4/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.280857 dbm-agent-8.33.4/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.4/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-23 03:55:41.000000 dbm-agent-8.33.4/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10688 2023-04-30 15:53:02.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10850 2023-04-30 15:52:27.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18776 2023-04-28 07:24:00.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18774 2023-04-28 09:40:34.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.4/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-29 08:25:25.000000 dbm-agent-8.33.4/dbma/static/cnfs/redis.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      710 2023-04-29 07:42:18.000000 dbm-agent-8.33.4/dbma/static/cnfs/redisd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:47:32.280857 dbm-agent-8.33.4/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.4/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-01 08:46:12.000000 dbm-agent-8.33.4/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 08:47:32.281857 dbm-agent-8.33.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-28 09:25:35.000000 dbm-agent-8.33.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.895332 dbm-agent-8.33.5/bin/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.5/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.5/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.5/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-05-03 07:49:15.000000 dbm-agent-8.33.5/bin/dbma-cli-redis
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.5/bin/dbma-cli-single-instance
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.895332 dbm-agent-8.33.5/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-03 07:49:59.000000 dbm-agent-8.33.5/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.896332 dbm-agent-8.33.5/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.5/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.897332 dbm-agent-8.33.5/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.5/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.5/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.5/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-04-29 08:19:09.000000 dbm-agent-8.33.5/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.897332 dbm-agent-8.33.5/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.5/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.898332 dbm-agent-8.33.5/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.5/dbma/components/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.898332 dbm-agent-8.33.5/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.5/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.5/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.5/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    21072 2023-04-28 07:22:47.000000 dbm-agent-8.33.5/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-24 11:29:32.000000 dbm-agent-8.33.5/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15167 2023-04-28 07:25:52.000000 dbm-agent-8.33.5/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.5/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-28 09:01:15.000000 dbm-agent-8.33.5/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.899332 dbm-agent-8.33.5/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.5/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.5/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.5/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.899332 dbm-agent-8.33.5/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:32:56.000000 dbm-agent-8.33.5/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 11:31:39.000000 dbm-agent-8.33.5/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-25 10:26:23.000000 dbm-agent-8.33.5/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.900332 dbm-agent-8.33.5/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.5/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-28 09:33:50.000000 dbm-agent-8.33.5/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-05-03 07:49:55.000000 dbm-agent-8.33.5/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-04-28 08:47:44.000000 dbm-agent-8.33.5/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7288 2023-05-03 07:49:01.000000 dbm-agent-8.33.5/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-04-29 08:09:50.000000 dbm-agent-8.33.5/dbma/components/redis/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.901332 dbm-agent-8.33.5/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.5/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.901332 dbm-agent-8.33.5/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.5/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.5/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-28 05:54:34.000000 dbm-agent-8.33.5/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-28 05:39:01.000000 dbm-agent-8.33.5/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-04-22 08:57:17.000000 dbm-agent-8.33.5/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.5/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.902332 dbm-agent-8.33.5/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.902332 dbm-agent-8.33.5/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.5/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.894332 dbm-agent-8.33.5/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.907332 dbm-agent-8.33.5/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-23 03:55:41.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-04-30 15:53:02.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-04-30 15:52:27.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18776 2023-04-28 07:24:00.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-04-28 09:40:34.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.5/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-03 06:34:41.000000 dbm-agent-8.33.5/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-04-29 07:42:18.000000 dbm-agent-8.33.5/dbma/static/cnfs/redisd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:49:59.907332 dbm-agent-8.33.5/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.5/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-03 06:53:15.000000 dbm-agent-8.33.5/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:49:59.908332 dbm-agent-8.33.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-28 09:25:35.000000 dbm-agent-8.33.5/setup.py
```

### Comparing `dbm-agent-8.33.4/PKG-INFO` & `dbm-agent-8.33.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.4
+Version: 8.33.5
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.4/README.md` & `dbm-agent-8.33.5/README.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/bin/dbm-agent` & `dbm-agent-8.33.5/bin/dbm-agent`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/bin/dbma-cli-init` & `dbm-agent-8.33.5/bin/dbma-cli-init`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/bin/dbma-cli-single-instance` & `dbm-agent-8.33.5/bin/dbma-cli-single-instance`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.33.5/dbm_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.4
+Version: 8.33.5
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.33.4/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.33.5/dbm_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/bil/daemon.py` & `dbm-agent-8.33.5/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/bil/fs.py` & `dbm-agent-8.33.5/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/bil/net.py` & `dbm-agent-8.33.5/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/bil/osuser.py` & `dbm-agent-8.33.5/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/bil/sudos.py` & `dbm-agent-8.33.5/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.33.5/dbma/components/mysql/backups/cloneplugin.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/commons.py` & `dbm-agent-8.33.5/dbma/components/mysql/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/config.py` & `dbm-agent-8.33.5/dbma/components/mysql/config.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/exceptions.py` & `dbm-agent-8.33.5/dbma/components/mysql/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/install.py` & `dbm-agent-8.33.5/dbma/components/mysql/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/instance.py` & `dbm-agent-8.33.5/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/replica.py` & `dbm-agent-8.33.5/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/source.py` & `dbm-agent-8.33.5/dbma/components/mysql/source.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.33.5/dbma/components/mysql/views/defaultsview.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.33.5/dbma/components/mysql/views/handlers.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/orchestrator/install.py` & `dbm-agent-8.33.5/dbma/components/orchestrator/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/redis/commons.py` & `dbm-agent-8.33.5/dbma/components/redis/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/redis/config.py` & `dbm-agent-8.33.5/dbma/components/redis/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,7 +77,21 @@
 
     def generate_config_file(self):
         """生成配置文件 /etc/redis-{self.port}.conf"""
         config_file = "/etc/redis-{}.conf".format(self.port)
         with open(config_file, "w") as config_object:
             content = self.render_config()
             config_object.write(content)
+
+
+@dataclass
+class RedisReplicaConfig(RedisConfig):
+    """Redis 从结点配置文件生成类
+
+    Parameters
+    ----------
+    RedisConfig :
+    """
+
+    is_replica: bool = True
+    # format et: 127.0.0.1 6379
+    replicaof: str = ""
```

### Comparing `dbm-agent-8.33.4/dbma/components/redis/exceptions.py` & `dbm-agent-8.33.5/dbma/components/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/components/redis/install.py` & `dbm-agent-8.33.5/dbma/components/redis/install.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- encoding: utf-8 -*-
 
 """Resdis 单机环境的安装"""
 
 
 import os
-import re
-import shutil
 import tarfile
 import logging
 from pathlib import Path
 from dbma.core import messages
 from dbma.bil.fun import fname
 from dbma.bil.osuser import RedisUser
 from dbma.components.redis.exceptions import (
@@ -18,15 +16,15 @@
 )
 from dbma.components.redis.commons import (
     default_redis_pkg,
     redis_pkg_re_pattern,
     default_redis_port,
 )
 from dbma.bil.cmdexecutor import exe_shell_cmd
-from dbma.components.redis.config import RedisConfig
+from dbma.components.redis.config import RedisConfig, RedisReplicaConfig
 from dbma.components.redis.systemd import RedisSystemdConfig
 
 
 def create_redis_user(port: int = 6379):
     """创建 redis 用户"""
     logging.info(messages.FUN_STARTS.format(fname()))
 
@@ -177,15 +175,17 @@
     ----------
     port : int, optional
         Redis 端口号, by default 6379
     """
     exe_shell_cmd("systemctl stop redisd-{}".format(port))
 
 
-def install_redis(port: int = 6379, pkg: Path = default_redis_pkg):
+def install_redis(
+    port: int = 6379, pkg: Path = default_redis_pkg, redis_config: RedisConfig = None
+):
     """安装 Redis 并让其监控到指定端口
 
     Parameters:
     -----------
     port : int, optional
         Redis 要监听的端口号, by default 6379
     pkg : Path, optional
@@ -199,18 +199,58 @@
         # 第一步：创建用户
         create_redis_user(port)
         # 第二步：创建数据目录
         create_redis_database_dir(port)
         # 第三步：解压
         decompression_redis_pkg(pkg)
         # 第四步：生成配置
-        redis_config = RedisConfig(port)
         redis_config.generate_config_file()
         # 第五步：生成 systemd 配置
         redis_systemd_config = RedisSystemdConfig(port, pkg_to_redis_basedir(pkg))
         redis_systemd_config.generate_systemd_config()
         # 第六步：启动 redis
         start_redis(port)
     except Exception as err:
         msg = str(err)
         logging.exception(err)
         raise err
+
+
+def install_resdis_master(port: int = 6379, pkg: Path = default_redis_pkg):
+    """安装 Redis master 结点
+
+    Parameters
+    ----------
+    port : int, optional
+        Redis 端口号, by default 6379
+    pkg : Path, optional
+        Redis 安装包, by default default_redis_pkg
+    """
+    logging.info(messages.FUN_STARTS.format(fname()))
+
+    redis_master_config = RedisConfig(port)
+    install_redis(port, pkg=pkg, redis_config=redis_master_config)
+
+    logging.info(messages.FUN_ENDS.format(fname()))
+
+
+def install_redis_replica(
+    port: int = 6379, replicaof: str = "127.0.0.1 6379", pkg: Path = default_redis_pkg
+):
+    """安装 Redis replica 结点
+
+    Parameters
+    ----------
+    port : int, optional
+        Redis 结点的端口号, by default 6379
+    master : str, optional
+        Redis Master 结点的标识("host port"), by default "127.0.0.1 6379"
+    pkg : Path, optional
+        Redis 的安装包, by default default_redis_pkg
+    """
+    logging.info(messages.FUN_STARTS.format(fname()))
+    logging.info("redis-port={}, redis-master={}, pkg={}".format(port, replicaof, pkg))
+
+    redis_replica_config = RedisReplicaConfig(port=port, replicaof=replicaof)
+    install_redis(port, pkg=pkg, redis_config=redis_replica_config)
+
+    logging.info(messages.FUN_ENDS.format(fname()))
```

### Comparing `dbm-agent-8.33.4/dbma/components/redis/systemd.py` & `dbm-agent-8.33.5/dbma/components/redis/systemd.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/agent/init.py` & `dbm-agent-8.33.5/dbma/core/agent/init.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/configs.py` & `dbm-agent-8.33.5/dbma/core/configs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/exception.py` & `dbm-agent-8.33.5/dbma/core/exception.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/httpserver.py` & `dbm-agent-8.33.5/dbma/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/messages.py` & `dbm-agent-8.33.5/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/core/threads/backends.py` & `dbm-agent-8.33.5/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.33.5/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.33.5/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.33.5/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/mysql-8.0.33.cnf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/redis.conf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/redis.conf.jinja`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Redis configuration file
 # redis-server /path/to/redis.conf
 
+# for basic
 port        {{port}}
 daemonize   {{daemonize}}
 bind        {{bind}}
 dir         {{redis_dir}}
 
 
 unixsocket  {{redis_dir}}/redis.sock
@@ -14,14 +15,19 @@
 loglevel    {{loglevel}}
 
 protected-mode  {{protected_mode}}
 tcp-backlog     {{tcp_backlog}}
 unixsocketperm  700
 tcp-keepalive   300
 
+{% if is_replica %}
+# for replica
+replicaof {{replicaof}}
+{% endif %}
+
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
 # base on redis-7.0.11
 # generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
```

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/redisd.service.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/redisd.service.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.33.5/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.33.5/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.4/setup.py` & `dbm-agent-8.33.5/setup.py`

 * *Files identical despite different names*

