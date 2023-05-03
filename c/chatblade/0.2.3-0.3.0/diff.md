# Comparing `tmp/chatblade-0.2.3.tar.gz` & `tmp/chatblade-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatblade-0.2.3.tar", last modified: Wed Apr 19 05:28:09 2023, max compression
+gzip compressed data, was "chatblade-0.3.0.tar", last modified: Wed May  3 15:13:52 2023, max compression
```

## Comparing `chatblade-0.2.3.tar` & `chatblade-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.353952 chatblade-0.2.3/
--rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.2.3/LICENSE
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-19 05:28:09.354025 chatblade-0.2.3/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)    10405 2023-04-11 09:29:23.000000 chatblade-0.2.3/README.md
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.346266 chatblade-0.2.3/chatblade/
--rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.2.3/chatblade/__init__.py
--rw-r--r--   0 npiv       (501) staff       (20)       86 2023-03-18 14:05:20.000000 chatblade-0.2.3/chatblade/__main__.py
--rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/chat.py
--rw-r--r--   0 npiv       (501) staff       (20)     4613 2023-04-19 05:17:37.000000 chatblade-0.2.3/chatblade/cli.py
--rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.2.3/chatblade/errors.py
--rw-r--r--   0 npiv       (501) staff       (20)     5590 2023-04-09 08:15:38.000000 chatblade-0.2.3/chatblade/parser.py
--rw-r--r--   0 npiv       (501) staff       (20)     4543 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/printer.py
--rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/session.py
--rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.2.3/chatblade/storage.py
--rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/utils.py
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.353856 chatblade-0.2.3/chatblade.egg-info/
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)      452 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/SOURCES.txt
--rw-r--r--   0 npiv       (501) staff       (20)        1 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/dependency_links.txt
--rw-r--r--   0 npiv       (501) staff       (20)       54 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/entry_points.txt
--rw-r--r--   0 npiv       (501) staff       (20)       49 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/requires.txt
--rw-r--r--   0 npiv       (501) staff       (20)       10 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/top_level.txt
--rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.2.3/pyproject.toml
--rw-r--r--   0 npiv       (501) staff       (20)      567 2023-04-19 05:28:09.354397 chatblade-0.2.3/setup.cfg
--rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.2.3/setup.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.346055 chatblade-0.3.0/
+-rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.3.0/LICENSE
+-rw-r--r--   0 npiv       (501) staff       (20)    10892 2023-05-03 15:13:52.346121 chatblade-0.3.0/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)    10588 2023-05-03 11:32:02.000000 chatblade-0.3.0/README.md
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.345312 chatblade-0.3.0/chatblade/
+-rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.3.0/chatblade/__init__.py
+-rw-r--r--   0 npiv       (501) staff       (20)      156 2023-04-25 05:44:29.000000 chatblade-0.3.0/chatblade/__main__.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/chat.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4613 2023-04-21 15:19:16.000000 chatblade-0.3.0/chatblade/cli.py
+-rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.3.0/chatblade/errors.py
+-rw-r--r--   0 npiv       (501) staff       (20)     6054 2023-05-03 11:20:12.000000 chatblade-0.3.0/chatblade/parser.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4644 2023-05-03 11:26:22.000000 chatblade-0.3.0/chatblade/printer.py
+-rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/session.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.3.0/chatblade/storage.py
+-rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/utils.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.345966 chatblade-0.3.0/chatblade.egg-info/
+-rw-r--r--   0 npiv       (501) staff       (20)    10892 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)      452 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/SOURCES.txt
+-rw-r--r--   0 npiv       (501) staff       (20)        1 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/dependency_links.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       54 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/entry_points.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       49 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/requires.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       10 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/top_level.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.3.0/pyproject.toml
+-rw-r--r--   0 npiv       (501) staff       (20)      567 2023-05-03 15:13:52.346512 chatblade-0.3.0/setup.cfg
+-rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.3.0/setup.py
```

### Comparing `chatblade-0.2.3/LICENSE` & `chatblade-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/PKG-INFO` & `chatblade-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.3
+Version: 0.3.0
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,19 +25,23 @@
 - check out the project, and run `pip install .`
 - or `pip install 'chatblade @ git+https://github.com/npiv/chatblade'`
 
 ### Via pypi
 
 The last released version can be installed with `pip install chatblade --upgrade`
 
-### via Brew tap (slow...)
+### Via Brew
 
