# Comparing `tmp/heist-salt-5.3.1.tar.gz` & `tmp/heist-salt-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heist-salt-5.3.1.tar", last modified: Wed Jul 13 16:14:01 2022, max compression
+gzip compressed data, was "heist-salt-6.0.0.tar", last modified: Wed May  3 19:49:26 2023, max compression
```

## Comparing `heist-salt-5.3.1.tar` & `heist-salt-6.0.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.495819 heist-salt-5.3.1/
--rw-r--r--   0 root         (0) root         (0)    11342 2022-07-13 16:13:48.000000 heist-salt-5.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-13 16:14:01.495819 heist-salt-5.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4757 2022-07-13 16:13:48.000000 heist-salt-5.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.487820 heist-salt-5.3.1/heist_salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/artifact/
--rw-r--r--   0 root         (0) root         (0)     8730 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/artifact/salt.py
--rw-r--r--   0 root         (0) root         (0)     1708 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.487820 heist-salt-5.3.1/heist_salt/heist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/heist/salt/
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/heist/salt/init.py
--rw-r--r--   0 root         (0) root         (0)     9565 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/heist/salt/minion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/salt/call/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/salt/call/contracts/
--rw-r--r--   0 root         (0) root         (0)      280 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/call/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/call/init.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/salt/key/
--rw-r--r--   0 root         (0) root         (0)      108 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/key/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt/salt/key/contracts/
--rw-r--r--   0 root         (0) root         (0)      134 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/key/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     5401 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/key/init.py
--rw-r--r--   0 root         (0) root         (0)     2125 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/key/local_master.py
--rw-r--r--   0 root         (0) root         (0)      108 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/salt/key/raas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.495819 heist-salt-5.3.1/heist_salt/service/
--rw-r--r--   0 root         (0) root         (0)       67 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/service/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.495819 heist-salt-5.3.1/heist_salt/service/salt/
--rw-r--r--   0 root         (0) root         (0)     4560 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/service/salt/minion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.495819 heist-salt-5.3.1/heist_salt/tool/
--rw-r--r--   0 root         (0) root         (0)      764 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/tool/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/tool/config.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/tool/init.py
--rw-r--r--   0 root         (0) root         (0)      310 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/tool/service.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-07-13 16:13:48.000000 heist-salt-5.3.1/heist_salt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 16:14:01.491820 heist-salt-5.3.1/heist_salt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-13 16:14:01.000000 heist-salt-5.3.1/heist_salt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2022-07-13 16:14:01.000000 heist-salt-5.3.1/heist_salt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 16:14:01.000000 heist-salt-5.3.1/heist_salt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2022-07-13 16:14:01.000000 heist-salt-5.3.1/heist_salt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-13 16:14:01.000000 heist-salt-5.3.1/heist_salt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      921 2022-07-13 16:13:48.000000 heist-salt-5.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-13 16:14:01.495819 heist-salt-5.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2005 2022-07-13 16:13:48.000000 heist-salt-5.3.1/setup.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    11342 2023-05-02 20:35:58.000000 heist-salt-6.0.0/LICENSE
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2417 2023-05-03 19:49:26.553431 heist-salt-6.0.0/PKG-INFO
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1856 2023-05-03 18:58:51.000000 heist-salt-6.0.0/README.rst
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/artifact/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    20587 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/artifact/salt.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1848 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/conf.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.546764 heist-salt-6.0.0/heist_salt/heist/
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/heist/salt/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)    17322 2023-05-03 15:04:25.000000 heist-salt-6.0.0/heist_salt/heist/salt/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     4684 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/master.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5991 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/minion.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5729 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/heist/salt/proxy.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/call/
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt/salt/call/contracts/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      280 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/call/contracts/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1851 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/call/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/init.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/key/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      108 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/api.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/key/contracts/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      134 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/contracts/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     6344 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2125 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/local_master.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      108 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/key/raas.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/salt/pillar/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1598 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/salt/pillar/init.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/service/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      186 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/service/init.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/service/salt/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     5702 2023-05-03 17:04:40.000000 heist-salt-6.0.0/heist_salt/service/salt/init.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.553431 heist-salt-6.0.0/heist_salt/tool/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      974 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/artifacts.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1607 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/config.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/init.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     1081 2023-05-02 20:35:58.000000 heist-salt-6.0.0/heist_salt/tool/service.py
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       18 2023-05-03 17:06:32.000000 heist-salt-6.0.0/heist_salt/version.py
+drwxr-xr-x   0 ch3ll     (1000) ch3ll     (1000)        0 2023-05-03 19:49:26.550098 heist-salt-6.0.0/heist_salt.egg-info/
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2417 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/PKG-INFO
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      850 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)        1 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       50 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/requires.txt
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       11 2023-05-03 19:49:26.000000 heist-salt-6.0.0/heist_salt.egg-info/top_level.txt
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)      921 2023-05-02 20:35:58.000000 heist-salt-6.0.0/pyproject.toml
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)       38 2023-05-03 19:49:26.553431 heist-salt-6.0.0/setup.cfg
+-rw-r--r--   0 ch3ll     (1000) ch3ll     (1000)     2095 2023-05-02 20:35:58.000000 heist-salt-6.0.0/setup.py
```

### Comparing `heist-salt-5.3.1/LICENSE` & `heist-salt-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heist-salt-5.3.1/heist_salt/conf.py` & `heist-salt-6.0.0/heist_salt/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CLI_CONFIG = {
     # The dyne will always be heist.
     # List the subcommands that will expose this option
-    "key_plugin": {"subcommands": ["salt.minion"], "dyne": "heist"},
-    "onedir": {"subcommands": ["salt.minion"], "dyne": "heist"},
+    "key_plugin": {"subcommands": ["salt.minion", "salt.master"], "dyne": "heist"},
+    "onedir": {"subcommands": ["salt.minion", "salt.master"], "dyne": "heist"},
 }
 CONFIG = {
     # This will show up in hub.OPT.heist.key_plugin
     "key_plugin": {
         "default": "local_master",
         "help": "Define the salt key plugin to use.",
         "dyne": "heist",
@@ -21,15 +21,15 @@
     "retry_key_count": {
         "default": 5,
         "help": "Amount of times to retry accepting the salt-key,"
         "while the salt minion is still starting up",
         "dyne": "heist",
     },
     "salt_repo_url": {
-        "default": "https://repo.saltproject.io/salt/",
+        "default": "https://repo.saltproject.io/salt/py3/",
         "help": "The url to a repo that contains the repo.json/repo.mp"
         "file and the Salt artifacts",
         "dyne": "heist",
     },
     "offline_mode": {
         "default": False,
         "help": "Do not query a repo for artifacts. Use the artifacts already in the artifact directory.",
@@ -41,15 +41,19 @@
         "type": bool,
         "action": "store_true",
         "help": "Use the onedir package of salt. If False, singlebin will be used.",
         "dyne": "heist",
     },
 }
 
-SUBCOMMANDS = {"salt.minion": {"help": "", "dyne": "heist"}}
+SUBCOMMANDS = {
+    "salt.minion": {"help": "", "dyne": "heist"},
+    "salt.master": {"help": "", "dyne": "heist"},
+    "salt.proxy": {"help": "", "dyne": "heist"},
+}
 DYNE = {
     "artifact": ["artifact"],
     "heist": ["heist"],
     "salt": ["salt"],
     "service": ["service"],
     "tool": ["tool"],
 }
```

### Comparing `heist-salt-5.3.1/heist_salt/salt/key/init.py` & `heist-salt-6.0.0/heist_salt/heist/salt/minion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,196 @@
-import asyncio
 import pathlib
+from typing import Dict
 
-import salt.config
+import asyncssh
 
 
-def accept_minion(hub, minion: str) -> bool:
-    return hub.salt.key[hub.OPT.heist.key_plugin].accept_minion(minion)
-
-
-def delete_minion(hub, minion: str) -> bool:
-    return hub.salt.key[hub.OPT.heist.key_plugin].delete_minion(minion)
+async def run(
+    hub,
+    remotes: Dict[str, Dict[str, str]],
+    artifact_version=None,
+    manage_service=None,
+    **kwargs,
+):
+    return await hub.heist.salt.init.run(
+        remotes,
+        artifact_version=artifact_version,
+        manage_service=manage_service,
+        **kwargs,
+    )
 
 
-async def check_pki_dir_empty(
-    hub, target_name, tunnel_plugin, key_dir, target_os="linux"
-):
+async def clean(hub, target_name, tunnel_plugin, service_plugin=None, vals=None):
     """
-    function to check if the pki directory is empty or not
+    Clean up the connections
     """
-    if target_os == "windows":
-        # Returns 0 exitcode if empty
-        check_dir = f"$items = Get-ChildItem -Path {key_dir}; exit $items.Count"
-        ret = await hub.tunnel[tunnel_plugin].cmd(target_name, check_dir)
-        if ret.returncode != 0:
-            hub.log.error(
-                "The minion pki directory is not empty. Not generating and accepting a key"
-            )
-            return False
-    else:
-        # Returns 0 exitcode if NOT empty
-        check_dir = f'[ "$(ls -A {key_dir})" ]'
-        ret = await hub.tunnel[tunnel_plugin].cmd(target_name, check_dir)
-        if ret.returncode == 0:
-            hub.log.error(
-                "The minion pki directory is not empty. Not generating and accepting a key"
-            )
+    await hub.heist.salt.init.clean(
+        target_name,
+        tunnel_plugin,
+        service_plugin,
+        vals,
+    )
+    target_id = hub.heist.CONS[target_name].get("target_id")
+    if target_id:
+        if not hub.salt.key.init.delete_minion(target_id):
+            hub.log.error(f"Could not delete the key for minion: {target_id}")
             return False
     return True
 
 
-async def generate_keys(
-    hub,
-    target_name,
-    tunnel_plugin,
-    run_dir,
-    user=None,
-    minion_id=None,
-    target_os="linux",
-):
-    binary_path = str(hub.tool.artifacts.get_salt_path(run_dir, target_os=target_os))
-    if not hub.tool.path.clean_path(
-        hub.heist.init.default(target_os, "run_dir_root"), run_dir
-    ):
-        hub.log.error(f"The path {run_dir} is not valid")
-        return False
-    is_windows = target_os == "windows"
+def get_service_name(hub, service_plugin, target_os="linux", start=True):
+    """
+    Get the service name for the given service
 
-    if is_windows:
-        key_dir = run_dir / "root_dir" / "conf" / "pki" / "minion"
-    else:
-        key_dir = run_dir / "root_dir" / "etc" / "salt" / "pki" / "minion"
+    :param service_plugin:
+        The service plugin being used to manage the service.
+    :param target_os:
+        The OS of the target.
+    :param start:
+        Return service name when starting the service.
+    """
+    return "salt-minion"
 
-    hub.log.debug(f"Create and secure pki dir and parent directores: {key_dir}")
-    if target_os == "windows":
-        # Owner (OW), System (SY), and Administrators (BA) have Full Control
-        sddl = "D:PAI(A;OICI;FA;;;OW)(A;OICI;FA;;;SY)(A;OICI;FA;;;BA)"
-        owner = r'[System.Security.Principal.NTAccount]"BUILTIN\Administrators"'
-        cmd = "; ".join(
-            [
-                f'New-Item -Path "{key_dir}" -Type Directory',
-                f'$acl = Get-Acl "{key_dir.parent}"',
-                f'$acl.SetSecurityDescriptorSddlForm("{sddl}")',
-                f"$acl.SetOwner({owner})",
-                f'Set-Acl -Path "{key_dir.parent}" -AclObject $acl',
-            ]
-        )
-    else:
-        # mkdir will not add the correct permissions to the parent directories
-        # unless each directory is specified
-        perms = 0o710 if hub.tunnel.asyncssh.CONS[target_name].get("sudo") else 0o700
-        cmd = f"mkdir -m{perms:o} -p {key_dir.parent.parent.parent} {key_dir.parent.parent} {key_dir.parent} {key_dir}"
 
-    await hub.tunnel[tunnel_plugin].cmd(target_name, cmd, target_os=target_os)
+async def tunnel_to_ports(hub, target_name, tunnel_plugin, salt_conf):
+    import salt.config
+    import salt.syspaths
 
-    if not is_windows and user:
-        await hub.tunnel[tunnel_plugin].cmd(
+    master_opts = salt.config.client_config(
+        pathlib.Path(salt.syspaths.CONFIG_DIR) / "master"
+    )
+    try:
+        await hub.tunnel[tunnel_plugin].tunnel(
             target_name,
-            f"chown -R {user}:{user} {key_dir.parent.parent.parent}",
+            salt_conf["publish_port"],
+            master_opts.get("publish_port", 4505),
         )
-
-    hub.log.debug("Making sure the PKI directory is empty")
-    if not await hub.salt.key.init.check_pki_dir_empty(
-        target_name, tunnel_plugin, key_dir, target_os=target_os
-    ):
+        await hub.tunnel[tunnel_plugin].tunnel(
+            target_name,
+            salt_conf["master_port"],
+            master_opts.get("master_port", 4506),
+        )
+        hub.log.info(f"Established SSH tunnel with {salt_conf['id']}")
+    except asyncssh.misc.ChannelListenError as err:
+        hub.log.error(f"Could not establish SSH tunnel with {salt_conf['id']}")
         return False
-
-    hub.log.debug(f"Generating minion keys: {key_dir}")
-    cmd = f"{binary_path} key --gen-keys=minion --gen-keys-dir={key_dir}"
-    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, cmd, target_os=target_os)
-    if ret.returncode != 0:
-        hub.log.error("Failed to generate minion keys")
+    except asyncssh.misc.ChannelOpenError as err:
+        hub.log.warning(f"SSH Channel closed unexpectedly with {salt_conf['id']}")
         return False
+    return True
 
-    hub.log.debug("Copying minion keys to the master")
-    opts = salt.config.client_config(hub.salt.key.local_master.DEFAULT_MASTER_CONFIG)
-    minion_key = pathlib.Path(opts["pki_dir"]) / "minions" / minion_id
 
-    await hub.tunnel[tunnel_plugin].get(
-        target_name,
-        key_dir / f"minion.pub",
-        minion_key,
-    )
-    if not minion_key.is_file():
-        hub.log.error("The minion key was not accepted")
+def generate_aliases(hub, run_dir, run_dir_root=None, target_os="linux"):
+    """
+    Generate the alias data for the Salt Minion
+    """
+    if not run_dir_root:
+        run_dir_root = hub.heist.init.default(target_os, "run_dir_root")
+
+    if not hub.tool.path.clean_path(run_dir_root, run_dir):
+        hub.log.error(
+            f"The run_dir {run_dir} is not a valid path when generating aliases"
+        )
         return False
 
-    hub.heist.CONS[target_name].update(
-        {
-            "minion_id": minion_id,
-        }
+    artifacts_dir = (
+        pathlib.Path(hub.tool.artifacts.get_artifact_dir(target_os=target_os))
+        / "scripts"
+        / "minion"
     )
-    hub.log.info(f"Accepted minion keys for {minion_id}")
-    return True
+    artifacts_dir.mkdir(parents=True, exist_ok=True)
+    aliases = {
+        "salt-call": {"file": artifacts_dir / "salt-call", "cmd": "salt-call"},
+        "salt-minion": {"file": artifacts_dir / "salt-minion", "cmd": "salt-minion"},
+    }
+
+    content = (
+        "#!/bin/bash\n"
+        'if [[ -z "${{SSL_CERT_DIR}}" ]] && command -v openssl &> /dev/null; then\n'
+        "_DIR=$(openssl version -d)\n"
+        'export SSL_CERT_DIR=${{_DIR:13:-1}}"/certs"\n'
+        'export SSL_CERT_FILE=${{_DIR:13:-1}}"/cert.pem"\n'
+        "fi\n"
+        f"exec {str(hub.tool.artifacts.get_salt_path(run_dir, run_dir_root=run_dir_root, target_os=target_os))}"
+        '/{alias} "${{@:1}}" -c '
+        f"{hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
+    )
+    if target_os == "windows":
+        content = (
+            "@ECHO OFF\n"
+            f"{str(hub.tool.artifacts.get_salt_path(run_dir, run_dir_root=run_dir_root, target_os=target_os))} "
+            "{alias} %* -c "
+            f"{hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
+        )
+    return aliases, artifacts_dir, content
+
+
+def get_salt_opts(
+    hub,
+    run_dir,
+    target_name,
+    run_dir_root=None,
+    target_os="linux",
+    target_id=None,
+    bootstrap=False,
+):
+    config = {}
+    roster = hub.heist.ROSTERS[target_name]
 
+    if not run_dir_root:
+        run_dir_root = hub.heist.init.default(target_os, "run_dir_root")
 
-async def accept_key_master(hub, target_name, tunnel_plugin, run_dir, minion_id=None):
+    if not hub.tool.path.clean_path(run_dir_root, run_dir):
+        hub.log.error(
+            f"The run_dir {run_dir} is not a valid path when getting salt opts"
+        )
+        return False
+
+    required = {
+        "root_dir": str(run_dir / "root_dir"),
+        "id": target_id,
+        "grains": {"minion_type": "heist"},
+    }
+    if not bootstrap:
+        required["master"] = "127.0.0.1"
+        required["master_port"] = 44506
+        required["publish_port"] = 44505
+    minion_opts = roster.get("minion_opts")
+    if minion_opts:
+        for key, value in minion_opts.items():
+            # Use configurations set by user
+            config[key] = value
+
+    for req in required.keys():
+        if not config.get(req):
+            config[req] = required[req]
+
+    return "minion", config
+
+
+def raw_run_cmd(
+    hub, service_plugin, run_dir, run_dir_root=None, target_os="linux", **kwargs
+):
     """
-    Accept the minions key on the salt-master
+    function to return the run_cmd used to start the salt
+    minion when using the raw service plugin
     """
-    if not minion_id:
-        hub.log.info("Querying minion id and attempting to accept the minion's key")
-        ret = await hub.salt.call.init.get_id(target_name, tunnel_plugin, run_dir)
-        if ret.returncode == 0:
-            minion_id = ret.stdout.split()[1]
-        else:
-            hub.log.error("Could not determine the minion_id")
-            return False
-    retry_key_count = hub.OPT.heist.get("retry_key_count", 5)
-    while retry_key_count > 0:
-        if hub.salt.key.init.accept_minion(minion_id):
-            break
-        await asyncio.sleep(5)
-        retry_key_count = retry_key_count - 1
-    else:
-        hub.log.error(f"Could not accept the key for the minion: {minion_id}")
+    if not run_dir_root:
+        run_dir_root = hub.heist.init.default(target_os, "run_dir_root")
+
+    if not hub.tool.path.clean_path(run_dir_root, run_dir):
+        hub.log.error(f"The {run_dir} directory is not valid")
         return False
-    hub.heist.CONS[target_name].update(
-        {
-            "minion_id": minion_id,
-        }
+
+    service_name = hub.heist[hub.SUBPARSER].get_service_name(
+        service_plugin, target_os=target_os
     )
-    hub.log.info(f"Accepted the key for minion: {minion_id}")
-    return True
+    run_cmd = (
+        str(
+            hub.tool.artifacts.get_salt_path(
+                run_dir, run_dir_root=run_dir_root, target_os=target_os
+            )
+            / service_name
+        )
+        + f" -c {hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
+    )
+    return run_cmd
```

### Comparing `heist-salt-5.3.1/heist_salt/salt/key/local_master.py` & `heist-salt-6.0.0/heist_salt/salt/key/local_master.py`

 * *Files identical despite different names*

### Comparing `heist-salt-5.3.1/heist_salt/tool/config.py` & `heist-salt-6.0.0/heist_salt/tool/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import tempfile
 
 import yaml
 
 
 def get_minion_opts(
-    hub, run_dir, target_name, target_os="linux", minion_id=None, bootstrap=False
+    hub,
+    run_dir,
+    target_name,
+    target_os="linux",
+    target_id=None,
+    bootstrap=False,
+    run_dir_root=None,
 ):
     config = {}
     roster = hub.heist.ROSTERS[target_name]
-    if not hub.tool.path.clean_path(
-        hub.heist.init.default(target_os, "run_dir_root"), run_dir
-    ):
-        hub.log.error(f"The {run_dir} directory is not valid")
+    if not run_dir_root:
+        run_dir_root = hub.heist.init.default(target_os, "run_dir_root")
+    if not hub.tool.path.clean_path(run_dir_root, run_dir):
+        hub.log.error(f"The {run_dir} directory is not valid when generating salt opts")
         return False
     required = {
         "root_dir": str(run_dir / "root_dir"),
-        "id": minion_id,
+        "id": target_id,
         "grains": {"minion_type": "heist"},
     }
     if not bootstrap:
         required["master"] = "127.0.0.1"
         required["master_port"] = 44506
         required["publish_port"] = 44505
     minion_opts = roster.get("minion_opts")
@@ -31,16 +37,20 @@
     for req in required.keys():
         if not config.get(req):
             config[req] = required[req]
 
     return config
 
 
-def mk_config(hub, config):
+def mk_config(hub, target_name, config, conf_file):
     """
     Create a config to use with this execution and return the file path
     for said config
     """
-    _, path = tempfile.mkstemp()
-    with open(path, "w+") as wfp:
+    perms = 0o710 if hub.tunnel.asyncssh.CONS[target_name].get("sudo") else 0o700
+    if not conf_file.parent.is_dir():
+        conf_file.parent.mkdir(mode=perms, parents=True)
+    if not conf_file.is_file():
+        conf_file.touch(mode=perms)
+    with open(conf_file, "w+") as wfp:
         yaml.safe_dump(config, wfp)
-    return path
+    return conf_file
```

### Comparing `heist-salt-5.3.1/heist_salt.egg-info/SOURCES.txt` & `heist-salt-6.0.0/heist_salt.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 heist_salt.egg-info/PKG-INFO
 heist_salt.egg-info/SOURCES.txt
 heist_salt.egg-info/dependency_links.txt
 heist_salt.egg-info/requires.txt
 heist_salt.egg-info/top_level.txt
 heist_salt/artifact/salt.py
 heist_salt/heist/salt/init.py
+heist_salt/heist/salt/master.py
 heist_salt/heist/salt/minion.py
+heist_salt/heist/salt/proxy.py
 heist_salt/salt/init.py
 heist_salt/salt/call/init.py
 heist_salt/salt/call/contracts/init.py
 heist_salt/salt/key/api.py
 heist_salt/salt/key/init.py
 heist_salt/salt/key/local_master.py
 heist_salt/salt/key/raas.py
 heist_salt/salt/key/contracts/init.py
+heist_salt/salt/pillar/init.py
 heist_salt/service/init.py
-heist_salt/service/salt/minion.py
+heist_salt/service/salt/init.py
 heist_salt/tool/artifacts.py
 heist_salt/tool/config.py
 heist_salt/tool/init.py
 heist_salt/tool/service.py
```

### Comparing `heist-salt-5.3.1/pyproject.toml` & `heist-salt-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heist-salt-5.3.1/setup.py` & `heist-salt-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
 
 with open("requirements/base.txt") as f:
     REQUIREMENTS = f.read().splitlines()
 
+with open("requirements/heist.txt") as f:
+    REQUIREMENTS.append(f.read().splitlines())
+
 
 class Clean(Command):
     user_options = []
 
     def initialize_options(self):
         pass
```

