# Comparing `tmp/heaserver-accounts-1.0.0a8.tar.gz` & `tmp/heaserver-accounts-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heaserver-accounts-1.0.0a8.tar", last modified: Mon Mar 21 22:13:30 2022, max compression
+gzip compressed data, was "dist\heaserver-accounts-1.0.0a9.tar", last modified: Tue Apr  5 21:36:37 2022, max compression
```

## Comparing `heaserver-accounts-1.0.0a8.tar` & `heaserver-accounts-1.0.0a9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:30.037117 heaserver-accounts-1.0.0a8/
--rw-rw-rw-   0        0        0    11625 2021-12-16 15:38:39.000000 heaserver-accounts-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0       39 2021-12-16 15:38:39.000000 heaserver-accounts-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     5527 2022-03-21 22:13:30.037117 heaserver-accounts-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3691 2022-03-03 18:54:20.000000 heaserver-accounts-1.0.0a8/README.md
--rw-rw-rw-   0        0        0       42 2022-03-21 22:13:30.037117 heaserver-accounts-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1892 2022-03-21 19:21:39.000000 heaserver-accounts-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:29.996116 heaserver-accounts-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:29.995117 heaserver-accounts-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:30.006117 heaserver-accounts-1.0.0a8/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a8/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0     9147 2022-03-21 19:21:33.000000 heaserver-accounts-1.0.0a8/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:30.006117 heaserver-accounts-1.0.0a8/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0     6375 2022-03-03 18:54:20.000000 heaserver-accounts-1.0.0a8/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:30.024117 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5527 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-03-21 22:13:29.000000 heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:29.996116 heaserver-accounts-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:29.996116 heaserver-accounts-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-03-21 22:13:30.036118 heaserver-accounts-1.0.0a8/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a8/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     1358 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a8/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.832487 heaserver-accounts-1.0.0a9/
+-rw-rw-rw-   0        0        0    11625 2021-12-16 15:38:39.000000 heaserver-accounts-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0       39 2021-12-16 15:38:39.000000 heaserver-accounts-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5527 2022-04-05 21:36:37.831486 heaserver-accounts-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3691 2022-03-03 18:54:20.000000 heaserver-accounts-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0       42 2022-04-05 21:36:37.832487 heaserver-accounts-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1892 2022-04-05 21:34:50.000000 heaserver-accounts-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.776486 heaserver-accounts-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.776486 heaserver-accounts-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.794487 heaserver-accounts-1.0.0a9/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a9/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0     9149 2022-04-05 21:27:48.000000 heaserver-accounts-1.0.0a9/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.800486 heaserver-accounts-1.0.0a9/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0     6375 2022-03-03 18:54:20.000000 heaserver-accounts-1.0.0a9/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.823490 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5527 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-04-05 21:36:37.000000 heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.777486 heaserver-accounts-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.777486 heaserver-accounts-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-04-05 21:36:37.830486 heaserver-accounts-1.0.0a9/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a9/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     1358 2022-01-25 21:42:35.000000 heaserver-accounts-1.0.0a9/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver-accounts-1.0.0a8/LICENSE` & `heaserver-accounts-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.0a8/PKG-INFO` & `heaserver-accounts-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: It manages account information details
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Description: # HEA Server AWS Accounts Microservice
         [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
```

### Comparing `heaserver-accounts-1.0.0a8/README.md` & `heaserver-accounts-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.0a8/setup.py` & `heaserver-accounts-1.0.0a9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="It manages account information details",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.8',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver>=1.0.0a57, <1.0.0a58'
+        'heaserver>=1.0.0a59, <1.0.0a60'
     ],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver-accounts-1.0.0a8/src/heaserver/account/service.py` & `heaserver-accounts-1.0.0a9/src/heaserver/account/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         url = URL(await type_to_resource_url(request=request, type_or_type_name=AWSBucket,
                                              file_system_type_or_type_name=AWSFileSystem)) / volume_id / 'buckets'
 
         async def get_one_bucket_dict(b: AWSBucket):
             logging.info("Bucket names  %s returning", b.display_name)
             return b.to_dict()
         bucket_dicts = await gather(*[get_one_bucket_dict(b) async for b in
-                                      client.get_all(app=request.app, url=url, obj=AWSBucket, headers=headers)])
+                                      client.get_all(app=request.app, url=url, type_=AWSBucket, headers=headers)])
 
     return await response.get_all(request, bucket_dicts)
 
 
 @routes.get('/volumes/{volume_id}/awsaccounts/me/opener')
 @action('heaserver-accounts-account-open-buckets',
         rel=f'hea-opener hea-context-aws hea-default {AWSBucket.get_mime_type()}', path='/volumes/{volume_id}/buckets/')
```

### Comparing `heaserver-accounts-1.0.0a8/src/heaserver/account/wstl/all.json` & `heaserver-accounts-1.0.0a9/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.0a8/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver-accounts-1.0.0a9/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: It manages account information details
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Description: # HEA Server AWS Accounts Microservice
         [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
```

### Comparing `heaserver-accounts-1.0.0a8/tests/heaserver/accounttest/testcase.py` & `heaserver-accounts-1.0.0a9/tests/heaserver/accounttest/testcase.py`

 * *Files identical despite different names*

