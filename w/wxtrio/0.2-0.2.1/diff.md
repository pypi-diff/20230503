# Comparing `tmp/wxtrio-0.2.tar.gz` & `tmp/wxtrio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxtrio-0.2.tar", last modified: Thu Feb  4 23:37:12 2021, max compression
+gzip compressed data, was "wxtrio-0.2.1.tar", last modified: Wed May  3 03:02:21 2023, max compression
```

## Comparing `wxtrio-0.2.tar` & `wxtrio-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-02-04 23:37:12.024437 wxtrio-0.2/
--rw-rw-rw-   0        0        0     1155 2021-02-04 23:37:12.023461 wxtrio-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      440 2020-08-11 16:41:16.000000 wxtrio-0.2/README.md
--rw-rw-rw-   0        0        0       42 2021-02-04 23:37:12.024437 wxtrio-0.2/setup.cfg
--rw-rw-rw-   0        0        0      968 2021-02-04 23:00:56.000000 wxtrio-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-04 23:37:11.965916 wxtrio-0.2/wxtrio/
--rw-rw-rw-   0        0        0       20 2020-08-11 16:41:16.000000 wxtrio-0.2/wxtrio/__init__.py
--rw-rw-rw-   0        0        0    14591 2021-01-16 00:38:58.000000 wxtrio-0.2/wxtrio/core.py
-drwxrwxrwx   0        0        0        0 2021-02-04 23:37:12.021510 wxtrio-0.2/wxtrio.egg-info/
--rw-rw-rw-   0        0        0     1155 2021-02-04 23:37:11.000000 wxtrio-0.2/wxtrio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2021-02-04 23:37:11.000000 wxtrio-0.2/wxtrio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-04 23:37:11.000000 wxtrio-0.2/wxtrio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2021-02-04 23:37:11.000000 wxtrio-0.2/wxtrio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-02-04 23:37:11.000000 wxtrio-0.2/wxtrio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.563202 wxtrio-0.2.1/
+-rw-rw-rw-   0        0        0     1514 2023-02-02 02:46:51.000000 wxtrio-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      987 2023-05-03 03:02:21.563202 wxtrio-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-02-01 23:08:51.000000 wxtrio-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1124 2023-05-03 03:02:10.000000 wxtrio-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:02:21.563202 wxtrio-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.548680 wxtrio-0.2.1/wxtrio/
+-rw-rw-rw-   0        0        0       43 2023-05-03 02:58:35.000000 wxtrio-0.2.1/wxtrio/__init__.py
+-rw-rw-rw-   0        0        0    17902 2023-05-03 02:53:40.000000 wxtrio-0.2.1/wxtrio/core.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:02:21.562202 wxtrio-0.2.1/wxtrio.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 03:02:21.000000 wxtrio-0.2.1/wxtrio.egg-info/top_level.txt
```

### Comparing `wxtrio-0.2/wxtrio/core.py` & `wxtrio-0.2.1/wxtrio/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,314 +1,477 @@
 """Implementation allowing wxPython to use async functions via trio.
    This is done by running trio in guest mode under wxPython.  The
    details are handled by wxtrio.App, a repleacement for wx.App
-   
+
    Additionally, async window even handlers can now be bound to window
    events.  All of this is handled automatically via monkey patching the
-   wx.Window.Bind method.  Finally, helper async functions are provided:
+   wx.EvtHandler.Bind method.  Finally, helper async functions are provided:
     - AsyncBind: a version of wx.Bind that accepts async functions for callbacks
     - DynamicBind: a version of wx.Bind that automatically determines whether to use the
-          syncronous or asyncronous version.  This is what wx.Window.Bind has been replace with.
-    - AsyncShowDialog: a version of wx.ShowDialog that processes a non-modal dialog asynchronously
+          syncronous or asyncronous version.  This is what wx.EvtHandler.Bind has been
+          replace with.
+    - AsyncShowDialog: a version of wx.ShowDialog that processes a non-modal dialog
+          asynchronously
     - StartCoroutine: launches a async function, tieing it to a wx window object.
-    In the case of both AsyncBind and StartCoroutine, the async task will automatically be
-    cancelled in the event that the window object is destroyed.
+    In the case of both AsyncBind and StartCoroutine, the async task will automatically
+    be cancelled in the event that the window object is destroyed.
 """
 import inspect
