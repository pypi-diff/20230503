# Comparing `tmp/paper-qa-1.3.0.tar.gz` & `tmp/paper-qa-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.3.0.tar", last modified: Sat Apr 29 19:10:37 2023, max compression
+gzip compressed data, was "paper-qa-1.4.0.tar", last modified: Wed May  3 07:10:33 2023, max compression
```

## Comparing `paper-qa-1.3.0.tar` & `paper-qa-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 19:09:49.000000 paper-qa-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 19:10:37.070681 paper-qa-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-29 19:09:49.000000 paper-qa-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 19:10:37.070681 paper-qa-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-29 19:09:49.000000 paper-qa-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-29 19:09:49.000000 paper-qa-1.3.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 07:09:45.000000 paper-qa-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-03 07:10:33.769626 paper-qa-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-05-03 07:09:45.000000 paper-qa-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.765626 paper-qa-1.4.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:10:33.769626 paper-qa-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-03 07:09:45.000000 paper-qa-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-03 07:09:45.000000 paper-qa-1.4.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.3.0/LICENSE` & `paper-qa-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.3.0/PKG-INFO` & `paper-qa-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.3.0
+Version: 1.4.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.3.0/README.md` & `paper-qa-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.3.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.4.0/paper_qa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.3.0
+Version: 1.4.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.3.0/paperqa/agent.py` & `paper-qa-1.4.0/paperqa/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from langchain.tools import BaseTool
-from .docs import Answer, Docs
-from langchain.agents import initialize_agent
-from langchain.chat_models import ChatOpenAI
+from langchain.agents import AgentType, initialize_agent
 from langchain.chains import LLMChain
-from langchain.agents import AgentType
-from .qaprompts import select_paper_prompt, make_chain
+from langchain.chat_models import ChatOpenAI
+from langchain.tools import BaseTool
 from rmrkl import ChatZeroShotAgent, RetryAgentExecutor
 
+from .docs import Answer, Docs
+from .qaprompts import make_chain, select_paper_prompt
+
 
 def status(answer: Answer, docs: Docs):
     return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: ${answer.cost:.2f}"
 
 
 class PaperSelection(BaseTool):
     name = "Select Papers"
@@ -87,32 +87,33 @@
         # call the parent class constructor
         super(AnswerTool, self).__init__()
 
         self.docs = docs
         self.answer = answer
 
     def _run(self, query: str) -> str:
-        self.answer = self.docs.query(
-            query, answer=self.answer
-        )
+        self.answer = self.docs.query(query, answer=self.answer)
         if "cannot answer" in self.answer.answer:
             self.answer = Answer(self.answer.question)