-Official Homebrew acceptance is pending, in the meantime you can use this brew tap:
 ```
-brew tap npiv/chatblade
+brew install chatblade
+```
+
+**Note**: if you were using the brew tap before, you will need to 
+```
+brew untap npiv/chatblade
 brew install chatblade
 ```
 
 ## Documentation
 
 ### Making queries
 
@@ -229,16 +233,16 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [-l] [-S sess] [--session-list] [--session-path]
-                 [--session-dump] [--session-delete] [--session-rename newsess]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
+                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
                  [query ...]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
   query                           Query to send to chat GPT
 
@@ -246,21 +250,22 @@
   -h, --help                      show this help message and exit
   --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
   --temperature t                 temperature (openai setting)
   -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
   -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
   -s, --stream                    Stream the incoming text to the terminal
   -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt at ~/.config/chatblade/name as system msg
+  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
   -e, --extract                   extract content from response if possible (either json or code block)
   -r, --raw                       print session as pure text, don't pretty print or format
   -n, --no-format                 do not add pretty print formatting to output
   -o, --only                      Only display the response, omit query
+  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
   -l, --last                      alias for '-S last', the default session if none is specified
   -S sess, --session sess         initiate or continue named session
   --session-list                  list sessions
   --session-path                  show path to session file
   --session-dump                  dump session to stdout
```

### Comparing `chatblade-0.2.3/README.md` & `chatblade-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 - check out the project, and run `pip install .`
 - or `pip install 'chatblade @ git+https://github.com/npiv/chatblade'`
 
 ### Via pypi
 
 The last released version can be installed with `pip install chatblade --upgrade`
 
-### via Brew tap (slow...)
+### Via Brew
 
-Official Homebrew acceptance is pending, in the meantime you can use this brew tap:
 ```
-brew tap npiv/chatblade
+brew install chatblade
+```
+
+**Note**: if you were using the brew tap before, you will need to 
+```
+brew untap npiv/chatblade
 brew install chatblade
 ```
 
 ## Documentation
 
 ### Making queries
 
@@ -219,16 +223,16 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [-l] [-S sess] [--session-list] [--session-path]
-                 [--session-dump] [--session-delete] [--session-rename newsess]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
+                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
                  [query ...]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
   query                           Query to send to chat GPT
 
@@ -236,21 +240,22 @@
   -h, --help                      show this help message and exit
   --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
   --temperature t                 temperature (openai setting)
   -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
   -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
   -s, --stream                    Stream the incoming text to the terminal
   -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt at ~/.config/chatblade/name as system msg
+  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
   -e, --extract                   extract content from response if possible (either json or code block)
   -r, --raw                       print session as pure text, don't pretty print or format
   -n, --no-format                 do not add pretty print formatting to output
   -o, --only                      Only display the response, omit query
+  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
   -l, --last                      alias for '-S last', the default session if none is specified
   -S sess, --session sess         initiate or continue named session
   --session-list                  list sessions
   --session-path                  show path to session file
   --session-dump                  dump session to stdout
```

### Comparing `chatblade-0.2.3/chatblade/chat.py` & `chatblade-0.3.0/chatblade/chat.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/chatblade/cli.py` & `chatblade-0.3.0/chatblade/cli.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/chatblade/parser.py` & `chatblade-0.3.0/chatblade/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,21 @@
     if options["openai_api_key"]:
         return options["openai_api_key"]
     elif "OPENAI_API_KEY" in os.environ:
         return os.environ["OPENAI_API_KEY"]
     else:
         return None
 
+def get_theme(options):
+    if options["theme"]:
+        return options["theme"]
+    elif "CHATBLADE_THEME" in os.environ:
+        return os.environ["CHATBLADE_THEME"]
+    else:
+        return None
 
 def extract_query(query):
     """The query comes from both the query and any piped input
     The user can provide either only a query, a piped input, or both
     in which case the piped input gets placed above the query
     """
     query = " ".join(query) if query else None
@@ -36,14 +43,15 @@
     else:
         return None
 
 
 def extract_options(options):
     options = vars(options)  # to map
     options["openai_api_key"] = get_openai_key(options)
+    options["theme"] = get_theme(options)
     options["model"] = {"3.5": "gpt-3.5-turbo", "4": "gpt-4"}[options["chat_gpt"]]
     del options["query"]
     del options["chat_gpt"]
     return utils.DotDict(options)
 
 
 def valid_session(sess):
