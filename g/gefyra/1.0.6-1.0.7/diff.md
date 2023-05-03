# Comparing `tmp/gefyra-1.0.6.tar.gz` & `tmp/gefyra-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.0.6.tar", max compression
+gzip compressed data, was "gefyra-1.0.7.tar", max compression
```

## Comparing `gefyra-1.0.6.tar` & `gefyra-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2151 2023-04-26 14:08:38.703776 gefyra-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/__init__.py
--rw-r--r--   0        0        0    13357 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/__main__.py
--rw-r--r--   0        0        0      169 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/list.py
--rw-r--r--   0        0        0     6142 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/up.py
--rw-r--r--   0        0        0     1264 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     5507 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8850 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     1608 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8959 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6677 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1037 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0      945 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/networking.py
--rw-r--r--   0        0        0     3918 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-04-26 14:08:38.707776 gefyra-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-05-03 12:42:11.634061 gefyra-1.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/__init__.py
+-rw-r--r--   0        0        0    13357 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/__main__.py
+-rw-r--r--   0        0        0      169 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/list.py
+-rw-r--r--   0        0        0     6142 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/up.py
+-rw-r--r--   0        0        0     1264 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     5507 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     1608 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8988 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1037 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0      945 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3940 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-05-03 12:42:11.634061 gefyra-1.0.7/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-03 12:42:11.634061 gefyra-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.7/PKG-INFO
```

### Comparing `gefyra-1.0.6/README.md` & `gefyra-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/__main__.py` & `gefyra-1.0.7/gefyra/__main__.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/bridge.py` & `gefyra-1.0.7/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/down.py` & `gefyra-1.0.7/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/list.py` & `gefyra-1.0.7/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/run.py` & `gefyra-1.0.7/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/status.py` & `gefyra-1.0.7/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/up.py` & `gefyra-1.0.7/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/api/utils.py` & `gefyra-1.0.7/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/cluster/manager.py` & `gefyra-1.0.7/gefyra/cluster/manager.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/cluster/resources.py` & `gefyra-1.0.7/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/cluster/utils.py` & `gefyra-1.0.7/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/configuration.py` & `gefyra-1.0.7/gefyra/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.0.6"
+__VERSION__ = "1.0.7"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
@@ -101,14 +101,15 @@
             self.CARGO_ENDPOINT = f"{cargo_endpoint_host}:{cargo_endpoint_port}"
         else:
             docker_os = self._get_docker_info_by_name("OperatingSystem")
             docker_server_name = self._get_docker_info_by_name("Name")
             logger.debug(f"Docker OS: {docker_os}")
             logger.debug(f"Docker Server Name: {docker_server_name}")
             # virtualized envs don't expose network interface to host
+            print(docker_os)
             if (
                 "docker desktop" in docker_os
                 or "windows" in docker_os
                 or "colima" in docker_server_name
             ):
                 try:
                     _ip_output = self.DOCKER.containers.run(
```

### Comparing `gefyra-1.0.6/gefyra/local/bridge.py` & `gefyra-1.0.7/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/cargo.py` & `gefyra-1.0.7/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.0.7/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/check.py` & `gefyra-1.0.7/gefyra/local/check.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/minikube.py` & `gefyra-1.0.7/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/networking.py` & `gefyra-1.0.7/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/gefyra/local/telemetry.py` & `gefyra-1.0.7/gefyra/local/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # All the data we collect is published here: ``
 # This data is supposed to help us develop Gefyra and make it a better tool, prioritize
 # issues and work on bugs, features and review of pull requests.
 # If you do not which to send telemetry data this is totally fine.
 # Just opt out via `gefyra telemetry --off`.
 #########################################################################################
 
-SENTRY_DSN = "https://a94b0a0194b045f79897f70f9727d299@sentry.unikube.io/3"
+SENTRY_DSN = "https://97c8c0409cb74a079a93f05021b329f0@o146863.ingest.sentry.io/4505119985172480"
 
 
 class CliTelemetry:
     dir_name = ".gefyra"
     file_name = "config.ini"
 
     def __init__(self):
```

### Comparing `gefyra-1.0.6/gefyra/local/utils.py` & `gefyra-1.0.7/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.6/pyproject.toml` & `gefyra-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.0.6"
+version = "1.0.7"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.0.6/PKG-INFO` & `gefyra-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.0.6
+Version: 1.0.7
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

