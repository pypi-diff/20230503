# Comparing `tmp/lesscode_tool-0.0.6.tar.gz` & `tmp/lesscode_tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tool-0.0.6.tar", last modified: Tue May  2 17:14:24 2023, max compression
+gzip compressed data, was "dist/lesscode_tool-0.0.7.tar", last modified: Wed May  3 02:18:08 2023, max compression
```

## Comparing `lesscode_tool-0.0.6.tar` & `lesscode_tool-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.6/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.6/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/entry_points.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/requires.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-02 17:14:23.000000 lesscode_tool-0.0.6/lesscode_tool.egg-info/top_level.txt
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/pkg/
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.6/pkg/__init__.py
--rwxr-xr-x   0 navy      (1000) navy      (1000)     1284 2023-05-02 16:39:02.000000 lesscode_tool-0.0.6/pkg/lesscode_tool.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/pkg/tool/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.6/pkg/tool/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)      816 2023-05-02 14:41:37.000000 lesscode_tool-0.0.6/pkg/tool/convert.py
--rw-r--r--   0 navy      (1000) navy      (1000)     6962 2023-05-02 17:01:35.000000 lesscode_tool-0.0.6/pkg/tool/new.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2178 2023-05-02 17:14:19.000000 lesscode_tool-0.0.6/pkg/tool/sqlacodegen.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-02 17:14:19.000000 lesscode_tool-0.0.6/pkg/version.py
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-02 17:14:24.000000 lesscode_tool-0.0.6/setup.cfg
--rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 16:52:06.000000 lesscode_tool-0.0.6/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/
+-rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.7/LICENSE
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.7/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/entry_points.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/requires.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/lesscode_tool.egg-info/top_level.txt
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/pkg/
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.7/pkg/__init__.py
+-rwxr-xr-x   0 navy      (1000) navy      (1000)     1284 2023-05-02 16:39:02.000000 lesscode_tool-0.0.7/pkg/lesscode_tool.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/pkg/tool/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.7/pkg/tool/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      815 2023-05-03 02:16:35.000000 lesscode_tool-0.0.7/pkg/tool/convert.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     6962 2023-05-02 17:01:35.000000 lesscode_tool-0.0.7/pkg/tool/new.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2339 2023-05-03 02:16:02.000000 lesscode_tool-0.0.7/pkg/tool/sqlacodegen.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-03 02:18:03.000000 lesscode_tool-0.0.7/pkg/version.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-03 02:18:08.000000 lesscode_tool-0.0.7/setup.cfg
+-rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 16:52:06.000000 lesscode_tool-0.0.7/setup.py
```

### Comparing `lesscode_tool-0.0.6/LICENSE` & `lesscode_tool-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.6/README.md` & `lesscode_tool-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.6/pkg/lesscode_tool.py` & `lesscode_tool-0.0.7/pkg/lesscode_tool.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.6/pkg/tool/convert.py` & `lesscode_tool-0.0.7/pkg/tool/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return s[0].lower() + s[1:]
 
 
 def retain_filed_quotation(key, origin):
     if isinstance(origin, str):
         origin = f"'{origin}'"
     elif key == "type":
-        origin = origin.__repr__()
+        origin = origin.__str__()
     return origin
 
 
 def field_type_handle(field_type):
     return field_type
```

### Comparing `lesscode_tool-0.0.6/pkg/tool/new.py` & `lesscode_tool-0.0.7/pkg/tool/new.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.6/pkg/tool/sqlacodegen.py` & `lesscode_tool-0.0.7/pkg/tool/sqlacodegen.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         t["columns"] = isp.get_columns(t.get("table"), schema=t.get("db"))
         table_class_str = f"""\n\nclass {to_upper_camel_case(t.get("table"))}(Base):\n    __tablename__ = '{t.get("table")}'\n\n"""
         for column in t["columns"]:
             field_type = column.get("type")
             if field_type:
                 field_module = field_type.__class__.__module__
                 field_class_name = field_type.__class__.__name__
+                if field_class_name == 'INTEGER' and isinstance(column.get("default"), str):
+                    column["default"] = eval(column.get("default"))
                 if field_module not in packages:
                     packages[field_module] = []
                 if field_class_name not in packages[field_module]:
                     packages[field_module].append(field_class_name)
             table_class_str += f"    {column.get('name')} = Column({dict2params_str(column)})\n"
         t["class_model"] = table_class_str
```

### Comparing `lesscode_tool-0.0.6/setup.py` & `lesscode_tool-0.0.7/setup.py`

 * *Files identical despite different names*

