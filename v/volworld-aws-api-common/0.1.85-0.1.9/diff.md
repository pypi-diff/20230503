# Comparing `tmp/volworld_aws_api_common-0.1.85.tar.gz` & `tmp/volworld_aws_api_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volworld_aws_api_common-0.1.85.tar", last modified: Wed May  3 04:57:00 2023, max compression
+gzip compressed data, was "volworld_aws_api_common-0.1.9.tar", last modified: Thu Feb  2 06:18:11 2023, max compression
```

## Comparing `volworld_aws_api_common-0.1.85.tar` & `volworld_aws_api_common-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,41 @@
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/LICENSE.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/README.rst
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/setup.cfg
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      387 2023-05-03 04:56:58.000000 volworld_aws_api_common-0.1.85/setup.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.200876 volworld_aws_api_common-0.1.85/src/
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.200876 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.200876 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      158 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/AA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/Aws.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      222 2023-05-03 00:54:51.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      200 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/ErrorCode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/HttpStatus.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       99 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/ProjectModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      116 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/QueryModeType.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/url/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/url/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      654 2023-05-03 01:13:12.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/url/authUrl.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      156 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/ProjectMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      150 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/QueryMode.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       89 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/Url.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3403 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/UserPool.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/api/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      424 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/api/OAPI.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     3049 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/api/OpenApiValidation.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/api/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     2444 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/api/request_open_api_validation.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/ATestRequest.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/__init__.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1009 2023-05-03 01:11:34.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/get__current_user.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1557 2023-05-03 01:09:39.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/post__login.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1303 2023-05-03 01:09:26.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/post__signup.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      547 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/request_util.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      669 2023-05-03 04:56:52.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/url.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.204877 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/behave/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      118 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/behave/ACotA.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/behave/__init__.py
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     4729 2023-05-03 00:45:42.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/request.py
-drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-05-03 04:57:00.200876 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/
--rw-rw-r--   0 gobi      (1000) gobi      (1000)      251 2023-05-03 04:57:00.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/PKG-INFO
--rw-rw-r--   0 gobi      (1000) gobi      (1000)     1880 2023-05-03 04:57:00.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/SOURCES.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-05-03 04:57:00.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/dependency_links.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-05-03 04:57:00.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/requires.txt
--rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-05-03 04:57:00.000000 volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/top_level.txt
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1070 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.9/LICENSE.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       31 2023-01-31 04:59:04.000000 volworld_aws_api_common-0.1.9/README.rst
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       38 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/setup.cfg
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      386 2023-02-02 06:18:08.000000 volworld_aws_api_common-0.1.9/setup.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:33.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      225 2023-02-02 02:33:23.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/AA.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       76 2023-02-01 01:40:45.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/Aws.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:23:59.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      859 2023-02-02 01:14:00.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/HttpStatus.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 01:05:27.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:32:05.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      429 2023-02-02 06:15:34.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/url/authUrl.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:24:05.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      146 2023-01-31 08:23:17.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/ATestRequest.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:25:50.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/__init__.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 02:25:47.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      750 2023-02-02 02:31:42.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      759 2023-02-02 02:31:35.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/act/act__signup_login.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        0 2023-02-02 00:30:46.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/__init__.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      708 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/get__current_user.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      939 2023-02-02 01:39:09.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__login.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      901 2023-02-02 01:35:45.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/post__signup.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      482 2023-02-02 06:17:48.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/url.py
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     4243 2023-02-02 01:36:03.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/request.py
+drwxrwxr-x   0 gobi      (1000) gobi      (1000)        0 2023-02-02 06:18:11.471278 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)      250 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/PKG-INFO
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)     1291 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)        1 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       22 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/requires.txt
+-rw-rw-r--   0 gobi      (1000) gobi      (1000)       24 2023-02-02 06:18:11.000000 volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/top_level.txt
```

### Comparing `volworld_aws_api_common-0.1.85/LICENSE.txt` & `volworld_aws_api_common-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/api/enum/HttpStatus.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/api/enum/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/aws/request/get__current_user.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/aws/request/get__current_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from volworld_aws_api_common.api.AA import AA
 from volworld_aws_api_common.api.url import authUrl
 from volworld_aws_api_common.test.aws.ATestRequest import ATestRequest
 from volworld_aws_api_common.test.request import get_request
-from volworld_aws_api_common.test.aws.request.request_util import response_to_dict
-from volworld_aws_api_common.api.enum.HttpStatus import HttpStatus
+
 
 def get__current_user(
         req: ATestRequest,
-        att_list,
         token: str = None):
     resp_json, resp = get_request(
-        authUrl.current_user_url(), req, att_list,
+        authUrl.currentUserUrl, req,
         token=token)
