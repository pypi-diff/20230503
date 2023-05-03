# Comparing `tmp/krx_rigger-0.0.3.tar.gz` & `tmp/krx_rigger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_rigger-0.0.3.tar", last modified: Wed May  3 13:59:59 2023, max compression
+gzip compressed data, was "dist/krx_rigger-0.0.4.tar", last modified: Wed May  3 14:18:56 2023, max compression
```

## Comparing `krx_rigger-0.0.3.tar` & `krx_rigger-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.3/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/test/
--rw-r--r--   0 nezah      (501) staff       (20)      385 2023-04-06 09:49:19.000000 krx_rigger-0.0.3/test/test_list.py
--rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.3/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 13:59:57.000000 krx_rigger-0.0.3/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/setup.cfg
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx/
--rw-r--r--   0 nezah      (501) staff       (20)     6460 2023-05-03 13:59:16.000000 krx_rigger-0.0.3/krx/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx_rigger.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.4/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/test/
+-rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.4/test/test_list.py
+-rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.4/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 14:18:55.000000 krx_rigger-0.0.4/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 14:18:56.000000 krx_rigger-0.0.4/krx/
+-rw-r--r--   0 nezah      (501) staff       (20)     6504 2023-05-03 14:18:55.000000 krx_rigger-0.0.4/krx/__init__.py
```

### Comparing `krx_rigger-0.0.3/LICENSE` & `krx_rigger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_rigger-0.0.3/setup.py` & `krx_rigger-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krx_rigger",
-    version="0.0.3",
+    version="0.0.4",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="krx web crawler wrapper",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/krx_rigger",
     packages=setuptools.find_packages(),
```

### Comparing `krx_rigger-0.0.3/krx/__init__.py` & `krx_rigger-0.0.4/krx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,17 @@
     def fetch_list(self, dt, time_sleep=0.3):
         items = self._fetch_list(dt, page=1)
         if items is not None:
             logger.info(f"dt : {dt}, total : {items.get('total_count')}, page : {items.get('total_page')}")
             result = items.get("items")
 
             for p in range(2, items.get("total_page") + 1):
-
                 ## check cache
                 cache_key = f"krxweb_list_{dt}"
-                keys = [x.get("") for x in result]
+                keys = [x.get("doc_id") for x in result]
                 diff = self.cache.differential(cache_key, keys)
                 logger.debug(f"diff : {diff}, cached keys : {len(self.cache.keys())}")
                 diff_ratio = float(len(diff)) / float(len(result)) * 100
                 if diff_ratio == float(0):
                     logger.info(f"diff ratio is {diff_ratio}% => break")
                     break
                 else:
@@ -128,15 +127,15 @@
         info_div = soup.select("div.info")
         if len(info_div) < 1:
             return None
         page_info = soup.select("div.info")[0].text.replace("\xa0", "").replace("\r", "").split("\n")
         current_page, total_page = map(lambda x: int(x), page_info[1].split(":")[1].strip().split("/"))
         total_count = soup.select("div.info")[0].select("em")[0].text
         trs = soup.find("table").select("tr")
-        items = [self._tr2dict(tr, dt) for tr in trs[1:]]
+        items = list(filter(lambda x: x is not None, [self._tr2dict(tr, dt) for tr in trs[1:]]))
         return {
             "page": current_page,
             "total_page": total_page,
             "total_count": total_count,
             "items": items
         }
```

