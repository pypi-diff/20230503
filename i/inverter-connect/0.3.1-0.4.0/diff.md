# Comparing `tmp/inverter-connect-0.3.1.tar.gz` & `tmp/inverter-connect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.3.1.tar", last modified: Fri Apr 28 11:07:53 2023, max compression
+gzip compressed data, was "inverter-connect-0.4.0.tar", last modified: Wed May  3 17:55:25 2023, max compression
```

## Comparing `inverter-connect-0.3.1.tar` & `inverter-connect-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.3.1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.3.1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.263191 inverter-connect-0.3.1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.263191 inverter-connect-0.3.1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.3.1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.3.1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    11371 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    10957 2023-04-28 10:46:47.000000 inverter-connect-0.3.1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.3.1/cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.263191 inverter-connect-0.3.1/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.263191 inverter-connect-0.3.1/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.263191 inverter-connect-0.3.1/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-04-28 11:06:30.000000 inverter-connect-0.3.1/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.3.1/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4114 2023-04-28 11:04:08.000000 inverter-connect-0.3.1/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    17969 2023-04-28 11:05:30.000000 inverter-connect-0.3.1/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.3.1/inverter/config.py
--rw-rw-r--   0 jens      (1000) users      (100)    10136 2023-04-28 11:07:05.000000 inverter-connect-0.3.1/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.3.1/inverter/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.3.1/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.3.1/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.3.1/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.3.1/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.3.1/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.3.1/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.3.1/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.3.1/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.3.1/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.3.1/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.3.1/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2557 2023-04-28 07:02:52.000000 inverter-connect-0.3.1/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.3.1/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-04-28 07:13:12.000000 inverter-connect-0.3.1/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.3.1/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.3.1/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.3.1/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    11371 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1544 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      259 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-28 11:07:53.000000 inverter-connect-0.3.1/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4731 2023-04-27 15:42:09.000000 inverter-connect-0.3.1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.3.1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.3.1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-28 11:07:53.267191 inverter-connect-0.3.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.4.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    13375 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    12961 2023-05-03 17:42:44.000000 inverter-connect-0.4.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.4.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.4.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-03 17:43:39.000000 inverter-connect-0.4.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.4.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4114 2023-04-28 11:04:08.000000 inverter-connect-0.4.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11799 2023-05-03 17:27:43.000000 inverter-connect-0.4.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.4.0/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.4.0/inverter/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10136 2023-04-28 11:07:05.000000 inverter-connect-0.4.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.4.0/inverter/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.4.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.4.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.4.0/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.4.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.4.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.4.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.4.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.4.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.4.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3015 2023-05-03 17:43:47.000000 inverter-connect-0.4.0/inverter/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.4.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-04-28 07:13:12.000000 inverter-connect-0.4.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.4.0/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.4.0/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.4.0/inverter/utilities/modbus_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    13375 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1575 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      259 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4774 2023-05-03 17:23:48.000000 inverter-connect-0.4.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.4.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.4.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/setup.cfg
```

### Comparing `inverter-connect-0.3.1/.github/workflows/tests.yml` & `inverter-connect-0.4.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/PKG-INFO` & `inverter-connect-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: inverter-connect
-Version: 0.3.1
-Summary: Get information from Deye Microinverter
-Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://github.com/jedie/inverter-connect
-Project-URL: Source, https://github.com/jedie/inverter-connect
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -23,14 +11,16 @@
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
+Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
+
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
 ~/inverter-connect$ ./cli.py --help
 ```
 
@@ -40,34 +30,22 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
 │ debug-settings              Display (anonymized) MQTT server username and password               │
-│ fix-code-style              Fix code style of all inverter source code files via darker          │
-│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish                     Build and upload this project to PyPi                                │
 │ publish-loop                Publish current data via MQTT (endless loop)                         │
 │ read-register               Read register(s) from the inverter                                   │
-│ safety                      Run safety check against current requirements files                  │
 │ set-time                    Set current date time in the inverter device.                        │
 │ store-settings              Store MQTT server settings.                                          │
-│ test                        Run unittests                                                        │
 │ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
@@ -107,19 +85,22 @@
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
- Or speficy one or more AT-commands, e.g.:
+ Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
- e.g.: Set NTP server:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1
+ e.g.: Set NTP server, enable NTP and check the values:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
+ NTPSER NTPEN
+ wait a while and request the current date time:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
@@ -161,14 +142,51 @@
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
 
 ----
 
 
+# start development
+
+For development, we have a separate CLI, just call it:
+```bash
+~/inverter-connect$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all inverter source code files via darker          │
+│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+----
+
+
 # credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
