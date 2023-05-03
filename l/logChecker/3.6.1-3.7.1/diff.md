# Comparing `tmp/logChecker-3.6.1.tar.gz` & `tmp/logChecker-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logChecker-3.6.1.tar", last modified: Tue Jan 10 18:08:05 2023, max compression
+gzip compressed data, was "logChecker-3.7.1.tar", last modified: Wed May  3 16:39:30 2023, max compression
```

## Comparing `logChecker-3.6.1.tar` & `logChecker-3.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-01-10 18:08:05.587744 logChecker-3.6.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1654 2022-11-28 15:01:26.000000 logChecker-3.6.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-01-10 18:08:05.587744 logChecker-3.6.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4467 2022-11-28 15:01:26.000000 logChecker-3.6.1/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-01-10 18:08:05.587744 logChecker-3.6.1/logChecker.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      288 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       58 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       15 2023-01-10 18:08:05.000000 logChecker-3.6.1/logChecker.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-01-10 18:08:05.587744 logChecker-3.6.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1038 2023-01-10 18:07:55.000000 logChecker-3.6.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-01-10 18:08:05.587744 logChecker-3.6.1/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-01-10 18:08:05.587744 logChecker-3.6.1/src/logChecker/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-01-10 18:07:52.000000 logChecker-3.6.1/src/logChecker/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    27004 2023-01-10 18:07:49.000000 logChecker-3.6.1/src/logChecker/logChecker.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1654 2022-11-28 15:01:26.000000 logChecker-3.7.1/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-05-03 16:39:29.993637 logChecker-3.7.1/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     4467 2022-11-28 15:01:26.000000 logChecker-3.7.1/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/logChecker.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      288 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       58 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       15 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-03 16:39:29.993637 logChecker-3.7.1/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1038 2023-05-03 16:38:51.000000 logChecker-3.7.1/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.989637 logChecker-3.7.1/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/src/logChecker/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-03 16:39:00.000000 logChecker-3.7.1/src/logChecker/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    30663 2023-05-03 15:04:12.000000 logChecker-3.7.1/src/logChecker/logChecker.py
```

### Comparing `logChecker-3.6.1/LICENSE` & `logChecker-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logChecker-3.6.1/PKG-INFO` & `logChecker-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logChecker
-Version: 3.6.1
+Version: 3.7.1
 Summary: A simple log analysis tool
 Home-page: https://github.com/laimaretto/logChecker
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Project-URL: Templates, https://github.com/laimaretto/logTemplates
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logChecker-3.6.1/README.md` & `logChecker-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `logChecker-3.6.1/logChecker.egg-info/PKG-INFO` & `logChecker-3.7.1/logChecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logChecker
-Version: 3.6.1
+Version: 3.7.1
 Summary: A simple log analysis tool
 Home-page: https://github.com/laimaretto/logChecker
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Project-URL: Templates, https://github.com/laimaretto/logTemplates
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logChecker-3.6.1/setup.py` & `logChecker-3.7.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='logChecker',
-    version='3.6.1',  
+    version='3.7.1',  
     description='A simple log analysis tool',
     long_description='A parsing tool to easily perform pre and post check comparisons after a maintenance window.',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/logChecker',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `logChecker-3.6.1/src/logChecker/logChecker.py` & `logChecker-3.7.1/src/logChecker/logChecker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 #!/usr/bin/env python3
-
-# Copyright (C) 2022 Lucas Aimaretto / laimaretto@gmail.com
+# 
+# Copyright (C) 2023 Lucas Aimaretto / laimaretto@gmail.com
 # Copyright (C) 2020 Manuel Saldivar / manuelsaldivar@outlook.com.ar, Lucas Aimaretto / laimaretto@gmail.com
-#
+# 
 # This is logCheck
-#
+# 
 # logCheck is free software: you can redistribute it and/or modify
 # it under the terms of the 3-clause BSD License.
-#
+# 
 # logCheck is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY of any kind whatsoever.
-#
+# 
 
 import textfsm
 import pandas as pd
 import glob
 import argparse
 from sys import platform as _platform
 import json
 import re
 from ttp import ttp
 import os
 
+import docx
+from docx.enum.style import WD_STYLE_TYPE 
+from docx.enum.text import WD_LINE_SPACING
+from docx.shared import Pt
+
+
 DATA_VALUE         = 'Value'
 DATA_COMMAND       = '#Command:'
 DATA_MAJOR_DWN     = '#majorDown:'
 DATA_FLTR_COLS     = '#filterColumns:'
 DATA_FLTR_ACTN     = '#filterAction:'
 DATA_SHOW_DIFF_COL = '#showDiffColumns'
 
