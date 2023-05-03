# Comparing `tmp/brilws-3.7.1.tar.gz` & `tmp/brilws-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brilws-3.7.1.tar", last modified: Wed Feb 15 14:33:35 2023, max compression
+gzip compressed data, was "dist/brilws-3.7.3.tar", last modified: Wed May  3 17:57:18 2023, max compression
```

## Comparing `brilws-3.7.1.tar` & `brilws-3.7.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/
--rw-r--r--   0 xiezhen    (501) staff       (20)       86 2023-02-01 14:28:38.000000 brilws-3.7.1/MANIFEST.in
--rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-02-15 14:33:35.000000 brilws-3.7.1/PKG-INFO
--rw-r--r--   0 xiezhen    (501) staff       (20)      442 2023-02-01 14:28:38.000000 brilws-3.7.1/README.md
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/brilws/
--rw-r--r--   0 xiezhen    (501) staff       (20)      430 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/RegexValidator.py
--rw-r--r--   0 xiezhen    (501) staff       (20)       34 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)       22 2023-02-14 16:21:28.000000 brilws-3.7.1/brilws/_version.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    72115 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/api.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/brilws/cli/
--rw-r--r--   0 xiezhen    (501) staff       (20)      219 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1695 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilcalc_beam.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     3407 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/cli/brilcalc_lumi.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    59092 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/cli/brilcalc_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1286 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/cli/brilcalc_trg.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      870 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilschema_create.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1576 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilschema_loaddata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1462 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilschema_loadmap.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1413 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilschema_loadresult.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     8529 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/brilschema_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      745 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/briltag_insertdata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      670 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/briltag_insertiov.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      626 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/briltag_listdata.py
--rw-r--r--   0 xiezhen    (501) staff       (20)      918 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/briltag_listiov.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     7448 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/cli/briltag_main.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    17731 2023-02-14 16:08:17.000000 brilws-3.7.1/brilws/cli/clicommonargs.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     8554 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/corrector.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/brilws/data/
--rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/data/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1407 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/data/bcm1fv1.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     1129 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/data/readdb3.ini
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/brilws/dbschema/
--rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/dbschema/__init__.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1322 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/dbschema/schema_fixed.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)      390 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/dbschema/schema_iov.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     4570 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/dbschema/schema_sharded.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     1562 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/dbschema/schema_trg.yaml
--rw-r--r--   0 xiezhen    (501) staff       (20)     4131 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/display.py
--rw-r--r--   0 xiezhen    (501) staff       (20)    15804 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/fileapi.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     5929 2023-02-07 14:09:13.000000 brilws-3.7.1/brilws/formatter.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     2197 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/lumiParameters.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1864 2023-02-14 15:52:46.000000 brilws-3.7.1/brilws/params.py
--rw-r--r--   0 xiezhen    (501) staff       (20)     1267 2023-02-01 14:28:38.000000 brilws-3.7.1/brilws/timeconvert.py
-drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-02-15 14:33:35.000000 brilws-3.7.1/brilws.egg-info/
--rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-02-15 14:33:33.000000 brilws-3.7.1/brilws.egg-info/PKG-INFO
--rw-r--r--   0 xiezhen    (501) staff       (20)     1125 2023-02-15 14:33:34.000000 brilws-3.7.1/brilws.egg-info/SOURCES.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)        1 2023-02-15 14:33:33.000000 brilws-3.7.1/brilws.egg-info/dependency_links.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)      172 2023-02-15 14:33:33.000000 brilws-3.7.1/brilws.egg-info/entry_points.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)        7 2023-02-15 14:33:33.000000 brilws-3.7.1/brilws.egg-info/top_level.txt
--rw-r--r--   0 xiezhen    (501) staff       (20)       79 2023-02-15 14:33:35.000000 brilws-3.7.1/setup.cfg
--rwxr-xr-x   0 xiezhen    (501) staff       (20)     1040 2023-02-01 14:28:38.000000 brilws-3.7.1/setup.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/
+-rw-r--r--   0 xiezhen    (501) staff       (20)       86 2023-04-28 15:39:36.000000 brilws-3.7.3/MANIFEST.in
+-rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-03 17:57:18.000000 brilws-3.7.3/PKG-INFO
+-rw-r--r--   0 xiezhen    (501) staff       (20)      442 2023-04-28 15:39:36.000000 brilws-3.7.3/README.md
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      430 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/RegexValidator.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)       34 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)       22 2023-05-03 17:51:23.000000 brilws-3.7.3/brilws/_version.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    73253 2023-05-03 17:42:14.000000 brilws-3.7.3/brilws/api.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/cli/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      219 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1695 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_beam.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     3407 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_lumi.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    59077 2023-04-28 15:45:47.000000 brilws-3.7.3/brilws/cli/brilcalc_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1286 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilcalc_trg.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      870 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_create.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1576 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loaddata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1462 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loadmap.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1413 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_loadresult.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     8529 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/brilschema_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      745 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_insertdata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      670 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_insertiov.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      626 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_listdata.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)      918 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_listiov.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     7448 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/briltag_main.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    17731 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/cli/clicommonargs.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     8554 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/corrector.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/data/
+-rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1407 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/bcm1fv1.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1129 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/data/readdb3.ini
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws/dbschema/
+-rw-r--r--   0 xiezhen    (501) staff       (20)        0 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/__init__.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1322 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_fixed.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)      390 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_iov.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     4581 2023-04-28 15:41:04.000000 brilws-3.7.3/brilws/dbschema/schema_sharded.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1562 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/dbschema/schema_trg.yaml
+-rw-r--r--   0 xiezhen    (501) staff       (20)     4131 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/display.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)    15804 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/fileapi.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     5929 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/formatter.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     2197 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/lumiParameters.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1864 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/params.py
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1267 2023-04-28 15:39:36.000000 brilws-3.7.3/brilws/timeconvert.py
+drwxr-xr-x   0 xiezhen    (501) staff       (20)        0 2023-05-03 17:57:18.000000 brilws-3.7.3/brilws.egg-info/
+-rw-r--r--   0 xiezhen    (501) staff       (20)      875 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/PKG-INFO
+-rw-r--r--   0 xiezhen    (501) staff       (20)     1125 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/SOURCES.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)        1 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/dependency_links.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)      172 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/entry_points.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)        7 2023-05-03 17:57:17.000000 brilws-3.7.3/brilws.egg-info/top_level.txt
+-rw-r--r--   0 xiezhen    (501) staff       (20)       79 2023-05-03 17:57:18.000000 brilws-3.7.3/setup.cfg
+-rwxr-xr-x   0 xiezhen    (501) staff       (20)     1040 2023-04-28 15:39:36.000000 brilws-3.7.3/setup.py
```

### Comparing `brilws-3.7.1/PKG-INFO` & `brilws-3.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: brilws
-Version: 3.7.1
+Version: 3.7.3
 Summary: bril worksuite
 Home-page: https://github.com/xiezhen/brilws
 Author: Zhen Xie
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.1
+Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.3
 Description: ### BRIL Work Suite
         python package for working with BRIL data 
         
         #### Install
         
         #### into brilconda virtual environment
         pip install brilws
