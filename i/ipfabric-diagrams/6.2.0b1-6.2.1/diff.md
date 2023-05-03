# Comparing `tmp/ipfabric_diagrams-6.2.0b1.tar.gz` & `tmp/ipfabric_diagrams-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_diagrams-6.2.0b1.tar", max compression
+gzip compressed data, was "ipfabric_diagrams-6.2.1.tar", max compression
```

## Comparing `ipfabric_diagrams-6.2.0b1.tar` & `ipfabric_diagrams-6.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1829 2023-03-16 17:27:29.558755 ipfabric_diagrams-6.2.0b1/ipfabric/__init__.py
--rw-r--r--   0        0        0     1666 2023-03-16 17:12:51.405968 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0     7488 2023-03-16 15:31:26.870204 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3612 2023-03-16 15:41:35.747531 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      580 2023-03-16 15:28:22.610735 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3755 2023-03-16 13:36:25.692670 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2022-08-08 12:49:07.558933 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     7009 2022-08-08 12:49:18.134109 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2277 2022-08-08 12:49:18.135111 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    10497 2023-03-16 15:25:53.031095 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    10534 2023-03-16 15:25:53.055402 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0       68 2023-03-28 16:36:30.062929 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     2608 2023-03-16 15:25:53.062465 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     1412 2023-03-28 16:01:35.397194 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     3187 2023-03-28 16:54:47.000317 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0      898 2023-03-16 17:12:51.413969 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/__init__.py
--rw-r--r--   0        0        0      167 2023-03-16 16:54:12.019841 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/graphs.py
--rw-r--r--   0        0        0     1562 2023-03-16 16:27:26.311693 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/icmp.py
--rw-r--r--   0        0        0     1087 2023-03-16 12:53:31.420028 ipfabric_diagrams-6.2.0b1/LICENSE
--rw-r--r--   0        0        0     1682 2023-03-28 17:56:52.632001 ipfabric_diagrams-6.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     2572 2023-03-16 16:54:08.805400 ipfabric_diagrams-6.2.0b1/README.md
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b1/setup.py
--rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1829 2023-03-16 17:27:29.558755 ipfabric_diagrams-6.2.1/ipfabric/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-10 12:53:47.700749 ipfabric_diagrams-6.2.1/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0     7488 2023-04-05 14:19:36.046256 ipfabric_diagrams-6.2.1/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2023-04-10 13:17:21.761764 ipfabric_diagrams-6.2.1/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      580 2023-03-16 15:28:22.610735 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3755 2023-03-16 13:36:25.692670 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2022-08-08 12:49:07.558933 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     7009 2022-08-08 12:49:18.134109 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2277 2022-08-08 12:49:18.135111 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    10507 2023-04-10 12:51:21.766806 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    10534 2023-03-16 15:25:53.055402 ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0       68 2023-03-28 16:36:30.062929 ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     2608 2023-03-16 15:25:53.062465 ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     1412 2023-03-28 16:01:35.397194 ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     3188 2023-04-10 12:49:46.822611 ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     1152 2023-04-10 12:54:57.346498 ipfabric_diagrams-6.2.1/ipfabric_diagrams/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-10 12:56:15.317912 ipfabric_diagrams-6.2.1/ipfabric_diagrams/graphs.py
+-rw-r--r--   0        0        0     2910 2023-04-10 13:13:28.968650 ipfabric_diagrams-6.2.1/ipfabric_diagrams/icmp.py
+-rw-r--r--   0        0        0     1087 2023-03-16 12:53:31.420028 ipfabric_diagrams-6.2.1/LICENSE
+-rw-r--r--   0        0        0     1678 2023-05-03 15:51:01.800119 ipfabric_diagrams-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2572 2023-03-16 16:54:08.805400 ipfabric_diagrams-6.2.1/README.md
+-rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.1/setup.py
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.1/PKG-INFO
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/__init__.py` & `ipfabric_diagrams-6.2.1/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/__init__.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,29 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from .graphs import IPFDiagram
-from .input_models import *
+from .input_models import (
+    Unicast,
+    Multicast,
+    Host2GW,
+    Network,
+    OtherOptions,
+    Algorithm,
+    EntryPoint,
+    Layout,
+    NetworkSettings,
+    PathLookupSettings,
+    Overlay,
+    VALID_NET_PROTOCOLS,
+    VALID_PATH_PROTOCOLS,
+)
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
 __all__ = [
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/graphs.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/icmp.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/icmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 AUTHENTICATION_FAILED = ICMP(type=40, code=1)
 DECOMPRESSION_FAILED = ICMP(type=40, code=2)
 DECRYPTION_FAILED = ICMP(type=40, code=3)
 NEED_AUTHENTICATION = ICMP(type=40, code=4)
 NEED_AUTHORIZATION = ICMP(type=40, code=5)
 
 __all__ = [
+    "ICMP",
     "ECHO_REPLY",
     "NET_UNREACHABLE",
     "HOST_UNREACHABLE",
     "PROTOCOL_UNREACHABLE",
     "PORT_UNREACHABLE",
     "FRAGMENTATION_NEEDED",
     "SOURCE_ROUTE_FAILED",
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/__init__.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/constants.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,11 +275,11 @@
         return v
 
     def parameters(self):
         parameters = dict(type="topology", groupBy="siteName", paths=self.sites.copy())
         if self.all_network and ALL_NETWORK not in parameters["paths"]:
             parameters["paths"].append(ALL_NETWORK)
         if self.layouts:
-            parameters["layouts"] = [vars(l) for l in self.layouts]
+            parameters["layouts"] = [vars(layout) for layout in self.layouts]
         if self.technologies:
             parameters["technologies"] = self.technologies.technologies_parameters()
         return parameters
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/protocols.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/trace.py` & `ipfabric_diagrams-6.2.1/ipfabric/diagrams/output_models/trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         PatchHeader,
         DropPacket,
         SeverityEvent,
         SecurityCheckIgnored,
         SecurityCheck,
         DestinationNAT,
         PolicyBasedRouting,
-        SourceNAT
+        SourceNAT,
     ],
     Field(discriminator="type"),
 ]
 
 
 class Trace(BaseModel):
     chain: str
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/__init__.py` & `ipfabric_diagrams-6.2.1/ipfabric_diagrams/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,37 @@
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
 import logging
 
