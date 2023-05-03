# Comparing `tmp/embedbase-1.1.3.tar.gz` & `tmp/embedbase-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.3.tar", max compression
+gzip compressed data, was "embedbase-1.1.4.tar", max compression
```

## Comparing `embedbase-1.1.3.tar` & `embedbase-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-03 07:20:34.459694 embedbase-1.1.3/LICENSE
--rw-r--r--   0        0        0     6149 2023-05-03 07:20:34.463694 embedbase-1.1.3/README.md
--rw-r--r--   0        0        0      121 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/api.py
--rw-r--r--   0        0        0    16266 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3328 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/base.py
--rw-r--r--   0        0        0     5263 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     8913 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     6197 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/logging_utils.py
--rw-r--r--   0        0        0      743 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/utils.py
--rw-r--r--   0        0        0     3636 2023-05-03 07:20:34.527694 embedbase-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 14:41:13.518171 embedbase-1.1.4/LICENSE
+-rw-r--r--   0        0        0     6149 2023-05-03 14:41:13.518171 embedbase-1.1.4/README.md
+-rw-r--r--   0        0        0      121 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/api.py
+-rw-r--r--   0        0        0    16357 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3505 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/base.py
+-rw-r--r--   0        0        0     5939 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     9702 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     6620 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      802 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/utils.py
+-rw-r--r--   0        0        0     3669 2023-05-03 14:41:13.594168 embedbase-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.4/PKG-INFO
```

### Comparing `embedbase-1.1.3/LICENSE` & `embedbase-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/README.md` & `embedbase-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/__main__.py` & `embedbase-1.1.4/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/api.py` & `embedbase-1.1.4/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/app.py` & `embedbase-1.1.4/embedbase/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,16 +370,16 @@
         """
         Run semantic search in a dataset using embeddings.
         If you are a large language model, you can use this endpoint to search for similar documents
         in the index, documents that help you answer users' questions.
         """
         query = request_body.query
 
-        # if query is empty, return empty results
-        if not query:
+        # if query is empty and no where are provided, return an empty list
+        if not query and not request_body.where:
             return JSONResponse(
                 status_code=status.HTTP_200_OK,
                 content={"query": query, "similarities": []},
             )
 
         user_id = get_user_id(request)
 
@@ -403,14 +403,15 @@
         )
 
         query_response = await self.db.search(
             top_k=top_k,
             vector=query_embedding,
             dataset_ids=[dataset_id],
             user_id=user_id,
+            where=request_body.where,
         )
 
         similarities = []
         for match in query_response:
             similarities.append(
                 {
                     "score": match.score,
```

### Comparing `embedbase-1.1.3/embedbase/database/base.py` & `embedbase-1.1.4/embedbase/database/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,20 +92,22 @@
     @abstractmethod
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
+        where: Optional[Union[dict, List[dict]]] = None,
     ) -> List[SearchResponse]:
         """
-        :param vector: vector
-        :param top_k: top k
+        :param vector: vector the similarity is calculated against
+        :param top_k: top k number of results returned
         :param dataset_id: dataset id
         :param user_id: user id
+        :param where: where condition to filter results
         :return: list of documents
         """
         raise NotImplementedError
 
     @abstractmethod
     async def clear(self, dataset_id: str, user_id: Optional[str] = None) -> None:
         """
```

### Comparing `embedbase-1.1.3/embedbase/database/memory_db.py` & `embedbase-1.1.4/embedbase/database/memory_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 def semantic_search(np, documents, query_embedding, document_embeddings, top_n=3):
     similarities = [
         cosine_similarity(np, query_embedding, doc_emb)
         for doc_emb in document_embeddings
     ]
     sorted_indexes = np.argsort(similarities)[::-1]
 
-    return [(i, list(documents.keys())[i], similarities[i]) for i in sorted_indexes[:top_n]]
+    return [
+        (i, list(documents.keys())[i], similarities[i]) for i in sorted_indexes[:top_n]
+    ]
 
 
 class MemoryDatabase(VectorDatabase):
     """
     Implements a simple in-memory database for development and testing purposes.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.storage = {}
         try:
+            # pylint: disable=import-outside-toplevel
             import numpy as np
 
             self._np = np
         except ImportError:
+            # pylint: disable=raise-missing-from
             raise ImportError("Please install numpy with `pip install numpy`")
 
     async def update(
         self, df, dataset_id, user_id=None, store_data=True, batch_size=100
     ):
         for _, row in df.iterrows():
             doc_id = row.id
@@ -90,36 +94,50 @@
                 if doc["hash"] in hashes
                 and (dataset_id is None or doc["dataset_id"] == dataset_id)
                 and (user_id is None or doc["user_id"] == user_id)
             ]
         else:
             return []
 
