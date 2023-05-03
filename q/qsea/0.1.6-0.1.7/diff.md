# Comparing `tmp/qsea-0.1.6.tar.gz` & `tmp/qsea-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.6.tar", last modified: Tue Apr 11 22:32:00 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.7.tar", last modified: Wed May  3 16:34:52 2023, max compression
```

## Comparing `qsea-0.1.6.tar` & `qsea-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.237865 qsea-0.1.6/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 22:32:00.235784 qsea-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.222792 qsea-0.1.6/qsea/
--rw-rw-rw-   0        0        0    61145 2023-04-11 22:30:58.000000 qsea-0.1.6/qsea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.234783 qsea-0.1.6/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 22:32:00.237865 qsea-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-04-11 22:31:48.000000 qsea-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:34:52.190374 qsea-0.1.7/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-05-03 16:34:52.189375 qsea-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 16:34:52.181381 qsea-0.1.7/qsea/
+-rw-rw-rw-   0        0        0    61145 2023-04-11 22:30:58.000000 qsea-0.1.7/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:34:52.188375 qsea-0.1.7/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-05-03 16:34:50.000000 qsea-0.1.7/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-03 16:34:51.000000 qsea-0.1.7/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:34:50.000000 qsea-0.1.7/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-03 16:34:50.000000 qsea-0.1.7/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 16:34:50.000000 qsea-0.1.7/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:34:52.190374 qsea-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-05-03 16:33:30.000000 qsea-0.1.7/setup.py
```

### Comparing `qsea-0.1.6/LICENSE.txt` & `qsea-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.6/PKG-INFO` & `qsea-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.6/qsea/__init__.py` & `qsea-0.1.7/qsea/__init__.py`

 * *Files identical despite different names*

### Comparing `qsea-0.1.6/qsea.egg-info/PKG-INFO` & `qsea-0.1.7/qsea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.6/setup.py` & `qsea-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.6',
+    version='0.1.7',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
     keywords=['QlikSense', 'Qlik'],
     url='https://github.com/ncthuc/qsea',
     download_url='https://pypi.org/project/qsea/'
 )
 
-install_requires = ['pandas', 'datetime', 'websocket']
+install_requires = ['pandas', 'datetime', 'websocket-client']
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

