# Comparing `tmp/vpnkillswitch-0.1.8.tar.gz` & `tmp/vpnkillswitch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpnkillswitch-0.1.8.tar", last modified: Thu Jan 19 11:31:08 2023, max compression
+gzip compressed data, was "vpnkillswitch-0.1.9.tar", last modified: Mon Feb 13 12:03:47 2023, max compression
```

## Comparing `vpnkillswitch-0.1.8.tar` & `vpnkillswitch-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-19 11:31:08.469263 vpnkillswitch-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1066 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.8/LICENCE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-01-19 11:31:08.469263 vpnkillswitch-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      802 2023-01-19 11:16:33.000000 vpnkillswitch-0.1.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-01-19 11:31:08.469263 vpnkillswitch-0.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-19 11:31:08.461263 vpnkillswitch-0.1.8/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-19 11:31:08.465263 vpnkillswitch-0.1.8/src/vpnkillswitch/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.8/src/vpnkillswitch/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30084 2023-01-19 11:07:32.000000 vpnkillswitch-0.1.8/src/vpnkillswitch/systemipswitches.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-01-18 15:41:38.000000 vpnkillswitch-0.1.8/src/vpnkillswitch/vpnkillswitch.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-19 11:31:08.465263 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-01-19 11:31:08.000000 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2023-01-19 11:31:08.000000 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-01-19 11:31:08.000000 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-01-19 11:31:08.000000 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-01-19 11:31:08.000000 vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-13 12:03:47.187646 vpnkillswitch-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1066 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.9/LICENCE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-13 12:03:47.187646 vpnkillswitch-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      802 2023-02-13 11:59:14.000000 vpnkillswitch-0.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-02-13 12:03:47.187646 vpnkillswitch-0.1.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-13 12:03:47.183646 vpnkillswitch-0.1.9/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-13 12:03:47.187646 vpnkillswitch-0.1.9/src/vpnkillswitch/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-18 14:14:39.000000 vpnkillswitch-0.1.9/src/vpnkillswitch/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30403 2023-02-10 10:53:05.000000 vpnkillswitch-0.1.9/src/vpnkillswitch/systemipswitches.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2023-02-10 10:08:49.000000 vpnkillswitch-0.1.9/src/vpnkillswitch/vpnkillswitch.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-13 12:03:47.187646 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-13 12:03:47.000000 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2023-02-13 12:03:47.000000 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-02-13 12:03:47.000000 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-02-13 12:03:47.000000 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-13 12:03:47.000000 vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/top_level.txt
```

### Comparing `vpnkillswitch-0.1.8/LICENCE` & `vpnkillswitch-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `vpnkillswitch-0.1.8/PKG-INFO` & `vpnkillswitch-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vpnkillswitch
-Version: 0.1.8
+Version: 0.1.9
 Summary: A vpnkillswitch helper from rexbytes.com
 Author-email: Good Boy <pythonic@rexbytes.com>
 Project-URL: Homepage, https://github.com/RexBytes/vpnkillswitch
 Project-URL: Bug Tracker, https://github.com/RexBytes/vpnkillswitch/issues
-Project-URL: Download URL, https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.8.tar.gz
+Project-URL: Download URL, https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.9.tar.gz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `vpnkillswitch-0.1.8/pyproject.toml` & `vpnkillswitch-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vpnkillswitch"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Good Boy", email="pythonic@rexbytes.com" },
 ]
 description = "A vpnkillswitch helper from rexbytes.com"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -18,12 +18,12 @@
     "Operating System :: POSIX :: Linux",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/RexBytes/vpnkillswitch"
 "Bug Tracker" = "https://github.com/RexBytes/vpnkillswitch/issues"
-"Download URL" ="https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.8.tar.gz"
+"Download URL" ="https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.9.tar.gz"
 
 [project.scripts]
 vpnkillswitch = "vpnkillswitch:vpnkillswitch.vpnkillswitch"
```

### Comparing `vpnkillswitch-0.1.8/src/vpnkillswitch/systemipswitches.py` & `vpnkillswitch-0.1.9/src/vpnkillswitch/systemipswitches.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 class SystemIPSwitches:
     def __init__(self):
         self.systembash = SystemBash()
         self.systemctl = SystemCTL()
         self.systemd = SystemD()
 
-    def switch_on(self, granular: bool = False, netclass: str = "C"):
+    def switch_on(self, granular: bool = False, netclass: str = "C", interface: str = "tun+"):
         self.switch_flush()
-        self.switch_vpn(granular=granular, netclass=netclass)
-        self.switch_docker(granular)
+        self.switch_vpn(granular=granular, netclass=netclass, interface=interface)
+        self.switch_docker(granular=granular, interface=interface)
 
     def switch_off(self):
         try:
             self.systemctl.protect_ctl_disable()
         except Exception as e:
             print(e)
 
