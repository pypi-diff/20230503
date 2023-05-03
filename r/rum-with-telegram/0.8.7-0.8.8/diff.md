# Comparing `tmp/rum_with_telegram-0.8.7.tar.gz` & `tmp/rum_with_telegram-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.7.tar", last modified: Sun Apr 30 16:32:46 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.8.tar", last modified: Wed May  3 15:37:05 2023, max compression
```

## Comparing `rum_with_telegram-0.8.7.tar` & `rum_with_telegram-0.8.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.395792 rum_with_telegram-0.8.7/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.7/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-30 16:32:46.394795 rum_with_telegram-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.7/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.383824 rum_with_telegram-0.8.7/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-30 16:32:07.000000 rum_with_telegram-0.8.7/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.7/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    23983 2023-04-30 16:32:13.000000 rum_with_telegram-0.8.7/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3112 2023-04-30 16:31:39.000000 rum_with_telegram-0.8.7/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.7/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.392827 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 16:32:46.396791 rum_with_telegram-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-30 16:32:07.000000 rum_with_telegram-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.509322 rum_with_telegram-0.8.8/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-03 15:37:05.508190 rum_with_telegram-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.8/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.493716 rum_with_telegram-0.8.8/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-03 15:34:34.000000 rum_with_telegram-0.8.8/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.8.8/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    24241 2023-05-03 15:34:42.000000 rum_with_telegram-0.8.8/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3018 2023-05-03 15:18:36.000000 rum_with_telegram-0.8.8/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.8/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:05.506196 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 15:37:05.000000 rum_with_telegram-0.8.8/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 15:37:05.509826 rum_with_telegram-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-05-03 15:34:34.000000 rum_with_telegram-0.8.8/setup.py
```

### Comparing `rum_with_telegram-0.8.7/LICENSE` & `rum_with_telegram-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.7/PKG-INFO` & `rum_with_telegram-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.7
+Version: 0.8.8
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.7/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.8/rum_with_telegram/data_exchanger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import base64
 import datetime
+import io
+import json
 import logging
 
 from quorum_data_py import feed, get_trx_type, util
-from quorum_mininode_py import MiniNode
-from quorum_mininode_py.crypto import account
+from quorum_mininode_py import MiniNode, pvtkey_to_pubkey
 from telegram import Bot, Update
 from telegram.ext import Application, CommandHandler, ContextTypes, MessageHandler, filters
 
 from rum_with_telegram.config import get_config
 from rum_with_telegram.db_handle import DBHandle
 from rum_with_telegram.module import Relation
 
