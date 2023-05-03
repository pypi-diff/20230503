# Comparing `tmp/uniprot_redis-1.1.3.tar.gz` & `tmp/uniprot_redis-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniprot_redis-1.1.3.tar", max compression
+gzip compressed data, was "uniprot_redis-1.2.0.tar", max compression
```

## Comparing `uniprot_redis-1.1.3.tar` & `uniprot_redis-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      440 2023-05-03 09:18:40.676366 uniprot_redis-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-03 09:00:53.735912 uniprot_redis-1.1.3/uniprot_redis/__init__.py
--rw-r--r--   0        0        0     1226 2023-05-03 09:00:53.736104 uniprot_redis-1.1.3/uniprot_redis/__main__.py
--rw-r--r--   0        0        0     1805 2023-05-03 09:00:53.736256 uniprot_redis-1.1.3/uniprot_redis/server.py
--rw-r--r--   0        0        0     6158 2023-05-03 09:00:53.736533 uniprot_redis-1.1.3/uniprot_redis/store/__init__.py
--rw-r--r--   0        0        0     1646 2023-05-03 09:12:50.359281 uniprot_redis-1.1.3/uniprot_redis/store/schemas.py
--rw-r--r--   0        0        0      743 2023-05-03 09:18:52.294313 uniprot_redis-1.1.3/setup.py
--rw-r--r--   0        0        0      569 2023-05-03 09:18:52.294556 uniprot_redis-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      418 2023-02-17 16:21:54.989273 uniprot_redis-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-02-17 13:11:53.603236 uniprot_redis-1.2.0/uniprot_redis/__init__.py
+-rw-r--r--   0        0        0     1226 2023-02-17 13:11:53.603236 uniprot_redis-1.2.0/uniprot_redis/__main__.py
+-rw-r--r--   0        0        0     1811 2023-02-17 13:51:54.849456 uniprot_redis-1.2.0/uniprot_redis/server.py
+-rw-r--r--   0        0        0     5807 2023-02-17 13:56:07.563383 uniprot_redis-1.2.0/uniprot_redis/store/__init__.py
+-rw-r--r--   0        0        0     1609 2023-02-17 13:11:53.603236 uniprot_redis-1.2.0/uniprot_redis/store/schemas.py
+-rw-r--r--   0        0        0      743 2023-02-17 16:22:02.309908 uniprot_redis-1.2.0/setup.py
+-rw-r--r--   0        0        0      569 2023-02-17 16:22:02.310601 uniprot_redis-1.2.0/PKG-INFO
```

### Comparing `uniprot_redis-1.1.3/uniprot_redis/__main__.py` & `uniprot_redis-1.2.0/uniprot_redis/__main__.py`

 * *Files identical despite different names*

### Comparing `uniprot_redis-1.1.3/uniprot_redis/server.py` & `uniprot_redis-1.2.0/uniprot_redis/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 
 from .store import UniprotStore
 
 from .store.schemas import UniprotAC
 
 class UniprotRequest(BaseModel) : 
-    uniprotIDs : List[str]
+    uniprotIDs : List[UniprotAC]
 
 app = FastAPI()
 origins = ["*"]
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
```

### Comparing `uniprot_redis-1.1.3/uniprot_redis/store/__init__.py` & `uniprot_redis-1.2.0/uniprot_redis/store/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,15 @@
             try :
                 obj = UniprotDatum(id=prot.id, 
                     full_name=prot.fullName, 
                     name=prot.name, 
                     gene_name=prot.geneName,
                     taxid=prot.taxid,
                     sequence=prot.sequence,
-                    go = gos,
-                    subcellular_location = prot.subcellular_location)
+                    go = gos)
             except ValidationError as e:
                 print(f"Validation failed for {prot.id}: {str(e)}", file=stderr)
                 continue
             
             for sec_id in prot.AC:
                 correspondance_obj = SecondaryId(id=sec_id, parent_id=prot.id)
                 try:
@@ -118,18 +117,14 @@
             yield k
 
     @property
     def go_terms(self):
         for k in self.base_store.list_key(model=GODatum, skip_prefix=True):
             yield k
 
-    @property
-    def collections(self):
-        return self.base_store.list_key(model=UniprotCollection, skip_prefix=True)
-
     def get_protein(self, uniprot_id):
         try:
             correspondance_obj = self.base_store.get(uniprot_id, SecondaryId)
             obj = self.base_store.get(correspondance_obj.parent_id, UniprotDatum)
             return obj
         except StoreKeyNotFound:
             return None
@@ -138,18 +133,14 @@
 
     def get_proteins_with_mget(self, uniprot_ids):
         pass
 
     def get_proteins(self, uniprot_ids): 
         resp = {}
         for uniprot_id in uniprot_ids:
-            try :
-                UniprotAC.validate(uniprot_id)
-            except:
-                print(f"WARN : {uniprot_id} is not uniprot accession")
             resp[uniprot_id] = self.get_protein(uniprot_id)
         return resp
 
     def get_collections_from_prots(self, uniprot_ids):
         coll_for_prots = {}
         for coll_name, coll_content in self.list_collection():
             coll_for_prots[coll_name] = len(set(coll_content).intersection(set(uniprot_ids)))
```

### Comparing `uniprot_redis-1.1.3/uniprot_redis/store/schemas.py` & `uniprot_redis-1.2.0/uniprot_redis/store/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     id: UniprotAC
     full_name: str
     name: str
     gene_name: Optional[str]
     taxid: int
     sequence : str
     go : List[GODatum]
-    subcellular_location : List[str]
 
 class SecondaryId(BaseModel):
     id: UniprotAC
     parent_id: UniprotAC
 
 class UniprotCollection(BaseModel):
     comments:str
```

### Comparing `uniprot_redis-1.1.3/setup.py` & `uniprot_redis-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'fastapi>=0.79.0,<0.80.0',
  'pyproteinsext>=3.0.3,<4.0.0',
  'pyrediscore>=1.0.0,<2.0.0',
  'uvicorn>=0.18.2,<0.19.0']
 
 setup_kwargs = {
     'name': 'uniprot-redis',
-    'version': '1.1.3',
+    'version': '1.2.0',
     'description': '',
     'long_description': None,
     'author': 'Cecile Hilpert',
     'author_email': 'cecile.hilpert@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `uniprot_redis-1.1.3/PKG-INFO` & `uniprot_redis-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-redis
-Version: 1.1.3
+Version: 1.2.0
 Summary: 
 Author: Cecile Hilpert
 Author-email: cecile.hilpert@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

