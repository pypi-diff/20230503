# Comparing `tmp/krx_rigger-0.0.4.tar.gz` & `tmp/krx_rigger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_rigger-0.0.4.tar", last modified: Wed May  3 14:18:56 2023, max compression
+gzip compressed data, was "dist/krx_rigger-0.0.5.tar", last modified: Wed May  3 14:40:09 2023, max compression
```

## Comparing `krx_rigger-0.0.4.tar` & `krx_rigger-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.4/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/test/
--rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.4/test/test_list.py
--rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.4/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 14:18:55.000000 krx_rigger-0.0.4/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/setup.cfg
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx/
--rw-r--r--   0 nezah      (501) staff       (20)     6504 2023-05-03 14:18:55.000000 krx_rigger-0.0.4/krx/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx_rigger.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx_rigger.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx_rigger.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx_rigger.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx_rigger.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.5/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/test/
+-rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.5/test/test_list.py
+-rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.5/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:40:09.000000 krx_rigger-0.0.5/krx/
+-rw-r--r--   0 nezah      (501) staff       (20)     7216 2023-05-03 14:39:28.000000 krx_rigger-0.0.5/krx/__init__.py
```

### Comparing `krx_rigger-0.0.4/LICENSE` & `krx_rigger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_rigger-0.0.4/setup.py` & `krx_rigger-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krx_rigger",
-    version="0.0.4",
+    version="0.0.5",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="krx web crawler wrapper",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/krx_rigger",
     packages=setuptools.find_packages(),
```

### Comparing `krx_rigger-0.0.4/krx/__init__.py` & `krx_rigger-0.0.5/krx/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,40 +49,64 @@
             'scrnmode': '1',
         }
 
         response = self.session.get('https://kind.krx.co.kr/main.do', params=params)
         logger.info(response.status_code)
 
     def fetch_list(self, dt, time_sleep=0.3):
-        items = self._fetch_list(dt, page=1)
-        if items is not None:
-            logger.info(f"dt : {dt}, total : {items.get('total_count')}, page : {items.get('total_page')}")
-            result = items.get("items")
-
-            for p in range(2, items.get("total_page") + 1):
-                ## check cache
-                cache_key = f"krxweb_list_{dt}"
-                keys = [x.get("doc_id") for x in result]
-                diff = self.cache.differential(cache_key, keys)
-                logger.debug(f"diff : {diff}, cached keys : {len(self.cache.keys())}")
-                diff_ratio = float(len(diff)) / float(len(result)) * 100
-                if diff_ratio == float(0):
-                    logger.info(f"diff ratio is {diff_ratio}% => break")
-                    break
-                else:
-                    if diff_ratio < 80:
-                        logger.info(f"break")
+
+        results = []
+        page = 1
+        total_page = 1
+        page_no = 0
+
+        while page <= total_page:
+            items = self._fetch_list(dt, page=page)
+
+            if items is not None:
+                total_count = items.get('total_count')
+                total_page = items.get('total_page')
+                page_no = items.get('page')
+                page = page + 1
+
+                logger.info(f"dt : {dt}, total_count : {total_count}, total_page : {total_page}, current_page : {page_no}")
+
+                result = items.get("items")
+
+                if self.cache is not None:
+                    ## check cache
+                    cache_key = f"krxweb_list_{dt}"
+                    keys = [x.get("doc_id") for x in result]
+                    diff = self.cache.differential(cache_key, keys)
+                    logger.debug(f"diff : {diff}, cached keys : {len(self.cache.keys())}")
+                    diff_ratio = float(len(diff)) / float(len(result)) * 100
+                    if diff_ratio == float(0):
+                        logger.info(f"diff ratio is {diff_ratio}% => break")
+                        break
                     else:
-                        temp = self._fetch_list(dt, page=p)
-                        result.extend(temp.get("items"))
-                        time.sleep(time_sleep)
-                        logger.debug(f"page : {p}...")
-            return result
-        else:
-            logger.info("list empty")
+                        logger.info(f"diff ratio is {diff_ratio}%")
+                        results.extend([x for x in result if x.get("doc_id") in diff])
+                        self.cache.push_values(cache_key, keys)
+
+                        if diff_ratio < 80:
+                            logger.info(f"break")
+                            break
+                        else:
+                            logger.info(f"pause {time_sleep} sec...")
+                            time.sleep(time_sleep)
+                            continue
+                else:
+                    results.extend(result)
+
+                if total_page == page_no:
+                    logger.info(f"total page reached {total_page}")
+                    break
+
+        return results
+
 
     def _fetch_list(self, dt, page=1):
         headers = {
             'authority': 'kind.krx.co.kr',
             'accept': 'text/html, */*; q=0.01',
             'accept-language': 'en-US,en;q=0.9',
             'cache-control': 'no-cache',
```

