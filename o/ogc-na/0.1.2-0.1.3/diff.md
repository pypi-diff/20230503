# Comparing `tmp/ogc_na-0.1.2.tar.gz` & `tmp/ogc_na-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.2.tar", last modified: Fri Apr 28 08:49:57 2023, max compression
+gzip compressed data, was "ogc_na-0.1.3.tar", last modified: Wed May  3 10:14:54 2023, max compression
```

## Comparing `ogc_na-0.1.2.tar` & `ogc_na-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.156715 ogc_na-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.144714 ogc_na-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 08:49:43.000000 ogc_na-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-28 08:49:43.000000 ogc_na-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 08:49:43.000000 ogc_na-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-28 08:49:57.156715 ogc_na-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-28 08:49:43.000000 ogc_na-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-28 08:49:43.000000 ogc_na-0.1.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-28 08:49:43.000000 ogc_na-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 08:49:43.000000 ogc_na-0.1.2/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-28 08:49:43.000000 ogc_na-0.1.2/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 08:49:43.000000 ogc_na-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:49:57.156715 ogc_na-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 08:49:43.000000 ogc_na-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.156715 ogc_na-0.1.2/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 10:14:41.000000 ogc_na-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-03 10:14:41.000000 ogc_na-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 10:14:41.000000 ogc_na-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 10:14:54.271020 ogc_na-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 10:14:41.000000 ogc_na-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-03 10:14:41.000000 ogc_na-0.1.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 10:14:41.000000 ogc_na-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-03 10:14:41.000000 ogc_na-0.1.3/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-03 10:14:41.000000 ogc_na-0.1.3/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 10:14:41.000000 ogc_na-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:14:54.271020 ogc_na-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 10:14:41.000000 ogc_na-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_profile.py
```

### Comparing `ogc_na-0.1.2/.github/workflows/python-publish.yml` & `ogc_na-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/.gitignore` & `ogc_na-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/PKG-INFO` & `ogc_na-0.1.3/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ogc_na
-Version: 0.1.2
+Name: ogc-na
+Version: 0.1.3
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.2/README.md` & `ogc_na-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/docs/examples.md` & `ogc_na-0.1.3/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/docs/gen_ref_pages.py` & `ogc_na-0.1.3/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/docs/index.md` & `ogc_na-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/docs/tutorials.md` & `ogc_na-0.1.3/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/mkdocs.yml` & `ogc_na-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/annotate_schema.py` & `ogc_na-0.1.3/ogc/na/annotate_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -112,37 +112,40 @@
 The resulting context will be printed to the standard output.
 
 """
 
 from __future__ import annotations
 import argparse
 import dataclasses
-import functools
 import json
 import logging
+import re
 import sys
 from pathlib import Path
-from typing import Any, AnyStr
+from typing import Any, AnyStr, Callable
 from urllib.parse import urlparse, urljoin
 import yaml
 import requests
-from ogc.na.util import is_url, merge_dicts, load_yaml
+from ogc.na.util import is_url, merge_dicts, load_yaml, LRUCache
 
 try:
     from yaml import CLoader as YamlLoader, CDumper as YamlDumper
 except ImportError:
     from yaml import Loader as YamlLoader, Dumper as YamlDumper
 
 logger = logging.getLogger(__name__)
 
 ANNOTATION_CONTEXT = 'x-jsonld-context'
 ANNOTATION_ID = 'x-jsonld-id'
 ANNOTATION_TYPE = 'x-jsonld-type'
+ANNOTATION_PREFIXES = 'x-jsonld-prefixes'
 REF_ROOT_MARKER = '$_ROOT_/'
 
+context_term_cache = LRUCache(maxsize=20)
+
 
 @dataclasses.dataclass
 class AnnotatedSchema:
     source: str | Path
     is_json: bool
     schema: dict
 
@@ -214,127 +217,173 @@
         return None, urljoin(base_url, ref)
     else:
         fn_from = fn_from if isinstance(fn_from, Path) else Path(fn_from)
         ref = (fn_from.resolve().parent / ref).resolve()
         return ref, None
 
 
-@functools.lru_cache(maxsize=20)
-def read_context_terms(file: Path | str = None, url: str = None) -> dict[str, str]:
+def read_context_terms(ctx: Path | str | dict) -> tuple[dict[str, str], dict[str, str], dict[str, str]]:
     """
     Reads all the terms from a JSON-LD context document.
 
