# Comparing `tmp/FixedFloatApi-1.0.2.tar.gz` & `tmp/FixedFloatApi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FixedFloatApi-1.0.2.tar", last modified: Tue May  2 22:50:38 2023, max compression
+gzip compressed data, was "dist/FixedFloatApi-1.0.3.tar", last modified: Wed May  3 17:11:16 2023, max compression
```

## Comparing `FixedFloatApi-1.0.2.tar` & `FixedFloatApi-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2834 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      293 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1060 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     2834 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1488 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/fixedfloatapi/
--rw-rw-r--   0 root         (0) root         (0)     1522 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/fixedfloatapi/FixedFloatAPI.py
--rw-rw-r--   0 root         (0) root         (0)       54 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/fixedfloatapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       79 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1017 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3279 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      293 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/FixedFloatApi.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1060 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     3279 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1822 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/fixedfloatapi/
+-rw-rw-r--   0 root         (0) root         (0)     1878 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/fixedfloatapi/FixedFloatAPI.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/fixedfloatapi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-05-03 17:11:16.000000 FixedFloatApi-1.0.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1024 2023-05-03 17:10:11.000000 FixedFloatApi-1.0.3/setup.py
```

### Comparing `FixedFloatApi-1.0.2/FixedFloatApi.egg-info/PKG-INFO` & `FixedFloatApi-1.0.3/FixedFloatApi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FixedFloatApi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
-Home-page: https://github.com/Jobians/FixedFloatApi
+Home-page: https://github.com/Jobians/FixedFloatApi-Python
 Author: JobiansTechie
 Author-email: jobianstechie@gmail.com
 License: MIT
 Description: ## Installation
         
         ```bash
         pip install FixedFloatApi
@@ -70,17 +70,30 @@
         
         # get a QR code for a trade
         qr_code = api.qr({
             'id': 'TESTID',
             'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
         })
         print(qr_code)
+        
+        # Make a custom API request
+        method = 'some_method'
+        data = {'param1': 'value1', 'param2': 'value2'}
+        response = api.custom_request(method, data)
+        print(response)
         ```
         
-        For more information, see the [API documentation](https://fixedfloat.com/api).
+        For more information, see the [API documentation](https://fixedfloat.com/api)
+        
+        
+        ## Support
+        
+        If you find my work helpful, you can support me by donating:
+        
+        [![Donate](https://img.shields.io/badge/Donate-Crypto-0070BA.svg)](https://cwallet.com/t/TE6A6KMV)
         
 Keywords: FixedFloat,Api,FixedFloat Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FixedFloatApi-1.0.2/LICENSE.txt` & `FixedFloatApi-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FixedFloatApi-1.0.2/PKG-INFO` & `FixedFloatApi-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FixedFloatApi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
-Home-page: https://github.com/Jobians/FixedFloatApi
+Home-page: https://github.com/Jobians/FixedFloatApi-Python
 Author: JobiansTechie
 Author-email: jobianstechie@gmail.com
 License: MIT
 Description: ## Installation
         
         ```bash
         pip install FixedFloatApi
@@ -70,17 +70,30 @@
         
         # get a QR code for a trade
         qr_code = api.qr({
             'id': 'TESTID',
             'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
         })
         print(qr_code)
+        
+        # Make a custom API request
+        method = 'some_method'
+        data = {'param1': 'value1', 'param2': 'value2'}
+        response = api.custom_request(method, data)
+        print(response)
         ```
         
-        For more information, see the [API documentation](https://fixedfloat.com/api).
+        For more information, see the [API documentation](https://fixedfloat.com/api)
+        
+        
+        ## Support
+        
+        If you find my work helpful, you can support me by donating:
+        
+        [![Donate](https://img.shields.io/badge/Donate-Crypto-0070BA.svg)](https://cwallet.com/t/TE6A6KMV)
         
 Keywords: FixedFloat,Api,FixedFloat Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FixedFloatApi-1.0.2/README.md` & `FixedFloatApi-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -62,10 +62,23 @@
 
 # get a QR code for a trade
 qr_code = api.qr({
     'id': 'TESTID',
     'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
 })
 print(qr_code)
+
+# Make a custom API request
+method = 'some_method'
+data = {'param1': 'value1', 'param2': 'value2'}
+response = api.custom_request(method, data)
+print(response)
 ```
 
-For more information, see the [API documentation](https://fixedfloat.com/api).
+For more information, see the [API documentation](https://fixedfloat.com/api)
+
+
+## Support
+
+If you find my work helpful, you can support me by donating:
+
+[![Donate](https://img.shields.io/badge/Donate-Crypto-0070BA.svg)](https://cwallet.com/t/TE6A6KMV)
```

### Comparing `FixedFloatApi-1.0.2/fixedfloatapi/FixedFloatAPI.py` & `FixedFloatApi-1.0.3/fixedfloatapi/FixedFloatAPI.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import hashlib
 import requests
+import hmac
 
 class FixedFloatApi:
     RESP_OK = 0
     TYPE_FIXED = 'fixed'
     TYPE_FLOAT = 'float'
 
     def __init__(self, key, secret):
@@ -13,35 +14,42 @@
 
     def sign(self, data):
         parts = []
         if isinstance(data, dict):
             for key, value in data.items():
                 parts.append(f'{key}={value}')
             data = '&'.join(parts)
-        return hashlib.sha256(data.encode('utf-8'), self.secret.encode('utf-8')).hexdigest()
+        return hmac.new(self.secret.encode('utf-8'), data.encode('utf-8'), hashlib.sha256).hexdigest()
 
     def req(self, method, data):
         url = f'https://ff.io/api/v2/{method}'
 
         req = json.dumps(data)
 
         headers = {
             'Content-Type': 'application/json',
             'X-API-KEY': self.key,
             'X-API-SIGN': self.sign(req)
         }
 
         response = requests.post(url, headers=headers, data=req, verify=True)
 
-        result = response.json()
-        if result['code'] == self.RESP_OK:
-            return result['data']
-        else:
+        try:
+            result = response.json()
+        except ValueError:
+            raise Exception(f'Invalid JSON response: {response.content}')
+
+        if response.status_code != 200:
+            raise Exception(f'Request failed with status {response.status_code}: {result.get("msg", "")}')
+
+        if result['code'] != self.RESP_OK:
             raise Exception(result['msg'], result['code'])
 
+        return result['data']
+
     def ccies(self):
         return self.req('ccies', {})
 
     def price(self, data):
         return self.req('price', data)
 
     def create(self, data):
@@ -53,8 +61,11 @@
     def emergency(self, data):
         return self.req('emergency', data)
 
     def setEmail(self, data):
         return self.req('setEmail', data)
 
     def qr(self, data):
-        return self.req('qr', data)
+        return self.req('qr', data)
+
+    def custom_request(self, method, data):
+        return self.req(method, data)
```

### Comparing `FixedFloatApi-1.0.2/setup.py` & `FixedFloatApi-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FixedFloatApi',
     packages=find_packages(),
     include_package_data=True,
-    version='1.0.2',
+    version='1.0.3',
     license='MIT',
     description='Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='JobiansTechie',
     author_email='jobianstechie@gmail.com',
-    url='https://github.com/Jobians/FixedFloatApi',
+    url='https://github.com/Jobians/FixedFloatApi-Python',
     keywords=['FixedFloat', 'Api', 'FixedFloat Python'],
     install_requires=[
         'requests'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

