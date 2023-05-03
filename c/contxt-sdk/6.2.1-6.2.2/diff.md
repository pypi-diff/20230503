# Comparing `tmp/contxt_sdk-6.2.1.tar.gz` & `tmp/contxt_sdk-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contxt_sdk-6.2.1.tar", max compression
+gzip compressed data, was "contxt_sdk-6.2.2.tar", max compression
```

## Comparing `contxt_sdk-6.2.1.tar` & `contxt_sdk-6.2.2.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0      738 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/LICENSE
--rw-r--r--   0        0        0      589 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/README.md
--rw-r--r--   0        0        0      193 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/__init__.py
--rw-r--r--   0        0        0       64 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/__main__.py
--rw-r--r--   0        0        0     2442 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/auth/__init__.py
--rw-r--r--   0        0        0    11776 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/auth/cli.py
--rw-r--r--   0        0        0     1790 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/auth/jwt.py
--rw-r--r--   0        0        0     1437 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/auth/machine.py
--rw-r--r--   0        0        0     1964 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/clients.py
--rw-r--r--   0        0        0      611 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/auth.py
--rw-r--r--   0        0        0     3801 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/clusters.py
--rw-r--r--   0        0        0      740 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/edge_nodes.py
--rw-r--r--   0        0        0     5990 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/ems.py
--rw-r--r--   0        0        0     1348 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/facilities.py
--rw-r--r--   0        0        0    12886 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/iot.py
--rw-r--r--   0        0        0      832 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/metrics.py
--rw-r--r--   0        0        0      571 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/orgs.py
--rw-r--r--   0        0        0     3404 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/project_envs.py
--rw-r--r--   0        0        0     2422 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/projects.py
--rw-r--r--   0        0        0     2134 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/service_instances.py
--rw-r--r--   0        0        0     1770 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/commands/services.py
--rw-r--r--   0        0        0     1333 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/log.py
--rw-r--r--   0        0        0     1776 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/main.py
--rw-r--r--   0        0        0     3200 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/cli/utils.py
--rw-r--r--   0        0        0     7066 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/models/__init__.py
--rw-r--r--   0        0        0     3918 2023-04-28 14:02:36.334593 contxt_sdk-6.2.1/contxt/models/bus.py
--rw-r--r--   0        0        0    11536 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/contxt.py
--rw-r--r--   0        0        0     8567 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/ems.py
--rw-r--r--   0        0        0     2751 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/etl.py
--rw-r--r--   0        0        0     4702 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/events.py
--rw-r--r--   0        0        0     2119 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/facilities.py
--rw-r--r--   0        0        0     7031 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/iot.py
--rw-r--r--   0        0        0     1461 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/models/sis.py
--rw-r--r--   0        0        0       63 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/py.typed
--rw-r--r--   0        0        0      361 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/__init__.py
--rw-r--r--   0        0        0     7563 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/api.py
--rw-r--r--   0        0        0     1614 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/auth.py
--rw-r--r--   0        0        0     2440 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/bus.py
--rw-r--r--   0        0        0     4662 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/contxt.py
--rw-r--r--   0        0        0     1435 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/contxt_deployments.py
--rw-r--r--   0        0        0     4711 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/ems.py
--rw-r--r--   0        0        0     4428 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/events.py
--rw-r--r--   0        0        0    17622 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/iot.py
--rw-r--r--   0        0        0     3968 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/ngest.py
--rw-r--r--   0        0        0     2190 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/nionic.py
--rw-r--r--   0        0        0     6318 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/services/pagination.py
--rw-r--r--   0        0        0     2151 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/utils/__init__.py
--rw-r--r--   0        0        0     4501 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/utils/object_mapper.py
--rw-r--r--   0        0        0      546 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/utils/orgs.py
--rw-r--r--   0        0        0     8000 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/utils/serializer.py
--rw-r--r--   0        0        0     1558 2023-04-28 14:02:36.350594 contxt_sdk-6.2.1/contxt/workers.py
--rw-r--r--   0        0        0     1535 2023-04-28 14:02:52.203367 contxt_sdk-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 contxt_sdk-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-05-03 13:09:46.614061 contxt_sdk-6.2.2/LICENSE
+-rw-r--r--   0        0        0      678 2023-05-03 13:09:46.614061 contxt_sdk-6.2.2/README.md
+-rw-r--r--   0        0        0      193 2023-05-03 13:09:46.614061 contxt_sdk-6.2.2/contxt/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/__main__.py
+-rw-r--r--   0        0        0     2442 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/auth/__init__.py
+-rw-r--r--   0        0        0    11776 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/auth/cli.py
+-rw-r--r--   0        0        0     1790 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/auth/jwt.py
+-rw-r--r--   0        0        0     1437 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/auth/machine.py
+-rw-r--r--   0        0        0     1962 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/clients.py
+-rw-r--r--   0        0        0      611 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/auth.py
+-rw-r--r--   0        0        0     3801 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/clusters.py
+-rw-r--r--   0        0        0      740 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/edge_nodes.py
+-rw-r--r--   0        0        0     5990 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/ems.py
+-rw-r--r--   0        0        0     1348 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/facilities.py
+-rw-r--r--   0        0        0    12886 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/iot.py
+-rw-r--r--   0        0        0      832 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/metrics.py
+-rw-r--r--   0        0        0      571 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/orgs.py
+-rw-r--r--   0        0        0     3404 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/project_envs.py
+-rw-r--r--   0        0        0     2422 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/projects.py
+-rw-r--r--   0        0        0     2134 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/service_instances.py
+-rw-r--r--   0        0        0     1770 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/commands/services.py
+-rw-r--r--   0        0        0     1333 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/log.py
+-rw-r--r--   0        0        0     1738 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/main.py
+-rw-r--r--   0        0        0     3200 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/cli/utils.py
+-rw-r--r--   0        0        0     7066 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/__init__.py
+-rw-r--r--   0        0        0     3918 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/bus.py
+-rw-r--r--   0        0        0    11536 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/contxt.py
+-rw-r--r--   0        0        0     8567 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/ems.py
+-rw-r--r--   0        0        0     2751 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/etl.py
+-rw-r--r--   0        0        0     4702 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/events.py
+-rw-r--r--   0        0        0     2119 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/facilities.py
+-rw-r--r--   0        0        0     7031 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/iot.py
+-rw-r--r--   0        0        0     1461 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/models/sis.py
+-rw-r--r--   0        0        0       63 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/py.typed
+-rw-r--r--   0        0        0      361 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/__init__.py
+-rw-r--r--   0        0        0     7563 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/api.py
+-rw-r--r--   0        0        0     1614 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/auth.py
+-rw-r--r--   0        0        0     2440 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/bus.py
+-rw-r--r--   0        0        0     4662 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/contxt.py
+-rw-r--r--   0        0        0     1435 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/contxt_deployments.py
+-rw-r--r--   0        0        0     4654 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/ems.py
+-rw-r--r--   0        0        0     4344 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/events.py
+-rw-r--r--   0        0        0    17538 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/iot.py
+-rw-r--r--   0        0        0     3918 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/ngest.py
+-rw-r--r--   0        0        0     2106 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/nionic.py
+-rw-r--r--   0        0        0     6318 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/services/pagination.py
+-rw-r--r--   0        0        0     2151 2023-05-03 13:09:46.618061 contxt_sdk-6.2.2/contxt/utils/__init__.py
+-rw-r--r--   0        0        0     4501 2023-05-03 13:09:46.622061 contxt_sdk-6.2.2/contxt/utils/object_mapper.py
+-rw-r--r--   0        0        0     8000 2023-05-03 13:09:46.622061 contxt_sdk-6.2.2/contxt/utils/serializer.py
+-rw-r--r--   0        0        0     1558 2023-05-03 13:09:46.622061 contxt_sdk-6.2.2/contxt/workers.py
+-rw-r--r--   0        0        0     1535 2023-05-03 13:10:10.094180 contxt_sdk-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 contxt_sdk-6.2.2/PKG-INFO
```

### Comparing `contxt_sdk-6.2.1/LICENSE` & `contxt_sdk-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/README.md` & `contxt_sdk-6.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 
 ## CLI Usage
 
 ```sh
 contxt --help
 ```
 
