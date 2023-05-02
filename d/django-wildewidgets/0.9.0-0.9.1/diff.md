# Comparing `tmp/django-wildewidgets-0.9.0.tar.gz` & `tmp/django-wildewidgets-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-wildewidgets-0.9.0.tar", last modified: Fri Nov 12 22:42:16 2021, max compression
+gzip compressed data, was "dist/django-wildewidgets-0.9.1.tar", last modified: Sat Nov 13 02:35:22 2021, max compression
```

## Comparing `django-wildewidgets-0.9.0.tar` & `django-wildewidgets-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/
--rw-r--r--   0 glenn      (504) admin       (80)      118 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/MANIFEST.in
--rw-r--r--   0 glenn      (504) admin       (80)     3685 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     2685 2021-11-05 22:13:56.000000 django-wildewidgets-0.9.0/README.md
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/django_wildewidgets.egg-info/
--rw-r--r--   0 glenn      (504) admin       (80)     3685 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/django_wildewidgets.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     1406 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/django_wildewidgets.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (504) admin       (80)        1 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/django_wildewidgets.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (504) admin       (80)       13 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/django_wildewidgets.egg-info/top_level.txt
--rw-r--r--   0 glenn      (504) admin       (80)       38 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/setup.cfg
--rw-r--r--   0 glenn      (504) admin       (80)      613 2021-11-12 22:42:05.000000 django-wildewidgets-0.9.0/setup.py
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/wildewidgets/
--rw-r--r--   0 glenn      (504) admin       (80)       96 2021-11-12 22:42:05.000000 django-wildewidgets-0.9.0/wildewidgets/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)       63 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/admin.py
--rw-r--r--   0 glenn      (504) admin       (80)       99 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/apps.py
--rw-r--r--   0 glenn      (504) admin       (80)       57 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/models.py
--rw-r--r--   0 glenn      (504) admin       (80)    38615 2021-11-12 21:43:06.000000 django-wildewidgets-0.9.0/wildewidgets/tables.py
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/wildewidgets/templates/
--rw-r--r--   0 glenn      (504) admin       (80)     6148 2021-10-20 01:19:55.000000 django-wildewidgets-0.9.0/wildewidgets/templates/.DS_Store
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/
--rw-r--r--   0 glenn      (504) admin       (80)      728 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/altairchart.html
--rw-r--r--   0 glenn      (504) admin       (80)     2945 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/barchart.html
--rw-r--r--   0 glenn      (504) admin       (80)     5479 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/categorychart.html
--rw-r--r--   0 glenn      (504) admin       (80)      126 2021-11-10 23:02:07.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/crispy_form_modal.html
--rw-r--r--   0 glenn      (504) admin       (80)     1702 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/doughnutchart.html
--rw-r--r--   0 glenn      (504) admin       (80)     1550 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/doughnutchart_json.html
--rw-r--r--   0 glenn      (504) admin       (80)      288 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/header_with_controls.html
--rw-r--r--   0 glenn      (504) admin       (80)      203 2021-11-10 23:02:19.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/header_with_link_button.html
--rw-r--r--   0 glenn      (504) admin       (80)      256 2021-11-10 23:02:23.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/header_with_modal_button.html
--rw-r--r--   0 glenn      (504) admin       (80)     1904 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/menu.html
--rw-r--r--   0 glenn      (504) admin       (80)      604 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/modal.html
--rw-r--r--   0 glenn      (504) admin       (80)     2556 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/stackedbarchart.html
--rw-r--r--   0 glenn      (504) admin       (80)     2492 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/stackedbarchart_json.html
--rw-r--r--   0 glenn      (504) admin       (80)      762 2021-10-19 22:56:51.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/tabbed_widget.html
--rw-r--r--   0 glenn      (504) admin       (80)     9314 2021-11-12 21:43:12.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/table.html
--rw-r--r--   0 glenn      (504) admin       (80)      160 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/widget_stream.html
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-12 22:42:16.000000 django-wildewidgets-0.9.0/wildewidgets/templatetags/
--rw-r--r--   0 glenn      (504) admin       (80)        0 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templatetags/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)      782 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/templatetags/wildewidgets.py
--rw-r--r--   0 glenn      (504) admin       (80)       60 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/tests.py
--rw-r--r--   0 glenn      (504) admin       (80)      521 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.0/wildewidgets/views.py
--rw-r--r--   0 glenn      (504) admin       (80)    21523 2021-11-11 00:36:54.000000 django-wildewidgets-0.9.0/wildewidgets/wildewidgets.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/
+-rw-r--r--   0 glenn      (504) admin       (80)      118 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/MANIFEST.in
+-rw-r--r--   0 glenn      (504) admin       (80)     3685 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     2685 2021-11-05 22:13:56.000000 django-wildewidgets-0.9.1/README.md
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/django_wildewidgets.egg-info/
+-rw-r--r--   0 glenn      (504) admin       (80)     3685 2021-11-13 02:35:21.000000 django-wildewidgets-0.9.1/django_wildewidgets.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     1406 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/django_wildewidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (504) admin       (80)        1 2021-11-13 02:35:21.000000 django-wildewidgets-0.9.1/django_wildewidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       13 2021-11-13 02:35:21.000000 django-wildewidgets-0.9.1/django_wildewidgets.egg-info/top_level.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       38 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/setup.cfg
+-rw-r--r--   0 glenn      (504) admin       (80)      613 2021-11-13 02:35:14.000000 django-wildewidgets-0.9.1/setup.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/wildewidgets/
+-rw-r--r--   0 glenn      (504) admin       (80)       96 2021-11-13 02:35:14.000000 django-wildewidgets-0.9.1/wildewidgets/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)       63 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/admin.py
+-rw-r--r--   0 glenn      (504) admin       (80)       99 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/apps.py
+-rw-r--r--   0 glenn      (504) admin       (80)       57 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/models.py
+-rw-r--r--   0 glenn      (504) admin       (80)    38615 2021-11-12 21:43:06.000000 django-wildewidgets-0.9.1/wildewidgets/tables.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/wildewidgets/templates/
+-rw-r--r--   0 glenn      (504) admin       (80)     6148 2021-10-20 01:19:55.000000 django-wildewidgets-0.9.1/wildewidgets/templates/.DS_Store
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/
+-rw-r--r--   0 glenn      (504) admin       (80)      728 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/altairchart.html
+-rw-r--r--   0 glenn      (504) admin       (80)     2945 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/barchart.html
+-rw-r--r--   0 glenn      (504) admin       (80)     5479 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/categorychart.html
+-rw-r--r--   0 glenn      (504) admin       (80)      126 2021-11-10 23:02:07.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/crispy_form_modal.html
+-rw-r--r--   0 glenn      (504) admin       (80)     1702 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/doughnutchart.html
+-rw-r--r--   0 glenn      (504) admin       (80)     1550 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/doughnutchart_json.html
+-rw-r--r--   0 glenn      (504) admin       (80)      288 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/header_with_controls.html
+-rw-r--r--   0 glenn      (504) admin       (80)      203 2021-11-10 23:02:19.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/header_with_link_button.html
+-rw-r--r--   0 glenn      (504) admin       (80)      256 2021-11-10 23:02:23.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/header_with_modal_button.html
+-rw-r--r--   0 glenn      (504) admin       (80)     1904 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/menu.html
+-rw-r--r--   0 glenn      (504) admin       (80)      604 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/modal.html
+-rw-r--r--   0 glenn      (504) admin       (80)     2556 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/stackedbarchart.html
+-rw-r--r--   0 glenn      (504) admin       (80)     2492 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/stackedbarchart_json.html
+-rw-r--r--   0 glenn      (504) admin       (80)      762 2021-10-19 22:56:51.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/tabbed_widget.html
+-rw-r--r--   0 glenn      (504) admin       (80)     9314 2021-11-12 21:43:12.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/table.html
+-rw-r--r--   0 glenn      (504) admin       (80)      160 2021-11-10 23:01:48.000000 django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/widget_stream.html
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2021-11-13 02:35:22.000000 django-wildewidgets-0.9.1/wildewidgets/templatetags/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templatetags/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)      782 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/templatetags/wildewidgets.py
+-rw-r--r--   0 glenn      (504) admin       (80)       60 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/tests.py
+-rw-r--r--   0 glenn      (504) admin       (80)      521 2021-10-18 22:27:15.000000 django-wildewidgets-0.9.1/wildewidgets/views.py
+-rw-r--r--   0 glenn      (504) admin       (80)    21607 2021-11-13 02:34:28.000000 django-wildewidgets-0.9.1/wildewidgets/wildewidgets.py
```

### Comparing `django-wildewidgets-0.9.0/PKG-INFO` & `django-wildewidgets-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wildewidgets
-Version: 0.9.0
+Version: 0.9.1
 Summary: django-wildewidgets is a Django library designed to help you make charts, graphs, tables, and UI widgets quickly and easily with libraries like Chartjs, Altair, and Datatables.
 Home-page: https://github.com/caltechads/django-wildewidget
 Author: IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: ```
              _ _                                     _ _     _               _     _            _
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-wildewidgets Version: 0.9.0 Summary: django-
+Metadata-Version: 2.1 Name: django-wildewidgets Version: 0.9.1 Summary: django-
 wildewidgets is a Django library designed to help you make charts, graphs,
 tables, and UI widgets quickly and easily with libraries like Chartjs, Altair,
 and Datatables. Home-page: https://github.com/caltechads/django-wildewidget
 Author: IMSS ADS Author-email: imss-ads-staff@caltech.edu License: UNKNOWN
 Description: ``` _ _ _ _ _ _ _ _ | (_) (_) | | | (_) | | | | __| |_ __ _ _ __
 __ _ ___ _____ ___| | __| | _____ ___ __| | __ _ ___| |_ ___ / _` | |/ _` | '_
 \ / _` |/ _ \___\ \ /\ / / | |/ _` |/ _ \ \ /\ / / |/ _` |/ _` |/ _ \ __/ __| |
