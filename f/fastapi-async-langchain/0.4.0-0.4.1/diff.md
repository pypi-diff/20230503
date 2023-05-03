# Comparing `tmp/fastapi_async_langchain-0.4.0.tar.gz` & `tmp/fastapi_async_langchain-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.4.1.tar", max compression
```

## Comparing `fastapi_async_langchain-0.4.0.tar` & `fastapi_async_langchain-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-05-02 17:40:12.617572 fastapi_async_langchain-0.4.0/LICENSE
--rw-r--r--   0        0        0     1713 2023-05-02 17:40:12.617572 fastapi_async_langchain-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-02 17:40:12.821570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      509 2023-05-02 17:40:12.821570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      273 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/__init__.py
--rw-r--r--   0        0        0      784 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/base.py
--rw-r--r--   0        0        0      906 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py
--rw-r--r--   0        0        0      257 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/__init__.py
--rw-r--r--   0        0        0      971 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/base.py
--rw-r--r--   0        0        0     1172 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py
--rw-r--r--   0        0        0      171 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2502 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0     1295 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0     2225 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      536 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0      281 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     2907 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0     1379 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/llm.py
--rw-r--r--   0        0        0     2370 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/retrieval_qa.py
--rw-r--r--   0        0        0      481 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-03 09:40:30.718850 fastapi_async_langchain-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1713 2023-05-03 09:40:30.718850 fastapi_async_langchain-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/base.py
+-rw-r--r--   0        0        0      896 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py
+-rw-r--r--   0        0        0      257 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/base.py
+-rw-r--r--   0        0        0     1178 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py
+-rw-r--r--   0        0        0      171 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2502 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0      725 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0      782 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      536 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0      281 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     2907 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      927 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/llm.py
+-rw-r--r--   0        0        0      985 2023-05-03 09:40:30.902850 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/retrieval_qa.py
+-rw-r--r--   0        0        0      481 2023-05-03 09:40:30.902850 fastapi_async_langchain-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.1/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.4.0/LICENSE` & `fastapi_async_langchain-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/README.md` & `fastapi_async_langchain-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/base.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict
 
-from .base import AsyncStreamingResponseCallback
+from .base import AsyncLLMChainStreamingCallback
 
 SOURCE_DOCUMENT_TEMPLATE = """
 page content: {page_content}
 source: {source}
 """
 
 
-class AsyncRetrievalQAStreamingCallback(AsyncStreamingResponseCallback):
+class AsyncRetrievalQAStreamingCallback(AsyncLLMChainStreamingCallback):
     """AsyncStreamingResponseCallback handler for RetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
-        if outputs["source_documents"] is not None:
+        if "source_documents" in outputs:
             await self.send("\n\nSOURCE DOCUMENTS: \n")
             for document in outputs["source_documents"]:
                 await self.send(
                     self.source_document_template.format(
                         page_content=document.page_content,
                         source=document.metadata["source"],
                     )
```

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/base.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Any, Dict
 
 from ..streaming.retrieval_qa import SOURCE_DOCUMENT_TEMPLATE
-from .base import AsyncWebsocketCallback
+from .base import AsyncLLMChainWebsocketCallback
 
 
-class AsyncRetrievalQAWebsocketCallback(AsyncWebsocketCallback):
+class AsyncRetrievalQAWebsocketCallback(AsyncLLMChainWebsocketCallback):
     """AsyncWebsocketCallback handler for RetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
-        if outputs["source_documents"] is not None:
+        if "source_documents" in outputs:
             await self.websocket.send_json(
                 {
                     **self.response.dict(),
                     **{"message": "\n\nSOURCE DOCUMENTS: \n"},
                 }
             )
             for document in outputs["source_documents"]:
```

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/base.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/llm.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 from typing import Any, Awaitable, Callable, Dict, Union
 
 from langchain import LLMChain
-from langchain.callbacks import AsyncCallbackManager
 from starlette.types import Send
 
-from ..callbacks import AsyncLLMChainStreamingCallback, AsyncStreamingResponseCallback
+from ..callbacks import AsyncLLMChainStreamingCallback
 from .base import BaseLangchainStreamingResponse
 
 
 class LLMChainStreamingResponse(BaseLangchainStreamingResponse):
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
     def _create_chain_executor(
         chain: LLMChain, inputs: Union[Dict[str, Any], Any]
     ) -> Callable[[Send], Awaitable[Any]]:
         async def wrapper(send: Send):
-            if not isinstance(chain.llm.callback_manager, AsyncCallbackManager):
-                raise TypeError(
-                    "llm.callback_manager must be an instance of AsyncCallbackManager"
-                )
-            for handler in chain.llm.callback_manager.handlers:
-                if isinstance(handler, AsyncStreamingResponseCallback):
-                    chain.llm.callback_manager.remove_handler(handler)
-                    break
-            chain.llm.callback_manager.add_handler(
-                AsyncLLMChainStreamingCallback(send=send)
+            return await chain.arun(
+                input=inputs, callbacks=[AsyncLLMChainStreamingCallback(send=send)]
             )
-            return await chain.arun(inputs)
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/llm.py` & `fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/llm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 from typing import Any, Awaitable, Callable
 
 from fastapi import WebSocket
 from langchain import LLMChain
-from langchain.callbacks import AsyncCallbackManager
 
-from ..callbacks import AsyncLLMChainWebsocketCallback, AsyncWebsocketCallback
+from ..callbacks import AsyncLLMChainWebsocketCallback
 from ..schemas import WebsocketResponse
 from .base import BaseLangchainWebsocketConnection
 
 
 class LLMChainWebsocketConnection(BaseLangchainWebsocketConnection):
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
     def _create_chain_executor(
         chain: LLMChain,
         websocket: WebSocket,
         response: WebsocketResponse,
     ) -> Callable[[], Awaitable[Any]]:
         async def wrapper(user_message: str):
-            if not isinstance(chain.llm.callback_manager, AsyncCallbackManager):
-                raise TypeError(
-                    "llm.callback_manager must be an instance of AsyncCallbackManager"
-                )
-            for handler in chain.llm.callback_manager.handlers:
-                if isinstance(handler, AsyncWebsocketCallback):
-                    chain.llm.callback_manager.remove_handler(handler)
-                    break
-            chain.llm.callback_manager.add_handler(
-                AsyncLLMChainWebsocketCallback(websocket=websocket, response=response)
+            return await chain.arun(
+                inputs=user_message,
+                callbacks=[
+                    AsyncLLMChainWebsocketCallback(
+                        websocket=websocket, response=response
+                    )
+                ],
             )
-            return await chain.arun(user_message)
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.4.0/PKG-INFO` & `fastapi_async_langchain-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.4.0
+Version: 0.4.1
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: langchain (>=0.0.146,<0.0.147)
+Requires-Dist: langchain (>=0.0.157,<0.0.158)
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
```

