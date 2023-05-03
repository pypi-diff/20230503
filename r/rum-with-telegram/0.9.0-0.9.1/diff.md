# Comparing `tmp/rum_with_telegram-0.9.0.tar.gz` & `tmp/rum_with_telegram-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.0.tar", last modified: Wed May  3 16:19:59 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.1.tar", last modified: Wed May  3 17:05:26 2023, max compression
```

## Comparing `rum_with_telegram-0.9.0.tar` & `rum_with_telegram-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 16:19:59.063266 rum_with_telegram-0.9.0/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-03 16:19:59.062265 rum_with_telegram-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.0/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-03 16:19:59.045201 rum_with_telegram-0.9.0/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-03 16:18:59.000000 rum_with_telegram-0.9.0/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.9.0/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    24439 2023-05-03 16:19:06.000000 rum_with_telegram-0.9.0/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3018 2023-05-03 15:18:36.000000 rum_with_telegram-0.9.0/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.9.0/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-03 16:19:59.055639 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-03 16:19:58.000000 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-03 16:19:58.000000 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 16:19:58.000000 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-03 16:19:58.000000 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 16:19:58.000000 rum_with_telegram-0.9.0/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 16:19:59.063266 rum_with_telegram-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-03 16:18:59.000000 rum_with_telegram-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.124428 rum_with_telegram-0.9.1/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-03 17:05:26.123430 rum_with_telegram-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.1/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.098176 rum_with_telegram-0.9.1/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-03 17:05:10.000000 rum_with_telegram-0.9.1/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.9.1/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25084 2023-05-03 17:04:42.000000 rum_with_telegram-0.9.1/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3411 2023-05-03 16:46:43.000000 rum_with_telegram-0.9.1/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-03 16:46:43.000000 rum_with_telegram-0.9.1/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.107908 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:05:26.124428 rum_with_telegram-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-03 17:05:10.000000 rum_with_telegram-0.9.1/setup.py
```

### Comparing `rum_with_telegram-0.9.0/LICENSE` & `rum_with_telegram-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.0/PKG-INFO` & `rum_with_telegram-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.0
+Version: 0.9.1
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.0/rum_with_telegram/config.py` & `rum_with_telegram-0.9.1/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.0/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.1/rum_with_telegram/data_exchanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from quorum_data_py import feed, get_trx_type, util
 from quorum_mininode_py import MiniNode, pvtkey_to_pubkey
 from telegram import Bot, Update
 from telegram.ext import Application, CommandHandler, ContextTypes, MessageHandler, filters
 
 from rum_with_telegram.config import get_config
 from rum_with_telegram.db_handle import DBHandle
-from rum_with_telegram.module import Relation
+from rum_with_telegram.module import Relation, UsedKey
 
 logger = logging.getLogger(__name__)
 
 
 class DataExchanger:
     """the data exchanger between telegram bot/channel/chat-group and rum group-chain"""
 
@@ -429,16 +429,19 @@
         await update.message.reply_text(reply)
 
     async def command_show_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_show_pvtkey %s", update.message.message_id)
         userid = update.message.from_user.id
         username = update.message.from_user.username
         user = self.db.init_user(userid, username)
+        used = self.db.get_all(UsedKey, {"user_id": userid}, "user_id") or []
         if user:
-            text = f"Your private key (please keep it safe) is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others) is:\n```\n{user.address}\n```"
+            text = f"Your private key (please keep it safe) now is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others)  now is:\n```\n{user.address}\n```"
+            for i in used:
+                text += f"\n\nUsed private key (please keep it safe) is: \n```\n{i.pvtkey}\n```\nUsed Address (can show to others) is:\n```\n{i.address}\n```"
         else:
             text = f"show_key error {userid}"
 
         await update.message.reply_text(text, parse_mode="Markdown")
 
     async def command_new_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_new_pvtkey %s", update.message.message_id)
@@ -486,28 +489,36 @@
         user = self.db.get_first_user(userid)
 
         if not user:
             reply = "You have not registered yet. Please use command as `/new_key` to register."
             await update.message.reply_text(reply)
             return
 
