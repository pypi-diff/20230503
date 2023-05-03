# Comparing `tmp/botanix-0.1.0.tar.gz` & `tmp/botanix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botanix-0.1.0.tar", last modified: Sun Apr 30 14:42:27 2023, max compression
+gzip compressed data, was "botanix-0.2.0.tar", last modified: Wed May  3 15:05:58 2023, max compression
```

## Comparing `botanix-0.1.0.tar` & `botanix-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-04-30 14:42:27.349649 botanix-0.1.0/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.1.0/LICENSE
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-04-30 14:42:27.349756 botanix-0.1.0/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8168 2023-04-29 08:54:44.000000 botanix-0.1.0/README.md
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-04-30 14:42:27.348034 botanix-0.1.0/botanix/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.1.0/botanix/__init__.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.1.0/botanix/conversion_helper.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8357 2023-04-28 19:36:13.000000 botanix-0.1.0/botanix/handling.py
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-04-30 14:42:27.349438 botanix-0.1.0/botanix.egg-info/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-04-30 14:42:27.000000 botanix-0.1.0/botanix.egg-info/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-04-30 14:42:27.000000 botanix-0.1.0/botanix.egg-info/SOURCES.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-04-30 14:42:27.000000 botanix-0.1.0/botanix.egg-info/dependency_links.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-04-30 14:42:27.000000 botanix-0.1.0/botanix.egg-info/requires.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-04-30 14:42:27.000000 botanix-0.1.0/botanix.egg-info/top_level.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-04-30 14:42:27.350278 botanix-0.1.0/setup.cfg
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      372 2023-04-30 14:19:57.000000 botanix-0.1.0/setup.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 15:05:58.529034 botanix-0.2.0/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.2.0/LICENSE
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 15:05:58.529153 botanix-0.2.0/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8991 2023-05-01 07:52:10.000000 botanix-0.2.0/README.md
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 15:05:58.526913 botanix-0.2.0/botanix/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.2.0/botanix/__init__.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.2.0/botanix/conversion_helper.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8391 2023-05-03 09:12:41.000000 botanix-0.2.0/botanix/handling.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 15:05:58.528809 botanix-0.2.0/botanix.egg-info/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 15:05:58.000000 botanix-0.2.0/botanix.egg-info/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-05-03 15:05:58.000000 botanix-0.2.0/botanix.egg-info/SOURCES.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-05-03 15:05:58.000000 botanix-0.2.0/botanix.egg-info/dependency_links.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-05-03 15:05:58.000000 botanix-0.2.0/botanix.egg-info/requires.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-05-03 15:05:58.000000 botanix-0.2.0/botanix.egg-info/top_level.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-05-03 15:05:58.529583 botanix-0.2.0/setup.cfg
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      372 2023-05-03 15:05:37.000000 botanix-0.2.0/setup.py
```

### Comparing `botanix-0.1.0/LICENSE` & `botanix-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botanix-0.1.0/README.md` & `botanix-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -182,7 +182,13 @@
     result = m.handle(uid, message, u)
     if not result.handled:
       bot.send_message(uid, text='Sorry did not get it.')
   except Exception as ex:
     traceback.print_exc()
     bot.send_message(uid, text='There was an error. Please try again.')
 ```
+
+### Special Handlers: StartHandler and HelpHandler
+`botanix` considers Help and Start as generic handlers and treats them slightly differently in the sense that the updates that have `/start` or `/help` will be treated as calling them even if the user is midway in an established track. This means that if, for example, your `RegisterHandler` asks user's name and in response, the user types `/start`, then this message will not be received by that handler but by your `StartHandler`.
+
+This behaviour is governed by `MainHandler.generic_handler_names` which has the value `['help', 'start']`. You can change this behaviour by setting it to `[]` but typically you are meant to create `StartHandler` and `HelpHandler` and this behaviour is desirable since it provides a short-circuit to start again or see the help output.
+
```

### Comparing `botanix-0.1.0/botanix/conversion_helper.py` & `botanix-0.2.0/botanix/conversion_helper.py`

 * *Files identical despite different names*

### Comparing `botanix-0.1.0/botanix/handling.py` & `botanix-0.2.0/botanix/handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 class UnhandledMessage(Exception):
   def __init__(self, *args):
     super().__init__(args)
 
 
 class HandlingContext:
