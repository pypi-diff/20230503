# Comparing `tmp/jsonrpc-py-3.0.6.tar.gz` & `tmp/jsonrpc-py-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.6.tar", last modified: Tue May  2 09:55:03 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.7.tar", last modified: Wed May  3 09:14:02 2023, max compression
```

## Comparing `jsonrpc-py-3.0.6.tar` & `jsonrpc-py-3.0.7.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.775499 jsonrpc-py-3.0.6/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.769499 jsonrpc-py-3.0.6/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.778499 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.785500 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.788500 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.791500 jsonrpc-py-3.0.6/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9423 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.793501 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 09:55:03.797501 jsonrpc-py-3.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     5140 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.022167 jsonrpc-py-3.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-03 09:14:02.021167 jsonrpc-py-3.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:01.998165 jsonrpc-py-3.0.7/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:01.992165 jsonrpc-py-3.0.7/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.003166 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.010166 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.013166 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.017166 jsonrpc-py-3.0.7/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9423 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.018167 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 09:14:02.022167 jsonrpc-py-3.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.021167 jsonrpc-py-3.0.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.6/.gitlab-ci.yml` & `jsonrpc-py-3.0.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/LICENSE` & `jsonrpc-py-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/Makefile` & `jsonrpc-py-3.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/PKG-INFO` & `jsonrpc-py-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.6
+Version: 3.0.7
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.6/README.md` & `jsonrpc-py-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/changelog.rst` & `jsonrpc-py-3.0.7/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/conf.py` & `jsonrpc-py-3.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/deployment.rst` & `jsonrpc-py-3.0.7/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/index.rst` & `jsonrpc-py-3.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/quickstart.rst` & `jsonrpc-py-3.0.7/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/docs/reference.rst` & `jsonrpc-py-3.0.7/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/__init__.py` & `jsonrpc-py-3.0.7/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/asgi.py` & `jsonrpc-py-3.0.7/jsonrpc/asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.7/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/errors.py` & `jsonrpc-py-3.0.7/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/request.py` & `jsonrpc-py-3.0.7/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/response.py` & `jsonrpc-py-3.0.7/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/serializer.py` & `jsonrpc-py-3.0.7/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.7/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/jsonrpc/utilities.py` & `jsonrpc-py-3.0.7/jsonrpc/utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from asyncio import AbstractEventLoop, Future, Task, TaskGroup, get_running_loop
 from collections.abc import Callable, Coroutine, Generator, Iterable, Iterator, MutableMapping
 from contextvars import Context, copy_context
+from dataclasses import dataclass, field
 from functools import partial
+from heapq import heappop, heappush
 from inspect import iscoroutinefunction
-from typing import Any, Final, Literal, ParamSpec, TypeAlias, TypeGuard, TypeVar, final
+from typing import Any, Final, Generic, Literal, ParamSpec, TypeAlias, TypeGuard, TypeVar, final
 
 __all__: Final[tuple[str, ...]] = (
     "ensure_async",
     "is_iterable",
     "make_hashable",
     "multiple_coroutines",
     "Undefined",
@@ -52,41 +54,62 @@
         #: ---
         #: Non-hashable, non-iterable:
         raise
 
     return obj
 
 
-async def multiple_coroutines(coroutines: Iterable[CoroutineLike[T]], /) -> list[T]:
-    def exception_from_group(exc: BaseException) -> Iterator[BaseException]:
-        if isinstance(exc_group := exc, BaseExceptionGroup):
-            for nested in exc_group.exceptions:
-                yield from exception_from_group(nested)
-        else:
-            yield exc
+@dataclass(eq=False, slots=True)
+class multiple_coroutines(Generic[T]):
+    coroutines: Iterable[CoroutineLike[T]]
+    results: list[tuple[int, T]] = field(default_factory=list, init=False)
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__qualname__}({self.coroutines!r})"
+
+    def __await__(self) -> Generator[Any, None, list[T]]:
+        #: ---
+        #: Create a suitable iterator by calling __await__ on a coroutine.
+        return self.__await_impl__().__await__()
+
+    async def __await_impl__(self) -> list[T]:
+        context: Final[Context] = copy_context()
+        try:
+            async with TaskGroup() as tg:
+                for priority, coroutine in enumerate(self.coroutines):
+                    task: Task[T] = tg.create_task(coroutine, context=context)
+                    callback: partial[None] = partial(self.populate_results, priority=priority)
+                    task.add_done_callback(callback, context=context)
+        except BaseExceptionGroup as exc_group:
+            #: ---
+            #: Propagate the first raised exception from exception group:
+            exc, *_ = self.exception_from_group(exc_group)
+            raise exc from None
 
