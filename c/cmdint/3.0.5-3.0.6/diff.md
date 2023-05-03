# Comparing `tmp/cmdint-3.0.5.tar.gz` & `tmp/cmdint-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdint-3.0.5.tar", last modified: Tue Apr 11 07:48:47 2023, max compression
+gzip compressed data, was "cmdint-3.0.6.tar", last modified: Wed May  3 13:46:56 2023, max compression
```

## Comparing `cmdint-3.0.5.tar` & `cmdint-3.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/
--rw-rw-r--   0 neher     (1000) neher     (1000)    10172 2022-09-28 07:02:18.000000 cmdint-3.0.5/LICENSE
--rw-rw-r--   0 neher     (1000) neher     (1000)       37 2022-09-28 07:02:18.000000 cmdint-3.0.5/MANIFEST.in
--rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-11 07:48:47.701757 cmdint-3.0.5/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)     5890 2022-09-28 07:02:18.000000 cmdint-3.0.5/Readme.md
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/cmdint/
--rw-rw-r--   0 neher     (1000) neher     (1000)    47872 2023-04-11 07:47:26.000000 cmdint-3.0.5/cmdint/CmdInterface.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     3723 2022-09-28 07:02:18.000000 cmdint-3.0.5/cmdint/MessageLogger.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     6727 2022-09-28 07:09:09.000000 cmdint-3.0.5/cmdint/Utils.py
--rw-rw-r--   0 neher     (1000) neher     (1000)      201 2023-04-11 07:48:39.000000 cmdint-3.0.5/cmdint/__init__.py
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/cmdint.egg-info/
--rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)      298 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/SOURCES.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/dependency_links.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2022-09-29 13:25:31.000000 cmdint-3.0.5/cmdint.egg-info/not-zip-safe
--rw-rw-r--   0 neher     (1000) neher     (1000)       67 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/requires.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        7 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/top_level.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-04-11 07:48:47.701757 cmdint-3.0.5/setup.cfg
--rw-rw-r--   0 neher     (1000) neher     (1000)     1078 2023-04-11 07:48:39.000000 cmdint-3.0.5/setup.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-03 13:46:56.456855 cmdint-3.0.6/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    10172 2022-09-28 07:02:18.000000 cmdint-3.0.6/LICENSE
+-rw-rw-r--   0 neher     (1000) neher     (1000)       37 2022-09-28 07:02:18.000000 cmdint-3.0.6/MANIFEST.in
+-rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-05-03 13:46:56.456855 cmdint-3.0.6/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)     5890 2022-09-28 07:02:18.000000 cmdint-3.0.6/Readme.md
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-03 13:46:56.456855 cmdint-3.0.6/cmdint/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    48144 2023-05-03 13:45:44.000000 cmdint-3.0.6/cmdint/CmdInterface.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3723 2022-09-28 07:02:18.000000 cmdint-3.0.6/cmdint/MessageLogger.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     6727 2022-09-28 07:09:09.000000 cmdint-3.0.6/cmdint/Utils.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)      201 2023-05-03 13:46:47.000000 cmdint-3.0.6/cmdint/__init__.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-03 13:46:56.456855 cmdint-3.0.6/cmdint.egg-info/
+-rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-05-03 13:46:56.000000 cmdint-3.0.6/cmdint.egg-info/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)      298 2023-05-03 13:46:56.000000 cmdint-3.0.6/cmdint.egg-info/SOURCES.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-05-03 13:46:56.000000 cmdint-3.0.6/cmdint.egg-info/dependency_links.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2022-09-29 13:25:31.000000 cmdint-3.0.6/cmdint.egg-info/not-zip-safe
+-rw-rw-r--   0 neher     (1000) neher     (1000)       67 2023-05-03 13:46:56.000000 cmdint-3.0.6/cmdint.egg-info/requires.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        7 2023-05-03 13:46:56.000000 cmdint-3.0.6/cmdint.egg-info/top_level.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-05-03 13:46:56.456855 cmdint-3.0.6/setup.cfg
+-rw-rw-r--   0 neher     (1000) neher     (1000)     1078 2023-05-03 13:46:47.000000 cmdint-3.0.6/setup.py
```

### Comparing `cmdint-3.0.5/LICENSE` & `cmdint-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.5/PKG-INFO` & `cmdint-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdint
-Version: 3.0.5
+Version: 3.0.6
 Summary: Enables detailed logging of command line calls in a very lightweight manner.
 Home-page: https://github.com/MIC-DKFZ/cmdint/
 Author: Peter F. Neher
 Author-email: p.neher@dkfz.de
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmdint-3.0.5/Readme.md` & `cmdint-3.0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.5/cmdint/CmdInterface.py` & `cmdint-3.0.6/cmdint/CmdInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,18 @@
 
         if tar is not None:
             tar.close()
 
         start_time = datetime.now()
         self.__log['time']['start'] = start_time.strftime("%Y-%m-%d %H:%M:%S")
         self.__log['time']['utc_offset'] = time.localtime().tm_gmtoff
