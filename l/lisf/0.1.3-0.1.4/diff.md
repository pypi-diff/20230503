# Comparing `tmp/lisf-0.1.3.tar.gz` & `tmp/lisf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisf-0.1.3.tar", max compression
+gzip compressed data, was "lisf-0.1.4.tar", max compression
```

## Comparing `lisf-0.1.3.tar` & `lisf-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2662 2023-04-10 05:46:54.116518 lisf-0.1.3/lisf.py
--rw-r--r--   0        0        0      405 2023-04-10 05:51:43.589097 lisf-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 lisf-0.1.3/setup.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 lisf-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2692 2023-05-03 07:07:42.980251 lisf-0.1.4/lisf.py
+-rw-r--r--   0        0        0      405 2023-05-03 07:11:19.348401 lisf-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 lisf-0.1.4/setup.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 lisf-0.1.4/PKG-INFO
```

### Comparing `lisf-0.1.3/lisf.py` & `lisf-0.1.4/lisf.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def __delattr__(self, item):
         self.pop(item, None)
 
     def __dir__(self):
         return self._cache.keys()
 
     def __contains__(self, item):
-        return item in self._cache
+        return item in self._cache or item in self._lazy_loaders
 
     def register(self, key):
         def outer(func):
             return self.register_loader(key, func)
 
         if callable(key):
             func = key
```

