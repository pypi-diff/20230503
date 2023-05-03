# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a2.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a2.tar", last modified: Wed Apr 26 23:42:17 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a3.tar", last modified: Wed May  3 03:59:55 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a2.tar` & `heaserver-trash-aws-s3-1.0.0a3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.870536 heaserver-trash-aws-s3-1.0.0a2/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-04-26 23:42:17.869459 heaserver-trash-aws-s3-1.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 23:42:17.870536 heaserver-trash-aws-s3-1.0.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-04-26 23:41:45.000000 heaserver-trash-aws-s3-1.0.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.817972 heaserver-trash-aws-s3-1.0.0a2/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.817972 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.841809 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    47506 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.843808 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.865894 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.833809 heaserver-trash-aws-s3-1.0.0a2/tests/
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.834808 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.868557 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.470519 heaserver-trash-aws-s3-1.0.0a3/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-05-03 03:59:55.469519 heaserver-trash-aws-s3-1.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:59:55.470519 heaserver-trash-aws-s3-1.0.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2023-05-03 03:59:21.000000 heaserver-trash-aws-s3-1.0.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.431800 heaserver-trash-aws-s3-1.0.0a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.430230 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.443520 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    47564 2023-05-03 03:58:45.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.444520 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.465518 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.432802 heaserver-trash-aws-s3-1.0.0a3/tests/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.432802 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.468519 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a2/LICENSE` & `heaserver-trash-aws-s3-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a2/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a2/README.md` & `heaserver-trash-aws-s3-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a2/setup.py` & `heaserver-trash-aws-s3-1.0.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a2',
+    version='1.0.0a3',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver>=1.0.0a114, < 1.0.0a115'
+          'heaserver>=1.0.0a115, <1.0.0a116'
       ],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,18 +681,18 @@
       '404':
         $ref: '#/components/responses/404'
     """
     return await response.get_multiple_choices(request, await _get_deleted_item(request))
 
 
 def main() -> None:
-    config = init_cmd_line(
-        description='deleted file management', default_port=8080)
-    start(db=S3Manager, wstl_builder_factory=builder_factory(
-        __package__), config=config)
+    config = init_cmd_line(description='Deleted file management',
+                           default_port=8080)
+    start(package_name='heaserver-trash-aws-s3', db=S3Manager,
+          wstl_builder_factory=builder_factory(__package__), config=config)
 
 
 async def _list_object_versions_partial(s3: S3Client, bucket_id: str, continuation_token: str | None = None,
                                         prefix: str | None = None):
     list_partial = partial(s3.list_object_versions, Bucket=bucket_id)
     if continuation_token is not None:
         list_partial = partial(list_partial, KeyMarker=continuation_token)
```

### Comparing `heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

