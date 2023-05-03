# Comparing `tmp/embedbase-1.1.2.tar.gz` & `tmp/embedbase-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.2.tar", max compression
+gzip compressed data, was "embedbase-1.1.3.tar", max compression
```

## Comparing `embedbase-1.1.2.tar` & `embedbase-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-02 18:12:44.377590 embedbase-1.1.2/LICENSE
--rw-r--r--   0        0        0     6149 2023-05-02 18:12:44.377590 embedbase-1.1.2/README.md
--rw-r--r--   0        0        0      121 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/api.py
--rw-r--r--   0        0        0    16533 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3328 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/base.py
--rw-r--r--   0        0        0     2036 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4901 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     7957 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     5199 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/logging_utils.py
--rw-r--r--   0        0        0      743 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-02 18:12:44.437592 embedbase-1.1.2/embedbase/utils.py
--rw-r--r--   0        0        0     3636 2023-05-02 18:12:44.441592 embedbase-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 07:20:34.459694 embedbase-1.1.3/LICENSE
+-rw-r--r--   0        0        0     6149 2023-05-03 07:20:34.463694 embedbase-1.1.3/README.md
+-rw-r--r--   0        0        0      121 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/api.py
+-rw-r--r--   0        0        0    16266 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3328 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/base.py
+-rw-r--r--   0        0        0     5263 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     8913 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     6197 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-03 07:20:34.523694 embedbase-1.1.3/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      743 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-03 07:20:34.527694 embedbase-1.1.3/embedbase/utils.py
+-rw-r--r--   0        0        0     3636 2023-05-03 07:20:34.527694 embedbase-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.3/PKG-INFO
```

### Comparing `embedbase-1.1.2/LICENSE` & `embedbase-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/README.md` & `embedbase-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/__main__.py` & `embedbase-1.1.3/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/api.py` & `embedbase-1.1.3/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/app.py` & `embedbase-1.1.3/embedbase/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import asyncio
-import itertools
 import os
-from typing import Awaitable, Callable, Optional, Tuple, Union, Any
-import warnings
-from fastapi import FastAPI, Request
+from typing import Awaitable, Callable, Optional, Tuple, Union
+from fastapi import FastAPI, Request, status
 from fastapi.middleware import Middleware
 from starlette.types import Scope
-from embedbase.database.base import SearchResponse, VectorDatabase
+from embedbase.database.base import VectorDatabase
 from embedbase.embedding.base import Embedder
 from embedbase.logging_utils import get_logger
 from embedbase.models import (
     DeleteRequest,
     SearchRequest,
     AddRequest,
     UpdateRequest,
 )
-from embedbase.utils import embedbase_ascii
+from embedbase.utils import embedbase_ascii, get_user_id
 from embedbase.settings import Settings
 import hashlib
 import time
 import urllib.parse
 import uuid
 
-from fastapi import Request, status
 from fastapi.responses import JSONResponse, ORJSONResponse
 from pandas import DataFrame
 
-from embedbase.database.db_utils import batch_select
-from embedbase.utils import get_user_id
 
 UPLOAD_BATCH_SIZE = int(os.environ.get("UPLOAD_BATCH_SIZE", "100"))
 
 
 class Embedbase:
     """
     Embedbase is the main class of the Embedbase library.
@@ -161,16 +156,15 @@
         df_length = len(df)
 
         self.logger.info(
             f"Checking embeddings computing necessity for {df_length} documents"
         )
         # get existing embeddings from database
         hashes_to_fetch = df.hash.tolist()
-        existing_documents = await batch_select(
-            vector_database=self.db,
+        existing_documents = await self.db.select(
             hashes=list(set(hashes_to_fetch)),
             dataset_id=None,
             user_id=None,
         )
 
         def update_embedding(row, existing_documents):
             for doc in existing_documents:
@@ -200,16 +194,15 @@
                 embedding=await self.embedder.embed(
                     df[df.embedding.isna()].data.tolist()
                 )
             )
 
         # only insert if this dataset_id - user_id
         # pair does not have this hash
-        existing_documents_in_this_pair = await batch_select(
-            vector_database=self.db,
+        existing_documents_in_this_pair = await self.db.select(
             hashes=list(set(hashes_to_fetch)),
             dataset_id=dataset_id,
             user_id=user_id,
         )
 
         # filter out documents that already exist
         # in this dataset_id - user_id pair
@@ -299,16 +292,15 @@
         df_length = len(df)
 
         self.logger.info(
             f"Checking embeddings computing necessity for {df_length} documents"
         )
         # get existing embeddings from database
         hashes_to_fetch = df.hash.tolist()
-        existing_embeddings = await batch_select(
-            vector_database=self.db,
+        existing_embeddings = await self.db.select(
             hashes=list(set(hashes_to_fetch)),
             dataset_id=None,
             user_id=None,
         )
 
         def update_embedding(row, docs):
             for doc in docs:
```

### Comparing `embedbase-1.1.2/embedbase/database/base.py` & `embedbase-1.1.3/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/database/memory_db.py` & `embedbase-1.1.3/embedbase/database/memory_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,30 @@
     Dataset,
     SearchResponse,
     SelectResponse,
     VectorDatabase,
 )
 
 
+# Calculate cosine similarity
+def cosine_similarity(np, a, b):
+    return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
+
+
+# Semantic search function
+def semantic_search(np, documents, query_embedding, document_embeddings, top_n=3):
+    similarities = [
+        cosine_similarity(np, query_embedding, doc_emb)
+        for doc_emb in document_embeddings
+    ]
+    sorted_indexes = np.argsort(similarities)[::-1]
+
+    return [(i, list(documents.keys())[i], similarities[i]) for i in sorted_indexes[:top_n]]
+
+
 class MemoryDatabase(VectorDatabase):
     """
     Implements a simple in-memory database for development and testing purposes.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -76,38 +92,36 @@
                 and (user_id is None or doc["user_id"] == user_id)
             ]
         else:
             return []
 
     async def search(self, vector, top_k, dataset_ids, user_id=None):
         query_embedding = self._np.array(vector)
