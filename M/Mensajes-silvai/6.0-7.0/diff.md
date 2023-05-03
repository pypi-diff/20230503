# Comparing `tmp/Mensajes-silvai-6.0.tar.gz` & `tmp/Mensajes-silvai-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-silvai-6.0.tar", last modified: Wed May  3 18:13:18 2023, max compression
+gzip compressed data, was "Mensajes-silvai-7.0.tar", last modified: Wed May  3 18:58:51 2023, max compression
```

## Comparing `Mensajes-silvai-6.0.tar` & `Mensajes-silvai-7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.580011 Mensajes-silvai-6.0/
--rw-rw-rw-   0        0        0     1068 2023-05-03 17:53:07.000000 Mensajes-silvai-6.0/LICENSE
--rw-rw-rw-   0        0        0       58 2022-07-09 15:00:19.000000 Mensajes-silvai-6.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.559258 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-03 18:13:18.000000 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-03 18:13:18.000000 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:13:18.000000 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 18:13:18.000000 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 18:13:18.000000 Mensajes-silvai-6.0/Mensajes_silvai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      695 2023-05-03 18:13:18.578628 Mensajes-silvai-6.0/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-05-03 17:52:43.000000 Mensajes-silvai-6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.561225 Mensajes-silvai-6.0/mensajes/
--rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-silvai-6.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.566227 Mensajes-silvai-6.0/mensajes/adios/
--rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-silvai-6.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-silvai-6.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.571227 Mensajes-silvai-6.0/mensajes/hola/
--rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-silvai-6.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      383 2022-07-09 15:20:17.000000 Mensajes-silvai-6.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-05-03 17:45:14.000000 Mensajes-silvai-6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 18:13:18.580228 Mensajes-silvai-6.0/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-05-03 18:12:32.000000 Mensajes-silvai-6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:13:18.576229 Mensajes-silvai-6.0/tests/
--rw-rw-rw-   0        0        0        0 2022-07-08 18:23:47.000000 Mensajes-silvai-6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      268 2022-07-08 18:20:55.000000 Mensajes-silvai-6.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.082114 Mensajes-silvai-7.0/
+-rw-rw-rw-   0        0        0     1068 2023-05-03 17:53:07.000000 Mensajes-silvai-7.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-07-09 15:00:19.000000 Mensajes-silvai-7.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.060110 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/
+-rw-rw-rw-   0        0        0      747 2023-05-03 18:58:50.000000 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-03 18:58:51.000000 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:58:50.000000 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 18:58:50.000000 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 18:58:50.000000 Mensajes-silvai-7.0/Mensajes_silvai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      747 2023-05-03 18:58:51.080115 Mensajes-silvai-7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-05-03 17:52:43.000000 Mensajes-silvai-7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.063109 Mensajes-silvai-7.0/mensajes/
+-rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-silvai-7.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.068110 Mensajes-silvai-7.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-silvai-7.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-silvai-7.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.073110 Mensajes-silvai-7.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-silvai-7.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-05-03 18:45:36.000000 Mensajes-silvai-7.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-05-03 17:45:14.000000 Mensajes-silvai-7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 18:58:51.082946 Mensajes-silvai-7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-03 18:57:00.000000 Mensajes-silvai-7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:58:51.077111 Mensajes-silvai-7.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-08 18:23:47.000000 Mensajes-silvai-7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      268 2022-07-08 18:20:55.000000 Mensajes-silvai-7.0/tests/test_hola.py
```

### Comparing `Mensajes-silvai-6.0/LICENSE` & `Mensajes-silvai-7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-silvai-6.0/Mensajes_silvai.egg-info/PKG-INFO` & `Mensajes-silvai-7.0/Mensajes_silvai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Mensajes-silvai
-Version: 6.0
+Version: 7.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Isaac Silva
 Author-email: ijsc_11@hotmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mensajes
 
 El paquete de mensajerÃ­a para pruebas de Isaac Silva .
```

### Comparing `Mensajes-silvai-6.0/PKG-INFO` & `Mensajes-silvai-7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Mensajes-silvai
-Version: 6.0
+Version: 7.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Isaac Silva
 Author-email: ijsc_11@hotmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mensajes
 
 El paquete de mensajerÃ­a para pruebas de Isaac Silva .
```

### Comparing `Mensajes-silvai-6.0/setup.py` & `Mensajes-silvai-7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pickletools import long1
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-silvai',
-    version='6.0',
+    version='7.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Isaac Silva',
     author_email='ijsc_11@hotmail.com',
     url='https://www.hektor.dev',
     license_files=['LICENSE'],
@@ -20,10 +20,11 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Utilities',
     ],
 )
```

