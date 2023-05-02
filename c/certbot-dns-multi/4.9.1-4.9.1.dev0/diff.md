# Comparing `tmp/certbot-dns-multi-4.9.1.tar.gz` & `tmp/certbot-dns-multi-4.9.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-multi-4.9.1.tar", last modified: Sat Feb  4 23:13:48 2023, max compression
+gzip compressed data, was "certbot-dns-multi-4.9.1.dev0.tar", last modified: Sat Nov 26 07:12:15 2022, max compression
```

## Comparing `certbot-dns-multi-4.9.1.tar` & `certbot-dns-multi-4.9.1.dev0.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.140125 certbot-dns-multi-4.9.1/.github/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2077 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.github/build-manylinux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      464 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.github/build-wheel.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.140125 certbot-dns-multi-4.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.github/workflows/test-snap.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.140125 certbot-dns-multi-4.9.1/certbot_dns_multi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)    79907 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/main.go
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/dns_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-04 23:13:47.000000 certbot-dns-multi-4.9.1/certbot_dns_multi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-04 23:13:48.000000 certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/snap/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:48.144125 certbot-dns-multi-4.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 23:13:12.000000 certbot-dns-multi-4.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2077 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.github/build-manylinux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      464 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.github/build-wheel.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.github/workflows/test-snap.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    79907 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/main.go
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/dns_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2022-11-26 07:12:14.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-11-26 07:12:15.000000 certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:15.040155 certbot-dns-multi-4.9.1.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-26 07:12:03.000000 certbot-dns-multi-4.9.1.dev0/tests/__init__.py
```

### Comparing `certbot-dns-multi-4.9.1/.github/build-manylinux.py` & `certbot-dns-multi-4.9.1.dev0/.github/build-manylinux.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/.github/workflows/build-and-publish.yml` & `certbot-dns-multi-4.9.1.dev0/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/.github/workflows/test-snap.yml` & `certbot-dns-multi-4.9.1.dev0/.github/workflows/test-snap.yml`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/LICENSE.txt` & `certbot-dns-multi-4.9.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/PKG-INFO` & `certbot-dns-multi-4.9.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-multi
-Version: 4.9.1
+Version: 4.9.1.dev0
 Summary: Certbot DNS plugin supporting multiple providers, using github.com/go-acme/lego
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `certbot-dns-multi-4.9.1/README.md` & `certbot-dns-multi-4.9.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/go.mod` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/go.mod`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/go.sum` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/go.sum`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/bridge/main.go` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/bridge/main.go`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi/_internal/dns_multi.py` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi/_internal/dns_multi.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/PKG-INFO` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-multi
-Version: 4.9.1
+Version: 4.9.1.dev0
 Summary: Certbot DNS plugin supporting multiple providers, using github.com/go-acme/lego
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `certbot-dns-multi-4.9.1/certbot_dns_multi.egg-info/SOURCES.txt` & `certbot-dns-multi-4.9.1.dev0/certbot_dns_multi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 .flake8
 .gitignore
-Dockerfile
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 .github/build-manylinux.py
 .github/build-wheel.sh
 .github/workflows/build-and-publish.yml
-.github/workflows/docker.yml
 .github/workflows/test-snap.yml
 certbot_dns_multi/__init__.py
 certbot_dns_multi/_version.py
 certbot_dns_multi.egg-info/PKG-INFO
 certbot_dns_multi.egg-info/SOURCES.txt
 certbot_dns_multi.egg-info/dependency_links.txt
 certbot_dns_multi.egg-info/entry_points.txt
```

### Comparing `certbot-dns-multi-4.9.1/pyproject.toml` & `certbot-dns-multi-4.9.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/setup.py` & `certbot-dns-multi-4.9.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-multi-4.9.1/snap/snapcraft.yaml` & `certbot-dns-multi-4.9.1.dev0/snap/snapcraft.yaml`

 * *Files identical despite different names*

