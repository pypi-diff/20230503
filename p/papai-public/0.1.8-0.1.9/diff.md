# Comparing `tmp/papai_public-0.1.8.tar.gz` & `tmp/papai_public-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papai_public-0.1.8.tar", last modified: Wed Mar  8 16:08:35 2023, max compression
+gzip compressed data, was "dist/papai_public-0.1.9.tar", last modified: Thu Apr 27 08:56:33 2023, max compression
```

## Comparing `papai_public-0.1.8.tar` & `papai_public-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-08 16:08:35.778056 papai_public-0.1.8/
--rw-r--r--   0 user       (501) staff       (20)      160 2023-03-08 16:08:35.777871 papai_public-0.1.8/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)       38 2023-03-08 16:08:35.778122 papai_public-0.1.8/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      350 2023-03-08 16:07:35.000000 papai_public-0.1.8/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-08 16:08:35.776257 papai_public-0.1.8/src/
--rw-r--r--   0 user       (501) staff       (20)     3565 2022-11-04 15:37:12.000000 papai_public-0.1.8/src/object_storage_client.py
--rw-r--r--   0 user       (501) staff       (20)     2720 2023-03-08 16:07:35.000000 papai_public-0.1.8/src/papai_minio.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-03-08 16:08:35.777531 papai_public-0.1.8/src/papai_public.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      160 2023-03-08 16:08:35.000000 papai_public-0.1.8/src/papai_public.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      255 2023-03-08 16:08:35.000000 papai_public-0.1.8/src/papai_public.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-03-08 16:08:35.000000 papai_public-0.1.8/src/papai_public.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       61 2023-03-08 16:08:35.000000 papai_public-0.1.8/src/papai_public.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       34 2023-03-08 16:08:35.000000 papai_public-0.1.8/src/papai_public.egg-info/top_level.txt
+drwxr-xr-x   0 datategy   (502) staff       (20)        0 2023-04-27 08:56:33.389025 papai_public-0.1.9/
+-rw-r--r--   0 datategy   (502) staff       (20)      212 2023-04-27 08:56:33.388865 papai_public-0.1.9/PKG-INFO
+-rw-r--r--   0 datategy   (502) staff       (20)       38 2023-04-27 08:56:33.389084 papai_public-0.1.9/setup.cfg
+-rw-r--r--   0 datategy   (502) staff       (20)      359 2023-04-27 08:45:28.000000 papai_public-0.1.9/setup.py
+drwxr-xr-x   0 datategy   (502) staff       (20)        0 2023-04-27 08:56:33.388074 papai_public-0.1.9/src/
+-rw-r--r--   0 datategy   (502) staff       (20)     4070 2023-04-27 08:41:58.000000 papai_public-0.1.9/src/object_storage_client.py
+-rw-r--r--   0 datategy   (502) staff       (20)     2720 2023-03-08 16:01:34.000000 papai_public-0.1.9/src/papai_minio.py
+drwxr-xr-x   0 datategy   (502) staff       (20)        0 2023-04-27 08:56:33.388670 papai_public-0.1.9/src/papai_public.egg-info/
+-rw-r--r--   0 datategy   (502) staff       (20)      212 2023-04-27 08:56:33.000000 papai_public-0.1.9/src/papai_public.egg-info/PKG-INFO
+-rw-r--r--   0 datategy   (502) staff       (20)      255 2023-04-27 08:56:33.000000 papai_public-0.1.9/src/papai_public.egg-info/SOURCES.txt
+-rw-r--r--   0 datategy   (502) staff       (20)        1 2023-04-27 08:56:33.000000 papai_public-0.1.9/src/papai_public.egg-info/dependency_links.txt
+-rw-r--r--   0 datategy   (502) staff       (20)       67 2023-04-27 08:56:33.000000 papai_public-0.1.9/src/papai_public.egg-info/requires.txt
+-rw-r--r--   0 datategy   (502) staff       (20)       34 2023-04-27 08:56:33.000000 papai_public-0.1.9/src/papai_public.egg-info/top_level.txt
```

### Comparing `papai_public-0.1.8/src/object_storage_client.py` & `papai_public-0.1.9/src/object_storage_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,25 @@
                     "private_key_id": private_key_id,
                     "private_key": private_key,
                     "client_email": client_email,
                     "token_uri": "https://oauth2.googleapis.com/token",
                 }
                 credentials = service_account.Credentials.from_service_account_info(credentials_dict)
                 self.client = storage.Client(credentials=credentials)
+            elif self.client_type == "S3_OBJECT_STORAGE_SETTINGS":
+                endpoint = bucket_config["settings"]["endpoint"]
+                access_key = bucket_config["settings"]["access_key"]
+                secret_key = bucket_config["settings"]["secret_key"]
+
+                self.client = boto3.client(
+                    's3',
+                    aws_access_key_id=access_key,
+                    aws_secret_access_key=secret_key,
+                    endpoint_url=endpoint
+                )
             else:
                 logger.error(f"Object storage {bucket_config['settings']['kind']} not supported.")
         else:
             self.client_type = "MINIO"
             self.client = default_minio_client
 
     def read_from_bucket_to_file(self, bucket_name: str, object_name: str):
```

### Comparing `papai_public-0.1.8/src/papai_minio.py` & `papai_public-0.1.9/src/papai_minio.py`

 * *Files identical despite different names*

