# Comparing `tmp/promptwatch-0.0.3.tar.gz` & `tmp/promptwatch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.3.tar", last modified: Tue May  2 18:40:25 2023, max compression
+gzip compressed data, was "promptwatch-0.0.4.tar", last modified: Wed May  3 12:44:13 2023, max compression
```

## Comparing `promptwatch-0.0.3.tar` & `promptwatch-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.639824 promptwatch-0.0.3/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-05-02 18:40:25.639650 promptwatch-0.0.3/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3781 2023-04-21 05:55:12.000000 promptwatch-0.0.3/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.3/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-02 18:40:25.639868 promptwatch-0.0.3/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 11:55:00.000000 promptwatch-0.0.3/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.632914 promptwatch-0.0.3/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.637036 promptwatch-0.0.3/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-02 18:40:10.000000 promptwatch-0.0.3/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 08:57:06.000000 promptwatch-0.0.3/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.3/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.638902 promptwatch-0.0.3/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-02 10:03:23.000000 promptwatch-0.0.3/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34206 2023-05-02 18:26:30.000000 promptwatch-0.0.3/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13397 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 17:20:28.000000 promptwatch-0.0.3/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.638362 promptwatch-0.0.3/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.3/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.764048 promptwatch-0.0.4/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-03 12:44:13.763905 promptwatch-0.0.4/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.4/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.4/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-03 12:44:13.764086 promptwatch-0.0.4/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.4/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.761187 promptwatch-0.0.4/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.762681 promptwatch-0.0.4/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-03 12:43:27.000000 promptwatch-0.0.4/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.4/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.763678 promptwatch-0.0.4/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.4/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    31533 2023-05-03 12:39:13.000000 promptwatch-0.0.4/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13397 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.763388 promptwatch-0.0.4/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.4/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.3/PKG-INFO` & `promptwatch-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.3
+Version: 0.0.4
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
@@ -70,15 +70,15 @@
 👉 Details about LLM runs like:
 
   - final prompt text
   - generated text
   - execution details like model, temperature, etc. (everything you need to re-run the prompt with the same exact setup)
   - total used tokens
   - **costs (based on OpenAI price list per model)**
-  - **prompt template and it's parameters**
+  - **prompt template and its parameters**
   
  
 
 ### Custom logging
 
 PromptWatch tracks quite extensively standard LangChain tools, but if you have some custom code you'd like to track you can do so.
 
@@ -101,23 +101,23 @@
 
 
 ## Prompt template tracking
 
 You can register any LangChain prompt template for detailed monitoring
 
 ```python
-from promptwatch import PromptWatch
+from promptwatch import PromptWatch, register_prompt_template
 from langchain import OpenAI, LLMChain, PromptTemplate
 
 prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
 my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
 
+register_prompt_template("your_template_name",prompt_template) 
+
 with PromptWatch() as pw:
-    # register the template for detailed tracking
-    pw.register_prompt_template("your_template_name",prompt_template) 
     
     #execute the chain
     my_chain("The quick brown fox jumped over")
 
 ```
 
 This will allow you to associate the prompt template with a custom name (and function) and track it independently...
```

### Comparing `promptwatch-0.0.3/README.md` & `promptwatch-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 👉 Details about LLM runs like:
 
   - final prompt text
   - generated text
   - execution details like model, temperature, etc. (everything you need to re-run the prompt with the same exact setup)
   - total used tokens
   - **costs (based on OpenAI price list per model)**
-  - **prompt template and it's parameters**
+  - **prompt template and its parameters**
   
  
 
 ### Custom logging
 
 PromptWatch tracks quite extensively standard LangChain tools, but if you have some custom code you'd like to track you can do so.
 
@@ -89,23 +89,23 @@
 
 
 ## Prompt template tracking
 
 You can register any LangChain prompt template for detailed monitoring
 
 ```python
-from promptwatch import PromptWatch
+from promptwatch import PromptWatch, register_prompt_template
 from langchain import OpenAI, LLMChain, PromptTemplate
 
 prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
 my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
 
+register_prompt_template("your_template_name",prompt_template) 
+
 with PromptWatch() as pw:
-    # register the template for detailed tracking
-    pw.register_prompt_template("your_template_name",prompt_template) 
     
     #execute the chain
     my_chain("The quick brown fox jumped over")
 
 ```
 
 This will allow you to associate the prompt template with a custom name (and function) and track it independently...
