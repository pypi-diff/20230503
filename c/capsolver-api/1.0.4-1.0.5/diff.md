# Comparing `tmp/capsolver_api-1.0.4.tar.gz` & `tmp/capsolver_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver_api-1.0.4.tar", last modified: Sun Apr 16 22:07:41 2023, max compression
+gzip compressed data, was "capsolver_api-1.0.5.tar", last modified: Wed May  3 19:35:43 2023, max compression
```

## Comparing `capsolver_api-1.0.4.tar` & `capsolver_api-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/
--rw-rw-rw-   0        0        0     1083 2023-04-11 20:44:23.000000 capsolver_api-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2708 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-04-16 21:57:47.000000 capsolver_api-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.603962 capsolver_api-1.0.4/capsolver_api/
--rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.4/capsolver_api/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.4/capsolver_api/capsolver_api.py
--rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.4/capsolver_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.619413 capsolver_api-1.0.4/capsolver_api/recognitions/
--rw-rw-rw-   0        0        0     1054 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/aws_waf.py
--rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/funcaptcha.py
--rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/hcaptcha.py
--rw-rw-rw-   0        0        0     1301 2023-04-07 20:39:29.000000 capsolver_api-1.0.4/capsolver_api/recognitions/image_to_task.py
--rw-rw-rw-   0        0        0     1007 2023-04-08 09:37:59.000000 capsolver_api-1.0.4/capsolver_api/recognitions/recaptcha.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.634023 capsolver_api-1.0.4/capsolver_api/tasks/
--rw-rw-rw-   0        0        0     1279 2023-04-08 09:34:47.000000 capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_challenge.py
--rw-rw-rw-   0        0        0     1280 2023-04-08 09:33:49.000000 capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_turnstile.py
--rw-rw-rw-   0        0        0     1302 2023-04-08 09:34:38.000000 capsolver_api-1.0.4/capsolver_api/tasks/datadome.py
--rw-rw-rw-   0        0        0     1544 2023-04-08 09:34:31.000000 capsolver_api-1.0.4/capsolver_api/tasks/funcaptcha.py
--rw-rw-rw-   0        0        0     1874 2023-04-08 09:34:23.000000 capsolver_api-1.0.4/capsolver_api/tasks/geetest.py
--rw-rw-rw-   0        0        0     2047 2023-04-08 09:34:15.000000 capsolver_api-1.0.4/capsolver_api/tasks/hcaptcha.py
--rw-rw-rw-   0        0        0     1250 2023-04-08 09:34:09.000000 capsolver_api-1.0.4/capsolver_api/tasks/mtcaptcha.py
--rw-rw-rw-   0        0        0     2056 2023-04-08 09:34:03.000000 capsolver_api-1.0.4/capsolver_api/tasks/recaptchav2.py
--rw-rw-rw-   0        0        0     2146 2023-04-08 09:33:58.000000 capsolver_api-1.0.4/capsolver_api/tasks/recaptchav3.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.610409 capsolver_api-1.0.4/capsolver_api.egg-info/
--rw-rw-rw-   0        0        0     2708 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-04-16 22:06:09.000000 capsolver_api-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.101352 capsolver_api-1.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-04-11 20:44:23.000000 capsolver_api-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2711 2023-05-03 19:35:43.100343 capsolver_api-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1998 2023-05-03 19:33:40.000000 capsolver_api-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.077056 capsolver_api-1.0.5/capsolver_api/
+-rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.5/capsolver_api/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.5/capsolver_api/capsolver_api.py
+-rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.5/capsolver_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.089058 capsolver_api-1.0.5/capsolver_api/recognitions/
+-rw-rw-rw-   0        0        0     1055 2023-05-03 19:31:36.000000 capsolver_api-1.0.5/capsolver_api/recognitions/aws_waf.py
+-rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:22.000000 capsolver_api-1.0.5/capsolver_api/recognitions/funcaptcha.py
+-rw-rw-rw-   0        0        0     1063 2023-05-03 19:32:21.000000 capsolver_api-1.0.5/capsolver_api/recognitions/hcaptcha.py
+-rw-rw-rw-   0        0        0     1302 2023-05-03 19:31:41.000000 capsolver_api-1.0.5/capsolver_api/recognitions/image_to_task.py
+-rw-rw-rw-   0        0        0     1008 2023-05-03 19:31:43.000000 capsolver_api-1.0.5/capsolver_api/recognitions/recaptcha.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.099343 capsolver_api-1.0.5/capsolver_api/tasks/
+-rw-rw-rw-   0        0        0     1280 2023-05-03 19:32:15.000000 capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_challenge.py
+-rw-rw-rw-   0        0        0     1281 2023-05-03 19:32:09.000000 capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_turnstile.py
+-rw-rw-rw-   0        0        0     1303 2023-05-03 19:32:13.000000 capsolver_api-1.0.5/capsolver_api/tasks/datadome.py
+-rw-rw-rw-   0        0        0     1545 2023-05-03 19:31:51.000000 capsolver_api-1.0.5/capsolver_api/tasks/funcaptcha.py
+-rw-rw-rw-   0        0        0     1875 2023-05-03 19:31:53.000000 capsolver_api-1.0.5/capsolver_api/tasks/geetest.py
+-rw-rw-rw-   0        0        0     2048 2023-05-03 19:31:55.000000 capsolver_api-1.0.5/capsolver_api/tasks/hcaptcha.py
+-rw-rw-rw-   0        0        0     1251 2023-05-03 19:31:57.000000 capsolver_api-1.0.5/capsolver_api/tasks/mtcaptcha.py
+-rw-rw-rw-   0        0        0     2057 2023-05-03 19:31:58.000000 capsolver_api-1.0.5/capsolver_api/tasks/recaptchav2.py
+-rw-rw-rw-   0        0        0     2147 2023-05-03 19:32:00.000000 capsolver_api-1.0.5/capsolver_api/tasks/recaptchav3.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:35:43.083057 capsolver_api-1.0.5/capsolver_api.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 19:35:42.000000 capsolver_api-1.0.5/capsolver_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 19:35:43.101352 capsolver_api-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-05-03 19:33:08.000000 capsolver_api-1.0.5/setup.py
```

### Comparing `capsolver_api-1.0.4/LICENSE` & `capsolver_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.4/PKG-INFO` & `capsolver_api-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: capsolver.com library for Python
 Home-page: https://github.com/seadhy/capsolver-api
 Author: seadhy
 Author-email: seadhy@protonmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/seadhy/capsolver-api#capsolver-api-for-python
 Project-URL: Source, https://github.com/seadhy/capsolver-api/tree/main/capsolver_api