-            return "Failed to answer question. Deleting evidence. Consider rephrasing question or evidence statement." + status(
-                self.answer, self.docs
+            return (
+                "Failed to answer question. Deleting evidence. Consider rephrasing question or evidence statement."
+                + status(self.answer, self.docs)
             )
         return self.answer.answer + status(self.answer, self.docs)
 
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
 
 
 class Search(BaseTool):
     name = "Paper Search"
-    description = "Search for papers to add to cur. Input should be a string of keywords."
+    description = (
+        "Search for papers to add to cur. Input should be a string of keywords."
+    )
     docs: Docs = None
     answer: Answer = None
 
     def __init__(self, docs, answer):
         # call the parent class constructor
         super(Search, self).__init__()
 
@@ -139,15 +140,14 @@
 
     def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError()
 
 
 def make_tools(docs, answer):
-
     tools = []
 
     tools.append(Search(docs, answer))
     tools.append(PaperSelection(docs, answer))
     tools.append(ReadPapers(docs, answer))
     tools.append(AnswerTool(docs, answer))
     return tools
```

### Comparing `paper-qa-1.3.0/paperqa/contrib/zotero.py` & `paper-qa-1.4.0/paperqa/contrib/zotero.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file gets PDF files from the user's Zotero library
-import os
-from typing import Union, Optional
-from pathlib import Path
 import logging
+import os
 from collections import namedtuple
+from pathlib import Path
+from typing import Optional, Union
 
 try:
     from pyzotero import zotero
 except ImportError:
     raise ImportError("Please install pyzotero: `pip install pyzotero`")
 from ..paths import CACHE_PATH
-from ..utils import count_pdf_pages
 from ..types import StrPath
+from ..utils import count_pdf_pages
 
 ZoteroPaper = namedtuple(
     "ZoteroPaper", ["key", "title", "pdf", "num_pages", "zotero_key", "details"]
 )
 
 
 def _zotero_paper_repr(self) -> str:
```

### Comparing `paper-qa-1.3.0/paperqa/docs.py` & `paper-qa-1.4.0/paperqa/docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from typing import List, Optional, Tuple, Union, Callable
-from functools import reduce
+import asyncio
 import os
+import re
 import sys
-import asyncio
+from datetime import datetime
+from functools import reduce
 from pathlib import Path
-import re
-from .paths import CACHE_PATH
-from .utils import maybe_is_text, md5sum
-from .qaprompts import (
-    summary_prompt,
-    qa_prompt,
-    search_prompt,
-    citation_prompt,
-    select_paper_prompt,
-    make_chain,
-)
-from .types import Answer, Context
-from .readers import read_doc
-from langchain.vectorstores import FAISS
+from typing import Callable, List, Optional, Tuple, Union
+
+import langchain
+from langchain.cache import SQLiteCache
+from langchain.callbacks import OpenAICallbackHandler, get_openai_callback
+from langchain.callbacks.base import AsyncCallbackHandler
+from langchain.callbacks.manager import AsyncCallbackManager
+from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
-from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.embeddings.base import Embeddings
-from langchain.chat_models import ChatOpenAI
+from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.llms.base import LLM
-from langchain.callbacks import get_openai_callback, OpenAICallbackHandler
-from langchain.callbacks.base import AsyncCallbackHandler, AsyncCallbackManager
-from langchain.cache import SQLiteCache
-import langchain
-from datetime import datetime
+from langchain.vectorstores import FAISS
+
+from .paths import CACHE_PATH
+from .qaprompts import (citation_prompt, make_chain, qa_prompt, search_prompt,
+                        select_paper_prompt, summary_prompt)
+from .readers import read_doc
+from .types import Answer, Context
+from .utils import maybe_is_text, md5sum
 
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
 
 class Docs:
     """A collection of documents to be used for answering questions."""
@@ -40,41 +37,38 @@
         self,
         chunk_size_limit: int = 3000,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
         name: str = "default",
         index_path: Optional[Path] = None,
         embeddings: Optional[Embeddings] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x : []
     ) -> None:
         """Initialize the collection of documents.
 
         Args:
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
             embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
-            get_callbacks: A function that allows callbacks to built per stage of the pipeline.
         """
         self.docs = dict()
         self.chunk_size_limit = chunk_size_limit
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         self.update_llm(llm, summary_llm)
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
         self.index_path = index_path
         self.name = name
         if embeddings is None:
             embeddings = OpenAIEmbeddings()
         self.embeddings = embeddings
-        self.get_callbacks = get_callbacks
 
     def update_llm(
         self,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
@@ -92,30 +86,30 @@
     def add(
         self,
         path: str,
         citation: Optional[str] = None,
         key: Optional[str] = None,
         disable_check: bool = False,
         chunk_chars: Optional[int] = 3000,
-        overwrite: bool = False,
     ) -> None:
         """Add a document to the collection."""
 
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         md5 = md5sum(path)
         if path in self.docs:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
             cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
-            with get_openai_callback():
-                citation = cite_chain.run(texts[0])
+            if len(texts) == 0:
+                raise ValueError(f"Could not read document {path}. Is it empty?")
+            citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
                 author = re.search(r"([A-Z][a-z]+)", citation).group(1)
@@ -203,20 +197,18 @@
         if self._faiss_index is None and len(self.docs) > 0:
             self._build_faiss_index()
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
-        del state["get_callbacks"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
-        self.get_callbacks = lambda x: []
         try:
             self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
@@ -236,16 +228,17 @@
 
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None    
-        ) -> Answer:
+        key_filter: Optional[List[str]] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+    ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
             loop = asyncio.get_event_loop()
@@ -254,25 +247,27 @@
             asyncio.set_event_loop(loop)
         return loop.run_until_complete(
             self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-                key_filter=key_filter
+                key_filter=key_filter,
+                get_callbacks=get_callbacks,
             )
         )
 
     async def aget_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         key_filter: Optional[List[str]] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
     ) -> Answer:
         if len(self.docs) == 0:
             return answer
         if self._faiss_index is None:
             self._build_faiss_index()
         _k = k
         if key_filter is not None:
@@ -289,37 +284,40 @@
 
         async def process(doc):
             if key_filter is not None and doc.metadata["dockey"] not in key_filter:
                 return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None, None
