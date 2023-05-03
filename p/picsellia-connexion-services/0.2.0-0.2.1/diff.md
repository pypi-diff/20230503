# Comparing `tmp/picsellia_connexion_services-0.2.0.tar.gz` & `tmp/picsellia_connexion_services-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia_connexion_services-0.2.0.tar", max compression
+gzip compressed data, was "picsellia_connexion_services-0.2.1.tar", max compression
```

## Comparing `picsellia_connexion_services-0.2.0.tar` & `picsellia_connexion_services-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2022-01-03 09:40:20.048926 picsellia_connexion_services-0.2.0/LICENSE
--rw-r--r--   0        0        0     1091 2022-09-23 12:56:47.826096 picsellia_connexion_services-0.2.0/README.md
--rw-r--r--   0        0        0      409 2023-03-08 13:35:29.332565 picsellia_connexion_services-0.2.0/picsellia_connexion_services/__init__.py
--rw-r--r--   0        0        0      418 2022-10-11 04:51:31.756523 picsellia_connexion_services-0.2.0/picsellia_connexion_services/abstract_cached_connexions.py
--rw-r--r--   0        0        0     1492 2022-10-11 04:51:31.816522 picsellia_connexion_services-0.2.0/picsellia_connexion_services/abstract_service_connexion.py
--rw-r--r--   0        0        0     1488 2022-10-11 04:54:17.445905 picsellia_connexion_services-0.2.0/picsellia_connexion_services/cached_connexions.py
--rw-r--r--   0        0        0      480 2023-03-08 13:23:09.936839 picsellia_connexion_services-0.2.0/picsellia_connexion_services/exceptions.py
--rw-r--r--   0        0        0     5638 2023-03-08 13:18:08.351423 picsellia_connexion_services-0.2.0/picsellia_connexion_services/jwt_service.py
--rw-r--r--   0        0        0     1459 2023-02-16 06:43:51.941260 picsellia_connexion_services-0.2.0/picsellia_connexion_services/mock_cached_connexions.py
--rw-r--r--   0        0        0     3514 2023-03-08 13:27:04.273994 picsellia_connexion_services-0.2.0/picsellia_connexion_services/mock_service_connexion.py
--rw-r--r--   0        0        0     3367 2023-03-08 13:18:04.815407 picsellia_connexion_services-0.2.0/picsellia_connexion_services/token_service.py
--rw-r--r--   0        0        0      495 2023-03-08 13:27:19.166068 picsellia_connexion_services-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 picsellia_connexion_services-0.2.0/setup.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 picsellia_connexion_services-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-01-03 09:40:20.048926 picsellia_connexion_services-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1091 2022-09-23 12:56:47.826096 picsellia_connexion_services-0.2.1/README.md
+-rw-r--r--   0        0        0      409 2023-05-03 12:02:06.490232 picsellia_connexion_services-0.2.1/picsellia_connexion_services/__init__.py
+-rw-r--r--   0        0        0      418 2022-10-11 04:51:31.756523 picsellia_connexion_services-0.2.1/picsellia_connexion_services/abstract_cached_connexions.py
+-rw-r--r--   0        0        0     1492 2022-10-11 04:51:31.816522 picsellia_connexion_services-0.2.1/picsellia_connexion_services/abstract_service_connexion.py
+-rw-r--r--   0        0        0     1488 2022-10-11 04:54:17.445905 picsellia_connexion_services-0.2.1/picsellia_connexion_services/cached_connexions.py
+-rw-r--r--   0        0        0      480 2023-03-08 13:23:09.936839 picsellia_connexion_services-0.2.1/picsellia_connexion_services/exceptions.py
+-rw-r--r--   0        0        0     5638 2023-03-08 13:18:08.351423 picsellia_connexion_services-0.2.1/picsellia_connexion_services/jwt_service.py
+-rw-r--r--   0        0        0     1459 2023-02-16 06:43:51.941260 picsellia_connexion_services-0.2.1/picsellia_connexion_services/mock_cached_connexions.py
+-rw-r--r--   0        0        0     3505 2023-05-03 11:59:30.133449 picsellia_connexion_services-0.2.1/picsellia_connexion_services/mock_service_connexion.py
+-rw-r--r--   0        0        0     3367 2023-03-08 13:18:04.815407 picsellia_connexion_services-0.2.1/picsellia_connexion_services/token_service.py
+-rw-r--r--   0        0        0      495 2023-05-03 12:02:15.974280 picsellia_connexion_services-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 picsellia_connexion_services-0.2.1/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 picsellia_connexion_services-0.2.1/PKG-INFO
```

### Comparing `picsellia_connexion_services-0.2.0/LICENSE` & `picsellia_connexion_services-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/README.md` & `picsellia_connexion_services-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/abstract_service_connexion.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/abstract_service_connexion.py`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/cached_connexions.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/cached_connexions.py`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/jwt_service.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/jwt_service.py`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/mock_cached_connexions.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/mock_cached_connexions.py`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/mock_service_connexion.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/mock_service_connexion.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             "delete": {},
         }
 
     @staticmethod
     def handle_keywords(path):
         return path.replace(
             "<uuid>",
-            "[a-f0-9]{8}-[a-f0-9]{4}-4[a-f0-9]{3}-[89aAbB][a-f0-9]{3}-[a-f0-9]{12}",
+            "[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}",
         )
 
     def set_default_response(self, method: str, response: Any) -> None:
         self.default_responses[method] = response
 
     def set_response(self, method: str, regex_path: str, response: Any) -> None:
         self.responses[method][self.handle_keywords(regex_path)] = response
```

### Comparing `picsellia_connexion_services-0.2.0/picsellia_connexion_services/token_service.py` & `picsellia_connexion_services-0.2.1/picsellia_connexion_services/token_service.py`

 * *Files identical despite different names*

### Comparing `picsellia_connexion_services-0.2.0/setup.py` & `picsellia_connexion_services-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28,<3.0']
 
 setup_kwargs = {
     'name': 'picsellia-connexion-services',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Package for connection to Picsellia platforms with some wrapper around requests library',
     'long_description': '# Picsellia Services\n\nPicsellia Services is a Python library that wraps connexions with Picsellia micro services.\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install picsellia-connexion-services.\n\n```bash\npip install picsellia-connexion-services\n```\n\n## Usage\n### JwtToken\n```python\nfrom picsellia_connexion_services.jwt_service import JwtServiceConnexion\nservice = JwtServiceConnexion({\'api_token\': \'<api_token>\', \'deployment_id\': \'<deployment_id>\'}, \'localhost:8000\')\nservice.get(f\'/deployment/{deployment_id}/stats\')\n```\n\n## Usage in mocked tests\n\n```python\nfrom picsellia_connexion_services.mocked_service import MockedServiceConnexion\nservice = MockedServiceConnexion(\'test\')\nservice.set_next_mocked_response("get", "/ping", JsonResponse({"ok" : True}, status=status.HTTP_200_OK))\nservice.get("/ping")\n```\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)',
     'author': 'Thomas Darget',
     'author_email': 'thomas.darget@picsellia.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `picsellia_connexion_services-0.2.0/PKG-INFO` & `picsellia_connexion_services-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picsellia-connexion-services
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for connection to Picsellia platforms with some wrapper around requests library
 License: MIT
 Author: Thomas Darget
 Author-email: thomas.darget@picsellia.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