```

### Comparing `inverter-connect-0.3.1/README.md` & `inverter-connect-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: inverter-connect
+Version: 0.4.0
+Summary: Get information from Deye Microinverter
+Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/inverter-connect
+Project-URL: Source, https://github.com/jedie/inverter-connect
+Requires-Python: <4,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -11,14 +23,16 @@
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
+Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
+
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
 ~/inverter-connect$ ./cli.py --help
 ```
 
@@ -28,34 +42,22 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
 │ debug-settings              Display (anonymized) MQTT server username and password               │
-│ fix-code-style              Fix code style of all inverter source code files via darker          │
-│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish                     Build and upload this project to PyPi                                │
 │ publish-loop                Publish current data via MQTT (endless loop)                         │
 │ read-register               Read register(s) from the inverter                                   │
-│ safety                      Run safety check against current requirements files                  │
 │ set-time                    Set current date time in the inverter device.                        │
 │ store-settings              Store MQTT server settings.                                          │
-│ test                        Run unittests                                                        │
 │ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
@@ -95,19 +97,22 @@
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
- Or speficy one or more AT-commands, e.g.:
+ Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
- e.g.: Set NTP server:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1
+ e.g.: Set NTP server, enable NTP and check the values:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
+ NTPSER NTPEN
+ wait a while and request the current date time:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
@@ -149,14 +154,51 @@
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
 
 ----
 
 
+# start development
+
+For development, we have a separate CLI, just call it:
+```bash
+~/inverter-connect$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all inverter source code files via darker          │
+│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+----
+
+
 # credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
```

### Comparing `inverter-connect-0.3.1/cli.py` & `inverter-connect-0.4.0/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,26 +41,26 @@
     FILE_EXT = '.exe'
 else:
     # Files under Linux/Mac and all other than Windows, e.g.: .../.venv/bin/python
     BIN_NAME = 'bin'
     FILE_EXT = ''
 
 BASE_PATH = Path(__file__).parent
-VENV_PATH = BASE_PATH / '.venv'
+VENV_PATH = BASE_PATH / '.venv-app'
 BIN_PATH = VENV_PATH / BIN_NAME
 PYTHON_PATH = BIN_PATH / f'python{FILE_EXT}'
 PIP_PATH = BIN_PATH / f'pip{FILE_EXT}'
 PIP_SYNC_PATH = BIN_PATH / f'pip-sync{FILE_EXT}'
 
-DEP_LOCK_PATH = BASE_PATH / 'requirements.dev.txt'
+DEP_LOCK_PATH = BASE_PATH / 'requirements.txt'
 DEP_HASH_PATH = VENV_PATH / '.dep_hash'
 
 # script file defined in pyproject.toml as [console_scripts]
 # (Under Windows: ".exe" not added!)
-PROJECT_SHELL_SCRIPT = BIN_PATH / 'inverter'
+PROJECT_SHELL_SCRIPT = BIN_PATH / 'inverter_app'
 
 
 def get_dep_hash():
     """Get SHA512 hash from poetry.lock content."""
     return hashlib.sha512(DEP_LOCK_PATH.read_bytes()).hexdigest()
```

### Comparing `inverter-connect-0.3.1/inverter/.github/workflows/tests.yml` & `inverter-connect-0.4.0/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -35,27 +35,27 @@
         python-version: '${{ matrix.python-version }}'
         cache: 'pip' # caching pip dependencies
         cache-dependency-path: '**/requirements.dev.txt'
 
     - name: 'Bootstrap'
       # The first CLI call will create the .venv
       run: |
-        ./cli.py version
+        ./dev-cli.py version
 
     - name: 'CLI help'
       run: |
-        ./cli.py --help
+        ./dev-cli.py --help
 
     - name: 'Safety'
       run: |
-        ./cli.py safety
+        ./dev-cli.py safety
 
     - name: 'Run tests with Python v${{ matrix.python-version }}'
       run: |
-        ./cli.py coverage
+        ./dev-cli.py coverage
 
     - name: 'Upload coverage report'
       uses: codecov/codecov-action@v3
       # https://github.com/marketplace/actions/codecov
       with:
         fail_ci_if_error: false
         verbose: true
