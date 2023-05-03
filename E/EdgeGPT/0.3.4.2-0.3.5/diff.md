# Comparing `tmp/EdgeGPT-0.3.4.2.tar.gz` & `tmp/EdgeGPT-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.4.2.tar", last modified: Tue May  2 07:38:44 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.5.tar", last modified: Wed May  3 10:12:11 2023, max compression
```

## Comparing `EdgeGPT-0.3.4.2.tar` & `EdgeGPT-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:38:44.794526 EdgeGPT-0.3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 07:38:13.000000 EdgeGPT-0.3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 07:38:44.794526 EdgeGPT-0.3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 07:38:44.794526 EdgeGPT-0.3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-02 07:38:13.000000 EdgeGPT-0.3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:38:44.790526 EdgeGPT-0.3.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:38:44.794526 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:38:44.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28345 2023-05-02 07:38:13.000000 EdgeGPT-0.3.4.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 07:38:13.000000 EdgeGPT-0.3.4.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-03 10:12:10.000000 EdgeGPT-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29462 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.4.2/LICENSE` & `EdgeGPT-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.4.2/PKG-INFO` & `EdgeGPT-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.4.2
+Version: 0.3.5
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4.2 Summary: Reverse
-engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
-General Public License v2.0 Project-URL: Bug Report, https://github.com/
-acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
-Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.5 Summary: Reverse engineered
+Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
+Cheong Author-email: acheong@student.dalat.org License: GNU General Public
+License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
     version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
                              EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
```

### Comparing `EdgeGPT-0.3.4.2/README.md` & `EdgeGPT-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.4.2/setup.py` & `EdgeGPT-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.4.2",
+    version="0.3.5",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.4.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.5/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.4.2
+Version: 0.3.5
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4.2 Summary: Reverse
-engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
-General Public License v2.0 Project-URL: Bug Report, https://github.com/
-acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
-Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.5 Summary: Reverse engineered
+Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
+Cheong Author-email: acheong@student.dalat.org License: GNU General Public
+License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
     version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
                              EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
```

### Comparing `EdgeGPT-0.3.4.2/src/EdgeGPT.py` & `EdgeGPT-0.3.5/src/EdgeGPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
+        search_result: bool = False 
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -256,14 +257,17 @@
                     "conversationId": self.conversation_id,
                 },
             ],
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
+        if search_result:
+            have_search_result = ["InternalSearchQuery","InternalSearchResult","InternalLoaderMessage","RenderCardRequest"]
+            self.struct["arguments"][0]["allowedMessageTypes"]+=have_search_result
         if webpage_context:
             self.struct["arguments"][0]["previousMessages"] = [
                 {
                     "author": "user",
                     "description": webpage_context,
                     "contextType": "WebPage",
                     "messageType": "Context",
@@ -411,14 +415,15 @@
         prompt: str,
         wss_link: str,
         cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
+        search_result : bool = False
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
@@ -432,14 +437,15 @@
         if self.request.invocation_id == 0:
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
                 options=options,
                 webpage_context=webpage_context,
+                search_result=search_result
             )
         else:
             async with httpx.AsyncClient() as client:
                 response = await client.post(
                     "https://sydney.bing.com/sydney/UpdateConversation/",
                     json={
                         "messages": [
@@ -469,14 +475,15 @@
                 options=options,
             )
         # Send request
         await self.wss.send(_append_identifier(self.request.struct))
         final = False
         draw = False
         resp_txt = ""
+        result_text = ""
         resp_txt_no_link = ""
         while not final:
             objects = str(await self.wss.recv()).split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
@@ -487,20 +494,27 @@
                 ):
                     try:
                         if not draw:
                             if (
                                 response["arguments"][0]["messages"][0]["contentOrigin"]
                                 != "Apology"
                             ):
-                                resp_txt = response["arguments"][0]["messages"][0][
+                                resp_txt = result_text+response["arguments"][0]["messages"][0][
                                     "adaptiveCards"
                                 ][0]["body"][0].get("text", "")
-                                resp_txt_no_link = response["arguments"][0]["messages"][
+                                resp_txt_no_link = result_text+response["arguments"][0]["messages"][
                                     0
                                 ].get("text", "")
+                                if(response["arguments"][0]["messages"][0].get("messageType")):
+                                    resp_txt = resp_txt+response["arguments"][0]["messages"][0][
+                                    "adaptiveCards"
+                                    ][0]["body"][0]["inlines"][0].get("text")+"\n"
+                                    result_text = result_text+response["arguments"][0]["messages"][0][
+                                    "adaptiveCards"
+                                    ][0]["body"][0]["inlines"][0].get("text")+"\n"
                         yield False, resp_txt
                     except Exception as exc:
                         print(exc)
                         if not draw:
                             continue
                         for item in cookies:
                             if item["name"] == "_U":
@@ -609,51 +623,55 @@
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         options: dict = None,
         webpage_context: str | None = None,
+        search_result: bool = False
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
             cookies=self.cookies,
             webpage_context=webpage_context,
+            search_result=search_result
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return None
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
+        search_result: str = False
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
             cookies=self.cookies,
             webpage_context=webpage_context,
+            search_result=search_result
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
```

