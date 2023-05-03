# Comparing `tmp/wagtail-meta-preview-1.1.1.tar.gz` & `tmp/wagtail-meta-preview-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-meta-preview-1.1.1.tar", last modified: Wed May 18 20:05:28 2022, max compression
+gzip compressed data, was "wagtail-meta-preview-2.0.0.tar", last modified: Wed May  3 13:10:31 2023, max compression
```

## Comparing `wagtail-meta-preview-1.1.1.tar` & `wagtail-meta-preview-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.750969 wagtail-meta-preview-1.1.1/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/meta_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     9155 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.750969 wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.750969 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-05-18 20:05:15.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 20:05:28.754969 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-18 20:05:28.000000 wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.359748 wagtail-meta-preview-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.363747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/meta_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.351747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.367748 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.351747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.367748 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/top_level.txt
```

### Comparing `wagtail-meta-preview-1.1.1/LICENSE` & `wagtail-meta-preview-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/PKG-INFO` & `wagtail-meta-preview-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 1.1.1
+Version: 2.0.0
 Summary: Add preview panels for meta data to wagtail
 Home-page: https://github.com/rinti/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
+## Current supported versions
+
+Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+
+## Preview
+
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
 
 ## Documentation
 
@@ -39,12 +44,12 @@
 - [Settings](./docs/3-settings.md)
 
 ## Development
 
 ### Dev server
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
-start a server on http://localhost:8080/admin/ (user: admin, pw: admin) with a couple of page types to test with.
+start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
```

### Comparing `wagtail-meta-preview-1.1.1/README.md` & `wagtail-meta-preview-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
+## Current supported versions
+
+Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+
+## Preview
+
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
 
 ## Documentation
 
@@ -15,12 +21,12 @@
 - [Settings](./docs/3-settings.md)
 
 ## Development
 
 ### Dev server
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
-start a server on http://localhost:8080/admin/ (user: admin, pw: admin) with a couple of page types to test with.
+start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
```

### Comparing `wagtail-meta-preview-1.1.1/setup.py` & `wagtail-meta-preview-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,34 +11,35 @@
 testing_extras = ["black==19.10b0", "coverage==5.2.1"]
 
 setup(
     name="wagtail-meta-preview",
     version=version,
     description="Add preview panels for meta data to wagtail",
     long_description=readme,
+    long_description_content_type="text/markdown",
     author="Andreas Bernacca",
     author_email="ante.bernacca@gmail.com",
     url="https://github.com/rinti/wagtail-meta-preview",
-    install_requires=["wagtail>=2.7",],
-    extras_require={"testing": testing_extras,},
+    install_requires=["wagtail>=3.0.0"],
+    extras_require={
+        "testing": testing_extras,
+    },
     setup_requires=["wheel"],
     zip_safe=False,
     license="MIT License",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     package_data={},
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Framework :: Django",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 2",
+        "Framework :: Wagtail :: 3",
+        "Framework :: Wagtail :: 4",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/meta_settings.py` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/meta_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/utils.py` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/views.py` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview/wagtail_hooks.py` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview/wagtail_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.urls import path
 from django.utils.html import format_html
 from wagtail.admin.staticfiles import versioned_static
-from wagtail.core import hooks
+from wagtail import hooks
+
 from .views import get_image_rendition
 
 
 @hooks.register("insert_global_admin_css", order=100)
 def global_admin_css():
     """Add /static/css/custom.css to the admin."""
     return format_html(
```

### Comparing `wagtail-meta-preview-1.1.1/wagtail_meta_preview.egg-info/PKG-INFO` & `wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 1.1.1
+Version: 2.0.0
 Summary: Add preview panels for meta data to wagtail
 Home-page: https://github.com/rinti/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
+## Current supported versions
+
+Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+
+## Preview
+
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
 
 ## Documentation
 
@@ -39,12 +44,12 @@
 - [Settings](./docs/3-settings.md)
 
 ## Development
 
 ### Dev server
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
-start a server on http://localhost:8080/admin/ (user: admin, pw: admin) with a couple of page types to test with.
+start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
```

