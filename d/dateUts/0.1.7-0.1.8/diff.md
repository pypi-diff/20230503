# Comparing `tmp/dateUts-0.1.7.tar.gz` & `tmp/dateUts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dateUts-0.1.7.tar", last modified: Mon May  1 22:51:05 2023, max compression
+gzip compressed data, was "dateUts-0.1.8.tar", last modified: Wed May  3 14:08:55 2023, max compression
```

## Comparing `dateUts-0.1.7.tar` & `dateUts-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.669511 dateUts-0.1.7/
--rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.7/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4331 2023-05-01 22:51:05.668514 dateUts-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.7/README.md
--rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.7/commands.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.643581 dateUts-0.1.7/dateUts/
--rw-rw-rw-   0        0        0     4964 2023-04-26 21:20:07.000000 dateUts-0.1.7/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:51:05.667516 dateUts-0.1.7/dateUts.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 22:51:05.000000 dateUts-0.1.7/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:51:05.669511 dateUts-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-01 22:50:57.000000 dateUts-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:08:55.490768 dateUts-0.1.8/
+-rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.8/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4331 2023-05-03 14:08:55.489770 dateUts-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.8/README.md
+-rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.8/commands.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 14:08:55.465836 dateUts-0.1.8/dateUts/
+-rw-rw-rw-   0        0        0     5597 2023-05-03 14:07:53.000000 dateUts-0.1.8/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:08:55.488772 dateUts-0.1.8/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-05-03 14:08:55.000000 dateUts-0.1.8/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-03 14:08:55.000000 dateUts-0.1.8/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:08:55.000000 dateUts-0.1.8/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 14:08:55.000000 dateUts-0.1.8/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:08:55.490768 dateUts-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-03 14:08:11.000000 dateUts-0.1.8/setup.py
```

### Comparing `dateUts-0.1.7/CHANGELOG.txt` & `dateUts-0.1.8/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.7/LICENCE.txt` & `dateUts-0.1.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.7/PKG-INFO` & `dateUts-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.7
+Version: 0.1.8
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.7/README.md` & `dateUts-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.7/dateUts/__init__.py` & `dateUts-0.1.8/dateUts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date, datetime as dt, timedelta as td
+from dateutil.relativedelta import relativedelta
 
 
 class DateUts():
     date = None
 
     def __init__(self,date):
         self.date = date
@@ -21,16 +22,16 @@
 
 
 #========= USAGE ============
 #Ex1:
 # > sqlToDate('yyyy-MM-dd')
 # > <datetime>
 
-def sqlToDate(dt:str):
-    return DateUts(dt.strptime(dt,"%Y-%m-%d"))
+def sqlToDate(date_str:str):
+    return DateUts(dt.strptime(date_str,"%Y-%m-%d"))
 
 #========= USAGE ============
 #Ex1:
 # > dateToSql(<datetime>)
 # > 'yyyy-MM-dd'
 
 def dateToSql(dt:date):
@@ -97,20 +98,24 @@
 
 def dateAdd(date:date,qtd:int,unit:str="day",fmt=None):
     date = date.date if isinstance(date,DateUts) else date
     if unit == 'day':
         v = date + td(qtd) if qtd > 0 else date - td(abs(qtd))
     elif unit == 'year':
         v = date.replace(year = date.year + qtd)
-    elif unit == 'hours':
+    elif unit == 'hour':
         v = date + td(hours=qtd)
-    elif unit == 'minutes':
+    elif unit == 'minute':
         v = date + td(minutes=qtd)
-    elif unit == 'seconds':
+    elif unit == 'second':
         v = date + td(seconds=qtd)
+    elif unit == 'month':
+        v = date + relativedelta(months=qtd)
+
+
 
     return fmtDate(v,fmt)
 
 #========= USAGE ============ 
 #Obs: Today is "2022-05-23"
 #Ex1:
 # > lastWorkingDate()  ,  lastWorkingDate(fmt='%Y-%m-%d')   ,   lastWorkingDate(fmt='sql')
@@ -151,15 +156,27 @@
     try:
         dt = datetime.strptime(dt,fmt)
     except ValueError:
         return False
 
     return True
 
-lastWorkingDate(today())
+def firstDay(sql_dte:str|date,fmt:str=None):
+    dte = sql_dte if isinstance(sql_dte,date) or isinstance(sql_dte,DateUts) else sqlToDate(sql_dte)
+    dte = fmtDate(dte,"%Y-%m-01")
+    firstDay = sqlToDate(dte)
+    return fmtDate(firstDay,fmt)
+
+def lastDay(sql_dte:str|date,fmt:str=None):
+    dte = sql_dte if isinstance(sql_dte,date) or isinstance(sql_dte,DateUts) else sqlToDate(sql_dte)
+    dte = sqlToDate(dateAdd(dte,1,"month",fmt="%Y-%m-01"))
+    dte = dateAdd(dte,-1,"day")
+    return fmtDate(dte,fmt)
+
+
 
 Fnc_noWeekends = lambda dt:dt.weekday() not in [5,6]
 
 # a = DateUts(dt.now())
 # print(a)
 # a = lastWorkingDate(fmt="%Y-%m-%d")
 # rng = dateRange(sqlToDate("2022-05-01"),sqlToDate("2022-05-10"))
```

### Comparing `dateUts-0.1.7/dateUts.egg-info/PKG-INFO` & `dateUts-0.1.8/dateUts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.7
+Version: 0.1.8
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.7/setup.py` & `dateUts-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.7',
+  version='0.1.8',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