@@ -67,21 +67,21 @@
         self.systembash.run_off()
 
     def switch_protect(self):
         self.systemd.protect()
         self.systembash.run_protect()
         self.systemctl.protect_ctl_enable()
 
-    def switch_vpn(self, granular: bool = False, netclass: str = "C"):
-        self.systemd.openvpn(granular=granular, netclass=netclass)
+    def switch_vpn(self, granular: bool = False, netclass: str = "C", interface: str = 'tun+'):
+        self.systemd.openvpn(granular=granular, netclass=netclass, interface=interface)
         self.systembash.run_vpn4()
         self.systemctl.openvpn_ctl_enable()
 
-    def switch_docker(self, granular: bool = False):
-        self.systemd.docker(granular)
+    def switch_docker(self, granular: bool = False, interface: str = "tun+"):
+        self.systemd.docker(granular,interface)
         self.systembash.run_docker()
         self.systemctl.docker_ctl_enable()
 
     def switch_flush(self):
         self.switch_off()
         self.systemd.flush()
         self.systembash.run_flush()
@@ -232,41 +232,41 @@
     def synergy_off(self):
         (
             synergy_off_bash_filepath,
             synergy_off_bashtext,
         ) = self.service_bash_text.synergy_off_text()
         self.systemdfiles.writebash(synergy_off_bash_filepath, synergy_off_bashtext)
 
-    def openvpn(self, granular: bool = False, netclass: str = "C"):
+    def openvpn(self, granular: bool = False, netclass: str = "C", interface: str = 'tun+'):
         vpn_service_filepath, vpn_servicetext = self.service_unit_text.openvpn()
         if granular:
             (
                 vpn_bash_filepath,
                 vpn_bashtext,
             ) = self.service_bash_text.vpnkillswitch_g_text(netclass=netclass)
         else:
             (
                 vpn_bash_filepath,
                 vpn_bashtext,
-            ) = self.service_bash_text.vpnkillswitch_text(netclass=netclass)
+            ) = self.service_bash_text.vpnkillswitch_text(netclass=netclass, interface=interface)
         self.systemdfiles.writebash(vpn_bash_filepath, vpn_bashtext)
         self.systemdfiles.writeservice(vpn_service_filepath, vpn_servicetext)
 
-    def docker(self, granular: bool = False):
+    def docker(self, granular: bool = False, interface: str = 'tun+'):
         docker_service_filepath, docker_servicetext = self.service_unit_text.docker()
         if granular:
             (
                 docker_bash_filepath,
                 docker_bashtext,
             ) = self.service_bash_text.dockerkillswitch_g_text()
         else:
             (
                 docker_bash_filepath,
                 docker_bashtext,
-            ) = self.service_bash_text.dockerkillswitch_text()
+            ) = self.service_bash_text.dockerkillswitch_text(interface=interface)
         self.systemdfiles.writebash(docker_bash_filepath, docker_bashtext)
         self.systemdfiles.writeservice(docker_service_filepath, docker_servicetext)
 
     def erase_all(self):
         self.systemdfiles.erase_all()
 
 
@@ -648,15 +648,15 @@
 ip6tables --policy INPUT DROP
 ip6tables --policy FORWARD DROP
 ip6tables --policy OUTPUT DROP
 sysctl_file_disable_ipv6
 """
         return self.systemdfilepaths.protect_bash, text
 
-    def vpnkillswitch_text(self, netclass: str = "C"):
+    def vpnkillswitch_text(self, netclass: str = "C", interface: str = 'tun+'):
         if netclass == "C":
             netclassip = "192.168.0.0/16"
         if netclass == "B":
             netclassip = "172.16.0.0/12"
         if netclass == "A":
             netclassip = "10.0.0.0/8"
         text = f"""#!/bin/bash
@@ -672,15 +672,15 @@
 create_filter_chain 'RB_I_RELATED_AND_ESTABLISHED'
 create_filter_rule 'iptables -A RB_I_RELATED_AND_ESTABLISHED -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT'
 create_filter_rule 'iptables -A RB_I_RELATED_AND_ESTABLISHED  -i lo -j ACCEPT '
 create_filter_rule 'iptables -I INPUT  -j RB_I_RELATED_AND_ESTABLISHED'
 #let's create a chain named RB_OUTPUT_VPN_KILL_SWITCH to hold our VPN rules
 create_filter_chain 'RB_OUTPUT_VPN_KILL_SWITCH'
 create_filter_rule 'iptables -A RB_OUTPUT_VPN_KILL_SWITCH -p udp -m udp --dport 1194 -j ACCEPT'
