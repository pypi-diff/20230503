# Comparing `tmp/amseg-1.5.tar.gz` & `tmp/amseg-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amseg-1.5.tar", last modified: Thu Apr 14 11:34:09 2022, max compression
+gzip compressed data, was "dist/amseg-1.7.tar", last modified: Fri Apr 15 16:24:06 2022, max compression
```

## Comparing `amseg-1.5.tar` & `amseg-1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-14 11:34:09.000000 amseg-1.5/
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)       52 2022-04-13 10:55:29.000000 amseg-1.5/HOWTO-INSTALL.txt
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     1061 2021-10-30 23:55:37.000000 amseg-1.5/LICENSE.txt
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      159 2021-11-05 08:49:39.000000 amseg-1.5/MANIFEST
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3761 2022-04-14 11:34:09.000000 amseg-1.5/PKG-INFO
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2223 2021-12-21 11:15:10.000000 amseg-1.5/README.md
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2757 2022-04-14 11:19:50.000000 amseg-1.5/README.rst
-drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-14 11:34:09.000000 amseg-1.5/amseg/
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      217 2022-04-13 11:14:15.000000 amseg-1.5/amseg/__init__.py
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3313 2021-10-30 23:45:56.000000 amseg-1.5/amseg/amharicNormalizer.py
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)    13004 2021-10-30 23:45:56.000000 amseg-1.5/amseg/amharicRomanizer.py
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3730 2021-10-31 01:40:17.000000 amseg-1.5/amseg/amharicSegmenter.py
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)    10076 2022-04-14 10:49:41.000000 amseg-1.5/amseg/amharicTranslitrator.py
-drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-14 11:34:09.000000 amseg-1.5/amseg.egg-info/
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3761 2022-04-14 11:34:08.000000 amseg-1.5/amseg.egg-info/PKG-INFO
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      321 2022-04-14 11:34:08.000000 amseg-1.5/amseg.egg-info/SOURCES.txt
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)        1 2022-04-14 11:34:08.000000 amseg-1.5/amseg.egg-info/dependency_links.txt
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)        6 2022-04-14 11:34:08.000000 amseg-1.5/amseg.egg-info/top_level.txt
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)       79 2022-04-14 11:34:09.000000 amseg-1.5/setup.cfg
--rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2029 2022-04-14 11:33:37.000000 amseg-1.5/setup.py
+drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-15 16:24:06.000000 amseg-1.7/
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)       52 2022-04-13 10:55:29.000000 amseg-1.7/HOWTO-INSTALL.txt
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     1061 2021-10-30 23:55:37.000000 amseg-1.7/LICENSE.txt
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      159 2021-11-05 08:49:39.000000 amseg-1.7/MANIFEST
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3761 2022-04-15 16:24:06.000000 amseg-1.7/PKG-INFO
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2223 2021-12-21 11:15:10.000000 amseg-1.7/README.md
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2757 2022-04-14 11:19:50.000000 amseg-1.7/README.rst
+drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-15 16:24:06.000000 amseg-1.7/amseg/
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      217 2022-04-13 11:14:15.000000 amseg-1.7/amseg/__init__.py
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3313 2021-10-30 23:45:56.000000 amseg-1.7/amseg/amharicNormalizer.py
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)    13004 2021-10-30 23:45:56.000000 amseg-1.7/amseg/amharicRomanizer.py
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3730 2021-10-31 01:40:17.000000 amseg-1.7/amseg/amharicSegmenter.py
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)    10076 2022-04-15 16:22:45.000000 amseg-1.7/amseg/amharicTranslitrator.py
+drwxr-xr-x   0 seidmuhieyimam   (501) staff       (20)        0 2022-04-15 16:24:06.000000 amseg-1.7/amseg.egg-info/
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     3761 2022-04-15 16:24:06.000000 amseg-1.7/amseg.egg-info/PKG-INFO
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)      321 2022-04-15 16:24:06.000000 amseg-1.7/amseg.egg-info/SOURCES.txt
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)        1 2022-04-15 16:24:06.000000 amseg-1.7/amseg.egg-info/dependency_links.txt
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)        6 2022-04-15 16:24:06.000000 amseg-1.7/amseg.egg-info/top_level.txt
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)       79 2022-04-15 16:24:06.000000 amseg-1.7/setup.cfg
+-rw-r--r--   0 seidmuhieyimam   (501) staff       (20)     2029 2022-04-15 16:23:59.000000 amseg-1.7/setup.py
```

### Comparing `amseg-1.5/LICENSE.txt` & `amseg-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amseg-1.5/PKG-INFO` & `amseg-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: amseg
-Version: 1.5
+Version: 1.7
 Summary: This is an Amharic document segmentation and normalization tool
 Home-page: https://github.com/uhh-lt/amharicprocessor
 Author: Seid Muhie Yimam
 Author-email: seid.muhie.yimam@uni-hamburg.de
 License: MIT
