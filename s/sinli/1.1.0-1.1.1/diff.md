# Comparing `tmp/sinli-1.1.0.tar.gz` & `tmp/sinli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.0.tar", last modified: Thu Apr 13 12:48:20 2023, max compression
+gzip compressed data, was "sinli-1.1.1.tar", last modified: Wed May  3 16:33:01 2023, max compression
```

## Comparing `sinli-1.1.0.tar` & `sinli-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.497824 sinli-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2023-04-13 12:46:25.000000 sinli-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44158 2023-04-13 12:48:20.497824 sinli-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3934 2023-04-13 12:46:25.000000 sinli-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-13 12:46:25.000000 sinli-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:48:20.497824 sinli-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-13 12:46:25.000000 sinli-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4967 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.497824 sinli-1.1.0/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.497824 sinli-1.1.0/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7220 2023-04-13 12:46:25.000000 sinli-1.1.0/src/sinli/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.493824 sinli-1.1.0/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44158 2023-04-13 12:48:20.000000 sinli-1.1.0/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-13 12:48:20.000000 sinli-1.1.0/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:48:20.000000 sinli-1.1.0/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-13 12:48:20.000000 sinli-1.1.0/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-13 12:48:20.000000 sinli-1.1.0/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:48:20.497824 sinli-1.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-13 12:46:25.000000 sinli-1.1.0/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2023-05-03 16:31:54.000000 sinli-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    44158 2023-05-03 16:33:01.105139 sinli-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3934 2023-05-03 16:31:54.000000 sinli-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-03 16:31:54.000000 sinli-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 16:33:01.105139 sinli-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-03 16:31:54.000000 sinli-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.097139 sinli-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4967 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     7220 2023-05-03 16:31:54.000000 sinli-1.1.1/src/sinli/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.101139 sinli-1.1.1/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44158 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      753 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 16:33:01.000000 sinli-1.1.1/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:33:01.105139 sinli-1.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 16:31:54.000000 sinli-1.1.1/tests/test_document.py
```

### Comparing `sinli-1.1.0/LICENSE` & `sinli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/PKG-INFO` & `sinli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.0/README.md` & `sinli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/pyproject.toml` & `sinli-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.1.0"
+version = "1.1.1"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.1.0/src/sinli/common/encoded_values.py` & `sinli-1.1.1/src/sinli/common/encoded_values.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/__init__.py` & `sinli-1.1.1/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/envio/v8.py` & `sinli-1.1.1/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/factul/v1.py` & `sinli-1.1.1/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/libros/v8.py` & `sinli-1.1.1/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/libros/v9.py` & `sinli-1.1.1/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/mensaj/v1.py` & `sinli-1.1.1/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/doctype/pedido/v7.py` & `sinli-1.1.1/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli/document.py` & `sinli-1.1.1/src/sinli/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 
     def __post_init__(self):
         self.long_id_line.TYPE = "I"
         self.long_id_line.FANDE = "FANDE"
         self.short_id_line.TYPE = "I"
 
     def consume_line(line: str, doc: Self) -> Self:
-        print(f"[DEBUG] line: {line}")
+        print(f"\n[DEBUG] line: '{line}'")
 
         tdoc = line[0:1]
-        if tdoc == "I" and not doc.long_id_line: # generic processing, we still don't know:  # Subject
+        if tdoc == "I" and not doc.long_id_line.FROM: # generic processing, we still don't know the doctype:  # Long id
             doc.long_id_line = LongIdentificationLine.from_str(line)
             return doc
 
-        elif tdoc == "I" and not doc.short_id_line: # generic processing, we still don't know:  # Identification
+        elif tdoc == "I" and not doc.short_id_line.FROM: # generic processing, we still don't know the doctype:  # Short id
             doc.short_id_line = ShortIdentificationLine.from_str(line)
             version_str = doc.short_id_line.VERSION if hasattr(doc, "short_id_line") else "" # ex: "09"
             doctype_str = doc.short_id_line.DOCTYPE if hasattr(doc, "short_id_line") else ""
 
-            if doctype_str: # we just processed the identification line
+            if doctype_str: # we just processed the short identification line
                 from .doctype import DocumentType
                 doctype_tup = DocumentType[doctype_str]
                 doctype_class = doctype_tup.value[1].get(version_str)
                 if doctype_class == None:
                     doctype_class = doctype_tup.value[1].get("??")
                     print(f"[WARN] using class {doctype_class} to parse document at version {version_str}. Some fields may be missing or become mixed")
                 newdoc = doctype_class.from_document(doc)
```

### Comparing `sinli-1.1.0/src/sinli/line.py` & `sinli-1.1.1/src/sinli/line.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.0/src/sinli.egg-info/PKG-INFO` & `sinli-1.1.1/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.0/src/sinli.egg-info/SOURCES.txt` & `sinli-1.1.1/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