-create_filter_rule 'iptables -A RB_OUTPUT_VPN_KILL_SWITCH -o tun+ -j ACCEPT'
+create_filter_rule 'iptables -A RB_OUTPUT_VPN_KILL_SWITCH -o {interface} -j ACCEPT'
 create_filter_rule 'iptables -A RB_OUTPUT_VPN_KILL_SWITCH -o lo -j ACCEPT'
 #If you want to, you can also allow access to your local network.
 #The most common local network is class C, 192.168.0.0/16
 create_filter_rule 'iptables -A RB_OUTPUT_VPN_KILL_SWITCH -d {netclassip} -j ACCEPT'
 #You must check what local network class you car connected to.
 #Adjust for Class C, 192.168.0.0/16 Class B, 172.16.0.0/12 and class A 10.0.0.0/8
 #The following line is to allow a single ip address for your DNS server, 
@@ -749,21 +749,21 @@
 ip6tables --policy INPUT DROP
 ip6tables --policy FORWARD DROP
 ip6tables --policy OUTPUT DROP
 sysctl_file_disable_ipv6
 """
         return self.systemdfilepaths.vpn4_bash, text
 
-    def dockerkillswitch_text(self):
+    def dockerkillswitch_text(self,  interface: str = 'tun+'):
         text = f"""#!/bin/bash
 {self.bashfunctions}
 {self.procfunctions}
 create_filter_chain 'RB_DOCKER_VPN_KILL_SWITCH'
-create_filter_rule 'iptables -A RB_DOCKER_VPN_KILL_SWITCH -o tun+ -j ACCEPT'
-create_filter_rule 'iptables -A RB_DOCKER_VPN_KILL_SWITCH -i tun+ -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT'
+create_filter_rule 'iptables -A RB_DOCKER_VPN_KILL_SWITCH -o {interface} -j ACCEPT'
+create_filter_rule 'iptables -A RB_DOCKER_VPN_KILL_SWITCH -i {interface} -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT'
 create_filter_rule 'iptables -A RB_DOCKER_VPN_KILL_SWITCH -j DROP'
 create_filter_rule 'iptables -I DOCKER-USER  -j RB_DOCKER_VPN_KILL_SWITCH'
 ip6tables --policy INPUT DROP
 ip6tables --policy FORWARD DROP
 ip6tables --policy OUTPUT DROP
 sysctl_file_disable_ipv6
 """
```

### Comparing `vpnkillswitch-0.1.8/src/vpnkillswitch/vpnkillswitch.py` & `vpnkillswitch-0.1.9/src/vpnkillswitch/vpnkillswitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,21 @@
     )
     granularity_group.add_argument(
         "-g",
         "--granular",
         action="store_true",
         help="Creates a more granular iptables ruleset",
     )
+    granularity_group.add_argument(
+        "-i",
+        "--vint",
+        default="tun+",
+        choices=['tun+','proton+','proton0'],
+        help="Choose the name of your virtual interface",
+    )
     netclass_group = main_group_parser.add_argument_group(
         "netclass",
         "What ip class are you connected to A 10.0.0.0/8,B 172.16.0.0/12 or C  192.168.0.0/16 ?",
     )
     netclass_group.add_argument(
         "-n",
         "--netclass",
@@ -71,16 +78,16 @@
     )
 
     my_args = main_group_parser.parse_args()
 
     ipswitches = SystemIPSwitches()
 
     if my_args.on:
-        print(f"my_args.on:{my_args.on}, granularity:{my_args.granular}")
-        ipswitches.switch_on(granular=my_args.granular, netclass=my_args.netclass)
+        print(f"my_args.on:{my_args.on}, granularity:{my_args.granular}, interface:{my_args.vint}")
+        ipswitches.switch_on(granular=my_args.granular, netclass=my_args.netclass,interface=my_args.vint)
 
     if my_args.off:
         print(f"my_args.off:{my_args.off}")
         ipswitches.switch_off()
 
     if my_args.protect:
         print(f"my_args.protect:{my_args.protect}")
```

### Comparing `vpnkillswitch-0.1.8/src/vpnkillswitch.egg-info/PKG-INFO` & `vpnkillswitch-0.1.9/src/vpnkillswitch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vpnkillswitch
-Version: 0.1.8
+Version: 0.1.9
 Summary: A vpnkillswitch helper from rexbytes.com
 Author-email: Good Boy <pythonic@rexbytes.com>
 Project-URL: Homepage, https://github.com/RexBytes/vpnkillswitch
 Project-URL: Bug Tracker, https://github.com/RexBytes/vpnkillswitch/issues
-Project-URL: Download URL, https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.8.tar.gz
+Project-URL: Download URL, https://github.com/RexBytes/vpnkillswitch/archive/refs/tags/v0.1.9.tar.gz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

