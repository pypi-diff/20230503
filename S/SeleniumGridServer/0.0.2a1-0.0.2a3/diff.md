# Comparing `tmp/SeleniumGridServer-0.0.2a1.tar.gz` & `tmp/SeleniumGridServer-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeleniumGridServer-0.0.2a1.tar", last modified: Fri Jan 13 03:00:40 2023, max compression
+gzip compressed data, was "SeleniumGridServer-0.0.2a3.tar", last modified: Wed May  3 03:24:17 2023, max compression
```

## Comparing `SeleniumGridServer-0.0.2a1.tar` & `SeleniumGridServer-0.0.2a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 03:00:40.485297 SeleniumGridServer-0.0.2a1/
--rw-rw-rw-   0        0        0       17 2020-09-27 09:55:47.000000 SeleniumGridServer-0.0.2a1/MANIFEST.in
--rw-rw-rw-   0        0        0      272 2023-01-13 03:00:40.485297 SeleniumGridServer-0.0.2a1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2022-10-02 09:22:50.000000 SeleniumGridServer-0.0.2a1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 03:00:40.477291 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/
--rw-rw-rw-   0        0        0      272 2023-01-13 03:00:40.000000 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-01-13 03:00:40.000000 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 03:00:40.000000 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-01-13 03:00:40.000000 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-01-13 03:00:40.000000 SeleniumGridServer-0.0.2a1/SeleniumGridServer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-13 03:00:40.487294 SeleniumGridServer-0.0.2a1/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-01-13 03:00:19.000000 SeleniumGridServer-0.0.2a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-13 03:00:40.451933 SeleniumGridServer-0.0.2a1/src/
-drwxrwxrwx   0        0        0        0 2023-01-13 03:00:40.481305 SeleniumGridServer-0.0.2a1/src/SeleniumGridServer/
--rw-rw-rw-   0        0        0     1817 2023-01-13 02:42:04.000000 SeleniumGridServer-0.0.2a1/src/SeleniumGridServer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:24:17.395679 SeleniumGridServer-0.0.2a3/
+-rw-rw-rw-   0        0        0       17 2020-09-27 09:55:47.000000 SeleniumGridServer-0.0.2a3/MANIFEST.in
+-rw-rw-rw-   0        0        0      272 2023-05-03 03:24:17.392433 SeleniumGridServer-0.0.2a3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2022-10-02 09:22:50.000000 SeleniumGridServer-0.0.2a3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 03:24:17.377488 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-05-03 03:24:17.000000 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-05-03 03:24:17.000000 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:24:17.000000 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-03 03:24:17.000000 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 03:24:17.000000 SeleniumGridServer-0.0.2a3/SeleniumGridServer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:24:17.396681 SeleniumGridServer-0.0.2a3/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-05-03 03:24:05.000000 SeleniumGridServer-0.0.2a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:24:17.345239 SeleniumGridServer-0.0.2a3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:24:17.385458 SeleniumGridServer-0.0.2a3/src/SeleniumGridServer/
+-rw-rw-rw-   0        0        0     1973 2023-05-03 03:23:35.000000 SeleniumGridServer-0.0.2a3/src/SeleniumGridServer/__init__.py
```

### Comparing `SeleniumGridServer-0.0.2a1/setup.py` & `SeleniumGridServer-0.0.2a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='SeleniumGridServer',
-    version='0.0.2a1',
+    version='0.0.2a3',
     description='ChokChaisak',
     long_description=readme(),
     url='https://test.pypi.org/user/ChokChaisak/',
     author='ChokChaisak',
     author_email='ChokChaisak@gmail.com',
     license='ChokChaisak',
     install_requires=[
```

### Comparing `SeleniumGridServer-0.0.2a1/src/SeleniumGridServer/__init__.py` & `SeleniumGridServer-0.0.2a3/src/SeleniumGridServer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # encoding: utf-8
 import os
 import jdk
 import time
 import glob
 import urllib.request
 import psutil
+from robot.api.deco import keyword
 
 current_path = os.path.dirname(os.path.abspath(__file__)).replace('\\', '/')
 main_path = os.path.dirname(current_path)
 
-class SeleniumGridServer():
+class SeleniumGridServer(object):
     
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
     ROBOT_LIBRARY_VERSION = 0.1
     
     def __init__(self):
-        self.killdriver()
-        java_path = self.java_loader()
-        selenium_path = self.selenium()
-        port_num = [i.laddr.port for i in psutil.net_connections()]
-        if not 4444 in port_num:
-            command = '%s/java -jar %s standalone --port 4444' %(java_path, selenium_path)
-            os.popen(command)
-            time.sleep(5)
+        pass
         
     def killdriver(self):
         for proc in psutil.process_iter():
             if 'chromedriver' in proc.name():
                 proc.kill()
             if 'geckodriver' in proc.name():
                 proc.kill()
@@ -45,7 +39,19 @@
         return os_name[0].replace('\\', '/')
         
     def selenium(self):
         if not 'selenium-server.jar' in os.listdir(main_path):
             url = 'https://github.com/SeleniumHQ/selenium/releases/download/selenium-4.7.0/selenium-server-4.7.2.jar'
             urllib.request.urlretrieve(url, '%s/selenium-server.jar' %(main_path))
         return '%s/selenium-server.jar' %(main_path)
+
+    @keyword('Start Server')
+    def start_Server(self, port=4444):
+        self.port = port
+        self.killdriver()
+        java_path = self.java_loader()
+        selenium_path = self.selenium()
+        port_num = [i.laddr.port for i in psutil.net_connections()]
+        if not port in port_num:
+            command = '%s/java -jar %s standalone --port %s' %(java_path, selenium_path, port)
+            os.popen(command)
+            time.sleep(5)
```

