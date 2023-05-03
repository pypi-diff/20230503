# Comparing `tmp/capsolver_api-1.0.5.tar.gz` & `tmp/capsolver_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver_api-1.0.5.tar", last modified: Wed May  3 19:35:43 2023, max compression
+gzip compressed data, was "capsolver_api-1.0.6.tar", last modified: Wed May  3 19:57:18 2023, max compression
```

## Comparing `capsolver_api-1.0.5.tar` & `capsolver_api-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.101352 capsolver_api-1.0.5/
--rw-rw-rw-   0        0        0     1083 2023-04-11 20:44:23.000000 capsolver_api-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2711 2023-05-03 19:35:43.100343 capsolver_api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1998 2023-05-03 19:33:40.000000 capsolver_api-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.077056 capsolver_api-1.0.5/capsolver_api/
--rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.5/capsolver_api/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.5/capsolver_api/capsolver_api.py
--rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.5/capsolver_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.089058 capsolver_api-1.0.5/capsolver_api/recognitions/
--rw-rw-rw-   0        0        0     1055 2023-05-03 19:31:36.000000 capsolver_api-1.0.5/capsolver_api/recognitions/aws_waf.py
--rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:22.000000 capsolver_api-1.0.5/capsolver_api/recognitions/funcaptcha.py
--rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:21.000000 capsolver_api-1.0.5/capsolver_api/recognitions/hcaptcha.py
--rw-rw-rw-   0        0        0     1302 2023-05-03 19:31:41.000000 capsolver_api-1.0.5/capsolver_api/recognitions/image_to_task.py
--rw-rw-rw-   0        0        0     1008 2023-05-03 19:31:43.000000 capsolver_api-1.0.5/capsolver_api/recognitions/recaptcha.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.099343 capsolver_api-1.0.5/capsolver_api/tasks/
--rw-rw-rw-   0        0        0     1280 2023-05-03 19:32:15.000000 capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_challenge.py
--rw-rw-rw-   0        0        0     1281 2023-05-03 19:32:09.000000 capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_turnstile.py
--rw-rw-rw-   0        0        0     1303 2023-05-03 19:32:13.000000 capsolver_api-1.0.5/capsolver_api/tasks/datadome.py
--rw-rw-rw-   0        0        0     1545 2023-05-03 19:31:51.000000 capsolver_api-1.0.5/capsolver_api/tasks/funcaptcha.py
--rw-rw-rw-   0        0        0     1875 2023-05-03 19:31:53.000000 capsolver_api-1.0.5/capsolver_api/tasks/geetest.py
--rw-rw-rw-   0        0        0     2048 2023-05-03 19:31:55.000000 capsolver_api-1.0.5/capsolver_api/tasks/hcaptcha.py
--rw-rw-rw-   0        0        0     1251 2023-05-03 19:31:57.000000 capsolver_api-1.0.5/capsolver_api/tasks/mtcaptcha.py
--rw-rw-rw-   0        0        0     2057 2023-05-03 19:31:58.000000 capsolver_api-1.0.5/capsolver_api/tasks/recaptchav2.py
--rw-rw-rw-   0        0        0     2147 2023-05-03 19:32:00.000000 capsolver_api-1.0.5/capsolver_api/tasks/recaptchav3.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.083057 capsolver_api-1.0.5/capsolver_api.egg-info/
--rw-rw-rw-   0        0        0     2711 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 19:35:43.101352 capsolver_api-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-05-03 19:33:08.000000 capsolver_api-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:57:18.547038 capsolver_api-1.0.6/
+-rw-rw-rw-   0        0        0     1083 2023-04-11 20:44:23.000000 capsolver_api-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2711 2023-05-03 19:57:18.547038 capsolver_api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1998 2023-05-03 19:33:40.000000 capsolver_api-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 19:57:18.522716 capsolver_api-1.0.6/capsolver_api/
+-rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.6/capsolver_api/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.6/capsolver_api/capsolver_api.py
+-rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.6/capsolver_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:57:18.534229 capsolver_api-1.0.6/capsolver_api/recognitions/
+-rw-rw-rw-   0        0        0     1055 2023-05-03 19:31:36.000000 capsolver_api-1.0.6/capsolver_api/recognitions/aws_waf.py
+-rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:22.000000 capsolver_api-1.0.6/capsolver_api/recognitions/funcaptcha.py
+-rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:21.000000 capsolver_api-1.0.6/capsolver_api/recognitions/hcaptcha.py
+-rw-rw-rw-   0        0        0     1302 2023-05-03 19:31:41.000000 capsolver_api-1.0.6/capsolver_api/recognitions/image_to_task.py
+-rw-rw-rw-   0        0        0     1008 2023-05-03 19:31:43.000000 capsolver_api-1.0.6/capsolver_api/recognitions/recaptcha.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:57:18.545029 capsolver_api-1.0.6/capsolver_api/tasks/
+-rw-rw-rw-   0        0        0     1280 2023-05-03 19:32:15.000000 capsolver_api-1.0.6/capsolver_api/tasks/cloudflare_challenge.py
+-rw-rw-rw-   0        0        0     1281 2023-05-03 19:32:09.000000 capsolver_api-1.0.6/capsolver_api/tasks/cloudflare_turnstile.py
+-rw-rw-rw-   0        0        0     1303 2023-05-03 19:32:13.000000 capsolver_api-1.0.6/capsolver_api/tasks/datadome.py
+-rw-rw-rw-   0        0        0     1688 2023-05-03 19:56:20.000000 capsolver_api-1.0.6/capsolver_api/tasks/funcaptcha.py
+-rw-rw-rw-   0        0        0     1875 2023-05-03 19:31:53.000000 capsolver_api-1.0.6/capsolver_api/tasks/geetest.py
+-rw-rw-rw-   0        0        0     2048 2023-05-03 19:31:55.000000 capsolver_api-1.0.6/capsolver_api/tasks/hcaptcha.py
+-rw-rw-rw-   0        0        0     1251 2023-05-03 19:31:57.000000 capsolver_api-1.0.6/capsolver_api/tasks/mtcaptcha.py
+-rw-rw-rw-   0        0        0     2057 2023-05-03 19:31:58.000000 capsolver_api-1.0.6/capsolver_api/tasks/recaptchav2.py
+-rw-rw-rw-   0        0        0     2147 2023-05-03 19:32:00.000000 capsolver_api-1.0.6/capsolver_api/tasks/recaptchav3.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:57:18.528226 capsolver_api-1.0.6/capsolver_api.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-05-03 19:57:18.000000 capsolver_api-1.0.6/capsolver_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-05-03 19:57:18.000000 capsolver_api-1.0.6/capsolver_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 19:57:18.000000 capsolver_api-1.0.6/capsolver_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 19:57:18.000000 capsolver_api-1.0.6/capsolver_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 19:57:18.000000 capsolver_api-1.0.6/capsolver_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 19:57:18.547038 capsolver_api-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-05-03 19:56:48.000000 capsolver_api-1.0.6/setup.py
```

### Comparing `capsolver_api-1.0.5/LICENSE` & `capsolver_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/PKG-INFO` & `capsolver_api-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: capsolver.com library for Python
 Home-page: https://github.com/seadhy/capsolver-api
 Author: seadhy
 Author-email: seadhy@protonmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/seadhy/capsolver-api#capsolver-api-for-python
 Project-URL: Source, https://github.com/seadhy/capsolver-api/tree/main/capsolver_api
