# Comparing `tmp/easys-ordermanager-2.1.2.tar.gz` & `tmp/easys-ordermanager-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easys-ordermanager-2.1.2.tar", last modified: Thu Apr 13 15:08:47 2023, max compression
+gzip compressed data, was "easys-ordermanager-2.1.3.tar", last modified: Wed May  3 10:19:48 2023, max compression
```

## Comparing `easys-ordermanager-2.1.2.tar` & `easys-ordermanager-2.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/
--rw-r--r--   0 root         (0) root         (0)    12147 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     9321 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/CHANGELOG_SERIALIZER.md
--rw-r--r--   0 root         (0) root         (0)    34940 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22247 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/commands/i18n.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v1/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v2/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v3/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      519 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.220855 easys-ordermanager-2.1.2/easys_ordermanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.220855 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    13139 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93490 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v1/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93525 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v2/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94662 2023-04-13 14:49:23.000000 easys-ordermanager-2.1.2/easys_ordermanager/v3/serializer.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22247 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)    12228 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     9435 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/CHANGELOG_SERIALIZER.md
+-rw-r--r--   0 root         (0) root         (0)    34940 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22442 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/dev/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/dev/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/management/commands/i18n.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v1/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v2/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/dev/tests/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/dev/tests/v3/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/easys_ordermanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.989673 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93490 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v1/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93587 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v2/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94724 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/v3/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/easys_ordermanager/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22442 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-03 10:19:48.000000 easys-ordermanager-2.1.3/easys_ordermanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-03 10:19:48.993674 easys-ordermanager-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-05-03 09:45:58.000000 easys-ordermanager-2.1.3/setup.py
```

### Comparing `easys-ordermanager-2.1.2/CHANGELOG.md` & `easys-ordermanager-2.1.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 2.1.3 (2023-05-03)
+* Updates to Serializer v2 & v3, see serializer changelog
+
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
 
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
```

### Comparing `easys-ordermanager-2.1.2/CHANGELOG_SERIALIZER.md` & `easys-ordermanager-2.1.3/CHANGELOG_SERIALIZER.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Serializer changes
 
+## 2.1.3
+
+### v2/v3
+
+#### `OrderLineInAppSerializer`
+* Added `INAPP_AUDIENCE_EMPTY` to `target_audiences` choices.
+
 ## 2.1.2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
 * Made `target_page_type` required.
 * Removed fields:
   - `expected_clicks`
   - `expected_conversions`
@@ -14,15 +21,15 @@
   - `call_to_action`
   - `is_generic_campaign`
   - `generic_topics`
   - `remarketing_setup_fee`
   - `remarketing_budget`
 
 #### `OrderLineLandingpageSerializer`
-* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required.
 
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
@@ -60,15 +67,15 @@
 
 #### `OrderLineSerializer`
 * Added new field `down_payment`, optional
 * Added new field `detail_domain` accepting `OrderLineDomainSerializer` data, optional
 
 #### `Serializer`
 
-* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain 
+* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain
   product provided in the same payload
 
 ## 2.0.12
 
 ### v2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
```

### Comparing `easys-ordermanager-2.1.2/LICENSE.md` & `easys-ordermanager-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/PKG-INFO` & `easys-ordermanager-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.2
+Version: 2.1.3
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -30,14 +30,17 @@
 ### Django 4.1
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.1.3 (2023-05-03)
+* Updates to Serializer v2 & v3, see serializer changelog
+
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
 
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
@@ -426,14 +429,21 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.1.3
+
+### v2/v3
+
+#### `OrderLineInAppSerializer`
+* Added `INAPP_AUDIENCE_EMPTY` to `target_audiences` choices.
+
 ## 2.1.2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
 * Made `target_page_type` required.
 * Removed fields:
   - `expected_clicks`
   - `expected_conversions`
@@ -444,15 +454,15 @@
   - `call_to_action`
   - `is_generic_campaign`
   - `generic_topics`
   - `remarketing_setup_fee`
   - `remarketing_budget`
 
 #### `OrderLineLandingpageSerializer`
-* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required.
 
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
@@ -490,15 +500,15 @@
 
 #### `OrderLineSerializer`
 * Added new field `down_payment`, optional
 * Added new field `detail_domain` accepting `OrderLineDomainSerializer` data, optional
 
 #### `Serializer`
 
-* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain 
+* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain
   product provided in the same payload
 
 ## 2.0.12
 
 ### v2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
```

### Comparing `easys-ordermanager-2.1.2/dev/management/commands/i18n.py` & `easys-ordermanager-2.1.3/dev/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/dev/tests/v3/test_serializer.py` & `easys-ordermanager-2.1.3/dev/tests/v3/test_serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc` & `easys-ordermanager-2.1.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x38d93764 (Thu Apr 13 10:28:08 2023 UTC)
+moddate:  0x562d5264 (Wed May  3 09:45:58 2023 UTC)
 files sz: 300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
