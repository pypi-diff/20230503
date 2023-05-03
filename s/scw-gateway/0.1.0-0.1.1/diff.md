# Comparing `tmp/scw_gateway-0.1.0.tar.gz` & `tmp/scw_gateway-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.1.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.1.1.tar", max compression
```

## Comparing `scw_gateway-0.1.0.tar` & `scw_gateway-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-02 06:01:09.633059 scw_gateway-0.1.0/README.md
--rw-r--r--   0        0        0      260 2023-05-02 06:29:42.403869 scw_gateway-0.1.0/cli/cli.py
--rw-r--r--   0        0        0     2886 2023-05-02 09:05:37.136210 scw_gateway-0.1.0/cli/gateway.py
--rw-r--r--   0        0        0      875 2023-05-02 09:04:00.236075 scw_gateway-0.1.0/cli/model.py
--rw-r--r--   0        0        0      956 2023-05-02 14:16:27.256834 scw_gateway-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 scw_gateway-0.1.0/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 scw_gateway-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/cli/__init__.py
+-rw-r--r--   0        0        0     2456 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/cli/cli.py
+-rw-r--r--   0        0        0     3390 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/cli/gateway.py
+-rw-r--r--   0        0        0     1170 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/cli/infra.py
+-rw-r--r--   0        0        0     1037 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/cli/model.py
+-rw-r--r--   0        0        0      956 2023-05-03 12:19:10.194080 scw_gateway-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 scw_gateway-0.1.1/setup.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 scw_gateway-0.1.1/PKG-INFO
```

### Comparing `scw_gateway-0.1.0/cli/gateway.py` & `scw_gateway-0.1.1/cli/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,40 +6,56 @@
 from cli.model import Route
 
 
 class GatewayManager(object):
     def __init__(
         self,
         admin_url,
+        local=False,
     ):
         self.admin_url = admin_url
         self.routes_url = admin_url + "/routes"
         self.services_url = admin_url + "/services"
 
-        # TODO - add auth for deployed container
-        self.auth_headers = {}
+        if local:
+            self.auth_headers = {}
+            self.scw_client = None
+            self.containers = None
+        else:
+            # TODO - add auth for deployed container
+            self.auth_headers = {} if local else {}
 
-        # Initialise SCW client
-        self.scw_client = Client.from_config_file_and_env(profile_name="dev")
+            # Initialise SCW client
+            self.scw_client = Client.from_config_file_and_env(profile_name="dev")
 
-        # Initi Scaleway APIs
-        self.containers = ContainerV1Beta1API(self.scw_client)
+            # Initi Scaleway APIs
+            self.containers = ContainerV1Beta1API(self.scw_client)
 
     def _get_gateway_container(
         self,
     ):
         # TODO - use API to get deployed gateway container
         pass
 
     def add_route(self, route: Route):
         service_url = f"{self.services_url}/{route.name}"
         route_url = f"{self.routes_url}/{route.name}"
 
         self._do_request("PUT", service_url, data=route.service_json())
         resp = self._do_request("PUT", route_url, data=route.route_json())
+
+        if route.cors:
+            plugins_url = f"{route_url}/plugins"
+
+            try:
+                self._do_request("POST", plugins_url, data=route.cors_json())
+            except requests.HTTPError:
+                # TODO - avoid ignoring this, any way to create or update?
+                pass
+
         return resp
 
     def delete_route(self, route: Route):
         self._do_request("DELETE", f"{self.routes_url}/{route.name}")
         resp = self._do_request("DELETE", f"{self.services_url}/{route.name}")
         return resp
```

### Comparing `scw_gateway-0.1.0/pyproject.toml` & `scw_gateway-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
```

### Comparing `scw_gateway-0.1.0/setup.py` & `scw_gateway-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'slack-sdk>=3.21.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['scwgw = cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scw_gateway-0.1.0/PKG-INFO` & `scw_gateway-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

