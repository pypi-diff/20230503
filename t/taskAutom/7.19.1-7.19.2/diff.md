# Comparing `tmp/taskAutom-7.19.1.tar.gz` & `tmp/taskAutom-7.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-7.19.1.tar", last modified: Thu Feb  9 13:16:56 2023, max compression
+gzip compressed data, was "taskAutom-7.19.2.tar", last modified: Wed May  3 16:27:35 2023, max compression
```

## Comparing `taskAutom-7.19.1.tar` & `taskAutom-7.19.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-09 13:16:56.787852 taskAutom-7.19.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-02-09 13:16:56.787852 taskAutom-7.19.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.1/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-02-09 13:16:56.787852 taskAutom-7.19.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-02-09 13:16:42.000000 taskAutom-7.19.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-09 13:16:56.787852 taskAutom-7.19.1/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-09 13:16:56.787852 taskAutom-7.19.1/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-02-09 13:16:38.000000 taskAutom-7.19.1/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    64873 2023-02-09 13:16:34.000000 taskAutom-7.19.1/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-09 13:16:56.787852 taskAutom-7.19.1/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-02-09 13:16:56.000000 taskAutom-7.19.1/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.2/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-03 16:27:35.632553 taskAutom-7.19.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.2/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-03 16:27:35.632553 taskAutom-7.19.2/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-03 16:23:25.000000 taskAutom-7.19.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.628553 taskAutom-7.19.2/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-02 13:30:56.000000 taskAutom-7.19.2/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    64918 2023-05-03 14:19:43.000000 taskAutom-7.19.2/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:27:35.632553 taskAutom-7.19.2/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-03 16:27:35.000000 taskAutom-7.19.2/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-7.19.1/LICENSE` & `taskAutom-7.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.1/PKG-INFO` & `taskAutom-7.19.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.1
+Version: 7.19.2
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-7.19.1/README.md` & `taskAutom-7.19.2/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.1/setup.py` & `taskAutom-7.19.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='7.19.1',
+    version='7.19.2',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-7.19.1/src/taskAutom/taskAutom.py` & `taskAutom-7.19.2/src/taskAutom/taskAutom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2015-2022 Lucas Aimaretto / laimaretto@gmail.com
+# Copyright (C) 2015-2023 Lucas Aimaretto / laimaretto@gmail.com
 #
 # This is taskAutom
 #
 # taskAutom is free software: you can redistribute it and/or modify
 # it under the terms of the 3-clause BSD License.
 #
 # taskAutom is distributed in the hope that it will be useful,
@@ -40,26 +40,26 @@
 #logging.basicConfig(level=logging.DEBUG,format='[%(levelname)s] (%(threadName)-10s) %(message)s')
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
-	outputJob        = None,
+	outputJob        = 0,
 	logsDirectory    = None,
 	logsCsvFilename  = None,
 	logInfo          = None,
 	logFileName      = None,
 	logsDirTimestamp = None,
 	pluginFilename   = None,
 	cronTime         = dict(type=None),
 	jumpHosts        = dict(),
-	pluginType       = None,
+	pluginType       = 'show',
 	cmdVerify        = True,
-	auxRetry         = 5,
+	auxRetry         = 10,
 	inventoryFile    = None
 )
 
 # - Parameters per vendor
 DICT_VENDOR = dict(
 	nokia_sros=dict(
 		START_SCRIPT     = "", 
@@ -234,14 +234,15 @@
 
 		with open(dictParam['logsDirectory'] + '00_log_console.txt','w') as f:
 			for k in LOG_CONSOLE:
 				f.write(k+'\n')
 			f.close()
 
 		with open(dictParam['logsDirectory'] + '00_report.json', 'w') as f:
+			dictParam['version'] = '7.19.2'
 			dictParam['password'] = '*****'
 			dictParam.pop('data')
 			dictParam.pop('mod')
 			dictParam['routersTotal'] = len(df)
 			dictParam['routersFailed'] = len(dfFailed)
 			if len(dictParam['jumpHosts']) > 0:
 				for srv in dictParam['jumpHosts']:
@@ -1694,21 +1695,21 @@
 		open(dictParam['logsCsvFilename'],'w').close()
 
 	return dictParam
 
 def getDictParam():
 
 	parser = argparse.ArgumentParser(description='taskAutom Parameters.', prog='taskAutom', usage='%(prog)s [options]')
-	parser.add_argument('-v'  ,'--version',     help='Version', action='version', version='Lucas Aimaretto - (c)2023 - laimaretto@gmail.com - Version: 7.19.1' )
+	parser.add_argument('-v'  ,'--version',     help='Version', action='version', version='Lucas Aimaretto - (c)2023 - laimaretto@gmail.com - Version: 7.19.2' )
 
 	groupJobTypes = parser.add_argument_group('JobTypes')
-	groupJobTypes.add_argument('-j'  ,'--jobType',       type=int, required=True, choices=[0,2,3], default=0, help='Type of job. j=0 to check data and plugin; j=2, to execute. j=3, to upload files via SCP/SFTP.')
+	groupJobTypes.add_argument('-j'  ,'--jobType',       type=int, choices=[0,2,3], default=0, help='Type of job. j=0 to check data and plugin; j=2, to execute. j=3, to upload files via SCP/SFTP. Default=0')
 
 	groupPugin = parser.add_argument_group('Plugin')
-	groupPugin.add_argument('-pt' ,'--pluginType',      type=str, help='Type of plugin.', choices=['show','config'])
+	groupPugin.add_argument('-pt' ,'--pluginType',      type=str, help='Type of plugin.', default='show', choices=['show','config'])
 	groupPugin.add_argument('-py' ,'--pluginFilename' , type=str, help='PY Template File. Optional if jobType=3.')
 
 	groupData = parser.add_argument_group('Data Related')
 	groupData.add_argument('-d'  ,'--dataFile',        type=str, required=True, help='DATA File with parameters. Either CSV or XLSX. If XLSX, enable -xls option with sheet name.')
 	groupData.add_argument('-log','--logInfo' ,        type=str, required=True, help='Name of the log folder. Logs, MOP and scripts will be stored here.', )
 	groupData.add_argument('-fn','--logFileName' ,     type=str, help='Name of the log fileName, either "ip" or "hostname". Default=hostname', default='hostname', choices=['ip','hostname'] )
 	groupData.add_argument('-gc' ,'--dataGroupColumn', type=str, help='Only valid if using headers. Name of column, in the data file, to filter routers by. In general one should use the field where the IP of the router is. Default=ip', default='ip')
@@ -1744,15 +1745,15 @@
 	### reading parameters
 
 	dictParam = dict(
 		outputJob 		   = args.jobType,
 		dataFile           = args.dataFile,
 		xlsSheetName       = args.xlsSheetName,
 		useHeader          = True if args.useHeader == 'yes' else False,
-		passByRow          = True if args.passByRow  == 'yes' else False,
+		passByRow          = True if args.passByRow == 'yes' else False,
 		pluginFilename     = args.pluginFilename,
 		username 		   = args.username,
 		passwordFile       = args.passwordFile,
 		password 		   = None,
 		progNumThreads	   = args.threads,
 		logInfo 		   = args.logInfo,
 		logFileName        = args.logFileName,
```

### Comparing `taskAutom-7.19.1/taskAutom.egg-info/PKG-INFO` & `taskAutom-7.19.2/taskAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.1
+Version: 7.19.2
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

