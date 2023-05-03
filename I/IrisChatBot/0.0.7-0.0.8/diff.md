# Comparing `tmp/IrisChatBot-0.0.7.tar.gz` & `tmp/IrisChatBot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IrisChatBot-0.0.7.tar", last modified: Tue May  2 23:25:34 2023, max compression
+gzip compressed data, was "IrisChatBot-0.0.8.tar", last modified: Wed May  3 00:16:01 2023, max compression
```

## Comparing `IrisChatBot-0.0.7.tar` & `IrisChatBot-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.215209 IrisChatBot-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/IrisChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      617 2023-05-02 23:25:34.000000 IrisChatBot-0.0.7/IrisChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      552 2023-05-02 23:25:34.000000 IrisChatBot-0.0.7/IrisChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 23:25:34.000000 IrisChatBot-0.0.7/IrisChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-05-02 23:25:34.000000 IrisChatBot-0.0.7/IrisChatBot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      617 2023-05-02 23:25:34.215209 IrisChatBot-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/bancoazteca/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/
--rw-r--r--   0 root         (0) root         (0)     7204 2023-04-28 22:13:08.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/Clientes.py
--rw-r--r--   0 root         (0) root         (0)     6518 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/Credimax.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 23:25:34.211209 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/utilerias/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/utilerias/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-04-28 04:52:26.000000 IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/utilerias/constantes.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 23:25:34.215209 IrisChatBot-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-02 23:24:31.000000 IrisChatBot-0.0.7/setup.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.907210 IrisChatBot-0.0.8/
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/IrisChatBot.egg-info/
+-rwxrwxrwx   0 cycmovil  (1000) cycmovil  (1000)      587 2023-05-03 00:16:01.000000 IrisChatBot-0.0.8/IrisChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 cycmovil  (1000) cycmovil  (1000)      710 2023-05-03 00:16:01.000000 IrisChatBot-0.0.8/IrisChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 cycmovil  (1000) cycmovil  (1000)        1 2023-05-03 00:16:01.000000 IrisChatBot-0.0.8/IrisChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 cycmovil  (1000) cycmovil  (1000)        3 2023-05-03 00:16:01.000000 IrisChatBot-0.0.8/IrisChatBot.egg-info/top_level.txt
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     1073 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/LICENSE.txt
+-rw-rw-r--   0 cycmovil  (1000) cycmovil  (1000)      587 2023-05-03 00:16:01.907210 IrisChatBot-0.0.8/PKG-INFO
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)      472 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/README.md
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/com/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/com/bancoazteca/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     7204 2023-04-28 22:13:08.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/Clientes.py
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     6518 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/Credimax.py
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.903210 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/__init__.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.907210 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/seguridad/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     2087 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/seguridad/Apigee.py
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     4380 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/seguridad/Crypto.py
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     3071 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/seguridad/LlavesCobranza.py
+drwxrwxr-x   0 cycmovil  (1000) cycmovil  (1000)        0 2023-05-03 00:16:01.907210 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/utilerias/
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)        0 2023-04-27 21:02:45.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/utilerias/__init__.py
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     1627 2023-04-28 04:52:26.000000 IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/utilerias/constantes.py
+-rw-rw-r--   0 cycmovil  (1000) cycmovil  (1000)       38 2023-05-03 00:16:01.907210 IrisChatBot-0.0.8/setup.cfg
+-rw-r--r--   0 cycmovil  (1000) cycmovil  (1000)     1002 2023-05-03 00:13:02.000000 IrisChatBot-0.0.8/setup.py
```

### Comparing `IrisChatBot-0.0.7/IrisChatBot.egg-info/PKG-INFO` & `IrisChatBot-0.0.8/IrisChatBot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: IrisChatBot
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
 Home-page: http://devops:8181/cloud/irischatbot
 Author: Chapter Cloud and DevOps
 Author-email: clouddevops@elektra.com.mx
 License: License :: OSI Approved :: MIT License
-Description: UNKNOWN
 Keywords: BAZ,Cobranza,Cloud,Iris,Bot,ChatBot,Core
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE.txt
```

### Comparing `IrisChatBot-0.0.7/IrisChatBot.egg-info/SOURCES.txt` & `IrisChatBot-0.0.8/IrisChatBot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,9 +9,12 @@
 mx/com/__init__.py
 mx/com/bancoazteca/__init__.py
 mx/com/bancoazteca/cloud/__init__.py
 mx/com/bancoazteca/cloud/abonos/Clientes.py
 mx/com/bancoazteca/cloud/abonos/Credimax.py
 mx/com/bancoazteca/cloud/abonos/__init__.py
 mx/com/bancoazteca/cloud/core/__init__.py
+mx/com/bancoazteca/cloud/core/seguridad/Apigee.py
+mx/com/bancoazteca/cloud/core/seguridad/Crypto.py
+mx/com/bancoazteca/cloud/core/seguridad/LlavesCobranza.py
 mx/com/bancoazteca/cloud/core/utilerias/__init__.py
 mx/com/bancoazteca/cloud/core/utilerias/constantes.py
```

### Comparing `IrisChatBot-0.0.7/LICENSE.txt` & `IrisChatBot-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `IrisChatBot-0.0.7/PKG-INFO` & `IrisChatBot-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: IrisChatBot
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
 Home-page: http://devops:8181/cloud/irischatbot
 Author: Chapter Cloud and DevOps
 Author-email: clouddevops@elektra.com.mx
 License: License :: OSI Approved :: MIT License
-Description: UNKNOWN
 Keywords: BAZ,Cobranza,Cloud,Iris,Bot,ChatBot,Core
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE.txt
```

### Comparing `IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/Clientes.py` & `IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/Clientes.py`

 * *Files identical despite different names*

### Comparing `IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/abonos/Credimax.py` & `IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/abonos/Credimax.py`

 * *Files identical despite different names*

### Comparing `IrisChatBot-0.0.7/mx/com/bancoazteca/cloud/core/utilerias/constantes.py` & `IrisChatBot-0.0.8/mx/com/bancoazteca/cloud/core/utilerias/constantes.py`

 * *Files identical despite different names*

### Comparing `IrisChatBot-0.0.7/setup.py` & `IrisChatBot-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='IrisChatBot',
-    version='0.0.7',
+    version='0.0.8',
     packages=['mx', 'mx.com', 'mx.com.bancoazteca', 'mx.com.bancoazteca.cloud', 'mx.com.bancoazteca.cloud.core',
-              'mx.com.bancoazteca.cloud.core.utilerias', 'mx.com.bancoazteca.cloud.abonos'],
+              'mx.com.bancoazteca.cloud.core.utilerias', 'mx.com.bancoazteca.cloud.core.seguridad', 'mx.com.bancoazteca.cloud.abonos'],
     url='http://devops:8181/cloud/irischatbot',
     license='License :: OSI Approved :: MIT License',
     author='Chapter Cloud and DevOps',
     author_email='clouddevops@elektra.com.mx',
     description='',
     dependencies = [ # Optional
       "requests","pycryptodome"
```

