# Comparing `tmp/py_seasnake-0.3.0.tar.gz` & `tmp/py_seasnake-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_seasnake-0.3.0.tar", max compression
+gzip compressed data, was "py_seasnake-0.3.1.tar", max compression
```

## Comparing `py_seasnake-0.3.0.tar` & `py_seasnake-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-29 21:40:45.713848 py_seasnake-0.3.0/LICENSE
--rw-r--r--   0        0        0      745 2023-04-29 21:40:45.713848 py_seasnake-0.3.0/README.md
--rw-r--r--   0        0        0     1311 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/__init__.py
--rw-r--r--   0        0        0     3840 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/auth.py
--rw-r--r--   0        0        0     9230 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/base.py
--rw-r--r--   0        0        0     1445 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/io.py
--rw-r--r--   0        0        0     2775 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/projects.py
--rw-r--r--   0        0        0      386 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/__init__.py
--rw-r--r--   0        0        0     3114 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/base.py
--rw-r--r--   0        0        0     2853 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_lit.py
--rw-r--r--   0        0        0     2979 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_photo_quadrat.py
--rw-r--r--   0        0        0     2854 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_pit.py
--rw-r--r--   0        0        0     3741 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/bleaching.py
--rw-r--r--   0        0        0     2654 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/fish_belt.py
--rw-r--r--   0        0        0     2957 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/habitat_complexity.py
--rw-r--r--   0        0        0     2356 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/sample_event.py
--rw-r--r--   0        0        0      606 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/timer.py
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 py_seasnake-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-03 04:25:11.883497 py_seasnake-0.3.1/LICENSE
+-rw-r--r--   0        0        0      745 2023-05-03 04:25:11.883497 py_seasnake-0.3.1/README.md
+-rw-r--r--   0        0        0     1311 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/__init__.py
+-rw-r--r--   0        0        0     4062 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/auth.py
+-rw-r--r--   0        0        0     9230 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/base.py
+-rw-r--r--   0        0        0     1445 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/io.py
+-rw-r--r--   0        0        0     2775 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/projects.py
+-rw-r--r--   0        0        0      386 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/__init__.py
+-rw-r--r--   0        0        0     3114 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/base.py
+-rw-r--r--   0        0        0     2853 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_lit.py
+-rw-r--r--   0        0        0     2979 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_photo_quadrat.py
+-rw-r--r--   0        0        0     2854 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_pit.py
+-rw-r--r--   0        0        0     3741 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/bleaching.py
+-rw-r--r--   0        0        0     2654 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/fish_belt.py
+-rw-r--r--   0        0        0     2957 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/habitat_complexity.py
+-rw-r--r--   0        0        0     2356 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/sample_event.py
+-rw-r--r--   0        0        0      606 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/timer.py
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 py_seasnake-0.3.1/PKG-INFO
```

### Comparing `py_seasnake-0.3.0/LICENSE` & `py_seasnake-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/README.md` & `py_seasnake-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/pyproject.toml` & `py_seasnake-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "py-seasnake"
 packages = [
     { include = "seasnake" },
 ]
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease."
 authors = ["Dustin Sampson <gridcell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gridcell.github.io/py-seasnake/"
 repository = "https://github.com/gridcell/py-seasnake"
 documentation = "https://gridcell.github.io/py-seasnake/"
```

### Comparing `py_seasnake-0.3.0/seasnake/auth.py` & `py_seasnake-0.3.1/seasnake/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,23 @@
     def _load_token(self) -> Optional[str]:
         try:
             with open(self.auth_file, "r") as f:
                 return f.read()
         except Exception:
             return None
 
-    def get_token(self) -> Optional[str]:
+    def get_token(self, store: bool=False) -> Optional[str]:
+        """
+
+        Args:
+            store (bool, optional): Store token to disk. Defaults to False.
+
+        Returns:
+            Optional[str]: Access token
+        """
         client_id = CLIENT_ID
         domain = AUTH0_DOMAIN
         audience = AUDIENCE
 
         token = self._load_token()
         if self._token_expired(token) is False:
             return token
@@ -95,15 +103,16 @@
                 },
             )
 
             # If the request is successful, extract the access token and break out of the loop
             if response.status_code == 200:
                 json_response = response.json()
                 access_token = json_response["access_token"]
-                self._write_token(access_token)
+                if store:
+                    self._write_token(access_token)
                 return access_token
 
             # If the timeout is reached, exit the loop and inform the user
             elapsed_time = time.time() - start_time
             if elapsed_time > timeout:
                 print("Timeout reached. Please try again.")
                 break
```

### Comparing `py_seasnake-0.3.0/seasnake/base.py` & `py_seasnake-0.3.1/seasnake/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/io.py` & `py_seasnake-0.3.1/seasnake/io.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/projects.py` & `py_seasnake-0.3.1/seasnake/projects.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/base.py` & `py_seasnake-0.3.1/seasnake/summaries/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/benthic_lit.py` & `py_seasnake-0.3.1/seasnake/summaries/benthic_lit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/benthic_photo_quadrat.py` & `py_seasnake-0.3.1/seasnake/summaries/benthic_photo_quadrat.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/benthic_pit.py` & `py_seasnake-0.3.1/seasnake/summaries/benthic_pit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/bleaching.py` & `py_seasnake-0.3.1/seasnake/summaries/bleaching.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/fish_belt.py` & `py_seasnake-0.3.1/seasnake/summaries/fish_belt.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/habitat_complexity.py` & `py_seasnake-0.3.1/seasnake/summaries/habitat_complexity.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/summaries/sample_event.py` & `py_seasnake-0.3.1/seasnake/summaries/sample_event.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/seasnake/timer.py` & `py_seasnake-0.3.1/seasnake/timer.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.0/PKG-INFO` & `py_seasnake-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-seasnake
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease.
 Home-page: https://gridcell.github.io/py-seasnake/
 License: MIT
 Keywords: MERMAID,coral,fish,API
 Author: Dustin Sampson
 Author-email: gridcell@gmail.com
 Requires-Python: >=3.8,<3.12
```