-    :param file: file path to load
-    :param url: URL to load
+    :param ctx: file path (Path), URL (str) or dictionary (dict) to load
     :return: a dictionary with term -> URI mappings
     """
+
+    cached = context_term_cache.get(ctx)
+    if cached:
+        return cached
+
     context: dict[str, Any] | None = None
 
-    if file:
-        with open(file) as f:
+    if isinstance(ctx, Path):
+        with open(ctx) as f:
             context = json.load(f).get('@context')
-    elif url:
-        r = requests.get(url)
+    elif isinstance(ctx, str):
+        r = requests.get(ctx)
         r.raise_for_status()
         context = r.json().get('@context')
+    elif ctx:
+        context = ctx.get('@context')
 
     if not context:
-        return {}
+        return {}, {}, {}
 
-    result: dict[str, str] = {}
-    pending: dict[str, list] = {}
+    result: dict[str, str | tuple[str, str]] = {}
+    types: dict[str, str | tuple[str, str]] = {}
 
     vocab = context.get('@vocab')
 
+    def expand_uri(uri: str) -> str | tuple[str, str] | None:
+        if not uri:
+            return None
+
+        if ':' in uri:
+            # either URI or prefix:suffix
+            pref, suf = uri.split(':', 1)
+            if suf.startswith('//') or pref == 'urn':
+                # assume full URI
+                return uri
+            else:
+                # prefix:suffix -> add to pending for expansion
+                return pref, suf
+        elif vocab:
+            # append term_val to vocab to get URI
+            return f"{vocab}{term_id}"
+        else:
+            return uri
+
     for term, term_val in context.items():
         if not term.startswith("@"):
             # assume term
+            term_type = None
             if isinstance(term_val, str):
                 term_id = term_val
             elif isinstance(term_val, dict):
                 term_id = term_val.get('@id')
+                term_type = term_val.get('@type')
             else:
                 term_id = None
 
-            if term_id:
-                if ':' in term_id:
-                    # either URI or prefix:suffix
-                    pref, suf = term_id.split(':', 1)
-                    if suf.startswith('//'):
-                        # assume URI -> add to result
-                        result[term] = term_id
-                    else:
-                        # prefix:suffix -> add to pending for expansion
-                        pending[term] = [pref, suf]
-                elif vocab:
-                    # append term_val to vocab to get URI
-                    result[term] = f"{vocab}{term_id}"
-
-    for term, term_val in pending.items():
-        pref, suf = term_val
-        if pref in result:
-            result[term] = f"{result[pref]}{suf}"
+            expanded_id = expand_uri(term_id)
+            if expanded_id:
+                result[term] = expanded_id
+            expanded_type = expand_uri(term_type)
+            if expanded_type:
+                types[term] = expanded_type
+
+    prefixes = {}
+
+    def expand_result(d: dict[str, str | tuple[str, str]]) -> dict[str, str]:
+        r = {}
+        for term, term_val in d.items():
+            if isinstance(term_val, str):
+                r[term] = term_val
+            else:
+                pref, suf = term_val
+                if pref in result:
+                    r[term] = f"{result[pref]}{suf}"
+                    prefixes[pref] = result[pref]
+        return r
+
+    expanded_types = expand_result(types)
+    expanded_terms = expand_result(result)
 
-    return result
+    context_term_cache[ctx] = expanded_terms, prefixes, expanded_types
+    return expanded_terms, prefixes, expanded_types
 
 
 class SchemaAnnotator:
     """
     Builds a set of annotated JSON schemas from a collection of input schemas
     that have `x-jsonld-context`s to JSON-LD context documents.
 
     The results will be stored in the `schemas` property (a dictionary of
     schema-path-or-url -> AnnotatedSchema mappings).
     """
 
     def __init__(self, fn: Path | str | None = None, url: str | None = None,
-                 follow_refs: bool = True, ref_root: Path | str | None = None):
+                 follow_refs: bool = True, ref_root: Path | str | None = None,
+                 context: str | Path | dict | None = None):
         """
         :param fn: file path to load (root schema)
         :param url: URL to load (root schema)
         :follow_refs: whether to follow `$ref`s (otherwise just annotate the provided root schema)
         """
         self.schemas: dict[str | Path, AnnotatedSchema] = {}
         self.bundled_schema = None
         self.ref_root = Path(ref_root) if ref_root else None
         self._follow_refs = follow_refs
+        self._provided_context = context
 
         self._process_schema(fn, url)
 
     def _process_schema(self, fn: Path | str | None = None, url: str | None = None):
         contents, base_url = read_contents(fn, url)
         schema, is_json = load_json_yaml(contents)
 
         context_fn = schema.get(ANNOTATION_CONTEXT)
         schema.pop(ANNOTATION_CONTEXT, None)
 
         base_url = schema.get('$id', base_url)
 
-        if not context_fn:
-            terms = {}
-        elif base_url:
-            context_fn = urljoin(base_url, context_fn)
-            terms = read_context_terms(url=context_fn)
-        else:
-            context_fn = Path(fn).parent / context_fn
-            terms = read_context_terms(file=context_fn)
+        terms = {}
+        prefixes = {}
+        types = {}
+
+        if context_fn != self._provided_context or not (isinstance(context_fn, Path)
+                                                        and isinstance(self._provided_context, Path)
+                                                        and self._provided_context.resolve() == context_fn.resolve()):
+            # Only load the provided context if it's different from the schema-referenced one
+            terms, prefixes, types = read_context_terms(self._provided_context)
+
+        if context_fn:
+            if base_url:
+                context_fn = urljoin(base_url, str(context_fn))
+            else:
+                context_fn = Path(fn).parent / context_fn
+
+            for e in zip((terms, prefixes, types), read_context_terms(context_fn)):
+                e[0].update(e[1])
 
         def process_properties(obj: dict):
             properties: dict[str, dict] = obj.get('properties') if obj else None
-            if not properties:
-                return
+            if not isinstance(properties, dict):
+                raise ValueError('"properties" must be a dictionary')
 
             empty_properties = []
             for prop, prop_value in properties.items():
                 if not prop_value:
                     empty_properties.append(prop)
                     continue
                 if prop in terms:
                     prop_value[ANNOTATION_ID] = terms[prop]
-                if '$ref' in prop_value:
+                    if prop in types:
+                        prop_value[ANNOTATION_TYPE] = types[prop]
+                if '$ref' in prop_value and self._follow_refs:
 
                     ref_fn, ref_url = resolve_ref(prop_value['$ref'], fn, url, base_url)
                     ref = ref_fn or ref_url
 
                     if ref in self.schemas:
                         logger.info(' >> Found $ref to already-processed schema: %s', ref)
                     else:
@@ -342,21 +391,36 @@
                         if ref_url:
                             self._process_schema(url=ref)
                         else:
                             self._process_schema(fn=ref)
 
             properties.update({p: {ANNOTATION_ID: terms[p]} for p in empty_properties if p in terms})
 
-        schema_type = schema.get('type')
+        def process_subschema(subschema):
 
-        if schema_type == 'object':
-            process_properties(schema)
-        elif schema_type == 'array':
-            for k in ('prefixItems', 'items', 'contains'):
-                process_properties(schema.get(k))
+            schema_type = subschema.get('type')
+            if not schema_type and 'properties' in subschema:
+                schema_type = 'object'
+
+            if schema_type == 'object':
+                process_properties(subschema)
+            elif schema_type == 'array':
+                for k in ('prefixItems', 'items', 'contains'):
+                    process_properties(subschema.get(k))
+
+            for defs_prop in ('$defs', 'definitions'):
+                defs_value = subschema.get(defs_prop)
+                if isinstance(defs_value, dict):
+                    for defs_entry in defs_value.values():
+                        process_subschema(defs_entry)
+
+        process_subschema(schema)
+
+        if prefixes:
+            schema[ANNOTATION_PREFIXES] = prefixes
 
         self.schemas[fn or url] = AnnotatedSchema(
             source=fn or url,
             is_json=is_json,
             schema=schema
         )
 
@@ -385,26 +449,51 @@
             return parsed
 
         contents, base_url = read_contents(fn, url)
         schema = load_json_yaml(contents)[0]
 
         base_url = schema.get('$id', base_url)
 
+        prefixes = schema.get(ANNOTATION_PREFIXES, {}).items()
+        rev_prefixes = {v: k for k, v in prefixes}
+
+        def compact_uri(uri: str) -> str:
+            if uri.startswith('@'):
+                # JSON-LD keyword
+                return uri
+            parts = urlparse(uri)
+            if parts.fragment:
+                pref, suf = uri.rsplit('#', 1)
+                pref += '#'
+            elif len(parts.path) > 1:
+                pref, suf = uri.rsplit('/', 1)
+                pref += '/'
+            else:
+                return uri
+
+            if pref in rev_prefixes:
+                return f"{rev_prefixes[pref]}:{suf}"
+            else:
+                return uri
+
         own_context = {}
 
+        if prefixes:
+            own_context.update(prefixes)
+
         def read_properties(where: dict):
             if not isinstance(where, dict):
                 return
             for prop, prop_val in where.get('properties', {}).items():
                 if isinstance(prop_val, dict) and ANNOTATION_ID in prop_val:
                     prop_context = {
-                        '@id': prop_val[ANNOTATION_ID]
+                        '@id': compact_uri(prop_val[ANNOTATION_ID])
                     }
                     if ANNOTATION_TYPE in prop_val:
-                        prop_context['@type'] = prop_val[ANNOTATION_TYPE]
+                        prop_context['@type'] = compact_uri(prop_val[ANNOTATION_TYPE])
 
                     if '$ref' in prop_val:
                         ref_fn, ref_url = resolve_ref(prop_val['$ref'], fn, url, base_url)
                         prop_context['@context'] = self._build_context(ref_fn, ref_url)
 
                     if len(prop_context) == 1:
                         # shorten to just the id
@@ -455,14 +544,15 @@
     """
     Creates a "mirror" directory (named `annotated` by default) with the resulting
     schemas annotated by a `SchemaAnnotator`.
 
     :param annotator: a `SchemaAnnotator` with the annotated schemas to read
     :param subdir: a name for the mirror directory
     :param root_dir: root directory for computing relative paths to schemas