```

### Comparing `brilws-3.7.1/brilws/api.py` & `brilws-3.7.3/brilws/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1412,14 +1412,38 @@
     '''    
     sqlresult = pattern
     sqlresult = sqlresult.replace('*','.*')
     sqlresult = sqlresult.replace('?','.?')
     sqlresult = sqlresult.replace('!','^')    
     return sqlresult
 
+def is_hltpath_in_dataset(engine,hltconfigidhltpathidpairs,datasetname,schemaname=''):
+    '''
+    hltconfigidhltpathidpairs : [(hltconfigid,hltpathid)]
+    '''
+    datasettablename = dname = 'datasethltpathmap'
+    hlttablename = hname = 'hltpathl1seedmap'
+    if schemaname:
+        datasethltpathmap = '.'.join([schemaname,dname])
+        hltpathl1seedmap = '.'.join([schemaname,hname])
+    for (hltconfigid,hltpathid) in hltconfigidhltpathidpairs:
+      q = "select count(*) from {datasethltpathmap} d, {hltpathl1seedmap} h where h.hltconfigid=d.hltconfigid and d.hltconfigid=:hltconfigid and d.datasetpathname=:datasetname and h.hltpathid=:hltpathid".format(datasethltpathmap=datasethltpathmap,hltpathl1seedmap=hltpathl1seedmap)
+      binddict = {}
+      binddict['hltpathid'] = hltpathid
+      binddict['datasetname'] = datasetname
+      binddict['hltconfigid'] = hltconfigid
+      log.debug(q+','+str(binddict))
+    connection = engine.connect()
+    resultProxy = connection.execute(q,binddict)
+    for row in resultProxy:
+      result = int(row[0])
+      if result>0:
+        return True
+    return False
+
 def is_hltpathid_in_dataset(engine,hltpathid,datasetname,hltconfigid,schemaname=''):
     '''
     Check if a hltpathid and a dataset is in the same menu, no more relationship for now
     input :
        hltpathid : hltpathid 
        datasetname : dataset name
        hltconfigid : 