```

### Comparing `django-wildewidgets-0.9.0/README.md` & `django-wildewidgets-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/django_wildewidgets.egg-info/PKG-INFO` & `django-wildewidgets-0.9.1/django_wildewidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wildewidgets
-Version: 0.9.0
+Version: 0.9.1
 Summary: django-wildewidgets is a Django library designed to help you make charts, graphs, tables, and UI widgets quickly and easily with libraries like Chartjs, Altair, and Datatables.
 Home-page: https://github.com/caltechads/django-wildewidget
 Author: IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: ```
              _ _                                     _ _     _               _     _            _
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-wildewidgets Version: 0.9.0 Summary: django-
+Metadata-Version: 2.1 Name: django-wildewidgets Version: 0.9.1 Summary: django-
 wildewidgets is a Django library designed to help you make charts, graphs,
 tables, and UI widgets quickly and easily with libraries like Chartjs, Altair,
 and Datatables. Home-page: https://github.com/caltechads/django-wildewidget
 Author: IMSS ADS Author-email: imss-ads-staff@caltech.edu License: UNKNOWN
 Description: ``` _ _ _ _ _ _ _ _ | (_) (_) | | | (_) | | | | __| |_ __ _ _ __
 __ _ ___ _____ ___| | __| | _____ ___ __| | __ _ ___| |_ ___ / _` | |/ _` | '_
 \ / _` |/ _ \___\ \ /\ / / | |/ _` |/ _ \ \ /\ / / |/ _` |/ _` |/ _ \ __/ __| |