+    :param output_fn_transform: optional callable to transform the output path
     """
     wd = (Path(root_dir) if root_dir else Path()).resolve()
     subdir = subdir if isinstance(subdir, Path) else Path(subdir)
     result = []
     for path, schema in annotator.schemas.items():
 
         if isinstance(path, Path):
```

### Comparing `ogc_na-0.1.2/ogc/na/domain_config.py` & `ogc_na-0.1.3/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/download.py` & `ogc_na-0.1.3/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/ingest_json.py` & `ogc_na-0.1.3/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/profile.py` & `ogc_na-0.1.3/ogc/na/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     def _load_profiles(self):
         g: Graph = Graph()
         for src in self._srcs:
             if isinstance(src, str) and src.startswith('sparql:'):
                 endpoint = src[len('sparql:'):]
                 logger.info("Fetching profiles from SPARQL endpoint %s", endpoint)
-                assert util.isurl(endpoint)
+                assert util.is_url(endpoint, http_only=True)
                 s = g.query(PROFILES_QUERY.replace('__SERVICE__', f"SERVICE <{endpoint}>")).graph
                 util.copy_triples(s, g)
             else:
                 g.parse(src)
 
         # resolve recursive isProfileOf and sameAs
         g = g.query(PROFILES_QUERY.replace('__SERVICE__', '')).graph
```

### Comparing `ogc_na-0.1.2/ogc/na/provenance.py` & `ogc_na-0.1.3/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/update_vocabs.py` & `ogc_na-0.1.3/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc/na/util.py` & `ogc_na-0.1.3/ogc/na/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 General utilities module.
 """
 from __future__ import annotations
 import os.path
 import shlex
 from glob import glob
 from pathlib import Path