@@ -1427,26 +1451,27 @@
        True or False
     '''
     datasettablename = dname = 'datasethltpathmap'
     hlttablename = hname = 'hltpathl1seedmap'
     if schemaname:
         datasethltpathmap = '.'.join([schemaname,dname])
         hltpathl1seedmap = '.'.join([schemaname,hname])
-    q = "select count(*) from {datasethltpathmap} d, {hltpathl1seedmap} h where h.hltconfigid=d.hltconfigid and d.hltconfigid=:hltconfigid and d.datasetpathname=:datasetname and h.hltpathid=:hltpathid".format(datasethltpathmap=datasethltpathmap,hltpathl1seedmap=hltpathl1seedmap,)
+    q = "select count(*) from {datasethltpathmap} d, {hltpathl1seedmap} h where h.hltconfigid=d.hltconfigid and d.hltconfigid=:hltconfigid and d.datasetpathname=:datasetname and h.hltpathid=:hltpathid".format(datasethltpathmap=datasethltpathmap,hltpathl1seedmap=hltpathl1seedmap)
     binddict = {}
     binddict['hltpathid'] = hltpathid
     binddict['datasetname'] = datasetname
     binddict['hltconfigid'] = hltconfigid
     log.debug(q+','+str(binddict))
     connection = engine.connect()
     resultProxy = connection.execute(q,binddict)
-    result = 0
     for row in resultProxy:
       result = int(row[0])
-    return result
+      if result>0:
+          return True
+    return False
 
 def get_dataset_presc(engine,hltconfigid,datasetname,schemaname=''):
     '''
     input: 
         hltconnfigid 
         datasetname
     output:
```

### Comparing `brilws-3.7.1/brilws/cli/brilcalc_beam.py` & `brilws-3.7.3/brilws/cli/brilcalc_beam.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilcalc_lumi.py` & `brilws-3.7.3/brilws/cli/brilcalc_lumi.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilcalc_main.py` & `brilws-3.7.3/brilws/cli/brilcalc_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,20 +624,20 @@
                   sys.exit(0)
               if pargs.dataset is not None:
                   datasethltpairs = set()
                   for k in hltl1map: 
                     hpaths = [h[0] for h in hltl1map[k]]
                     for hp in hpaths:                        
                       datasethltpairs.add( (k,hp) )
-                  for (hltconfigid,hltpathid) in datasethltpairs:
-                    r = api.is_hltpathid_in_dataset(dbengine,hltpathid,pargs.dataset,hltconfigid,schemaname=dbschema)
+                  #for (hltconfigid,hltpathid) in datasethltpairs:
+                  r = api.is_hltpath_in_dataset(dbengine,datasethltpairs,pargs.dataset,schemaname=dbschema)
                   ##check hltpathid and dataset are in the same menu
-                    if not r:
-                      print( 'dataset {} and hltpath{} are not in the same menu'.format(pargs.dataset,pargs.hltpath) )
-                      sys.exit(0)
+                  if not r:
+                    print( 'dataset {} and hltpath{} are not in the same menu'.format(pargs.dataset,pargs.hltpath) )
+                    sys.exit(0)
 
           rselectrange = [] 
           if datasources :
               for [qt,nt,ds,rs] in datasources:
                   if rs is None: 
                       continue
                   for r,l in rs.iteritems():