@@ -52,15 +52,15 @@
                                 website_key='a5f74b19-9e45-40e0-b45d-47ff91b7a6c2'
                                 )
 
 captcha_key = capsolver.get_solution(task_id)
 print(captcha_key)
 ````
 
-### Hcaptcha
+### RecaptchaV2
 ````python
 from capsolver_api import ReCaptchaV2Task
 
 
 capsolver = ReCaptchaV2Task('your_capsolver_api_key')
```

### Comparing `capsolver_api-1.0.4/README.md` & `capsolver_api-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                                 website_key='a5f74b19-9e45-40e0-b45d-47ff91b7a6c2'
                                 )
 
 captcha_key = capsolver.get_solution(task_id)
 print(captcha_key)
 ````
 
-### Hcaptcha
+### RecaptchaV2
 ````python
 from capsolver_api import ReCaptchaV2Task
 
 
 capsolver = ReCaptchaV2Task('your_capsolver_api_key')
 
 
@@ -58,8 +58,8 @@
 
 ### And others:
 - Cloudflare (Turnstile / Challenge)
 - Datadome
 - Geetest
 - Mtcaptcha
 - Other recognitions
-- More information for [docs](https://docs.capsolver.com/guide/getting-started.html)
+- More information for [docs](https://docs.capsolver.com/guide/getting-started.html)
```

### Comparing `capsolver_api-1.0.4/capsolver_api/__init__.py` & `capsolver_api-1.0.5/capsolver_api/__init__.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.4/capsolver_api/capsolver_api.py` & `capsolver_api-1.0.5/capsolver_api/capsolver_api.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.4/capsolver_api/recognitions/aws_waf.py` & `capsolver_api-1.0.5/capsolver_api/recognitions/aws_waf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class AwsWafClassification(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key)
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/recognitions/funcaptcha.py` & `capsolver_api-1.0.5/capsolver_api/recognitions/funcaptcha.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class FunCaptchaClassification(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key)
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/recognitions/hcaptcha.py` & `capsolver_api-1.0.5/capsolver_api/recognitions/hcaptcha.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class HCaptchaClassification(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key)
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/recognitions/image_to_task.py` & `capsolver_api-1.0.5/capsolver_api/recognitions/image_to_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class ImageToTextTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key)
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/recognitions/recaptcha.py` & `capsolver_api-1.0.5/capsolver_api/recognitions/recaptcha.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class ReCaptchaClassification(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key)
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_challenge.py` & `capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class CloudflareChallengeTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'Cloudflare')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_turnstile.py` & `capsolver_api-1.0.5/capsolver_api/tasks/cloudflare_turnstile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class CloudflareTurnstileTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'Cloudflare')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/datadome.py` & `capsolver_api-1.0.5/capsolver_api/tasks/datadome.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class DatadomeTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'Datadome')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/funcaptcha.py` & `capsolver_api-1.0.5/capsolver_api/tasks/funcaptcha.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class FunCaptchaTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'FunCaptcha')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/geetest.py` & `capsolver_api-1.0.5/capsolver_api/tasks/geetest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class GeeTestTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'GeeTest')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/hcaptcha.py` & `capsolver_api-1.0.5/capsolver_api/tasks/hcaptcha.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class HCaptchaTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'HCaptcha')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/mtcaptcha.py` & `capsolver_api-1.0.5/capsolver_api/tasks/mtcaptcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class MtCaptchaTask(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'MtCaptcha')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/recaptchav2.py` & `capsolver_api-1.0.5/capsolver_api/tasks/recaptchav2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class ReCaptchaV2Task(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'ReCaptcha')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api/tasks/recaptchav3.py` & `capsolver_api-1.0.5/capsolver_api/tasks/recaptchav3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Literal
-from ..capsolver_py import Capsolver
+from ..capsolver_api import Capsolver
 
 
 class ReCaptchaV3Task(Capsolver):
     def __init__(self, client_key: str):
         super().__init__(client_key, 'ReCaptcha')
 
     def create_task(self,
```

### Comparing `capsolver_api-1.0.4/capsolver_api.egg-info/PKG-INFO` & `capsolver_api-1.0.5/capsolver_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: capsolver.com library for Python
 Home-page: https://github.com/seadhy/capsolver-api
 Author: seadhy
 Author-email: seadhy@protonmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/seadhy/capsolver-api#capsolver-api-for-python
 Project-URL: Source, https://github.com/seadhy/capsolver-api/tree/main/capsolver_api
@@ -52,15 +52,15 @@
                                 website_key='a5f74b19-9e45-40e0-b45d-47ff91b7a6c2'
                                 )
 
 captcha_key = capsolver.get_solution(task_id)
 print(captcha_key)
 ````
 
-### Hcaptcha
+### RecaptchaV2
 ````python
 from capsolver_api import ReCaptchaV2Task
 
 
 capsolver = ReCaptchaV2Task('your_capsolver_api_key')
```

### Comparing `capsolver_api-1.0.4/capsolver_api.egg-info/SOURCES.txt` & `capsolver_api-1.0.5/capsolver_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.4/setup.py` & `capsolver_api-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 
 setup(
     name='capsolver_api',
-    version='1.0.4',
+    version='1.0.5',
     author='seadhy',
     author_email='seadhy@protonmail.com',
     description='capsolver.com library for Python',
     long_description=long_description,
     license="MIT",
     long_description_content_type='text/markdown',
     url='https://github.com/seadhy/capsolver-api',
```