@@ -13,15 +13,15 @@
    
      1           2 LOAD_CONST               0 ('easys-ordermanager')
                  4 STORE_NAME               0 (__title__)
    
      2           6 LOAD_CONST               1 ('API definition of RH order manager for EasyS')
                  8 STORE_NAME               1 (__description__)
    
-     3          10 LOAD_CONST               2 ('2.1.2')
+     3          10 LOAD_CONST               2 ('2.1.3')
                 12 STORE_NAME               2 (__version__)
    
      4          14 LOAD_CONST               3 ('https://gitlab.herocentral.de/development/easys-ordermanager')
                 16 STORE_NAME               3 (__url__)
    
      5          18 LOAD_CONST               4 ('RegioHelden developers')
                 20 STORE_NAME               4 (__author__)
@@ -32,15 +32,15 @@
      7          26 LOAD_CONST               6 ('GPL 3')
                 28 STORE_NAME               6 (__license__)
                 30 LOAD_CONST               7 (None)
                 32 RETURN_VALUE
    consts
       'easys-ordermanager'
       'API definition of RH order manager for EasyS'
-      '2.1.2'
+      '2.1.3'
       'https://gitlab.herocentral.de/development/easys-ordermanager'
       'RegioHelden developers'
       'opensource@regiohelden.de'
       'GPL 3'
       None
    names      ('__title__', '__description__', '__version__', '__url__', '__author__', '__author_email__', '__license__')
    varnames   ()
```

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/fields.py` & `easys-ordermanager-2.1.3/easys_ordermanager/fields.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po` & `easys-ordermanager-2.1.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/v1/serializer.py` & `easys-ordermanager-2.1.3/easys_ordermanager/v1/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/v2/serializer.py` & `easys-ordermanager-2.1.3/easys_ordermanager/v2/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     (DISPLAY_CHANNEL_TRAVEL, 'travel', _('Travel')),
     (DISPLAY_CHANNEL_WOMEN, 'women', _('Women')),
     (DISPLAY_CHANNEL_CONSTRUCTION_AND_LIVING, 'construction_and_living', _('Construction & Living')),
     (DISPLAY_CHANNEL_MEN, 'men', _('Men')),
     (DISPLAY_CHANNEL_EAT_AND_DRINK, 'eat_and_drink', _('Eating & Drinking')),
 )
 
+INAPP_AUDIENCE_EMPTY = 0
 INAPP_AUDIENCE_GEBRAUCHTWAGEN_INTERESSENTEN = 1
 INAPP_AUDIENCE_B2B_AUTOMOTIVE = 2
 INAPP_AUDIENCE_AUTOBESITZER = 3
 INAPP_AUDIENCE_SERIENJUNKIES = 4
 INAPP_AUDIENCE_HEAVY_STREAMER = 5
 INAPP_AUDIENCE_MOVIE_LOVER = 6
 INAPP_AUDIENCE_ENTERTAINMENT_LOVER = 7
@@ -533,14 +534,15 @@
 INAPP_AUDIENCE_MILLENIALS = 36
 INAPP_AUDIENCE_MOMS_KIDS = 37
 INAPP_AUDIENCE_FAMILIENVATER = 38
 INAPP_AUDIENCE_BEST_AGER = 39
 INAPP_AUDIENCE_BOSSHOME = 40
 INAPP_AUDIENCE_HOBBYKOCHE = 41
 INAPP_AUDIENCE_CHOICES = Choices(
+    (INAPP_AUDIENCE_EMPTY, '', '-'),
     (INAPP_AUDIENCE_GEBRAUCHTWAGEN_INTERESSENTEN, 'gebrauchtwagen_interessenten', _('Interested in used cars')),
     (INAPP_AUDIENCE_B2B_AUTOMOTIVE, 'b2b_automotive', _('B2B Automotive')),
     (INAPP_AUDIENCE_AUTOBESITZER, 'autobesitzer', _('Car owners')),
     (INAPP_AUDIENCE_SERIENJUNKIES, 'serienjunkies', _('Series junkies')),
     (INAPP_AUDIENCE_HEAVY_STREAMER, 'heavy_streamer', _('Heavy streamers')),
     (INAPP_AUDIENCE_MOVIE_LOVER, 'movie_lover', _('Movie lovers')),
     (INAPP_AUDIENCE_ENTERTAINMENT_LOVER, 'entertainment_lover', _('Entertainment lovers')),
```

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/v3/serializer.py` & `easys-ordermanager-2.1.3/easys_ordermanager/v3/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,14 +529,15 @@
     (DISPLAY_CHANNEL_TRAVEL, 'travel', _('Travel')),
     (DISPLAY_CHANNEL_WOMEN, 'women', _('Women')),
     (DISPLAY_CHANNEL_CONSTRUCTION_AND_LIVING, 'construction_and_living', _('Construction & Living')),
     (DISPLAY_CHANNEL_MEN, 'men', _('Men')),
     (DISPLAY_CHANNEL_EAT_AND_DRINK, 'eat_and_drink', _('Eating & Drinking')),
 )
 
