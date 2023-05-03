# Comparing `tmp/halborn_ctf-0.1.4.tar.gz` & `tmp/halborn_ctf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halborn_ctf-0.1.4.tar", last modified: Tue May  2 18:12:19 2023, max compression
+gzip compressed data, was "halborn_ctf-0.1.5.tar", last modified: Wed May  3 09:34:41 2023, max compression
```

## Comparing `halborn_ctf-0.1.4.tar` & `halborn_ctf-0.1.5.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.601361 halborn_ctf-0.1.4/
--rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.coveragerc
--rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.readthedocs.yml
--rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/AUTHORS.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/CHANGELOG.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/LICENSE.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-02 18:12:19.601444 halborn_ctf-0.1.4/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.4/README.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.594621 halborn_ctf-0.1.4/docs/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/Makefile
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.594998 halborn_ctf-0.1.4/docs/_static/
--rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/_static/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/authors.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/changelog.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-02 08:35:26.000000 halborn_ctf-0.1.4/docs/conf.py
--rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/contributing.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1649 2023-05-02 13:58:34.000000 halborn_ctf-0.1.4/docs/index.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/license.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       39 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/readme.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.590304 halborn_ctf-0.1.4/docs/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.595776 halborn_ctf-0.1.4/docs/src/getting_started/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-02 17:58:39.000000 halborn_ctf-0.1.4/docs/src/getting_started/examples.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.4/docs/src/getting_started/installation.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     8664 2023-05-02 18:10:20.000000 halborn_ctf-0.1.4/docs/src/getting_started/quick_start.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/pyproject.toml
--rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-02 18:12:19.601840 halborn_ctf-0.1.4/setup.cfg
--rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/setup.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.590451 halborn_ctf-0.1.4/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.597601 halborn_ctf-0.1.4/src/halborn_ctf/
--rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.4/src/halborn_ctf/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.4/src/halborn_ctf/cli.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:03:03.000000 halborn_ctf-0.1.4/src/halborn_ctf/functions.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.599183 halborn_ctf-0.1.4/src/halborn_ctf/network/
--rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/_generic.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.600112 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/__init__.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.600687 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_utils.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/json_rpc.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.4/src/halborn_ctf/shell.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     3598 2023-05-02 15:27:02.000000 halborn_ctf-0.1.4/src/halborn_ctf/state.py
--rw-r--r--   0 fr0zn      (501) staff       (20)    20343 2023-05-02 18:11:40.000000 halborn_ctf-0.1.4/src/halborn_ctf/templates.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.598846 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1262 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/SOURCES.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/dependency_links.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/entry_points.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/not-zip-safe
--rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/requires.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/top_level.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.601165 halborn_ctf-0.1.4/tests/
--rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/tests/conftest.py
--rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/tests/test_skeleton.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/tox.ini
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.468179 halborn_ctf-0.1.5/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/.coveragerc
+-rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/.readthedocs.yml
+-rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.5/AUTHORS.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/CHANGELOG.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.5/LICENSE.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-03 09:34:41.468248 halborn_ctf-0.1.5/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.5/README.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.461291 halborn_ctf-0.1.5/docs/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/Makefile
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.461639 halborn_ctf-0.1.5/docs/_static/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/_static/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/authors.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/changelog.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-03 09:08:19.000000 halborn_ctf-0.1.5/docs/conf.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/contributing.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1646 2023-05-03 08:57:14.000000 halborn_ctf-0.1.5/docs/index.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/docs/license.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.457236 halborn_ctf-0.1.5/docs/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.462368 halborn_ctf-0.1.5/docs/src/getting_started/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-03 09:12:11.000000 halborn_ctf-0.1.5/docs/src/getting_started/examples.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.5/docs/src/getting_started/installation.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     8582 2023-05-03 08:43:10.000000 halborn_ctf-0.1.5/docs/src/getting_started/quick_start.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.462716 halborn_ctf-0.1.5/docs/src/user_guide/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1706 2023-05-03 09:31:00.000000 halborn_ctf-0.1.5/docs/src/user_guide/faq.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/pyproject.toml
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-03 09:34:41.468602 halborn_ctf-0.1.5/setup.cfg
+-rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/setup.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.457396 halborn_ctf-0.1.5/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.464411 halborn_ctf-0.1.5/src/halborn_ctf/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.5/src/halborn_ctf/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.5/src/halborn_ctf/cli.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:37:52.000000 halborn_ctf-0.1.5/src/halborn_ctf/functions.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.466131 halborn_ctf-0.1.5/src/halborn_ctf/network/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/_generic.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.466993 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/__init__.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.467466 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_json_rpc/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_utils.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.5/src/halborn_ctf/network/filters/json_rpc.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.5/src/halborn_ctf/shell.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     3675 2023-05-03 08:37:30.000000 halborn_ctf-0.1.5/src/halborn_ctf/state.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)    22521 2023-05-03 09:32:47.000000 halborn_ctf-0.1.5/src/halborn_ctf/templates.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.465809 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1274 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/SOURCES.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/dependency_links.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/entry_points.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/not-zip-safe
+-rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/requires.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-03 09:34:41.000000 halborn_ctf-0.1.5/src/halborn_ctf.egg-info/top_level.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-03 09:34:41.467985 halborn_ctf-0.1.5/tests/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/tests/conftest.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.5/tests/test_skeleton.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.5/tox.ini
```

### Comparing `halborn_ctf-0.1.4/.coveragerc` & `halborn_ctf-0.1.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/.gitignore` & `halborn_ctf-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/.readthedocs.yml` & `halborn_ctf-0.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/CONTRIBUTING.rst` & `halborn_ctf-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/LICENSE.txt` & `halborn_ctf-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/PKG-INFO` & `halborn_ctf-0.1.5/src/halborn_ctf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: halborn_ctf
-Version: 0.1.4
+Name: halborn-ctf
+Version: 0.1.5
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.4/README.rst` & `halborn_ctf-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/docs/Makefile` & `halborn_ctf-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/docs/conf.py` & `halborn_ctf-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/docs/index.rst` & `halborn_ctf-0.1.5/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
    src/getting_started/quick_start
    src/getting_started/examples
 
 .. toctree::
    :maxdepth: 1
    :caption: User Guide
 
