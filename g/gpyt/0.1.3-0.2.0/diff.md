# Comparing `tmp/gpyt-0.1.3.tar.gz` & `tmp/gpyt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.1.3.tar", max compression
+gzip compressed data, was "gpyt-0.2.0.tar", max compression
```

## Comparing `gpyt-0.1.3.tar` & `gpyt-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      657 2023-05-01 23:17:49.417304 gpyt-0.1.3/README.md
--rw-r--r--   0        0        0     1351 2023-05-02 00:03:47.517304 gpyt-0.1.3/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.1.3/gpyt/__main__.py
--rw-r--r--   0        0        0     1863 2023-05-01 23:46:09.787304 gpyt-0.1.3/gpyt/app.py
--rw-r--r--   0        0        0     1558 2023-05-02 00:00:28.177304 gpyt-0.1.3/gpyt/assistant.py
--rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.1.3/gpyt/debug.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.1.3/gpyt/exception.py
--rw-r--r--   0        0        0      353 2023-05-02 00:04:48.157304 gpyt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 gpyt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-05-03 03:53:32.417304 gpyt-0.2.0/README.md
+-rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.0/gpyt/__main__.py
+-rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/_app.py
+-rw-r--r--   0        0        0     4150 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/app.py
+-rw-r--r--   0        0        0     2012 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/assistant.py
+-rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.0/gpyt/debug.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.0/gpyt/exception.py
+-rw-r--r--   0        0        0      736 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/styles.cssx
+-rw-r--r--   0        0        0      427 2023-05-03 03:53:32.417304 gpyt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 gpyt-0.2.0/PKG-INFO
```

### Comparing `gpyt-0.1.3/README.md` & `gpyt-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 > WIP
 
 ### How to run:
 ```sh
 $ pip install gpyt
 
-add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME
+add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
 $ python -m gpyt
 ```
 
 ### Desired Features
 * `copy` to copy GPT's response to clipboard
 * color coded responses
@@ -22,7 +22,8 @@
 * store chat logs somewhere.
 * add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
   (informal) or -f (for file input) or --dan (for jailbreak)
 * scrolling text (adjustable speed, or disable all together)
 * use streams api?
 * model select CLI
 * loading wheel
+* textual !!!
```

### Comparing `gpyt-0.1.3/gpyt/app.py` & `gpyt-0.2.0/gpyt/_app.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.1.3/gpyt/assistant.py` & `gpyt-0.2.0/gpyt/assistant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import openai
+import openai_async
+import asyncio
 
 
 class Assistant:
     """
     Represents an OpenAI GPT assistant.
 
     It can generate responses based on user input and conversation history.
@@ -12,38 +13,54 @@
         self.api_key = api_key
         self.model = model
         self.prompt = prompt
         self.memory = memory
         self.messages = [
             {"role": "system", "content": self.prompt},
         ]
-        openai.api_key = self.api_key
 
     def clear_history(self):
         """
         Wipe all message history during this conversation, except for the
         first system message
         """
         self.messages = [self.messages[0]]
 
-    def get_response(self, user_input: str) -> str:
+    async def get_response(self, user_input: str) -> str:
         """
         Use OpenAI API to retrieve a ChatCompletion response from a GPT model.
 
         Memory can be configured so that the assistant forgets previous messages
         you or it has sent. (saves tokens ($$$) as well)
         """
         if not self.memory:
             self.clear_history()
         self.messages.append({"role": "user", "content": user_input})
 
         try:
-            response = openai.ChatCompletion.create(  # type: ignore
-                model=self.model, messages=self.messages
-            )["choices"][0]["message"]
+            response = await openai_async.chat_complete(  # type: ignore
+                api_key=self.api_key,
+                timeout=30,
+                payload={"model": self.model, "messages": self.messages},
+            )
         except:
-            return "Could not generate Assistant completion. Ensure you've configured an API_KEY and are connected to the internet!"
+            return "Could not generate Assistant completion. Ensure you've configured an API_KEY and are connected to the internet! This could also be due to a timeout, check your latency to openai!"
+
+        message = response.json()["choices"][0]["message"]
 
         if self.memory:
-            self.messages.append(response)
+            self.messages.append(message)
+
+        return message["content"]
+
+
+async def _test() -> None:
+    from gpyt import API_KEY, MODEL, PROMPT
+
+    gpt = Assistant(api_key=API_KEY or "", model=MODEL, prompt=PROMPT)
+
+    response = await gpt.get_response("Hi, how are you!")
+    print(response)
+
 
-        return response["content"]
+if __name__ == "__main__":
+    asyncio.run(_test())
```

### Comparing `gpyt-0.1.3/PKG-INFO` & `gpyt-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.1.3
+Version: 0.2.0
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: openai-async (>=0.0.3,<0.0.4)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: textual[dev] (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
 Interact with GPT on the command line.
 
 
 > WIP
 
 ### How to run:
 ```sh
 $ pip install gpyt
 
-add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME
+add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
 $ python -m gpyt
 ```
 
 ### Desired Features
 * `copy` to copy GPT's response to clipboard
 * color coded responses
@@ -36,8 +38,9 @@
 * store chat logs somewhere.
 * add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
   (informal) or -f (for file input) or --dan (for jailbreak)
 * scrolling text (adjustable speed, or disable all together)
 * use streams api?
 * model select CLI
 * loading wheel
+* textual !!!
```