-        similarities = [
-            (
-                doc_id,
-                self._np.dot(doc["embedding"], query_embedding)
-                / (
-                    self._np.linalg.norm(doc["embedding"])
-                    * self._np.linalg.norm(query_embedding)
-                ),
-            )
-            for doc_id, doc in self.storage.items()
-            if doc["dataset_id"] in dataset_ids
-            and (user_id is None or doc["user_id"] == user_id)
-        ]
-        similarities.sort(key=lambda x: x[1], reverse=True)
+        similarities = semantic_search(
+            self._np,
+            self.storage,
+            query_embedding,
+            [
+                doc["embedding"]
+                for doc in self.storage.values()
+                if doc["dataset_id"] in dataset_ids
+                and (user_id is None or doc["user_id"] == user_id)
+            ],
+            top_n=top_k,
+        )
         return [
             SearchResponse(
                 id=doc_id,
                 score=sim,
                 data=self.storage[doc_id]["data"],
                 metadata=self.storage[doc_id]["metadata"],
                 embedding=self.storage[doc_id]["embedding"].tolist(),
                 hash=self.storage[doc_id]["hash"],
             )
-            for doc_id, sim in similarities[:top_k]
+            for idx, doc_id, sim in similarities
         ]
 
     async def delete(self, ids, dataset_id, user_id=None):
         for doc_id in ids:
             if (
                 doc_id in self.storage
                 and (
```

### Comparing `embedbase-1.1.2/embedbase/database/postgres_db.py` & `embedbase-1.1.3/embedbase/database/postgres_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 import json
 from typing import List, Optional
-
+import itertools
 from pandas import DataFrame, Series
 
 from embedbase.database import VectorDatabase
 from embedbase.database.base import Dataset, SearchResponse, SelectResponse
 
 
 class Postgres(VectorDatabase):
@@ -86,18 +87,20 @@
 SELECT dataset_id, user_id, COUNT(*) AS documents_count
 FROM documents
 GROUP BY dataset_id, user_id;
 """
             )
 
         except ImportError:
+            # pylint: disable=raise-missing-from
             raise ImportError(
                 "Please install pgvector and psycopg with `pip install pgvector psycopg[binary]`"
             )
         except psycopg.OperationalError:
+            # pylint: disable=raise-missing-from
             raise psycopg.OperationalError(
                 "Please run a postgresql and create a database named embedbase"
             )
         except Exception as e:
             print(e)
 
     async def select(
@@ -115,46 +118,67 @@
 
         query = """
 select id, data, embedding, hash, metadata
 from documents
 where
     {conditions}
 """
-        conditions = []
+
+        async def _fetch(ids, hashes) -> List[dict]:
+            try:
+                conditions = []
+                if ids:
+                    conditions.append(
+                        sql.SQL("id in ({})").format(
+                            sql.SQL(",").join(map(sql.Literal, ids))
+                        )
+                    )
+                if hashes:
+                    conditions.append(
+                        sql.SQL("hash in ({})").format(
+                            sql.SQL(",").join(map(sql.Literal, hashes))
+                        )
+                    )
+                if dataset_id:
+                    conditions.append(
+                        sql.SQL("dataset_id = {}").format(sql.Literal(dataset_id))
+                    )
+                if user_id:
+                    conditions.append(
+                        sql.SQL("user_id = {}").format(sql.Literal(user_id))
+                    )
+                return list(self.conn.execute(
+                    sql.SQL(query).format(conditions=sql.SQL(" and ").join(conditions))
+                ))
+            except Exception as e:
+                raise e
+
+        # we need to run parallel requests with postgres
+        n = 50
+        docs = []
         if ids:
-            conditions.append(
-                sql.SQL("id in ({})").format(sql.SQL(",").join(map(sql.Literal, ids)))
-            )
-        if hashes:
-            conditions.append(
-                sql.SQL("hash in ({})").format(
-                    sql.SQL(",").join(map(sql.Literal, hashes))
-                )
-            )
-        if dataset_id:
-            conditions.append(
-                sql.SQL("dataset_id = {}").format(sql.Literal(dataset_id))
-            )
-        if user_id:
-            conditions.append(sql.SQL("user_id = {}").format(sql.Literal(user_id)))
-        data = []
-        results = self.conn.execute(
-            sql.SQL(query).format(conditions=sql.SQL(" and ").join(conditions))
-        )
-        for row in results:
-            data.append(
-                SelectResponse(
-                    id=row[0],
-                    data=row[1],
-                    embedding=row[2].tolist(),
-                    hash=row[3],
-                    metadata=row[4],
-                )
+            elements = [ids[i : i + n] for i in range(0, len(ids), n)]
+            docs = await asyncio.gather(
+                *[_fetch(e, []) for e in elements]
+            )
+        else:
+            elements = [hashes[i : i + n] for i in range(0, len(hashes), n)]
+            docs = await asyncio.gather(
+                *[_fetch([], e) for e in elements]
+            )
+        return [
+            SelectResponse(
+                id=row[0],
+                data=row[1],
+                embedding=row[2].tolist(),
+                hash=row[3],
+                metadata=row[4],
             )
-        return data
+            for row in itertools.chain.from_iterable(docs)
+        ]
 
     async def update(
         self,
         df: DataFrame,
         dataset_id: str,
         user_id: Optional[str] = None,
         batch_size: Optional[int] = 100,
```

### Comparing `embedbase-1.1.2/embedbase/database/supabase_db.py` & `embedbase-1.1.3/embedbase/database/supabase_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import itertools
 from typing import List, Optional
 from pandas import DataFrame, Series
 from embedbase.database import VectorDatabase
 from embedbase.database.base import Dataset, SearchResponse, SelectResponse
 from embedbase.utils import BatchGenerator
 
 
@@ -34,41 +35,64 @@
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
         distinct: bool = True,
     ):
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
 
-        req = self.supabase.table("documents").select("*")
+        # raise if both ids and hashes are provided
+        assert not (ids and hashes), "ids and hashes cannot be provided at the same time"
+        # TODO not supported yet
+
+        async def _fetch(ids, hashes) -> List[dict]:
+            try:
+                req = self.supabase.table("documents").select("*")
+                if ids:
+                    req = req.in_("id", ids)
+                    if distinct:
+                        # hack: supabase does not support distinct
+                        req = req.order("id", desc=True)
+                        req = req.limit(len(ids))
+                if hashes:
+                    req = req.in_("hash", hashes)
+                    if distinct:
+                        # hack: supabase does not support distinct
+                        req = req.order("hash", desc=True)
+                        req = req.limit(len(hashes))
+                if dataset_id:
+                    req = req.eq("dataset_id", dataset_id)
+                if user_id:
+                    req = req.eq("user_id", user_id)
+
+                return req.execute().data
+            except Exception as e:
+                raise e
+
+        # we need to run parallel requests with supabase
+        n = 50
+        docs = []
         if ids:
-            req = req.in_("id", ids)
-            if distinct:
-                # hack: supabase does not support distinct
-                req = req.order("id", desc=True)
-                req = req.limit(len(ids))
-        if hashes:
-            req = req.in_("hash", hashes)
-            if distinct:
-                # hack: supabase does not support distinct
-                req = req.order("hash", desc=True)
-                req = req.limit(len(hashes))
-        if dataset_id:
-            req = req.eq("dataset_id", dataset_id)
-        if user_id:
-            req = req.eq("user_id", user_id)
-
+            elements = [ids[i : i + n] for i in range(0, len(ids), n)]
+            docs = await asyncio.gather(
+                *[_fetch(e, []) for e in elements]
+            )
+        else:
+            elements = [hashes[i : i + n] for i in range(0, len(hashes), n)]
+            docs = await asyncio.gather(
+                *[_fetch([], e) for e in elements]
+            )
         return [
             SelectResponse(
                 id=row["id"],
                 data=row["data"],
                 embedding=row["embedding"],
                 hash=row["hash"],
                 metadata=row["metadata"],
             )
-            for row in req.execute().data
+            for row in itertools.chain.from_iterable(docs)
         ]
 
     async def update(
         self,
         df: DataFrame,
         dataset_id: str,
         user_id: Optional[str] = None,
```

### Comparing `embedbase-1.1.2/embedbase/embedding/base.py` & `embedbase-1.1.3/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/embedding/cohere.py` & `embedbase-1.1.3/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/embedding/openai.py` & `embedbase-1.1.3/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/firebase_auth.py` & `embedbase-1.1.3/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/logging_utils.py` & `embedbase-1.1.3/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/models.py` & `embedbase-1.1.3/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/settings.py` & `embedbase-1.1.3/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/strings.py` & `embedbase-1.1.3/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/embedbase/utils.py` & `embedbase-1.1.3/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.2/pyproject.toml` & `embedbase-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.2"
+version = "1.1.3"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

### Comparing `embedbase-1.1.2/PKG-INFO` & `embedbase-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.2
+Version: 1.1.3
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