-Download-URL: https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_15.tar.gz
+Download-URL: https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_17.tar.gz
 Keywords: Amharic,Amharic sentence splitter,Amharic document normalizer,Amharic Latin to Fidel Transliteration
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `amseg-1.5/README.md` & `amseg-1.7/README.md`

 * *Files identical despite different names*

### Comparing `amseg-1.5/README.rst` & `amseg-1.7/README.rst`

 * *Files identical despite different names*

### Comparing `amseg-1.5/amseg/amharicNormalizer.py` & `amseg-1.7/amseg/amharicNormalizer.py`

 * *Files identical despite different names*

### Comparing `amseg-1.5/amseg/amharicRomanizer.py` & `amseg-1.7/amseg/amharicRomanizer.py`

 * *Files identical despite different names*

### Comparing `amseg-1.5/amseg/amharicSegmenter.py` & `amseg-1.7/amseg/amharicSegmenter.py`

 * *Files identical despite different names*

### Comparing `amseg-1.5/amseg/amharicTranslitrator.py` & `amseg-1.7/amseg/amharicTranslitrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         norm = norm.replace("p", "ፕ")
         norm = norm.replace("ca", "ካ")
         norm = norm.replace("ci", "ሲ")
         norm = norm.replace("ce", "ሰ")
         norm = norm.replace("cu", "ኩ")
         norm = norm.replace("c ", "ክ")
         norm = norm.replace(" gn ", "ግን")
-        norm = norm.replace("c", "ቸ")
+        norm = norm.replace("c", "ች")
         norm = norm.replace("xe", "ዘ")
         norm = norm.replace("xu", "ዙ")
         norm = norm.replace("xi", "ዚ")
         norm = norm.replace("xa", "ዛ")
         norm = norm.replace("xo", "ዞ")
         norm = norm.replace("x", "ክስ")
         norm = norm.replace("xs", "ክስ")
```

### Comparing `amseg-1.5/amseg.egg-info/PKG-INFO` & `amseg-1.7/amseg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: amseg
-Version: 1.5
+Version: 1.7
 Summary: This is an Amharic document segmentation and normalization tool
 Home-page: https://github.com/uhh-lt/amharicprocessor
 Author: Seid Muhie Yimam
 Author-email: seid.muhie.yimam@uni-hamburg.de
 License: MIT
-Download-URL: https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_15.tar.gz
+Download-URL: https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_17.tar.gz
 Keywords: Amharic,Amharic sentence splitter,Amharic document normalizer,Amharic Latin to Fidel Transliteration
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `amseg-1.5/setup.py` & `amseg-1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, Extension
 def readme():
     with open('README.rst') as f:
         return f.read()
 setup(
   name = 'amseg',         # Amharic Sentence segmentation, tokenization and normalization tools
   packages = ['amseg'],   # Chose the same as "name"
-  version = '1.5',      # Start with a small number and increase it with every change you make
+  version = '1.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is an Amharic document segmentation and normalization tool',   # Give a short description about your library
   long_description=readme(),
   author = 'Seid Muhie Yimam',                   # Type in your name
   author_email = 'seid.muhie.yimam@uni-hamburg.de',      # Type in your E-Mail
   url = 'https://github.com/uhh-lt/amharicprocessor',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_15.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/uhh-lt/amharicprocessor/archive/rehistoryfs/tags/v_17.tar.gz',    # I explain this later on
   keywords = ['Amharic', 'Amharic sentence splitter', 'Amharic document normalizer', 'Amharic Latin to Fidel Transliteration'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
          # 'validators',
         #  'beautifulsoup4',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

