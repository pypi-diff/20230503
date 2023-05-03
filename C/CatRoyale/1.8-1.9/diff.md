# Comparing `tmp/CatRoyale-1.8.tar.gz` & `tmp/CatRoyale-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CatRoyale-1.8.tar", last modified: Mon May  1 11:12:11 2023, max compression
+gzip compressed data, was "CatRoyale-1.9.tar", last modified: Mon May  1 11:14:58 2023, max compression
```

## Comparing `CatRoyale-1.8.tar` & `CatRoyale-1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.943647 CatRoyale-1.8/
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.892650 CatRoyale-1.8/CatRoyale.egg-info/
--rw-rw-rw-   0        0        0      222 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 11:12:11.000000 CatRoyale-1.8/CatRoyale.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       78 2023-05-01 11:05:27.000000 CatRoyale-1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      222 2023-05-01 11:12:11.943647 CatRoyale-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-01 10:48:10.000000 CatRoyale-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.895648 CatRoyale-1.8/assets/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:54:38.000000 CatRoyale-1.8/assets/__init__.py
--rw-rw-rw-   0        0        0      528 2023-04-23 11:35:23.000000 CatRoyale-1.8/assets/image_locations.json
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.909654 CatRoyale-1.8/assets/images/
--rw-rw-rw-   0        0        0      455 2023-03-25 12:46:51.000000 CatRoyale-1.8/assets/images/Inventory_Bar.png
--rw-rw-rw-   0        0        0      212 2023-03-25 12:46:51.000000 CatRoyale-1.8/assets/images/Inventory_Slot.png
--rw-rw-rw-   0        0        0      214 2023-03-25 12:46:51.000000 CatRoyale-1.8/assets/images/Inventory_select.png
--rw-rw-rw-   0        0        0      498 2023-04-24 15:22:32.000000 CatRoyale-1.8/assets/images/arrow.png
--rw-rw-rw-   0        0        0    12841 2023-03-25 16:24:31.000000 CatRoyale-1.8/assets/images/cat.png
--rw-rw-rw-   0        0        0    27199 2023-04-22 14:53:45.000000 CatRoyale-1.8/assets/images/enemy_cat.png
--rw-rw-rw-   0        0        0     2170 2023-03-22 21:48:06.000000 CatRoyale-1.8/assets/images/grass.png
--rw-rw-rw-   0        0        0   127269 2023-03-22 20:35:26.000000 CatRoyale-1.8/assets/images/items.png
--rw-rw-rw-   0        0        0    19155 2023-03-28 16:20:17.000000 CatRoyale-1.8/assets/images/loading_screen.png
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.911652 CatRoyale-1.8/assets/images/map/
--rw-rw-rw-   0        0        0     2795 2023-04-26 18:20:17.000000 CatRoyale-1.8/assets/images/map/level00.png
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.938645 CatRoyale-1.8/classes/
--rw-rw-rw-   0        0        0        0 2023-04-22 13:48:02.000000 CatRoyale-1.8/classes/__init__.py
--rw-rw-rw-   0        0        0     5339 2023-05-01 10:16:04.000000 CatRoyale-1.8/classes/box.py
--rw-rw-rw-   0        0        0    24994 2023-05-01 10:34:53.000000 CatRoyale-1.8/classes/character.py
--rw-rw-rw-   0        0        0      996 2023-05-01 10:31:13.000000 CatRoyale-1.8/classes/config.py
--rw-rw-rw-   0        0        0     2077 2023-05-01 10:14:35.000000 CatRoyale-1.8/classes/event_stack.py
--rw-rw-rw-   0        0        0     1054 2023-05-01 10:23:12.000000 CatRoyale-1.8/classes/functions.py
--rw-rw-rw-   0        0        0     3741 2023-05-01 10:26:03.000000 CatRoyale-1.8/classes/game_map.py
--rw-rw-rw-   0        0        0     2193 2023-05-01 08:26:56.000000 CatRoyale-1.8/classes/health_bars.py
--rw-rw-rw-   0        0        0    14266 2023-05-01 10:27:16.000000 CatRoyale-1.8/classes/inventory.py
--rw-rw-rw-   0        0        0     4440 2023-05-01 10:05:02.000000 CatRoyale-1.8/classes/item.py
--rw-rw-rw-   0        0        0      521 2023-05-01 10:06:08.000000 CatRoyale-1.8/classes/map_reader.py
--rw-rw-rw-   0        0        0      362 2023-05-01 10:10:10.000000 CatRoyale-1.8/classes/message_service.py
--rw-rw-rw-   0        0        0     1718 2023-04-30 19:32:21.000000 CatRoyale-1.8/classes/text_display.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:12:11.942651 CatRoyale-1.8/config/
--rw-rw-rw-   0        0        0        0 2023-05-01 11:05:20.000000 CatRoyale-1.8/config/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-04-30 19:34:37.000000 CatRoyale-1.8/config/config.json
--rw-rw-rw-   0        0        0    15824 2023-05-01 10:34:59.000000 CatRoyale-1.8/main.py
--rw-rw-rw-   0        0        0       88 2023-05-01 10:53:12.000000 CatRoyale-1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 11:12:11.944648 CatRoyale-1.8/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-05-01 11:12:02.000000 CatRoyale-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.497570 CatRoyale-1.9/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.452561 CatRoyale-1.9/CatRoyale.egg-info/
+-rw-rw-rw-   0        0        0      222 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 11:14:58.000000 CatRoyale-1.9/CatRoyale.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       78 2023-05-01 11:05:27.000000 CatRoyale-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      222 2023-05-01 11:14:58.496570 CatRoyale-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-05-01 10:48:10.000000 CatRoyale-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.454562 CatRoyale-1.9/assets/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:54:38.000000 CatRoyale-1.9/assets/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-04-23 11:35:23.000000 CatRoyale-1.9/assets/image_locations.json
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.466564 CatRoyale-1.9/assets/images/
+-rw-rw-rw-   0        0        0      455 2023-03-25 12:46:51.000000 CatRoyale-1.9/assets/images/Inventory_Bar.png
+-rw-rw-rw-   0        0        0      212 2023-03-25 12:46:51.000000 CatRoyale-1.9/assets/images/Inventory_Slot.png
+-rw-rw-rw-   0        0        0      214 2023-03-25 12:46:51.000000 CatRoyale-1.9/assets/images/Inventory_select.png
+-rw-rw-rw-   0        0        0      498 2023-04-24 15:22:32.000000 CatRoyale-1.9/assets/images/arrow.png
+-rw-rw-rw-   0        0        0    12841 2023-03-25 16:24:31.000000 CatRoyale-1.9/assets/images/cat.png
+-rw-rw-rw-   0        0        0    27199 2023-04-22 14:53:45.000000 CatRoyale-1.9/assets/images/enemy_cat.png
+-rw-rw-rw-   0        0        0     2170 2023-03-22 21:48:06.000000 CatRoyale-1.9/assets/images/grass.png
+-rw-rw-rw-   0        0        0   127269 2023-03-22 20:35:26.000000 CatRoyale-1.9/assets/images/items.png
+-rw-rw-rw-   0        0        0    19155 2023-03-28 16:20:17.000000 CatRoyale-1.9/assets/images/loading_screen.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.468561 CatRoyale-1.9/assets/images/map/
+-rw-rw-rw-   0        0        0     2795 2023-04-26 18:20:17.000000 CatRoyale-1.9/assets/images/map/level00.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.492572 CatRoyale-1.9/classes/
+-rw-rw-rw-   0        0        0        0 2023-04-22 13:48:02.000000 CatRoyale-1.9/classes/__init__.py
+-rw-rw-rw-   0        0        0     5339 2023-05-01 10:16:04.000000 CatRoyale-1.9/classes/box.py
+-rw-rw-rw-   0        0        0    24994 2023-05-01 10:34:53.000000 CatRoyale-1.9/classes/character.py
+-rw-rw-rw-   0        0        0      996 2023-05-01 10:31:13.000000 CatRoyale-1.9/classes/config.py
+-rw-rw-rw-   0        0        0     2077 2023-05-01 10:14:35.000000 CatRoyale-1.9/classes/event_stack.py
+-rw-rw-rw-   0        0        0     1054 2023-05-01 10:23:12.000000 CatRoyale-1.9/classes/functions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-01 10:26:03.000000 CatRoyale-1.9/classes/game_map.py
+-rw-rw-rw-   0        0        0     2193 2023-05-01 08:26:56.000000 CatRoyale-1.9/classes/health_bars.py
+-rw-rw-rw-   0        0        0    14266 2023-05-01 10:27:16.000000 CatRoyale-1.9/classes/inventory.py
+-rw-rw-rw-   0        0        0     4440 2023-05-01 10:05:02.000000 CatRoyale-1.9/classes/item.py
+-rw-rw-rw-   0        0        0      521 2023-05-01 10:06:08.000000 CatRoyale-1.9/classes/map_reader.py
+-rw-rw-rw-   0        0        0      362 2023-05-01 10:10:10.000000 CatRoyale-1.9/classes/message_service.py
+-rw-rw-rw-   0        0        0     1718 2023-04-30 19:32:21.000000 CatRoyale-1.9/classes/text_display.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:14:58.495565 CatRoyale-1.9/config/
+-rw-rw-rw-   0        0        0        0 2023-05-01 11:05:20.000000 CatRoyale-1.9/config/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-04-30 19:34:37.000000 CatRoyale-1.9/config/config.json
+-rw-rw-rw-   0        0        0    15824 2023-05-01 10:34:59.000000 CatRoyale-1.9/main.py
+-rw-rw-rw-   0        0        0       88 2023-05-01 10:53:12.000000 CatRoyale-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:14:58.497570 CatRoyale-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-01 11:14:49.000000 CatRoyale-1.9/setup.py
```

### Comparing `CatRoyale-1.8/CatRoyale.egg-info/SOURCES.txt` & `CatRoyale-1.9/CatRoyale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/image_locations.json` & `CatRoyale-1.9/assets/image_locations.json`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/cat.png` & `CatRoyale-1.9/assets/images/cat.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/enemy_cat.png` & `CatRoyale-1.9/assets/images/enemy_cat.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/grass.png` & `CatRoyale-1.9/assets/images/grass.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/items.png` & `CatRoyale-1.9/assets/images/items.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/loading_screen.png` & `CatRoyale-1.9/assets/images/loading_screen.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/assets/images/map/level00.png` & `CatRoyale-1.9/assets/images/map/level00.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/box.py` & `CatRoyale-1.9/classes/box.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/character.py` & `CatRoyale-1.9/classes/character.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/config.py` & `CatRoyale-1.9/classes/config.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/event_stack.py` & `CatRoyale-1.9/classes/event_stack.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/functions.py` & `CatRoyale-1.9/classes/functions.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/game_map.py` & `CatRoyale-1.9/classes/game_map.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/health_bars.py` & `CatRoyale-1.9/classes/health_bars.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/inventory.py` & `CatRoyale-1.9/classes/inventory.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/item.py` & `CatRoyale-1.9/classes/item.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/map_reader.py` & `CatRoyale-1.9/classes/map_reader.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/classes/text_display.py` & `CatRoyale-1.9/classes/text_display.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/config/config.json` & `CatRoyale-1.9/config/config.json`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/main.py` & `CatRoyale-1.9/main.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.8/setup.py` & `CatRoyale-1.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="CatRoyale",
-    version="1.8",
+    version="1.9",
     description="A cat themed battle royale game",
     author="Tarsoly Barnabás",
     author_email="tarsoly.barnabas2002@gmail.com",
     url="https://github.com/Iseroo/Python-kotprog",
     packages=["classes", "assets", "config"],
     py_modules=["main"],
     install_requires=["pygame", "webcolors", "pillow", "ordered_set"],
     include_package_data=True,
     entry_points={
         'console_scripts': [
-            'CatRoyale = CatRoyale:main'
+            'CatRoyale = main'
         ]
     },
 
 )
```