-from typing import Optional, Union, Any
+from time import time
+from typing import Optional, Union, Any, Hashable
 
 import requests
 import rfc3987
 from rdflib import Graph
 from pyshacl import validate as shacl_validate
 from urllib.parse import urlparse
 
 from ogc.na.validation import ValidationReport
 
 import yaml
+
 try:
     from yaml import CLoader as YamlLoader, CSafeLoader as SafeYamlLoader, CDumper as YamlDumper
 except ImportError:
     from yaml import Loader as YamlLoader, SafeLoader as SafeYamlLoader, Dumper as YamlDumper
 
 
 def copy_triples(src: Graph, dst: Optional[Graph] = None) -> Graph:
@@ -101,15 +103,15 @@
     return ValidationReport(shacl_validate(data_graph=g,
                                            shacl_graph=shacl_graph,
                                            ont_graph=extra,
                                            inference='rdfs',
                                            advanced=True))
 
 
-def isurl(url: str, http_only: bool = False) -> bool:
+def is_url(url: str, http_only: bool = False) -> bool:
     """
     Checks whether a string is a valid URL.
 
     :param url: the input string
     :param http_only: whether to only accept HTTP and HTTPS URL's as valid
     :return: `True` if this is a valid URL, otherwise `False`
     """
@@ -184,25 +186,46 @@
             node = dst.setdefault(k, {})
             merge_dicts(v, node)
         else:
             dst[k] = v
     return dst
 
 