-            cb = OpenAICallbackHandler()
-            manager = AsyncCallbackManager([cb] + self.get_callbacks('evidence:' + doc.metadata['key']))
-            summary_chain = make_chain(summary_prompt, self.summary_llm, manager)
+            callbacks = [OpenAICallbackHandler()] + get_callbacks(
+                "evidence:" + doc.metadata["key"]
+            )
+            summary_chain = make_chain(summary_prompt, self.summary_llm)
             c = Context(
                 key=doc.metadata["key"],
                 citation=doc.metadata["citation"],
                 context=await summary_chain.arun(
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
+                    callbacks=callbacks,
                 ),
                 text=doc.page_content,
             )
             if "Not applicable" not in c.context:
                 return c, cb
             return None, None
 
-        results = await asyncio.gather(*[process(doc) for doc in docs])
+        with get_openai_callback() as cb:
+            results = await asyncio.gather(*[process(doc) for doc in docs])
         # filter out failures
         results = [r for r in results if r[0] is not None]
         answer.tokens += sum([cb.total_tokens for _, cb in results])
         answer.cost += sum([cb.total_cost for _, cb in results])
-        contexts = [c for c,_ in results if c is not None]
+        contexts = [c for c, _ in results if c is not None]
         if len(contexts) == 0:
             return answer
         contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
         contexts = contexts[:max_sources]
         # add to answer (if not already there)
         keys = [c.key for c in answer.contexts]
         for c in contexts:
@@ -361,14 +359,15 @@
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
     ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
@@ -381,26 +380,28 @@
                 query,
                 k=k,
                 max_sources=max_sources,
                 length_prompt=length_prompt,
                 marginal_relevance=marginal_relevance,
                 answer=answer,
                 key_filter=key_filter,
+                get_callbacks=get_callbacks,
             )
         )
 
     async def aquery(
         self,
         query: str,
         k: int = 10,
         max_sources: int = 5,
         length_prompt: str = "about 100 words",
         marginal_relevance: bool = True,
         answer: Optional[Answer] = None,
         key_filter: Optional[bool] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(query)
         if len(answer.contexts) == 0:
             if key_filter or (key_filter is None and len(self.docs) > 5):
@@ -410,29 +411,33 @@
                 answer.cost += cb.total_cost
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 key_filter=keys if key_filter else None,
+                get_callbacks=get_callbacks,
             )
         context_str, contexts = answer.context, answer.contexts
         bib = dict()
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
             cb = OpenAICallbackHandler()
-            manager = AsyncCallbackManager([cb] + self.get_callbacks('answer'))
-            qa_chain = make_chain(qa_prompt, self.llm, manager)
+            callbacks = [OpenAICallbackHandler()] + get_callbacks("answer")
+            qa_chain = make_chain(qa_prompt, self.llm)
             answer_text = await qa_chain.arun(
-                    question=query, context_str=context_str, length=length_prompt
-                )
+                question=query,
+                context_str=context_str,
+                length=length_prompt,
+                callbacks=callbacks,
+            )
             answer.tokens += cb.total_tokens
             answer.cost += cb.total_cost
         # it still happens lol
         if "(Foo2012)" in answer_text:
             answer_text = answer_text.replace("(Foo2012)", "")
         for c in contexts:
             key = c.key
```

### Comparing `paper-qa-1.3.0/paperqa/qaprompts.py` & `paper-qa-1.4.0/paperqa/qaprompts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-import langchain.prompts as prompts
 from datetime import datetime
+from typing import Any, Dict, List, Optional
+
+import langchain.prompts as prompts
+from langchain.callbacks.manager import AsyncCallbackManagerForChainRun
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
-from langchain.schema import SystemMessage
-from langchain.prompts.chat import HumanMessagePromptTemplate, ChatPromptTemplate
+from langchain.prompts.chat import (ChatPromptTemplate,
+                                    HumanMessagePromptTemplate)
+from langchain.schema import LLMResult, SystemMessage
 
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
     template="Summarize and provide direct quotes from the text below to help answer a question. "
     "Do not directly answer the question, instead summarize and "
     "quote to give evidence to help answer the question. "
     "Do not use outside sources. "
@@ -69,22 +73,34 @@
     input_variables=["text"],
     template="Provide a possible citation for the following text in MLA Format. Today's date is {date}\n"
     "{text}\n\n"
     "Citation:",
     partial_variables={"date": _get_datetime},
 )
 
