# Comparing `tmp/wxtrio-0.2.1.tar.gz` & `tmp/wxtrio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxtrio-0.2.1.tar", last modified: Wed May  3 03:02:21 2023, max compression
+gzip compressed data, was "wxtrio-0.2.2.tar", last modified: Wed May  3 06:08:42 2023, max compression
```

## Comparing `wxtrio-0.2.1.tar` & `wxtrio-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.563202 wxtrio-0.2.1/
--rw-rw-rw-   0        0        0     1514 2023-02-02 02:46:51.000000 wxtrio-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      987 2023-05-03 03:02:21.563202 wxtrio-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-02-01 23:08:51.000000 wxtrio-0.2.1/README.md
--rw-rw-rw-   0        0        0     1124 2023-05-03 03:02:10.000000 wxtrio-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 03:02:21.563202 wxtrio-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.548680 wxtrio-0.2.1/wxtrio/
--rw-rw-rw-   0        0        0       43 2023-05-03 02:58:35.000000 wxtrio-0.2.1/wxtrio/__init__.py
--rw-rw-rw-   0        0        0    17902 2023-05-03 02:53:40.000000 wxtrio-0.2.1/wxtrio/core.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.562202 wxtrio-0.2.1/wxtrio.egg-info/
--rw-rw-rw-   0        0        0      987 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 06:08:42.847641 wxtrio-0.2.2/
+-rw-rw-rw-   0        0        0     1514 2023-02-02 02:46:51.000000 wxtrio-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      987 2023-05-03 06:08:42.846638 wxtrio-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-02-01 23:08:51.000000 wxtrio-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1124 2023-05-03 03:02:10.000000 wxtrio-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 06:08:42.847641 wxtrio-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 06:08:42.833196 wxtrio-0.2.2/wxtrio/
+-rw-rw-rw-   0        0        0       43 2023-05-03 06:02:42.000000 wxtrio-0.2.2/wxtrio/__init__.py
+-rw-rw-rw-   0        0        0    17053 2023-05-03 06:05:14.000000 wxtrio-0.2.2/wxtrio/core.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:08:42.846133 wxtrio-0.2.2/wxtrio.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-05-03 06:08:42.000000 wxtrio-0.2.2/wxtrio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-03 06:08:42.000000 wxtrio-0.2.2/wxtrio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:08:42.000000 wxtrio-0.2.2/wxtrio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-03 06:08:42.000000 wxtrio-0.2.2/wxtrio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 06:08:42.000000 wxtrio-0.2.2/wxtrio.egg-info/top_level.txt
```

### Comparing `wxtrio-0.2.1/LICENSE` & `wxtrio-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxtrio-0.2.1/PKG-INFO` & `wxtrio-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxtrio
-Version: 0.2.1
+Version: 0.2.2
 Summary: Async wxPtyon with trio.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/lojack5/wxtrio
 Keywords: wxPython,trio,async,GUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `wxtrio-0.2.1/pyproject.toml` & `wxtrio-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wxtrio-0.2.1/wxtrio/core.py` & `wxtrio-0.2.2/wxtrio/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     - StartCoroutine: launches a async function, tieing it to a wx window object.
     In the case of both AsyncBind and StartCoroutine, the async task will automatically
     be cancelled in the event that the window object is destroyed.
 """
 import inspect
 import warnings
 from collections import defaultdict
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from functools import partial
 from typing import (
     Any,
     Awaitable,
     Callable,
     Generic,
     ParamSpec,
@@ -117,18 +117,15 @@
             raise RuntimeError('No orignal method to call')
 
 
 SPAWN_TIMEOUT = 1  # Timeout to wait for a nursery when spawning a child task
 
 
 @dataclass(slots=True)
-class WindowBindingData:
-    event_handlers: defaultdict[int, list] = field(
-        default_factory=lambda: defaultdict(list)
-    )  # List of event handlers this window is async subscribed to
+class EvtHandlerNursery:
     nursery: trio.Nursery | None = (
         None  # nursury for launching tasks/event handler instances for this window
     )
     nursery_queued: bool = (
         False  # `True` when this window's nursury has be queued for creation
     )
 
@@ -139,15 +136,15 @@
         return self.nursery
 
 
 class App(wx.App):
     def __init__(self, *args, **kwargs) -> None:
         # TODO: implement non-guest mode option?
         self.nursery: trio.Nursery | None = None
-        self.handler_bindings = defaultdict(WindowBindingData)
+        self.handler_nurseries = defaultdict(EvtHandlerNursery)
         self.pending_tasks: list = []
         self._patch_evthandler_methods()
         super().__init__(*args, **kwargs)
 
     def _patch_evthandler_methods(self) -> None:
         """Patch the wx.EvtHandler methods with our replacements."""
         self._BindSync = MethodPatch(wx.EvtHandler, 'Bind', replacement_method=Bind)
@@ -183,28 +180,28 @@
         )
         return True
 
     def _trio_done_callback(self, trio_outcome) -> None:
         # Make sure wxPython shuts down,
         # As it may rely on some trio tasks that
         # have stopped
-        str(trio_outcome)  # unwrap any exceptions
+        trio_outcome.unwrap()
         wx.Exit()
 
     async def _trio_main(self) -> None:
         """Main async function to run under trio.  Simply creates
         needed nursuries to house upcoming async tasks, then
         waits forever, until cancelled when the wx.App gets
         shutdown.
         """
         async with trio.open_nursery() as nursery:
             # 1) Create the main trio nursery
             self.nursery = nursery
             # 2) Create nurseries for each window for long running tasks
-            for evthandler in self.handler_bindings:
+            for evthandler in self.handler_nurseries:
                 self.nursery.start_soon(self._build_nursery, evthandler)
             # 3) Start any pending tasks
             for evthandler, coroutine in self.pending_tasks:
                 self.nursery.start_soon(self._spawn_into, evthandler, coroutine)
             # Set `pending_tasks` to None to cause an exception if used later
             self.pending_tasks = None  # type: ignore
             # Wait until the application exits
@@ -219,27 +216,15 @@
         id: int = wx.ID_ANY,
         id2: int = wx.ID_ANY,
     ) -> None:
         """Binds an event handler to a wx Event callback.  Automatically detects if the
         handler is async or sync, and bind appropriately.
         """
         if inspect.iscoroutinefunction(handler):
-            # 'async def' function that has not been called
-            self._queue_cleanup(evthandler)
-            self.handler_bindings[evthandler].event_handlers[
-                event_binder.typeId
-            ].append(handler)
-            self._BindSync(
-                evthandler,
-                event_binder,
-                lambda event: self.OnEvent(event, evthandler, event_binder.typeId),
-                source=source,
-                id=id,
-                id2=id2,
-            )
+            self.AsyncBind(evthandler, event_binder, handler, source, id, id2)
         elif inspect.iscoroutine(handler):
             # 'async def' function that has been called and returned an awaitable object
             raise TypeError(
                 'Event handler is an awaitable object returned from an async function. '
                 'Do not call the async function.'
             )
         elif inspect.isawaitable(handler):
@@ -255,17 +240,17 @@
             handler = cast(SyncHandler, handler)
             self._BindSync(
                 evthandler, event_binder, handler, source=source, id=id, id2=id2
             )
 
     def AsyncBind(
         self,
+        evthandler: wx.EvtHandler,
         event_binder: wx.PyEventBinder,
         handler: AsyncHandler,
-        evthandler: wx.EvtHandler,
         source=None,
         id: int = wx.ID_ANY,
         id2: int = wx.ID_ANY,
     ) -> None:
         """Bind a coroutine as a wx Event callback on the given wx EvtHandler.
         Note: when evthandler is destroyed, any running corouting bound to it will be
             cancelled.
@@ -276,78 +261,75 @@
         id: Used to specify the source of the event by ID, instead of instance
         id2: Used (when needed) to specify a range of IDs, for example with
             EVT_MENU_RANGE.
         """
         if not inspect.iscoroutinefunction(handler):
             raise TypeError('async_handler must be a async function or coroutine.')
         self._queue_cleanup(evthandler)
-        self.handler_bindings[evthandler].event_handlers[event_binder.typeId].append(
-            handler
-        )
         self._BindSync(
             evthandler,
             event_binder,
-            lambda event: self.OnEvent(event, evthandler, event_binder.typeId),
+            lambda event: self.OnEvent(evthandler, handler, event),
             source=source,
             id=id,
             id2=id2,
         )
 
     def _queue_cleanup(self, evthandler: wx.EvtHandler) -> None:
         """By 'cleanup' we mean: establish a nursery for this evthandler that can then
         be cancelled when the evthandler gets destroyed, cleaning up any associated
         tasks.
         """
-        bindings = self.handler_bindings[evthandler]
+        handler_nursery = self.handler_nurseries[evthandler]
         # If a nursery does not yet exist for this event handler:
         #  - If there is a main nursery, launch a task to create a sub-nursery for our
         #    event handler
         #  - If not, wait until the main loops starts, nurseries will be created then
         if (
             self.nursery is not None
-            and bindings.nursery is None
-            and not bindings.nursery_queued
+            and handler_nursery.nursery is None
+            and not handler_nursery.nursery_queued
         ):
-            bindings.nursery_queued = True
+            handler_nursery.nursery_queued = True
             self.nursery.start_soon(self._build_nursery, evthandler)
 
     async def _build_nursery(self, evthandler: wx.EvtHandler) -> None:
         """Create a nursery for managing tasks associated with the wx EvtHandler
         object.
         """
-        if self.handler_bindings[evthandler].nursery is not None:
+        if self.handler_nurseries[evthandler].nursery is not None:
             # Trying to create a nursery twice is a code smell
             warnings.warn(
                 f'Attempted to create nursery for {evthandler} multiple times.'
             )
         async with trio.open_nursery() as nursery:
-            bindings = self.handler_bindings[evthandler]
-            bindings.nursery = nursery
+            handler_nursery = self.handler_nurseries[evthandler]
+            handler_nursery.nursery = nursery
             # TODO: EVT_WINDOW_DESTROY might not be triggered for non-window EvtHandler
             # objects, monkey patch Destroy instead?
             self._BindSync(
                 evthandler,
                 wx.EVT_WINDOW_DESTROY,
                 lambda event: self.OnDestroy(event, evthandler),
                 evthandler,
             )
             await trio.sleep_forever()
         # We reach here when the nursery has been cancelled, ie: when OnDestroy is
         # triggered for this EvtHandler.
-        del self.handler_bindings[evthandler]
+        del self.handler_nurseries[evthandler]
 
     async def _spawn_into(
         self, evthandler: wx.EvtHandler, coroutine: AsyncMethod
     ) -> None:
         """Spawn the child coroutine into the nursery associated with the wx_window."""
         with trio.move_on_after(SPAWN_TIMEOUT) as cancel_scope:
             # The wx EvtHandler's nursery may not be set up fully yet,
             # _build_nursery was queued in trio, but might not have begun to run,
             # so wait up to 10 seconds.
-            nursery = await self.handler_bindings[evthandler].wait_nursery()
+            nursery = await self.handler_nurseries[evthandler].wait_nursery()
         if cancel_scope.cancelled_caught:
             raise RuntimeError(f'Failed to nursery for {evthandler}, timed out.')
         nursery.start_soon(coroutine)
 
     def StartCoroutine(
         self,
         evthandler: wx.EvtHandler,
@@ -369,34 +351,31 @@
             self._BindSync(
                 evthandler,
                 wx.EVT_CLOSE,
                 lambda event: self.OnDestroy(event, evthandler),
                 evthandler,
             )
 
-    def OnEvent(
-        self, event: wx.Event, evthandler: wx.EvtHandler, event_id: int
-    ) -> None:
+    def OnEvent(self, evthandler: wx.EvtHandler, handler, event: wx.Event) -> None:
         """An event occurred for something we've bound to an async event handler."""
-        bindings = self.handler_bindings[evthandler]
-        for async_handler in bindings.event_handlers[event_id]:
-            # if this even handler is bound already, the nurser is in fact created
-            bindings.nursery.start_soon(async_handler, event.Clone())  # type: ignore
+        bindings = self.handler_nurseries[evthandler]
+        if bindings.nursery:
+            bindings.nursery.start_soon(handler, event.Clone())
 
     def OnDestroy(self, event: wx.Event, evthandler: wx.EvtHandler) -> None:
         """Clean up any running tasks associated with the EvtHandler that is being
         destroyed.
         """
         self.CancelCoroutines(evthandler)
         event.Skip()
 
     def CancelCoroutines(self, evthandler: wx.EvtHandler) -> None:
         """Cancel all trio coroutines associated with an EvtHandler."""
-        if evthandler in self.handler_bindings:
-            if nursery := self.handler_bindings[evthandler].nursery:
+        if evthandler in self.handler_nurseries:
+            if nursery := self.handler_nurseries[evthandler].nursery:
                 nursery.cancel_scope.cancel()
 
 
 def get_app() -> App:
     """Return the wx.App instance, or raise an exception if it is not a wxtrio.App."""
     app = wx.App.Get()
     if not isinstance(app, App):
@@ -422,15 +401,15 @@
     evthandler: wx.EvtHandler,
     event: wx.PyEventBinder,
     handler: AsyncHandler,
     source=None,
     id: int = wx.ID_ANY,
     id2: int = wx.ID_ANY,
 ) -> None:
-    get_app().AsyncBind(event, handler, evthandler, source, id, id2)
+    get_app().AsyncBind(evthandler, event, handler, source, id, id2)
 
 
 def StartCoroutine(
     evthandler: wx.EvtHandler,
     coroutine: Callable[..., Awaitable[Any]],
     bind_onclose: bool = True,
 ) -> None:
```

### Comparing `wxtrio-0.2.1/wxtrio.egg-info/PKG-INFO` & `wxtrio-0.2.2/wxtrio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxtrio
-Version: 0.2.1
+Version: 0.2.2
 Summary: Async wxPtyon with trio.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/lojack5/wxtrio
 Keywords: wxPython,trio,async,GUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