```

### Comparing `django-wildewidgets-0.9.0/django_wildewidgets.egg-info/SOURCES.txt` & `django-wildewidgets-0.9.1/django_wildewidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/setup.py` & `django-wildewidgets-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-wildewidgets',
-    version="0.9.0",
+    version="0.9.1",
     description='django-wildewidgets is a Django library designed to help you make charts, graphs, tables, and UI widgets quickly and easily with libraries like Chartjs, Altair, and Datatables.',
     long_description=open('README.md', 'rt').read(),
     long_description_content_type="text/markdown",
     author="IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url='https://github.com/caltechads/django-wildewidget',
     packages=find_packages(exclude=['bin']),
```

### Comparing `django-wildewidgets-0.9.0/wildewidgets/tables.py` & `django-wildewidgets-0.9.1/wildewidgets/tables.py`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/.DS_Store` & `django-wildewidgets-0.9.1/wildewidgets/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/altairchart.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/altairchart.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/barchart.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/barchart.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/categorychart.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/categorychart.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/doughnutchart.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/doughnutchart.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/doughnutchart_json.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/doughnutchart_json.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/menu.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/menu.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/modal.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/modal.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/stackedbarchart.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/stackedbarchart.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/stackedbarchart_json.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/stackedbarchart_json.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/tabbed_widget.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/tabbed_widget.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templates/wildewidgets/table.html` & `django-wildewidgets-0.9.1/wildewidgets/templates/wildewidgets/table.html`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/templatetags/wildewidgets.py` & `django-wildewidgets-0.9.1/wildewidgets/templatetags/wildewidgets.py`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/views.py` & `django-wildewidgets-0.9.1/wildewidgets/views.py`

 * *Files identical despite different names*

