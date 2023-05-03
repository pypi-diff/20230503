# Comparing `tmp/remindmail-2023.5.1.1.tar.gz` & `tmp/remindmail-2023.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.5.1.1.tar", last modified: Mon May  1 17:11:59 2023, max compression
+gzip compressed data, was "remindmail-2023.5.3.1.tar", last modified: Wed May  3 20:03:47 2023, max compression
```

## Comparing `remindmail-2023.5.1.1.tar` & `remindmail-2023.5.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.5.1.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.5.1.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.5.1.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.5.1.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.5.1.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.5.1.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25042 2023-05-01 17:09:57.000000 remindmail-2023.5.1.1/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.5.1.1/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 17:11:59.810828 remindmail-2023.5.1.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-01 17:11:59.000000 remindmail-2023.5.1.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-01 17:11:59.000000 remindmail-2023.5.1.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-01 17:11:59.000000 remindmail-2023.5.1.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-01 17:11:59.000000 remindmail-2023.5.1.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-01 17:11:59.000000 remindmail-2023.5.1.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.5.3.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.5.3.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.5.3.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    25030 2023-05-03 20:03:29.000000 remindmail-2023.5.3.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.5.3.1/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-03 20:03:47.013663 remindmail-2023.5.3.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-03 20:03:47.000000 remindmail-2023.5.3.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.5.1.1/LICENSE.md` & `remindmail-2023.5.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.1.1/PKG-INFO` & `remindmail-2023.5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.5.1.1
+Version: 2023.5.3.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2023.5.1.1/README.md` & `remindmail-2023.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.1.1/setup.cfg` & `remindmail-2023.5.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.05.01.1
+version = 2023.05.03.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.5.1.1/src/remind/__main__.py` & `remindmail-2023.5.3.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.1.1/src/remind/reminder.py` & `remindmail-2023.5.3.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.1.1/src/remind/remindmail.py` & `remindmail-2023.5.3.1/src/remind/remindmail.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             "remindmail", "day_generated")
 
         if day_of_month_reminders_generated == '':
             day_of_month_reminders_generated = 0
 
         # do not generate more than once in one day unless `remind generate force`
         if not (today_index != day_of_month_reminders_generated
-                and generate_date.hour > 3) and not force and not dry_run:
+                and datetime.today().hour > 3) and not force and not dry_run:
             RemindMail().log_msg(
-                "Reminders have already been generated in the past 12 hours.", level="debug")
+                "Reminders have already been generated today.", level="debug")
             return
 
         RemindMail().log_msg("Generating reminders")
 
         command = ''
 
         current_time = RemindMailUtils().get_user_time()
```

### Comparing `remindmail-2023.5.1.1/src/remind/remindmail_utils.py` & `remindmail-2023.5.3.1/src/remind/remindmail_utils.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.5.1.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.5.3.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.5.1.1
+Version: 2023.5.3.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