@@ -279,15 +285,15 @@
 	Reads logs, and stores router logs in memory for processing
 
 	Args:
 		logFolder (string):  name of folder
 		formatJson (string): "yes" or "no"
 	"""
 
-	if formatJson == 'yes':
+	if formatJson is True:
 
 		ending = '*rx.json'
 
 	else:
 
 		ending = '*rx.txt'
 
@@ -302,15 +308,15 @@
 		listContent  = [f.replace("\\", '/') for f in glob.glob(logFolder  + ending)]
 	else:
 		print(str(_platform) + ": not a valid platform. Quitting....")
 		quit()
 
 	d = {}
 
-	if formatJson == 'yes':
+	if formatJson is True:
 
 		for name in listContent:
 			with open(name) as f:
 				d[name] = json.load(f)
 
 	else:
 	
@@ -658,25 +664,128 @@
 		if len(dfMajor) > 0:
 			dfMajor.to_excel(writer, sheet_name=sheet_name, startrow=(len(dfData)+(len(dfDiff)))+10, startcol=0)
 		
 		print('#',idx,template)
 	
 	writer.save() #saves workbook to file in python file directory
 
+def renderAtp(dictParam):
+	"""[Generates a ATP based on the json logs obtained from taskAutom.]
+
+	Args:
+		dictParam
+
+	Returns:
+		None
+	"""
+
+	preFolder  = dictParam['preFolder']
+	postFolder = dictParam['postFolder']
+
+	jsonFilesPre = [preFolder+x for x in os.listdir(preFolder) if '.json' in x and x != '00_report.json']
+	if postFolder != '':
+		jsonFilesPos = [postFolder+x for x in os.listdir(postFolder) if '.json' in x and x != '00_report.json']
+
+	job0docx = "./ATP.docx"
+
+	print("\nGenerating ATP: " + job0docx)
+
+	myDoc    = docx.Document()
+	myStyles = myDoc.styles  
+
+	styleConsole = myStyles.add_style('Console', WD_STYLE_TYPE.PARAGRAPH)
+	styleConsole.font.name = 'Courier'
+	styleConsole.font.size = Pt(9)
+	styleConsole.paragraph_format.keep_together = True
+
+	styleConsole.paragraph_format.line_spacing_rule = WD_LINE_SPACING.SINGLE
+	#styleConsole.paragraph_format.line_spacing = Pt(10)
+	#styleConsole.paragraph_format.line_spacing = .2
+	styleConsole.paragraph_format.space_after = Pt(2)
+
+	myDoc.add_heading('ATP', 0)
+
+	charset_allowed = [chr(c) for c in range(32,127)] + ['\n']
+
+	if preFolder != '':
+
+		docMainTitle = myDoc.add_paragraph('Pre-Check')
+		docMainTitle.style = myDoc.styles['Heading 1']
+		docMainTitle.paragraph_format.line_spacing = 1.5	
+
+		for f in jsonFilesPre:
+			
+			with open(f) as myFile:
+				
+				logs  = json.load(myFile)
+				keys  = [x for x in logs.keys() if 'show' in x]
+
+				routerTitle = f'Router {logs["name"]} ({logs["ip"]})'
+
+				docRouterTitle = myDoc.add_paragraph(routerTitle)
+				docRouterTitle.style = myDoc.styles['Heading 2']
+				docRouterTitle.paragraph_format.line_spacing = 1.5
+
+				for key in keys:
+					showTitle   = key.rstrip('\n').lstrip('\n')
+					showContent = ''.join([x for x in logs[key] if x in charset_allowed]).rstrip('\n').lstrip('\n')
+
+					docShowTitle = myDoc.add_paragraph(showTitle)
+					docShowTitle.style = myDoc.styles['Heading 3']
+					docShowTitle.paragraph_format.line_spacing = 1.5
+
+					docShowContent = myDoc.add_paragraph(showContent)
+					docShowContent.style = myDoc.styles['Console']
+
+	if postFolder != '':
+
+		docMainTitle = myDoc.add_paragraph('Post-Check')
+		docMainTitle.style = myDoc.styles['Heading 1']
+		docMainTitle.paragraph_format.line_spacing = 1.5
+
+		for f in jsonFilesPos:
+			
+			with open(f) as myFile:
+				
+				logs  = json.load(myFile)
+				keys  = [x for x in logs.keys() if 'show' in x]
+
+				routerTitle = f'Router {logs["name"]} ({logs["ip"]})'
+
+				docRouterTitle = myDoc.add_paragraph(routerTitle)
+				docRouterTitle.style = myDoc.styles['Heading 2']
+				docRouterTitle.paragraph_format.line_spacing = 1.5
+
+				for key in keys:
+					showTitle   = key.rstrip('\n').lstrip('\n')
+					showContent = ''.join([x for x in logs[key] if x in charset_allowed]).rstrip('\n').lstrip('\n')
+
+					docShowTitle = myDoc.add_paragraph(showTitle)
+					docShowTitle.style = myDoc.styles['Heading 3']
+					docShowTitle.paragraph_format.line_spacing = 1.5
+
+					docShowContent = myDoc.add_paragraph(showContent)
+					docShowContent.style = myDoc.styles['Console']		
+
+	myDoc.save(job0docx)
+
+	print("ATP done...")
+
 def fncRun(dictParam):
 
 	preFolder          = dictParam['preFolder']
 	postFolder         = dictParam['postFolder']
 	csvTemplate        = dictParam['csvTemplate']
 	formatJson         = dictParam['formatJson']
 	templateFolder     = dictParam['templateFolder']
 	templateEngine     = dictParam['templateEngine']
 	templateFolderPost = dictParam['templateFolderPost']
 	routerId           = dictParam['routerId']
 	showResults        = dictParam['showResults']
+	genAtp             = dictParam['genAtp']
 
 	if _platform == "win64" or _platform == "win32":
 		templateFolder = templateFolder.replace('/', '\\')
 		if templateFolderPost != '':
 			templateFolderPost = templateFolderPost.replace('/','\\')
 
 	if preFolder != '' and postFolder == '':
@@ -690,14 +799,17 @@
 
 		for tmpltName in df_final.keys():
 			count_dif[tmpltName]   = pd.DataFrame(columns=df_final[tmpltName].columns)
 			searchMajor[tmpltName] = pd.DataFrame(columns=df_final[tmpltName].columns)
 
 		constructExcel(df_final, count_dif, searchMajor, preFolder)
 
+		if genAtp is True:
+			renderAtp(dictParam)		
+
 	elif preFolder != '' and postFolder != '':
 
 		if templateFolder == templateFolderPost:
 			dTmpltPre  = readTemplate(csvTemplate, templateFolder, templateEngine)
 			dTmpltPost = readTemplate(csvTemplate, templateFolderPost, templateEngine)
 		elif templateFolder != '' and templateFolderPost == '':
 			templateFolderPost = templateFolder
@@ -738,14 +850,17 @@
 			count_dif       = searchDiffOnly(datosEquipoPre, datosEquipoPost, dTmpltPre, routerId)
 
 		searchMajor     = findMajor(count_dif, dTmpltPre, routerId, showResults)
 		df_final        = makeTable(datosEquipoPre, datosEquipoPost)
 
 		constructExcel(df_final, count_dif, searchMajor, postFolder)
 
+		if genAtp is True:
+			renderAtp(dictParam)		
+
 	elif preFolder == '':
 		print('No PRE folder defined. Please Verify.')
 
 
 
 def main():
 
@@ -755,28 +870,30 @@
 	parser1.add_argument('-csv', '--csvTemplate',   type=str, default='', help='CSV with list of templates names to be used in parsing. If the file is omitted, then all the templates inside --templateFolder, will be considered for parsing. Default=None.')
 	parser1.add_argument('-json', '--formatJson',   type=str, default = 'yes', choices=['yes','no'], help='logs in json format: yes or no. Default=yes.')
 	parser1.add_argument('-tf', '--templateFolder', type=str, default='Templates/', help='Folder where templates reside. Used both for PRE and POST logs. Default=Templates/')
 	parser1.add_argument('-tf-post', '--templateFolderPost', type=str, default='', help='If set, use this folder of templates for POST logs.')
 	parser1.add_argument('-te', '--templateEngine', choices=['ttp','textFSM'], default='textFSM', type=str, help='Engine for parsing. Default=textFSM.')
 	parser1.add_argument('-ri', '--routerId',       choices=['name','ip','both'], default='name', type=str, help='Router Id to be used within the tables in the Excel report. Default=name.')
 	parser1.add_argument('-sr', '--showResults',    choices=['all','diff'], default='all', type=str, help='When comparison is done, show all variables or only the differences. Only available if --ri/--routerId=name. Default=all)')
-	parser1.add_argument('-v'  ,'--version',        help='Version', action='version', version='Lucas Aimaretto - (c)2023 - Version: 3.6.1' )
+	parser1.add_argument('-ga', '--genAtp',        type=str, help='Generate ATP document in docx format, based on the contents of the json files from taskAutom. Default=no', default='no', choices=['no','yes'])
+	parser1.add_argument('-v'  ,'--version',        help='Version', action='version', version='Lucas Aimaretto - (c)2023 - Version: 3.7.1' )
 
 	args               = parser1.parse_args()
 
 	dictParam = dict(
 		preFolder          = args.preFolder,
 		postFolder         = args.postFolder,
 		csvTemplate        = args.csvTemplate,
-		formatJson         = args.formatJson,
+		formatJson         = True if args.formatJson == 'yes' else False,
 		templateFolder     = args.templateFolder,
 		templateEngine     = args.templateEngine,
 		templateFolderPost = args.templateFolderPost,
 		routerId           = args.routerId,
 		showResults        = args.showResults,
+		genAtp             = True if args.genAtp == 'yes' else False,		
 	)
 
 	if dictParam['showResults'] == 'diff' and dictParam['routerId'] != 'name':
 		print('If showResults is "diff", routerId must be "name"\nQuitting ...')
 		quit()
 
 	fncRun(dictParam)
```