@@ -133,14 +141,20 @@
     )
     display_opts.add_argument(
         "-o",
         "--only",
         help="Only display the response, omit query",
         action="store_true",
     )
+    display_opts.add_argument(
+        "--theme",
+        metavar="theme",
+        type=str,
+        help="Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME",
+    )
 
     session_opts = parser.add_argument_group("session options")
     session_opts.add_argument(
         "-l",
         "--last",
         dest="session",
         action="store_const",
```

### Comparing `chatblade-0.2.3/chatblade/printer.py` & `chatblade-0.3.0/chatblade/printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 COLORS = {"user": "blue", "assistant": "green", "system": "red"}
 
 
 def print_message(message, args):
     printable = message.content
     if not args.raw:
         printable = detect_and_format_message(
-            message.content, cutoff=1000 if message.role == "user" else None
+            message.content, cutoff=1000 if message.role == "user" else None, theme=args.theme
         )
     if not args.no_format:
       console.print(Rule(message.role, style=COLORS[message.role]))
 
     if args.raw:
         print(message.content)
     else:
@@ -82,24 +82,25 @@
         print(extract_json(message.content))
     elif contains_block(message.content):
         print(extract_block(message.content))
     else:
         print(message.content.strip())
 
 
-def detect_and_format_message(msg, cutoff=None):
+def detect_and_format_message(msg, cutoff=None, theme=None):
     if cutoff and len(msg) > cutoff:
         msg = "... **text shortened** ... " + msg[-cutoff:]
         return msg
     elif contains_json(msg):
         utils.debug(detected="json")
         return JSON(extract_json(msg))
     elif looks_like_markdown(msg):
         utils.debug(detected="markdown")
-        return Markdown(msg)
+        theme = "monokai" if theme is None else theme
+        return Markdown(msg,code_theme=theme)
     else:
         utils.debug(detected="regular")
         return msg
 
 
 def extract_json_lists(str_lists, flatten=False):
     lists = [json.loads(extract_json(x)) for x in str_lists if contains_json(x)]
```

### Comparing `chatblade-0.2.3/chatblade/session.py` & `chatblade-0.3.0/chatblade/session.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/chatblade/storage.py` & `chatblade-0.3.0/chatblade/storage.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/chatblade/utils.py` & `chatblade-0.3.0/chatblade/utils.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.3/chatblade.egg-info/PKG-INFO` & `chatblade-0.3.0/chatblade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.3
+Version: 0.3.0
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,19 +25,23 @@
 - check out the project, and run `pip install .`
 - or `pip install 'chatblade @ git+https://github.com/npiv/chatblade'`
 
 ### Via pypi
 
 The last released version can be installed with `pip install chatblade --upgrade`
 
-### via Brew tap (slow...)
+### Via Brew
 
-Official Homebrew acceptance is pending, in the meantime you can use this brew tap:
 ```
-brew tap npiv/chatblade
+brew install chatblade
+```
+
+**Note**: if you were using the brew tap before, you will need to 
+```
+brew untap npiv/chatblade
 brew install chatblade
 ```
 
 ## Documentation
 
 ### Making queries
 
@@ -229,16 +233,16 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [-l] [-S sess] [--session-list] [--session-path]
-                 [--session-dump] [--session-delete] [--session-rename newsess]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
+                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
                  [query ...]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
   query                           Query to send to chat GPT
 
@@ -246,21 +250,22 @@
   -h, --help                      show this help message and exit
   --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
   --temperature t                 temperature (openai setting)
   -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
   -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
   -s, --stream                    Stream the incoming text to the terminal
   -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt at ~/.config/chatblade/name as system msg
+  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
   -e, --extract                   extract content from response if possible (either json or code block)
   -r, --raw                       print session as pure text, don't pretty print or format
   -n, --no-format                 do not add pretty print formatting to output
   -o, --only                      Only display the response, omit query
+  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
   -l, --last                      alias for '-S last', the default session if none is specified
   -S sess, --session sess         initiate or continue named session
   --session-list                  list sessions
   --session-path                  show path to session file
   --session-dump                  dump session to stdout
```

### Comparing `chatblade-0.2.3/setup.cfg` & `chatblade-0.3.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chatblade
-version = 0.2.3
+version = 0.3.0
 description = CLI Swiss Army Knife for ChatGPT
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/npiv/chatblade
 keywords = chatblade chatgpt cli python
 project_urls =
```