-def make_chain(prompt, llm, callback_manager=None):
-    if callback_manager is not None:
-        # need to clone to attach
-        llm = llm.copy()
-        llm.callback_manager = callback_manager
+
+class FallbackLLMChain(LLMChain):
+    """Chain that falls back to synchronous generation if the async generation fails."""
+
+    async def agenerate(
+        self,
+        input_list: List[Dict[str, Any]],
+        run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
+    ) -> LLMResult:
+        """Generate LLM result from inputs."""
+        try:
+            return await super().agenerate(input_list, run_manager=run_manager)
+        except NotImplementedError as e:
+            return self.generate(input_list, run_manager=run_manager)
+
+
+def make_chain(prompt, llm):
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
             content="You are a scholarly researcher that answers in an unbiased, scholarly tone. "
             "You sometimes refuse to answer if there is insufficient information.",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
         prompt = ChatPromptTemplate.from_messages(
             [system_message_prompt, human_message_prompt]
         )
-    return LLMChain(prompt=prompt, llm=llm)
+    return FallbackLLMChain(prompt=prompt, llm=llm)
```

### Comparing `paper-qa-1.3.0/paperqa/readers.py` & `paper-qa-1.4.0/paperqa/readers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import os
-from .paths import OCR_CACHE_PATH
-from .version import __version__
-from html2text import html2text
-from pathlib import Path
 import json
 import logging
+import os
 from hashlib import md5
+from pathlib import Path
 
-from langchain.text_splitter import TokenTextSplitter
+from html2text import html2text
 from langchain.cache import SQLiteCache
 from langchain.schema import Generation
+from langchain.text_splitter import TokenTextSplitter
+
+from .paths import OCR_CACHE_PATH
+from .version import __version__
 
 OCR_CACHE = None
 
 
 def _get_ocr_cache() -> SQLiteCache:
     """Used to lazily create the cache directory and cache object."""
     global OCR_CACHE
@@ -65,15 +66,14 @@
             )
         )
     pdfFileObj.close()
     return splits, metadatas
 
 
 def parse_txt(path, citation, key, chunk_chars=2000, overlap=50, html=False):
-
     try:
         with open(path) as f:
             doc = f.read()
     except UnicodeDecodeError:
         with open(path, encoding="utf-8", errors="ignore") as f:
             doc = f.read()
     if html:
```

### Comparing `paper-qa-1.3.0/paperqa/types.py` & `paper-qa-1.4.0/paperqa/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Union, List, Dict, Any
-from pathlib import Path
 from dataclasses import dataclass
+from pathlib import Path
+from typing import Any, Dict, List, Union
 
 StrPath = Union[str, Path]
 
 
 @dataclass
 class Answer:
     """A class to hold the answer to a question."""
```

### Comparing `paper-qa-1.3.0/paperqa/utils.py` & `paper-qa-1.4.0/paperqa/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 import string
+
 import pypdf
 
 from .types import StrPath
 
 
 def maybe_is_text(s, thresh=2.5):
     if len(s) == 0:
```

### Comparing `paper-qa-1.3.0/setup.py` & `paper-qa-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
     license="MIT",
     packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
-        "langchain>=0.0.129",
+        "langchain>=0.0.157",
         "openai>=0.27.0",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
-        "rmrkl"
+        "rmrkl>=0.0.2",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `paper-qa-1.3.0/tests/test_paperqa.py` & `paper-qa-1.4.0/tests/test_paperqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import paperqa
-import requests
 import os
 import pickle
-from paperqa.utils import strings_similarity
+from unittest import IsolatedAsyncioTestCase
+
+import requests
 from langchain.llms import OpenAI
 from langchain.llms.fake import FakeListLLM
-from unittest import IsolatedAsyncioTestCase
+
+import paperqa
+from paperqa.utils import strings_similarity
 
 
 def test_maybe_is_text():
     assert paperqa.maybe_is_text(
         "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
     )
     assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
@@ -249,31 +251,34 @@
         "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
     )
     # add with new dockey
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = docs.query("What country is Bates from?", key_filter=True)
     # the filter shouldn't trigger, so just checking that it doesn't crash
 
+
 def test_nonopenai_model():
-    responses = ["This is a test", "This is another test"]
+    responses = ["This is a test", "This is another test"] * 50
     model = FakeListLLM(responses=responses)
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=model)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query("What country is Bates from?")
 
+
 def test_agent():
     docs = paperqa.Docs()
     answer = paperqa.run_agent(docs, "What compounds target AKT1")
     print(answer)
 
+
 def test_zotera():
     from paperqa.contrib import ZoteroDB
 
     docs = paperqa.Docs()
     try:
         zotero = ZoteroDB(library_type="user")  # "group" if group library
     except ValueError:
```

