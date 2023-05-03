# Comparing `tmp/ckanext-dc_serve-0.9.4.tar.gz` & `tmp/ckanext-dc_serve-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dc_serve-0.9.4.tar", last modified: Wed Jun 22 07:56:13 2022, max compression
+gzip compressed data, was "ckanext-dc_serve-0.9.5.tar", last modified: Thu Apr 27 11:00:05 2023, max compression
```

## Comparing `ckanext-dc_serve-0.9.4.tar` & `ckanext-dc_serve-0.9.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/ckanext/dc_serve/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-22 07:55:30.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/res_file_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/route_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.622429 ckanext-dc_serve-0.9.4/ckanext/dc_serve/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/ckanext/dc_serve/templates/package/
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_res_file_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)    17189 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-22 07:56:13.000000 ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-22 07:56:13.626429 ckanext-dc_serve-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-06-22 07:55:20.000000 ckanext-dc_serve-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.358983 ckanext-dc_serve-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-27 11:00:05.354983 ckanext-dc_serve-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.350983 ckanext-dc_serve-0.9.5/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.350983 ckanext-dc_serve-0.9.5/ckanext/dc_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 10:59:54.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/res_file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/route_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.346983 ckanext-dc_serve-0.9.5/ckanext/dc_serve/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.350983 ckanext-dc_serve-0.9.5/ckanext/dc_serve/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.354983 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_res_file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:00:05.354983 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 11:00:05.000000 ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:00:05.358983 ckanext-dc_serve-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-27 10:59:44.000000 ckanext-dc_serve-0.9.5/setup.py
```

### Comparing `ckanext-dc_serve-0.9.4/CHANGELOG` & `ckanext-dc_serve-0.9.5/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.9.5
+ - fix: support dclab 0.49.1 (condense has new kwarg)
+ - ref: cleanup
 0.9.4
  - fix: properly support dclab 0.43.0 (HDF5Scalar feature and `tolist`)
 0.9.3
  - setup: bump dclab from 0.37.0 to 0.43.0 (zstandard compression)
 0.9.2
  - maintenance release
 0.9.1
```

### Comparing `ckanext-dc_serve-0.9.4/LICENSE` & `ckanext-dc_serve-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/PKG-INFO` & `ckanext-dc_serve-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dc_serve
-Version: 0.9.4
+Version: 0.9.5
 Summary: Serve DC files via GET requests on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dc_serve
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
@@ -71,13 +71,13 @@
     vagrant up
     # Run the tests
     vagrant ssh -- sudo bash /testing/vagrant-run-tests.sh
 
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ckanext.dc_serve.svg
    :target: https://pypi.python.org/pypi/ckanext.dc_serve
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/DCOR-dev/ckanext-dc_serve/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/DCOR-dev/ckanext-dc_serve/check.yml
    :target: https://github.com/DCOR-dev/ckanext-dc_serve/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/DCOR-dev/ckanext-dc_serve
    :target: https://codecov.io/gh/DCOR-dev/ckanext-dc_serve
```

### Comparing `ckanext-dc_serve-0.9.4/README.rst` & `ckanext-dc_serve-0.9.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,11 +57,11 @@
     vagrant up
     # Run the tests
     vagrant ssh -- sudo bash /testing/vagrant-run-tests.sh
 
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ckanext.dc_serve.svg
    :target: https://pypi.python.org/pypi/ckanext.dc_serve
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/DCOR-dev/ckanext-dc_serve/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/DCOR-dev/ckanext-dc_serve/check.yml
    :target: https://github.com/DCOR-dev/ckanext-dc_serve/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/DCOR-dev/ckanext-dc_serve
    :target: https://codecov.io/gh/DCOR-dev/ckanext-dc_serve
```

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/_version.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/cli.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @click.option('--modified-days', default=-1,
               help='Only run for datasets modified within this number of days '
                    + 'in the past. Set to -1 to apply to all datasets.')
 @click.command()
 def run_jobs_dc_serve(modified_days=-1):
-    """Compute condensed resource all .rtdc files
+    """Compute condensed resources for all .rtdc files
 
     This also happens for draft datasets.
     """
     # go through all datasets
     datasets = model.Session.query(model.Package)
 
     if modified_days >= 0:
```

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/jobs.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,21 @@
                     resource_id=resource["id"],
                     locker_id="DCOR_generate_condensed") as fl:
                 # The CKANResourceFileLock creates a lock file if not present
                 # and then sets `is_locked` to True if the lock was acquired.
                 # If the lock could not be acquired, that means that another
                 # process is currently doing what we are attempting to do, so
                 # we can just ignore this resource. The reason why I
-                # implemented this is because I wanted to add an automated
+                # implemented this is that I wanted to add an automated
                 # background job for generating missing condensed files, but
                 # then several processes would end up condensing the same
                 # resource.
                 if fl.is_locked:
                     # run in subprocess to circumvent memory leak
-                    # https://github.com/ZELLMECHANIK-DRESDEN/dclab/issues/138
+                    # https://github.com/DC-analysis/dclab/issues/138
                     # condense(path_out=cond, path_in=path, check_suffix=False)
                     p = multiprocessing.Process(target=condense,
-                                                args=(cond, path, False))
+                                                args=(cond, path, True, False))
                     p.start()
                     p.join()
                     return True
     return False
```

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/plugin.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/res_file_lock.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/res_file_lock.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/route_funcs.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/route_funcs.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/serve.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/serve.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/templates/package/resource_read.html` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/templates/package/resource_read.html`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/helper_methods.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_jobs.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_res_file_lock.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_res_file_lock.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext/dc_serve/tests/test_serve.py` & `ckanext-dc_serve-0.9.5/ckanext/dc_serve/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/PKG-INFO` & `ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dc-serve
-Version: 0.9.4
+Version: 0.9.5
 Summary: Serve DC files via GET requests on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dc_serve
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
@@ -71,13 +71,13 @@
     vagrant up
     # Run the tests
     vagrant ssh -- sudo bash /testing/vagrant-run-tests.sh
 
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ckanext.dc_serve.svg
    :target: https://pypi.python.org/pypi/ckanext.dc_serve
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/DCOR-dev/ckanext-dc_serve/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/DCOR-dev/ckanext-dc_serve/check.yml
    :target: https://github.com/DCOR-dev/ckanext-dc_serve/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/DCOR-dev/ckanext-dc_serve
    :target: https://codecov.io/gh/DCOR-dev/ckanext-dc_serve
```

### Comparing `ckanext-dc_serve-0.9.4/ckanext_dc_serve.egg-info/SOURCES.txt` & `ckanext-dc_serve-0.9.5/ckanext_dc_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dc_serve-0.9.4/setup.py` & `ckanext-dc_serve-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     license='AGPLv3+',
     keywords=["CKAN", "DCOR", "RT-DC"],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     package_dir={name: name},
     namespace_packages=['ckanext'],
     install_requires=[
         # the "ckan" dependency is implied
-        "dclab>=0.43.0",
+        "dclab>=0.49.1",
         "dcor_shared>=0.2.0",
     ],
     include_package_data=True,
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points='''
```