@@ -196,19 +197,15 @@
 
     async def handle_private_chat(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """send message to rum group and telegram channel"""
         message_id = update.message.message_id
         logger.info("handle_private_chat %s", message_id)
         userid = update.message.from_user.id
         if userid in self.config.BLACK_LIST_TGIDS:
-            await context.bot.send_message(
-                chat_id=userid,
-                text="You are in the blacklist.",
-                reply_to_message_id=update.message.message_id,
-            )
+            await update.message.reply_text("You are in the blacklist.")
             return
         _first_name = update.message.from_user.first_name
         _last_name = update.message.from_user.last_name
         _fullname = f"{_first_name} {_last_name}" if _last_name else _first_name
         _text = update.message.text or update.message.caption or ""
         if _text.startswith("/profile"):
             await self.command_profile(update, context)
@@ -350,19 +347,15 @@
         )
         self.db.add_or_update(Relation, relation, "trx_id")
 
     async def handle_group_message(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """handle group message"""
         userid = update.message.from_user.id
         if userid in self.config.BLACK_LIST_TGIDS:
-            await context.bot.send_message(
-                chat_id=userid,
-                text="You are in the blacklist.",
-                reply_to_message_id=update.message.message_id,
-            )
+            await update.message.reply_text("You are in the blacklist.")
             return
 
         if update.message.reply_to_message:
             await self._handle_reply_message(update, context)
             return
         logger.info(
             "handle_group_message %s without reply_to_message",
@@ -398,33 +391,26 @@
         self.db.add_or_update(Relation, relation, "trx_id")
 
     async def command_start(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """/start command handler"""
         logger.info("start command_start %s", update.message.message_id)
         username = update.message.from_user.username or ""
         text = f"Hello {username}! I'm {self.config.TG_BOT_NAME}. \nI can send your message (such as text, photo) as a new microblog from telgram to the blockchain of RUM network. \nTry to say something to me."
-        await context.bot.send_message(
-            chat_id=update.message.chat_id,
-            text=text,
-            reply_to_message_id=update.message.message_id,
-        )
+        await update.message.reply_text(text)
 
     async def command_profile(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """/profile command handler, change user name or avatar for the blockchain of rum network"""
         logger.info("start command_name %s", update.message.message_id)
         _text = update.message.text or update.message.caption or ""
         name = _text.replace("/profile", "").strip(" '\"")
         reply = f"Enter name: ```{name}```\n"
 
         if len(name) > 32 or len(name) < 2:
-            await context.bot.send_message(
-                chat_id=update.message.chat_id,
-                text="Change your nickname or avatar for blockchian of rum group.\nUse command as `/profile your-nickname` , nickname should be 2-32 characters, and you can add a picture as avatar.",
-                reply_to_message_id=update.message.message_id,
-            )
+            reply = "Change your nickname or avatar for blockchian of rum group.\nUse command as `/profile your-nickname` , nickname should be 2-32 characters, and you can add a picture as avatar."
+            await update.message.reply_text(reply)
             return
         _photo = update.message.photo
         if _photo:
             image = await context.bot.get_file(_photo[-1].file_id)
             avatar = bytes(await image.download_as_bytearray())
         else:
             avatar = None
@@ -436,108 +422,114 @@
             self.rum.change_account(user.pvtkey)
             resp = self.rum.api.post_content(data)
             if "trx_id" in resp:
                 reply += f"Profile updated. View {self.config.FEED_URL_BASE}/users/{address}"
             else:
                 reply += "Profile update failed. Please try again later."
 
-        await context.bot.send_message(
-            chat_id=update.message.chat_id,
-            text=reply,
-            reply_to_message_id=update.message.message_id,
-        )
+        await update.message.reply_text(reply)
 
     async def command_show_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
-        logger.info("start command_show_pvtkey")
+        logger.info("start command_show_pvtkey %s", update.message.message_id)
         userid = update.message.from_user.id
         username = update.message.from_user.username
-        chat_id = update.message.chat_id
-        message_id = update.message.message_id
         user = self.db.init_user(userid, username)
         if user:
             text = f"Your private key (please keep it safe) is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others) is:\n```\n{user.address}\n```"
         else:
             text = f"show_key error {userid}"
-        await context.bot.send_message(
-            chat_id=chat_id,
-            text=text,
-            reply_to_message_id=message_id,
-            parse_mode="Markdown",
-        )
+
+        await update.message.reply_text(text, parse_mode="Markdown")
 
     async def command_new_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
-        logger.info("start command_new_pvtkey")
+        logger.info("start command_new_pvtkey %s", update.message.message_id)
         userid = update.message.from_user.id
         username = update.message.from_user.username
-        chat_id = update.message.chat_id
-        message_id = update.message.message_id
         user = self.db.init_user(userid, username, is_cover=True)
         if user:
             text = f"Your private key (please keep it safe) is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others) is:\n```\n{user.address}\n```"
         else:
             text = f"new_key error {userid}"
 
-        await context.bot.send_message(
-            chat_id=chat_id,
-            text=text,
-            reply_to_message_id=message_id,
-            parse_mode="Markdown",
-        )
+        await update.message.reply_text(text, parse_mode="Markdown")
 
     async def command_import_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
-        logger.info("start command_import_pvtkey")
+        logger.info("start command_import_pvtkey %s", update.message.message_id)
         userid = update.message.from_user.id
         username = update.message.from_user.username
-        chat_id = update.message.chat_id
-        message_id = update.message.message_id
         _text = update.message.text or update.message.caption or ""
         pvtkey = _text.replace("/import_pvtkey", "").strip(" '\"")
         text = f"Try to import private key: \n```\n{pvtkey}\n```\n"
         try:
-            account.private_key_to_pubkey(pvtkey)
+            pvtkey_to_pubkey(pvtkey)
             user = self.db.init_user(userid, username, pvtkey=pvtkey, is_cover=True)
             if user:
                 text += "Success. Please keep it safe."
             else:
                 text += "Something wrong. Please try again later."
         except Exception as err:
             logger.error(err)
             text += "Please Use command as `/import_key 0x5ee77ca3c261cdd...adeffaf` . Please check your private key and try again."
 
-        await context.bot.send_message(
-            chat_id=chat_id,
-            text=text,
-            reply_to_message_id=message_id,
-            parse_mode="Markdown",
-        )
+        await update.message.reply_text(text, parse_mode="Markdown")
+
+    def get_all_trxs(self, senders, start_trx=None):
+        trxs = self.rum.api.get_content(senders=senders, start_trx=start_trx, num=20)
+        if len(trxs) == 0:
+            return None
+        for i in trxs:
+            yield i
+        return self.get_all_trxs(senders, trxs[-1]["trx_id"])
+
+    async def command_export_data(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
+        logger.info("start command_export_data %s", update.message.message_id)
+        userid = update.message.from_user.id
+        user = self.db.get_first_user(userid)
+
+        if not user:
+            reply = "You have not registered yet. Please use command as `/new_key` to register."
+            await update.message.reply_text(reply)
+            return
+
+        trxs = [i for i in self.get_all_trxs([user.pubkey]) if i]
+        # create file-like object in memory
+        data = json.dumps(trxs).encode("utf-8")
+        with io.BytesIO(data) as buffer:
+            buffer.seek(0)
+            # send file to user
+            await context.bot.send_document(
+                chat_id=update.message.chat_id,
+                document=buffer,
+                filename=f"{user.pubkey}_{datetime.date.today()}.json",
+                reply_to_message_id=update.message.message_id,
+            )
+
+        reply = f"You have exported your data, that is {len(trxs)} trxs in blockchain of rum-group.\nYour private key is:\n```{user.pvtkey}```\nPlease keep it safe."
+        await update.message.reply_text(reply, parse_mode="Markdown")
 
     async def command_my_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_my_nft")
         # TODO
 
     async def command_grant_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_grant_nft")
         userid = update.message.from_user.id
         if userid not in self.config.ADMIN_USERIDS:
-            reply = "You are not admin."
-            await context.bot.send_message(
-                chat_id=update.message.chat_id,
-                text=reply,
-                reply_to_message_id=update.message.message_id,
-            )
+            await update.message.reply_text("You are not admin.")
             return
         # TODO
 
     def run(self):
         self.app.add_handler(CommandHandler("start", self.command_start))
         self.app.add_handler(CommandHandler("profile", self.command_profile))
         self.app.add_handler(CommandHandler("show_pvtkey", self.command_show_pvtkey))
         # TODO: add logs to map userid and pvtkey
         self.app.add_handler(CommandHandler("new_pvtkey", self.command_new_pvtkey))
         self.app.add_handler(CommandHandler("import_pvtkey", self.command_import_pvtkey))
+        self.app.add_handler(CommandHandler("export_data", self.command_export_data))
         # TODO:
         self.app.add_handler(CommandHandler("my_nft", self.command_my_nft))
         self.app.add_handler(CommandHandler("grant_nft", self.command_grant_nft))
 
         content_filter = (filters.TEXT | filters.PHOTO) & ~filters.COMMAND
         # private chat message:
         # send to tg channel and rum group as new post
```

### Comparing `rum_with_telegram-0.8.7/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.8/rum_with_telegram/db_handle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,80 @@
-import logging
-
-from quorum_mininode_py.crypto import account
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker
-
-from rum_with_telegram.module import Base, Relation, User
-
-logger = logging.getLogger(__name__)
-
-
-class DBHandle:
-    def __init__(self, db_url: str, echo: bool = False):
-        logger.info("db_url: %s", db_url)
-        self.engine = create_engine(db_url, echo=echo)
-        self.Session = sessionmaker(bind=self.engine)
-        Base.metadata.create_all(self.engine)
-
-    def init_user(self, userid, username=None, pvtkey=None, is_cover=False):
-        _user = self.get_first(User, {"user_id": userid}, "user_id")
-        if _user and not is_cover:
-            return _user
-        pvtkey = pvtkey or account.create_private_key()
-
-        try:
-            pubkey = account.private_key_to_pubkey(pvtkey)
-            address = account.private_key_to_address(pvtkey)
-        except Exception as err:
-            logger.error("init_user: %s", err)
-            return None
-
-        user = {
-            "user_id": userid,
-            "username": username,
-            "pvtkey": pvtkey,
-            "pubkey": pubkey,
-            "address": address,
-        }
-        self.add_or_update(User, user, "user_id")
-        return self.get_first(User, {"user_id": userid}, "user_id")
-
-    def get_first(self, table, payload: dict, pk: str):
-        with self.Session() as session:
-            return session.query(table).filter_by(**{pk: payload[pk]}).first()
-
-    def get_all(self, table, payload: dict, pk: str):
-        with self.Session() as session:
-            return session.query(table).filter_by(**{pk: payload[pk]}).all()
-
-    def get_trx_sent(self, channel_message_id):
-        with self.Session() as session:
-            relation = (
-                session.query(Relation)
-                .filter_by(channel_message_id=channel_message_id, chat_type="private")
-                .first()
-            )
-            if relation and relation.trx_id:
-                return relation
-            relations = (
-                session.query(Relation).filter_by(channel_message_id=channel_message_id).all()
-            )
-            for relation in relations:
-                if relation.trx_id:
-                    return relation
-        return None
-
-    def is_exist(self, table, payload: dict, pk: str):
-        with self.Session() as session:
-            return session.query(table).filter_by(**{pk: payload[pk]}).count() > 0
-
-    def add_or_update(self, table, payload, pk):
-        with self.Session() as session:
-            obj = session.query(table).filter_by(**{pk: payload[pk]}).first()
-            if obj:
-                session.query(table).filter_by(**{pk: payload[pk]}).update(payload)
-                logger.info("update to db: %s %s", pk, payload[pk])
-            else:
-                obj = table(**payload)
-                session.add(obj)
-                logger.info("add to db: %s %s", pk, payload[pk])
-            try:
-                session.commit()
-            except Exception as err:
-                session.rollback()
-                logger.info(err)
+import logging
+
+from quorum_mininode_py import RumAccount
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+
+from rum_with_telegram.module import Base, Relation, User
+
+logger = logging.getLogger(__name__)
+
+
+class DBHandle:
+    def __init__(self, db_url: str, echo: bool = False):
+        logger.info("db_url: %s", db_url)
+        self.engine = create_engine(db_url, echo=echo)
+        self.Session = sessionmaker(bind=self.engine)
+        Base.metadata.create_all(self.engine)
+
+    def init_user(self, userid, username=None, pvtkey=None, is_cover=False):
+        _user = self.get_first_user(userid)
+        if _user and not is_cover:
+            return _user
+        account = RumAccount(pvtkey=pvtkey)
+        user = {
+            "user_id": userid,
+            "username": username,
+            "pvtkey": account.pvtkey,
+            "pubkey": account.pubkey,
+            "address": account.address,
+        }
+        self.add_or_update(User, user, "user_id")
+        return self.get_first_user(userid)
+
+    def get_first(self, table, payload: dict, pk: str):
+        with self.Session() as session:
+            return session.query(table).filter_by(**{pk: payload[pk]}).first()
+
+    def get_first_user(self, userid):
+        return self.get_first(User, {"user_id": userid}, "user_id")
+
+    def get_all(self, table, payload: dict, pk: str):
+        with self.Session() as session:
+            return session.query(table).filter_by(**{pk: payload[pk]}).all()
+
+    def get_trx_sent(self, channel_message_id):
+        with self.Session() as session:
+            relation = (
+                session.query(Relation)
+                .filter_by(channel_message_id=channel_message_id, chat_type="private")
+                .first()
+            )
+            if relation and relation.trx_id:
+                return relation
+            relations = (
+                session.query(Relation).filter_by(channel_message_id=channel_message_id).all()
+            )
+            for relation in relations:
+                if relation.trx_id:
+                    return relation
+        return None
+
+    def is_exist(self, table, payload: dict, pk: str):
+        with self.Session() as session:
+            return session.query(table).filter_by(**{pk: payload[pk]}).count() > 0
+
+    def add_or_update(self, table, payload, pk):
+        with self.Session() as session:
+            obj = session.query(table).filter_by(**{pk: payload[pk]}).first()
+            if obj:
+                session.query(table).filter_by(**{pk: payload[pk]}).update(payload)
+                logger.info("update to db: %s %s", pk, payload[pk])
+            else:
+                obj = table(**payload)
+                session.add(obj)
+                logger.info("add to db: %s %s", pk, payload[pk])
+            try:
+                session.commit()
+            except Exception as err:
+                session.rollback()
+                logger.info(err)
```

### Comparing `rum_with_telegram-0.8.7/rum_with_telegram/module.py` & `rum_with_telegram-0.8.8/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.7/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.8/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.7
+Version: 0.8.8
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.7/setup.py` & `rum_with_telegram-0.8.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.7",
+    version="0.8.8",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
@@ -30,10 +30,9 @@
     packages=setuptools.find_packages(exclude=["example"]),
     python_requires=">=3.7",
     install_requires=[
         "python-telegram-bot==20.2",
         "quorum-data-py",
         "quorum-mininode-py",
         "sqlalchemy",
-        "eth-account==0.5.8",
     ],
 )
```

