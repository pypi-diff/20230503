# Comparing `tmp/yerbamate-0.9.22.tar.gz` & `tmp/yerbamate-0.9.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yerbamate-0.9.22.tar", last modified: Sat Apr 22 15:21:21 2023, max compression
+gzip compressed data, was "yerbamate-0.9.23.tar", last modified: Wed May  3 21:05:38 2023, max compression
```

## Comparing `yerbamate-0.9.22.tar` & `yerbamate-0.9.23.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.553157 yerbamate-0.9.22/
--rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.22/LICENSE
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.22/MANIFEST.in
--rw-r--r--   0 al        (1000) al        (1001)    11581 2023-04-22 15:21:21.553157 yerbamate-0.9.22/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.22/README.md
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/packages/
--rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.22/packages/requirements.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/packages/yerbamate/
--rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.545158 yerbamate-0.9.22/packages/yerbamate/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     4429 2023-04-09 09:45:27.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/environment.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/mate.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.546158 yerbamate-0.9.22/packages/yerbamate/api/data/
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)    11315 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/module_manager.py
--rw-r--r--   0 al        (1000) al        (1001)    14686 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/module_repository.py
--rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/package.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.548158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/
--rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.549158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/io.py
--rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/local.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/
--rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/remote.py
--rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/sources/source.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.550158 yerbamate-0.9.22/packages/yerbamate/api/data/utils/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.551158 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/exp_util.py
--rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/git_util.py
--rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/data/utils/gitdir.py
--rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/api/mate_api.py
--rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/constants.py
--rw-r--r--   0 al        (1000) al        (1001)     5800 2023-04-09 09:45:16.000000 yerbamate-0.9.22/packages/yerbamate/environment.py
--rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/mate.py
--rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/mate_cli.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.551158 yerbamate-0.9.22/packages/yerbamate/utils/
--rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.552157 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/bunch.py
--rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/git_url_parser.py
--rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/utils/utils.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.553157 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/top_level.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.545158 yerbamate-0.9.22/packages/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)    11581 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)     3195 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       82 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/requires.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-22 15:21:21.000000 yerbamate-0.9.22/packages/yerbamate.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) al        (1001)      107 2023-04-22 15:21:21.553157 yerbamate-0.9.22/setup.cfg
--rw-r--r--   0 al        (1000) al        (1001)     1278 2023-04-22 15:20:20.000000 yerbamate-0.9.22/setup.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-04-22 15:21:21.544158 yerbamate-0.9.22/src/
--rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.22/src/mate
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/
+-rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.23/LICENSE
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.23/MANIFEST.in
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-05-03 21:05:38.460908 yerbamate-0.9.23/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.23/README.md
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.449909 yerbamate-0.9.23/packages/
+-rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.23/packages/requirements.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.450909 yerbamate-0.9.23/packages/yerbamate/
+-rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.452909 yerbamate-0.9.23/packages/yerbamate/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4429 2023-04-09 09:45:27.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/environment.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/mate.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.452909 yerbamate-0.9.23/packages/yerbamate/api/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.453909 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.453909 yerbamate-0.9.23/packages/yerbamate/api/data/
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.454908 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11315 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/module_manager.py
+-rw-r--r--   0 al        (1000) al        (1001)    14686 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/module_repository.py
+-rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/package.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.454908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.455908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.455908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/
+-rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/io.py
+-rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/local.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/
+-rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/remote.py
+-rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/source.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.457908 yerbamate-0.9.23/packages/yerbamate/api/data/utils/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.458908 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/exp_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/git_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/gitdir.py
+-rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/mate_api.py
+-rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/constants.py
+-rw-r--r--   0 al        (1000) al        (1001)     5857 2023-05-03 21:03:55.000000 yerbamate-0.9.23/packages/yerbamate/environment.py
+-rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/mate.py
+-rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/mate_cli.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.458908 yerbamate-0.9.23/packages/yerbamate/utils/
+-rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/bunch.py
+-rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/git_url_parser.py
+-rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/utils.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/top_level.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.451908 yerbamate-0.9.23/packages/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)     3195 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       82 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) al        (1001)      107 2023-05-03 21:05:38.460908 yerbamate-0.9.23/setup.cfg
+-rw-r--r--   0 al        (1000) al        (1001)     1278 2023-05-03 21:04:55.000000 yerbamate-0.9.23/setup.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.449909 yerbamate-0.9.23/src/
+-rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.23/src/mate
```

### Comparing `yerbamate-0.9.22/LICENSE` & `yerbamate-0.9.23/LICENSE`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/PKG-INFO` & `yerbamate-0.9.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.22
+Version: 0.9.23
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
 <!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
```

### Comparing `yerbamate-0.9.22/README.md` & `yerbamate-0.9.23/README.md`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/__pycache__/environment.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/__pycache__/environment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/__pycache__/mate.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/__pycache__/mate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/module_manager.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/module_manager.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/module_repository.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/module_repository.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/package.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/package.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/io.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/io.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/local/local.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/local.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/sources/remote/remote.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/remote.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/utils/git_util.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/utils/git_util.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/data/utils/gitdir.py` & `yerbamate-0.9.23/packages/yerbamate/api/data/utils/gitdir.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/api/mate_api.py` & `yerbamate-0.9.23/packages/yerbamate/api/mate_api.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/environment.py` & `yerbamate-0.9.23/packages/yerbamate/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         self.hparams = {}
 
         # set command to True
         try:
             setattr(self, sys.argv[1], True)
         except:
             pass
+        
+        self.args = sys.argv[1:]
 
         self._root = self.__find_root()
 
         # parse python -m module train arg=1 arg2=2
         for arg in sys.argv:
             if "=" not in arg:
                 continue
@@ -86,15 +88,15 @@
         for key in results:
             if key in self.env:
                 result = self.env[key]
                 break
         if result is None:
             return
         if not os.path.exists(result):
-            os.makedirs(result)
+            os.makedirs(result, exist_ok=True)
 
         save_file = os.path.join(result, "experiment.py")
         # copy from self._path to save_file
         shutil.copyfile(self._path, save_file)
 
         # ipdb.set_trace()
```

### Comparing `yerbamate-0.9.22/packages/yerbamate/mate.py` & `yerbamate-0.9.23/packages/yerbamate/mate.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/mate_cli.py` & `yerbamate-0.9.23/packages/yerbamate/mate_cli.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/__init__.py` & `yerbamate-0.9.23/packages/yerbamate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc` & `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/bunch.py` & `yerbamate-0.9.23/packages/yerbamate/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/git_url_parser.py` & `yerbamate-0.9.23/packages/yerbamate/utils/git_url_parser.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/utils/utils.py` & `yerbamate-0.9.23/packages/yerbamate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/packages/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.23/packages/yerbamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.22
+Version: 0.9.23
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
 <!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
```

### Comparing `yerbamate-0.9.22/packages/yerbamate.egg-info/SOURCES.txt` & `yerbamate-0.9.23/packages/yerbamate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.22/setup.py` & `yerbamate-0.9.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 setup(
     name="yerbamate",
     description=" A python module and experiment manager for deep learning",
     author="Giulio Zani, Ali Rahimi",
     author_email="yerba.mate.dl@proton.me",
     url="https://github.com/oalee/yerbamate",
-    python_requires=">=3.9",
-    version="0.9.22",
+    python_requires=">=3.8",
+    version="0.9.23",
     packages=find_packages("packages", exclude=["tests"]),
     include_package_data=True,
     package_dir={"": "packages/"},
     license="Apache License 2.0",
     license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type='text/markdown',
```

