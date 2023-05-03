# Comparing `tmp/decentralizedroutines-2.0.2.tar.gz` & `tmp/decentralizedroutines-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.0.2.tar", last modified: Wed May  3 15:06:31 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.0.3.tar", last modified: Wed May  3 16:35:32 2023, max compression
```

## Comparing `decentralizedroutines-2.0.2.tar` & `decentralizedroutines-2.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/
--rw-rw-rw-   0        0        0    35823 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     1159 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      505 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/README.md
--rw-rw-rw-   0        0        0      108 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      865 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.327675 decentralizedroutines-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.336435 decentralizedroutines-2.0.2/src/decentralizedroutines/
--rw-rw-rw-   0        0        0    10251 2023-05-03 15:05:33.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-rw-   0        0        0        0 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/__init__.py
--rw-rw-rw-   0        0        0      648 2022-12-19 22:11:23.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/defaults.py
--rw-rw-rw-   0        0        0     1301 2023-01-16 18:07:39.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/master.py
--rw-rw-rw-   0        0        0     1352 2023-02-28 18:56:12.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/runroutines.py
--rw-rw-rw-   0        0        0     3367 2023-01-14 21:08:08.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/schedule_sequence.py
--rw-rw-rw-   0        0        0     1982 2022-12-11 09:13:36.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/update_version_requirements.py
--rw-rw-rw-   0        0        0     8934 2023-02-28 12:30:21.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/worker.py
--rw-rw-rw-   0        0        0     9542 2023-02-27 10:18:30.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/worker_lib.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.346436 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 16:35:32.418889 decentralizedroutines-2.0.3/
+-rw-rw-rw-   0        0        0    35823 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1159 2023-05-03 16:35:32.418889 decentralizedroutines-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      865 2023-05-03 16:35:32.421889 decentralizedroutines-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 16:35:32.397889 decentralizedroutines-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 16:35:32.408891 decentralizedroutines-2.0.3/src/decentralizedroutines/
+-rw-rw-rw-   0        0        0    10305 2023-05-03 16:35:19.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-rw-   0        0        0        0 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/__init__.py
+-rw-rw-rw-   0        0        0      648 2022-12-19 22:11:23.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/defaults.py
+-rw-rw-rw-   0        0        0     1301 2023-01-16 18:07:39.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/master.py
+-rw-rw-rw-   0        0        0     1352 2023-02-28 18:56:12.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/runroutines.py
+-rw-rw-rw-   0        0        0     3367 2023-01-14 21:08:08.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/schedule_sequence.py
+-rw-rw-rw-   0        0        0     1982 2022-12-11 09:13:36.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-rw-   0        0        0     8934 2023-02-28 12:30:21.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/worker.py
+-rw-rw-rw-   0        0        0     9542 2023-02-27 10:18:30.000000 decentralizedroutines-2.0.3/src/decentralizedroutines/worker_lib.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:35:32.418889 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/
+-rw-rw-rw-   0        0        0     1159 2023-05-03 16:35:32.000000 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-05-03 16:35:32.000000 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:35:32.000000 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-03 16:35:32.000000 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-03 16:35:32.000000 decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.0.2/LICENSE` & `decentralizedroutines-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/PKG-INFO` & `decentralizedroutines-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.0.2
+Version: 2.0.3
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.0.2/setup.cfg` & `decentralizedroutines-2.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6563 656e 7472 616c 697a 6564   = decentralized
 00000020: 726f 7574 696e 6573 0d0a 7665 7273 696f  routines..versio
-00000030: 6e20 3d20 322e 302e 320d 0a61 7574 686f  n = 2.0.2..autho
+00000030: 6e20 3d20 322e 302e 330d 0a61 7574 686f  n = 2.0.3..autho
 00000040: 7220 3d20 4a6f 7365 2043 6172 6c69 746f  r = Jose Carlito
 00000050: 2064 6520 4f6c 6976 6569 7261 2046 696c   de Oliveira Fil
 00000060: 686f 0d0a 6175 7468 6f72 5f65 6d61 696c  ho..author_email
 00000070: 203d 206a 6361 726c 6974 6f6f 6c69 7665   = jcarlitoolive
 00000080: 6972 6140 676d 6169 6c2e 636f 6d0d 0a64  ira@gmail.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 204d 6173  escription = Mas
 000000a0: 7465 722f 576f 726b 6572 2069 6d70 6c65  ter/Worker imple
```

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/RoutineScheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                 s['Run Times'] = dttm
                 sched = sched.reindex(columns=s.index.union(sched.columns))
                 sched = pd.concat([sched, pd.DataFrame(s).T])
 
         sched = sched.sort_values(by=['Run Times','Name']).reset_index(drop=True)
         sched['Status'] = np.nan
         sched['Last Message'] = np.nan
-        sched['index'] = [s.lower() for s in sched['index']]
+        sched['index'] = [s.lower().replace('\\','/') for s in sched['index']]
         sched.loc[sched['Dependencies'].isnull(),'Dependencies'] = ''
-        sched['Dependencies'] = [s.lower() for s in sched['Dependencies']]
+        sched['Dependencies'] = [s.lower().replace('\\','/') for s in sched['Dependencies']]
 
 
         uruntimes = sched['Run Times'].unique()
         runtime = uruntimes[0]
         sched_sort = pd.DataFrame(columns=sched.columns)
         for runtime in uruntimes:
             # mark pending routines
@@ -96,15 +96,15 @@
     def UpdateRoutinesStatus(self):
         sched = self.schedule                
         local_tz = pytz.timezone(str(get_localzone()))
         # RefreshLogs
         dflogs = self.consumer.readLogs()
         if not dflogs.empty:
             dflogs['index'] = dflogs['user_name']+':'+dflogs['logger_name']
-            dflogs['index'] = [s.lower() for s in dflogs['index']]
+            dflogs['index'] = [s.lower().replace('\\','/') for s in dflogs['index']]
 
             dflogs = dflogs[dflogs['asctime'].notnull()].copy()
             dflogs['asctime'] = pd.to_datetime(dflogs['asctime'])
             dflogs['asctime'] = [dt.astimezone(tz=local_tz) for dt in dflogs['asctime']]
 
             i=0
             for i in sched.index:
```

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/master.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/master.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/runroutines.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/schedule_sequence.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/schedule_sequence.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/update_version_requirements.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/worker.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.0.3/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.0.2
+Version: 2.0.3
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.0.3/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

