# Comparing `tmp/KMMTR-0.0.1.tar.gz` & `tmp/KMMTR-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-0.0.1.tar", last modified: Thu Apr 20 09:05:14 2023, max compression
+gzip compressed data, was "KMMTR-0.0.2.tar", last modified: Wed May  3 02:59:05 2023, max compression
```

## Comparing `KMMTR-0.0.1.tar` & `KMMTR-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-20 09:05:14.725624 KMMTR-0.0.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-20 09:05:14.724693 KMMTR-0.0.1/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6295 2023-04-20 03:28:47.000000 KMMTR-0.0.1/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6509 2023-04-20 09:00:35.000000 KMMTR-0.0.1/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.1/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-20 09:05:14.725332 KMMTR-0.0.1/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-04-20 09:05:14.000000 KMMTR-0.0.1/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-04-20 09:05:14.000000 KMMTR-0.0.1/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-04-20 09:05:14.000000 KMMTR-0.0.1/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-04-20 09:05:14.000000 KMMTR-0.0.1/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-04-20 09:05:14.000000 KMMTR-0.0.1/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-04-20 09:05:14.725496 KMMTR-0.0.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-04-20 09:05:14.725666 KMMTR-0.0.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-04-20 09:03:22.000000 KMMTR-0.0.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-03 02:59:05.131583 KMMTR-0.0.2/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-03 02:59:05.130607 KMMTR-0.0.2/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6295 2023-04-20 03:28:47.000000 KMMTR-0.0.2/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6511 2023-05-03 02:58:16.000000 KMMTR-0.0.2/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.2/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-03 02:59:05.131241 KMMTR-0.0.2/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-03 02:59:05.000000 KMMTR-0.0.2/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-03 02:59:05.000000 KMMTR-0.0.2/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-03 02:59:05.000000 KMMTR-0.0.2/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-03 02:59:05.000000 KMMTR-0.0.2/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-03 02:59:05.000000 KMMTR-0.0.2/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-03 02:59:05.131442 KMMTR-0.0.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.2/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-03 02:59:05.131626 KMMTR-0.0.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-03 02:58:27.000000 KMMTR-0.0.2/setup.py
```

### Comparing `KMMTR-0.0.1/KMMTR/KMM.py` & `KMMTR-0.0.2/KMMTR/KMM.py`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.1/KMMTR/KMMTR.py` & `KMMTR-0.0.2/KMMTR/KMMTR.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             print("The estimator.fit does not have 'sample_weight' attribute.")
             print('Please provide another Regressor')
             raise ValueError("Error of Regressor")
 
 def GenerateReg(Regressor_name):
     if Regressor_name == 'RF':
         from sklearn.ensemble import RandomForestRegressor
-        mdoel = RandomForestRegressor
+        mdoel = RandomForestRegressor()
     elif Regressor_name == 'LR':
         from sklearn import linear_model
         mdoel = linear_model.LinearRegression()
     else:
         print('Sorry, Bin did not define this function for you, please pass it in yourself')
     return mdoel
```

### Comparing `KMMTR-0.0.1/KMMTR.egg-info/PKG-INFO` & `KMMTR-0.0.2/KMMTR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.1
+Version: 0.0.2
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.1/PKG-INFO` & `KMMTR-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.1
+Version: 0.0.2
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.1/README.md` & `KMMTR-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.1/setup.py` & `KMMTR-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='0.0.1',  # 版本
+    version='0.0.2',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

