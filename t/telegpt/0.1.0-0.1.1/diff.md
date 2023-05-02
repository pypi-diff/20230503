# Comparing `tmp/telegpt-0.1.0.tar.gz` & `tmp/telegpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegpt-0.1.0.tar", last modified: Tue May  2 21:53:20 2023, max compression
+gzip compressed data, was "telegpt-0.1.1.tar", last modified: Tue May  2 21:58:09 2023, max compression
```

## Comparing `telegpt-0.1.0.tar` & `telegpt-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:53:20.093368 telegpt-0.1.0/
--rw-r--r--   0 fernando   (501) staff       (20)     1691 2023-05-02 21:53:20.093621 telegpt-0.1.0/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      574 2023-05-02 21:50:51.000000 telegpt-0.1.0/README.md
--rw-r--r--   0 fernando   (501) staff       (20)       90 2023-03-19 01:39:53.000000 telegpt-0.1.0/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)     1640 2023-05-02 21:53:20.095209 telegpt-0.1.0/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:53:20.076523 telegpt-0.1.0/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:53:20.082013 telegpt-0.1.0/src/telegpt/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2023-03-07 23:09:44.000000 telegpt-0.1.0/src/telegpt/__init__.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:53:20.092873 telegpt-0.1.0/src/telegpt/apis/
--rw-r--r--   0 fernando   (501) staff       (20)      133 2023-03-27 19:38:46.000000 telegpt-0.1.0/src/telegpt/apis/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)      404 2023-03-19 02:51:31.000000 telegpt-0.1.0/src/telegpt/apis/exchange.py
--rw-r--r--   0 fernando   (501) staff       (20)     1977 2023-03-27 19:23:33.000000 telegpt-0.1.0/src/telegpt/apis/gpt.py
--rw-r--r--   0 fernando   (501) staff       (20)     1156 2023-03-21 00:21:25.000000 telegpt-0.1.0/src/telegpt/apis/whisper.py
--rw-r--r--   0 fernando   (501) staff       (20)     5945 2023-05-02 21:37:14.000000 telegpt-0.1.0/src/telegpt/bot.py
--rw-r--r--   0 fernando   (501) staff       (20)      120 2023-05-02 21:52:30.000000 telegpt-0.1.0/src/telegpt/main.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2023-03-19 01:39:24.000000 telegpt-0.1.0/src/telegpt/py.typed
--rw-r--r--   0 fernando   (501) staff       (20)      451 2023-03-20 22:58:20.000000 telegpt-0.1.0/src/telegpt/utils.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:53:20.089976 telegpt-0.1.0/src/telegpt.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1691 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      495 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)       46 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/entry_points.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2023-05-02 21:52:09.000000 telegpt-0.1.0/src/telegpt.egg-info/not-zip-safe
--rw-r--r--   0 fernando   (501) staff       (20)       56 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)        8 2023-05-02 21:53:20.000000 telegpt-0.1.0/src/telegpt.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:58:09.231104 telegpt-0.1.1/
+-rw-r--r--   0 fernando   (501) staff       (20)     1806 2023-05-02 21:58:09.231319 telegpt-0.1.1/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      689 2023-05-02 21:57:10.000000 telegpt-0.1.1/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)       90 2023-03-19 01:39:53.000000 telegpt-0.1.1/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)     1640 2023-05-02 21:58:09.235401 telegpt-0.1.1/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:58:09.202832 telegpt-0.1.1/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:58:09.210937 telegpt-0.1.1/src/telegpt/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2023-03-07 23:09:44.000000 telegpt-0.1.1/src/telegpt/__init__.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:58:09.229918 telegpt-0.1.1/src/telegpt/apis/
+-rw-r--r--   0 fernando   (501) staff       (20)      133 2023-03-27 19:38:46.000000 telegpt-0.1.1/src/telegpt/apis/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)      404 2023-03-19 02:51:31.000000 telegpt-0.1.1/src/telegpt/apis/exchange.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1977 2023-03-27 19:23:33.000000 telegpt-0.1.1/src/telegpt/apis/gpt.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1156 2023-03-21 00:21:25.000000 telegpt-0.1.1/src/telegpt/apis/whisper.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5945 2023-05-02 21:37:14.000000 telegpt-0.1.1/src/telegpt/bot.py
+-rw-r--r--   0 fernando   (501) staff       (20)      120 2023-05-02 21:52:30.000000 telegpt-0.1.1/src/telegpt/main.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2023-03-19 01:39:24.000000 telegpt-0.1.1/src/telegpt/py.typed
+-rw-r--r--   0 fernando   (501) staff       (20)      451 2023-03-20 22:58:20.000000 telegpt-0.1.1/src/telegpt/utils.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2023-05-02 21:58:09.223502 telegpt-0.1.1/src/telegpt.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1806 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      495 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       46 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/entry_points.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2023-05-02 21:52:09.000000 telegpt-0.1.1/src/telegpt.egg-info/not-zip-safe
+-rw-r--r--   0 fernando   (501) staff       (20)       56 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        8 2023-05-02 21:58:09.000000 telegpt-0.1.1/src/telegpt.egg-info/top_level.txt
```

### Comparing `telegpt-0.1.0/PKG-INFO` & `telegpt-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegpt
-Version: 0.1.0
+Version: 0.1.1
 Maintainer: Fernando Perez-Garcia
 Maintainer-email: fepegar@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/fepegar/telegram-gpt-bot
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -24,29 +24,31 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Telegram bot for ChatGPT
 
