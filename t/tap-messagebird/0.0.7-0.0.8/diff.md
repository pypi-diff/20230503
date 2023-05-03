# Comparing `tmp/tap_messagebird-0.0.7.tar.gz` & `tmp/tap_messagebird-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_messagebird-0.0.7.tar", max compression
+gzip compressed data, was "tap_messagebird-0.0.8.tar", max compression
```

## Comparing `tap_messagebird-0.0.7.tar` & `tap_messagebird-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/LICENSE
--rw-r--r--   0        0        0     3370 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/README.md
--rw-r--r--   0        0        0     1208 2023-04-26 14:41:09.838933 tap_messagebird-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      117 2023-04-26 14:41:09.838933 tap_messagebird-0.0.7/tap_messagebird/__init__.py
--rw-r--r--   0        0        0     3857 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/client.py
--rw-r--r--   0        0        0     3044 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/schemas/conversation.json
--rw-r--r--   0        0        0      993 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/schemas/conversation_message.json
--rw-r--r--   0        0        0     4240 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/schemas/message.json
--rw-r--r--   0        0        0     5208 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/streams.py
--rw-r--r--   0        0        0     1590 2023-04-26 14:40:29.006779 tap_messagebird-0.0.7/tap_messagebird/tap.py
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 tap_messagebird-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 19:46:52.737018 tap_messagebird-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3380 2023-05-03 19:46:52.737018 tap_messagebird-0.0.8/README.md
+-rw-r--r--   0        0        0     1225 2023-05-03 19:47:10.681314 tap_messagebird-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-05-03 19:47:10.685314 tap_messagebird-0.0.8/tap_messagebird/__init__.py
+-rw-r--r--   0        0        0     3857 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/client.py
+-rw-r--r--   0        0        0     3329 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/conversation.json
+-rw-r--r--   0        0        0      993 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/conversation_message.json
+-rw-r--r--   0        0        0     4240 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/message.json
+-rw-r--r--   0        0        0     6789 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/streams.py
+-rw-r--r--   0        0        0     1590 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/tap.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 tap_messagebird-0.0.8/PKG-INFO
```

### Comparing `tap_messagebird-0.0.7/LICENSE` & `tap_messagebird-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.7/README.md` & `tap_messagebird-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Messagebird tap class.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
 ## Capabilities
 
 * `catalog`
+# `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
```

### Comparing `tap_messagebird-0.0.7/pyproject.toml` & `tap_messagebird-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "tap-messagebird"
-version = "0.0.7"
+version = "0.0.8"
 description = "`tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Meltano Team <hello@meltano.com>"]
 keywords = [
     "ELT",
     "Messagebird",
 ]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "<3.11,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = { version=">=0.24,<0.26"}
+singer-sdk = { version=">=0.24,<0.27"}
 fs-s3fs = { version = "^1.1.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 responses = "0.23.1"
 
 [tool.poetry.extras]
@@ -38,15 +38,15 @@
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.ruff]
-ignore = ["ANN101", "PLR2004", "N818"]
+ignore = ["ANN101", "PLR2004", "N818", "G004", "EM101"]
 select = ["ALL"]
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
 "scripts/*" = ["ANN", "D", "INP"]
 "tests/*" = ["ANN"]
```

### Comparing `tap_messagebird-0.0.7/tap_messagebird/client.py` & `tap_messagebird-0.0.8/tap_messagebird/client.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.7/tap_messagebird/schemas/conversation.json` & `tap_messagebird-0.0.8/tap_messagebird/schemas/conversation.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982717803030303%*

 * *Differences: {"'properties'": "{'contact': {'properties': {'createdDatetime': {'format': 'date-time'}, "*

 * *                 "'updatedDatetime': {'format': 'date-time'}}}, 'channels': {'items': "*

 * *                 "{'properties': {'createdDatetime': {'format': 'date-time'}, 'updatedDatetime': "*

 * *                 "{'format': 'date-time'}}}}, 'createdDatetime': {'format': 'date-time'}, "*

 * *                 "'updatedDatetime': {'format': 'date-time'}, 'lastReceivedDatetime': {'format': "*

 * *                 "'date-time'}}"}*

```diff
@@ -1,13 +1,14 @@
 {
     "properties": {
         "channels": {
             "items": {
                 "properties": {
                     "createdDatetime": {
+                        "format": "date-time",
                         "type": "string"
                     },
                     "id": {
                         "type": "string"
                     },
                     "name": {
                         "type": "string"
@@ -15,24 +16,26 @@
                     "platformId": {
                         "type": "string"
                     },
                     "status": {
                         "type": "string"
                     },
                     "updatedDatetime": {
+                        "format": "date-time",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
             "type": "array"
         },
         "contact": {
             "properties": {
                 "createdDatetime": {
+                    "format": "date-time",
                     "type": "string"
                 },
                 "customDetails": {
                     "properties": {
                         "custom1": {
                             "type": [
                                 "null",
@@ -72,32 +75,35 @@
                 "lastName": {
                     "type": "string"
                 },
                 "msisdn": {
                     "type": "integer"
                 },
                 "updatedDatetime": {
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": "object"
         },
         "contactId": {
             "type": "string"
         },
         "createdDatetime": {
+            "format": "date-time",
             "type": "string"
         },
         "id": {
             "type": "string"
         },
         "lastReceivedDatetime": {
+            "format": "date-time",
             "type": "string"
         },
         "lastUsedChannelId": {
             "type": "string"
         },
         "lastUsedPlatformId": {
             "type": "string"
@@ -113,12 +119,13 @@
             },
             "type": "object"
         },
         "status": {
             "type": "string"
         },
         "updatedDatetime": {
+            "format": "date-time",
             "type": "string"
         }
     },
     "type": "object"
 }
```