-    return response_to_dict(resp_json, resp)
 
-def act__current_user(att_list, token: str = None) -> dict:
-    resp = get__current_user(ATestRequest(True), att_list, token)
-    assert resp[AA.HttpStatus] == HttpStatus.Ok_200
-    return resp
+    data = None
+    error = None
+
+    if AA.___Error___ in resp_json.keys():
+        error = resp_json[AA.___Error___]
+    else:
+        data = resp_json[AA.Data]
 
-def act__current_user___error(att_list, token: str = None) -> dict:
-    resp = get__current_user(ATestRequest(True), att_list, token)
-    assert AA.___Error___ in resp
-    return resp
+    return {
+        AA.Data: data,
+        AA.___Error___: error,
+        AA.HttpStatus: resp.status_code,
+        AA.Response: resp
+    }
```

### Comparing `volworld_aws_api_common-0.1.85/src/volworld_aws_api_common/test/request.py` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common/test/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,141 +1,133 @@
 import json
 import requests
 from requests import Response
 
 from volworld_common.api import CA
 from volworld_common.test.Timer import Timer
-from volworld_common.util.json import print_json_by_attributes
 
 from volworld_aws_api_common.test.aws.ATestRequest import ATestRequest
 
 APP_HEADER = {
     'Content-Type': 'application/json',
     'X-Requested-With': 'XMLHttpRequest',
-    'Accept': 'application/json',
-    'Accept-Encoding': 'deflate, gzip'}
+    'Accept': 'application/json'}
 
 
 def auth_header(token: str):
     return {
         # 'Authorization': token,  # self.token_type_ + " " + self.token_,
-        # 'AuthorizeToken': token,
-        'Authorization': f"Bearer {token}",
-        'Accept': 'application/json',
-        'Accept-Encoding': 'gzip, deflate'
+        'AuthorizeToken': token,
+        'Accept': 'application/json'
     }
 
 
-# def print_json(j, print_long_att: bool = False):
-#     if not print_long_att:
-#         print(json.dumps(j, indent=4, sort_keys=True))
-#         return
-#
-#     abb_att = dict()
-#     for name in CA.__dict__:
-#         abb = CA.__dict__[name]
-#         abb_att[f"\"{abb}\":"] = f"\"{abb}__{name}\":"
-#     res = json.dumps(j, indent=4, sort_keys=True)
-#     for att in abb_att.keys():
-#         res = res.replace(att, abb_att[att])
-#     print(res)
+def print_json(j, print_long_att: bool = False):
+    if not print_long_att:
+        print(json.dumps(j, indent=4, sort_keys=True))
+        return
+
+    abb_att = dict()
+    for name in CA.__dict__:
+        abb = CA.__dict__[name]
+        abb_att[f"\"{abb}\":"] = f"\"{abb}__{name}\":"
+    res = json.dumps(j, indent=4, sort_keys=True)
+    for att in abb_att.keys():
+        res = res.replace(att, abb_att[att])
+    print(res)
 
 
-def post_url(url: str, post_j: dict, attList,
+def post_url(url: str, post_j: dict,
              print_url_params: bool = True,
              print_long_att: bool = True,
              # status_code: int = -1,
              headers: dict = None) -> (dict, Response):
-    print('[post_url] print_long_att = ', print_long_att)
     if headers is None:
         headers = APP_HEADER
     if print_url_params:
         print(f'==== [Url] [{url}] ====')
         print('=== POST ===')
         print('<code>')
-        print_json_by_attributes(post_j, attList, print_long_att)
+        print_json(post_j, print_long_att)
         print('</code>')
     session = requests.Session()
     print('[post_url] session = ', session.cookies.get_dict())
-    print('[post_url] req headers = ', headers)
     resp = requests.post(url, headers=headers, json=post_j)
     print(f'[post_url] resp headers = {resp.headers}')
     print(f'[post_url] resp = {resp.text}')
     resp_json = resp.json()
     if print_url_params:
         print('=== Response ===')
         print('<code>')
-        print_json_by_attributes(resp_json, attList, print_long_att)
+        print_json(resp_json, print_long_att)
         print('</code>')
     # if status_code > 0:
     #     assert(resp.status_code == status_code), resp.status_code
     print('[post_url] session.cookies = ', session.cookies.get_dict())
     return resp_json, resp
 
 
 def post_request(
         url: str,
         post_j: dict,
         req: ATestRequest,
-        attList,
         token: str = None) -> (dict, Response):
     headers = None
     if token is not None:
         headers = auth_header(token)
     with Timer(url):
-        return post_url(url, post_j, attList,
+        return post_url(url, post_j,
                         print_url_params=req.print_url_params,
                         print_long_att=req.print_long_att,
                         # status_code=status_code,
                         headers=headers)
 
 
-def get_url(url: str, attList, params=None, cookies: dict = None,
+def get_url(url: str, params=None, cookies: dict = None,
             print_url_params: bool = True,
             print_long_att: bool = True,
             headers: dict = None) -> (dict, Response):
     if headers is None:
         headers = APP_HEADER
     if params is None:
         params = dict()
     if print_url_params:
         print(f'==== [Url] [{url}] ====')
         print('=== GET ===')
         print('<code>')
-        print_json_by_attributes(params, attList, print_long_att)
+        print_json(params, print_long_att)
         print('</code>')
     session = requests.Session()
     print('[get_url] session = ', session.cookies.get_dict())
     print('[get_url] cookies = ', cookies)
 
     resp = requests.get(url, headers=headers, params=params, cookies=cookies)
     print(f'[get_url] resp headers = {resp.headers}')
     print(f'[get_url] resp = {resp.text}')
     resp_json = resp.json()
     if print_url_params:
         print('=== Response ===')
         print('<code>')
-        print_json_by_attributes(resp_json, attList, print_long_att)
+        print_json(resp_json, print_long_att)
         print('</code>')
     # if status_code > 0:
     #     assert(resp.status_code == status_code), resp.status_code
     print('[get_url] session = ', session.cookies.get_dict())
     return resp_json, resp
 
 
 def get_request(
         url: str,
         req: ATestRequest,
-        attList,
         params: dict = None,
         cookies: dict = None,
         token: str = None) -> (dict, Response):
     headers = None
     if token is not None:
         headers = auth_header(token)
     with Timer(url):
         if params is None:
             params = dict()
-        return get_url(url, attList, params, cookies,
+        return get_url(url, params, cookies,
                        print_url_params=req.print_url_params,
                        print_long_att=req.print_long_att,
                        headers=headers)
```

