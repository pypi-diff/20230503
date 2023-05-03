# Comparing `tmp/simple_aws_rds-0.1.1.tar.gz` & `tmp/simple_aws_rds-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_rds-0.1.1.tar", last modified: Wed May  3 16:16:23 2023, max compression
+gzip compressed data, was "simple_aws_rds-0.1.2.tar", last modified: Wed May  3 17:20:20 2023, max compression
```

## Comparing `simple_aws_rds-0.1.1.tar` & `simple_aws_rds-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:16:23.564985 simple_aws_rds-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 16:16:23.564858 simple_aws_rds-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3657 2023-05-03 16:15:22.000000 simple_aws_rds-0.1.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      508 2023-05-03 16:10:13.000000 simple_aws_rds-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-03 15:59:50.000000 simple_aws_rds-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 15:36:24.000000 simple_aws_rds-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 16:16:23.565026 simple_aws_rds-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 15:36:40.000000 simple_aws_rds-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:16:23.563767 simple_aws_rds-0.1.1/simple_aws_rds/
--rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.1.1/simple_aws_rds/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 15:36:45.000000 simple_aws_rds-0.1.1/simple_aws_rds/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      122 2023-05-03 16:11:07.000000 simple_aws_rds-0.1.1/simple_aws_rds/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:16:23.564431 simple_aws_rds-0.1.1/simple_aws_rds/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.1/simple_aws_rds/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5969 2023-05-03 16:09:39.000000 simple_aws_rds-0.1.1/simple_aws_rds/rds.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:16:23.564319 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 16:16:23.000000 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 16:16:23.000000 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 16:16:23.000000 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-05-03 16:16:23.000000 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 16:16:23.000000 simple_aws_rds-0.1.1/simple_aws_rds.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 16:16:23.564691 simple_aws_rds-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.1.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2733 2023-05-03 16:16:00.000000 simple_aws_rds-0.1.1/tests/test_rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.413216 simple_aws_rds-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 17:20:20.413054 simple_aws_rds-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3657 2023-05-03 16:15:22.000000 simple_aws_rds-0.1.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      736 2023-05-03 17:19:59.000000 simple_aws_rds-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-03 15:59:50.000000 simple_aws_rds-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 15:36:24.000000 simple_aws_rds-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 17:20:20.413275 simple_aws_rds-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 15:36:40.000000 simple_aws_rds-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.409819 simple_aws_rds-0.1.2/simple_aws_rds/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.1.2/simple_aws_rds/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 17:19:02.000000 simple_aws_rds-0.1.2/simple_aws_rds/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      122 2023-05-03 16:11:07.000000 simple_aws_rds-0.1.2/simple_aws_rds/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.411908 simple_aws_rds-0.1.2/simple_aws_rds/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/simple_aws_rds/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6040 2023-05-03 17:18:56.000000 simple_aws_rds-0.1.2/simple_aws_rds/rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.411754 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.412560 simple_aws_rds-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.1.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2733 2023-05-03 16:16:00.000000 simple_aws_rds-0.1.2/tests/test_rds.py
```

### Comparing `simple_aws_rds-0.1.1/LICENSE.txt` & `simple_aws_rds-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.1/PKG-INFO` & `simple_aws_rds-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_rds
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.1.1/README.rst` & `simple_aws_rds-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.1/requirements-doc.txt` & `simple_aws_rds-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.1/setup.py` & `simple_aws_rds-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.1/simple_aws_rds/rds.py` & `simple_aws_rds-0.1.2/simple_aws_rds/rds.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,24 +116,25 @@
         cls,
         bsm: "BotoSesManager",
         db_instance_identifier: str = NOTHING,
         filters: T.List[dict] = NOTHING,
     ) -> "RDSDBInstanceIterProxy":
         def run():
             paginator = bsm.rds_client.get_paginator("describe_db_instances")
-            response_iterator = paginator.paginate(
-                **resolve_kwargs(
-                    DBInstanceIdentifier=db_instance_identifier,
-                    Filters=filters,
-                    PaginationConfig={
-                        "MaxItems": 9999,
-                        "PageSize": 100,
-                    },
-                )
+            kwargs = resolve_kwargs(
+                DBInstanceIdentifier=db_instance_identifier,
+                Filters=filters,
+                PaginationConfig={
+                    "MaxItems": 9999,
+                    "PageSize": 100,
+                },
             )
+            if db_instance_identifier is not NOTHING:
+                del kwargs["PaginationConfig"]
+            response_iterator = paginator.paginate(**kwargs)
             for response in response_iterator:
                 yield from cls._yield_dict_from_describe_db_instances_response(response)
 
         return RDSDBInstanceIterProxy(run())
 
     @classmethod
     def from_id(
```

### Comparing `simple_aws_rds-0.1.1/simple_aws_rds.egg-info/PKG-INFO` & `simple_aws_rds-0.1.2/simple_aws_rds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-rds
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.1.1/tests/test_rds.py` & `simple_aws_rds-0.1.2/tests/test_rds.py`

 * *Files identical despite different names*