-   source/user_guide/faq
+   src/user_guide/faq
 
 .. toctree::
    :maxdepth: 1
    :caption: Developer Guide
 
    Contributions & Help <contributing>
    Authors <authors>
```

### Comparing `halborn_ctf-0.1.4/docs/src/getting_started/examples.rst` & `halborn_ctf-0.1.5/docs/src/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/docs/src/getting_started/installation.rst` & `halborn_ctf-0.1.5/docs/src/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/docs/src/getting_started/quick_start.rst` & `halborn_ctf-0.1.5/docs/src/getting_started/quick_start.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 .. code-block:: console
 
     $ cat challenge.py
 
 
 .. code::
 
-    from halborn_ctf.templates import GenericChallenge 
+    from halborn_ctf.templates import GenericChallenge
 
     class Challenge(GenericChallenge):
 
         HAS_SOLVER = True
 
         CHALLENGE_NAME = 'MY CHALLENGE'
 
         def build(self):
             # Do build....
             pass
 
         def run(self):
             # Do deployment
             pass
-        
+
         def solver(self):
             self.solved = True
 
 
 You can now test that the challenge does build with (:mod:`halborn_ctf.templates.GenericChallenge.build`):
 
 .. code-block:: console
@@ -56,33 +56,33 @@
 
     2023-05-02 16:26:48 | root | __enter__ | INFO | pid=41948  pgid=41948
     2023-05-02 16:26:48 | werkzeug | _log | INFO | WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
     * Running on all addresses (0.0.0.0)
     * Running on http://127.0.0.1:8080
 
 
-You should see that a server has been spawned locally on port ``8080``. 
+You should see that a server has been spawned locally on port ``8080``.
 
 By default the challenge will expose the following routes:
 
