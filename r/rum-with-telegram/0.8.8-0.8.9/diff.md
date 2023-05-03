# Comparing `tmp/rum_with_telegram-0.8.8.tar.gz` & `tmp/rum_with_telegram-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.8.tar", last modified: Wed May  3 15:37:05 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.9.tar", last modified: Wed May  3 16:04:28 2023, max compression
```

## Comparing `rum_with_telegram-0.8.8.tar` & `rum_with_telegram-0.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.509322 rum_with_telegram-0.8.8/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.8/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-03 15:37:05.508190 rum_with_telegram-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.8/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.493716 rum_with_telegram-0.8.8/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-03 15:34:34.000000 rum_with_telegram-0.8.8/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.8.8/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    24241 2023-05-03 15:34:42.000000 rum_with_telegram-0.8.8/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3018 2023-05-03 15:18:36.000000 rum_with_telegram-0.8.8/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.8/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.506196 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 15:37:05.509826 rum_with_telegram-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-05-03 15:34:34.000000 rum_with_telegram-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:28.076855 rum_with_telegram-0.8.9/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-03 16:04:28.074861 rum_with_telegram-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.9/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:28.050729 rum_with_telegram-0.8.9/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-03 16:03:31.000000 rum_with_telegram-0.8.9/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.8.9/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    24401 2023-05-03 16:03:11.000000 rum_with_telegram-0.8.9/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3018 2023-05-03 15:18:36.000000 rum_with_telegram-0.8.9/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.9/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:28.072867 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-03 16:04:27.000000 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-03 16:04:28.000000 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:04:27.000000 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-03 16:04:27.000000 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 16:04:27.000000 rum_with_telegram-0.8.9/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:04:28.076855 rum_with_telegram-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-03 16:03:31.000000 rum_with_telegram-0.8.9/setup.py
```

### Comparing `rum_with_telegram-0.8.8/LICENSE` & `rum_with_telegram-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.8/PKG-INFO` & `rum_with_telegram-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.8
+Version: 0.8.9
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.8/rum_with_telegram/config.py` & `rum_with_telegram-0.8.9/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.8/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.9/rum_with_telegram/data_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,40 +474,42 @@
 
     def get_all_trxs(self, senders, start_trx=None):
         trxs = self.rum.api.get_content(senders=senders, start_trx=start_trx, num=20)
         if len(trxs) == 0:
             return None
         for i in trxs:
             yield i
-        return self.get_all_trxs(senders, trxs[-1]["trx_id"])
+        return self.get_all_trxs(senders, trxs[-1]["TrxId"])
 
     async def command_export_data(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_export_data %s", update.message.message_id)
         userid = update.message.from_user.id
         user = self.db.get_first_user(userid)
 
         if not user:
             reply = "You have not registered yet. Please use command as `/new_key` to register."
             await update.message.reply_text(reply)
             return
 
         trxs = [i for i in self.get_all_trxs([user.pubkey]) if i]
-        # create file-like object in memory
-        data = json.dumps(trxs).encode("utf-8")
-        with io.BytesIO(data) as buffer:
-            buffer.seek(0)
-            # send file to user
-            await context.bot.send_document(
-                chat_id=update.message.chat_id,
-                document=buffer,
-                filename=f"{user.pubkey}_{datetime.date.today()}.json",
-                reply_to_message_id=update.message.message_id,
-            )
-
-        reply = f"You have exported your data, that is {len(trxs)} trxs in blockchain of rum-group.\nYour private key is:\n```{user.pvtkey}```\nPlease keep it safe."
+        if len(trxs) > 0:
+            # create file-like object in memory
+            data = json.dumps(trxs).encode("utf-8")
+            with io.BytesIO(data) as buffer:
+                buffer.seek(0)
+                # send file to user
+                await context.bot.send_document(
+                    chat_id=update.message.chat_id,
+                    document=buffer,
+                    filename=f"{user.pubkey}_{datetime.date.today()}.json",
+                    reply_to_message_id=update.message.message_id,
+                )
+            reply = f"You have exported your data, that is {len(trxs)} trxs in blockchain of rum-group.\nYour private key is:\n```{user.pvtkey}```\nPlease keep it safe."
+        else:
+            reply = "You have not any data in blockchain of rum-group."
         await update.message.reply_text(reply, parse_mode="Markdown")
 
     async def command_my_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_my_nft")
         # TODO
 
     async def command_grant_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
```

### Comparing `rum_with_telegram-0.8.8/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.9/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.8/rum_with_telegram/module.py` & `rum_with_telegram-0.8.9/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.8/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.9/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.8
+Version: 0.8.9
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.8/setup.py` & `rum_with_telegram-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.8",
+    version="0.8.9",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
@@ -27,12 +27,12 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(exclude=["example"]),
     python_requires=">=3.7",
     install_requires=[
         "python-telegram-bot==20.2",
-        "quorum-data-py",
+        "quorum-data-py>=1.2.7",
         "quorum-mininode-py",
         "sqlalchemy",
     ],
 )
```