-        CmdInterface.log_message('START: ' + self.__log['name'] + ', ' + self.__log['description'])
+        if self.__log['description'] is not None:
+            CmdInterface.log_message('START: ' + self.__log['name'] + ', ' + self.__log['description'])
+        else:
+            CmdInterface.log_message('START: ' + self.__log['name'])
         if CmdInterface.__message_log_level == MessageLogLevel.START_AND_END_MESSAGES and not self.__silent:
             CmdInterface.send_message('START ' + self.__log['name'])
         return start_time
 
     def __log_end(self, start_time: datetime, return_code: int) -> datetime:
         """
         Log end time and duration of command execution:
@@ -530,15 +533,18 @@
         hours, remainder = divmod(duration.seconds, 3600)
         hours += duration.days * 24
         minutes, seconds = divmod(remainder, 60)
         duration_formatted = '%d:%02d:%02d' % (hours, minutes, seconds)
         self.__log['time']['duration'] = duration_formatted
 
         # log end messages & return code
-        CmdInterface.log_message('END: ' + self.__log['name'] + ', ' + self.__log['description'])
+        if self.__log['description'] is not None:
+            CmdInterface.log_message('END: ' + self.__log['name'] + ', ' + self.__log['description'])
+        else:
+            CmdInterface.log_message('END: ' + self.__log['name'])
         if (CmdInterface.__throw_on_error or CmdInterface.__exit_on_error) and return_code <= 0:
             print('EXCEPTION:', self.__log['name'], self.__log['description'])
             CmdInterface.log_message('Exiting due to error: ' + self.__return_code_meanings[return_code])
         self.__log['return_code'] = return_code
         self.update_log()
 
         if not self.__silent and \
```

### Comparing `cmdint-3.0.5/cmdint/MessageLogger.py` & `cmdint-3.0.6/cmdint/MessageLogger.py`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.5/cmdint/Utils.py` & `cmdint-3.0.6/cmdint/Utils.py`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.5/cmdint.egg-info/PKG-INFO` & `cmdint-3.0.6/cmdint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdint
-Version: 3.0.5
+Version: 3.0.6
 Summary: Enables detailed logging of command line calls in a very lightweight manner.
 Home-page: https://github.com/MIC-DKFZ/cmdint/
 Author: Peter F. Neher
 Author-email: p.neher@dkfz.de
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmdint-3.0.5/setup.py` & `cmdint-3.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='cmdint',
-      version='3.0.5',
+      version='3.0.6',
       description='Enables detailed logging of command line calls in a very lightweight manner.',
       long_description='CmdInterface enables detailed logging of command line and python experiments in a very lightweight manner (coding wise). It wraps your command line or python function calls in a few lines of code and logs everything you might need to reproduce the experiment later on or to simply check what you did a couple of years ago.',
       url='https://github.com/MIC-DKFZ/cmdint/',
       author='Peter F. Neher',
       author_email='p.neher@dkfz.de',
       license='Apache 2.0',
       packages=['cmdint'],
```