+Send voice notes in any language (which will be translated to English) or text messages to ChatGPT.
+
 ## Set environment variables
 
-- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather).
+- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather)
 - `TELEGRAM_CLIENT_ID`: Telegram client ID from [@userinfobot](https://t.me/userinfobot)
-- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/).
+- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/)
 
 ## Installation
 
 ```shell
-pip install .
+pip install telegpt
 ```
 
 ## Launch the bot
 
 ```shell
 telegpt
 ```
 
 ## Usage
 
-- `/new`: Restart the bot so it forget the last conversation.
+- Text `/new` to the bot to restart so it forget the last conversation.
 - Voice notes in any language will be translated to English before being passed to ChatGPT.
```

### Comparing `telegpt-0.1.0/README.md` & `telegpt-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Telegram bot for ChatGPT
 
+Send voice notes in any language (which will be translated to English) or text messages to ChatGPT.
+
 ## Set environment variables
 
-- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather).
+- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather)
 - `TELEGRAM_CLIENT_ID`: Telegram client ID from [@userinfobot](https://t.me/userinfobot)
-- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/).
+- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/)
 
 ## Installation
 
 ```shell
-pip install .
+pip install telegpt
 ```
 
 ## Launch the bot
 
 ```shell
 telegpt
 ```
 
 ## Usage
 
-- `/new`: Restart the bot so it forget the last conversation.
+- Text `/new` to the bot to restart so it forget the last conversation.
 - Voice notes in any language will be translated to English before being passed to ChatGPT.
```

### Comparing `telegpt-0.1.0/setup.cfg` & `telegpt-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telegpt
-version = 0.1.0
+version = 0.1.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 maintainer = Fernando Perez-Garcia
 maintainer_email = fepegar@gmail.com
 license = MIT
 license_file = LICENSE
 platforms = OS Independent
```

### Comparing `telegpt-0.1.0/src/telegpt/apis/gpt.py` & `telegpt-0.1.1/src/telegpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `telegpt-0.1.0/src/telegpt/apis/whisper.py` & `telegpt-0.1.1/src/telegpt/apis/whisper.py`

 * *Files identical despite different names*

### Comparing `telegpt-0.1.0/src/telegpt/bot.py` & `telegpt-0.1.1/src/telegpt/bot.py`

 * *Files identical despite different names*

### Comparing `telegpt-0.1.0/src/telegpt.egg-info/PKG-INFO` & `telegpt-0.1.1/src/telegpt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegpt
-Version: 0.1.0
+Version: 0.1.1
 Maintainer: Fernando Perez-Garcia
 Maintainer-email: fepegar@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/fepegar/telegram-gpt-bot
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -24,29 +24,31 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Telegram bot for ChatGPT
 
+Send voice notes in any language (which will be translated to English) or text messages to ChatGPT.
+
 ## Set environment variables
 
-- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather).
+- `TELEGRAM_BOT_TOKEN`: Telegram token from bot created using [@BotFather](https://t.me/botfather)
 - `TELEGRAM_CLIENT_ID`: Telegram client ID from [@userinfobot](https://t.me/userinfobot)
-- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/).
+- `OPENAI_API_KEY`: OpenAI API key from [OpenAI](https://beta.openai.com/)
 
 ## Installation
 
 ```shell
-pip install .
+pip install telegpt
 ```
 
 ## Launch the bot
 
 ```shell
 telegpt
 ```
 
 ## Usage
 
-- `/new`: Restart the bot so it forget the last conversation.
+- Text `/new` to the bot to restart so it forget the last conversation.
 - Voice notes in any language will be translated to English before being passed to ChatGPT.
```