+import warnings
 from collections import defaultdict
+from dataclasses import dataclass, field
 from functools import partial
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Generic,
+    ParamSpec,
+    TypeVar,
+    cast,
+)
 
-import wx
 import trio
-import attr
+import wx
 
 # Commonly used trio core functionality
 from trio import sleep
 
+P = ParamSpec('P')
+T = TypeVar('T')
+SyncHandler = Callable[[wx.Event], None]
+AsyncHandler = Callable[[wx.Event], Awaitable[None]]
+EventHandler = SyncHandler | AsyncHandler
+AsyncMethod = Callable[P, Awaitable[T]]
+
 
 __all__ = [
     'sleep',
-    'App', 'Bind', 'AsyncBind', 'StartCoroutine', 'AsyncShowDialog',
+    'App',
+    'Bind',
+    'AsyncBind',
+    'StartCoroutine',
+    'AsyncShowDialog',
 ]
 
 
-class MethodPatch:
-    __slots__ = ('getter', 'setter', 'original_method', 'installed_method', )
-
-    def __init__(self, cls, method_name, *, replacement_method=None):
+class MethodPatch(Generic[P, T]):
+    __slots__ = (
+        'getter',
+        'setter',
+        'original_method',
+        'installed_method',
+    )
+
+    def __init__(
+        self,
+        cls: type,
+        method_name: str,
+        *,
+        replacement_method: Callable[P, T] | None = None,
+    ):
         self.getter = partial(getattr, cls, method_name, None)
         self.setter = partial(setattr, cls, method_name)
         self.original_method = self.getter()
         self.installed_method = None
         if replacement_method is not None:
             self.install(replacement_method)
 
-    def install(self, replacement_method):
+    def install(self, replacement_method: Callable[P, T]):
         current_method = self.getter()
         if current_method == self.original_method:
             # Original method currently in place, good to patch
             self.setter(replacement_method)
             self.installed_method = replacement_method
         elif current_method == self.installed_method:
             # Already installed, good to go
             pass
+        elif self.original_method is not None:
+            warnings.warn(
+                f'Unknown replacement method for {self.original_method.__name__} in '
+                'place, skipping install.'
+            )
         else:
-            raise Warning(f'Unknown replacement method for {self.original_method.__name__} in place, skipping install.')
+            warnings.warn(
+                f'Unknown method {current_method} in place, skipping install.'
+            )
 
     def uninstall(self):
         current_method = self.getter()
-        if current_method == self.installed_method:
+        if current_method is self.installed_method:
             self.setter(self.original_method)
-            self.installed_method = None
-        elif self.installed_method is not None:
-            raise Warning(f'Unknown replacement method for {self.original_method.__name__} in place, cannot uninstall.')
+            self.installed_method = self.original_method
+        elif self.installed_method is not None and self.original_method:
+            warnings.warn(
+                f'Unknown replacement method for {self.original_method.__name__} in '
+                'place, cannot uninstall.'
+            )
+        else:
+            # Should never get here
+            raise RuntimeError('Unknown error')
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
         """Call the original method."""
-        return self.original_method(*args, **kwargs)
+        if self.original_method:
+            return self.original_method(*args, **kwargs)
+        else:
+            raise RuntimeError('No orignal method to call')
 
 
-SPAWN_TIMEOUT = 1   # Timeout to wait for a nursery when spawning a child task
+SPAWN_TIMEOUT = 1  # Timeout to wait for a nursery when spawning a child task
 
 
-@attr.s(slots=True)
+@dataclass(slots=True)
 class WindowBindingData:
-    event_handlers = attr.ib(default=defaultdict(list)) # List of event handlers this window is async subscribed to
-    nursery = attr.ib(default=None) # nursury for launching tasks/event handler instances for this window
-    nursery_queued = attr.ib(default=False) # `True` when this window's nursury has be queued for creation
+    event_handlers: defaultdict[int, list] = field(
+        default_factory=lambda: defaultdict(list)
+    )  # List of event handlers this window is async subscribed to
+    nursery: trio.Nursery | None = (
+        None  # nursury for launching tasks/event handler instances for this window
+    )
+    nursery_queued: bool = (
+        False  # `True` when this window's nursury has be queued for creation
+    )
 
