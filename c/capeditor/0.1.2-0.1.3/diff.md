# Comparing `tmp/capeditor-0.1.2.tar.gz` & `tmp/capeditor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.1.2.tar", last modified: Wed May  3 13:58:13 2023, max compression
+gzip compressed data, was "capeditor-0.1.3.tar", last modified: Wed May  3 14:02:52 2023, max compression
```

## Comparing `capeditor-0.1.2.tar` & `capeditor-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 13:58:00.000000 capeditor-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 13:58:13.655614 capeditor-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-03 13:58:00.000000 capeditor-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.651614 capeditor-0.1.2/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/static/css/header.css
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/static/js/common.js
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/static/js/hide_attributes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.651614 capeditor-0.1.2/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/alert_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/alert_filter_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/alert_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/alert_item_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/alert_list_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/latest_alert_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/pagination_include.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/widgets/basemap_polygon.html
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templates/capeditor/widgets/polygon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/templatetags/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 13:58:00.000000 capeditor-0.1.2/capeditor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:13.655614 capeditor-0.1.2/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 13:58:13.000000 capeditor-0.1.2/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 13:58:13.000000 capeditor-0.1.2/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:58:13.000000 capeditor-0.1.2/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 13:58:13.000000 capeditor-0.1.2/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:58:13.000000 capeditor-0.1.2/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:58:13.655614 capeditor-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 13:58:00.000000 capeditor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 14:02:38.000000 capeditor-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 14:02:52.200347 capeditor-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-03 14:02:38.000000 capeditor-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.196347 capeditor-0.1.3/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.196347 capeditor-0.1.3/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/static/css/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/static/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/static/js/hide_attributes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.196347 capeditor-0.1.3/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/alert_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/alert_filter_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/alert_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/alert_item_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/alert_list_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/latest_alert_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/pagination_include.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/widgets/basemap_polygon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templates/capeditor/widgets/polygon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.200347 capeditor-0.1.3/capeditor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/templatetags/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 14:02:38.000000 capeditor-0.1.3/capeditor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:52.196347 capeditor-0.1.3/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 14:02:52.000000 capeditor-0.1.3/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 14:02:52.000000 capeditor-0.1.3/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:02:52.000000 capeditor-0.1.3/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 14:02:52.000000 capeditor-0.1.3/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 14:02:52.000000 capeditor-0.1.3/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:02:52.200347 capeditor-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 14:02:38.000000 capeditor-0.1.3/setup.py
```

### Comparing `capeditor-0.1.2/README.md` & `capeditor-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
+[![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
 
 The **Common Alerting Protocol (CAP)** provides an open, non-proprietary
 digital message format for all types of alerts and notifications. It
 does not address any particular application or telecommunications
```

### Comparing `capeditor-0.1.2/capeditor/migrations/0001_initial.py` & `capeditor-0.1.3/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/models.py` & `capeditor-0.1.3/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/renderers.py` & `capeditor-0.1.3/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/serializers.py` & `capeditor-0.1.3/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/static/css/header.css` & `capeditor-0.1.3/capeditor/static/css/header.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/static/css/style.css` & `capeditor-0.1.3/capeditor/static/css/style.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/static/js/common.js` & `capeditor-0.1.3/capeditor/static/js/common.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/static/js/hide_attributes.js` & `capeditor-0.1.3/capeditor/static/js/hide_attributes.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/alert_detail.html` & `capeditor-0.1.3/capeditor/templates/capeditor/alert_detail.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/alert_filter_include.html` & `capeditor-0.1.3/capeditor/templates/capeditor/alert_filter_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/alert_index.html` & `capeditor-0.1.3/capeditor/templates/capeditor/alert_index.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/alert_item_include.html` & `capeditor-0.1.3/capeditor/templates/capeditor/alert_item_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/alert_list_include.html` & `capeditor-0.1.3/capeditor/templates/capeditor/alert_list_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/latest_alert_include.html` & `capeditor-0.1.3/capeditor/templates/capeditor/latest_alert_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/pagination_include.html` & `capeditor-0.1.3/capeditor/templates/capeditor/pagination_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templates/capeditor/widgets/polygon.html` & `capeditor-0.1.3/capeditor/templates/capeditor/widgets/polygon.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/templatetags/pagination.py` & `capeditor-0.1.3/capeditor/templatetags/pagination.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/utils.py` & `capeditor-0.1.3/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/views.py` & `capeditor-0.1.3/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/wagtail_hooks.py` & `capeditor-0.1.3/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor/widgets.py` & `capeditor-0.1.3/capeditor/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/capeditor.egg-info/SOURCES.txt` & `capeditor-0.1.3/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.2/setup.py` & `capeditor-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='capeditor',
-    version='0.1.2',
+    version='0.1.3',
     description='Wagtail CAP Editor can be used as standalone or integrated into website',
     author='Grace Amondi',
     author_email='miswa.grace@gmail.com',
     install_requires=[
         'Django>=4.0.0',
         'djangorestframework-xml>=2.0.0',
         'six>=1.16.0',
```

