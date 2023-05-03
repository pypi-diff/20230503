# Comparing `tmp/shortzy-0.0.5.tar.gz` & `tmp/shortzy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortzy-0.0.5.tar", last modified: Tue Sep 20 16:16:16 2022, max compression
+gzip compressed data, was "shortzy-0.0.6.tar", last modified: Wed May  3 20:47:23 2023, max compression
```

## Comparing `shortzy-0.0.5.tar` & `shortzy-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0 kevinnadar   (501) staff       (20)        0 2022-09-20 16:16:16.680000 shortzy-0.0.5/
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)    34523 2022-07-25 18:03:44.000000 shortzy-0.0.5/LICENSE
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)     6141 2022-09-20 16:16:16.900000 shortzy-0.0.5/PKG-INFO
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)     5442 2022-07-26 18:01:03.000000 shortzy-0.0.5/README.md
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)       38 2022-09-20 16:16:16.900000 shortzy-0.0.5/setup.cfg
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)     1132 2022-09-20 16:15:40.000000 shortzy-0.0.5/setup.py
-drwxrwxrwx   0 kevinnadar   (501) staff       (20)        0 2022-09-20 16:16:16.680000 shortzy-0.0.5/shortzy/
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)       25 2022-07-26 17:34:16.000000 shortzy-0.0.5/shortzy/__init__.py
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)     8316 2022-09-20 16:15:02.000000 shortzy-0.0.5/shortzy/main.py
-drwxrwxrwx   0 kevinnadar   (501) staff       (20)        0 2022-09-20 16:16:16.680000 shortzy-0.0.5/shortzy.egg-info/
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)     6141 2022-09-20 16:16:16.000000 shortzy-0.0.5/shortzy.egg-info/PKG-INFO
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)      216 2022-09-20 16:16:16.000000 shortzy-0.0.5/shortzy.egg-info/SOURCES.txt
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)        1 2022-09-20 16:16:16.000000 shortzy-0.0.5/shortzy.egg-info/dependency_links.txt
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)        8 2022-09-20 16:16:16.000000 shortzy-0.0.5/shortzy.egg-info/requires.txt
--rwxrwxrwx   0 kevinnadar   (501) staff       (20)        8 2022-09-20 16:16:16.000000 shortzy-0.0.5/shortzy.egg-info/top_level.txt
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.480000 shortzy-0.0.6/
+-rwx------   0 kevinnadar   (501) staff       (20)    34523 2023-05-03 20:47:23.580000 shortzy-0.0.6/LICENSE
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-03 20:47:23.910000 shortzy-0.0.6/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)     5442 2023-05-03 20:47:23.590000 shortzy-0.0.6/README.md
+-rwx------   0 kevinnadar   (501) staff       (20)       38 2023-05-03 20:47:23.910000 shortzy-0.0.6/setup.cfg
+-rwx------   0 kevinnadar   (501) staff       (20)     1146 2023-05-03 20:47:23.640000 shortzy-0.0.6/setup.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.510000 shortzy-0.0.6/shortzy/
+-rwx------   0 kevinnadar   (501) staff       (20)       25 2023-05-03 20:47:23.700000 shortzy-0.0.6/shortzy/__init__.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5227 2023-05-03 20:47:23.720000 shortzy-0.0.6/shortzy/adlinkfly.py
+-rwx------   0 kevinnadar   (501) staff       (20)     4552 2023-05-03 20:47:23.760000 shortzy-0.0.6/shortzy/main.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5105 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy/shareus.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-03 20:47:23.520000 shortzy-0.0.6/shortzy.egg-info/
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy.egg-info/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)      256 2023-05-03 20:47:23.800000 shortzy-0.0.6/shortzy.egg-info/SOURCES.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        1 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/dependency_links.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/requires.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-03 20:47:23.810000 shortzy-0.0.6/shortzy.egg-info/top_level.txt
```

### Comparing `shortzy-0.0.5/LICENSE` & `shortzy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.5/PKG-INFO` & `shortzy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.5
+Version: 0.0.6
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
-Keywords: python,droplink,gplink,url-shortener,earn money,shareus
+Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.5 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.6 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
-shortener,earn money,shareus Platform: UNKNOWN Classifier: Development Status
-:: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE
+shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
+System :: Microsoft :: Windows Description-Content-Type: text/markdown License-
+File: LICENSE
                                     [Logo]
                                **** Shortzy ****
         A Unofficial Wrapper for Adlinkfly Site and Alternative Sites
              Â· Report_Bug_/_Request_Feature Â· Usage Â· Reference
 --- # Shortzy An Unofficial Python version of Adlinkfly and Alternative Website
 API wrapper. Used to Short your long link and let you earn from it. ##
 Installation Install shortzy with pip ```bash pip install shortzy ``` To
```

### Comparing `shortzy-0.0.5/README.md` & `shortzy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.5/setup.py` & `shortzy-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper'
 
 # Setting up
 setup(
     name="shortzy",
     version=VERSION,
     author="Kevin Nadar",
@@ -20,17 +20,17 @@
     author_email="jesikamaraj@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['aiohttp',],
     url="https://github.com/kevinnadar22/shortzy",
-    keywords=['python', 'droplink', 'gplink', 'url-shortener', 'earn money', 'shareus'],
+    keywords=['python', 'droplink', 'gplink', 'url-shortener', 'earn money', 'shareus', 'adlinkfly'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `shortzy-0.0.5/shortzy.egg-info/PKG-INFO` & `shortzy-0.0.6/shortzy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.5
+Version: 0.0.6
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
-Keywords: python,droplink,gplink,url-shortener,earn money,shareus
+Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.5 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.6 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
-shortener,earn money,shareus Platform: UNKNOWN Classifier: Development Status
-:: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE
+shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
+System :: Microsoft :: Windows Description-Content-Type: text/markdown License-
+File: LICENSE
                                     [Logo]
                                **** Shortzy ****
         A Unofficial Wrapper for Adlinkfly Site and Alternative Sites
              Â· Report_Bug_/_Request_Feature Â· Usage Â· Reference
 --- # Shortzy An Unofficial Python version of Adlinkfly and Alternative Website
 API wrapper. Used to Short your long link and let you earn from it. ##
 Installation Install shortzy with pip ```bash pip install shortzy ``` To
```