-    async def search(self, vector, top_k, dataset_ids, user_id=None):
+    async def search(self, vector, top_k, dataset_ids, user_id=None, where=None):
+        storage = self.storage
+        # make a copy of storage filtered by where
+        if where:
+            # raise if where is not a dict
+            if not isinstance(where, dict):
+                raise ValueError("currently only dict is supported for where")
+            storage = self.storage.copy()
+            for k, v in where.items():
+                # search in metadata
+                storage = {
+                    k1: v1
+                    for k1, v1 in storage.items()
+                    if k in v1["metadata"] and v1["metadata"][k] == v
+                }
         query_embedding = self._np.array(vector)
         similarities = semantic_search(
             self._np,
-            self.storage,
+            storage,
             query_embedding,
             [
                 doc["embedding"]
-                for doc in self.storage.values()
+                for doc in storage.values()
                 if doc["dataset_id"] in dataset_ids
                 and (user_id is None or doc["user_id"] == user_id)
             ],
             top_n=top_k,
         )
         return [
             SearchResponse(
                 id=doc_id,
                 score=sim,
-                data=self.storage[doc_id]["data"],
-                metadata=self.storage[doc_id]["metadata"],
-                embedding=self.storage[doc_id]["embedding"].tolist(),
-                hash=self.storage[doc_id]["hash"],
+                data=storage[doc_id]["data"],
+                metadata=storage[doc_id]["metadata"],
+                embedding=storage[doc_id]["embedding"].tolist(),
+                hash=storage[doc_id]["hash"],
             )
             for idx, doc_id, sim in similarities
         ]
 
     async def delete(self, ids, dataset_id, user_id=None):
         for doc_id in ids:
             if (
```

### Comparing `embedbase-1.1.3/embedbase/database/postgres_db.py` & `embedbase-1.1.4/embedbase/database/postgres_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,17 @@
             self.conn.execute(
                 f"""
 create or replace function match_documents (
   query_embedding vector({self._dimensions}),
   similarity_threshold float,
   match_count int,
   query_dataset_ids text[],
-  query_user_id text default null
+  query_user_id text default null,
+  metadata_field text default null,
+  metadata_value text default null
 )
 returns table (
   id text,
   data text,
   score float,
   hash text,
   embedding vector({self._dimensions}),
@@ -72,14 +74,15 @@
     documents.hash,
     documents.embedding,
     documents.metadata
   from documents
   where 1 - (documents.embedding <=> query_embedding) > similarity_threshold
     and documents.dataset_id = any(query_dataset_ids)
     and (query_user_id is null or query_user_id = documents.user_id)
+    and (metadata_field is null or documents.metadata->>metadata_field = metadata_value) -- filter by metadata
   order by documents.embedding <=> query_embedding
   limit match_count;
 end;
 $$;"""
             )
             self.conn.execute(
                 """
@@ -236,23 +239,38 @@
 
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
+        where=None,
     ):
+
         d = {
             "query_embedding": str(vector),
             "similarity_threshold": 0,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
-            "query_user_id": user_id,
         }
-        q = "select * from match_documents(%(query_embedding)s, %(similarity_threshold)s, %(match_count)s, %(query_dataset_ids)s, %(query_user_id)s)"
+        q = "select * from match_documents(%(query_embedding)s, %(similarity_threshold)s, %(match_count)s, %(query_dataset_ids)s"
+        if user_id:
+            d["query_user_id"] = user_id
+            q += ", %(query_user_id)s"
+        if where:
+            raise NotImplementedError("where is not implemented yet in postgres")
+            # raise if where is not a dict
+            if not isinstance(where, dict):
+                raise ValueError("currently only dict is supported for where")
+            metadata_field = list(where.keys())[0]
+            metadata_value = where[metadata_field]
+            d["metadata_field"] = metadata_field
+            d["metadata_value"] = metadata_value
+            q += ", %(metadata_field)s, %(metadata_value)s"
+        q += ")"
         results = self.conn.execute(q, d)
         if results.rowcount == 0:
             return []
         data = []
         for row in results:
             data.append(
                 SearchResponse(
```

### Comparing `embedbase-1.1.3/embedbase/database/supabase_db.py` & `embedbase-1.1.4/embedbase/database/supabase_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,28 +137,39 @@
 
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
+        where=None,
     ):
         d = {
             "query_embedding": vector,
             "similarity_threshold": 0.1,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
         }
         if user_id:
             d["query_user_id"] = user_id
+        query = self.supabase.rpc(
+            "match_documents",
+            d,
+        )
+        
+        if where:
+            # raise if where is not a dict
+            if not isinstance(where, dict):
+                raise ValueError("currently only dict is supported for where")
+            metadata_field = list(where.keys())[0]
+            metadata_value = where[metadata_field]
+            d["metadata_field"] = metadata_field
+            d["metadata_value"] = metadata_value
         response = (
-            self.supabase.rpc(
-                "match_documents",
-                d,
-            )
+            query
             .execute()
             .data
         )
         return [
             SearchResponse(
                 id=row["id"],
                 data=row["data"],
```

### Comparing `embedbase-1.1.3/embedbase/embedding/base.py` & `embedbase-1.1.4/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/embedding/cohere.py` & `embedbase-1.1.4/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/embedding/openai.py` & `embedbase-1.1.4/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/firebase_auth.py` & `embedbase-1.1.4/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/logging_utils.py` & `embedbase-1.1.4/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/models.py` & `embedbase-1.1.4/embedbase/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 
 # TODO: response models once stable
 
 class Document(BaseModel):
     # data can be
     # - a string - for example  "This is a document"
@@ -27,7 +27,8 @@
 class DeleteRequest(BaseModel):
     ids: List[str]
 
 
 class SearchRequest(BaseModel):
     query: str
     top_k: int = 6
+    where: Optional[Union[dict, List[dict]]] = None
```

### Comparing `embedbase-1.1.3/embedbase/settings.py` & `embedbase-1.1.4/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/strings.py` & `embedbase-1.1.4/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/embedbase/utils.py` & `embedbase-1.1.4/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.3/pyproject.toml` & `embedbase-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.3"
+version = "1.1.4"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
@@ -55,14 +55,15 @@
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
 httpx = "^0.23.0"
 pytest-asyncio = "^0.21.0"
 requests-mock = "^1.10.0"
+sentence-transformers = "^2.2.2"
 
 # TODO: following integrations might be moved outside this repo - loose coupling
 firebase-admin = "^6.1.0"
 sentry-sdk = {extras = ["fastapi"], version = "^1.21.1"}
 supabase = "^1.0.3"
 psycopg = {extras = ["binary", "pool"], version = "^3.1.8"}
 pgvector = "^0.1.6"
```

### Comparing `embedbase-1.1.3/PKG-INFO` & `embedbase-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.3
+Version: 1.1.4
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