-  def __init__(self, uid:int, track_name:str, step:int=0):
+  def __init__(self, uid:int, track_nam:str, step:int=0):
     self.uid = uid
-    self.track_name = track_name
+    self.track_name = track_nam
     self.custom = {}
     self.timestamp = get_time_as_decimal()
     self.step = step
 
   def put_custom(self, key:str, val):
     """
     Puts a custom value in the context
@@ -124,24 +124,24 @@
 #
 class BaseHandler:
   handler_method_pattern = '[_A-Za-z0-9]+_(\d+)'
 
   def __init__(self):
     self.step_handlers = None
 
-  def handle(self, command: str, update: Update, context: HandlingContext) -> HandlingResult:
+  async def handle(self, command: str, update: Update, context: HandlingContext) -> HandlingResult:
     self.ensure_steps_built()
     uid = context.uid
     step = context.step
     if step not in self.step_handlers:
       raise UnhandledMessage(
         f'Step {step} does not exist in class {self.__class__.__name__}. Command was {command} and user id {uid}')
     last_result = HandlingResult.success_result()
     for h in self.step_handlers[step]:
-      last_result = h(command, update, context)
+      last_result = await h(command, update, context)
       if last_result.handled:
         return last_result # break out
     return last_result
 
   def get_class_name(self):
     if hasattr(self.__class__, 'track_name'):
       return self.__class__.track_name.lower()
@@ -174,19 +174,19 @@
     """
     Returns active contex
     :param uid:
     :return:
     """
     pass
 
-  def new_context(self, uid: int, track_name: str) -> HandlingContext:
+  def new_context(self, uid: int, track_nam: str) -> HandlingContext:
     """
     Creates, stores and returns a new context
     :param uid:
-    :param track_name:
+    :param track_nam:
     :return:
     """
     pass
 
   def put_context(self, uid: int, context: HandlingContext) -> None:
     """
     Updates the stored context
@@ -212,38 +212,38 @@
 
   def __init__(self, store: BaseContextStore, *list_of_handlers: BaseHandler):
     self.handlers = {}
     self.store = store
     for h in list_of_handlers:
       self.handlers[h.get_class_name()] = h
 
-  def handle(self, uid: int, message_text: str, update: Update) -> HandlingResult:
+  async def handle(self, uid: int, message_text: str, update: Update) -> HandlingResult:
     message_text = message_text.lower()
     ctx = self.store.get_active_context(uid)
     m = re.match(MainHandler.command_pattern, message_text)
     if m is None:
       if ctx is None:
         return HandlingResult.unhandled_result('Your choice does not exist.')
       else:
-        track_name = ctx.track_name
-        if track_name not in self.handlers:
+        track_nam = ctx.track_name
+        if track_nam not in self.handlers:
           raise UnhandledMessage(f'Could not find a handler for command {message_text}')
-        return self._do_handle(uid, message_text, update, ctx, track_name)
+        return await self._do_handle(uid, message_text, update, ctx, track_nam)
     else:  # this is a top level command (start of a track)
       class_command = m.groups()[0]  # is the same as track_name
       if class_command not in self.handlers:
         raise UnhandledMessage(f'Could not find a handler for command {message_text}')
       if class_command in MainHandler.generic_handler_names:
-        ctx = HandlingContext(uid, track_name=class_command) # create a dummy context and not store since they do not have follow up
+        ctx = HandlingContext(uid, track_nam=class_command) # create a dummy context and not store since they do not have follow up
       else:
         ctx = self.store.new_context(uid, class_command)  # renew context
-      return self._do_handle(uid, message_text, update, ctx, class_command)
+      return await self._do_handle(uid, message_text, update, ctx, class_command)
 
-  def _do_handle(self, uid: int, command: str, update: Update, context: HandlingContext, class_command: str) -> HandlingResult:
-    result = self.handlers[class_command].handle(command, update, context)
+  async def _do_handle(self, uid: int, command: str, update: Update, context: HandlingContext, class_command: str) -> HandlingResult:
+    result = await self.handlers[class_command].handle(command, update, context)
     if result.handled and not result.is_terminal:
       if result.step_override is None:
         context.move_to_next()  # increase the step
       else:
         context.override_step(result.step_override)  # change the step
       self.store.put_context(uid, context)
     if result.is_terminal:
```

