# Comparing `tmp/slackdoor-0.6.8.tar.gz` & `tmp/slackdoor-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackdoor-0.6.8.tar", max compression
+gzip compressed data, was "slackdoor-0.6.9.tar", max compression
```

## Comparing `slackdoor-0.6.8.tar` & `slackdoor-0.6.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2192 2022-12-10 17:52:41.000000 slackdoor-0.6.8/LICENSE
--rw-r--r--   0        0        0       22 2023-05-02 02:28:12.748175 slackdoor-0.6.8/door/__init__.py
--rw-r--r--   0        0        0    11040 2023-03-15 18:22:18.000000 slackdoor-0.6.8/door/core.py
--rw-r--r--   0        0        0     5142 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/decorators.py
--rw-r--r--   0        0        0    52953 2023-03-15 18:32:18.000000 slackdoor-0.6.8/door/dispatch.py
--rw-r--r--   0        0        0     5648 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/models/__init__.py
--rw-r--r--   0        0        0     1637 2023-03-15 18:26:59.000000 slackdoor-0.6.8/door/models/files/file.py
--rw-r--r--   0        0        0    13307 2023-03-15 18:27:19.000000 slackdoor-0.6.8/door/models/messages/message.py
--rw-r--r--   0        0        0      412 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/plugins/__init__.py
--rw-r--r--   0        0        0     1656 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/base.py
--rw-r--r--   0        0        0     2507 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/commands/leave.py
--rw-r--r--   0        0        0     2097 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/plugins/examples/channel_joined.py
--rw-r--r--   0        0        0     3858 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/plugins/examples/general.py
--rw-r--r--   0        0        0      898 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/run.py
--rw-r--r--   0        0        0     4298 2023-03-15 18:50:59.000000 slackdoor-0.6.8/door/sentry.py
--rw-r--r--   0        0        0     1895 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/settings.py
--rw-r--r--   0        0        0    22537 2023-03-15 18:29:02.000000 slackdoor-0.6.8/door/slack.py
--rw-r--r--   0        0        0     7266 2023-05-02 02:26:45.689997 slackdoor-0.6.8/door/utils/__init__.py
--rw-r--r--   0        0        0      980 2023-03-15 18:18:02.000000 slackdoor-0.6.8/door/utils/collections.py
--rw-r--r--   0        0        0     2442 2023-01-29 20:50:33.000000 slackdoor-0.6.8/door/utils/interactive.py
--rw-r--r--   0        0        0      966 2022-12-10 17:52:41.000000 slackdoor-0.6.8/door/utils/plugins.py
--rw-r--r--   0        0        0     2317 2023-05-02 02:28:12.740232 slackdoor-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 slackdoor-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     2192 2022-12-10 17:52:41.000000 slackdoor-0.6.9/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-02 23:56:54.621577 slackdoor-0.6.9/door/__init__.py
+-rw-r--r--   0        0        0    11040 2023-03-15 18:22:18.000000 slackdoor-0.6.9/door/core.py
+-rw-r--r--   0        0        0     5142 2023-03-15 18:18:02.000000 slackdoor-0.6.9/door/decorators.py
+-rw-r--r--   0        0        0    53228 2023-05-02 23:55:45.796112 slackdoor-0.6.9/door/dispatch.py
+-rw-r--r--   0        0        0     5648 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/models/__init__.py
+-rw-r--r--   0        0        0     1637 2023-03-15 18:26:59.000000 slackdoor-0.6.9/door/models/files/file.py
+-rw-r--r--   0        0        0    13307 2023-03-15 18:27:19.000000 slackdoor-0.6.9/door/models/messages/message.py
+-rw-r--r--   0        0        0      412 2023-03-15 18:18:02.000000 slackdoor-0.6.9/door/plugins/__init__.py
+-rw-r--r--   0        0        0     1656 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/plugins/base.py
+-rw-r--r--   0        0        0     2507 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/plugins/commands/leave.py
+-rw-r--r--   0        0        0     2097 2023-03-15 18:18:02.000000 slackdoor-0.6.9/door/plugins/examples/channel_joined.py
+-rw-r--r--   0        0        0     3858 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/plugins/examples/general.py
+-rw-r--r--   0        0        0      898 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/run.py
+-rw-r--r--   0        0        0     4298 2023-03-15 18:50:59.000000 slackdoor-0.6.9/door/sentry.py
+-rw-r--r--   0        0        0     1895 2023-03-15 18:18:02.000000 slackdoor-0.6.9/door/settings.py
+-rw-r--r--   0        0        0    22537 2023-03-15 18:29:02.000000 slackdoor-0.6.9/door/slack.py
+-rw-r--r--   0        0        0     7369 2023-05-02 22:19:26.991393 slackdoor-0.6.9/door/utils/__init__.py
+-rw-r--r--   0        0        0      980 2023-03-15 18:18:02.000000 slackdoor-0.6.9/door/utils/collections.py
+-rw-r--r--   0        0        0     2442 2023-01-29 20:50:33.000000 slackdoor-0.6.9/door/utils/interactive.py
+-rw-r--r--   0        0        0      966 2022-12-10 17:52:41.000000 slackdoor-0.6.9/door/utils/plugins.py
+-rw-r--r--   0        0        0     2317 2023-05-02 23:56:54.611334 slackdoor-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 slackdoor-0.6.9/PKG-INFO
```

### Comparing `slackdoor-0.6.8/LICENSE` & `slackdoor-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/core.py` & `slackdoor-0.6.9/door/core.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/decorators.py` & `slackdoor-0.6.9/door/decorators.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/dispatch.py` & `slackdoor-0.6.9/door/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from door.plugins import PluginHandler
 from door.utils.interactive import ephemeral_notification, generic_dismiss_message_button, ack_open_url_button
 from door.models.files.file import File
 from door.models.messages.message import Message, MultiMessage
 from door.sentry import adjust_start
 from door.slack import Slack
