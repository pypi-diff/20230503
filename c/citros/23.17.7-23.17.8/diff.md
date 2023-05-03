# Comparing `tmp/citros-23.17.7.tar.gz` & `tmp/citros-23.17.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.17.7.tar", last modified: Thu Apr 27 14:22:56 2023, max compression
+gzip compressed data, was "citros-23.17.8.tar", last modified: Wed May  3 06:20:04 2023, max compression
```

## Comparing `citros-23.17.7.tar` & `citros-23.17.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 14:22:31.000000 citros-23.17.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:22:56.643752 citros-23.17.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 14:22:31.000000 citros-23.17.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.639752 citros-23.17.7/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-27 14:22:31.000000 citros-23.17.7/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.639752 citros-23.17.7/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 14:22:31.000000 citros-23.17.7/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 14:22:31.000000 citros-23.17.7/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 14:22:31.000000 citros-23.17.7/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 14:22:31.000000 citros-23.17.7/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 14:22:31.000000 citros-23.17.7/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 14:22:31.000000 citros-23.17.7/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 14:22:31.000000 citros-23.17.7/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 14:22:31.000000 citros-23.17.7/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:22:31.000000 citros-23.17.7/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 14:22:31.000000 citros-23.17.7/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 14:22:31.000000 citros-23.17.7/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 14:22:31.000000 citros-23.17.7/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 14:22:31.000000 citros-23.17.7/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 14:22:31.000000 citros-23.17.7/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.639752 citros-23.17.7/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:22:56.000000 citros-23.17.7/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 14:22:56.000000 citros-23.17.7/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:22:56.000000 citros-23.17.7/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 14:22:56.000000 citros-23.17.7/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:22:56.000000 citros-23.17.7/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 14:22:31.000000 citros-23.17.7/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:22:56.643752 citros-23.17.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 14:22:31.000000 citros-23.17.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:56.643752 citros-23.17.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:31.000000 citros-23.17.7/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:22:31.000000 citros-23.17.7/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.140258 citros-23.17.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 06:19:45.000000 citros-23.17.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 06:20:04.140258 citros-23.17.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 06:19:45.000000 citros-23.17.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.136258 citros-23.17.8/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-03 06:19:45.000000 citros-23.17.8/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.136258 citros-23.17.8/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 06:19:45.000000 citros-23.17.8/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 06:19:45.000000 citros-23.17.8/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.136258 citros-23.17.8/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 06:19:45.000000 citros-23.17.8/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-03 06:19:45.000000 citros-23.17.8/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.140258 citros-23.17.8/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 06:19:45.000000 citros-23.17.8/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-03 06:19:45.000000 citros-23.17.8/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 06:19:45.000000 citros-23.17.8/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.140258 citros-23.17.8/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 06:19:45.000000 citros-23.17.8/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 06:19:45.000000 citros-23.17.8/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-03 06:19:45.000000 citros-23.17.8/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.140258 citros-23.17.8/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-03 06:19:45.000000 citros-23.17.8/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 06:19:45.000000 citros-23.17.8/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-03 06:19:45.000000 citros-23.17.8/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 06:19:45.000000 citros-23.17.8/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.136258 citros-23.17.8/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 06:20:04.000000 citros-23.17.8/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 06:20:04.000000 citros-23.17.8/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:20:04.000000 citros-23.17.8/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 06:20:04.000000 citros-23.17.8/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 06:20:04.000000 citros-23.17.8/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 06:19:45.000000 citros-23.17.8/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:20:04.140258 citros-23.17.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 06:19:45.000000 citros-23.17.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:20:04.140258 citros-23.17.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:19:45.000000 citros-23.17.8/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:19:45.000000 citros-23.17.8/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.17.7/LICENSE` & `citros-23.17.8/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/PKG-INFO` & `citros-23.17.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.7
+Version: 23.17.8
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.7/README.md` & `citros-23.17.8/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/bin/citros` & `citros-23.17.8/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/__init__.py` & `citros-23.17.8/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/citros.py` & `citros-23.17.8/citros/citros.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
                     role{
                         id
                         role
                     }           
                     organization{
                         id 
                         name
+                        domain_prefix
                     }                    
                 }
             }  
             """
         try:
             result = self.gql_execute(query)            
             self._user = result["currentUser"]
```

### Comparing `citros-23.17.7/citros/citros_bag.py` & `citros-23.17.8/citros/citros_bag.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,19 +210,22 @@
     def sync_bag_google_bucket(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):
         self.log.debug("------------------------------------------------------------------------------------")
         self.log.debug("uploading bag to google bucket")
         if not self.citros.isAuthenticated():
             self.log.debug("not authenticated. please login first.")
             return False, "not authenticated. please login first." , None       
         
+        user = self.citros.getUser()
+        tenant =  user["organization"]["domain_prefix"]
+        
         bag_file_name = path_to_bag.split('/')[-1]            
-        data_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={batch_run_id + "/sid-" + simulation_run_id + "/" + bag_file_name}'        
+        data_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + bag_file_name}'        
         
         metadata_name = path_to_metadata.split('/')[-1]  
-        metadata_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={batch_run_id + "/sid-" + simulation_run_id + "/" + metadata_name}'        
+        metadata_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + metadata_name}'        
 
         google_token = self.get_bag_access_token()
         # self.log.debug("google_token", google_token)
         if google_token is None:
             error_text = f"[ERROR] at sync_bag, failed to get google token from CITROS."
             self.log.error(error_text)                                  
             return False, error_text, None
```

### Comparing `citros-23.17.7/citros/citros_batch.py` & `citros-23.17.8/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/citros_events.py` & `citros-23.17.8/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/citros_integration.py` & `citros-23.17.8/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/citros_params.py` & `citros-23.17.8/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/citros_utils.py` & `citros-23.17.8/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/launches/__init__.py` & `citros-23.17.8/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/launches/launch.py` & `citros-23.17.8/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/logger/__init__.py` & `citros-23.17.8/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/logger/logger.py` & `citros-23.17.8/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/logger/logger_pg_handler.py` & `citros-23.17.8/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/parsers/__init__.py` & `citros-23.17.8/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/parsers/parser_ros2.py` & `citros-23.17.8/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/rosbag/__init__.py` & `citros-23.17.8/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/rosbag/reader_base.py` & `citros-23.17.8/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/rosbag/reader_mcap.py` & `citros-23.17.8/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros/rosbag/reader_sqlite.py` & `citros-23.17.8/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/citros.egg-info/PKG-INFO` & `citros-23.17.8/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.7
+Version: 23.17.8
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.7/citros.egg-info/SOURCES.txt` & `citros-23.17.8/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.17.7/setup.py` & `citros-23.17.8/setup.py`

 * *Files identical despite different names*

