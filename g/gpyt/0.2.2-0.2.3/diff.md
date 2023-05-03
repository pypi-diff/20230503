# Comparing `tmp/gpyt-0.2.2.tar.gz` & `tmp/gpyt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.2.tar", max compression
+gzip compressed data, was "gpyt-0.2.3.tar", max compression
```

## Comparing `gpyt-0.2.2.tar` & `gpyt-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      836 2023-05-03 04:02:05.947304 gpyt-0.2.2/README.md
--rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.2/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.2/gpyt/__main__.py
--rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.2/gpyt/_app.py
--rw-r--r--   0        0        0     4150 2023-05-03 03:53:32.417304 gpyt-0.2.2/gpyt/app.py
--rw-r--r--   0        0        0     2012 2023-05-03 03:53:32.417304 gpyt-0.2.2/gpyt/assistant.py
--rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.2/gpyt/debug.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.2/gpyt/exception.py
--rw-r--r--   0        0        0      736 2023-05-03 03:53:32.417304 gpyt-0.2.2/gpyt/styles.cssx
--rw-r--r--   0        0        0      427 2023-05-03 04:02:24.337304 gpyt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 gpyt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-05-03 04:06:01.897304 gpyt-0.2.3/README.md
+-rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.3/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.3/gpyt/__main__.py
+-rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.3/gpyt/_app.py
+-rw-r--r--   0        0        0     4641 2023-05-03 06:34:17.987304 gpyt-0.2.3/gpyt/app.py
+-rw-r--r--   0        0        0     2044 2023-05-03 06:34:17.987304 gpyt-0.2.3/gpyt/assistant.py
+-rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.3/gpyt/debug.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.3/gpyt/exception.py
+-rw-r--r--   0        0        0      780 2023-05-03 06:34:17.987304 gpyt-0.2.3/gpyt/styles.cssx
+-rw-r--r--   0        0        0      427 2023-05-03 06:34:17.987304 gpyt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 gpyt-0.2.3/PKG-INFO
```

### Comparing `gpyt-0.2.2/gpyt/__init__.py` & `gpyt-0.2.3/gpyt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.2/gpyt/_app.py` & `gpyt-0.2.3/gpyt/_app.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.2/gpyt/app.py` & `gpyt-0.2.3/gpyt/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from assistant import Assistant
 from gpyt import API_KEY, ARGS, INTRO, MODEL, PROMPT
+from typing import Generator
 
+from textual import work
 from textual.app import App, ComposeResult
 from textual.containers import ScrollableContainer, Container
 from textual.reactive import reactive
 from textual.widgets import (
     Button,
     Footer,
     Header,
-    LoadingIndicator,
     Markdown,
     Static,
     Label,
     Input,
 )
 
 
@@ -23,59 +24,74 @@
         yield Label(f"🤖: {INTRO}", id="help-text")
         yield Input(placeholder="How far away is the Sun?", id="user-input")
         # yield Button("Submit", variant="success", id="submit")
 
     async def on_input_submitted(self, event: Input.Submitted) -> None:
         user_input = event.input.value
         event.input.value = ""
-        # await self.run_action(f"app.action_fetch_assistant_response('{user_input}')")
-        await app.fetch_assistant_response(user_input)
+        app.fetch_assistant_response(user_input)
 
 
 class AssistantResponse(Static):
     """
     Each User/Assistant interaction
-
-    is_dummy indicates that this widget is soon to be removed from the dom
-    and is being used purely for the loading indicator while awaiting assistant
-    response.
     """
 
-    def __init__(self, markdown: str = "", question: str = "", is_dummy=False):
+    def __init__(self, question: str = ""):
         super().__init__()
-        self.markdown = markdown
         self.question = question
-        self.loading_indicator = LoadingIndicator() if is_dummy else Label()
+        self.response_view = Markdown()
 
     def compose(self) -> ComposeResult:
-        yield Label(f"😀: {self.question}", classes="convo")
+        self.user_question = Label(f"😀: {self.question}", classes="convo")
+        yield self.user_question
         yield Label("🤖:", classes="convo")