-from ipfabric.diagrams import *
+from ipfabric.diagrams import (
+    IPFDiagram,
+    Unicast,
+    Multicast,
+    Host2GW,
+    Network,
+    OtherOptions,
+    Algorithm,
+    EntryPoint,
+    Layout,
+    NetworkSettings,
+    PathLookupSettings,
+    Overlay,
+    VALID_NET_PROTOCOLS,
+    VALID_PATH_PROTOCOLS,
+)
 
 logger = logging.getLogger("ipfabric_diagrams")
 
-logger.warning("ipfabric_diagrams will be merged into ipfabric in v7.0.0 with backwards compatability until then.\n"
-               "Please update imports from `ipfabric_diagrams` to `ipfabric.diagrams`")
+logger.warning(
+    "ipfabric_diagrams will be merged into ipfabric in v7.0.0 with backwards compatability until then.\n"
+    "Please update imports from `ipfabric_diagrams` to `ipfabric.diagrams`"
+)
 
 __all__ = [
     "IPFDiagram",
     "Unicast",
     "Multicast",
     "Host2GW",
     "Network",
```

### Comparing `ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/icmp.py` & `ipfabric_diagrams-6.2.1/ipfabric_diagrams/icmp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,62 @@
 """
 For backwards compatability until ipfabric_diagrams is merged into ipfabric in v7.0.0
 """
 
-from ipfabric.diagrams.icmp import *
+from ipfabric.diagrams.icmp import (
+    ICMP,
+    ECHO_REPLY,
+    NET_UNREACHABLE,
+    HOST_UNREACHABLE,
+    PROTOCOL_UNREACHABLE,
+    PORT_UNREACHABLE,
+    FRAGMENTATION_NEEDED,
+    SOURCE_ROUTE_FAILED,
+    DESTINATION_NETWORK_UNKNOWN,
+    DESTINATION_HOST_UNKNOWN,
+    SOURCE_HOST_ISOLATED,
+    DESTINATION_NETWORK_ADMIN_PROHIBITED,
+    DESTINATION_HOST_ADMIN_PROHIBITED,
+    DESTINATION_NETWORK_UNREACHABLE_FOR_TOS,
+    DESTINATION_HOST_UNREACHABLE_FOR_TOS,
+    COMMUNICATION_ADMINISTRATIVELY_PROHIBITED,
+    HOST_PRECEDENCE_VIOLATION,
+    PRECEDENCE_CUTOFF_IN_EFFECT,
+    SOURCE_QUENCH,
+    REDIRECT_DATAGRAM_FOR_THE_NETWORK,
+    REDIRECT_DATAGRAM_FOR_THE_HOST,
+    REDIRECT_DATAGRAM_FOR_THE_TOS_AND_NETWORK,
+    REDIRECT_DATAGRAM_FOR_THE_TOS_AND_HOST,
+    ALTERNATE_ADDRESS_FOR_HOST,
+    ECHO_REQUEST,
+    NORMAL_ROUTER_ADVERTISEMENT,
+    DOES_NOT_ROUTE_COMMON_TRAFFIC,
+    ROUTER_SOLICITATION,
+    TIME_TO_LIVE_EXCEEDED_IN_TRANSIT,
+    FRAGMENT_REASSEMBLY_TIME_EXCEEDED,
+    POINTER_INDICATES_THE_ERROR,
+    MISSING_A_REQUIRED_OPTION,
+    BAD_LENGTH,
+    TIMESTAMP_REQUEST,
+    TIMESTAMP_REPLY,
+    INFORMATION_REQUEST,
+    INFORMATION_REPLY,
+    MASK_REQUEST,
+    MASK_REPLY,
+    BAD_SPI,
+    AUTHENTICATION_FAILED,
+    DECOMPRESSION_FAILED,
+    DECRYPTION_FAILED,
+    NEED_AUTHENTICATION,
+    NEED_AUTHORIZATION,
+)
+
 
 __all__ = [
+    "ICMP",
     "ECHO_REPLY",
     "NET_UNREACHABLE",
     "HOST_UNREACHABLE",
     "PROTOCOL_UNREACHABLE",
     "PORT_UNREACHABLE",
     "FRAGMENTATION_NEEDED",
     "SOURCE_ROUTE_FAILED",
```

### Comparing `ipfabric_diagrams-6.2.0b1/LICENSE` & `ipfabric_diagrams-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/pyproject.toml` & `ipfabric_diagrams-6.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric-diagrams"
-version = "v6.2.0b1"
+version = "v6.2.1"
 description = "Python package for interacting with IP Fabric Diagrams"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-ipfabric = "~6.2.0b0"
+ipfabric = "~6.2.2"
 typing-extensions = "^4.5"
 rich = {version = "^13.3.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
```

### Comparing `ipfabric_diagrams-6.2.0b1/README.md` & `ipfabric_diagrams-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b1/setup.py` & `ipfabric_diagrams-6.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
  'ipfabric.diagrams.output_models',
  'ipfabric_diagrams']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ipfabric>=6.2.0b0,<6.3.0', 'typing-extensions>=4.5,<5.0']
+['ipfabric>=6.2.2,<6.3.0', 'typing-extensions>=4.5,<5.0']
 
 extras_require = \
 {'examples': ['rich>=13.3.0,<14.0.0']}
 
 setup_kwargs = {
     'name': 'ipfabric-diagrams',
-    'version': '6.2.0b1',
+    'version': '6.2.1',
     'description': 'Python package for interacting with IP Fabric Diagrams',
     'long_description': "# IP Fabric\n\nipfabric_diagrams is a Python module for connecting to and graphing topologies against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation.\n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth='TOKEN')`\n  - User/Pass: `IPFClient(auth=('USER', 'PASS'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API's are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK's match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric-diagrams\n```\n\n## Introduction\n\nThis package is used for diagramming via the API for IP Fabric v4.3.0.  \nExamples can be located under [examples](examples/) directory.\n\n## Authentication\nPlease take a look at [python-ipfabric](https://gitlab.com/ip-fabric/integrations/python-ipfabric#authentication) \nfor all authentication options.\n\n```python\nfrom ipfabric.diagrams import IPFDiagram\nipf = IPFDiagram(base_url='https://demo3.ipfabric.io/', auth='token', verify=False, timeout=15)\n```\n\n## Development\n\nIPFabric uses poetry for the python packaging module. Install poetry globally:\n\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo test and build:\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric_diagrams ipfabric\npoetry update\n```\n",
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams',
```

### Comparing `ipfabric_diagrams-6.2.0b1/PKG-INFO` & `ipfabric_diagrams-6.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ipfabric-diagrams
-Version: 6.2.0b1
+Version: 6.2.1
 Summary: Python package for interacting with IP Fabric Diagrams
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
-Requires-Dist: ipfabric (>=6.2.0b0,<6.3.0)
+Requires-Dist: ipfabric (>=6.2.2,<6.3.0)
 Requires-Dist: rich (>=13.3.0,<14.0.0) ; extra == "examples"
 Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 Description-Content-Type: text/markdown
```