-    def populate_results(task: Task[T]) -> None:
+        return list(self.iter_results())
+
+    def populate_results(self, task: Task[T], *, priority: int) -> None:
         if not task.cancelled() and task.exception() is None:
             result: Final[T] = task.result()
-            results.append(result)
+            heappush(self.results, (priority, result))
 
-    context: Context = copy_context()
-    results: list[T] = []
-    try:
-        async with TaskGroup() as tg:
-            for _, coroutine in enumerate(coroutines):
-                task: Task[T] = tg.create_task(coroutine, context=context)
-                task.add_done_callback(populate_results, context=context)
-    except BaseExceptionGroup as exc_group:
-        #: ---
-        #: Propagate the first raised exception from exception group:
-        exc, *_ = exception_from_group(exc_group)
-        raise exc from None
+    def exception_from_group(self, exc: BaseException) -> Iterator[BaseException]:
+        if isinstance(exc_group := exc, BaseExceptionGroup):
+            for nested in exc_group.exceptions:
+                yield from self.exception_from_group(nested)
+        else:
+            yield exc
 
-    return results
+    def iter_results(self) -> Iterator[T]:
+        while True:
+            try:
+                _, result = heappop(self.results)
+                yield result
+            except IndexError:
+                break
 
 
 @final
 class UndefinedType:
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> Literal["Undefined"]:
```

### Comparing `jsonrpc-py-3.0.6/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.7/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.6
+Version: 3.0.7
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.6/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.7/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
 docs/changelog/v3.x.x/v3.0.5.rst
 docs/changelog/v3.x.x/v3.0.6.rst
+docs/changelog/v3.x.x/v3.0.7.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.6/pyproject.toml` & `jsonrpc-py-3.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_asgi.py` & `jsonrpc-py-3.0.7/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_dispatcher.py` & `jsonrpc-py-3.0.7/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_errors.py` & `jsonrpc-py-3.0.7/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_request.py` & `jsonrpc-py-3.0.7/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_response.py` & `jsonrpc-py-3.0.7/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_serializer.py` & `jsonrpc-py-3.0.7/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.6/tests/test_utilities.py` & `jsonrpc-py-3.0.7/tests/test_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,25 @@
         self.assertIsInstance(results, MutableSequence)
         self.assertCountEqual(results, ["a", "b", "c"])
 
         for mock in mocks:
             with self.subTest(mock=mock):
                 mock.assert_awaited_once()
 
+    async def test_multiple_coroutines_preserved_order(self) -> None:
+        results: list[str] = await multiple_coroutines(
+            (
+                sleep(0.04, "a"),  # <-- accepted latest but should be first in results
+                sleep(0.02, "b"),  # <-- accepted second and should be second in results
+                sleep(0.01, "c"),  # <-- accepted first but should be third in results
+                sleep(0.03, "d"),  # <-- accepted third but should be latest in results
+            )
+        )
+        self.assertListEqual(results, ["a", "b", "c", "d"])
+
     async def test_multiple_coroutines_exception(self) -> None:
         first_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("first exception"))
         second_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("second exception"))
 
         async def inner(mock: AsyncMock) -> Any:
             return await mock()
```