-    async def wait_nursery(self):
+    async def wait_nursery(self) -> trio.Nursery:
         """Wait until this windows's nursury object is created."""
         while self.nursery is None:
             await trio.sleep(0.1)
+        return self.nursery
 
 
 class App(wx.App):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         # TODO: implement non-guest mode option?
-        self.nursery = None
-        self.window_bindings = defaultdict(WindowBindingData)
-        self.pending_tasks = []
-        self._patch_window_methods()
+        self.nursery: trio.Nursery | None = None
+        self.handler_bindings = defaultdict(WindowBindingData)
+        self.pending_tasks: list = []
+        self._patch_evthandler_methods()
         super().__init__(*args, **kwargs)
 
-    def _patch_window_methods(self):
-        """Patch the wx.Window methods with our replacements."""
-        self._BindSync = MethodPatch(wx.Window, 'Bind', replacement_method=Bind)
-        self._StartCoroutinePatch = MethodPatch(wx.Window, 'StartCoroutine', replacement_method=StartCoroutine)
-        self._CancelCoroutinePatch = MethodPatch(wx.Window, 'CancelCoroutines', replacement_method=self.CancelCoroutines)
+    def _patch_evthandler_methods(self) -> None:
+        """Patch the wx.EvtHandler methods with our replacements."""
+        self._BindSync = MethodPatch(wx.EvtHandler, 'Bind', replacement_method=Bind)
+        self._StartCoroutinePatch = MethodPatch(
+            wx.EvtHandler, 'StartCoroutine', replacement_method=StartCoroutine
+        )
+        self._CancelCoroutinePatch = MethodPatch(
+            wx.EvtHandler, 'CancelCoroutines', replacement_method=self.CancelCoroutines
+        )
 
-    def _unpatch_window_methods(self):
-        """Uninstall replacement methods from wx.Window."""
+    def _unpatch_evthandler_methods(self) -> None:
+        """Uninstall replacement methods from wx.EvtHandler."""
         self._BindSync.uninstall()
         self._StartCoroutinePatch.uninstall()
         self._CancelCoroutinePatch.uninstall()
 
-    def ExitMainLoop(self):
-        """Called internally by wxPython to signal that the main application should exit."""
-        self.nursery.cancel_scope.cancel()
-        self._unpatch_window_methods()
+    def ExitMainLoop(self) -> None:
+        """Called internally by wxPython to signal that the main application should
+        exit.
+        """
+        self._unpatch_evthandler_methods()
+        if self.nursery:
+            self.nursery.cancel_scope.cancel()
         super().ExitMainLoop()
 
-    def OnInit(self):
+    def OnInit(self) -> bool:
         """Called by wxPython once it is in a state ready to begin the main loop."""
         # Start trio in guest mode
         trio.lowlevel.start_guest_run(
             self._trio_main,
             run_sync_soon_threadsafe=wx.CallAfter,
             done_callback=self._trio_done_callback,
         )
         return True
 
-    def _trio_done_callback(self, trio_outcome):
+    def _trio_done_callback(self, trio_outcome) -> None:
         # Make sure wxPython shuts down,
         # As it may rely on some trio tasks that
         # have stopped
+        str(trio_outcome)  # unwrap any exceptions
         wx.Exit()
 
-    async def _trio_main(self):
+    async def _trio_main(self) -> None:
         """Main async function to run under trio.  Simply creates
-           needed nursuries to house upcoming async tasks, then
-           waits forever, until cancelled when the wx.App gets
-           shutdown.
+        needed nursuries to house upcoming async tasks, then
+        waits forever, until cancelled when the wx.App gets
+        shutdown.
         """
         async with trio.open_nursery() as nursery:
             # 1) Create the main trio nursery
             self.nursery = nursery
             # 2) Create nurseries for each window for long running tasks
-            for wx_window in self.window_bindings:
-                self.nursery.start_soon(self._build_nursery, wx_window)
+            for evthandler in self.handler_bindings:
+                self.nursery.start_soon(self._build_nursery, evthandler)
             # 3) Start any pending tasks
