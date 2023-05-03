# Comparing `tmp/chatapi-translate-0.1.tar.gz` & `tmp/chatapi-translate-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatapi-translate-0.1.tar", last modified: Wed May  3 07:07:34 2023, max compression
+gzip compressed data, was "chatapi-translate-0.2.tar", last modified: Wed May  3 07:12:38 2023, max compression
```

## Comparing `chatapi-translate-0.1.tar` & `chatapi-translate-0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:07:34.028806 chatapi-translate-0.1/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3204 2023-05-03 07:07:34.028806 chatapi-translate-0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:07:34.008807 chatapi-translate-0.1/chatapi_translate/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.1/chatapi_translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7638 2023-05-03 06:58:54.000000 chatapi-translate-0.1/chatapi_translate/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:07:34.028806 chatapi-translate-0.1/chatapi_translate/translator/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.1/chatapi_translate/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.1/chatapi_translate/translator/ali.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.1/chatapi_translate/translator/baidu.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.1/chatapi_translate/translator/caiyun.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.1/chatapi_translate/translator/chatgpt.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.1/chatapi_translate/translator/deepl.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.1/chatapi_translate/translator/google.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.1/chatapi_translate/translator/tencent.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.1/chatapi_translate/translator/utils.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.1/chatapi_translate/translator/volcengine.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-05-03 06:51:05.000000 chatapi-translate-0.1/chatapi_translate/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:07:34.028806 chatapi-translate-0.1/chatapi_translate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3204 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 07:07:33.000000 chatapi-translate-0.1/chatapi_translate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:07:34.028806 chatapi-translate-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1379 2023-05-03 07:06:24.000000 chatapi-translate-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:12:38.085749 chatapi-translate-0.2/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-05-03 07:12:38.085749 chatapi-translate-0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:12:38.085749 chatapi-translate-0.2/chatapi_translate/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.2/chatapi_translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7638 2023-05-03 06:58:54.000000 chatapi-translate-0.2/chatapi_translate/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:12:38.085749 chatapi-translate-0.2/chatapi_translate/translator/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.2/chatapi_translate/translator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.2/chatapi_translate/translator/ali.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.2/chatapi_translate/translator/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.2/chatapi_translate/translator/caiyun.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.2/chatapi_translate/translator/chatgpt.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.2/chatapi_translate/translator/deepl.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.2/chatapi_translate/translator/google.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.2/chatapi_translate/translator/tencent.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.2/chatapi_translate/translator/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.2/chatapi_translate/translator/volcengine.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-05-03 06:51:05.000000 chatapi-translate-0.2/chatapi_translate/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:12:38.085749 chatapi-translate-0.2/chatapi_translate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 07:12:38.000000 chatapi-translate-0.2/chatapi_translate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:12:38.085749 chatapi-translate-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-03 07:12:28.000000 chatapi-translate-0.2/setup.py
```

### Comparing `chatapi-translate-0.1/LICENSE` & `chatapi-translate-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/PKG-INFO` & `chatapi-translate-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.1
+Version: 0.2
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.1/chatapi_translate/api.py` & `chatapi-translate-0.2/chatapi_translate/api.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/__init__.py` & `chatapi-translate-0.2/chatapi_translate/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/ali.py` & `chatapi-translate-0.2/chatapi_translate/translator/ali.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/baidu.py` & `chatapi-translate-0.2/chatapi_translate/translator/baidu.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/caiyun.py` & `chatapi-translate-0.2/chatapi_translate/translator/caiyun.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/chatgpt.py` & `chatapi-translate-0.2/chatapi_translate/translator/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/deepl.py` & `chatapi-translate-0.2/chatapi_translate/translator/deepl.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/google.py` & `chatapi-translate-0.2/chatapi_translate/translator/google.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/tencent.py` & `chatapi-translate-0.2/chatapi_translate/translator/tencent.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/utils.py` & `chatapi-translate-0.2/chatapi_translate/translator/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/translator/volcengine.py` & `chatapi-translate-0.2/chatapi_translate/translator/volcengine.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate/utils.py` & `chatapi-translate-0.2/chatapi_translate/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/chatapi_translate.egg-info/PKG-INFO` & `chatapi-translate-0.2/chatapi_translate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.1
+Version: 0.2
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.1/chatapi_translate.egg-info/SOURCES.txt` & `chatapi-translate-0.2/chatapi_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.1/setup.py` & `chatapi-translate-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'code: https://github.com/aitsc/chatapi-translate'
 
 setup(
     name='chatapi-translate',
-    version='0.1',
+    version='0.2',
     description="ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='MIT',
     url='https://github.com/aitsc/chatapi-translate',
     keywords='tools',
@@ -26,20 +26,20 @@
     ],
     entry_points={
         'console_scripts': [
             'chatapi-translate=chatapi_translate.api:main',
         ],
     },
     install_requires=[
-        'fastapi>=0.95.1',
-        'uvicorn>=0.22.0',
-        'sse-starlette>=1.3.4',
-        'requests>=2.29.0',
-        'commentjson>=0.9.0',
-        'asyncio>=3.4.3',
-        'httpx>=0.24.0',
-        'aiohttp>=3.8.4',
-        'aiolimiter>=1.0.0',
-        'watchdog>=3.0.0',
+        'fastapi',
+        'uvicorn',
+        'sse-starlette',
+        'requests',
+        'commentjson',
+        'asyncio',
+        'httpx',
+        'aiohttp',
+        'aiolimiter',
+        'watchdog',
     ],
     python_requires='>=3.7',
 )
```

