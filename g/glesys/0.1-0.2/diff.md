# Comparing `tmp/glesys-0.1.tar.gz` & `tmp/glesys-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glesys-0.1.tar", last modified: Wed May  3 14:51:16 2023, max compression
+gzip compressed data, was "glesys-0.2.tar", last modified: Wed May  3 19:53:27 2023, max compression
```

## Comparing `glesys-0.1.tar` & `glesys-0.2.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/
--rw-r--r--   0 anton     (1000) anton     (1000)    34523 2023-05-03 13:55:42.000000 glesys-0.1/LICENSE
--rw-r--r--   0 anton     (1000) anton     (1000)    10688 2023-05-03 14:51:16.767670 glesys-0.1/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)    10046 2023-05-03 14:10:45.000000 glesys-0.1/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.764337 glesys-0.1/glesys/
--rw-r--r--   0 anton     (1000) anton     (1000)      647 2023-05-03 13:55:42.000000 glesys-0.1/glesys/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)      507 2023-05-03 13:55:42.000000 glesys-0.1/glesys/__main__.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.764337 glesys-0.1/glesys/api/
--rw-r--r--   0 anton     (1000) anton     (1000)     3580 2023-05-03 13:55:42.000000 glesys-0.1/glesys/api/__init__.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/glesys/cli/
--rw-r--r--   0 anton     (1000) anton     (1000)      447 2023-05-03 13:55:42.000000 glesys-0.1/glesys/cli/args.py
--rw-r--r--   0 anton     (1000) anton     (1000)      151 2023-05-03 13:55:42.000000 glesys-0.1/glesys/cli/args_router.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/glesys/cli/arguments/
--rw-r--r--   0 anton     (1000) anton     (1000)     1783 2023-05-03 13:55:42.000000 glesys-0.1/glesys/cli/arguments/dns.py
--rw-r--r--   0 anton     (1000) anton     (1000)     1435 2023-05-03 13:55:42.000000 glesys-0.1/glesys/cli/arguments/letsencrypt.py
--rw-r--r--   0 anton     (1000) anton     (1000)     1019 2023-05-03 13:55:42.000000 glesys-0.1/glesys/configuration.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/glesys/dns/
--rw-r--r--   0 anton     (1000) anton     (1000)      958 2023-05-03 13:55:42.000000 glesys-0.1/glesys/dns/cli_handler.py
--rw-r--r--   0 anton     (1000) anton     (1000)      427 2023-05-03 13:55:42.000000 glesys-0.1/glesys/exceptions.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.764337 glesys-0.1/glesys/hooks/
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/glesys/hooks/letsencrypt/
--rw-r--r--   0 anton     (1000) anton     (1000)     1472 2023-05-03 13:55:42.000000 glesys-0.1/glesys/hooks/letsencrypt/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)     2501 2023-05-03 13:55:42.000000 glesys-0.1/glesys/hooks/letsencrypt/cli_handler.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.767670 glesys-0.1/glesys/models/
--rw-r--r--   0 anton     (1000) anton     (1000)      282 2023-05-03 13:55:42.000000 glesys-0.1/glesys/models/configuration.py
--rw-r--r--   0 anton     (1000) anton     (1000)     3475 2023-05-03 13:55:42.000000 glesys-0.1/glesys/output.py
--rw-r--r--   0 anton     (1000) anton     (1000)      182 2023-05-03 13:55:42.000000 glesys-0.1/glesys/session.py
--rw-r--r--   0 anton     (1000) anton     (1000)    15152 2023-05-03 13:55:42.000000 glesys-0.1/glesys/workers.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 14:51:16.764337 glesys-0.1/glesys.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)    10688 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      616 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)      121 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/entry_points.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       94 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        7 2023-05-03 14:51:16.000000 glesys-0.1/glesys.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) anton     (1000)     1491 2023-05-03 13:55:42.000000 glesys-0.1/pyproject.toml
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2023-05-03 14:51:16.767670 glesys-0.1/setup.cfg
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/
+-rw-r--r--   0 anton     (1000) anton     (1000)    34523 2023-05-03 13:55:42.000000 glesys-0.2/LICENSE
+-rw-r--r--   0 anton     (1000) anton     (1000)    10739 2023-05-03 19:53:27.932412 glesys-0.2/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)    10097 2023-05-03 19:36:52.000000 glesys-0.2/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/
+-rw-r--r--   0 anton     (1000) anton     (1000)      647 2023-05-03 19:38:16.000000 glesys-0.2/glesys/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      507 2023-05-03 13:55:42.000000 glesys-0.2/glesys/__main__.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/api/
+-rw-r--r--   0 anton     (1000) anton     (1000)      346 2023-05-03 19:22:51.000000 glesys-0.2/glesys/api/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2421 2023-05-03 17:16:13.000000 glesys-0.2/glesys/api/dns.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     1026 2023-05-03 19:36:25.000000 glesys-0.2/glesys/api/ip.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     4110 2023-05-03 19:19:58.000000 glesys-0.2/glesys/api/server.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/cli/
+-rw-r--r--   0 anton     (1000) anton     (1000)      447 2023-05-03 13:55:42.000000 glesys-0.2/glesys/cli/args.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      231 2023-05-03 19:25:40.000000 glesys-0.2/glesys/cli/args_router.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/cli/arguments/
+-rw-r--r--   0 anton     (1000) anton     (1000)     1783 2023-05-03 13:55:42.000000 glesys-0.2/glesys/cli/arguments/dns.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      768 2023-05-03 19:33:30.000000 glesys-0.2/glesys/cli/arguments/ip.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     1435 2023-05-03 13:55:42.000000 glesys-0.2/glesys/cli/arguments/letsencrypt.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2599 2023-05-03 19:15:27.000000 glesys-0.2/glesys/cli/arguments/server.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      169 2023-05-03 19:25:29.000000 glesys-0.2/glesys/cli/ip.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      978 2023-05-03 19:15:50.000000 glesys-0.2/glesys/cli/server.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     1019 2023-05-03 13:55:42.000000 glesys-0.2/glesys/configuration.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/dns/
+-rw-r--r--   0 anton     (1000) anton     (1000)      958 2023-05-03 13:55:42.000000 glesys-0.2/glesys/dns/cli_handler.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      427 2023-05-03 13:55:42.000000 glesys-0.2/glesys/exceptions.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     1174 2023-05-03 19:04:32.000000 glesys-0.2/glesys/helpers.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/hooks/
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/hooks/letsencrypt/
+-rw-r--r--   0 anton     (1000) anton     (1000)     1472 2023-05-03 13:55:42.000000 glesys-0.2/glesys/hooks/letsencrypt/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2501 2023-05-03 13:55:42.000000 glesys-0.2/glesys/hooks/letsencrypt/cli_handler.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys/models/
+-rw-r--r--   0 anton     (1000) anton     (1000)      281 2023-05-03 17:08:05.000000 glesys-0.2/glesys/models/configuration.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3475 2023-05-03 13:55:42.000000 glesys-0.2/glesys/output.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      182 2023-05-03 13:55:42.000000 glesys-0.2/glesys/session.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    15152 2023-05-03 13:55:42.000000 glesys-0.2/glesys/workers.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2023-05-03 19:53:27.932412 glesys-0.2/glesys.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)    10739 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      786 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)      121 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/entry_points.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       94 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        7 2023-05-03 19:53:27.000000 glesys-0.2/glesys.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)     1491 2023-05-03 13:55:42.000000 glesys-0.2/pyproject.toml
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2023-05-03 19:53:27.932412 glesys-0.2/setup.cfg
```

### Comparing `glesys-0.1/LICENSE` & `glesys-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glesys-0.1/PKG-INFO` & `glesys-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glesys
-Version: 0.1
+Version: 0.2
 Summary: A SDK/helper library to work with Glesys API.
 Author-email: Anton Hvornum <anton@hvornum.se>
 License: AGPL-1.0-or-later
 Project-URL: Home, https://api.glesys.com/
 Project-URL: Documentation, https://glesys.se/kb/artikel/api-dokumentation
 Project-URL: Source, https://github.com/Torxed/python-glesys
 Keywords: linux,glesys,server,oauth2,openid,connect
