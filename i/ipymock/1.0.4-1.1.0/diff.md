# Comparing `tmp/ipymock-1.0.4.tar.gz` & `tmp/ipymock-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.0.4.tar", last modified: Sun Apr 30 09:41:14 2023, max compression
+gzip compressed data, was "ipymock-1.1.0.tar", last modified: Wed May  3 19:15:30 2023, max compression
```

## Comparing `ipymock-1.0.4.tar` & `ipymock-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.765576 ipymock-1.0.4/
--rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.4/LICENSE
--rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.4/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-04-30 09:41:14.765125 ipymock-1.0.4/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-04-30 09:39:51.000000 ipymock-1.0.4/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.761087 ipymock-1.0.4/ipymock/
--rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/__init__.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2454 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/_nbdev.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/agi.py
--rw-rw-r--   0 saintway   (501) staff       (20)    16107 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/browser.py
--rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/llm.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-30 09:39:30.000000 ipymock-1.0.4/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.763519 ipymock-1.0.4/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-30 09:41:14.764442 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.4/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/PKG-INFO
--rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/SOURCES.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/dependency_links.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.4/ipymock.egg-info/not-zip-safe
--rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/requires.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-30 09:41:14.000000 ipymock-1.0.4/ipymock.egg-info/top_level.txt
--rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-04-30 08:37:11.000000 ipymock-1.0.4/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-30 09:41:14.765661 ipymock-1.0.4/setup.cfg
--rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.4/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.325563 ipymock-1.1.0/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.1.0/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.1.0/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-05-03 19:15:30.325027 ipymock-1.1.0/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-05-03 19:12:45.000000 ipymock-1.1.0/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.319378 ipymock-1.1.0/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     3111 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18424 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.323157 ipymock-1.1.0/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.324226 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.1.0/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-05-03 19:06:22.000000 ipymock-1.1.0/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-05-03 19:15:30.325662 ipymock-1.1.0/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.1.0/setup.py
```

### Comparing `ipymock-1.0.4/LICENSE` & `ipymock-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/PKG-INFO` & `ipymock-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.4
+Version: 1.1.0
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.4/README.md` & `ipymock-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/ipymock/__init__.py` & `ipymock-1.1.0/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/ipymock/_nbdev.py` & `ipymock-1.1.0/ipymock/_nbdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,34 @@
          "handle_conversation_detail": "2_browser.ipynb",
          "start_conversation": "2_browser.ipynb",
          "generate_title": "2_browser.ipynb",
          "rename_title": "2_browser.ipynb",
          "delete_conversation": "2_browser.ipynb",
          "recover_conversation": "2_browser.ipynb",
          "clear_conversations": "2_browser.ipynb",
+         "init": "2_browser.ipynb",
+         "login": "2_browser.ipynb",
+         "open_chat": "2_browser.ipynb",
+         "remove_portal": "2_browser.ipynb",
+         "chatgpt_textbox": "2_browser.ipynb",
+         "chatgpt_streaming": "2_browser.ipynb",
+         "chatgpt_big_response": "2_browser.ipynb",
+         "chatgpt_small_response": "2_browser.ipynb",
+         "request": "2_browser.ipynb",
+         "get_last_response": "2_browser.ipynb",
+         "get_response": "2_browser.ipynb",
+         "ask": "2_browser.ipynb",
          "attrdict": "2_browser.ipynb",
          "attributize": "2_browser.ipynb",
+         "retry_on_status_code": "2_browser.ipynb",
+         "content": "2_browser.ipynb",
+         "new_id": "2_browser.ipynb",
          "delta": "2_browser.ipynb",
-         "mock_create": "2_browser.ipynb",
          "chat_delta": "2_browser.ipynb",
+         "mock_create": "2_browser.ipynb",
          "mock_chat_create": "2_browser.ipynb",
          "mock_openai": "2_browser.ipynb",
          "embeddings_model": "4_agi.ipynb",
          "mock_embed_create": "3_llm.ipynb",
          "mock_openai_embed": "3_llm.ipynb",
          "embedding_size": "4_agi.ipynb",
          "index": "4_agi.ipynb",
