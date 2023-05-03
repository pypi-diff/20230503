# Comparing `tmp/osim_utils-0.3.0.tar.gz` & `tmp/osim_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.3.0.tar", max compression
+gzip compressed data, was "osim_utils-0.3.1.tar", max compression
```

## Comparing `osim_utils-0.3.0.tar` & `osim_utils-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.3.0/README.md
--rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.3.0/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     3034 2023-05-03 13:04:39.071296 osim_utils-0.3.0/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.3.0/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.3.0/osim_utils/constants.py
--rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.3.0/osim_utils/decorators.py
--rw-r--r--   0        0        0      665 2023-05-03 10:56:19.733679 osim_utils-0.3.0/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.3.0/osim_utils/logger.py
--rw-r--r--   0        0        0      408 2023-05-03 14:43:36.318178 osim_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 osim_utils-0.3.0/setup.py
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.3.1/README.md
+-rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.3.1/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     3186 2023-05-03 15:23:43.069814 osim_utils-0.3.1/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.3.1/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.3.1/osim_utils/constants.py
+-rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.3.1/osim_utils/decorators.py
+-rw-r--r--   0        0        0      665 2023-05-03 10:56:19.733679 osim_utils-0.3.1/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.3.1/osim_utils/logger.py
+-rw-r--r--   0        0        0      408 2023-05-03 15:23:43.070182 osim_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.3.1/PKG-INFO
```

### Comparing `osim_utils-0.3.0/osim_utils/clients/epmc.py` & `osim_utils-0.3.1/osim_utils/clients/epmc.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.3.0/osim_utils/clients/openalex.py` & `osim_utils-0.3.1/osim_utils/clients/openalex.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,24 @@
         quoted_dois = [urllib.parse.quote(x) for x in dois]
         sublists = chunk_list(quoted_dois, self.max_page_size)
         for sl in sublists:
             query = "|".join(sl)
             params = {"filter": f"doi:{query}", "per-page": self.max_page_size}
             yield self.get(self.works_endpoint, params=params, **kwargs)
 
-    def get_embl_works(self, filters: dict) -> dict:
+    def get_embl_works(self, filters: dict, **kwargs) -> dict:
         """
         Queries works associated with any of the EMBL ROR ids in ror_id2site
 
         Args:
             filters: additional filters to apply to query
                 (see https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/filter-entity-lists)
+            **kwargs: additional parameters to be passed to the OpenAlex API
 
         Returns:
 
         """
         filter_str = f"institutions.ror:{'|'.join(ror_id2site.keys())}"
         for k, v in filters.items():
             filter_str += f",{k}:{v}"
-        return self.get(self.works_endpoint, params={"filter": filter_str})
+        params = {"filter": filter_str} | kwargs.pop("params", dict())
+        return self.get(self.works_endpoint, params=params, **kwargs)
```

### Comparing `osim_utils-0.3.0/osim_utils/decorators.py` & `osim_utils-0.3.1/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.3.0/osim_utils/exceptions.py` & `osim_utils-0.3.1/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.3.0/osim_utils/logger.py` & `osim_utils-0.3.1/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.3.0/PKG-INFO` & `osim_utils-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