-        response_view = Markdown(self.markdown)
-        container = Container(
-            response_view, self.loading_indicator, id="response-container"
-        )
+        container = Container(self.response_view, id="response-container")
         container.border_subtitle = "message-id: 0x18239123"
         yield container
 
+    @work()
+    def update_response(self, content: str) -> None:
+        app.call_from_thread(self.response_view.update, content)
+        # self.response_view.update(content)
+
 
 class AssistantResponses(Static):
     """Container for individual AssistantResponse widgets"""
 
     def compose(self) -> ComposeResult:
         self.container = ScrollableContainer()
 
         yield self.container
 
-    def add_response(
-        self, markdown: str, question: str, dummy_response: AssistantResponse
-    ) -> None:
-        new_response = AssistantResponse(markdown=markdown, question=question)
-        self.container.mount(new_response)
-        dummy_response.remove()
-        new_response.scroll_visible()
+    @work()
+    def add_response(self, stream: Generator, question: str) -> None:
+        new_response = AssistantResponse(question=question)
+        app.call_from_thread(self.container.mount, new_response)
+        app.call_from_thread(new_response.scroll_visible)
+        markdown = ""
+        update_frequency = 10
+        i = 0
+        for data in stream:
+            i += 1
+            try:  # HACK: should check for attr, not try/except
+                markdown = markdown + data["choices"][0]["delta"]["content"]
+                if i % update_frequency == 0:
+                    app.call_from_thread(new_response.update_response, markdown)
+                    app.call_from_thread(self.container.scroll_end)
+            except:
+                continue
+
+        app.call_from_thread(new_response.update_response, markdown)
+        # app.call_from_thread(self.container.scroll_page_up)
+        app.call_from_thread(
+            new_response.user_question.scroll_visible, duration=2, easing="out_back"
+        )
+        app.assistant.log_assistant_response(markdown)
+        print("scrolling up")
 
 
 class AssistantApp(App):
     """Base app for all user->assistant interactions"""
 
     BINDINGS = [("ctrl+b", "toggle_dark", "Toggle Dark Mode")]
 
@@ -94,23 +110,26 @@
         self.assistant_responses.border_title = "Conversation History"
         user_input = UserInput()
         user_input.border_subtitle = "Press Enter To Submit"
         # yield ScrollableContainer(user_input, assistant_responses)
         yield user_input
         yield self.assistant_responses
 