```

### Comparing `ipymock-1.0.4/ipymock/agi.py` & `ipymock-1.1.0/ipymock/agi.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/ipymock/browser.py` & `ipymock-1.1.0/ipymock/browser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/2_browser.ipynb (unless otherwise specified).
 
 __all__ = ['common', 'get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
-           'attrdict', 'attributize', 'delta', 'mock_create', 'chat_delta', 'mock_chat_create', 'mock_openai']
+           'init', 'login', 'open_chat', 'remove_portal', 'request', 'get_last_response', 'get_response', 'ask',
+           'attrdict', 'attributize', 'retry_on_status_code', 'content', 'new_id', 'delta', 'chat_delta', 'mock_create',
+           'mock_chat_create', 'mock_openai']
 
 # Internal Cell
 from queue import Queue
 
 class Common:
     chat_gpt_base_url = 'http://127.0.0.1:8080'
     access_token = None
@@ -21,33 +23,37 @@
     exit_for_loop_channel = Queue()
     response_text_channel = Queue()
     conversation_done_channel = Queue()
     parent_message_id = ''
     conversation_id = ''
     reload_conversations_channel = Queue()
 
+    config = {}
+    driver = None
+
 # Internal Cell
 import json, os, requests, sys, time, uuid
 
 # Cell
 common = Common()
 
 # open the JSON file and read the access_token and conversation_id
 with open(os.path.expanduser('~/.config/ipymock/config.json'), 'r') as f:
-    config = json.load(f)
-    common.access_token = config.get('access_token', None)
-    common.conversation_id = config.get('conversation_id', None)
+    common.config = json.load(f)
+    common.chat_gpt_base_url = common.config.get('chat_gpt_base_url', common.chat_gpt_base_url)
+    common.access_token = common.config.get('access_token', common.access_token)
+    common.conversation_id = common.config.get('conversation_id', common.conversation_id)
 
 # Cell
 def get_conversations():
-    response = requests.get(f'{common.chat_gpt_base_url}/conversations?offset=0&limit=100', headers = {'Authorization': common.access_token})
+    response = requests.get(f'{common.chat_gpt_base_url}/conversations?offset=0&limit=100', headers = {'Authorization': f'Bearer {common.access_token}'})
     return response.json()
 
 def get_conversation(conversation_id):
-    response = requests.get(f'{common.chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': common.access_token})
+    response = requests.get(f'{common.chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': f'Bearer {common.access_token}'})
 
     if response.status_code >= 400:
         sys.stderr.write(f'Error Status Code: {response.status_code}\n{response.text}\n')
     response.raise_for_status()
 
     conversation = response.json()
     current_node = conversation['current_node']
@@ -174,67 +180,226 @@
     else:
         common.reload_conversations_channel.put(True)
 
 def generate_title(conversation_id):
     requests.post(
         f'{common.chat_gpt_base_url}/conversation/gen_title/{conversation_id}',
         headers = {
-            'Authorization': common.access_token,
+            'Authorization': f'Bearer {common.access_token}',
             'Content-Type': 'application/json'
         },
         data = json.dumps({
             'message_id': get_conversation(conversation_id),
             'model': common.chat_gpt_model
         })
     )
 
 def rename_title(conversation_id, title):
     requests.patch(
         f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': common.access_token,
+            'Authorization': f'Bearer {common.access_token}',
             'Content-Type': 'application/json'
         },
         data = json.dumps({
             'title': title
         })
     )
 
 def delete_conversation(conversation_id):
     requests.patch(
         f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': common.access_token,
+            'Authorization': f'Bearer {common.access_token}',
             'Content-Type': 'application/json'
         },
         data=json.dumps({
             'is_visible': False
         })
     )
 
 def recover_conversation(conversation_id):
     requests.patch(
         f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': common.access_token,
+            'Authorization': f'Bearer {common.access_token}',
             'Content-Type': 'application/json'
         },
         data=json.dumps({
             'is_visible': True
         })
     )
 
 def clear_conversations():
