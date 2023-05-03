# Comparing `tmp/pyghs-0.1.1.tar.gz` & `tmp/pyghs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghs-0.1.1.tar", last modified: Sun Apr 30 04:07:09 2023, max compression
+gzip compressed data, was "pyghs-0.2.0.tar", last modified: Wed May  3 11:50:33 2023, max compression
```

## Comparing `pyghs-0.1.1.tar` & `pyghs-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994519 pyghs-0.1.1/
--rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-30 04:07:09.994391 pyghs-0.1.1/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      564 2023-04-29 07:30:53.000000 pyghs-0.1.1/README.md
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.993350 pyghs-0.1.1/ghs/
--rw-r--r--   0 chaoying   (501) staff       (20)       46 2023-04-29 07:13:49.000000 pyghs-0.1.1/ghs/__init__.py
--rw-r--r--   0 chaoying   (501) staff       (20)     4055 2023-04-30 04:06:28.000000 pyghs-0.1.1/ghs/storage.py
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994040 pyghs-0.1.1/pyghs.egg-info/
--rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      221 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/SOURCES.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/dependency_links.txt
--rw-r--r--   0 chaoying   (501) staff       (20)       29 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/requires.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/top_level.txt
--rw-r--r--   0 chaoying   (501) staff       (20)      501 2023-04-30 04:00:33.000000 pyghs-0.1.1/pyproject.toml
--rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-04-30 04:07:09.994557 pyghs-0.1.1/setup.cfg
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994154 pyghs-0.1.1/tests/
--rw-r--r--   0 chaoying   (501) staff       (20)      830 2023-04-30 03:59:02.000000 pyghs-0.1.1/tests/test_storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-03 11:50:33.873633 pyghs-0.2.0/
+-rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-05-03 11:50:33.873512 pyghs-0.2.0/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      497 2023-05-03 11:47:43.000000 pyghs-0.2.0/README.md
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-03 11:50:33.872574 pyghs-0.2.0/ghs/
+-rw-r--r--   0 chaoying   (501) staff       (20)       94 2023-05-03 11:18:07.000000 pyghs-0.2.0/ghs/__init__.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     4385 2023-05-03 11:50:18.000000 pyghs-0.2.0/ghs/async_storage.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     1510 2023-05-03 11:50:17.000000 pyghs-0.2.0/ghs/config.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     4030 2023-05-03 11:50:18.000000 pyghs-0.2.0/ghs/storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-03 11:50:33.873153 pyghs-0.2.0/pyghs.egg-info/
+-rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-05-03 11:50:33.000000 pyghs-0.2.0/pyghs.egg-info/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      284 2023-05-03 11:50:33.000000 pyghs-0.2.0/pyghs.egg-info/SOURCES.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-05-03 11:50:33.000000 pyghs-0.2.0/pyghs.egg-info/dependency_links.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)       63 2023-05-03 11:50:33.000000 pyghs-0.2.0/pyghs.egg-info/requires.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-05-03 11:50:33.000000 pyghs-0.2.0/pyghs.egg-info/top_level.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)      549 2023-05-03 11:46:10.000000 pyghs-0.2.0/pyproject.toml
+-rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-05-03 11:50:33.873665 pyghs-0.2.0/setup.cfg
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-03 11:50:33.873378 pyghs-0.2.0/tests/
+-rw-r--r--   0 chaoying   (501) staff       (20)      691 2023-05-03 11:37:33.000000 pyghs-0.2.0/tests/test_async_storage.py
+-rw-r--r--   0 chaoying   (501) staff       (20)      587 2023-05-03 11:49:01.000000 pyghs-0.2.0/tests/test_storage.py
```

### Comparing `pyghs-0.1.1/ghs/storage.py` & `pyghs-0.2.0/ghs/async_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import base64
 import io
 import json
 
 import aiohttp
 import pandas as pd
 
+from ghs.config import settings
 
-class GHS:
+
+class AsyncGHS:
     def __init__(
         self,
-        access_token: str,
         repository: str,
+        access_token: str | None = None,
     ) -> None:
         self.repository = repository
-        self._session = self._get_session(access_token)
+        if access_token is None and not settings.access_token:
+            raise ValueError("access_token is required")
+        self._session = self._get_session(access_token or settings.access_token)
 
     async def create(self, path: str, df: pd.DataFrame) -> None:
         payload = {
             "message": "Create",
-            "content": base64.b64encode(df.to_csv().encode()).decode(),
+            "content": base64.b64encode(
+                df.reset_index(drop=True).to_csv(index=False).encode()
+            ).decode(),
         }
         async with self._session.put(
             f"/repos/{self.repository}/contents/{path}", data=json.dumps(payload)
         ) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError as e:
@@ -46,15 +52,17 @@
             if upsert:
                 await self.create(path, df)
                 return
             raise
         payload = {
             "message": "Update",
             "sha": sha,
-            "content": base64.b64encode(df.to_csv().encode()).decode(),
+            "content": base64.b64encode(
+                df.reset_index(drop=True).to_csv(index=False).encode()
+            ).decode(),
         }
         async with self._session.put(
             f"/repos/{self.repository}/contents/{path}", data=json.dumps(payload)
         ) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError as e:
@@ -107,12 +115,12 @@
             },
             base_url="https://api.github.com",
         )
 
     async def close(self) -> None:
         await self._session.close()
 
-    async def __aenter__(self) -> "GHS":
+    async def __aenter__(self) -> "AsyncGHS":
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:
         await self.close()
```

