# Comparing `tmp/getRoutersConfig-0.0.3.tar.gz` & `tmp/getRoutersConfig-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getRoutersConfig-0.0.3.tar", last modified: Mon Apr 24 18:58:02 2023, max compression
+gzip compressed data, was "getRoutersConfig-0.0.4.tar", last modified: Wed May  3 09:44:45 2023, max compression
```

## Comparing `getRoutersConfig-0.0.3.tar` & `getRoutersConfig-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:58:02.825940 getRoutersConfig-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-04-22 13:23:07.000000 getRoutersConfig-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4156 2023-04-24 18:58:02.825940 getRoutersConfig-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-04-24 17:58:07.000000 getRoutersConfig-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:58:02.809881 getRoutersConfig-0.0.3/app/
-drwxrwxrwx   0        0        0        0 2023-04-24 18:58:02.813973 getRoutersConfig-0.0.3/app/getRoutersConfig/
--rw-rw-rw-   0        0        0       48 2023-04-22 20:51:53.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:58:02.824940 getRoutersConfig-0.0.3/app/getRoutersConfig/src/
--rw-rw-rw-   0        0        0     9535 2023-04-24 18:18:52.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/src/CiscoClass.py
--rw-rw-rw-   0        0        0     4106 2023-04-20 14:25:04.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/src/HuaweiClass.py
--rw-rw-rw-   0        0        0     1028 2023-04-24 17:47:13.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/src/RouterClass.py
--rw-rw-rw-   0        0        0        0 2023-04-22 18:35:47.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/src/__init__.py
--rw-rw-rw-   0        0        0     2307 2023-04-23 13:29:05.000000 getRoutersConfig-0.0.3/app/getRoutersConfig/src/main.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:58:02.818363 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/
--rw-rw-rw-   0        0        0     4156 2023-04-24 18:58:02.000000 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-04-24 18:58:02.000000 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:58:02.000000 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-24 18:58:02.000000 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 18:58:02.000000 getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 18:58:02.826943 getRoutersConfig-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-04-24 18:55:22.000000 getRoutersConfig-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.072579 getRoutersConfig-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4464 2023-05-03 09:44:45.068573 getRoutersConfig-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:44.969003 getRoutersConfig-0.0.4/app/
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:44.995573 getRoutersConfig-0.0.4/app/getRoutersConfig/
+-rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.056582 getRoutersConfig-0.0.4/app/getRoutersConfig/src/
+-rw-rw-rw-   0        0        0     9798 2023-05-02 15:33:04.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/CiscoClass.py
+-rw-rw-rw-   0        0        0     4106 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/HuaweiClass.py
+-rw-rw-rw-   0        0        0     1096 2023-05-02 15:35:16.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/RouterClass.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-03 09:35:35.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.037577 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/
+-rw-rw-rw-   0        0        0     4464 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:44:45.073576 getRoutersConfig-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-02 15:36:10.000000 getRoutersConfig-0.0.4/setup.py
```

### Comparing `getRoutersConfig-0.0.3/LICENSE` & `getRoutersConfig-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.3/PKG-INFO` & `getRoutersConfig-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.3
+Version: 0.0.4
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netmiko.svg)](https://img.shields.io/pypi/pyversions/netmiko)
 
 # What it does ?
@@ -46,14 +46,23 @@
         "weeks": 0,
         "days": 2,
         "hours": 2,
         "minutes": 44
 }
 ```
 
+# Disconnect from router
+```python
+from getRoutersConfig import setInformations
+
+router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
+
+system_information = router.disconnect()
+```
+
 # Get static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 static_routes = router.getStaticRoutes()
```

### Comparing `getRoutersConfig-0.0.3/app/getRoutersConfig/src/CiscoClass.py` & `getRoutersConfig-0.0.4/app/getRoutersConfig/src/CiscoClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ipaddress import IPv4Network
 import re
 
 class Cisco:
     def __init__(self, net_connect):
         self.net_connect = net_connect
 
