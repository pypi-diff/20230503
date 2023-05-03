# Comparing `tmp/minidatabase-1.6.tar.gz` & `tmp/minidatabase-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidatabase-1.6.tar", last modified: Tue May  2 10:15:39 2023, max compression
+gzip compressed data, was "minidatabase-1.6.1.tar", last modified: Wed May  3 02:21:26 2023, max compression
```

## Comparing `minidatabase-1.6.tar` & `minidatabase-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.285803 minidatabase-1.6/
--rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3824 2023-05-02 10:15:39.284803 minidatabase-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2929 2023-05-02 10:12:16.000000 minidatabase-1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.268562 minidatabase-1.6/minidatabase/
--rw-rw-rw-   0        0        0     1623 2023-05-02 09:56:27.000000 minidatabase-1.6/minidatabase/WebMDB.py
--rw-rw-rw-   0        0        0       65 2023-05-02 04:28:10.000000 minidatabase-1.6/minidatabase/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.6/minidatabase/minidb.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.282136 minidatabase-1.6/minidatabase.egg-info/
--rw-rw-rw-   0        0        0     3824 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:15:39.285803 minidatabase-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-05-02 10:15:29.000000 minidatabase-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:21:26.627783 minidatabase-1.6.1/
+-rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3826 2023-05-03 02:21:26.627783 minidatabase-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2929 2023-05-02 10:12:16.000000 minidatabase-1.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 02:21:26.609681 minidatabase-1.6.1/minidatabase/
+-rw-rw-rw-   0        0        0     1873 2023-05-03 01:39:59.000000 minidatabase-1.6.1/minidatabase/WebMDB.py
+-rw-rw-rw-   0        0        0       85 2023-05-02 13:13:38.000000 minidatabase-1.6.1/minidatabase/__init__.py
+-rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.6.1/minidatabase/minidb.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:21:26.627783 minidatabase-1.6.1/minidatabase.egg-info/
+-rw-rw-rw-   0        0        0     3826 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 02:21:26.000000 minidatabase-1.6.1/minidatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 02:21:26.627783 minidatabase-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-05-03 01:36:25.000000 minidatabase-1.6.1/setup.py
```

### Comparing `minidatabase-1.6/LICENSE.txt` & `minidatabase-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minidatabase-1.6/PKG-INFO` & `minidatabase-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidatabase
-Version: 1.6
+Version: 1.6.1
 Summary: A tiny database system based on  python dictionary.
 Home-page: http://osdn.xyz
 Author: HansenL
 Author-email: hansenl@foxmail.com
 License:  GNU GENERAL PUBLIC LICENSE
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `minidatabase-1.6/README.rst` & `minidatabase-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `minidatabase-1.6/minidatabase/WebMDB.py` & `minidatabase-1.6.1/minidatabase/WebMDB.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from flask import Flask
-import minidb
+from minidatabase import minidb
+import sys
 #MiniDataBase Web Server Service
 #Develop By HansenL
-if __name__ == "__main__":
+def service(p,nzm,passwd):
     print("Welcome to use WebMDB Server.")
-    p=int(input("Please enter the service port->"))
-    nzm=input("Please enter the MiniDataBase File name->")
-    passwd=input("Please enter the Database Password ->")
     cursor=minidb.connect(nzm)
     app=Flask(__name__)
     @app.route('/')
     def status():
         return 'WebMDB Services has been opened.'
     @app.route('/%s/append/<tag>/<value>'%passwd)
     def append(tag,value):
@@ -45,7 +43,20 @@
     def search_tags(keyword):
         return str(cursor.search_tag(keyword))
     @app.route('/%s/search_value/<keyword>'%passwd)
     def search_values(keyword):
         return str(cursor.search_value(keyword))
     app.run(port=p)
 
+if __name__ == "__main__":
+    if len(sys.argv)==1:
+        p=int(input("Please enter the service port->"))
+        nzm=input("Please enter the MiniDataBase File name->")
+        passwd=input("Please enter the Database Password ->")
+        service(p,nzm,passwd)
+    else:
+        p=sys.argv[1]
+        nzm=sys.argv[2]
+        passwd=sys.argv[3]
+        service(p,nzm,passwd)
+        
+
```

### Comparing `minidatabase-1.6/minidatabase/minidb.py` & `minidatabase-1.6.1/minidatabase/minidb.py`

 * *Files identical despite different names*

### Comparing `minidatabase-1.6/minidatabase.egg-info/PKG-INFO` & `minidatabase-1.6.1/minidatabase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidatabase
-Version: 1.6
+Version: 1.6.1
 Summary: A tiny database system based on  python dictionary.
 Home-page: http://osdn.xyz
 Author: HansenL
 Author-email: hansenl@foxmail.com
 License:  GNU GENERAL PUBLIC LICENSE
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `minidatabase-1.6/setup.py` & `minidatabase-1.6.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r",encoding='gb18030',errors='ignore') as f:
   long_description = f.read()
 setup(name='minidatabase',  
-      version='1.6',  
+      version='1.6.1',  
       description='A tiny database system based on  python dictionary.',
       long_description=long_description,
       author='HansenL',
       author_email='hansenl@foxmail.com',
       url='http://osdn.xyz',
       install_requires=["requests","flask"],
       license=' GNU GENERAL PUBLIC LICENSE',
@@ -22,10 +22,10 @@
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Topic :: Software Development :: Libraries'
       ],
       entry_points={
-"consloe_scripts":["minidb=minidatabase.minidb:main"]
+"console_scripts":["minidb=minidatabase.minidb:main","webmdb=minidatabase.WebMDB:service"]
           }
       )
```