-from door.utils import Plural, partial_mask
+from door.utils import Plural, partial_mask, strip_mrkdwn
 
 from sentry_sdk import start_transaction, start_span, set_user, set_tag, capture_exception
 
 
 @dataclass(frozen=True, slots=True)
 class MessageHandlerResponse:
     message: Message | None = None
@@ -315,14 +315,18 @@
         text = re.sub(r"```(.+?)```", _get_next_code_block, text, flags=re.DOTALL)
         text = re.sub(r"`(.+?)`", _get_next_backtick_block, text)
 
         # Slack encodes &, < and > because they are used internally... which means we can't match on "&"
         # FIXME: what could go wrong by doing this?
         text = text.replace("&amp;", "&")
 
+        # Remove bold/italic formatting, but don't strip URLs (or groups) because some plugins
+        # may need to detect whether a "trigger" occurs inside a URL to be able to ignore it
+        text = strip_mrkdwn(text, strip_urls=False, strip_groups=False)
+
         return text, codeblocks, backticks
 
     async def _process_message_handlers(  # noqa: PLR0912
         self, text: str, message: dict[str, Any], client: AsyncWebClient, context: AsyncBoltContext, logger: Logger
     ) -> MessageHandlerResponse | None:
         """
         Given a message event, process it for triggers and return the response(s)
```

### Comparing `slackdoor-0.6.8/door/models/__init__.py` & `slackdoor-0.6.9/door/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/models/files/file.py` & `slackdoor-0.6.9/door/models/files/file.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/models/messages/message.py` & `slackdoor-0.6.9/door/models/messages/message.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/plugins/base.py` & `slackdoor-0.6.9/door/plugins/base.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/plugins/commands/leave.py` & `slackdoor-0.6.9/door/plugins/commands/leave.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/plugins/examples/channel_joined.py` & `slackdoor-0.6.9/door/plugins/examples/channel_joined.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/plugins/examples/general.py` & `slackdoor-0.6.9/door/plugins/examples/general.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/run.py` & `slackdoor-0.6.9/door/run.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/sentry.py` & `slackdoor-0.6.9/door/sentry.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/settings.py` & `slackdoor-0.6.9/door/settings.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/slack.py` & `slackdoor-0.6.9/door/slack.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/utils/__init__.py` & `slackdoor-0.6.9/door/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,21 +106,23 @@
 
 
 def fix_timestamp(timestamp: str) -> str:
     # convert Z to +00:00 (RFC 3339 format), or change ±0000 to ±00:00, so datetime.fromisoformat works
     return re.sub(r"[+-](\d\d)(\d\d)$", r"+\1:\2", timestamp.replace("Z", "+00:00"))
 
 
-def strip_mrkdwn(text: str) -> str:
+def strip_mrkdwn(text: str, *, strip_urls: bool = True, strip_groups: bool = True) -> str:
     """Strip Slack-flavored 'mrkdwn' formatting"""
     text = re.sub(r"\*_((?:\S)(?:.*?))_\*", r"\1", text)  # strip *_..._*
     text = re.sub(r"_\*((?:\S)(?:.*?))\*_", r"\1", text)  # strip *_..._*
     text = re.sub(r"([*_])((?:\S)(?:.*?))(?:\1)", r"\2", text)  # strip *...* or _..._
-    text = re.sub(r"<(?!!)([^>]+?)(?:\|[^>]+?)?>", r"\1", text)  # strip URLs
-    text = re.sub(r"(?:<![^>]+?\|)([^>]+?)(?:>)", r"\1", text)  # strip Slack ! links (<!subteam^SXYZ|@groupname>)
+    if strip_urls:
+        text = re.sub(r"<(?!!)([^>]+?)(?:\|[^>]+?)?>", r"\1", text)  # strip URLs
+    if strip_groups:
+        text = re.sub(r"(?:<![^>]+?\|)([^>]+?)(?:>)", r"\1", text)  # strip Slack ! links (<!subteam^SXYZ|@groupname>)
     return text.replace("\n", " • ")
 
 
 def ensure_slack_ts(ts: str) -> str:
     """Ensure the timestamp is Slack-compatible by adding the '.' if necessary"""
     if not isinstance(ts, str):
         ts = str(ts)
```

### Comparing `slackdoor-0.6.8/door/utils/collections.py` & `slackdoor-0.6.9/door/utils/collections.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/utils/interactive.py` & `slackdoor-0.6.9/door/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/door/utils/plugins.py` & `slackdoor-0.6.9/door/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `slackdoor-0.6.8/pyproject.toml` & `slackdoor-0.6.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors = ["Eddy G <eddyg@users.noreply.github.com>"]
 license = "MIT"
 repository = "https://github.com/eddyg/slackdoor"
 packages = [
     {include = "door"}
 ]
 
-version = "0.6.8"
+version = "0.6.9"
 # NOTE: uses the 'poetry_bumpversion' plugin to keep versions in sync
 # Use:
 #   poetry version {patch|minor|major|prepatch|preminor|premajor|prerelease}
 # to bump the version and have it be "authoritative" here and in __init__
 # To tag:
 #   git tag $(awk -F'"' '/^version =/{print $2}' pyproject.toml)
 #   git push -o ci.skip && git push --tags
```

### Comparing `slackdoor-0.6.8/PKG-INFO` & `slackdoor-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackdoor
-Version: 0.6.8
+Version: 0.6.9
 Summary: An opinionated and powerful chatbot framework for Slack
 Home-page: https://github.com/eddyg/slackdoor
 License: MIT
 Author: Eddy G
 Author-email: eddyg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

