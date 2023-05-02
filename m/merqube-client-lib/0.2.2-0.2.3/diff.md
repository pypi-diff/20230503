# Comparing `tmp/merqube_client_lib-0.2.2.tar.gz` & `tmp/merqube_client_lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.2.2.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.2.3.tar", max compression
```

## Comparing `merqube_client_lib-0.2.2.tar` & `merqube_client_lib-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      207 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0    10941 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/merqube_client_lib/types.py
--rw-r--r--   0        0        0     1545 2023-05-02 19:46:00.759556 merqube_client_lib-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    10941 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/types.py
+-rw-r--r--   0        0        0     1677 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.3/PKG-INFO
```

### Comparing `merqube_client_lib-0.2.2/LICENSE` & `merqube_client_lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.2/merqube_client_lib/session.py` & `merqube_client_lib-0.2.3/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.2/pyproject.toml` & `merqube_client_lib-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.2.2"
+version = "0.2.3"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
+readme = "README.md"
+license = "APACHE-2.0"
+homepage = "https://github.com/merqube/merqube-client-lib"
+include = [
+    "LICENSE",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10,<4.0"
 requests = "*"
 pydantic = {"version" = "^1.10.5"}
 pandas = "^1.3.0"
 Flask = "~2"
```