### Comparing `volworld_aws_api_common-0.1.85/src/volworld_aws_api_common.egg-info/SOURCES.txt` & `volworld_aws_api_common-0.1.9/src/volworld_aws_api_common.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,24 @@
 src/volworld_aws_api_common.egg-info/PKG-INFO
 src/volworld_aws_api_common.egg-info/SOURCES.txt
 src/volworld_aws_api_common.egg-info/dependency_links.txt
 src/volworld_aws_api_common.egg-info/requires.txt
 src/volworld_aws_api_common.egg-info/top_level.txt
 src/volworld_aws_api_common/api/AA.py
 src/volworld_aws_api_common/api/Aws.py
-src/volworld_aws_api_common/api/Url.py
 src/volworld_aws_api_common/api/__init__.py
-src/volworld_aws_api_common/api/enum/ErrorCode.py
 src/volworld_aws_api_common/api/enum/HttpStatus.py
-src/volworld_aws_api_common/api/enum/ProjectModeType.py
-src/volworld_aws_api_common/api/enum/QueryModeType.py
 src/volworld_aws_api_common/api/enum/__init__.py
 src/volworld_aws_api_common/api/url/__init__.py
 src/volworld_aws_api_common/api/url/authUrl.py
-src/volworld_aws_api_common/test/ProjectMode.py
-src/volworld_aws_api_common/test/QueryMode.py
-src/volworld_aws_api_common/test/Url.py
-src/volworld_aws_api_common/test/UserPool.py
 src/volworld_aws_api_common/test/__init__.py
 src/volworld_aws_api_common/test/request.py
-src/volworld_aws_api_common/test/api/OAPI.py
-src/volworld_aws_api_common/test/api/OpenApiValidation.py
-src/volworld_aws_api_common/test/api/__init__.py
-src/volworld_aws_api_common/test/api/request_open_api_validation.py
 src/volworld_aws_api_common/test/aws/ATestRequest.py
 src/volworld_aws_api_common/test/aws/__init__.py
 src/volworld_aws_api_common/test/aws/url.py
+src/volworld_aws_api_common/test/aws/act/__init__.py
+src/volworld_aws_api_common/test/aws/act/act__signup.py
+src/volworld_aws_api_common/test/aws/act/act__signup_login.py
 src/volworld_aws_api_common/test/aws/request/__init__.py
 src/volworld_aws_api_common/test/aws/request/get__current_user.py
 src/volworld_aws_api_common/test/aws/request/post__login.py
-src/volworld_aws_api_common/test/aws/request/post__signup.py
-src/volworld_aws_api_common/test/aws/request/request_util.py
-src/volworld_aws_api_common/test/behave/ACotA.py
-src/volworld_aws_api_common/test/behave/__init__.py
+src/volworld_aws_api_common/test/aws/request/post__signup.py
```

