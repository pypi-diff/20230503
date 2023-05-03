# Comparing `tmp/magyar-2.9.8.tar.gz` & `tmp/magyar-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.8.tar", last modified: Mon Apr 24 08:06:58 2023, max compression
+gzip compressed data, was "magyar-2.9.9.tar", last modified: Wed May  3 19:34:15 2023, max compression
```

## Comparing `magyar-2.9.8.tar` & `magyar-2.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-24 08:06:58.405506 magyar-2.9.8/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5329 2023-04-24 08:06:58.405506 magyar-2.9.8/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     4931 2023-04-24 08:05:27.000000 magyar-2.9.8/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-24 08:06:58.401506 magyar-2.9.8/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5329 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    36025 2023-04-24 08:05:27.000000 magyar-2.9.8/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-24 08:06:58.405506 magyar-2.9.8/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-04-24 07:32:32.000000 magyar-2.9.8/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-03 19:34:15.241380 magyar-2.9.9/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5398 2023-05-03 19:34:15.237380 magyar-2.9.9/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5000 2023-05-03 19:14:22.000000 magyar-2.9.9/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-03 19:34:15.237380 magyar-2.9.9/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5398 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    36183 2023-05-03 19:14:22.000000 magyar-2.9.9/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-03 19:34:15.241380 magyar-2.9.9/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-05-03 19:14:22.000000 magyar-2.9.9/setup.py
```

### Comparing `magyar-2.9.8/PKG-INFO` & `magyar-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.8
+Version: 2.9.9
 Summary: Hungarian names,animals,food, fruit, river ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -122,14 +122,19 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
+3. Listák ABC sorrendbe rendezése  </br>
+
+
+    magyar.abc(lista):
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.8/README.md` & `magyar-2.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
+3. Listák ABC sorrendbe rendezése  </br>
+
+
+    magyar.abc(lista):
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.8/magyar.egg-info/PKG-INFO` & `magyar-2.9.9/magyar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.8
+Version: 2.9.9
 Summary: Hungarian names,animals,food, fruit, river ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -122,14 +122,19 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
+3. Listák ABC sorrendbe rendezése  </br>
+
+
+    magyar.abc(lista):
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.8/magyar.py` & `magyar-2.9.9/magyar.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,8 +362,12 @@
 
 def tordel(lst, n=None):  # lst = kiírandó lista, n = hany kerüljön  egy sorba
     if n is None:
         n = 10
     for i in range(0, len(lst), n):
         row = lst[i:i+n]
         print(", ".join(map(str, row)), end=", ")
-        print()
+        print()
+
+ABECEDARAK = 'aábcdeéfghiíjklmnoóöőpqrstuúüűvwxyz'
+def abc(lista):
+    return sorted(lista, key=lambda s: [ABECEDARAK.find(c) for c in s.lower()])
```

### Comparing `magyar-2.9.8/setup.py` & `magyar-2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.8",
+    version="2.9.9",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names,animals,food, fruit, river ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

