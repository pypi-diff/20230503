# Comparing `tmp/homewizard-kitchen-0.2.3.tar.gz` & `tmp/homewizard-kitchen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homewizard-kitchen-0.2.3.tar", last modified: Wed May  3 20:40:18 2023, max compression
+gzip compressed data, was "homewizard-kitchen-0.3.0.tar", last modified: Wed May  3 20:45:09 2023, max compression
```

## Comparing `homewizard-kitchen-0.2.3.tar` & `homewizard-kitchen-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.989082 homewizard-kitchen-0.2.3/
--rw-rw-rw-   0        0        0     1094 2023-02-04 15:20:26.000000 homewizard-kitchen-0.2.3/LICENSE.md
--rw-rw-rw-   0        0        0      902 2023-05-03 20:40:18.989082 homewizard-kitchen-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-02-19 22:51:12.000000 homewizard-kitchen-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.966072 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/
--rw-rw-rw-   0        0        0      902 2023-05-03 20:40:18.000000 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-05-03 20:40:18.000000 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:40:18.000000 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-03 20:40:18.000000 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 20:40:18.000000 homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.972166 homewizard-kitchen-0.2.3/hwkitchen/
--rw-rw-rw-   0        0        0       70 2023-02-04 13:37:39.000000 homewizard-kitchen-0.2.3/hwkitchen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.972166 homewizard-kitchen-0.2.3/hwkitchen/enums/
--rw-rw-rw-   0        0        0       39 2023-02-20 23:22:21.000000 homewizard-kitchen-0.2.3/hwkitchen/enums/__init__.py
--rw-rw-rw-   0        0        0      282 2023-03-10 12:45:07.000000 homewizard-kitchen-0.2.3/hwkitchen/enums/kettle_status.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.980998 homewizard-kitchen-0.2.3/hwkitchen/models/
--rw-rw-rw-   0        0        0       26 2023-02-04 13:37:12.000000 homewizard-kitchen-0.2.3/hwkitchen/models/__init__.py
--rw-rw-rw-   0        0        0     2837 2023-02-20 01:29:43.000000 homewizard-kitchen-0.2.3/hwkitchen/models/kettle.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:40:18.980998 homewizard-kitchen-0.2.3/hwkitchen/services/
--rw-rw-rw-   0        0        0       33 2023-02-25 18:54:47.000000 homewizard-kitchen-0.2.3/hwkitchen/services/__init__.py
--rw-rw-rw-   0        0        0     7881 2023-02-25 22:52:34.000000 homewizard-kitchen-0.2.3/hwkitchen/services/hw_socket.py
--rw-rw-rw-   0        0        0      594 2023-05-03 20:39:36.000000 homewizard-kitchen-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 20:40:18.989082 homewizard-kitchen-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.473103 homewizard-kitchen-0.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-02-04 15:20:26.000000 homewizard-kitchen-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0      902 2023-05-03 20:45:09.472078 homewizard-kitchen-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-02-19 22:51:12.000000 homewizard-kitchen-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.470079 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/
+-rw-rw-rw-   0        0        0      902 2023-05-03 20:45:09.000000 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-05-03 20:45:09.000000 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 20:45:09.000000 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 20:45:09.000000 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 20:45:09.000000 homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.470079 homewizard-kitchen-0.3.0/hwkitchen/
+-rw-rw-rw-   0        0        0       70 2023-02-04 13:37:39.000000 homewizard-kitchen-0.3.0/hwkitchen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.471079 homewizard-kitchen-0.3.0/hwkitchen/enums/
+-rw-rw-rw-   0        0        0       39 2023-02-20 23:22:21.000000 homewizard-kitchen-0.3.0/hwkitchen/enums/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-03-10 12:45:07.000000 homewizard-kitchen-0.3.0/hwkitchen/enums/kettle_status.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.471079 homewizard-kitchen-0.3.0/hwkitchen/models/
+-rw-rw-rw-   0        0        0       26 2023-02-04 13:37:12.000000 homewizard-kitchen-0.3.0/hwkitchen/models/__init__.py
+-rw-rw-rw-   0        0        0     2837 2023-02-20 01:29:43.000000 homewizard-kitchen-0.3.0/hwkitchen/models/kettle.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:45:09.472078 homewizard-kitchen-0.3.0/hwkitchen/services/
+-rw-rw-rw-   0        0        0       33 2023-02-25 18:54:47.000000 homewizard-kitchen-0.3.0/hwkitchen/services/__init__.py
+-rw-rw-rw-   0        0        0     7881 2023-02-25 22:52:34.000000 homewizard-kitchen-0.3.0/hwkitchen/services/hw_socket.py
+-rw-rw-rw-   0        0        0      617 2023-05-03 20:45:01.000000 homewizard-kitchen-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 20:45:09.473103 homewizard-kitchen-0.3.0/setup.cfg
```

### Comparing `homewizard-kitchen-0.2.3/LICENSE.md` & `homewizard-kitchen-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `homewizard-kitchen-0.2.3/PKG-INFO` & `homewizard-kitchen-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homewizard-kitchen
-Version: 0.2.3
+Version: 0.3.0
 Summary: Manage your Homewizard Kitchen Kettle using Python
 Author-email: Lesley De Keyser <me@lesley.co>
 Project-URL: Homepage, https://github.com/lesleyxyz/python-homewizard-kitchen
 Project-URL: Bug Tracker, https://github.com/lesleyxyz/python-homewizard-kitchen/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `homewizard-kitchen-0.2.3/homewizard_kitchen.egg-info/PKG-INFO` & `homewizard-kitchen-0.3.0/homewizard_kitchen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homewizard-kitchen
-Version: 0.2.3
+Version: 0.3.0
 Summary: Manage your Homewizard Kitchen Kettle using Python
 Author-email: Lesley De Keyser <me@lesley.co>
 Project-URL: Homepage, https://github.com/lesleyxyz/python-homewizard-kitchen
 Project-URL: Bug Tracker, https://github.com/lesleyxyz/python-homewizard-kitchen/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `homewizard-kitchen-0.2.3/hwkitchen/models/kettle.py` & `homewizard-kitchen-0.3.0/hwkitchen/models/kettle.py`

 * *Files identical despite different names*

### Comparing `homewizard-kitchen-0.2.3/hwkitchen/services/hw_socket.py` & `homewizard-kitchen-0.3.0/hwkitchen/services/hw_socket.py`

 * *Files identical despite different names*

### Comparing `homewizard-kitchen-0.2.3/pyproject.toml` & `homewizard-kitchen-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "homewizard-kitchen"
-version = "0.2.3"
+version = "0.3.0"
 authors = [
     { name="Lesley De Keyser", email="me@lesley.co" },
 ]
 description = "Manage your Homewizard Kitchen Kettle using Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
 dependencies = [
     "websockets>=10.0",
     "httpx>=0.10.0",
+    "jsonpatch>1.20",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lesleyxyz/python-homewizard-kitchen"
 "Bug Tracker" = "https://github.com/lesleyxyz/python-homewizard-kitchen/issues"
 
 [build-system]
```