-- ``/state``: Does return challenge public state: ``{"ready":true,"state":{}}`` (http://127.0.0.1:8080/state)
+- ``/info``: Does return challenge public state: ``{"ready":true,"state":{}}`` (http://127.0.0.1:8080/info)
 
 
-.. note:: 
-    Since we have set ``HAS_SOLVER`` (:mod:`halborn_ctf.templates.GenericChallenge.HAS_SOLVER`). The ``solver`` function must exist. 
+.. note::
+    Since we have set ``HAS_SOLVER`` (:mod:`halborn_ctf.templates.GenericChallenge.HAS_SOLVER`). The ``solver`` function must exist.
     The ``/solved`` route will also be exposed (http://127.0.0.1:8080/solved). Each time the route is accessed this function will be executed before responding the HTTP request.
 
     The route is now returning that the challenge is solved as we set ``self.solved = True``::
 
         {
             "msg": "Solved",
             "solved": true
         }
-    
-.. tip:: 
+
+.. tip::
     If the function does take a lot to execute or does require background processing take a look at :ref:`periodic-solver`.
 
 
 Service mapping
 ---------------
 
 The previous code does have the minimum required functions to run a challenge. However, it does not have any functionallity and there is no way to access services. To register
@@ -100,16 +100,16 @@
 
     class Challenge(GenericChallenge):
 
         HAS_SOLVER = True
 
         CHALLENGE_NAME = 'MY CHALLENGE'
 
-        # rule1: A request to http://challenge/ will be proxied to http://127.0.0.1:9999/. 
-        # rule2: A request to http://challenge/my_path/file will be proxied to http://127.0.0.1:9999/my_path/file. 
+        # rule1: A request to http://challenge/ will be proxied to http://127.0.0.1:9999/.
+        # rule2: A request to http://challenge/my_path/file will be proxied to http://127.0.0.1:9999/my_path/file.
 
         PATH_MAPPING = {
             '/': {
                 'port': 9999,
                 'path': '/',
                 'methods': ['GET']
             },
@@ -130,48 +130,48 @@
             network.wait_for_port(9999)
 
         def solver(self):
             response = requests.get('http://127.0.0.1:9999')
             if "halborn_ctf.txt" in response:
                 self.solved = True
 
-The previous challenge does use functions from this framework to run a shell command in the background with an http 
-server on the current directory. It then waits for the port to be listening. 
+The previous challenge does use functions from this framework to run a shell command in the background with an http
+server on the current directory. It then waits for the port to be listening.
 
 If you now try to access http://127.0.0.1:8080 you will be able to see the current directory listing. This is achieved by the ``PATH_MAPPING`` attribute which proxies
 any request on the ``/`` path to the server listening on port ``9999``. It also proxies any subpath request ``/<path:path>`` to the same server from the ``/`` path.
 
-If you now try to request http://127.0.0.1:8080/solved you will see that the challenge does report as not being solved. 
+If you now try to request http://127.0.0.1:8080/solved you will see that the challenge does report as not being solved.
 
 .. tip::
 
     To solve the challenge create a file named ``halborn_ctf.txt`` under the challenge directory:
 
     .. code-block:: console
-        
-        $ touch halborn_ctf.txt 
+
+        $ touch halborn_ctf.txt
 
 
 
 Downloadable files
 ------------------
 
 
 Some challenges require the players to have some files to be used. For that the ``HAS_FILES`` (:mod:`halborn_ctf.templates.GenericChallenge.HAS_FILES`) flag can be set to ``True``. Doing so, a function named ``files`` should be declared.
 
 We can create a file as a test to be exposed with the challenge:
 
 
 .. code-block:: console
 
-    $ echo "Test content" > test.txt 
+    $ echo "Test content" > test.txt
 
 .. code::
 
-    from halborn_ctf.templates import GenericChallenge 
+    from halborn_ctf.templates import GenericChallenge
 
     class Challenge(GenericChallenge):
 
         HAS_SOLVER = True
         HAS_FILES = True
 
         CHALLENGE_NAME = 'MY CHALLENGE'
@@ -179,37 +179,37 @@
         def build(self):
             # Do build....
             pass
 
         def run(self):
             # Do deployment....
             pass
-        
+
         def solver(self):
             self.solved = True
-        
+
         def files(self):
             return [
                 'test.txt'
             ]
 
 
 If we now try to access the server at ``/files`` (http://127.0.0.1:8080/files) a ``MY_CHALLENGE.zip`` file will be downloaded. The name is taken from ``CHALLENGE_NAME``. The content of the file should include the ``test.txt`` and the ``challenge.py`` file itself.
 
 Working with the state
 ----------------------
 
-If you want to persist variables across ``build`` and ``run`` and all periodic functions 
-you can use the :obj:`halborn_ctf.templates.GenericChallenge.state` and :obj:`halborn_ctf.templates.GenericChallenge.state_public` 
+If you want to persist variables across ``build`` and ``run`` and all periodic functions
+you can use the :obj:`halborn_ctf.templates.GenericChallenge.state` and :obj:`halborn_ctf.templates.GenericChallenge.state_public`
 properties. This property can be accessed anywhere but must be declared on the ``__init__`` function with the initial values.
 
 
 .. code::
 
-    from halborn_ctf.templates import GenericChallenge 
+    from halborn_ctf.templates import GenericChallenge
 
     class Challenge(GenericChallenge):
 
         HAS_SOLVER = True
         HAS_FILES = True
 
         CHALLENGE_NAME = 'MY CHALLENGE'
@@ -224,40 +224,40 @@
         def build(self):
             # Do build....
             pass
 
         def run(self):
             # Do deployment
             pass
-        
+
         def solver(self):
             self.state.solved_attempts += 1
 
             if self.state.solved_attempts == 2:
                 self.solved = True
-        
+
         def files(self):
             return [
                 'test.txt'
             ]
 
 
 .. note::
-    The ``state_public`` can be accessed and seen on the ``/state`` challenge route. (http://127.0.0.1:8080/state)
+    The ``state_public`` can be accessed and seen on the ``/info`` challenge route. (http://127.0.0.1:8080/info)
 
 .. _periodic-solver:
 
-Periodic solver 
+Periodic solver
 ---------------
 
 If the function does take a lot to execute or does require background processing you can always define a periodic function and start it before setting the challenge to ready. Take a look on how to use the decorator under :obj:`halborn_ctf.functions.periodic`.
 
 .. code::
 
-    from halborn_ctf.templates import GenericChallenge 
+    from halborn_ctf.templates import GenericChallenge
 
     from halborn_ctf.functions import periodic
 
     class Challenge(GenericChallenge):
 
         HAS_SOLVER = True
 
@@ -280,15 +280,15 @@
             pass
 
         def run(self):
             # Do deployment
 
             ########### Start the periodic function ##########
             self.my_checker()
-        
+
         def solver(self):
             # The solve is done on the `my_checker` function
             pass
 
 
 The previous challenge will be logging the ``Checking...`` string on the console every 1 second.
```

### Comparing `halborn_ctf-0.1.4/setup.cfg` & `halborn_ctf-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/setup.py` & `halborn_ctf-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/__init__.py` & `halborn_ctf-0.1.5/src/halborn_ctf/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/cli.py` & `halborn_ctf-0.1.5/src/halborn_ctf/cli.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/functions.py` & `halborn_ctf-0.1.5/src/halborn_ctf/functions.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/_generic.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/_generic.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/__init__.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_utils.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/filters/_utils.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/json_rpc.py` & `halborn_ctf-0.1.5/src/halborn_ctf/network/filters/json_rpc.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/shell.py` & `halborn_ctf-0.1.5/src/halborn_ctf/shell.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/state.py` & `halborn_ctf-0.1.5/src/halborn_ctf/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,17 @@
         _dict = args[0]
         for k in _dict.keys():
             if type(_dict[k]) == dict:
                 _dict[k] = State(_dict[k])
         super(State,self).__init__(_dict)
 
     def __getattr__(self, key):
-        return self.get(key, None)
+        if key not in self:
+            raise ValueError(f'Key "{key}" not found')
+        return self.get(key)
 
     # def __setitem__(self, key, value):
     #     super().__setitem__(key, value)
         # raise NotImplementedError()
 
     # def __getitem__(self, key):
     #     raise NotImplementedError()
```

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf/templates.py` & `halborn_ctf-0.1.5/src/halborn_ctf/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 - Test the template by using the ``halborn_ctf`` CLI (:obj:`halborn_ctf.cli.run`)::
 
     halborn_ctf run -vv
 
 - Server can be accessed under ``localhost:8080`` by default.
 
 """
+from dataclasses import dataclass
 import logging
 import flask
 from flask_cors import CORS
 from flask import Response, request
 import requests
 import os
 import zipfile
@@ -109,31 +110,49 @@
     STATIC = 1
     """If the flag is statically defined or embedded into the challenge somewhere.
     """
     DYNAMIC = 2
     """When the challenge is deployed a ``FLAG`` environment variable will be set.
     """
 
+@dataclass
+class StrFile():
+    """It allows to create a container for temporary generated files from strings. It can be used on the
+    :obj:`GenericChallenge.HAS_FILES` to add on-the fly files:
+
+    Example::
+
+        from halborn_ctf.templates import StrFile
+
+        def files(self):
+            return [
+                StrFile('folder/test.txt', 'THIS IS THE CONTENT')
+            ]
+
+    """
+    filepath: str
+    content: str
+
 class GenericChallenge(ABC):
     """Generic CTF challenge template
 
     Each created/deployed challenge does have two steps defined, :obj:`build` and :obj:`run`. The ``build`` step is only executed once
     when the challenge is created and uploaded into the platform for playing. The ``run`` step is always executed for each player request
     to deploy a new challenge.
 
     This template does also expose the challenge by using an HTTP server. The server does allow registering routes to it by using
     the :obj:`PATH_MAPPING` attribute.
 
     An attribute named :obj:`state` can be used to store any sort of object that will persiste between the ``build`` and ``run`` steps. Furthermore,
     this attribute can be used to store anything that would be used across the different functions. The `state_public` property will be exposed
-    under the `/state` path on the challenge domain.
+    under the `/info` path on the challenge domain.
 
     The following routes will be exposed under ``localhost:8080``:
 
-    - ``/state``: Does contain general info of the challenge such as :obj:`ready` and :obj:`state_public`.
+    - ``/info``: Does contain general info of the challenge such as :obj:`ready` and :obj:`state_public`.
     - ``/solved``: Does execute the "solver" function and display if the challenge was solved together with a solved message or hint to the player.
 
     Note:
         Only if :attr:`HAS_SOLVER` == ``True``.
 
     - ``/files``: Does download the files listed under the "files" function as a zip file named by :attr:`CHALLENGE_NAME`.
 
@@ -158,28 +177,83 @@
             return [
                 "filter.py",
                 "folder/test.sol",
                 "folder2/**",
                 "folder3/*.sol",
             ]
 
+    Tip:
+        You can also create virtual files from strings using :obj:`StrFile`.
+
     Note:
         Each time the user request the `/files` route a zip archive with all of the listed files will be downloaded.
     """
+
     HAS_SOLVER = False
     """
     (bool): If the challenge has a solver. The required function "solver" should be present. Although it is possible
     to have periodic functions (:obj:`periodic`) that set the :obj:`solved`.
     You can keep the method defined like this if the latter is being used::
 
         def solver(self):
             pass
 
     Note:
-        This function will be executed each time the user requests the `/solved` route.
+        This function will be executed each time the user requests the ``/solved`` route.
+    """
+
+    HAS_DETAILS = False
+    """
+    (bool): If the challenge has dynamic or specific implementation details. The required function "details" should be present.
+    This function must return a string. You can format the string using any ``state`` variable or any dynamic content (for example a file content).
+
+    The string does support ``Markdown`` syntax and will be displayed on the platform UI and under the ``/info`` route
+
+    Example::
+
+        DETAILS_TEMPLATE = '''
+        This is a detailed description of the challenge:
+
+        You will require:
+
+        - This
+        - That
+
+        You can also check: {custom_value}
+
+        Don't forget: {extra}
+
+        Helper:
+
+        ``` python
+        def helper():
+            pass
+        ```
+        '''
+
+        ...
+
+        def __init__(self):
+            super().__init__()
+
+            self.state = {
+                'custom_value': 0x1337
+            }
+
+
+        def details(self):
+            return DETAILS_TEMPLATE.format(
+                **self.state,
+                **{
+                    'extra': "Extra info"
+                }
+            )
+
+    Note:
+        This function will be executed each time the user requests the ``/info`` route.
     """
 
     PATH_MAPPING = {}
     """
     (dict[str, MappingInfo]): Mapping used internally to register the challenge URL's paths.
     It does contain a mapping of ``path`` to ``MappingInfo`` dictionary details.
 
@@ -229,14 +303,29 @@
             }
 
     Note:
         There is no need to specify any of the required field for the filter such as ``listen_port``, ``to_port``, ``to_host`` as those will
         be extracted from the mapping itself and a random listening port used and remapped.
     """
 
+    def _check_feature_enabled(self, feature_name, required_function):
+        if getattr(self, feature_name):
+            try:
+                getattr(self, required_function)
+            except:
+                raise NotImplementedError(f'Missing function "{required_function}" ({feature_name} == True)')
+        else:
+            try:
+                getattr(self, required_function)
+                raise NotImplementedError(f'Remove "{required_function}" function ({feature_name} == False)')
+            except:
+                pass
+
+
+
     def __init__(self) -> None:
         super().__init__()
 
         self._app = flask.Flask('Challenge')
         self.log = logging.getLogger(self.CHALLENGE_NAME)
 
         CORS(self._app)
@@ -253,37 +342,17 @@
 
         if self.HAS_SOLVER:
             self._solved = False
             self._solved_msg = None
             # self._state._setattr('solved', False)
             # self._state._setattr('solved_msg', None)
 
-        if self.HAS_FILES:
-            try:
-                getattr(self, 'files')
-            except:
-                raise NotImplementedError('Missing function "files" (HAS_FILES == True)')
-        else:
-            try:
-                getattr(self, 'files')
-                raise NotImplementedError('Remove "files" function (HAS_FILES == False)')
-            except:
-                pass
-
-        if self.HAS_SOLVER:
-            try:
-                getattr(self, 'solver')
-            except:
-                raise NotImplementedError('Missing function "solver" (HAS_SOLVER == True)')
-        else:
-            try:
-                getattr(self, 'solver')
-                raise NotImplementedError('Remove "solver" function (HAS_SOLVER == False)')
-            except:
-                pass
+        self._check_feature_enabled('HAS_FILES', 'files')
+        self._check_feature_enabled('HAS_SOLVER', 'solver')
+        self._check_feature_enabled('HAS_DETAILS', 'details')
 
         if not self.HAS_SOLVER and self.FLAG_TYPE == FlagType.NONE:
             raise ValueError("HAS_SOLVER == False and FLAG_TYPE == NONE")
 
         self._path_mapping: dict[str, MappingInfo] = {}
 
     # @property
@@ -369,69 +438,83 @@
 
             Reading an state value::
 
                 print(self.state.custom)
                 # Changed value
 
         """
+        if not self._state_set:
+            raise ValueError("State not initialized")
         return self._state
 
     @state.setter
     def state(self, value):
         if self._state_set:
             raise ValueError("State already set, use state.update instead")
         self._state._merge(value)
         # self._state = State(value)
         self._state_set = True
 
     @property
     def state_public(self):
-        """(State): It will expose the state content into the challenge ``/state`` route. Refer to :obj:`state`.
+        """(State): It will expose the state content into the challenge ``/info`` route. Refer to :obj:`state`.
         """
+        if not self._state_public_set:
+            raise ValueError("State not initialized")
         return self._state_public
 
     @state_public.setter
     def state_public(self, value):
         if self._state_public_set:
             raise ValueError("State already set, use state_public.update instead")
         self._state_public._merge(value)
         # self._state_public_set = State(value)
         self._state_public_set = True
 
     def _app_info_handler(self):
-        if not self.ready:
+        if not self._ready:
             return Response("Challenge not ready", status=503)
 
-        return {
-            'ready': self.ready,
-            'state': self.state_public,
+        _return = {
+            'ready': self._ready,
+            'state': self._state_public,
         }
 
+        if self.HAS_DETAILS:
+            _return['details'] = self.details()
+        else:
+            _return['details'] = None
+
+        return _return
+
     def _app_files_handler(self):
-        if not self.ready:
+        if not self._ready:
             return Response("Challenge not ready", status=503)
 
         name = self.CHALLENGE_NAME.replace(' ','_')
 
         fileName = f"{name}.zip"
         files = self.files() + ['challenge.py']
 
         memory_file = BytesIO()
         with zipfile.ZipFile(memory_file, 'w', zipfile.ZIP_DEFLATED) as zipf:
             for _added in files:
-                for result in glob.glob(_added):
-                    zipf.write(result)
+                if type(_added) == StrFile:
+                    zipf.writestr(_added.filepath, _added.content)
+                else:
+                    for result in glob.glob(_added):
+                        zipf.write(result)
 
         memory_file.seek(0)
         return flask.send_file(memory_file,
                         download_name=fileName,
                         as_attachment=True)
 
     def _app_solved_handler(self):
-        if not self.ready:
+        if not self._ready:
             return Response("Challenge not ready", status=503)
 
         # If not solved, we check on the solver
         if not self.solved:
             try:
                 self.solver()
             except Exception as e:
@@ -512,15 +595,15 @@
         cli.show_server_banner = lambda *x: None
 
         self._app.run(host='0.0.0.0', port=os.environ.get('PORT', 8080), use_reloader=False, debug=False)
 
     #######################################
 
     def _register_flask_paths(self):
-        self._app.add_url_rule('/state', 'public-state', self._app_info_handler, methods=['GET'])
+        self._app.add_url_rule('/info', 'info', self._app_info_handler, methods=['GET'])
         if self.HAS_FILES:
             self._app.add_url_rule('/files', 'files', self._app_files_handler, methods=['GET'])
         if self.HAS_SOLVER:
             self._app.add_url_rule('/solved', 'solved', self._app_solved_handler, methods=['GET'])
 
     def _build(self):
         with _CleanChildProcesses():
@@ -546,15 +629,15 @@
 
             self._register_flask_paths()
 
             self.run()
 
             self._register_challenge_paths()
 
-            self.ready = True
+            self._ready = True
 
             self._flask_run()
 
 
     @abstractmethod
     def build(self):
         """All the static funtionality that should be executed during the build phase of the challenge container. The running container will
```

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf.egg-info/PKG-INFO` & `halborn_ctf-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: halborn-ctf
-Version: 0.1.4
+Name: halborn_ctf
+Version: 0.1.5
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.4/src/halborn_ctf.egg-info/SOURCES.txt` & `halborn_ctf-0.1.5/src/halborn_ctf.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
-docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 docs/src/getting_started/examples.rst
 docs/src/getting_started/installation.rst
 docs/src/getting_started/quick_start.rst
+docs/src/user_guide/faq.rst
 src/halborn_ctf/__init__.py
 src/halborn_ctf/cli.py
 src/halborn_ctf/functions.py
 src/halborn_ctf/shell.py
 src/halborn_ctf/state.py
 src/halborn_ctf/templates.py
 src/halborn_ctf.egg-info/PKG-INFO
```

### Comparing `halborn_ctf-0.1.4/tests/test_skeleton.py` & `halborn_ctf-0.1.5/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.4/tox.ini` & `halborn_ctf-0.1.5/tox.ini`

 * *Files identical despite different names*