```

### Comparing `brilws-3.7.1/brilws/cli/brilcalc_trg.py` & `brilws-3.7.3/brilws/cli/brilcalc_trg.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilschema_create.py` & `brilws-3.7.3/brilws/cli/brilschema_create.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilschema_loaddata.py` & `brilws-3.7.3/brilws/cli/brilschema_loaddata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilschema_loadmap.py` & `brilws-3.7.3/brilws/cli/brilschema_loadmap.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilschema_loadresult.py` & `brilws-3.7.3/brilws/cli/brilschema_loadresult.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/brilschema_main.py` & `brilws-3.7.3/brilws/cli/brilschema_main.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/briltag_insertdata.py` & `brilws-3.7.3/brilws/cli/briltag_insertdata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/briltag_insertiov.py` & `brilws-3.7.3/brilws/cli/briltag_insertiov.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/briltag_listdata.py` & `brilws-3.7.3/brilws/cli/briltag_listdata.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/briltag_listiov.py` & `brilws-3.7.3/brilws/cli/briltag_listiov.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/briltag_main.py` & `brilws-3.7.3/brilws/cli/briltag_main.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/cli/clicommonargs.py` & `brilws-3.7.3/brilws/cli/clicommonargs.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/corrector.py` & `brilws-3.7.3/brilws/corrector.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/data/bcm1fv1.yaml` & `brilws-3.7.3/brilws/data/bcm1fv1.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/data/readdb3.ini` & `brilws-3.7.3/brilws/data/readdb3.ini`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/dbschema/schema_fixed.yaml` & `brilws-3.7.3/brilws/dbschema/schema_fixed.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/dbschema/schema_sharded.yaml` & `brilws-3.7.3/brilws/dbschema/schema_sharded.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -80,25 +80,24 @@
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
     - avglumi: float
    pk: [ datatagid ]
 
-BCM1FSI_RAW_&suffix: #per ls
+RAMSES_RAW_&suffix:         #per ls but from online
    columns:
     - datatagid: int64
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
     - avglumi: float
-    - bxlumiblob: blob
    pk: [ datatagid ]
-
+   
 BCM1FUTCA_RAW_&suffix: #per ls
    columns:
     - datatagid: int64
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
@@ -156,53 +155,51 @@
     - timestampsec: uint32
     - normtag: string
     - normtagid: int64
     - avglumi: float
     - bxlumiblob: blob
    pk: [datatagid,normtagid]
 
-BCM1FSI_RESULT_&suffix:
+BCM1FUTCA_RESULT_&suffix:
    columns:
     - datatagid: int64
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
     - normtag: string
     - normtagid: int64
     - avglumi: float
     - bxlumiblob: blob
    pk: [datatagid,normtagid]
-
-BCM1FUTCA_RESULT_&suffix:
+   
+DT_RESULT_&suffix:         #per ls but from online
    columns:
     - datatagid: int64
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
     - normtag: string
     - normtagid: int64
     - avglumi: float
-    - bxlumiblob: blob
-   pk: [datatagid,normtagid]
-   
-DT_RESULT_&suffix:         #per ls but from online
+   pk: [ datatagid,normtagid]
+
+RAMSES_RESULT_&suffix:         #per ls but from online
    columns:
     - datatagid: int64
     - fillnum: uint32
     - runnum: uint32
     - lsnum: uint32
     - timestampsec: uint32
     - normtag: string
     - normtagid: int64
     - avglumi: float
    pk: [ datatagid,normtagid]
 
-
 ONLINE_RESULT_&suffix:
    columns:
     - runnum: uint32
     - lsnum: uint32
     - fillnum: uint32
     - timestampsec: uint32
     - cmson: bool
```

### Comparing `brilws-3.7.1/brilws/dbschema/schema_trg.yaml` & `brilws-3.7.3/brilws/dbschema/schema_trg.yaml`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/display.py` & `brilws-3.7.3/brilws/display.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/fileapi.py` & `brilws-3.7.3/brilws/fileapi.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/formatter.py` & `brilws-3.7.3/brilws/formatter.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/lumiParameters.py` & `brilws-3.7.3/brilws/lumiParameters.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/params.py` & `brilws-3.7.3/brilws/params.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws/timeconvert.py` & `brilws-3.7.3/brilws/timeconvert.py`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/brilws.egg-info/PKG-INFO` & `brilws-3.7.3/brilws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: brilws
-Version: 3.7.1
+Version: 3.7.3
 Summary: bril worksuite
 Home-page: https://github.com/xiezhen/brilws
 Author: Zhen Xie
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.1
+Download-URL: https://github.com/xiezhen/brilws/tarball/3.7.3
 Description: ### BRIL Work Suite
         python package for working with BRIL data 
         
         #### Install
         
         #### into brilconda virtual environment
         pip install brilws
```

### Comparing `brilws-3.7.1/brilws.egg-info/SOURCES.txt` & `brilws-3.7.3/brilws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brilws-3.7.1/setup.py` & `brilws-3.7.3/setup.py`

 * *Files identical despite different names*