+INAPP_AUDIENCE_EMPTY = 0
 INAPP_AUDIENCE_GEBRAUCHTWAGEN_INTERESSENTEN = 1
 INAPP_AUDIENCE_B2B_AUTOMOTIVE = 2
 INAPP_AUDIENCE_AUTOBESITZER = 3
 INAPP_AUDIENCE_SERIENJUNKIES = 4
 INAPP_AUDIENCE_HEAVY_STREAMER = 5
 INAPP_AUDIENCE_MOVIE_LOVER = 6
 INAPP_AUDIENCE_ENTERTAINMENT_LOVER = 7
@@ -571,14 +572,15 @@
 INAPP_AUDIENCE_MILLENIALS = 36
 INAPP_AUDIENCE_MOMS_KIDS = 37
 INAPP_AUDIENCE_FAMILIENVATER = 38
 INAPP_AUDIENCE_BEST_AGER = 39
 INAPP_AUDIENCE_BOSSHOME = 40
 INAPP_AUDIENCE_HOBBYKOCHE = 41
 INAPP_AUDIENCE_CHOICES = Choices(
+    (INAPP_AUDIENCE_EMPTY, '', '-'),
     (INAPP_AUDIENCE_GEBRAUCHTWAGEN_INTERESSENTEN, 'gebrauchtwagen_interessenten', _('Interested in used cars')),
     (INAPP_AUDIENCE_B2B_AUTOMOTIVE, 'b2b_automotive', _('B2B Automotive')),
     (INAPP_AUDIENCE_AUTOBESITZER, 'autobesitzer', _('Car owners')),
     (INAPP_AUDIENCE_SERIENJUNKIES, 'serienjunkies', _('Series junkies')),
     (INAPP_AUDIENCE_HEAVY_STREAMER, 'heavy_streamer', _('Heavy streamers')),
     (INAPP_AUDIENCE_MOVIE_LOVER, 'movie_lover', _('Movie lovers')),
     (INAPP_AUDIENCE_ENTERTAINMENT_LOVER, 'entertainment_lover', _('Entertainment lovers')),
```

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager/validators.py` & `easys-ordermanager-2.1.3/easys_ordermanager/validators.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager.egg-info/PKG-INFO` & `easys-ordermanager-2.1.3/easys_ordermanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.2
+Version: 2.1.3
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -30,14 +30,17 @@
 ### Django 4.1
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.1.3 (2023-05-03)
+* Updates to Serializer v2 & v3, see serializer changelog
+
 ## 2.1.2 (2023-04-12)
 * Updates to Serializer v3, see serializer changelog
 * Fixed missing development dependency
 
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
@@ -426,14 +429,21 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.1.3
+
+### v2/v3
+
+#### `OrderLineInAppSerializer`
+* Added `INAPP_AUDIENCE_EMPTY` to `target_audiences` choices.
+
 ## 2.1.2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
 * Made `target_page_type` required.
 * Removed fields:
   - `expected_clicks`
   - `expected_conversions`
@@ -444,15 +454,15 @@
   - `call_to_action`
   - `is_generic_campaign`
   - `generic_topics`
   - `remarketing_setup_fee`
   - `remarketing_budget`
 
 #### `OrderLineLandingpageSerializer`
-* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required.
 
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
@@ -490,15 +500,15 @@
 
 #### `OrderLineSerializer`
 * Added new field `down_payment`, optional
 * Added new field `detail_domain` accepting `OrderLineDomainSerializer` data, optional
 
 #### `Serializer`
 
-* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain 
+* Added validation: if any OrderLine detail contains `easys_orderline_domain_id` it must reference a domain
   product provided in the same payload
 
 ## 2.0.12
 
 ### v2
 
 #### `OrderLineGoogleAdsPremiumSerializer`
```

### Comparing `easys-ordermanager-2.1.2/easys_ordermanager.egg-info/SOURCES.txt` & `easys-ordermanager-2.1.3/easys_ordermanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.2/setup.py` & `easys-ordermanager-2.1.3/setup.py`

 * *Files identical despite different names*

