# Comparing `tmp/cyral-gimme-db-token-0.8.1.tar.gz` & `tmp/cyral-gimme-db-token-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyral-gimme-db-token-0.8.1.tar", max compression
+gzip compressed data, was "cyral-gimme-db-token-0.8.2.tar", max compression
```

## Comparing `cyral-gimme-db-token-0.8.1.tar` & `cyral-gimme-db-token-0.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      289 2022-08-29 17:46:12.090658 cyral-gimme-db-token-0.8.1/gimme_db_token/__init__.py
--rw-r--r--   0        0        0     7006 2022-09-13 20:22:49.107781 cyral-gimme-db-token-0.8.1/gimme_db_token/__main__.py
--rw-r--r--   0        0        0     6207 2022-09-13 20:22:49.108241 cyral-gimme-db-token-0.8.1/gimme_db_token/_aws.py
--rw-r--r--   0        0        0     2492 2022-09-13 20:22:49.108715 cyral-gimme-db-token-0.8.1/gimme_db_token/_client.py
--rw-r--r--   0        0        0     1463 2022-09-13 20:22:49.109109 cyral-gimme-db-token-0.8.1/gimme_db_token/_config.py
--rw-r--r--   0        0        0     1840 2022-08-29 17:46:12.090939 cyral-gimme-db-token-0.8.1/gimme_db_token/_crypto.py
--rw-r--r--   0        0        0     1838 2022-08-29 17:46:12.091002 cyral-gimme-db-token-0.8.1/gimme_db_token/_pgpass.py
--rw-r--r--   0        0        0      920 2022-09-13 20:22:49.109601 cyral-gimme-db-token-0.8.1/gimme_db_token/_token.py
--rw-r--r--   0        0        0      688 2022-09-13 20:22:49.109887 cyral-gimme-db-token-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      833 2022-09-13 20:29:46.623839 cyral-gimme-db-token-0.8.1/setup.py
--rw-r--r--   0        0        0      628 2022-09-13 20:29:46.623987 cyral-gimme-db-token-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2022-07-09 19:18:36.652390 cyral-gimme-db-token-0.8.2/gimme_db_token/__init__.py
+-rw-r--r--   0        0        0     7006 2023-05-02 22:34:49.615866 cyral-gimme-db-token-0.8.2/gimme_db_token/__main__.py
+-rw-r--r--   0        0        0     6655 2023-05-02 22:34:49.616392 cyral-gimme-db-token-0.8.2/gimme_db_token/_aws.py
+-rw-r--r--   0        0        0     2492 2023-05-02 22:34:49.616868 cyral-gimme-db-token-0.8.2/gimme_db_token/_client.py
+-rw-r--r--   0        0        0     1463 2023-05-02 22:34:49.617242 cyral-gimme-db-token-0.8.2/gimme_db_token/_config.py
+-rw-r--r--   0        0        0     1840 2022-07-09 19:18:36.653209 cyral-gimme-db-token-0.8.2/gimme_db_token/_crypto.py
+-rw-r--r--   0        0        0     1838 2023-05-02 22:34:49.617710 cyral-gimme-db-token-0.8.2/gimme_db_token/_pgpass.py
+-rw-r--r--   0        0        0      920 2023-05-02 22:34:49.618181 cyral-gimme-db-token-0.8.2/gimme_db_token/_token.py
+-rw-r--r--   0        0        0      697 2023-05-02 22:34:49.619560 cyral-gimme-db-token-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 cyral-gimme-db-token-0.8.2/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 cyral-gimme-db-token-0.8.2/PKG-INFO
```

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/__main__.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     default=5 * 60,
     envvar="CYRAL_DB_TOKEN_TIMEOUT",
     type=click.INT,
     show_envvar=True,
     help="Number of seconds to wait for Cyral server to respond before timeout",
 )
 @click.option("-v", "--verbose", is_flag=True)
-@click.version_option(version="0.8.1")
+@click.version_option(version="0.8.2")
 def update_token(
     db,
     address,
     tenant,
     sidecar,
     autoconfigure,
     profile,
```

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_aws.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,22 +83,24 @@
         values.update({"cli_legacy_plugin_path": get_cli_legacy_plugin_path()})
     config_path = get_config_file_path("config_file")
     write_config_file(values, config_path)
 
 
 def update_s3_proxy_endpoint(aws_profile_name, sidecar_endpoint):
     sidecar_endpoint = sidecar_endpoint.replace("http://", "").replace("https://", "")