### Comparing `django-wildewidgets-0.9.0/wildewidgets/wildewidgets.py` & `django-wildewidgets-0.9.1/wildewidgets/wildewidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import random
 import re
 
 from django import template
 from django.apps import apps
 from django.conf import settings
+from django.core.exceptions import ImproperlyConfigured
 from django.db.models import Q
 from django.http import JsonResponse
 from django.urls import reverse_lazy
 from django.views.generic import View
 
 
 class JSONDataView(View):
@@ -581,16 +582,16 @@
         self.tabs.append((name,widget))
 
     def get_context_data(self, **kwargs):
         kwargs['tabs'] = self.tabs
         return kwargs
  
 
-class HeaderWithControls(TemplateWidget):
-    template_name = 'core/header_with_controls.html'
+class BasicHeader(TemplateWidget):
+    template_name = 'wildewidgets/header_with_controls.html'
     header_level = 1
     header_text = None
     css_class = None
     css_id = None
     badge_text = None
     badge_class = "warning"
 
@@ -600,68 +601,68 @@
         kwargs['css_class'] = self.css_class
         kwargs['css_id'] = self.css_id
         kwargs['badge_text'] = self.badge_text
         kwargs['badge_class'] = self.badge_class
         return kwargs
 
 
-class HeaderWithLinkButton(HeaderWithControls):
-    template_name = 'core/header_with_link_button.html'
+class HeaderWithLinkButton(BasicHeader):
+    template_name = 'wildewidgets/header_with_link_button.html'
     url = None
     link_text = None
     button_class = "primary"
 
     def get_context_data(self, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs['url'] = self.url
         kwargs['link_text'] = self.link_text
         kwargs['button_class'] = self.button_class
         return kwargs
 
 
-class HeaderWithFormButton(HeaderWithControls):
-    template_name = 'core/header_with_form_button.html'
+class HeaderWithFormButton(BasicHeader):
+    template_name = 'wildewidgets/header_with_form_button.html'
     url = None
     button_text = None
 
     def get_context_data(self, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs['url'] = self.url
         kwargs['button_text'] = self.link_text
         return kwargs
 
 
-class HeaderWithModalButton(HeaderWithControls):
-    template_name = 'core/header_with_modal_button.html'
+class HeaderWithModalButton(BasicHeader):
+    template_name = 'wildewidgets/header_with_modal_button.html'
     modal_id = None
     button_text = None
     button_class = "primary"
 
     def get_context_data(self, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs['modal_id'] = self.modal_id
         kwargs['button_text'] = self.button_text
         kwargs['button_class'] = self.button_class
         return kwargs
 
 
 class ModalWidget(TemplateWidget):
-    template_name = 'core/modal.html'
+    template_name = 'wildewidgets/modal.html'
     modal_id = None
     modal_title = None
 
     def get_context_data(self, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs['modal_id'] = self.modal_id
         kwargs['modal_title'] = self.modal_title
         return kwargs
 
 
 class CrispyFormModalWidget(ModalWidget):
-    template_name = 'core/crispy_form_modal.html'
+    template_name = 'wildewidgets/crispy_form_modal.html'
     form_class = None
     form = None
 
     def get_context_data(self, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         if self.form_class:
             kwargs['form'] = self.form_class()
@@ -669,15 +670,15 @@
             kwargs['form'] = self.form
         else:
             raise ImproperlyConfigured("Either 'form_class' or 'form' must be set")
         return kwargs
 
 
 class WidgetStream(TemplateWidget):
-    template_name = 'core/widget_stream.html'
+    template_name = 'wildewidgets/widget_stream.html'
 
     def __init__(self):
         self.widgets = []
 
     def add_widget(self, widget, css_class=None):
         self.widgets.append((widget, css_class))
```