-def is_url(s: str) -> bool:
-    try:
-        url = urlparse(s)
-        return bool(url.scheme and url.netloc)
-    except ValueError:
-        return False
-
-
 def glob_list_split(s: str, exclude_dirs: bool = True, recursive: bool = False) -> list[str]:
     result = []
     for e in shlex.split(s):
         if is_url(s):
             result.append(s)
         else:
             for fn in glob(e, recursive=recursive):
                 if not exclude_dirs or os.path.isfile(fn):
                     result.append(fn)
     return result
+
+
+class LRUCache:
+
+    def __init__(self, maxsize: int = 10):
+        self._cache: dict[Hashable, Any] = {}
+        self._last_access: dict[Hashable, float] = {}
+        self._maxsize = maxsize
+
+    def __contains__(self, item):
+        return item in self._cache
+
+    def __len__(self):
+        return len(self._cache)
+
+    def get(self, key, default=None):
+        if not isinstance(key, Hashable):
+            return default
+        return self._cache.get(key, default)
+
+    def __setitem__(self, key, value):
+        if not isinstance(key, Hashable):
+            return
+        if len(self._cache) >= self._maxsize and key not in self._cache:
+            key_to_remove = min(self._last_access, key=self._last_access.get)
+            del self._cache[key_to_remove]
+            del self._last_access[key_to_remove]
+        self._cache[key] = value
+        self._last_access[key] = time()
```

### Comparing `ogc_na-0.1.2/ogc/na/validation.py` & `ogc_na-0.1.3/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ogc-na
-Version: 0.1.2
+Name: ogc_na
+Version: 0.1.3
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.2/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.1.3/ogc_na.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,11 @@
 test/__init__.py
 test/test_annotate_schema.py
 test/test_ingest_json.py
 test/test_profile.py
 test/data/empty.ttl
 test/data/profile_tree.ttl
 test/data/profile_tree_cyclic.ttl
+test/data/sample-context.jsonld
+test/data/sample-schema-prop-c.yml
+test/data/sample-schema.yml
 test/data/uplift_context_valid.yml
```

### Comparing `ogc_na-0.1.2/pyproject.toml` & `ogc_na-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/rdf/domaincfg.vocab.ttl` & `ogc_na-0.1.3/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/test/data/uplift_context_valid.yml` & `ogc_na-0.1.3/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/test/test_ingest_json.py` & `ogc_na-0.1.3/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.2/test/test_profile.py` & `ogc_na-0.1.3/test/test_profile.py`

 * *Files identical despite different names*