-    requests.patch(f'{common.chat_gpt_base_url}/conversations', headers = {'Authorization': common.access_token}, data = {'is_visible': False})
+    requests.patch(f'{common.chat_gpt_base_url}/conversations', headers = {'Authorization': f'Bearer {common.access_token}'}, data = {'is_visible': False})
 
     common.conversation_id = ''
     common.parent_message_id = ''
     common.reload_conversations_channel.put(True)
 
 # Internal Cell
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support import expected_conditions
+from selenium.webdriver.support.ui import WebDriverWait
+
+import undetected_chromedriver as uc
+
+# Cell
+def init():
+    options = uc.ChromeOptions()
+    options.add_argument('--headless')
+    common.driver = uc.Chrome(options = options)
+
+    login()
+    open_chat()
+
+    global start_conversation
+    start_conversation = ask
+
+def login():
+    common.driver.get('https://chat.openai.com/auth/login')
+
+    WebDriverWait(common.driver, 5).until(
+        expected_conditions.presence_of_element_located((By.XPATH, '//*[text()="Log in"]'))
+    )
+
+    common.driver.execute_script('''
+    document.evaluate(
+      '//*[text()="Log in"]',
+      document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null
+    ).snapshotItem(0).dispatchEvent(
+      new MouseEvent('click', {
+        view: window,
+        bubbles: true,
+        cancelable: true
+      })
+    );
+    ''')
+
+    WebDriverWait(common.driver, 5).until(
+        expected_conditions.presence_of_element_located((By.XPATH, '//button[@data-provider="google"]'))
+    )
+
+    common.driver.execute_script('''
+    document.evaluate(
+      '//button[@data-provider="google"]',
+      document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null
+    ).snapshotItem(0).dispatchEvent(
+      new MouseEvent('click', {
+        view: window,
+        bubbles: true,
+        cancelable: true
+      })
+    );
+    ''')
+
+    WebDriverWait(common.driver, 5).until(
+        expected_conditions.presence_of_element_located((By.XPATH, '//input[@type="email"]'))
+    )
+
+    common.driver.execute_script(f'''
+    const google_email_input = document.evaluate('//input[@type="email"]', document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null).snapshotItem(0);
+    google_email_input.value = '{common.config['email']}';
+    google_email_input.dispatchEvent(
+      new Event('input', {{
+        view: window,
+        bubbles: true,
+        cancelable: true
+      }})
+    );
+    ''')
+
+    WebDriverWait(common.driver, 5).until(
+        expected_conditions.presence_of_element_located((By.XPATH, '//*[@id="identifierNext"]'))
+    )
+
+    common.driver.execute_script('''
+    document.evaluate(
+      '//*[@id="identifierNext"]',
+      document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null
+    ).snapshotItem(0).dispatchEvent(
+      new MouseEvent('click', {
+        view: window,
+        bubbles: true,
+        cancelable: true
+      })
+    );
+    ''')
+
+    WebDriverWait(common.driver, 5).until(
+        expected_conditions.element_to_be_clickable((By.XPATH, '//input[@type="password"]'))
+    ).click()
+
+    ActionChains(common.driver).send_keys(common.config['password']).send_keys(Keys.ENTER).perform()
+
+    remove_portal()
+
+def open_chat():
+    common.driver.get(f'https://chat.openai.com/c/{common.config["conversation_id"]}')
+    remove_portal()
+
+def remove_portal():
+    WebDriverWait(common.driver, 10).until(
+        expected_conditions.presence_of_element_located((By.ID, 'headlessui-portal-root'))
+    )
+
+    common.driver.execute_script('''
+    document.getElementById('headlessui-portal-root').remove();
+    ''')
+
+# Internal Cell
+chatgpt_textbox = (By.TAG_NAME, 'textarea')
+chatgpt_streaming = (By.CLASS_NAME, 'result-streaming')
+chatgpt_big_response = (By.XPATH, '//div[@class="flex-1 overflow-hidden"]//div[p]')
+chatgpt_small_response = (By.XPATH, '//div[starts-with(@class, "markdown prose w-full break-words")]')
+
+# Cell
+def request(prompt: str) -> None:
+    textbox = WebDriverWait(common.driver, 5).until(
+        expected_conditions.element_to_be_clickable(chatgpt_textbox)
+    )
+    textbox.click()
+    common.driver.execute_script('''
+var element = arguments[0], txt = arguments[1];
+element.value += txt;
+element.dispatchEvent(new Event("change"));
+''',
+        textbox,
+        prompt,
+    )
+    textbox.send_keys(Keys.ENTER)
+
+def get_last_response():
+    responses = common.driver.find_elements(*chatgpt_big_response)
+    if responses:
+        response = responses[-1]
+        if 'text-red' in response.get_attribute('class'):
+            raise ValueError(response.text)
+        return response
+    return common.driver.find_elements(*chatgpt_small_response)[-1]
+
+def get_response() -> str:
+    result_streaming = WebDriverWait(common.driver, 3).until(
+        expected_conditions.presence_of_element_located(chatgpt_streaming)
+    )
+    while result_streaming:
+        response = get_last_response()
+        response = response.get_attribute('innerHTML')
+        yield response
+        result_streaming = common.driver.find_elements(*chatgpt_streaming)
+    response = get_last_response()
+    yield response.get_attribute('innerHTML')
+
+def ask(prompt: str) -> str:
+    request(prompt)
+    return get_response()
+
+# Internal Cell
 import random, string
 
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
@@ -244,231 +409,144 @@
         for key in obj:
             obj[key] = attributize(obj[key])
         return attrdict(obj)
     if isinstance(obj, list):
         return [attributize(item) for item in obj]
     return obj
 
