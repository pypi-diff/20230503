# Comparing `tmp/decentralizedroutines-2.0.1.tar.gz` & `tmp/decentralizedroutines-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.0.1.tar", last modified: Mon May  1 18:27:05 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.0.2.tar", last modified: Wed May  3 15:06:31 2023, max compression
```

## Comparing `decentralizedroutines-2.0.1.tar` & `decentralizedroutines-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 18:27:05.869331 decentralizedroutines-2.0.1/
--rw-rw-rw-   0        0        0    35823 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1159 2023-05-01 18:27:05.870333 decentralizedroutines-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      505 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.1/README.md
--rw-rw-rw-   0        0        0      108 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      865 2023-05-01 18:27:05.872333 decentralizedroutines-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 18:27:05.849332 decentralizedroutines-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 18:27:05.859333 decentralizedroutines-2.0.1/src/decentralizedroutines/
--rw-rw-rw-   0        0        0    10171 2023-02-28 13:56:02.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-rw-   0        0        0        0 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/__init__.py
--rw-rw-rw-   0        0        0      648 2022-12-19 22:11:23.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/defaults.py
--rw-rw-rw-   0        0        0     1301 2023-01-16 18:07:39.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/master.py
--rw-rw-rw-   0        0        0     1352 2023-02-28 18:56:12.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/runroutines.py
--rw-rw-rw-   0        0        0     3367 2023-01-14 21:08:08.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/schedule_sequence.py
--rw-rw-rw-   0        0        0     1982 2022-12-11 09:13:36.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/update_version_requirements.py
--rw-rw-rw-   0        0        0     8934 2023-02-28 12:30:21.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/worker.py
--rw-rw-rw-   0        0        0     9542 2023-02-27 10:18:30.000000 decentralizedroutines-2.0.1/src/decentralizedroutines/worker_lib.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:27:05.869331 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-05-01 18:27:05.000000 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-05-01 18:27:05.000000 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 18:27:05.000000 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-01 18:27:05.000000 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 18:27:05.000000 decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/
+-rw-rw-rw-   0        0        0    35823 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1159 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      865 2023-05-03 15:06:31.347435 decentralizedroutines-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.327675 decentralizedroutines-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.336435 decentralizedroutines-2.0.2/src/decentralizedroutines/
+-rw-rw-rw-   0        0        0    10251 2023-05-03 15:05:33.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-rw-   0        0        0        0 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/__init__.py
+-rw-rw-rw-   0        0        0      648 2022-12-19 22:11:23.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/defaults.py
+-rw-rw-rw-   0        0        0     1301 2023-01-16 18:07:39.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/master.py
+-rw-rw-rw-   0        0        0     1352 2023-02-28 18:56:12.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/runroutines.py
+-rw-rw-rw-   0        0        0     3367 2023-01-14 21:08:08.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/schedule_sequence.py
+-rw-rw-rw-   0        0        0     1982 2022-12-11 09:13:36.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-rw-   0        0        0     8934 2023-02-28 12:30:21.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/worker.py
+-rw-rw-rw-   0        0        0     9542 2023-02-27 10:18:30.000000 decentralizedroutines-2.0.2/src/decentralizedroutines/worker_lib.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:06:31.346436 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/
+-rw-rw-rw-   0        0        0     1159 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-03 15:06:31.000000 decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.0.1/LICENSE` & `decentralizedroutines-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/PKG-INFO` & `decentralizedroutines-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.0.1
+Version: 2.0.2
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.0.1/setup.cfg` & `decentralizedroutines-2.0.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6563 656e 7472 616c 697a 6564   = decentralized
 00000020: 726f 7574 696e 6573 0d0a 7665 7273 696f  routines..versio
-00000030: 6e20 3d20 322e 302e 310d 0a61 7574 686f  n = 2.0.1..autho
+00000030: 6e20 3d20 322e 302e 320d 0a61 7574 686f  n = 2.0.2..autho
 00000040: 7220 3d20 4a6f 7365 2043 6172 6c69 746f  r = Jose Carlito
 00000050: 2064 6520 4f6c 6976 6569 7261 2046 696c   de Oliveira Fil
 00000060: 686f 0d0a 6175 7468 6f72 5f65 6d61 696c  ho..author_email
 00000070: 203d 206a 6361 726c 6974 6f6f 6c69 7665   = jcarlitoolive
 00000080: 6972 6140 676d 6169 6c2e 636f 6d0d 0a64  ira@gmail.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 204d 6173  escription = Mas
 000000a0: 7465 722f 576f 726b 6572 2069 6d70 6c65  ter/Worker imple
@@ -40,15 +40,15 @@
 00000270: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
 00000280: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
 00000290: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
 000002a0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
 000002b0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
 000002c0: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
 000002d0: 7569 7265 7320 3d20 0d0a 0973 6861 7265  uires = ...share
-000002e0: 6464 6174 613d 3d32 2e30 2e31 0d0a 0970  ddata==2.0.1...p
+000002e0: 6464 6174 613d 3d32 2e30 2e32 0d0a 0970  ddata==2.0.2...p
 000002f0: 7375 7469 6c3d 3d35 2e39 2e30 0d0a 0974  sutil==5.9.0...t
 00000300: 7a6c 6f63 616c 3d3d 342e 310d 0a0d 0a5b  zlocal==4.1....[
 00000310: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
 00000320: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
 00000330: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
 00000340: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
 00000350: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
```

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/RoutineScheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 if expiredidx.any():
                     expiredids = expiredidx.index[expiredidx]
                     sched.loc[expiredids,'Status'] = 'EXPIRED'
                 dfpending = dfpending[~expiredidx]
                 i=0
                 for i in dfpending.index:
                     r = dfpending.loc[i]
-                    if not str(r['Dependencies'])=='':
+                    if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
                         run=True
                         sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
                         dependencies = r['Dependencies'].replace('\n','').split(',')                
                         for dep in dependencies:                            
                             idx = sched['index']==dep
                             idx = (idx) & (sched['Run Times']<=runtime.astimezone(tz=local_tz))                            
                             ids = sched.index[idx]
@@ -151,15 +151,15 @@
         if expiredidx.any():
             expiredids = expiredidx.index[expiredidx]
             sched.loc[expiredids,'Status'] = 'EXPIRED'
         
         dfpending = dfpending[~expiredidx]
         for i in dfpending.index:
             r = dfpending.loc[i]
-            if not str(r['Dependencies'])=='':
+            if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
                 run=True
                 sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
                 dependencies = r['Dependencies'].replace('\n','').split(',')                
                 for dep in dependencies:                    
                     idx = sched['index']==dep                    
                     idx = (idx) & (sched['Run Times']<=datetime.now().astimezone(tz=local_tz))
                     ids = sched.index[idx]
```

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/master.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/master.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/runroutines.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/schedule_sequence.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/schedule_sequence.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/update_version_requirements.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/worker.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.0.2/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.0.1
+Version: 2.0.2
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.0.1/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.0.2/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