-    values = {
-        "s3": {
-            "proxy": f"http://{sidecar_endpoint}",
-        },
-        "__section__": "profile " + aws_profile_name,
-    }
     config_path = get_config_file_path("config_file")
-    write_config_file(values, config_path)
+
+    for command in ["s3", "s3api"]:
+        values = {
+            command: {
+                "proxy": f"http://{sidecar_endpoint}",
+            },
+            "__section__": "profile " + aws_profile_name,
+        }
+        write_config_file(values, config_path)
 
 
 def s3_proxy_is_configured(aws_profile_name):
     session = get_session()
     config = session.full_config
     # a correctly configured config looks like the following:
     # {
@@ -106,14 +108,17 @@
     #         "s3-proxy":"awscli_plugin_s3_proxy"
     #     },
     #     "profiles":{
     #         "cyral":{
     #             "ca_bundle":"/home/user/.aws/cyral_ca_bundle.pem",
     #             "s3":{
     #                 "proxy":"http://sidecar.endpoint:453"
+    #             },
+    #             "s3api":{
+    #                 "proxy":"http://sidecar.endpoint:453"
     #             }
     #         }
     #     }
     # }
     return (
         # check if the config has a plugins field
         config.get("plugins")
@@ -127,14 +132,18 @@
         and config["profiles"][aws_profile_name].get("ca_bundle")
         # check if the value given to "ca_bundle" is a valid file
         and Path(config["profiles"][aws_profile_name]["ca_bundle"]).is_file()
         # check if "s3" got a value for the given aws profile
         and config["profiles"][aws_profile_name].get("s3")
         # check if "proxy" got a non-None value inside that s3 object
         and config["profiles"][aws_profile_name]["s3"].get("proxy")
+        # check if "s3api" got a value for the given aws profile
+        and config["profiles"][aws_profile_name].get("s3api")
+        # check if "proxy" got a non-None value inside that s3api object
+        and config["profiles"][aws_profile_name]["s3api"].get("proxy")
         # check if s3 proxy plugin is installed
         and s3_plugin_is_installed()
     )
 
 
 def install_s3_proxy_plugin():
     # install plugin using pip
```

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_client.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_client.py`

 * *Files identical despite different names*

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_config.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_config.py`

 * *Files identical despite different names*

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_crypto.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_crypto.py`

 * *Files identical despite different names*

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_pgpass.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_pgpass.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     with open(path, "w") as f:
         f.write(content)
 
 
 def update_pgpass_str(pgpass, hosts, access_token):
     for host in hosts:
         newline = f"{host}:*:*:*:{access_token}"
-        p = re.compile(fr"{host}:\*:\*:\*:.*")
+        p = re.compile(rf"{host}:\*:\*:\*:.*")
         pgpass, num_replaces = p.subn(newline, pgpass)
         if num_replaces == 0:
             # match is not found, add line on top
             pgpass = "\n".join((newline, pgpass))
     return pgpass
```

### Comparing `cyral-gimme-db-token-0.8.1/gimme_db_token/_token.py` & `cyral-gimme-db-token-0.8.2/gimme_db_token/_token.py`

 * *Files identical despite different names*

### Comparing `cyral-gimme-db-token-0.8.1/setup.py` & `cyral-gimme-db-token-0.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['awscli>=1.22.55,<2.0.0',
  'click>=8.0.3,<9.0.0',
- 'cryptography>=36.0.1,<37.0.0',
+ 'cryptography>=39.0.1,<40.0.0',
  'requests>=2.27.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['gimme_db_token = gimme_db_token.__main__:run']}
 
 setup_kwargs = {
     'name': 'cyral-gimme-db-token',
-    'version': '0.8.1',
+    'version': '0.8.2',
     'description': 'Eases using Cyral for SSO login to databases.',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Cyral',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `cyral-gimme-db-token-0.8.1/PKG-INFO` & `cyral-gimme-db-token-0.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cyral-gimme-db-token
-Version: 0.8.1
+Version: 0.8.2
 Summary: Eases using Cyral for SSO login to databases.
 Author: Cyral
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: awscli (>=1.22.55,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: cryptography (>=36.0.1,<37.0.0)
+Requires-Dist: cryptography (>=39.0.1,<40.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
```

