# Comparing `tmp/hakai_api-1.3.0.tar.gz` & `tmp/hakai_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakai_api-1.3.0.tar", last modified: Tue May  2 18:41:39 2023, max compression
+gzip compressed data, was "hakai_api-1.4.0.tar", last modified: Tue May  2 23:44:24 2023, max compression
```

## Comparing `hakai_api-1.3.0.tar` & `hakai_api-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 18:41:39.709599 hakai_api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-02 18:41:24.000000 hakai_api-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/hakai_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-02 18:41:24.000000 hakai_api-1.3.0/hakai_api/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 18:41:24.000000 hakai_api-1.3.0/hakai_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/hakai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:41:39.709599 hakai_api-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 18:41:24.000000 hakai_api-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.940628 hakai_api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 23:44:24.940628 hakai_api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-02 23:44:11.000000 hakai_api-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.936628 hakai_api-1.4.0/hakai_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-02 23:44:11.000000 hakai_api-1.4.0/hakai_api/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 23:44:11.000000 hakai_api-1.4.0/hakai_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.936628 hakai_api-1.4.0/hakai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:44:24.940628 hakai_api-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 23:44:11.000000 hakai_api-1.4.0/setup.py
```

### Comparing `hakai_api-1.3.0/PKG-INFO` & `hakai_api-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai_api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.3.0/README.md` & `hakai_api-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hakai_api-1.3.0/hakai_api/Client.py` & `hakai_api-1.4.0/hakai_api/Client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,109 +1,128 @@
 """Get authorized requests to the Hakai API using the requests library.
 
 Written by: Taylor Denouden, Chris Davis, and Nate Rosenstock
 Last updated: April 2021
 """
 
-import os
 import json
+import os
 from datetime import datetime
-from time import mktime, sleep
+from time import mktime
 from typing import Dict, Union
 
 from requests_oauthlib import OAuth2Session
 
 
 class Client(OAuth2Session):
     _credentials_file = os.path.expanduser("~/.hakai-api-auth")
+    DEFAULT_API_ROOT = "https://hecate.hakai.org/api"
+    DEFAULT_LOGIN_PAGE = "https://hecate.hakai.org/api-client-login"
 
     def __init__(
-        self,
-        api_root: str = "https://hecate.hakai.org/api",
-        login_page: str = "https://hecate.hakai.org/api-client-login",
-        credentials: Union[str, Dict] = None,
+            self,
+            api_root: str = DEFAULT_API_ROOT,
+            login_page: str = DEFAULT_LOGIN_PAGE,
+            credentials: Union[str, Dict] = None,
     ):
         """Create a new Client class with credentials.
 
         Params:
             api_root: The base url of the hakai api you want to call.
                       Defaults to the production server.
             credentials (str, Dict): Credentials token retrieved from the hakai api login page.
                                      If `None`, loads cached credentials or prompts for log in.
-        """     
+        """
         self._api_root = api_root
-        self._authorization_base_url = login_page
+        self._login_page = login_page
+        self._credentials = None
 
-        if credentials is None:
-            # Try to get cached credentials, prompt user if the file can't be loaded
-            self._credentials = self._try_to_load_credentials_file() or self._get_credentials_from_web()
+        if isinstance(credentials, dict):
+            self._credentials = credentials
         elif isinstance(credentials, str):
             # Parse credentials from string
-            self._credentials = dict(map(lambda x: x.split("="), credentials.split("&")))
-        elif isinstance(credentials, dict):
-            self._credentials = credentials
+            self._credentials = dict(
+                map(lambda x: x.split("="), credentials.split("&")))
+        elif self.file_credentials_are_valid():
+            self._credentials = self._get_credentials_from_file()
         else:
-            raise ValueError("`credentials` parameter should be str, dict, or None type.")
+            self._credentials = self._get_credentials_from_web()
+
+        if self._credentials is None:
+            raise ValueError("Credentials could not be set.")
 
         # Cache the credentials
-        self._save_credentials(self._credentials)
+        self._save_credentials_to_file(self._credentials)
 
         # Init the OAuth2Session parent class with credentials
         super(Client, self).__init__(token=self._credentials)
 
     @property
     def api_root(self) -> str:
         """Return the api base url."""
         return self._api_root
 
     @property
+    def login_page(self) -> str:
+        """Return the login page url."""
+        return self._login_page
+
+    @property
     def credentials(self) -> Dict:
         """Return the credentials object."""
+        if self._credentials is None:
+            raise ValueError("Credentials have not been set.")
         return self._credentials
 
     @classmethod
     def reset_credentials(cls):
+        """Remove the cached credentials file."""
         if os.path.isfile(cls._credentials_file):
             os.remove(cls._credentials_file)
 
-    def _save_credentials(self, credentials: Dict):
+    def _save_credentials_to_file(self, credentials: Dict):
         """Save the credentials object to a file."""
         with open(self._credentials_file, "w") as outfile:
             json.dump(credentials, outfile)
 
-    def _try_to_load_credentials_file(self) -> Union[Dict, bool]:
-        """Try to load the cached credentials file."""
-        if not os.path.isfile(self._credentials_file):
+    @classmethod
+    def file_credentials_are_valid(cls) -> bool:
+        """Check if the cached credentials exist and are valid."""
+        if not os.path.isfile(cls._credentials_file):
             return False
 
-        with open(self._credentials_file, "rb") as infile:
+        with open(cls._credentials_file, "rb"):
             try:
-                credentials = json.load(infile)
+                credentials = cls._get_credentials_from_file()
                 expires_at = int(credentials["expires_at"])
             except (KeyError, ValueError):
-                os.remove(self._credentials_file)
+                os.remove(cls._credentials_file)
                 return False
 
             now = int(
                 (
-                    mktime(datetime.now().timetuple())
-                    + datetime.now().microsecond / 1000000.0
+                        mktime(datetime.now().timetuple())
+                        + datetime.now().microsecond / 1000000.0
                 )
             )  # utc timestamp
 
             if now > expires_at:
-                os.remove(self._credentials_file)
+                os.remove(cls._credentials_file)
                 return False
 
-            return credentials
+        return True
+
+    @classmethod
+    def _get_credentials_from_file(cls) -> Dict:
+        """Get user credentials from a cached file."""
+        with open(cls._credentials_file, "rb") as infile:
+            return json.load(infile)
 
     def _get_credentials_from_web(self) -> Dict:
         """Get user credentials from a web sign-in."""
         print("Please go here and authorize:")
-        print(self._authorization_base_url)
-
-        sleep(0.05)  # Workaround for input / print stream race condition
+        print(self.login_page, flush=True)
         response = input("\nCopy and past your credentials from the login page:\n")
 
         # Reformat response to dict
         credentials = dict(map(lambda x: x.split("="), response.split("&")))
         return credentials
```

### Comparing `hakai_api-1.3.0/hakai_api.egg-info/PKG-INFO` & `hakai_api-1.4.0/hakai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.3.0/setup.py` & `hakai_api-1.4.0/setup.py`

 * *Files identical despite different names*

