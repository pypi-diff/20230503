# Comparing `tmp/MKN_third_codes-0.6.4.4.tar.gz` & `tmp/MKN_third_codes-0.6.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.4.4.tar", last modified: Wed May  3 09:26:05 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.4.5.tar", last modified: Wed May  3 09:27:46 2023, max compression
```

## Comparing `MKN_third_codes-0.6.4.4.tar` & `MKN_third_codes-0.6.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:05.269879 MKN_third_codes-0.6.4.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:05.258908 MKN_third_codes-0.6.4.4/MKN_third_codes/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:05.268882 MKN_third_codes-0.6.4.4/MKN_third_codes/constructions/
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.4.4/MKN_third_codes/constructions/mkn_globals.py
--rw-rw-rw-   0        0        0     9637 2023-05-03 09:23:06.000000 MKN_third_codes-0.6.4.4/MKN_third_codes/constructions/mkn_utils.py
--rw-rw-rw-   0        0        0    28008 2023-05-03 09:23:26.000000 MKN_third_codes-0.6.4.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:05.266888 MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7542 2023-05-03 09:26:05.000000 MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-03 09:26:05.000000 MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:26:05.000000 MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 09:26:05.000000 MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7542 2023-05-03 09:26:05.269879 MKN_third_codes-0.6.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     4322 2023-05-03 09:25:35.000000 MKN_third_codes-0.6.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 09:26:05.269879 MKN_third_codes-0.6.4.4/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-03 09:26:03.000000 MKN_third_codes-0.6.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:27:46.154405 MKN_third_codes-0.6.4.5/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 09:27:46.143435 MKN_third_codes-0.6.4.5/MKN_third_codes/
+drwxrwxrwx   0        0        0        0 2023-05-03 09:27:46.152411 MKN_third_codes-0.6.4.5/MKN_third_codes/constructions/
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.4.5/MKN_third_codes/constructions/mkn_globals.py
+-rw-rw-rw-   0        0        0     9637 2023-05-03 09:23:06.000000 MKN_third_codes-0.6.4.5/MKN_third_codes/constructions/mkn_utils.py
+-rw-rw-rw-   0        0        0    28008 2023-05-03 09:23:26.000000 MKN_third_codes-0.6.4.5/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:27:46.151414 MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7542 2023-05-03 09:27:46.000000 MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-03 09:27:46.000000 MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:27:46.000000 MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 09:27:46.000000 MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7542 2023-05-03 09:27:46.153408 MKN_third_codes-0.6.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4322 2023-05-03 09:25:35.000000 MKN_third_codes-0.6.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:27:46.154405 MKN_third_codes-0.6.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-03 09:27:32.000000 MKN_third_codes-0.6.4.5/setup.py
```

### Comparing `MKN_third_codes-0.6.4.4/LICENSE.txt` & `MKN_third_codes-0.6.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.4/MKN_third_codes/constructions/mkn_globals.py` & `MKN_third_codes-0.6.4.5/MKN_third_codes/constructions/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.4/MKN_third_codes/constructions/mkn_utils.py` & `MKN_third_codes-0.6.4.5/MKN_third_codes/constructions/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.4.5/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.4.5/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.4.4
+Version: 0.6.4.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -57,21 +57,21 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
-## 0.6.4.3 (02/05/2023)
+## 0.6.4.5 (03/05/2023)
 ```
 ------------------
 ━ Да как нормально настроить импорты???
 ------------------
 ```
-## 0.6.4.2 (02/05/2023)
+## 0.6.4.2 (03/05/2023)
 ```
 ------------------
 ┏ исправленная структуризация проекта
 ┃   ┣ global_variables -переименовано-> mkn_globals
 ┃   ┣ utils -переименовано-> mkn_utils
 ┃   ┗ combinations перемещено в mkn_globals
 ┗ структура изменена
```

### Comparing `MKN_third_codes-0.6.4.4/PKG-INFO` & `MKN_third_codes-0.6.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.4.4
+Version: 0.6.4.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -57,21 +57,21 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
-## 0.6.4.3 (02/05/2023)
+## 0.6.4.5 (03/05/2023)
 ```
 ------------------
 ━ Да как нормально настроить импорты???
 ------------------
 ```
-## 0.6.4.2 (02/05/2023)
+## 0.6.4.2 (03/05/2023)
 ```
 ------------------
 ┏ исправленная структуризация проекта
 ┃   ┣ global_variables -переименовано-> mkn_globals
 ┃   ┣ utils -переименовано-> mkn_utils
 ┃   ┗ combinations перемещено в mkn_globals
 ┗ структура изменена
```

### Comparing `MKN_third_codes-0.6.4.4/README.md` & `MKN_third_codes-0.6.4.5/README.md`

 * *Files identical despite different names*