-def delta(prompt):
-    id = ''.join(
+def retry_on_status_code(func):
+    '''Retry decorator that retries a function on specific status codes.'''
+    def wrapper(*args, **kwargs):
+        wait_second = 1
+        while True:
+            try:
+                return func(*args, **kwargs)
+            except requests.exceptions.HTTPError as err:
+                sys.stderr.write(
+                    f'{err}\n'
+                    f'text = {repr(err.response.text)}\n'
+                )
+                status_code = err.response.status_code
+                if status_code in (401, 403, 413, 500):
+                    # status code 413: the caller should split the prompt first
+                    break
+                if status_code >= 400:
+                    sys.stderr.write(
+                        f'Retrying...\n'
+                    )
+                    time.sleep(wait_second)
+                    wait_second *= 2
+                    continue
+                break
+    return wrapper
+
+@retry_on_status_code
+def content(prompt):
+    for response in start_conversation(prompt):
+        pass
+    if response == '':
+        sys.stderr.write(
+            f'Error Responding: response = {repr(response)}\n'
+        )
+    return response
+
+def new_id():
+    return ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
-    wait_second = 1
-    while True:
-        res = ''
-        response = ''
-        try:
-            for response in start_conversation(prompt):
-                yield attributize({
-                    'choices': [
-                        {
-                            'index': 0,
-                            'logprobs': None,
-                            'text': response[len(res):],
-                        }
-                    ],
-                    'id': f'cmpl-{id}',
-                })
-                res = response
-        except requests.exceptions.HTTPError as err:
-            sys.stderr.write(
-                f'{err}\n'
-                f'response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            status_code = err.response.status_code
-            if status_code == 413:
-                # caller should split the prompt
-                break
-            # if status_code == 429:
-            #     break
-            if status_code >= 400 and status_code != 500:
-                time.sleep(wait_second)
-                wait_second *= 2
-                continue
-            break
-        if response == '':
-            sys.stderr.write(
-                f'Error Responding: response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            time.sleep(wait_second)
-            wait_second *= 2
-            continue
-        break
+
+def delta(prompt):
+    res = ''
+    for response in start_conversation(prompt):
+        yield attributize({
+            'choices': [
+                {
+                    'index': 0,
+                    'logprobs': None,
+                    'text': response[len(res):],
+                }
+            ],
+            'id': f'cmpl-{new_id()}',
+        })
+        res = response
+    if response == '':
+        sys.stderr.write(
+            f'Error Responding: response = {repr(response)}\n'
+        )
+
+def chat_delta(prompt):
+    res = ''
+    for response in start_conversation(prompt):
+        yield attributize({
+            'choices': [
+                {
+                    'index': 0,
+                    'delta': {
+                        'content': response[len(res):],
+                    }
+                }
+            ],
+            'id': f'chatcmpl-{new_id()}',
+        })
+        res = response
+    if response == '':
+        sys.stderr.write(
+            f'Error Responding: response = {repr(response)}\n'
+        )
 
 def mock_create(*args, **kwargs):
     prompts = []
     if isinstance(kwargs['prompt'], str):
         prompts = [kwargs['prompt']]
     if isinstance(kwargs['prompt'], list):
         prompts = kwargs['prompt']
     prompts = [prompt.strip() for prompt in prompts]
 
     if kwargs.get('stream', False):
         return delta('\n'.join(prompts))
 
     choices = []
     for prompt in prompts:
-        response = ''
-        wait_second = 1
-        while True:
-            try:
-                for response in start_conversation(prompt):
-                    pass
-            except requests.exceptions.HTTPError as err:
-                sys.stderr.write(
-                    f'{err}\n'
-                    f'response = {repr(response)}\n'
-                    f'Retrying...\n'
-                )
-                status_code = err.response.status_code
-                if status_code == 413:
-                    # caller should split the prompt
-                    break
-                # if status_code == 429:
-                #     break
-                if status_code >= 400 and status_code != 500:
-                    time.sleep(wait_second)
-                    wait_second *= 2
-                    continue
-                break
-            if response == '':
-                sys.stderr.write(
-                    f'Error Responding: response = {repr(response)}\n'
-                    f'Retrying...\n'
-                )
-                time.sleep(wait_second)
-                wait_second *= 2
-                continue
-            break
         choices.append({
             'finish_reason': 'stop',
             'index': 0,
             'logprobs': None,
-            'text': response,
+            'text': content(prompt),
         })
-    id = ''.join(
-        random.choices(string.ascii_letters + string.digits, k = 29)
-    )
     return attributize({
         'choices': choices,
-        'id': f'cmpl-{id}',
+        'id': f'cmpl-{new_id()}',
         'usage': {
             'completion_tokens': 0,
             'prompt_tokens': 0,
             'total_tokens': 0,
         },
     })
 
-def chat_delta(prompt):
-    id = ''.join(
-        random.choices(string.ascii_letters + string.digits, k = 29)
-    )
-    wait_second = 1
-    while True:
-        res = ''
-        response = ''
-        try:
-            for response in start_conversation(prompt):
-                yield attributize({
-                    'choices': [
-                        {
-                            'index': 0,
-                            'delta': {
-                                'content': response[len(res):],
-                            }
-                        }
-                    ],
-                    'id': f'chatcmpl-{id}',
-                })
-                res = response
-        except requests.exceptions.HTTPError as err:
-            sys.stderr.write(
-                f'{err}\n'
-                f'response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            status_code = err.response.status_code
-            if status_code == 413:
-                # caller should split the prompt
-                break
-            # if status_code == 429:
-            #     break
-            if status_code >= 400 and status_code != 500:
-                time.sleep(wait_second)
-                wait_second *= 2
-                continue
-            break
-        if response == '':
-            sys.stderr.write(
-                f'Error Responding: response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            time.sleep(wait_second)
-            wait_second *= 2
-            continue
-        break
-
 def mock_chat_create(*args, **kwargs):
     summarized_prompt = ''
     for message in kwargs['messages']:
         summarized_prompt += f"{message['role']}:\n\n{message['content']}\n\n\n"
     summarized_prompt.strip()
 
     if kwargs.get('stream', False):
         return chat_delta(summarized_prompt)
 
-    response = ''
-    wait_second = 1
-    while True:
-        try:
-            for response in start_conversation(summarized_prompt):
-                pass
-        except requests.exceptions.HTTPError as err:
-            sys.stderr.write(
-                f'{err}\n'
-                f'response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            status_code = err.response.status_code
-            if status_code == 413:
-                # caller should split the prompt
-                break
-            # if status_code == 429:
-            #     break
-            if status_code >= 400 and status_code != 500:
-                time.sleep(wait_second)
-                wait_second *= 2
-                continue
-            break
-        if response == '':
-            sys.stderr.write(
-                f'Error Responding: response = {repr(response)}\n'
-                f'Retrying...\n'
-            )
-            time.sleep(wait_second)
-            wait_second *= 2
-            continue
-        break
-    id = ''.join(
-        random.choices(string.ascii_letters + string.digits, k = 29)
-    )
     return attributize({
         'choices': [
             {
                 'finish_reason': 'stop',
                 'index': 0,
                 'message': {
-                    'content': response,
+                    'content': content(summarized_prompt),
                     'role': 'assistant',
                 }
             }
         ],
-        'id': f'chatcmpl-{id}',
+        'id': f'chatcmpl-{new_id()}',
         'usage': {
             'completion_tokens': 0,
             'prompt_tokens': 0,
             'total_tokens': 0,
         },
     })
```

### Comparing `ipymock-1.0.4/ipymock/llm.py` & `ipymock-1.1.0/ipymock/llm.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/ipymock/reader.py` & `ipymock-1.1.0/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.4/ipymock.egg-info/PKG-INFO` & `ipymock-1.1.0/ipymock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.4
+Version: 1.1.0
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-1.0.4/settings.ini` & `ipymock-1.1.0/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = 2023 onwards, Neuro Spirit, DAO.
 branch = main
-version = 1.0.4
+version = 1.1.0
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-1.0.4/setup.py` & `ipymock-1.1.0/setup.py`

 * *Files identical despite different names*

