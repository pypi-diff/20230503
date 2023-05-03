# Comparing `tmp/pulumi_docker-4.3.0a1682956971.tar.gz` & `tmp/pulumi_docker-4.3.0a1683145388.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker-4.3.0a1682956971.tar", last modified: Mon May  1 16:08:21 2023, max compression
+gzip compressed data, was "pulumi_docker-4.3.0a1683145388.tar", last modified: Wed May  3 20:28:05 2023, max compression
```

## Comparing `pulumi_docker-4.3.0a1682956971.tar` & `pulumi_docker-4.3.0a1683145388.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:21.197832 pulumi_docker-4.3.0a1682956971/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-01 16:08:21.197832 pulumi_docker-4.3.0a1682956971/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:21.193832 pulumi_docker-4.3.0a1682956971/pulumi_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:21.197832 pulumi_docker-4.3.0a1682956971/pulumi_docker/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/get_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/get_remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:21.193832 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 16:08:21.000000 pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:21.197832 pulumi_docker-4.3.0a1682956971/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-01 16:08:20.000000 pulumi_docker-4.3.0a1682956971/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/pulumi_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/pulumi_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/get_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/get_remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:28:05.769434 pulumi_docker-4.3.0a1683145388/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 20:28:05.000000 pulumi_docker-4.3.0a1683145388/setup.py
```

### Comparing `pulumi_docker-4.3.0a1682956971/PKG-INFO` & `pulumi_docker-4.3.0a1683145388/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.3.0a1682956971
+Version: 4.3.0a1683145388
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -43,15 +43,15 @@
 
     $ pip install pulumi_docker
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-docker/sdk/v3
+    $ go get github.com/pulumi/pulumi-docker/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Docker
```

### Comparing `pulumi_docker-4.3.0a1682956971/README.md` & `pulumi_docker-4.3.0a1683145388/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     $ pip install pulumi_docker
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-docker/sdk/v3
+    $ go get github.com/pulumi/pulumi-docker/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Docker
```

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/__init__.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/_enums.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/_inputs.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/_utilities.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/config/outputs.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/config/vars.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/container.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/get_logs.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/get_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/get_network.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/get_plugin.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/get_registry_image.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/get_remote_image.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/get_remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/image.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/network.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/outputs.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/plugin.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/provider.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/registry_image.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/remote_image.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/secret.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/service.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/service_config.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/service_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/tag.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker/volume.py` & `pulumi_docker-4.3.0a1683145388/pulumi_docker/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/PKG-INFO` & `pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-docker
-Version: 4.3.0a1682956971
+Version: 4.3.0a1683145388
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -43,15 +43,15 @@
 
     $ pip install pulumi_docker
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-docker/sdk/v3
+    $ go get github.com/pulumi/pulumi-docker/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Docker
```

### Comparing `pulumi_docker-4.3.0a1682956971/pulumi_docker.egg-info/SOURCES.txt` & `pulumi_docker-4.3.0a1683145388/pulumi_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.3.0a1682956971/setup.py` & `pulumi_docker-4.3.0a1683145388/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.3.0a1682956971"
-PLUGIN_VERSION = "4.3.0-alpha.1682956971+e0b3e397"
+VERSION = "4.3.0a1683145388"
+PLUGIN_VERSION = "4.3.0-alpha.1683145388+80e3af9d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'docker', PLUGIN_VERSION])
         except OSError as error:
```

