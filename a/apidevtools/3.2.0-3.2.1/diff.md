# Comparing `tmp/apidevtools-3.2.0.tar.gz` & `tmp/apidevtools-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.2.0.tar", last modified: Sat Apr 22 17:48:14 2023, max compression
+gzip compressed data, was "apidevtools-3.2.1.tar", last modified: Wed May  3 11:57:54 2023, max compression
```

## Comparing `apidevtools-3.2.0.tar` & `apidevtools-3.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.542450 apidevtools-3.2.0/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-04-22 17:48:14.542450 apidevtools-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.0/README.md
--rw-rw-rw-   0        0        0     1774 2023-04-22 17:46:53.000000 apidevtools-3.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 17:48:14.542450 apidevtools-3.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.321451 apidevtools-3.2.0/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.339450 apidevtools-3.2.0/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.0/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.0/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.370485 apidevtools-3.2.0/src/apidevtools/media/
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.0/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.2.0/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.0/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.386451 apidevtools-3.2.0/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.0/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.0/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.401451 apidevtools-3.2.0/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.431484 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-03-21 23:30:17.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6604 2023-04-22 17:44:37.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     1792 2023-03-29 11:40:43.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.448485 apidevtools-3.2.0/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.0/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.460490 apidevtools-3.2.0/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.316451 apidevtools-3.2.0/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.461451 apidevtools-3.2.0/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.467485 apidevtools-3.2.0/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.482485 apidevtools-3.2.0/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.504451 apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.526450 apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.541450 apidevtools-3.2.0/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.0/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.0/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:48:14.357450 apidevtools-3.2.0/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-04-22 17:48:14.000000 apidevtools-3.2.0/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-04-22 17:48:14.000000 apidevtools-3.2.0/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 17:48:14.000000 apidevtools-3.2.0/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-22 17:48:14.000000 apidevtools-3.2.0/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-22 17:48:14.000000 apidevtools-3.2.0/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.912418 apidevtools-3.2.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-05-03 11:57:54.911419 apidevtools-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.1/README.md
+-rw-rw-rw-   0        0        0     1774 2023-05-03 11:56:08.000000 apidevtools-3.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:57:54.912418 apidevtools-3.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.640179 apidevtools-3.2.1/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.659180 apidevtools-3.2.1/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.1/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.1/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.692183 apidevtools-3.2.1/src/apidevtools/media/
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.1/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.2.1/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.1/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.737222 apidevtools-3.2.1/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.1/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.1/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.749220 apidevtools-3.2.1/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.781220 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6651 2023-05-03 11:55:37.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.798252 apidevtools-3.2.1/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.812321 apidevtools-3.2.1/src/apidevtools/template/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/create.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.636180 apidevtools-3.2.1/src/apidevtools/template/template/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.813321 apidevtools-3.2.1/src/apidevtools/template/template/api/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.820420 apidevtools-3.2.1/src/apidevtools/template/template/api/build/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/build/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/build/compose.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.837421 apidevtools-3.2.1/src/apidevtools/template/template/api/src/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/app.py
+-rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/const.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.866418 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/
+-rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/auth.py
+-rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/item.py
+-rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/user.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.893420 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/
+-rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/auth.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/item.py
+-rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/user.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.910419 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/__init__.py
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/item.py
+-rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/user.py
+-rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template.zip
+-rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.1/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.678213 apidevtools-3.2.1/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.2.0/LICENSE.txt` & `apidevtools-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/PKG-INFO` & `apidevtools-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.0
+Version: 3.2.1
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.0/README.md` & `apidevtools-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/pyproject.toml` & `apidevtools-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.2.0"
+version = "3.2.1"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
```

### Comparing `apidevtools-3.2.0/src/apidevtools/logman.py` & `apidevtools-3.2.1/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/media/imgproc.py` & `apidevtools-3.2.1/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/media/telegraph.py` & `apidevtools-3.2.1/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/security/encryptor.py` & `apidevtools-3.2.1/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/security/hasher.py` & `apidevtools-3.2.1/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         records = Records(await self.connector.fetchall(query, args), record_t)
         if rel_depth and _is_dict(record_t):
             self.logger.warning(f'`ORM.select(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and rel_depth else ():
             for relation in record.relations():
                 query, args = await self.connector._constructor__select_relations(relation)
                 instances = await (await self.select(query, args, relation.rel_schema_t, rel_depth=rel_depth - 1)).all()
-                records = await self.__attach_instances(records, record, relation, instances, index)
+                records, record = await self.__attach_instances(records, record, relation, instances, index)
         return records
 
     async def insert(
             self,
             instance: Instance, record_t: RecordType = dict[str, Any], tablename: str = None
     ) -> Record:
         instance, tablename = await self.__parse_parameters(instance, tablename)
@@ -67,15 +67,15 @@
         records = Records(await self.connector.fetchall(query, args), record_t)
         if rel_depth and _is_dict(record_t):
             self.logger.warning(f'`ORM.update(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and rel_depth else ():
             for relation in record.relations():
                 query, args = await self.connector._constructor__select_relations(relation)
                 instances = await (await self.select(query, args, relation.rel_schema_t, rel_depth=rel_depth - 1)).all()
-                records = await self.__attach_instances(records, record, relation, instances, index)
+                records, record = await self.__attach_instances(records, record, relation, instances, index)
         return records
 
     async def delete(
             self,
             instance: Instance, record_t: RecordType = dict[str, Any], tablename: str = None,
             *, rel_depth: int = 0, del_depth: int = INF
     ) -> Records:
@@ -88,29 +88,29 @@
             self.logger.warning(f'`ORM.delete(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and del_depth else ():
             for relation in record.relations():
                 instances = await (await self.delete(
                     relation.where, relation.rel_schema_t, relation.rel_schema_t.__tablename__, del_depth=del_depth - 1
                 )).all()
                 if rel_depth:
-                    records = await self.__attach_instances(records, record, relation, instances, index)
+                    records, record = await self.__attach_instances(records, record, relation, instances, index)
         await self.connector.execute(*(await self.connector._constructor__delete_instances(instance, tablename)))
         return records
 
     async def __attach_instances(
             self,
             records: Records, record: Record, relation: Relation, instances: list[Schema], index: int
-    ) -> Records:
+    ) -> tuple[Records, Record]:
         if isinstance(record, dict):
             record[relation.propname] = instances
         elif isinstance(record, Schema):
             record = relation.ext_schema_t(**dict(record))
             setattr(record, relation.propname, instances)
         records._records[index] = relation.ext_schema_t(**dict(record))
-        return records
+        return records, record
 
     async def __parse_parameters(
             self,
             instance: Instance, tablename: str
     ) -> tuple[dict[str, Any], str]:
         if isinstance(instance, Schema):
             tablename = instance.__tablename__
```

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,7 +49,16 @@
     async def get(self, key: Any, convert: bool = False) -> bytes | None:
         try:
             value = await self.pool.get(str(key))
             return _evaluate(value, convert)
         except Exception as error:
             self.logger.error(error)
             return None
+
+    async def delete(self, key: Any, convert: bool = False) -> bytes | None:
+        try:
+            value = await self.pool.delete(str(key))
+            return _evaluate(value, convert)
+        except Exception as error:
+            self.logger.error(error)
+            return None
+
```

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.2.1/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/create.py` & `apidevtools-3.2.1/src/apidevtools/template/create.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/app.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/app.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/const.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/const.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/auth.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/item.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/crud/user.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/auth.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/item.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/routers/user.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template/api/src/schemas/user.py` & `apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/template/template.zip` & `apidevtools-3.2.1/src/apidevtools/template/template.zip`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools/utils.py` & `apidevtools-3.2.1/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.0/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.2.1/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.0
+Version: 3.2.1
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.0/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.2.1/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