### Comparing `tap_messagebird-0.0.7/tap_messagebird/schemas/conversation_message.json` & `tap_messagebird-0.0.8/tap_messagebird/schemas/conversation_message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.7/tap_messagebird/schemas/message.json` & `tap_messagebird-0.0.8/tap_messagebird/schemas/message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.7/tap_messagebird/streams.py` & `tap_messagebird-0.0.8/tap_messagebird/streams.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Stream type classes for tap-messagebird."""
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable
+from typing import TYPE_CHECKING, Any, Iterable, cast
+
+import pendulum
 
 from tap_messagebird.client import MessagebirdOffsetPaginator, MessagebirdStream
 
 if TYPE_CHECKING:
     import requests
 
 
@@ -49,15 +51,15 @@
 
 class ConversationsStream(MessagebirdConversations):
     """Conversations stream."""
 
     name = "conversation"
     path = "/conversations"
     primary_keys = ["id"]
-    replication_key = None
+    replication_key = "lastReceivedDatetime"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "conversation.json"
 
     def get_child_context(
         self,
         record: dict,
         context: dict | None,  # noqa: ARG002
@@ -66,42 +68,72 @@
         if record["status"] == "archived":
             return None
 
         return {
             "_sdc_conversations_id": record["id"],
         }
 
+    def get_records(self, context: dict | None) -> Iterable[dict[str, Any]]:
+        """Return a generator of record-type dictionary objects.
+
+        Each record emitted should be a dictionary of property names to their values.
+
+        Args:
+            context: Stream partition or context dictionary.
+
+        Yields:
+            One item per (possibly processed) record in the API.
+        """
+        starting_replication_key_value = self.get_starting_timestamp(context)
+        if starting_replication_key_value is None:
+            # Shouldn't be possible, but mypy complains
+            raise ValueError(  # noqa: TRY003
+                "No starting replication key value found.",
+            )
+        starting_replication_key_value = pendulum.instance(
+            starting_replication_key_value,
+        )
+
+        for record in self.request_records(context):
+            transformed_record = self.post_process(record, context)
+            if transformed_record is None:
+                # Record filtered out during post_process()
+                continue
+            record_last_received_datetime: pendulum.DateTime = cast(
+                pendulum.DateTime,
+                pendulum.parse(record[self.replication_key]),
+            )
+            # Conversations are returned in descending order, so we can stop
+            # There's no filtering paramater just this default ordering
+            if record_last_received_datetime < starting_replication_key_value:
+                self.logger.info(
+                    "Breaking after hitting a record with replication key %s < %s",
+                    record_last_received_datetime,
+                    starting_replication_key_value,
+                )
+                break
+            yield transformed_record
+
 
 class ConversationMessagesStream(MessagebirdConversations):
     """Conversation Messages stream.
 
-    Messages stream doesn't pull all messages.
+    This stream pulls WhatsApp messages, while the messages stream
+    doesn't seem to pull them.
     """
 
     name = "conversation_message"
     path = "/conversations/{_sdc_conversations_id}/messages"
     primary_keys = ["id"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "conversation_message.json"
     parent_stream_type = ConversationsStream
-
-    def get_url_params(
-        self,
-        context: dict | None,
-        next_page_token: Any | None,
-    ) -> dict[str, Any]:
-        """Return a dictionary of values to be used in URL parameterization."""
-        params = super().get_url_params(
-            context=context,
-            next_page_token=next_page_token,
-        )
-        if params.get("from") is None:
-            params["from"] = self.config["start_date"]
-        return params
+    # We don't need to track state per conversation
+    state_partitioning_keys: list[str] = []
 
     def get_records(self, context: dict | None) -> Iterable[dict[str, Any]]:
         """Return a generator of record-type dictionary objects.
 
         Each record emitted should be a dictionary of property names to their values.
 
         Args:
@@ -152,13 +184,14 @@
     ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization."""
         params = super().get_url_params(
             context=context,
             next_page_token=next_page_token,
         )
         if params.get("from") is None:
-            params["from"] = self.config["start_date"]
+            from_date = pendulum.parse(self.config["start_date"]).to_iso8601_string()
+            params["from"] = from_date
         return params
 
 
 class ConversationArchivedWarning(Exception):
     """Conversation is archived and we recieved an error."""
```

### Comparing `tap_messagebird-0.0.7/tap_messagebird/tap.py` & `tap_messagebird-0.0.8/tap_messagebird/tap.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.7/PKG-INFO` & `tap_messagebird-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: tap-messagebird
-Version: 0.0.7
+Version: 0.0.8
 Summary: `tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Messagebird
 Author: Meltano Team
 Author-email: hello@meltano.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: s3
 Requires-Dist: fs-s3fs (>=1.1.1,<2.0.0) ; extra == "s3"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: singer-sdk (>=0.24,<0.26)
+Requires-Dist: singer-sdk (>=0.24,<0.27)
 Description-Content-Type: text/markdown
 
 # `tap-messagebird`
 
 Messagebird tap class.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
 ## Capabilities
 
 * `catalog`
+# `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
```