+        if user.export_at and user.export_at > datetime.datetime.now() - datetime.timedelta(
+            hours=1
+        ):
+            reply = "You have exported your data in one hour. Please try again later."
+            await update.message.reply_text(reply)
+            return
+
         trxs = [i for i in self.get_all_trxs([user.pubkey]) if i]
         if len(trxs) > 0:
             # create file-like object in memory
-            data = json.dumps(trxs, indent=4).encode("utf-8")
+            data = json.dumps(trxs, indent=4, ensure_ascii=False).encode("utf-8")
             with io.BytesIO(data) as buffer:
                 buffer.seek(0)
                 # send file to user
                 await context.bot.send_document(
                     chat_id=update.message.chat_id,
                     document=buffer,
                     filename=f"{datetime.date.today()}_export_data_{self.config.TG_BOT_NAME}.json",
                     reply_to_message_id=update.message.message_id,
                 )
             reply = f"You have exported your data, that is {len(trxs)} trxs in blockchain of rum-group.\nYour private key is:\n```{user.pvtkey}```\nPlease keep it safe."
+            self.db.update_user_export_at(userid)
         else:
             reply = "You have not any data in blockchain of rum-group."
         await update.message.reply_text(reply, parse_mode="Markdown")
 
     async def command_my_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_my_nft")
         # TODO
```

### Comparing `rum_with_telegram-0.9.0/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.1/rum_with_telegram/db_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import logging
 
 from quorum_mininode_py import RumAccount
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy.sql import func
 
-from rum_with_telegram.module import Base, Relation, User
+from rum_with_telegram.module import Base, Relation, UsedKey, User
 
 logger = logging.getLogger(__name__)
 
 
 class DBHandle:
     def __init__(self, db_url: str, echo: bool = False):
         logger.info("db_url: %s", db_url)
         self.engine = create_engine(db_url, echo=echo)
         self.Session = sessionmaker(bind=self.engine)
         Base.metadata.create_all(self.engine)
 
     def init_user(self, userid, username=None, pvtkey=None, is_cover=False):
         _user = self.get_first_user(userid)
-        if _user and not is_cover:
-            return _user
+        if _user:
+            if not is_cover:
+                return _user
+            used = {"user_id": userid, "pvtkey": _user.pvtkey}
+            self.add_or_update(UsedKey, used, "user_id")
         account = RumAccount(pvtkey=pvtkey)
         user = {
             "user_id": userid,
             "username": username,
             "pvtkey": account.pvtkey,
             "pubkey": account.pubkey,
             "address": account.address,
@@ -74,7 +78,12 @@
                 session.add(obj)
                 logger.info("add to db: %s %s", pk, payload[pk])
             try:
                 session.commit()
             except Exception as err:
                 session.rollback()
                 logger.info(err)
+
+    def update_user_export_at(self, userid):
+        with self.Session() as session:
+            session.query(User).filter_by(user_id=userid).update({"export_at": func.now()})
+            session.commit()
```

### Comparing `rum_with_telegram-0.9.0/rum_with_telegram/module.py` & `rum_with_telegram-0.9.1/rum_with_telegram/module.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,9 +34,17 @@
 
     id = Column(Integer, primary_key=True)
     user_id = Column(Integer, unique=True, index=True, default=None)
     username = Column(String, index=True, default=None)
     pvtkey = Column(String, unique=True, default=None)
     pubkey = Column(String, unique=True, default=None)
     address = Column(String, unique=True, default=None)
+    export_at = Column(DateTime, default=None)
     created_at = Column(DateTime, default=func.now())
     updated_at = Column(DateTime, onupdate=func.now())
+
+
+class UsedKey(Base):
+    __tablename__ = "used_keys"
+    id = Column(Integer, primary_key=True)
+    user_id = Column(Integer, index=True)
+    pvtkey = Column(String)
```

### Comparing `rum_with_telegram-0.9.0/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.1/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.0
+Version: 0.9.1
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.0/setup.py` & `rum_with_telegram-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.0",
+    version="0.9.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