```

### Comparing `capsolver_api-1.0.5/README.md` & `capsolver_api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/__init__.py` & `capsolver_api-1.0.6/capsolver_api/__init__.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/capsolver_api.py` & `capsolver_api-1.0.6/capsolver_api/capsolver_api.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/recognitions/aws_waf.py` & `capsolver_api-1.0.6/capsolver_api/recognitions/aws_waf.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/recognitions/funcaptcha.py` & `capsolver_api-1.0.6/capsolver_api/recognitions/funcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/recognitions/hcaptcha.py` & `capsolver_api-1.0.6/capsolver_api/recognitions/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/recognitions/image_to_task.py` & `capsolver_api-1.0.6/capsolver_api/recognitions/image_to_task.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/recognitions/recaptcha.py` & `capsolver_api-1.0.6/capsolver_api/recognitions/recaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_challenge.py` & `capsolver_api-1.0.6/capsolver_api/tasks/cloudflare_challenge.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_turnstile.py` & `capsolver_api-1.0.6/capsolver_api/tasks/cloudflare_turnstile.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/datadome.py` & `capsolver_api-1.0.6/capsolver_api/tasks/datadome.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/funcaptcha.py` & `capsolver_api-1.0.6/capsolver_api/tasks/funcaptcha.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,32 @@
 
     def create_task(self,
                     task_type: Literal['FunCaptchaTask', 'FunCaptchaTaskProxyLess'] = None,
                     website_url: str = None,
                     website_key: str = None,
                     api_js_subdomain: Optional[str] = None,
                     data: Optional[str] = None,
-                    proxy: Optional[str] = None
+                    proxy: Optional[str] = None,
+                    useragent: Optional[str] = None
                     ):
 
         if all((task_type, website_url, website_key)):
             payload = {
               "clientKey": self.client_key,
               "task": {
                 "type": task_type,
                 "websiteURL": website_url,
-                "websiteKey": website_key,
+                "websitePublicKey": website_key,
               }
             }
 
             payload['task'].update({'funcaptchaApiJSSubdomain': api_js_subdomain} if api_js_subdomain else {})
             payload['task'].update({'data': data} if data else {})
             payload['task'].update({'proxy': proxy} if proxy else {})
+            payload['task'].update({'userAgent': useragent} if useragent else {})
 
             create_task_req = self.make_request('/createTask', payload)
             if create_task_req.status_code == 200:
                 return create_task_req.json()['taskId']
             else:
                 print('Error: ' + create_task_req.text)
         else:
```

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/geetest.py` & `capsolver_api-1.0.6/capsolver_api/tasks/geetest.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/hcaptcha.py` & `capsolver_api-1.0.6/capsolver_api/tasks/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/mtcaptcha.py` & `capsolver_api-1.0.6/capsolver_api/tasks/mtcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/recaptchav2.py` & `capsolver_api-1.0.6/capsolver_api/tasks/recaptchav2.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api/tasks/recaptchav3.py` & `capsolver_api-1.0.6/capsolver_api/tasks/recaptchav3.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/capsolver_api.egg-info/PKG-INFO` & `capsolver_api-1.0.6/capsolver_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: capsolver.com library for Python
 Home-page: https://github.com/seadhy/capsolver-api
 Author: seadhy
 Author-email: seadhy@protonmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/seadhy/capsolver-api#capsolver-api-for-python
 Project-URL: Source, https://github.com/seadhy/capsolver-api/tree/main/capsolver_api
```

### Comparing `capsolver_api-1.0.5/capsolver_api.egg-info/SOURCES.txt` & `capsolver_api-1.0.6/capsolver_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.5/setup.py` & `capsolver_api-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 
 setup(
     name='capsolver_api',
-    version='1.0.5',
+    version='1.0.6',
     author='seadhy',
     author_email='seadhy@protonmail.com',
     description='capsolver.com library for Python',
     long_description=long_description,
     license="MIT",
     long_description_content_type='text/markdown',
     url='https://github.com/seadhy/capsolver-api',
```