@@ -22,16 +22,15 @@
 It's also a CLI tool to access a subset of all those features as well as housing a LetsEncrypt  [certbot](https://github.com/certbot/certbot) Authenticator plugin.
 
 *Small Disclaimer: I have no affiliation with Glesys, I just appreciate their API and services*
 
 # Installation
 
 ```
-$ python -m build .
-$ sudo python -m installer dist/*.whl
+$ pip install glesys
 ```
 
 # Usage
 
 :information_source: This assumes a valid `glesys.toml` configuration.
 
 ## List all domains
@@ -78,44 +77,46 @@
 
 ```
 $ sudo glesys lets-encrypt --individual --hostname '*.hvornum.se' --hostname 'hvornum.se'
 ```
 
 # Supported API Endpoints
 
- * [ ] https://api.glesys.com/server/list
- * [ ] https://api.glesys.com/server/details
- * [ ] https://api.glesys.com/server/networkadapters
+As of 2023-05-03 [API Doc Spec](https://github.com/GleSYS/API/wiki/API-Documentation).
+
+ * [x] https://api.glesys.com/server/list
+ * [x] https://api.glesys.com/server/details
+ * [x] https://api.glesys.com/server/networkadapters
  * [ ] https://api.glesys.com/server/backup
  * [ ] https://api.glesys.com/server/status
  * [ ] https://api.glesys.com/server/reboot
  * [ ] https://api.glesys.com/server/reset
  * [ ] https://api.glesys.com/server/stop
  * [ ] https://api.glesys.com/server/start
  * [ ] https://api.glesys.com/server/create
  * [ ] https://api.glesys.com/server/createfrombackup
  * [ ] https://api.glesys.com/server/createmanualbackup
  * [ ] https://api.glesys.com/server/deletemanualbackup
  * [ ] https://api.glesys.com/server/destroy
  * [ ] https://api.glesys.com/server/edit
  * [ ] https://api.glesys.com/server/clone
- * [ ] https://api.glesys.com/server/limits
+ * [x] https://api.glesys.com/server/limits
  * [ ] https://api.glesys.com/server/resetlimit
  * [ ] https://api.glesys.com/server/listbackups
  * [ ] https://api.glesys.com/server/console
  * [ ] https://api.glesys.com/server/resetpassword
  * [ ] https://api.glesys.com/server/templates
  * [ ] https://api.glesys.com/server/allowedarguments
  * [ ] https://api.glesys.com/server/resourceusage
- * [ ] https://api.glesys.com/server/costs
+ * [x] https://api.glesys.com/server/costs
  * [ ] https://api.glesys.com/server/listiso
  * [ ] https://api.glesys.com/server/mountiso
  * [ ] https://api.glesys.com/server/estimatedcost
  * [ ] https://api.glesys.com/server/previewcloudconfig
- * [ ] https://api.glesys.com/ip/listfree
+ * [x] https://api.glesys.com/ip/listfree
  * [ ] https://api.glesys.com/ip/listown
  * [ ] https://api.glesys.com/ip/details
  * [ ] https://api.glesys.com/ip/take
  * [ ] https://api.glesys.com/ip/release
  * [ ] https://api.glesys.com/ip/add
  * [ ] https://api.glesys.com/ip/remove
  * [ ] https://api.glesys.com/ip/setptr
```

### Comparing `glesys-0.1/README.md` & `glesys-0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 It's also a CLI tool to access a subset of all those features as well as housing a LetsEncrypt  [certbot](https://github.com/certbot/certbot) Authenticator plugin.
 
 *Small Disclaimer: I have no affiliation with Glesys, I just appreciate their API and services*
 
 # Installation
 
 ```
-$ python -m build .
-$ sudo python -m installer dist/*.whl
+$ pip install glesys
 ```
 
 # Usage
 
 :information_source: This assumes a valid `glesys.toml` configuration.
 
 ## List all domains
@@ -60,44 +59,46 @@
 
 ```
 $ sudo glesys lets-encrypt --individual --hostname '*.hvornum.se' --hostname 'hvornum.se'
 ```
 
 # Supported API Endpoints
 
- * [ ] https://api.glesys.com/server/list
- * [ ] https://api.glesys.com/server/details
- * [ ] https://api.glesys.com/server/networkadapters
+As of 2023-05-03 [API Doc Spec](https://github.com/GleSYS/API/wiki/API-Documentation).
+
+ * [x] https://api.glesys.com/server/list
+ * [x] https://api.glesys.com/server/details
+ * [x] https://api.glesys.com/server/networkadapters
  * [ ] https://api.glesys.com/server/backup
  * [ ] https://api.glesys.com/server/status
  * [ ] https://api.glesys.com/server/reboot
  * [ ] https://api.glesys.com/server/reset
  * [ ] https://api.glesys.com/server/stop
  * [ ] https://api.glesys.com/server/start
  * [ ] https://api.glesys.com/server/create
  * [ ] https://api.glesys.com/server/createfrombackup
  * [ ] https://api.glesys.com/server/createmanualbackup
  * [ ] https://api.glesys.com/server/deletemanualbackup
  * [ ] https://api.glesys.com/server/destroy
  * [ ] https://api.glesys.com/server/edit
  * [ ] https://api.glesys.com/server/clone
- * [ ] https://api.glesys.com/server/limits
+ * [x] https://api.glesys.com/server/limits
  * [ ] https://api.glesys.com/server/resetlimit
  * [ ] https://api.glesys.com/server/listbackups
  * [ ] https://api.glesys.com/server/console
  * [ ] https://api.glesys.com/server/resetpassword
  * [ ] https://api.glesys.com/server/templates
  * [ ] https://api.glesys.com/server/allowedarguments
  * [ ] https://api.glesys.com/server/resourceusage
- * [ ] https://api.glesys.com/server/costs
+ * [x] https://api.glesys.com/server/costs
  * [ ] https://api.glesys.com/server/listiso
  * [ ] https://api.glesys.com/server/mountiso
  * [ ] https://api.glesys.com/server/estimatedcost
  * [ ] https://api.glesys.com/server/previewcloudconfig
- * [ ] https://api.glesys.com/ip/listfree
+ * [x] https://api.glesys.com/ip/listfree
  * [ ] https://api.glesys.com/ip/listown
  * [ ] https://api.glesys.com/ip/details
  * [ ] https://api.glesys.com/ip/take
  * [ ] https://api.glesys.com/ip/release
  * [ ] https://api.glesys.com/ip/add
  * [ ] https://api.glesys.com/ip/remove
  * [ ] https://api.glesys.com/ip/setptr
```

### Comparing `glesys-0.1/glesys/__init__.py` & `glesys-0.2/glesys/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .cli.args_router import loaded
 from .cli.args import load_arguments
 
 session = None
-__version__ = "0.1"
+__version__ = "0.2"
 
 def run_as_a_module():
 	# global session
 
 	args = load_arguments()
 	
 	# import importlib
```

### Comparing `glesys-0.1/glesys/cli/arguments/dns.py` & `glesys-0.2/glesys/cli/arguments/dns.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/cli/arguments/letsencrypt.py` & `glesys-0.2/glesys/cli/arguments/letsencrypt.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/configuration.py` & `glesys-0.2/glesys/configuration.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/dns/cli_handler.py` & `glesys-0.2/glesys/dns/cli_handler.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/hooks/letsencrypt/__init__.py` & `glesys-0.2/glesys/hooks/letsencrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/hooks/letsencrypt/cli_handler.py` & `glesys-0.2/glesys/hooks/letsencrypt/cli_handler.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/output.py` & `glesys-0.2/glesys/output.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys/workers.py` & `glesys-0.2/glesys/workers.py`

 * *Files identical despite different names*

### Comparing `glesys-0.1/glesys.egg-info/PKG-INFO` & `glesys-0.2/glesys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glesys
-Version: 0.1
+Version: 0.2
 Summary: A SDK/helper library to work with Glesys API.
 Author-email: Anton Hvornum <anton@hvornum.se>
 License: AGPL-1.0-or-later
 Project-URL: Home, https://api.glesys.com/
 Project-URL: Documentation, https://glesys.se/kb/artikel/api-dokumentation
 Project-URL: Source, https://github.com/Torxed/python-glesys
 Keywords: linux,glesys,server,oauth2,openid,connect
@@ -22,16 +22,15 @@
 It's also a CLI tool to access a subset of all those features as well as housing a LetsEncrypt  [certbot](https://github.com/certbot/certbot) Authenticator plugin.
 
 *Small Disclaimer: I have no affiliation with Glesys, I just appreciate their API and services*
 
 # Installation
 
 ```
-$ python -m build .
-$ sudo python -m installer dist/*.whl
+$ pip install glesys
 ```
 
 # Usage
 
 :information_source: This assumes a valid `glesys.toml` configuration.
 
 ## List all domains
@@ -78,44 +77,46 @@
 
 ```
 $ sudo glesys lets-encrypt --individual --hostname '*.hvornum.se' --hostname 'hvornum.se'
 ```
 
 # Supported API Endpoints
 
- * [ ] https://api.glesys.com/server/list
- * [ ] https://api.glesys.com/server/details
- * [ ] https://api.glesys.com/server/networkadapters
+As of 2023-05-03 [API Doc Spec](https://github.com/GleSYS/API/wiki/API-Documentation).
+
+ * [x] https://api.glesys.com/server/list
+ * [x] https://api.glesys.com/server/details
+ * [x] https://api.glesys.com/server/networkadapters
  * [ ] https://api.glesys.com/server/backup
  * [ ] https://api.glesys.com/server/status
  * [ ] https://api.glesys.com/server/reboot
  * [ ] https://api.glesys.com/server/reset
  * [ ] https://api.glesys.com/server/stop
  * [ ] https://api.glesys.com/server/start
  * [ ] https://api.glesys.com/server/create
  * [ ] https://api.glesys.com/server/createfrombackup
  * [ ] https://api.glesys.com/server/createmanualbackup
  * [ ] https://api.glesys.com/server/deletemanualbackup
  * [ ] https://api.glesys.com/server/destroy
  * [ ] https://api.glesys.com/server/edit
  * [ ] https://api.glesys.com/server/clone
- * [ ] https://api.glesys.com/server/limits
+ * [x] https://api.glesys.com/server/limits
  * [ ] https://api.glesys.com/server/resetlimit
  * [ ] https://api.glesys.com/server/listbackups
  * [ ] https://api.glesys.com/server/console
  * [ ] https://api.glesys.com/server/resetpassword
  * [ ] https://api.glesys.com/server/templates
  * [ ] https://api.glesys.com/server/allowedarguments
  * [ ] https://api.glesys.com/server/resourceusage
- * [ ] https://api.glesys.com/server/costs
+ * [x] https://api.glesys.com/server/costs
  * [ ] https://api.glesys.com/server/listiso
  * [ ] https://api.glesys.com/server/mountiso
  * [ ] https://api.glesys.com/server/estimatedcost
  * [ ] https://api.glesys.com/server/previewcloudconfig
- * [ ] https://api.glesys.com/ip/listfree
+ * [x] https://api.glesys.com/ip/listfree
  * [ ] https://api.glesys.com/ip/listown
  * [ ] https://api.glesys.com/ip/details
  * [ ] https://api.glesys.com/ip/take
  * [ ] https://api.glesys.com/ip/release
  * [ ] https://api.glesys.com/ip/add
  * [ ] https://api.glesys.com/ip/remove
  * [ ] https://api.glesys.com/ip/setptr
```

### Comparing `glesys-0.1/glesys.egg-info/SOURCES.txt` & `glesys-0.2/glesys.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 glesys/__init__.py
 glesys/__main__.py
 glesys/configuration.py
 glesys/exceptions.py
+glesys/helpers.py
 glesys/output.py
 glesys/session.py
 glesys/workers.py
 glesys.egg-info/PKG-INFO
 glesys.egg-info/SOURCES.txt
 glesys.egg-info/dependency_links.txt
 glesys.egg-info/entry_points.txt
 glesys.egg-info/requires.txt
 glesys.egg-info/top_level.txt
 glesys/api/__init__.py
+glesys/api/dns.py
+glesys/api/ip.py
+glesys/api/server.py
 glesys/cli/args.py
 glesys/cli/args_router.py
+glesys/cli/ip.py
+glesys/cli/server.py
 glesys/cli/arguments/dns.py
+glesys/cli/arguments/ip.py
 glesys/cli/arguments/letsencrypt.py
+glesys/cli/arguments/server.py
 glesys/dns/cli_handler.py
 glesys/hooks/letsencrypt/__init__.py
 glesys/hooks/letsencrypt/cli_handler.py
 glesys/models/configuration.py
```

### Comparing `glesys-0.1/pyproject.toml` & `glesys-0.2/pyproject.toml`

 * *Files identical despite different names*