-            for wx_window, coroutine in self.pending_tasks:
-                self.nursery.start_soon(self._spawn_into, wx_window, coroutine)
-            self.pending_tasks = None
+            for evthandler, coroutine in self.pending_tasks:
+                self.nursery.start_soon(self._spawn_into, evthandler, coroutine)
+            # Set `pending_tasks` to None to cause an exception if used later
+            self.pending_tasks = None  # type: ignore
             # Wait until the application exits
             await trio.sleep_forever()
 
-    def DynamicBind(self, wx_window, wx_event_binder, handler, source=None, id=wx.ID_ANY, id2=wx.ID_ANY):
-        """Binds an event handler to a wx Event callback.  Automatically detects if the handler
-           is async or sync, and bind appropriately.
+    def DynamicBind(
+        self,
+        evthandler: wx.EvtHandler,
+        event_binder: wx.PyEventBinder,
+        handler: EventHandler,
+        source=None,
+        id: int = wx.ID_ANY,
+        id2: int = wx.ID_ANY,
+    ) -> None:
+        """Binds an event handler to a wx Event callback.  Automatically detects if the
+        handler is async or sync, and bind appropriately.
         """
         if inspect.iscoroutinefunction(handler):
             # 'async def' function that has not been called
-            self._queue_cleanup(wx_window)
-            self.window_bindings[wx_window].event_handlers[wx_event_binder.typeId].append(handler)
-            self._BindSync(wx_window, wx_event_binder, lambda event: self.OnEvent(event, wx_window, wx_event_binder.typeId), source=source, id=id, id2=id2)
+            self._queue_cleanup(evthandler)
+            self.handler_bindings[evthandler].event_handlers[
+                event_binder.typeId
+            ].append(handler)
+            self._BindSync(
+                evthandler,
+                event_binder,
+                lambda event: self.OnEvent(event, evthandler, event_binder.typeId),
+                source=source,
+                id=id,
+                id2=id2,
+            )
         elif inspect.iscoroutine(handler):
             # 'async def' function that has been called and returned an awaitable object
-            raise TypeError('Event handler is an awaitable object returned from an async function.  Do not call the async function.')
+            raise TypeError(
+                'Event handler is an awaitable object returned from an async function. '
+                'Do not call the async function.'
+            )
         elif inspect.isawaitable(handler):
             # Some other awaitable object
-            raise TypeError('Event handler is an awaitable object.  Pass either a function or an async function.')
+            raise TypeError(
+                'Event handler is an awaitable object.  Pass either a function or an '
+                'async function.'
+            )
         elif not callable(handler):
             raise TypeError('Event handler is not callable.')
         else:
             # Sync event handler
-            self._BindSync(wx_window, wx_event_binder, handler, source=source, id=id, id2=id2)
-
-    def AsyncBind(self, wx_event_binder, async_handler, wx_window, source=None, id=wx.ID_ANY, id2=wx.ID_ANY):
-        """Bind a coroutine as a wx Event callback on the given wx_window.
-           Note: when wx_window is destroyed, any running corouting bount to it will be cancelled.
-           wx_event: One of the wx.EVT_* event binding objects
-           async_handler: Your async function that will handle the event
-           source: Part of the wx event handling system (for distinguising between events of the same
-                   type, but originating from different source child windows
-           id: Used to specify the source of the event by ID, instead of instance
-           id2: Used (when needed) to specify a range of IDs, for example with EVT_MENU_RANGE.
+            handler = cast(SyncHandler, handler)
+            self._BindSync(
+                evthandler, event_binder, handler, source=source, id=id, id2=id2
+            )
+
+    def AsyncBind(
+        self,
+        event_binder: wx.PyEventBinder,
+        handler: AsyncHandler,
+        evthandler: wx.EvtHandler,
+        source=None,
+        id: int = wx.ID_ANY,
+        id2: int = wx.ID_ANY,
+    ) -> None:
+        """Bind a coroutine as a wx Event callback on the given wx EvtHandler.
+        Note: when evthandler is destroyed, any running corouting bound to it will be
+            cancelled.
+        wx_event: One of the wx.EVT_* event binding objects
+        async_handler: Your async function that will handle the event
+        source: Part of the wx event handling system (for distinguising between events
+            of the same type, but originating from different source child windows
+        id: Used to specify the source of the event by ID, instead of instance
+        id2: Used (when needed) to specify a range of IDs, for example with
+            EVT_MENU_RANGE.
         """
-        if not inspect.iscoroutinefunction(async_handler):
+        if not inspect.iscoroutinefunction(handler):
             raise TypeError('async_handler must be a async function or coroutine.')
-        self._queue_cleanup(wx_window)
-        self.window_bindings[wx_window].event_handlers[wx_event_binder.typeId].append(async_handler)
-        self._BindSync(wx_window, wx_event_binder, lambda event: self.OnEvent(event, wx_window, wx_event_binder.typeId), source=source, id=id, id2=id2)
-
-    def _queue_cleanup(self, wx_window):
-        """By 'cleanup' we mean: establish a nursery for this window that can then be
-           cancelled when the window gets destroyed, cleaning up any associated tasks.
+        self._queue_cleanup(evthandler)
+        self.handler_bindings[evthandler].event_handlers[event_binder.typeId].append(
+            handler
+        )
+        self._BindSync(
+            evthandler,
+            event_binder,
+            lambda event: self.OnEvent(event, evthandler, event_binder.typeId),
+            source=source,
+            id=id,
+            id2=id2,
+        )
+
+    def _queue_cleanup(self, evthandler: wx.EvtHandler) -> None:
+        """By 'cleanup' we mean: establish a nursery for this evthandler that can then
+        be cancelled when the evthandler gets destroyed, cleaning up any associated
+        tasks.
         """
-        bindings = self.window_bindings[wx_window]
-        # If a nursery does not yet exist for this window:
-        #  - If there is a main nursery, launch a task to create a sub-nursery for our window
+        bindings = self.handler_bindings[evthandler]
+        # If a nursery does not yet exist for this event handler:
+        #  - If there is a main nursery, launch a task to create a sub-nursery for our
+        #    event handler
         #  - If not, wait until the main loops starts, nurseries will be created then
-        if self.nursery is not None and bindings.nursery is None and not bindings.nursery_queued:
+        if (
+            self.nursery is not None
+            and bindings.nursery is None
+            and not bindings.nursery_queued
+        ):
             bindings.nursery_queued = True
-            self.nursery.start_soon(self._build_nursery, wx_window)
+            self.nursery.start_soon(self._build_nursery, evthandler)
 
-    async def _build_nursery(self, wx_window):
-        """Create a nursery for managing tasks associated with the wx_window object."""
-        if self.window_bindings[wx_window].nursery is not None:
+    async def _build_nursery(self, evthandler: wx.EvtHandler) -> None:
+        """Create a nursery for managing tasks associated with the wx EvtHandler
+        object.
+        """
+        if self.handler_bindings[evthandler].nursery is not None:
             # Trying to create a nursery twice is a code smell
-            raise Warning(f'Attempted to create nursery for {wx_window} multiple times.')
+            warnings.warn(
+                f'Attempted to create nursery for {evthandler} multiple times.'
+            )
         async with trio.open_nursery() as nursery:
-            bindings = self.window_bindings[wx_window]
+            bindings = self.handler_bindings[evthandler]
             bindings.nursery = nursery
-            self._BindSync(wx_window, wx.EVT_WINDOW_DESTROY, lambda event: self.OnDestroy(event, wx_window), wx_window)
+            # TODO: EVT_WINDOW_DESTROY might not be triggered for non-window EvtHandler
+            # objects, monkey patch Destroy instead?
+            self._BindSync(
+                evthandler,
+                wx.EVT_WINDOW_DESTROY,
+                lambda event: self.OnDestroy(event, evthandler),
+                evthandler,
+            )
             await trio.sleep_forever()
         # We reach here when the nursery has been cancelled, ie: when OnDestroy is
-        # triggered for this window.
-        del self.window_bindings[wx_window]
+        # triggered for this EvtHandler.
+        del self.handler_bindings[evthandler]
 
-    async def _spawn_into(self, wx_window, coroutine):
+    async def _spawn_into(
+        self, evthandler: wx.EvtHandler, coroutine: AsyncMethod
+    ) -> None:
         """Spawn the child coroutine into the nursery associated with the wx_window."""
         with trio.move_on_after(SPAWN_TIMEOUT) as cancel_scope:
-            # The wx_window's nursery may not be set up fully yet,
+            # The wx EvtHandler's nursery may not be set up fully yet,
             # _build_nursery was queued in trio, but might not have begun to run,
             # so wait up to 10 seconds.
-            await self.window_bindings[wx_window].wait_nursery()
+            nursery = await self.handler_bindings[evthandler].wait_nursery()
         if cancel_scope.cancelled_caught:
-            raise RuntimeError(f'Failed to nursery for {wx_window}, timed out.')
-        self.window_bindings[wx_window].nursery.start_soon(coroutine)
+            raise RuntimeError(f'Failed to nursery for {evthandler}, timed out.')
+        nursery.start_soon(coroutine)
 
-
-    def StartCoroutine(self, wx_window, coroutine, bind_onclose=True):
-        """Start a coroutine, and attach its lifetime to the `wx_window`.
-           If `bind_onclose`, then also bind a custom OnClose event handler
-           to cancel all associated coroutines.
+    def StartCoroutine(
+        self,
+        evthandler: wx.EvtHandler,
+        coroutine: AsyncMethod,
+        bind_onclose: bool = True,
+    ) -> None:
+        """Start a coroutine, and attach its lifetime to the wx EvtHandler. If
+        `bind_onclose`, then also bind a custom OnClose event handler to cancel all
+        associated coroutines.
         """
-        self._queue_cleanup(wx_window)
+        self._queue_cleanup(evthandler)
         if self.nursery is None:
             # No nursery yet, stash this task for later
-            self.pending_tasks.append((wx_window, coroutine))
+            self.pending_tasks.append((evthandler, coroutine))
         else:
             # Spawn it
-            self.nursery.start_soon(self._spawn_into, wx_window, coroutine)
+            self.nursery.start_soon(self._spawn_into, evthandler, coroutine)
         if bind_onclose:
-            self._BindSync(wx_window, wx.EVT_CLOSE, lambda event: self.OnDestroy(event, wx_window), wx_window)
-
-    def OnEvent(self, wx_event, wx_window, wx_event_id):
-        """An event occurred for something we've bound to an async event
-           handler.
+            self._BindSync(
+                evthandler,
+                wx.EVT_CLOSE,
+                lambda event: self.OnDestroy(event, evthandler),
+                evthandler,
+            )
+
+    def OnEvent(
+        self, event: wx.Event, evthandler: wx.EvtHandler, event_id: int
+    ) -> None:
+        """An event occurred for something we've bound to an async event handler."""
+        bindings = self.handler_bindings[evthandler]
+        for async_handler in bindings.event_handlers[event_id]:
+            # if this even handler is bound already, the nurser is in fact created
+            bindings.nursery.start_soon(async_handler, event.Clone())  # type: ignore
+
+    def OnDestroy(self, event: wx.Event, evthandler: wx.EvtHandler) -> None:
+        """Clean up any running tasks associated with the EvtHandler that is being
+        destroyed.
         """
-        bindings = self.window_bindings[wx_window]
-        for async_handler in bindings.event_handlers[wx_event_id]:
-            bindings.nursery.start_soon(async_handler, wx_event.Clone())
-
-    def OnDestroy(self, wx_event, wx_window):
-        """Clean up any running tasks associated with the window
-           that is being destroyed.
-        """
-        self.CancelCoroutines(wx_window)
-        wx_event.Skip()
+        self.CancelCoroutines(evthandler)
+        event.Skip()
 
-    def CancelCoroutines(self, wx_window):
-        """Cancel all trio coroutines associated with a window."""
-        if wx_window in self.window_bindings:
-            self.window_bindings[wx_window].nursery.cancel_scope.cancel()
+    def CancelCoroutines(self, evthandler: wx.EvtHandler) -> None:
+        """Cancel all trio coroutines associated with an EvtHandler."""
+        if evthandler in self.handler_bindings:
+            if nursery := self.handler_bindings[evthandler].nursery:
+                nursery.cancel_scope.cancel()
 
 
-def Bind(wx_window, wx_event, handler, source=None, id=wx.ID_ANY, id2=wx.ID_ANY):
-    '''Initial Bind call.  Get the wx.App instance and verify it is a wxt.App
-       instance.
-    '''
+def get_app() -> App:
+    """Return the wx.App instance, or raise an exception if it is not a wxtrio.App."""
     app = wx.App.Get()
     if not isinstance(app, App):
         raise RuntimeError('wx App must be a wxtrio.App object')
-    app.DynamicBind(wx_window, wx_event, handler, source, id, id2)
+    return app
 
 
-def AsyncBind(wx_event, async_callback, wx_window, source=None, id=wx.ID_ANY, id2=wx.ID_ANY):
-    app = wx.App.Get()
-    if not isinstance(app, App):
-        raise RuntimeError('wx App must be a wxtrio.App object')
-    app.AsyncBind(wx_event, async_callback, wx_window, source, id, id2)
+def Bind(
+    evthandler: wx.EvtHandler,
+    event: wx.PyEventBinder,
+    handler: EventHandler,
+    source=None,
+    id: int = wx.ID_ANY,
+    id2: int = wx.ID_ANY,
+) -> None:
+    """Initial Bind call.  Get the wx.App instance and verify it is a wxt.App
+    instance.
+    """
+    get_app().DynamicBind(evthandler, event, handler, source, id, id2)
 
 
-def StartCoroutine(wx_window, coroutine, bind_onclose=True):
-    """Start a coroutine opened by `wx_window`.  If `bind_onclose`
-       then also binds a custom OnClose event handler to the window
-       which will cancel all coroutines.
+def AsyncBind(
+    evthandler: wx.EvtHandler,
+    event: wx.PyEventBinder,
+    handler: AsyncHandler,
+    source=None,
+    id: int = wx.ID_ANY,
+    id2: int = wx.ID_ANY,
+) -> None:
+    get_app().AsyncBind(event, handler, evthandler, source, id, id2)
+
+
+def StartCoroutine(
+    evthandler: wx.EvtHandler,
+    coroutine: Callable[..., Awaitable[Any]],
+    bind_onclose: bool = True,
+) -> None:
+    """Start a coroutine opened by `wx_window`.  If `bind_onclose` then also binds a
+    custom OnClose event handler to the window which will cancel all coroutines.
     """
-    app = wx.App.Get()
-    if not isinstance(app, App):
-        raise RuntimeError('wx App must be a wxtrio.App object')
-    app.StartCoroutine(wx_window, coroutine, bind_onclose)
+    get_app().StartCoroutine(evthandler, coroutine, bind_onclose)
 
 
-async def AsyncShowDialog(dialog):
+async def AsyncShowDialog(dialog: wx.Dialog) -> int:
     """Shows a non-modal wx Dialog asyncronously"""
     closed = trio.Event()
-    def end_dialog(return_code):
+
+    def end_dialog(return_code: int) -> None:
         dialog.SetReturnCode(return_code)
         dialog.Hide()
         closed.set()
-    def on_button(event):
+
+    def on_button(event: wx.Event) -> None:
         # Logic copied from src/common/dlgcmn.cpp:
         # wxDialogBase::OnButton, EndDialog, and AcceptAndClose
         event_id = event.GetId()
         if event_id == dialog.GetAffirmativeId():
             if dialog.Validate() and dialog.TransferDataFromWindow():
                 end_dialog(event_id)
         elif event_id == wx.ID_APPLY:
             if dialog.Validate():
                 dialog.TransferDataFromWindow()
-        elif event_id == dialog.GetEscapeId() or (event_id == wx.ID_CANCEL and dialog.GetEscapeId() == wx.ID_ANY):
+        elif event_id == dialog.GetEscapeId() or (
+            event_id == wx.ID_CANCEL and dialog.GetEscapeId() == wx.ID_ANY
+        ):
             end_dialog(wx.ID_CANCEL)
         else:
             event.Skip()
-    def on_close(event):
+
+    def on_close(event: wx.Event) -> None:
         closed.set()
         dialog.Hide()
+
     dialog.Bind(wx.EVT_CLOSE, on_close)
     dialog.Bind(wx.EVT_BUTTON, on_button)
     dialog.Show()
     await closed.wait()
     return dialog.GetReturnCode()
```