```

### Comparing `inverter-connect-0.3.1/inverter/api.py` & `inverter-connect-0.4.0/inverter/api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/connection.py` & `inverter-connect-0.4.0/inverter/connection.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.4.0/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/definitions.py` & `inverter-connect-0.4.0/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/mqtt4homeassistant/converter.py` & `inverter-connect-0.4.0/inverter/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/mqtt4homeassistant/data_classes.py` & `inverter-connect-0.4.0/inverter/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/mqtt4homeassistant/mqtt.py` & `inverter-connect-0.4.0/inverter/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/mqtt4homeassistant/tests/test_converter.py` & `inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/publish_loop.py` & `inverter-connect-0.4.0/inverter/publish_loop.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/tests/test_api.py` & `inverter-connect-0.4.0/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/tests/test_connect.py` & `inverter-connect-0.4.0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/tests/test_definitions.py` & `inverter-connect-0.4.0/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/tests/test_project_setup.py` & `inverter-connect-0.4.0/inverter/tests/test_project_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,48 +8,57 @@
 from packaging.version import Version
 
 from inverter import __version__
 from inverter.cli.cli_app import PACKAGE_ROOT
 
 
 class ProjectSetupTestCase(TestCase):
+    app_cli_bin = PACKAGE_ROOT / 'cli.py'
+    dev_cli_bin = PACKAGE_ROOT / 'dev-cli.py'
+
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+
+        assert_is_file(cls.app_cli_bin)
+        assert_is_file(cls.dev_cli_bin)
+
     def test_version(self):
         self.assertIsNotNone(__version__)
 
         version = Version(__version__)  # Will raise InvalidVersion() if wrong formatted
         self.assertEqual(str(version), __version__)
 
-        cli_bin = PACKAGE_ROOT / 'cli.py'
-        assert_is_file(cli_bin)
+        # The "app" cli:
+        output = subprocess.check_output([self.app_cli_bin, 'version'], text=True)
+        self.assertIn(f'inverter v{__version__}', output)
 
-        output = subprocess.check_output([cli_bin, 'version'], text=True)
+        # The "development" cli:
+        output = subprocess.check_output([self.dev_cli_bin, 'version'], text=True)
         self.assertIn(f'inverter v{__version__}', output)
 
     def test_code_style(self):
-        cli_bin = PACKAGE_ROOT / 'cli.py'
-        assert_is_file(cli_bin)
-
         try:
             output = subprocess_cli(
-                cli_bin=cli_bin,
+                cli_bin=self.dev_cli_bin,
                 args=('check-code-style',),
                 exit_on_error=False,
             )
         except subprocess.CalledProcessError as err:
             self.assertIn('.venv/bin/darker', err.stdout)  # darker was called?
         else:
             if 'Code style: OK' in output:
                 self.assertIn('.venv/bin/darker', output)  # darker was called?
                 return  # Nothing to fix -> OK
 
         # Try to "auto" fix code style:
 
         try:
             output = subprocess_cli(
-                cli_bin=cli_bin,
+                cli_bin=self.dev_cli_bin,
                 args=('fix-code-style',),
                 exit_on_error=False,
             )
         except subprocess.CalledProcessError as err:
             output = err.stdout
 
         self.assertIn('.venv/bin/darker', output)  # darker was called?
```

### Comparing `inverter-connect-0.3.1/inverter/tests/test_readme.py` & `inverter-connect-0.4.0/inverter/tests/test_readme.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bx_py_utils.auto_doc import assert_readme_block
 from bx_py_utils.path import assert_is_file
 from manageprojects.test_utils.click_cli_utils import invoke_click
 from manageprojects.tests.base import BaseTestCase
 
 from inverter import constants
 from inverter.cli.cli_app import PACKAGE_ROOT, cli
+from inverter.cli.dev import cli as dev_cli
 
 
 def assert_cli_help_in_readme(text_block: str, marker: str):
     README_PATH = PACKAGE_ROOT / 'README.md'
     assert_is_file(README_PATH)
 
     text_block = text_block.replace(constants.CLI_EPILOG, '')
@@ -31,14 +32,27 @@
                 'print-at-commands',
                 'print-values',
                 constants.CLI_EPILOG,
             ),
         )
         assert_cli_help_in_readme(text_block=stdout, marker='main help')
 