-    def getipv4StaticRoutes(self) -> list:
+    def getIpv4StaticRoutes(self) -> list:
         output = self.net_connect.send_command(f"show running-config | i ip route")
 
         v4_routes = []
         new_v4_routes = self.separate_section(r"(^.*ip route.*$)", output)
 
         for route in new_v4_routes:
             re_route = r'ip route( vrf (?P<vrf>\S+))? (?P<subnet_address>\d+.\d+.\d+.\d+) (?P<subnet_mask>\d+.\d+.\d+.\d+) (?P<gateway>\d+.\d+.\d+.\d+)( (?P<metric>\d+))?( tag (?P<tag>\d+))?( name (?P<name>(\S|\s)+))?' #(?!.*\btrack\b)
@@ -158,17 +158,17 @@
         res_dhcp = []
         options = []
 
         new_dhcp = self.separate_section(r"(^ip dhcp pool.*$)", output_v4)
 
         for dhcp in new_dhcp:
             re_dhcp_pool_name = r"^ip dhcp pool (?P<dhcp_pool_name>.+)$"
-            re_network = r"network (?P<network_address>\d+.\d+.\d+.\d+) (?P<network_mask>\d+.\d+.\d+.\d+)"
-            re_default_router = r"default-router (?P<default_router>\d+.\d+.\d+.\d+)"
-            re_dns_server = r"dns-server (?P<dns_server>.+)"
+            re_network = r"(network (?P<network_address>\d+.\d+.\d+.\d+) (?P<network_mask>\d+.\d+.\d+.\d+))?"
+            re_default_router = r"(default-router (?P<default_router>\d+.\d+.\d+.\d+))?"
+            re_dns_server = r"(dns-server (?P<dns_server>.+))?"
             re_options = r"option (?P<code>\d+) (?P<string_type>\S+) (?P<string>\S+)"
 
             match_dhcp_pool_name = re.search(re_dhcp_pool_name, dhcp, flags=re.M)
             match_network = re.search(re_network, dhcp, flags=re.M)
             match_default_router = re.search(re_default_router, dhcp, flags=re.M)
             match_dns_server = re.search(re_dns_server, dhcp, flags=re.M)
             match_options = re.findall(re_options, dhcp, flags=re.M)
@@ -180,19 +180,19 @@
                         "string_type": option[1],
                         "string": str(option[2]).replace('"', '')
                     })
 
             res_dhcp.append({
                 "name": match_dhcp_pool_name.group('dhcp_pool_name'),
                 "network": {
-                    "subnet_address": match_network.group('network_address'),
+                    "subnet_address": match_network.group('network_address') if match_network.group('network_address') else "",
                     "mask": {
-                        "octets": match_network.group('network_address'),
-                        "cidr": IPv4Network((0, match_network.group('network_mask'))).prefixlen,
+                        "octets": match_network.group('network_address') if match_network.group('network_address') else "",
+                        "cidr": IPv4Network((0, match_network.group('network_mask'))).prefixlen if match_network.group('network_address') else "",
                     }
                 },
-                "default_router": match_default_router.group('default_router'),
-                "dns_server": [i for i in match_dns_server.group('dns_server').strip().split(' ')],
+                "default_router": match_default_router.group('default_router') if match_default_router.group('default_router') else "",
+                "dns_server": [i for i in match_dns_server.group('dns_server').strip().split(' ')] if match_dns_server.group('dns_server') else "",
                 "option": options
             })
 
         return res_dhcp
```

### Comparing `getRoutersConfig-0.0.3/app/getRoutersConfig/src/HuaweiClass.py` & `getRoutersConfig-0.0.4/app/getRoutersConfig/src/HuaweiClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.3/app/getRoutersConfig/src/RouterClass.py` & `getRoutersConfig-0.0.4/app/getRoutersConfig/src/RouterClass.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,27 @@
         self.router_type = router_type
         self.net_connect = net_connect
         if self.router_type == "huawei":
             self.router = Huawei(self.net_connect)
         elif self.router_type == "cisco_ios":
             self.router = Cisco(self.net_connect)
 
