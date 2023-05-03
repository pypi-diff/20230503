# Comparing `tmp/simple_aws_ec2-0.1.2.tar.gz` & `tmp/simple_aws_ec2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.1.2.tar", last modified: Wed May  3 16:08:17 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.1.3.tar", last modified: Wed May  3 17:17:59 2023, max compression
```

## Comparing `simple_aws_ec2-0.1.2.tar` & `simple_aws_ec2-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:08:17.677765 simple_aws_ec2-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 16:08:17.677621 simple_aws_ec2-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3860 2023-05-03 16:06:52.000000 simple_aws_ec2-0.1.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-05-03 16:05:34.000000 simple_aws_ec2-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-05-03 14:53:32.000000 simple_aws_ec2-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 14:58:41.000000 simple_aws_ec2-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 16:08:17.677811 simple_aws_ec2-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:08:17.676267 simple_aws_ec2-0.1.2/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.1.2/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 16:06:59.000000 simple_aws_ec2-0.1.2/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      116 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.2/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:08:17.677036 simple_aws_ec2-0.1.2/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.2/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6560 2023-05-03 16:07:55.000000 simple_aws_ec2-0.1.2/simple_aws_ec2/ec2.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:08:17.676918 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 16:08:17.000000 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 16:08:17.000000 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 16:08:17.000000 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      257 2023-05-03 16:08:17.000000 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 16:08:17.000000 simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:08:17.677430 simple_aws_ec2-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3457 2023-05-03 15:15:52.000000 simple_aws_ec2-0.1.2/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.298587 simple_aws_ec2-0.1.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 17:17:59.298389 simple_aws_ec2-0.1.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3860 2023-05-03 16:06:52.000000 simple_aws_ec2-0.1.3/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      903 2023-05-03 17:17:41.000000 simple_aws_ec2-0.1.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-05-03 14:53:32.000000 simple_aws_ec2-0.1.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 14:58:41.000000 simple_aws_ec2-0.1.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 17:17:59.298642 simple_aws_ec2-0.1.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.1.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289245 simple_aws_ec2-0.1.3/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 17:17:00.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      116 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289972 simple_aws_ec2-0.1.3/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6621 2023-05-03 17:16:12.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289839 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      257 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.297126 simple_aws_ec2-0.1.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3457 2023-05-03 15:15:52.000000 simple_aws_ec2-0.1.3/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.1.2/LICENSE.txt` & `simple_aws_ec2-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.2/PKG-INFO` & `simple_aws_ec2-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_ec2
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.1.2/README.rst` & `simple_aws_ec2-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.2/release-history.rst` & `simple_aws_ec2-0.1.3/release-history.rst`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.3 (2023-05-03)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that when you describe ec2 instances with instance ids, we should not use any paginator configuration.
+
+
 0.1.2 (2023-05-04)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - rename ``Ec2InstanceIterproxy`` to ``Ec2InstanceIterProxy``.
```

### Comparing `simple_aws_ec2-0.1.2/requirements-doc.txt` & `simple_aws_ec2-0.1.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.2/setup.py` & `simple_aws_ec2-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.2/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.1.3/simple_aws_ec2/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,24 +150,25 @@
         filters: T.List[dict] = NOTHING,
         instance_ids: T.List[str] = NOTHING,
     ) -> "Ec2InstanceIterProxy":
         """ """
 
         def run():
             paginator = bsm.ec2_client.get_paginator("describe_instances")
-            response_iterator = paginator.paginate(
-                **resolve_kwargs(
-                    Filters=filters,
-                    InstanceIds=instance_ids,
-                    PaginationConfig={
-                        "MaxItems": 9999,
-                        "PageSize": 100,
-                    },
-                )
+            kwargs = resolve_kwargs(
+                Filters=filters,
+                InstanceIds=instance_ids,
+                PaginationConfig={
+                    "MaxItems": 9999,
+                    "PageSize": 100,
+                },
             )
+            if instance_ids is not NOTHING:
+                del kwargs["PaginationConfig"]
+            response_iterator = paginator.paginate(**kwargs)
             for response in response_iterator:
                 yield from cls._yield_dict_from_describe_instances_response(response)
 
         return Ec2InstanceIterProxy(run())
 
     @classmethod
     def from_id(cls, bsm: "BotoSesManager", inst_id: str) -> T.Optional["Ec2Instance"]:
```

### Comparing `simple_aws_ec2-0.1.2/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-ec2
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.1.2/tests/test_ec2.py` & `simple_aws_ec2-0.1.3/tests/test_ec2.py`

 * *Files identical despite different names*

