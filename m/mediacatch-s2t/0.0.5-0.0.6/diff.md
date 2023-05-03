# Comparing `tmp/mediacatch-s2t-0.0.5.tar.gz` & `tmp/mediacatch-s2t-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacatch-s2t-0.0.5.tar", last modified: Mon Apr 24 13:42:18 2023, max compression
+gzip compressed data, was "mediacatch-s2t-0.0.6.tar", last modified: Wed May  3 13:37:41 2023, max compression
```

## Comparing `mediacatch-s2t-0.0.5.tar` & `mediacatch-s2t-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.5/LICENSE
--rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.5/MANIFEST.in
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/README.md
--rw-rw-r--   0 frederik  (1002) mc       (10000)      899 2023-04-24 13:31:58.000000 mediacatch-s2t-0.0.5/pyproject.toml
--rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/setup.cfg
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/mediacatch_s2t/
--rw-rw-r--   0 frederik  (1002) mc       (10000)      546 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/__init__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     1297 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/__main__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     5729 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/uploader.py
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      414 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/requires.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/top_level.txt
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/tests/
--rw-rw-r--   0 frederik  (1002) mc       (10000)     2464 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/tests/test_uploader.py
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.6/LICENSE
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.6/MANIFEST.in
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.6/README.md
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      899 2023-05-03 13:35:20.000000 mediacatch-s2t-0.0.6/pyproject.toml
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/setup.cfg
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/mediacatch_s2t/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      994 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/__init__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     1297 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/__main__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    14007 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/uploader.py
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      445 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/requires.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/top_level.txt
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/tests/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    10862 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/tests/test_multipart_upload.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     2884 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/tests/test_uploader.py
```

### Comparing `mediacatch-s2t-0.0.5/LICENSE` & `mediacatch-s2t-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.5/PKG-INFO` & `mediacatch-s2t-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.5
+Version: 0.0.6
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mediacatch-s2t-0.0.5/README.md` & `mediacatch-s2t-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.5/pyproject.toml` & `mediacatch-s2t-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mediacatch-s2t"
-version = "0.0.5"
+version = "0.0.6"
 description = "Upload a media file and get the transcription link."
 readme = "README.md"
 authors = [{ name = "MediaCatch", email = "support@mediacatch.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mediacatch-s2t-0.0.5/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-0.0.6/src/mediacatch_s2t/__main__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.5
+Version: 0.0.6
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mediacatch-s2t-0.0.5/tests/test_uploader.py` & `mediacatch-s2t-0.0.6/tests/test_uploader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from unittest import mock
 
 import responses
-from mediacatch_s2t import URL, PRESIGNED_ENDPOINT, TRANSCRIPT_ENDPOINT, UPDATE_STATUS_ENDPOINT
+from mediacatch_s2t import URL, SINGLE_UPLOAD_ENDPOINT, TRANSCRIPT_ENDPOINT, UPDATE_STATUS_ENDPOINT
 from mediacatch_s2t.uploader import upload_and_get_transcription, Uploader
 
 
 @mock.patch("pathlib.Path.is_file", return_value=True)
 def test_is_file_exist_mocked_return_true(mock_is_file):
     assert Uploader('fake file', 'fake key')._is_file_exist() is True
 
 
 @mock.patch("subprocess.run")
 def test_get_duration_mocked_return_value(mock_subprocess):
     mock_subprocess.return_value.returncode = 0
-    mock_subprocess.return_value.stdout = '{"streams": [{"codec_type": "audio", "duration": 1}]}'
+    mock_subprocess.return_value.stdout = '{"streams": [{"codec_type": "audio", "duration": "1"}]}'
     mock_subprocess.return_value.stderr = None
-    assert Uploader('fake file', 'fake key').get_duration() == (1000, {'codec_type': 'audio', 'duration': 1})
+    assert Uploader('fake file', 'fake key').get_duration() == (1000, {'codec_type': 'audio', 'duration': '1'})
+
+
+@mock.patch("subprocess.run")
+def test_get_duration_audio_not_available_mocked_return_value(mock_subprocess):
+    mock_subprocess.return_value.returncode = 0
+    mock_subprocess.return_value.stdout = '{"streams": [{"codec_type": "audio"}], "format": {"duration": "1"}}'
+    mock_subprocess.return_value.stderr = None
+    assert Uploader('fake file', 'fake key').get_duration() == (1000, {"duration": "1"})
 
 
 def test_estimated_result_time():
     assert Uploader('fake file', 'fake key').estimated_result_time(10000) == 1
 
 @responses.activate
 @mock.patch("builtins.open", new_callable=mock.mock_open,
@@ -37,15 +45,15 @@
     mock_Path.return_value.is_file.side_effect = side_effect
 
     mock_subprocess.return_value.returncode = 0
     mock_subprocess.return_value.stdout = '{"streams": [{"codec_type": "audio", "duration": 100}]}'
     mock_subprocess.return_value.stderr = None
 
     responses.add(
-        responses.POST, f'{URL}{PRESIGNED_ENDPOINT}', status=200,
+        responses.POST, f'{URL}{SINGLE_UPLOAD_ENDPOINT}', status=200,
         json={
             'url': URL_EXAMPLE,
             'fields': {'key': 'all fields we need'},
             'id': 'some-id'
         }
     )
     responses.add(
```