-    async def fetch_assistant_response(self, user_input: str) -> None:
-        dummy_assistant_response = AssistantResponse(question=user_input, is_dummy=True)
-        self.assistant_responses.container.mount(dummy_assistant_response)
-        dummy_assistant_response.scroll_visible()
-        assistant_response_markdown = await self.assistant.get_response(user_input)
-        self.assistant_responses.add_response(
-            markdown=assistant_response_markdown,
+    def test(self, x: int) -> int:
+        return x + 4
+
+    @work()
+    def fetch_assistant_response(self, user_input: str) -> None:
+        # self.run_worker(self.assistant.get_response_stream(user_input))
+        assistant_response_stream = self.assistant.get_response_stream(user_input)
+
+        app.call_from_thread(
+            self.assistant_responses.add_response,
             question=user_input,
-            dummy_response=dummy_assistant_response,
+            stream=assistant_response_stream,
         )
 
     def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
 
 class gpyt(AssistantApp):
```

### Comparing `gpyt-0.2.2/gpyt/assistant.py` & `gpyt-0.2.3/gpyt/assistant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import openai_async
-import asyncio
+import openai
+from typing import Generator
 
 
 class Assistant:
     """
     Represents an OpenAI GPT assistant.
 
     It can generate responses based on user input and conversation history.
@@ -13,54 +13,58 @@
         self.api_key = api_key
         self.model = model
         self.prompt = prompt
         self.memory = memory
         self.messages = [
             {"role": "system", "content": self.prompt},
         ]
+        openai.api_key = self.api_key
 
     def clear_history(self):
         """
         Wipe all message history during this conversation, except for the
         first system message
         """
         self.messages = [self.messages[0]]
 
-    async def get_response(self, user_input: str) -> str:
+    def get_response_stream(self, user_input: str) -> Generator:
         """
         Use OpenAI API to retrieve a ChatCompletion response from a GPT model.
 
         Memory can be configured so that the assistant forgets previous messages
         you or it has sent. (saves tokens ($$$) as well)
         """
         if not self.memory:
             self.clear_history()
         self.messages.append({"role": "user", "content": user_input})
 
-        try:
-            response = await openai_async.chat_complete(  # type: ignore
-                api_key=self.api_key,
-                timeout=30,
-                payload={"model": self.model, "messages": self.messages},
-            )
-        except:
-            return "Could not generate Assistant completion. Ensure you've configured an API_KEY and are connected to the internet! This could also be due to a timeout, check your latency to openai!"
+        response = openai.ChatCompletion.create(  # type: ignore
+            model=self.model,
+            messages=self.messages,
+            stream=True,
+        )
 
-        message = response.json()["choices"][0]["message"]
+        return response  # type: ignore
 
-        if self.memory:
-            self.messages.append(message)
+    def log_assistant_response(self, final_response: str) -> None:
+        if not self.memory:
+            return
 
-        return message["content"]
+        self.messages.append({"role": "assistant", "content": final_response})
 
 
-async def _test() -> None:
+def _test() -> None:
     from gpyt import API_KEY, MODEL, PROMPT
 
     gpt = Assistant(api_key=API_KEY or "", model=MODEL, prompt=PROMPT)
 
-    response = await gpt.get_response("Hi, how are you!")
-    print(response)
+    # response = gpt.get_response("Hi, how are you!")
+    response_iterator = gpt.get_response_stream("hi how are you!")
+    for response in response_iterator:
+        try:
+            print(response["choices"][0]["delta"]["content"], end="", flush=True)
+        except:
+            continue
 
 
 if __name__ == "__main__":
-    asyncio.run(_test())
+    _test()
```

### Comparing `gpyt-0.2.2/gpyt/styles.cssx` & `gpyt-0.2.3/gpyt/styles.cssx`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+* {
+  transition: color 1000ms in_quint;
+}
+
 Screen {
   overflow: hidden;
 }
 
 UserInput {
   border: panel $primary-background;
   background: $surface-lighten-1;
```

### Comparing `gpyt-0.2.2/PKG-INFO` & `gpyt-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.2
+Version: 0.2.3
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
@@ -12,15 +12,15 @@
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: textual[dev] (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
-Interact with GPT on the command line.
+TUI GPT frontend on the command line with Textual.
 
 > WIP
 
 
 ## Demo
 
 ![gpyt demo](./media/gpyt-show-1.gif)
@@ -35,24 +35,24 @@
 add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
 $ python -m gpyt
 ```
 
 ### Desired Features
 
-* `copy` to copy GPT's response to clipboard
-* add gpt jailbreaks (DAN-esque)
-* `new` to start a new chat (clear all history and console window)
-* store chat logs somewhere.
-* add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
-  (informal) or -f (for file input) or --dan (for jailbreak)
-* scrolling text (adjustable speed, or disable all together)
-* use streams api?
-* model select CLI
-* add API_KEY from CLI
+- [ ] `copy` to copy GPT's response to clipboard
+- [ ] add gpt jailbreaks (DAN-esque)
+- [ ] `new` to start a new chat (clear all history and console window)
+- [ ] store chat logs somewhere.
+- [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
+- [ ] (informal) or -f (for file input) or --dan (for jailbreak)
+- [ ] scrolling text (adjustable speed, or disable all together)
+- [ ] use streams api?
+- [ ] model select CLI
+- [ ] add API_KEY from CLI
 
 
 ### Completed Features
 
-[x] loading wheel
-[x] textual !!!
+- [x] loading wheel
+- [x] textual !!!
```