+## Tests
+
+```sh
+docker compose up -d --wait
+poetry run poe test
+docker compose down
+```
+
 ## Documentation
 
 Please refer to <https://ndustrialio.github.io/contxt-sdk-python>.
 
 ## Contributing
 
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `contxt_sdk-6.2.1/contxt/auth/__init__.py` & `contxt_sdk-6.2.2/contxt/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/auth/cli.py` & `contxt_sdk-6.2.2/contxt/auth/cli.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/auth/jwt.py` & `contxt_sdk-6.2.2/contxt/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/auth/machine.py` & `contxt_sdk-6.2.2/contxt/auth/machine.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/clients.py` & `contxt_sdk-6.2.2/contxt/cli/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Optional
 
 import click
 
 from contxt.auth.cli import CliAuth
 from contxt.services import (
     ContxtDeploymentService,
     ContxtService,
@@ -16,15 +15,15 @@
 
 
 @dataclass
 class Clients:
     """Holds a user and all client API's"""
 
     env: str
-    org_slug: Optional[str]
+    org_slug: str
 
     @cachedproperty
     def org_id(self) -> str:
         if not self.org_slug:
             # Check if user only has access to a single org
             token = self.contxt.session.auth.token_provider.decoded_access_token
             orgs = token.get("organizations", [])
@@ -46,20 +45,20 @@
 
     @cachedproperty
     def contxt_deployments(self) -> ContxtDeploymentService:
         return ContxtDeploymentService(auth=self.auth, env=self.env)
 
     @cachedproperty
     def ems(self) -> EmsService:
-        return EmsService(auth=self.auth, env=self.env, org_id=self.org_id)
+        return EmsService(auth=self.auth, env=self.env, org_id=self.org_id, org_slug=self.org_slug)
 
     @cachedproperty
     def events(self) -> EventsService:
-        return EventsService(auth=self.auth, env=self.env, org_id=self.org_id)
+        return EventsService(auth=self.auth, env=self.env, org_slug=self.org_slug)
 
     @cachedproperty
     def nionic(self) -> NionicService:
-        return NionicService(auth=self.auth, env=self.env, org_id=self.org_id)
+        return NionicService(auth=self.auth, env=self.env, org_slug=self.org_slug)
 
     @cachedproperty
     def iot(self) -> IotService:
-        return IotService(auth=self.auth, env=self.env, org_id=self.org_id)
+        return IotService(auth=self.auth, env=self.env, org_slug=self.org_slug)
```

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/auth.py` & `contxt_sdk-6.2.2/contxt/cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/clusters.py` & `contxt_sdk-6.2.2/contxt/cli/commands/clusters.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/edge_nodes.py` & `contxt_sdk-6.2.2/contxt/cli/commands/edge_nodes.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/ems.py` & `contxt_sdk-6.2.2/contxt/cli/commands/ems.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/facilities.py` & `contxt_sdk-6.2.2/contxt/cli/commands/facilities.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/iot.py` & `contxt_sdk-6.2.2/contxt/cli/commands/iot.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/metrics.py` & `contxt_sdk-6.2.2/contxt/cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/orgs.py` & `contxt_sdk-6.2.2/contxt/cli/commands/orgs.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/project_envs.py` & `contxt_sdk-6.2.2/contxt/cli/commands/project_envs.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/projects.py` & `contxt_sdk-6.2.2/contxt/cli/commands/projects.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/service_instances.py` & `contxt_sdk-6.2.2/contxt/cli/commands/service_instances.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/commands/services.py` & `contxt_sdk-6.2.2/contxt/cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/log.py` & `contxt_sdk-6.2.2/contxt/cli/log.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/cli/main.py` & `contxt_sdk-6.2.2/contxt/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Main CLI"""
 
 import logging
 from pathlib import Path
-from typing import Optional
 
 import click
 from requests import RequestException
 
 from contxt import __version__
 from contxt.cli.clients import Clients
 from contxt.cli.log import init as init_logger
@@ -47,15 +46,15 @@
     envvar="CONTXT_ENV",
     help="Environment for all API's",
 )
 @click.option("--org", envvar="CONTXT_ORG", help="Organization slug")
 @click.option("-v", "--verbose", count=True, help="Increase verbosity")
 @click.version_option(__version__, "-V", "--version")
 @click.pass_context
-def cli(ctx: click.Context, env: str, org: Optional[str], verbose: int) -> None:
+def cli(ctx: click.Context, env: str, org: str, verbose: int) -> None:
     """Contxt CLI"""
     init_logger(verbose)
     ctx.obj = Clients(env=env, org_slug=org)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `contxt_sdk-6.2.1/contxt/cli/utils.py` & `contxt_sdk-6.2.2/contxt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/__init__.py` & `contxt_sdk-6.2.2/contxt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/bus.py` & `contxt_sdk-6.2.2/contxt/models/bus.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/contxt.py` & `contxt_sdk-6.2.2/contxt/models/contxt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/ems.py` & `contxt_sdk-6.2.2/contxt/models/ems.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/etl.py` & `contxt_sdk-6.2.2/contxt/models/etl.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/events.py` & `contxt_sdk-6.2.2/contxt/models/events.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/facilities.py` & `contxt_sdk-6.2.2/contxt/models/facilities.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/iot.py` & `contxt_sdk-6.2.2/contxt/models/iot.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/models/sis.py` & `contxt_sdk-6.2.2/contxt/models/sis.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/api.py` & `contxt_sdk-6.2.2/contxt/services/api.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/auth.py` & `contxt_sdk-6.2.2/contxt/services/auth.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/bus.py` & `contxt_sdk-6.2.2/contxt/services/bus.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/contxt.py` & `contxt_sdk-6.2.2/contxt/services/contxt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/contxt_deployments.py` & `contxt_sdk-6.2.2/contxt/services/contxt_deployments.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/services/ems.py` & `contxt_sdk-6.2.2/contxt/services/ems.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import date, datetime, timedelta, timezone
 from typing import Iterable, List, Optional
 
 from ..auth import Auth
 from ..models.ems import Facility, MainService, ResourceType, UtilityContract, UtilitySpend, UtilityUsage
-from ..utils.orgs import get_slug_or_org_id
 from .api import ApiEnvironment, ConfiguredApi
 from .pagination import PagedRecords
 
 
 class EmsService(ConfiguredApi):
     """EMS API client"""
 
@@ -20,19 +19,20 @@
         ApiEnvironment(
             name="staging",
             base_url="https://{tenant}.api.staging.ndustrial.io/rest/ems/v1",
             client_id="vMV67yaRFgjBB1JFbT3vXBOlohFdG1I4",
         ),
     )
 
-    def __init__(self, auth: Auth, org_id: str, env: str = "production", **kwargs) -> None:
+    def __init__(
+        self, auth: Auth, org_id: str, org_slug: str, env: str = "production", **kwargs
+    ) -> None:
         super().__init__(env=env, auth=auth, **kwargs)
         self.org_id = org_id
-        tenant = get_slug_or_org_id(org_id)
-        self.base_url = self.base_url.format(tenant=tenant)
+        self.base_url = self.base_url.format(tenant=org_slug)
 
     def get_facility(self, id: int) -> Facility:
         return Facility.from_api(self.get(f"{self.org_id}/facilities/{id}"))
 
     def get_main_services(
         self, facility_id: int, resource_type: Optional[ResourceType] = None
     ) -> List[MainService]:
```

### Comparing `contxt_sdk-6.2.1/contxt/services/events.py` & `contxt_sdk-6.2.2/contxt/services/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Iterable, List, Optional
 
 from ..auth import Auth
 from ..models.events import Event, EventDefinition, EventType, TriggeredEvent
-from ..utils.orgs import get_slug_or_org_id
 from .api import ApiEnvironment, ConfiguredApi
 from .pagination import PagedRecords, PageOptions
 
 
 class EventsService(ConfiguredApi):
     """Events API client"""
 
@@ -19,18 +18,17 @@
         ApiEnvironment(
             name="staging",
             base_url="https://{tenant}.api.staging.ndustrial.io/rest/events/v1",
             client_id="dn4MaocJFdKtsBy9sFFaTeuJWL1nt5xu",
         ),
     )
 
-    def __init__(self, auth: Auth, org_id: str, env: str = "production", **kwargs) -> None:
+    def __init__(self, auth: Auth, org_slug: str, env: str = "production", **kwargs) -> None:
         super().__init__(env=env, auth=auth, **kwargs)
-        tenant = get_slug_or_org_id(org_id)
-        self.base_url = self.base_url.format(tenant=tenant)
+        self.base_url = self.base_url.format(tenant=org_slug)
 
     def set_human_readable_parameters(self, event_definition: EventDefinition) -> None:
         statement = ""
         for k, v in event_definition.parameters.items():
             if k == "$chain":
                 for d1, d2 in zip(v[:-1], v[1:]):
                     event1 = self.get_event(d1.get("event_id"))
```

### Comparing `contxt_sdk-6.2.1/contxt/services/iot.py` & `contxt_sdk-6.2.2/contxt/services/iot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     FieldGrouping,
     FieldTimeSeries,
     UnprovisionedField,
     Window,
 )
 from ..utils import is_datetime_aware, make_logger
 from ..utils.object_mapper import ObjectMapper
-from ..utils.orgs import get_slug_or_org_id
 from .api import ApiEnvironment, ConfiguredApi
 from .pagination import DataPoint, PagedRecords, PagedTimeSeries, PageOptions
 
 logger = make_logger(__name__)
 
 
 class IotService(ConfiguredApi):
@@ -46,18 +45,17 @@
         ApiEnvironment(
             name="staging",
             base_url="https://{tenant}.api.staging.ndustrial.io/rest/iot/v1",
             client_id="m35AEcxD8hf65sq04ZU7yFxqpqVkKzES",
         ),
     )
 
-    def __init__(self, auth: Auth, org_id: str, env: str = "production", **kwargs) -> None:
+    def __init__(self, auth: Auth, org_slug: str, env: str = "production", **kwargs) -> None:
         super().__init__(env=env, auth=auth, **kwargs)
-        tenant = get_slug_or_org_id(org_id)
-        self.base_url = self.base_url.format(tenant=tenant)
+        self.base_url = self.base_url.format(tenant=org_slug)
 
     def provision_field_for_feed(self, feed_id: int, field: Field) -> Field:
         resp = self.post(f"feeds/{feed_id}/fields", data=field.post())
         return Field.from_api(resp)
 
     def create_grouping(
         self, facility_id: int, label: str, description: str, is_public: bool, field_category_id: str
```

### Comparing `contxt_sdk-6.2.1/contxt/services/ngest.py` & `contxt_sdk-6.2.2/contxt/services/ngest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from copy import deepcopy
 from datetime import datetime, timezone
 from typing import Dict, List
 
 from ..utils import is_datetime_aware, make_logger
-from ..utils.orgs import get_slug_or_org_id
 from .api import ApiEnvironment, ConfiguredApi
 
 logger = make_logger(__name__)
 
 
 class NgestService(ConfiguredApi):
     """Ngest API client"""
@@ -16,25 +15,26 @@
         ApiEnvironment(
             name="production",
             base_url="https://{tenant}.api.ndustrial.io/rest/data/v1",
             client_id="AhVAWkq2FEoQtWAP7EidZ9uzrc4ED1Dx",
         ),
     )
 
-    def __init__(self, org_id: str, env: str = "production", **kwargs) -> None:
+    def __init__(self, org_slug: str, env: str = "production", **kwargs) -> None:
         self.env = env
         super().__init__(env=env, **kwargs)
-        tenant = get_slug_or_org_id(org_id)
-        self.base_url = self.base_url.format(tenant=tenant)
+        self.base_url = self.base_url.format(tenant=org_slug)
 
     @staticmethod
     def specialize(
-        feed_key: str, feed_token: str, org_id: str, env: str = "production"
+        feed_key: str, feed_token: str, org_slug: str, env: str = "production"
     ) -> "SpecializedNgestService":
-        return SpecializedNgestService(env=env, feed_key=feed_key, feed_token=feed_token, org_id=org_id)
+        return SpecializedNgestService(
+            env=env, feed_key=feed_key, feed_token=feed_token, org_slug=org_slug
+        )
 
     def _format_time_series(self, feed_key: str, time_series: Dict[str, Dict[datetime, float]]) -> Dict:
         # Enforce all datetimes are tz-aware
         assert all(
             is_datetime_aware(dt) for time_series in time_series.values() for dt in time_series.keys()
         ), "Timezone-aware datetimes required"
 
@@ -91,16 +91,16 @@
             # Update remaining data
             data["data"] = data["data"][per_request:]
 
         return responses
 
 
 class SpecializedNgestService(NgestService):
-    def __init__(self, feed_key: str, feed_token: str, org_id: str, env: str = "production") -> None:
-        super().__init__(env=env, org_id=org_id)
+    def __init__(self, feed_key: str, feed_token: str, org_slug: str, env: str = "production") -> None:
+        super().__init__(env=env, org_slug=org_slug)
         self.feed_key = feed_key
         self.feed_token = feed_token
 
     def send_time_series(  # type: ignore
         self, time_series: Dict[str, Dict[datetime, float]], per_request: int = 50
     ) -> List[Dict]:
         return super().send_time_series(
```

### Comparing `contxt_sdk-6.2.1/contxt/services/nionic.py` & `contxt_sdk-6.2.2/contxt/services/nionic.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from sgqlc.endpoint.requests import RequestsEndpoint
 from sgqlc.operation import Operation
 
 from contxt.models.facilities import Facility, MetricData, MetricLabel, Mutation, Query
 from contxt.services.api import ApiEnvironment, BaseGraphService
 
 from ..auth import Auth
-from ..utils.orgs import get_slug_or_org_id
 
 
 class NionicService(BaseGraphService):
     """Nionic API client"""
 
     _envs = (
         ApiEnvironment(
@@ -22,18 +21,17 @@
         ApiEnvironment(
             name="staging",
             base_url="https://{tenant}.api.staging.ndustrial.io",
             client_id="vhGxildn8hRRWZj49y18BGtbjTkFHcTG",
         ),
     )
 
-    def __init__(self, auth: Auth, org_id: str, env: str = "production", **kwargs) -> None:
+    def __init__(self, auth: Auth, org_slug: str, env: str = "production", **kwargs) -> None:
         super().__init__(env=env, auth=auth, **kwargs)
-        tenant = get_slug_or_org_id(org_id)
-        self.base_url = self.base_url.format(tenant=tenant)
+        self.base_url = self.base_url.format(tenant=org_slug)
         self.endpoint = RequestsEndpoint(self.base_url.rstrip("/") + "/graphql", session=self.session)
 
     def get_facilities(self) -> List[Facility]:
         op = Operation(Query)
         op.facilities().nodes().__fields__(*list(Facility._ContainerTypeMeta__fields.keys()))
         return (op + self.run(op)).facilities.nodes
```

### Comparing `contxt_sdk-6.2.1/contxt/services/pagination.py` & `contxt_sdk-6.2.2/contxt/services/pagination.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/utils/__init__.py` & `contxt_sdk-6.2.2/contxt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/utils/object_mapper.py` & `contxt_sdk-6.2.2/contxt/utils/object_mapper.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/utils/serializer.py` & `contxt_sdk-6.2.2/contxt/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/contxt/workers.py` & `contxt_sdk-6.2.2/contxt/workers.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.2.1/pyproject.toml` & `contxt_sdk-6.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contxt-sdk"
-version = "6.2.1"
+version = "6.2.2"
 description = "Contxt SDK from ndustrial"
 authors = ["ndustrial <dev@ndustrial.io>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/ndustrialio/contxt-sdk-python"
 packages = [ { include = "contxt" } ]
```

### Comparing `contxt_sdk-6.2.1/PKG-INFO` & `contxt_sdk-6.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contxt-sdk
-Version: 6.2.1
+Version: 6.2.2
 Summary: Contxt SDK from ndustrial
 Home-page: https://github.com/ndustrialio/contxt-sdk-python
 License: ISC
 Author: ndustrial
 Author-email: dev@ndustrial.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
@@ -40,14 +40,22 @@
 
 ## CLI Usage
 
 ```sh
 contxt --help
 ```
 
+## Tests
+
+```sh
+docker compose up -d --wait
+poetry run poe test
+docker compose down
+```
+
 ## Documentation
 
 Please refer to <https://ndustrialio.github.io/contxt-sdk-python>.
 
 ## Contributing
 
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md).
```