```

### Comparing `promptwatch-0.0.3/setup.py` & `promptwatch-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/caching.py` & `promptwatch-0.0.4/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/client.py` & `promptwatch-0.0.4/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/data_model.py` & `promptwatch-0.0.4/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/decorators.py` & `promptwatch-0.0.4/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.0.4/src/promptwatch/langchain/langchain_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -383,119 +383,65 @@
         
     
     
         
 
 
 
+class PromptWatchLlmCache(BaseCache):
 
-class _CachedLLM(LLM):
-    """Cached LLM wrapper around the actual LLM."""
-    inner_llm:Any
-    cache_namespace_key:Optional[str]
-    cache_embeddings:Optional[Embeddings]
-    token_limit:Optional[int]
-    similarity_limit:Optional[float]
+    def __init__(self, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
+        
+        self.cache_namespace_key = cache_namespace_key
+        self.cache_embeddings = cache_embeddings
+        self.similarity_limit=similarity_limit
+        
+        self.embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
 
-       
-    def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
-        super().__init__(inner_llm=inner_llm, cache_namespace_key=cache_namespace_key, cache_embeddings=cache_embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
-       
-    @property
-    def _llm_type(self) -> str:
-        """Return type of llm."""
-        return "cached-llm"
-    
-    def generate_prompt(
-        self, prompts: List[PromptValue], stop: Optional[List[str]] = None
-    ) -> LLMResult:
-        # overriding generate_prompt becasuse we want to pass down the prompts to the inner llm
+        self.token_limit=token_limit
+
+    def lookup(self, prompt: str, llm_string: str) -> Optional[List[Generation]]:
+        """Look up based on prompt and llm_string."""
         promptwatch_context = PromptWatch.get_active_instance()
+        cache_prompt_key = f"{llm_string}\n:{prompt}"
+        
         if promptwatch_context:
-            promptwatch_context.add_context(FORMATTED_PROMPT_CONTEXT_KEY, prompts)
-        return self.generate(prompts, stop=stop)
-    
-    
-    def generate(
-        self, prompts: List[PromptValue], stop: Optional[List[str]] = None
-    ) -> LLMResult:
-        """ Overriding default to skip tracing + passing down the original prompt value"""
-        output = self._generate(prompts, stop=stop)
-        return output
+            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
+            cached_res=cache.get(cache_prompt_key)
+            
+            if cached_res:         
+                return  [Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata, "_cached_result":cached_res})]
+       
+            else:
+                return None
+
     
-    async def agenerate(
-        self, prompts: List[PromptValue], stop: Optional[List[str]] = None
-    ) -> LLMResult:
-        """ Overriding default to skip tracing"""
-        output = await self._agenerate(prompts, stop=stop)
-        return output
+    def update(self, prompt: str, llm_string: str, return_val: List[Generation]) -> None:
+        """Update cache based on prompt and llm_string."""
+        
+        cached_res = return_val[0].generation_info.get("_cached_result")
+
+        
+        promptwatch_context = PromptWatch.get_active_instance()
+        cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
+        cache.add(cached_res)
+
+
+
+
     
-    def _get_from_cache(self, prompt: PromptValue, stop: Optional[List[str]] = None):
+    def clear(self, until:datetime=None) -> None:
         promptwatch_context = PromptWatch.get_active_instance()
         if promptwatch_context:
-            start_time=datetime.datetime.now(tz=datetime.timezone.utc)
-            embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
-            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
-            cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt.to_string()}" if stop else prompt.to_string()
-            cached_res = cache.get(cache_prompt_req)
-            if cached_res and promptwatch_context.langchain.langchain_callback_handler:
-                prompts_strings = [prompt.to_string() if not isinstance(prompt,str) else prompt]
-                
-                promptwatch_context.langchain.langchain_callback_handler.on_llm_start({"name":self.__class__.__name__},prompts_strings)
-                
-                #custom on_llm_end !:
-
-                #override start time with the real start time before caching
-                current_llm_prompt:LlmPrompt = promptwatch_context.current_activity
-                current_llm_prompt.start_time=start_time
-                current_llm_prompt.generated = cached_res.result
-                current_llm_prompt.metadata["cached"]=True
-                current_llm_prompt.metadata["cache_info"]=cached_res.metadata
-             
-                promptwatch_context._close_current_activity()
-
-           
-            return  cached_res, lambda cached_res,result : cache.add(cached_res, result) 
-        else:
-            return None, None
-        
-    def _call(self, prompt: Union[str, PromptValue], stop: Optional[List[str]] = None) -> str:
-        """ Implementing abstract call method."""
-        cached_res,callback=self._get_from_cache(prompt, stop=stop)
-        if not cached_res:
-            if isinstance(prompt, ChatPromptValue):
-                prompt=prompt.messages
-            elif not isinstance(prompt, str):
-                prompt=prompt.to_string()
-            self.callback_manager.on_llm_start(
-                {"name": self.__class__.__name__}, prompt_strings, verbose=self.verbose
-            )
-            res = self.inner_llm.generate([prompt], stop) #using generate because we want callbacks to be called
-            if isinstance(res ,BaseMessage):
-                res = res.content
-            if callback:
-                callback(cached_res, res)
-            return res
-        else:
-            return cached_res.result
-        
-        
-    async def _acall(self, prompt: str, stop: Optional[List[str]] = None) -> str:
-        """ Implementing abstract async call method."""
-        
-        cached_res,callback=self._get_from_cache(prompt, stop=stop)
-        if not cached_res:
-            res = await self.inner_llm._acall(prompt, stop=stop)
-            if callback:
-                callback(cached_res, res)
-            return res
+            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
+            cache.clear()
         else:
-            self.promp
-            return cached_res.result
-    
+            Client().clear(self.cache_namespace_key,until=until)
+
+
 
 
 
 
 def convert_chat_messages( msg:Union[BaseMessage, List[BaseMessage]]):
         if isinstance(msg, BaseMessage):
                 if isinstance(msg,HumanMessage):
@@ -692,14 +638,15 @@
     
     inner_llm:Any
     cache_namespace_key:Optional[str]
     cache_embeddings:Optional[Embeddings]
     token_limit:Optional[int]
     similarity_limit:Optional[float]
     def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
+        
         super().__init__(inner_llm=inner_llm, cache_namespace_key=cache_namespace_key, cache_embeddings=cache_embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
        
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "cached-chat-llm"
     
@@ -718,15 +665,15 @@
         prompt = ChatPromptValue(messages=messages).to_string()
         
         if promptwatch_context:
             
             embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
             cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
             
-            cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt.to}" if stop else prompt
+            cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt}" if stop else prompt
             cached_res = cache.get(cache_prompt_req)
            
            
             return  cached_res, lambda cached_res,result : cache.add(cached_res, result) 
         else:
             return None, None
```

### Comparing `promptwatch-0.0.3/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.4/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch/utils.py` & `promptwatch-0.0.4/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.3/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.4/src/promptwatch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.3
+Version: 0.0.4
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
@@ -70,15 +70,15 @@
 👉 Details about LLM runs like:
 
   - final prompt text
   - generated text
   - execution details like model, temperature, etc. (everything you need to re-run the prompt with the same exact setup)
   - total used tokens
   - **costs (based on OpenAI price list per model)**
-  - **prompt template and it's parameters**
+  - **prompt template and its parameters**
   
  
 
 ### Custom logging
 
 PromptWatch tracks quite extensively standard LangChain tools, but if you have some custom code you'd like to track you can do so.
 
@@ -101,23 +101,23 @@
 
 
 ## Prompt template tracking
 
 You can register any LangChain prompt template for detailed monitoring
 
 ```python
-from promptwatch import PromptWatch
+from promptwatch import PromptWatch, register_prompt_template
 from langchain import OpenAI, LLMChain, PromptTemplate
 
 prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
 my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
 
+register_prompt_template("your_template_name",prompt_template) 
+
 with PromptWatch() as pw:
-    # register the template for detailed tracking
-    pw.register_prompt_template("your_template_name",prompt_template) 
     
     #execute the chain
     my_chain("The quick brown fox jumped over")
 
 ```
 
 This will allow you to associate the prompt template with a custom name (and function) and track it independently...
```

### Comparing `promptwatch-0.0.3/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.0.4/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

