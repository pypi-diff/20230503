# Comparing `tmp/eniris-0.3.3.tar.gz` & `tmp/eniris-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.3.3.tar", last modified: Tue Apr 18 11:50:11 2023, max compression
+gzip compressed data, was "eniris-0.4.0.tar", last modified: Wed May  3 12:16:05 2023, max compression
```

## Comparing `eniris-0.3.3.tar` & `eniris-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 11:50:00.000000 eniris-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-18 11:50:11.643923 eniris-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-18 11:50:00.000000 eniris-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-18 11:50:00.000000 eniris-0.3.3/eniris/ApiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:50:00.000000 eniris-0.3.3/eniris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:50:11.643923 eniris-0.3.3/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 11:50:11.000000 eniris-0.3.3/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:50:11.643923 eniris-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 11:50:00.000000 eniris-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-03 12:15:51.000000 eniris-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-03 12:16:05.508996 eniris-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-03 12:15:51.000000 eniris-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-03 12:15:51.000000 eniris-0.4.0/eniris/ApiDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:15:51.000000 eniris-0.4.0/eniris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:16:05.508996 eniris-0.4.0/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:16:05.000000 eniris-0.4.0/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:16:05.508996 eniris-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-03 12:15:51.000000 eniris-0.4.0/setup.py
```

### Comparing `eniris-0.3.3/LICENSE` & `eniris-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.3.3/PKG-INFO` & `eniris-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.3.3
+Version: 0.4.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `eniris-0.3.3/README.md` & `eniris-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.3.3/eniris/ApiDriver.py` & `eniris-0.4.0/eniris/ApiDriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+from typing import Union, Callable
 import datetime
 import requests
 import logging
 import time
+from http import HTTPStatus
 
 class AuthenticationFailure(Exception):
     "Raised when failing to authentiate to the Insights API"
     pass
-    
-class RetryFailure(Exception):
-    "Raised when authentication was succesful, an API call failed repeatedly"
-    pass
+
+def checkRetryCondition(response: requests.Response) -> bool:
+  """ Checks a HTTP response for status codes that indicate a temporary fault condition. Mainly responses that indicate a temporary server failure. For these conditions it makes sense to retry the HTTP request later.
+  
+  Args:
+    response (requests.Response)
+
+  Returns:
+    bool: True if the HTTP response contains an error status code that corresponds with a temporary server failure.
+  """
+  RETRY_STATUS_CODES = {
+    HTTPStatus.TOO_MANY_REQUESTS,
+    HTTPStatus.INTERNAL_SERVER_ERROR,
+    HTTPStatus.SERVICE_UNAVAILABLE
+  }
+  return response.status_code in RETRY_STATUS_CODES
+
 
 # Provide an easy interface to interact with the API, in the style of the requests library (https://docs.python-requests.org/en/master/)
 class ApiDriver:
   def __init__(self, username:str, password:str, authUrl:str = 'https://authentication.eniris.be', apiUrl:str = 'https://api.eniris.be', timeoutS:int = 60, maximumRetries:int = 4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60):
     """Constructor. You must specify at least username and password or a credentialsPath where they are stored as a json of the form {'login': USERNAME, 'password': PASSWORD}
 
     Args:
@@ -71,101 +86,91 @@
     resp = requests.post(self.authUrl + '/auth/logout', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
     if resp.status_code == 204 or resp.status_code == 401:
       # The refresh token was either succesfully added to the deny list, or it was already invalid
       self.refreshDtAndToken = None
       self.accessDtAndToken = None 
     else:
       raise AuthenticationFailure("logout failed: " + resp.text)
+  
+  def __retry(self, requests_function:Callable, path:str, retryNr = 0, **req_function_kwargs) -> requests.Response:
+    """Execute the given requests_function with the provided req_function_kwargs keyword arguments. If the function fails, it will try again until the amount of retries has exceeded.
+
+    Args:
+        requests_function (Callable): Requests function to use. Can be requests.get, requests.post, requests.put or requests.delete
+        path (str): Path relative to the apiUrl.
+        retryNr (int, optional): How often the call has been tried already. Defaults to 0.
+        req_function_kwargs (dict): Keyword arguments for the requests_function.
+
+    Returns:
+        requests.Response: HTTP response
+    """
+    req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
+    try:
+      resp = requests_function(req_path, **req_function_kwargs)
+    except requests.Timeout as e:
+      resp = e
+    if isinstance(resp, requests.Timeout):
+      if retryNr+1 <= self.maximumRetries:
+        logging.warning("Retrying API call after timeout.")
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        resp = self.__retry(requests_function, path, retryNr+1, **req_function_kwargs)
+      else:
+        raise requests.Timeout(resp)
+    elif (checkRetryCondition(resp)) and retryNr+1 <= self.maximumRetries:
+        logging.warning(f'Retrying API call after response with status code {resp.status_code} ({HTTPStatus(resp.status_code).phrase}): {resp.text}')
+        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
+        resp = self.__retry(requests_function, path, retryNr+1, **req_function_kwargs)
+    return resp
       
-  def get(self, path:str, params = None, retryNr = 0) -> requests.Response:
+  def get(self, path:str, params = None, **kwargs) -> requests.Response:
     """API GET call
 
     Args:
         path (str): Path relative to the apiUrl.
         params (dict, optional): URL parameters. Defaults to None.
-        retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    try:
-      req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
-      return requests.get(req_path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
-    except Exception as e:
-      if retryNr+1 > self.maximumRetries:
-        raise RetryFailure()
-      else:
-        logging.debug("Retrying after unexpected exception: " + str(e))
-        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
-        return self.get(path, params, retryNr+1)
-  
-  def post(self, path:str, json = None, params = None, data = None, retryNr = 0) -> requests.Response:
-    """API POST call
+    return self.__retry(requests.get, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+
+  def post(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
+    """API POST call()
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
-        retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    try:
-      req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
-      return requests.post(req_path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
-    except Exception as e:
-      if retryNr+1 > self.maximumRetries:
-        raise RetryFailure()
-      else:
-        logging.debug("Retrying after unexpected exception: " + str(e))
-        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
-        return self.post(path, json, params, data, retryNr+1)
+    return self.__retry(requests.post, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
     
-  def put(self, path:str, json = None, params = None, data = None, retryNr = 0) -> requests.Response:
+  def put(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
     """API PUT call
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
-        retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    try:
-      req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
-      return requests.put(req_path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
-    except Exception as e:
-      if retryNr > self.maximumRetries:
-        raise RetryFailure()
-      else:
-        logging.debug("Retrying after unexpected exception: " + str(e))
-        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
-        return self.put(path, json, params, data, retryNr+1)
+    return self.__retry(requests.put, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
   
-  def delete(self, path:str, params = None, retryNr = 0) -> requests.Response:
+  def delete(self, path:str, params = None, **kwargs) -> requests.Response:
     """API DELETE call
 
     Args:
         path (str): Path relative to the baseUrl.
         params (dict, optional): URL parameters. Defaults to None.
-        retryNr (int, optional): How often the call has been tried already. Defaults to 0.
 
     Returns:
         requests.Response: API call response
     """
     self._authenticate()
-    try:
-      req_path = path if path.startswith('http://') or path.startswith('https://') else self.apiUrl + path
-      return requests.delete(req_path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
-    except Exception as e:
-      if retryNr > self.maximumRetries:
-        raise RetryFailure()
-      else:
-        logging.debug("Retrying after unexpected exception: " + str(e))
-        time.sleep(min(self.initialRetryDelayS*2**retryNr, self.maximumRetryDelayS))
-        return self.delete(path, params, retryNr+1)
+    return self.__retry(requests.delete, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
```

### Comparing `eniris-0.3.3/eniris.egg-info/PKG-INFO` & `eniris-0.4.0/eniris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.3.3
+Version: 0.4.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `eniris-0.3.3/setup.py` & `eniris-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.3.3',
+  version = '0.4.0',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.3.3.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.4.0.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests',
   ],
   classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
   ],
 )
```