+    def disconnect(self):
+        self.net_connect.disconnect()
+
     def getFullConfiguration(self):
         return {
             "system": self.router.getSystemInformation(),
-            "ipv4StaticRoutes": self.router.getipv4StaticRoutes(),
+            "ipv4StaticRoutes": self.router.getIpv4StaticRoutes(),
             "interfaces": self.router.getInterfaces(),
             "dhcp": self.router.getDhcp()
         }
 
-    def getipv4StaticRoutes(self):
-        return self.router.getipv4StaticRoutes()
+    def getIpv4StaticRoutes(self):
+        return self.router.getIpv4StaticRoutes()
     
     def getSystemInformation(self):
         return self.router.getSystemInformation()
     
     def getInterfaces(self):
         return self.router.getInterfaces()
```

### Comparing `getRoutersConfig-0.0.3/app/getRoutersConfig/src/main.py` & `getRoutersConfig-0.0.4/app/getRoutersConfig/src/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from netmiko import ConnectHandler, redispatch
 import time
 from .RouterClass import Router
 from pysnmp.hlapi import *
 
-def setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='') -> Router:
+def setInformations(host_ip: str='', host_port: int=22, host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: int=22) -> Router:
     if not bastion_ip:
         device_type: str = getDeviceType(host_ip, host_snmp_community)
 
     host = {
         'device_type': device_type if not bastion_ip else "terminal_server",
         'ip': host_ip if not bastion_ip else bastion_ip,
         'username': user,
         'password': password,
         'port': host_port if not bastion_ip else bastion_port,
+        # 'session_log': 'output.log'
     }
 
     net_connect = ConnectHandler(**host)
 
+    time.sleep(3)
+
     if bastion_ip:
-        output = net_connect.write_channel(f"snmpwalk -v2c -c covareck {host_ip} SNMPv2-MIB::sysDescr\n")
 
+        net_connect.write_channel(f"snmpwalk -v2c -c covareck {host_ip} SNMPv2-MIB::sysDescr\n")
+        net_connect.write_channel(f"ssh {host_ip}\r\n")
+
+        time.sleep(2)
+        output = net_connect.read_channel()
+        print(output)
         if "huawei" in output.lower():
             device_type: str = "huawei"
         elif "cisco" in output.lower():
             device_type: str = "cisco_ios"
 
-        net_connect.write_channel(f"ssh {host_ip}\r\n")
-
         time.sleep(2)
 
-        output = net_connect.read_channel()
-
         if 'password' in output.lower():
             net_connect.write_channel(password)
 
         redispatch(net_connect, device_type=device_type)
 
     return Router(device_type, net_connect)
```

### Comparing `getRoutersConfig-0.0.3/app/getRoutersConfig.egg-info/PKG-INFO` & `getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.3
+Version: 0.0.4
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netmiko.svg)](https://img.shields.io/pypi/pyversions/netmiko)
 
 # What it does ?
@@ -46,14 +46,23 @@
         "weeks": 0,
         "days": 2,
         "hours": 2,
         "minutes": 44
 }
 ```
 
+# Disconnect from router
+```python
+from getRoutersConfig import setInformations
+
+router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
+
+system_information = router.disconnect()
+```
+
 # Get static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 static_routes = router.getStaticRoutes()
```

### Comparing `getRoutersConfig-0.0.3/setup.py` & `getRoutersConfig-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="getRoutersConfig",
-    version="0.0.3",
+    version="0.0.4",
     description="get Cisco routers configuration as Json",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanielRicklin/getRoutersConfig",
     author="DanielRicklin",
     author_email="ricklin.daniel@outlook.fr",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=["netmiko >= 4.1.2"],
+    install_requires=["netmiko >= 4.1.2","pysnmp>=4.4.12"],
     extras_require={
         "dev": ["twine >= 4.0.2"],
     },
-    python_requires=">=3.10",
+    python_requires=">=3.7",
 )
 
 #python setup.py bdist_wheel sdist
 #python -m twine check dist/*
 #python -m twine upload dist/*
 
 #Test the code
 #pip install .
-#python main.py
+#python main.py
```