+    def test_dev_help(self):
+        stdout = invoke_click(dev_cli, '--help')
+        self.assert_in_content(
+            got=stdout,
+            parts=(
+                'Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...',
+                'fix-code-style',
+                'tox',
+                constants.CLI_EPILOG,
+            ),
+        )
+        assert_cli_help_in_readme(text_block=stdout, marker='dev help')
+
     def test_print_values_help(self):
         stdout = invoke_click(cli, 'print-values', '--help')
         self.assert_in_content(
             got=stdout,
             parts=(
                 'Usage: ./cli.py print-values [OPTIONS] IP',
                 '--port',
```

### Comparing `inverter-connect-0.3.1/inverter/utilities/cli.py` & `inverter-connect-0.4.0/inverter/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/utilities/credentials.py` & `inverter-connect-0.4.0/inverter/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter/utilities/modbus_converter.py` & `inverter-connect-0.4.0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.4.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.3.1
+Version: 0.4.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -23,14 +23,16 @@
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
+Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
+
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
 ~$ cd inverter-connect
 ~/inverter-connect$ ./cli.py --help
 ```
 
@@ -40,34 +42,22 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
 │ debug-settings              Display (anonymized) MQTT server username and password               │
-│ fix-code-style              Fix code style of all inverter source code files via darker          │
-│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish                     Build and upload this project to PyPi                                │
 │ publish-loop                Publish current data via MQTT (endless loop)                         │
 │ read-register               Read register(s) from the inverter                                   │
-│ safety                      Run safety check against current requirements files                  │
 │ set-time                    Set current date time in the inverter device.                        │
 │ store-settings              Store MQTT server settings.                                          │
-│ test                        Run unittests                                                        │
 │ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
@@ -107,19 +97,22 @@
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
- Or speficy one or more AT-commands, e.g.:
+ Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
- e.g.: Set NTP server:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1
+ e.g.: Set NTP server, enable NTP and check the values:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
+ NTPSER NTPEN
+ wait a while and request the current date time:
+ .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
 │                                                       [default: 48899; 1000<=x<=65535]           │
 │ --debug/--no-debug                                    [default: no-debug]                        │
 │ --help                                                Show this message and exit.                │
@@ -161,14 +154,51 @@
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
 
 ----
 
 
+# start development
+
+For development, we have a separate CLI, just call it:
+```bash
+~/inverter-connect$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all inverter source code files via darker          │
+│ install                     Run pip-sync and install 'inverter' via pip as editable.             │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+----
+
+
 # credits
 
 Others before me have done good work. In particular, I have learned a lot from the following projects:
 
 * https://github.com/s10l/deye-logger-at-cmd
 * https://github.com/kbialek/deye-inverter-mqtt
 * https://github.com/StephanJoubert/home_assistant_solarman
```

### Comparing `inverter-connect-0.3.1/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.4.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .editorconfig
 .flake8
 .gitignore
 README.md
 cli.py
+dev-cli.py
 pyproject.toml
 requirements.dev.txt
 requirements.txt
 .github/workflows/tests.yml
 inverter/.editorconfig
 inverter/.flake8
 inverter/.gitignore
@@ -18,14 +19,15 @@
 inverter/constants.py
 inverter/definitions.py
 inverter/exceptions.py
 inverter/publish_loop.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
+inverter/cli/dev.py
 inverter/definitions/deye_2mppt.yaml
 inverter/mqtt4homeassistant/__init__.py
 inverter/mqtt4homeassistant/converter.py
 inverter/mqtt4homeassistant/data_classes.py
 inverter/mqtt4homeassistant/mqtt.py
 inverter/mqtt4homeassistant/tests/__init__.py
 inverter/mqtt4homeassistant/tests/test_converter.py
```

### Comparing `inverter-connect-0.3.1/pyproject.toml` & `inverter-connect-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 ]
 
 [project.urls]
 Documentation = "https://github.com/jedie/inverter-connect"
 Source = "https://github.com/jedie/inverter-connect"
 
 [project.scripts]
-inverter = "inverter.__main__:main"
+inverter_app = "inverter.__main__:main"
+inverter_dev = "inverter.cli.dev:main"
 
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=7.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
```

### Comparing `inverter-connect-0.3.1/requirements.dev.txt` & `inverter-connect-0.4.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.3.1/requirements.txt` & `inverter-connect-0.4.0/requirements.txt`

 * *Files identical despite different names*

