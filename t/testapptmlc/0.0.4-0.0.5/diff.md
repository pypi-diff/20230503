# Comparing `tmp/testapptmlc-0.0.4.tar.gz` & `tmp/testapptmlc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testapptmlc-0.0.4.tar", last modified: Wed May  3 10:21:19 2023, max compression
+gzip compressed data, was "dist\testapptmlc-0.0.5.tar", last modified: Wed May  3 13:16:18 2023, max compression
```

## Comparing `testapptmlc-0.0.4.tar` & `testapptmlc-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      650 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.4/README.md
--rw-rw-rw-   0        0        0      565 2023-05-03 10:21:05.000000 testapptmlc-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1910 2023-05-03 10:21:01.000000 testapptmlc-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/src/
--rw-rw-rw-   0        0        0       22 2023-05-03 09:58:30.000000 testapptmlc-0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/src/runapp/
--rw-rw-rw-   0        0        0       43 2023-05-03 10:02:23.000000 testapptmlc-0.0.4/src/runapp/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-03 09:38:32.000000 testapptmlc-0.0.4/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:21:19.000000 testapptmlc-0.0.4/testapptmlc.egg-info/
--rw-rw-rw-   0        0        0      650 2023-05-03 10:21:18.000000 testapptmlc-0.0.4/testapptmlc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-03 10:21:18.000000 testapptmlc-0.0.4/testapptmlc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:21:18.000000 testapptmlc-0.0.4/testapptmlc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 10:21:18.000000 testapptmlc-0.0.4/testapptmlc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 10:21:18.000000 testapptmlc-0.0.4/testapptmlc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.5/README.md
+-rw-rw-rw-   0        0        0      565 2023-05-03 12:51:34.000000 testapptmlc-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      129 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1888 2023-05-03 13:14:50.000000 testapptmlc-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/src/runapp/
+-rw-rw-rw-   0        0        0       43 2023-05-03 12:51:20.000000 testapptmlc-0.0.5/src/runapp/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-03 13:06:07.000000 testapptmlc-0.0.5/src/runapp/app.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-05-03 13:16:17.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-03 13:16:18.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:16:17.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 13:16:17.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 13:16:17.000000 testapptmlc-0.0.5/src/testapptmlc.egg-info/top_level.txt
```

### Comparing `testapptmlc-0.0.4/LICENSE` & `testapptmlc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.0.4/PKG-INFO` & `testapptmlc-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.4
+Version: 0.0.5
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

### Comparing `testapptmlc-0.0.4/pyproject.toml` & `testapptmlc-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "testapptmlc"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="TMLC", email="visalakshi2001@gmail.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `testapptmlc-0.0.4/setup.py` & `testapptmlc-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='testapptmlc',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages= ["testapptmlc", "testapptmlc.runapp"],
-    package_dir={'testapptmlc': 'src'},
+    packages= find_packages(where="src"),
+    package_dir={'': 'src'},
     url='https://github.com/visalakshi2001/tmlc-pypi',
     keywords='speech recognizer',
     setup_requires=['vosk'],
     install_requires=['vosk'],
     cmdclass={
         'install': CustomInstallCommand,
     },
```

### Comparing `testapptmlc-0.0.4/src/runapp/app.py` & `testapptmlc-0.0.5/src/runapp/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # crack https://github.com/Eddie2111/ProblemSolvers/commit/a109ac434465359db62f41d9c7dddc8c2f37924e
+# model = Model("Vosk/vosk-model-en-in-0.5") 
 
-def recognise(recognizer):
-    mic = pyaudio.PyAudio()
-    stream = mic.open(rate=16000, channels=1, format=pyaudio.paInt16,input=True, frames_per_buffer=8192)
-    stream.start_stream()
-    print('start speaking')
-    
-    
-    while True:
-    
-        data = stream.read(4096)
-        if len(data) == 0:
-            break
-        if recognizer.AcceptWaveform(data):
-            x = recognizer.Result()
-            print(x)
-            break
-    return x
-
-if __name__ == "__main__":
-    from vosk import Model, KaldiRecognizer
-    import pyaudio
 
-    # model = Model("Vosk/vosk-model-en-in-0.5") 
+from vosk import Model, KaldiRecognizer
+import pyaudio
 
-    model = Model("Vosk/vosk-model-en-us-daanzu-20200905-lgraph")
+class Recognize(object):
 
-
-    recognizer = KaldiRecognizer(model,16000)
+    def __init__(self):
+        self.model = Model("Vosk/vosk-model-en-us-daanzu-20200905-lgraph")
+        self.recognizer = KaldiRecognizer(self.model,16000)
+
+    def __str__(self):
+        return """Class to initiate speech recognizer"""
+
+    def model(self):
+        return self.recognizer
+
+    @classmethod
+    def recognize(recognizer_model):
+        mic = pyaudio.PyAudio()
+        stream = mic.open(rate=16000, channels=1, format=pyaudio.paInt16,input=True, frames_per_buffer=8192)
+        stream.start_stream()
+        print('start speaking')
+
+        while True:
+            data = stream.read(4096)
+            if len(data) == 0:
+                break
+            if recognizer_model.AcceptWaveform(data):
+                x = recognizer_model.Result()
+                print(x)
+                break
+        return x
```

### Comparing `testapptmlc-0.0.4/testapptmlc.egg-info/PKG-INFO` & `testapptmlc-0.0.5/src/testapptmlc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.4
+Version: 0.0.5
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

