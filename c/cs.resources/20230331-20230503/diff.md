# Comparing `tmp/cs.resources-20230331.tar.gz` & `tmp/cs.resources-20230503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20230331.tar", last modified: Fri Mar 31 10:25:38 2023, max compression
+gzip compressed data, was "cs.resources-20230503.tar", last modified: Wed May  3 11:00:32 2023, max compression
```

## Comparing `cs.resources-20230331.tar` & `cs.resources-20230503.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:25:38.625817 cs.resources-20230331/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-03-31 10:25:06.000000 cs.resources-20230331/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    10672 2023-03-31 10:25:38.625951 cs.resources-20230331/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    14938 2023-03-31 10:25:12.000000 cs.resources-20230331/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:25:38.621684 cs.resources-20230331/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:25:38.622039 cs.resources-20230331/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:25:38.623875 cs.resources-20230331/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    25289 2023-03-31 10:24:50.000000 cs.resources-20230331/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:25:38.625547 cs.resources-20230331/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    10672 2023-03-31 10:25:38.000000 cs.resources-20230331/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      316 2023-03-31 10:25:38.000000 cs.resources-20230331/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-03-31 10:25:38.000000 cs.resources-20230331/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      180 2023-03-31 10:25:38.000000 cs.resources-20230331/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-03-31 10:25:38.000000 cs.resources-20230331/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    11065 2023-03-31 10:25:29.000000 cs.resources-20230331/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      999 2023-03-31 10:25:38.626545 cs.resources-20230331/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-03-31 10:25:12.000000 cs.resources-20230331/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-03 11:00:32.897973 cs.resources-20230503/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-05-03 10:59:50.000000 cs.resources-20230503/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10560 2023-05-03 11:00:32.898153 cs.resources-20230503/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14921 2023-05-03 10:59:57.000000 cs.resources-20230503/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-03 11:00:32.892877 cs.resources-20230503/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-03 11:00:32.893280 cs.resources-20230503/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-03 11:00:32.895622 cs.resources-20230503/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    25834 2023-05-03 10:59:34.000000 cs.resources-20230503/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-03 11:00:32.897640 cs.resources-20230503/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10560 2023-05-03 11:00:32.000000 cs.resources-20230503/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      316 2023-05-03 11:00:32.000000 cs.resources-20230503/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-05-03 11:00:32.000000 cs.resources-20230503/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      180 2023-05-03 11:00:32.000000 cs.resources-20230503/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-05-03 11:00:32.000000 cs.resources-20230503/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10953 2023-05-03 11:00:17.000000 cs.resources-20230503/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      999 2023-05-03 11:00:32.898871 cs.resources-20230503/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-05-03 10:59:57.000000 cs.resources-20230503/setup.py
```

### Comparing `cs.resources-20230331/PKG-INFO` & `cs.resources-20230503/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20230331
+Version: 20230503
 Summary: Resource management classes and functions.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,18 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20230331*:
-* @uses_runstate: use the prevailing RunState or create one.
-* MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
-* bugfix: _mom_state.open: only set self._teardown when opens==1.
+*Latest release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
 
 ## Class `ClosedError(builtins.Exception, builtins.BaseException)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
 
@@ -182,14 +180,17 @@
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
 # Release Log
 
 
 
+*Release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
+
 *Release 20230331*:
 * @uses_runstate: use the prevailing RunState or create one.
 * MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
 * bugfix: _mom_state.open: only set self._teardown when opens==1.
 
 *Release 20230217*:
 MultiOpenMixin: __repr__ for the state object.
```

### Comparing `cs.resources-20230331/README.md` & `cs.resources-20230503/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Resource management classes and functions.
 
-*Latest release 20230331*:
-* @uses_runstate: use the prevailing RunState or create one.
-* MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
-* bugfix: _mom_state.open: only set self._teardown when opens==1.
+*Latest release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
 
 ## Class `ClosedError(builtins.Exception, builtins.BaseException)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
 
@@ -246,14 +244,17 @@
 
 *Method `RunState.__nonzero__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.cancel(self)`*:
 Set the cancelled flag; the associated process should notice and stop.
 
+*Property `RunState.cancelled`*:
+Test the .cancelled attribute, including a poll if supplied.
+
 *Method `RunState.catch_signal(self, sig, call_previous=False, handle_signal=None)`*:
 Context manager to catch the signal or signals `sig` and
 cancel this `RunState`.
 Restores the previous handlers on exit.
 Yield a mapping of `sig`=>`old_handler`.
 
 Parameters:
@@ -322,14 +323,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
+
 *Release 20230331*:
 * @uses_runstate: use the prevailing RunState or create one.
 * MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
 * bugfix: _mom_state.open: only set self._teardown when opens==1.
 
 *Release 20230217*:
 MultiOpenMixin: __repr__ for the state object.
```

### Comparing `cs.resources-20230331/lib/python/cs/resources.py` & `cs.resources-20230503/lib/python/cs/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 '''
 
 from collections import defaultdict
 from contextlib import contextmanager
 import sys
 from threading import Condition, Lock, RLock, current_thread, main_thread
 import time
-from typing import Any, Tuple
+from typing import Any, Callable, Optional, Tuple
 
 from typeguard import typechecked
 
 from cs.context import stackattrs, setup_cmgr, ContextManagerMixin
 from cs.deco import default_params
 from cs.gimmicks import error, warning, nullcontext
 from cs.obj import Proxy
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
 from cs.py.func import prop
 from cs.py.stack import caller, frames as stack_frames, stack_dump
 from cs.threads import ThreadState, HasThreadState
 
-__version__ = '20230331'
+__version__ = '20230503'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -537,25 +537,31 @@
       * `notify_cancel`: a set of callables called with the `RunState` instance
         to be called whenever `.cancel` is called.
   '''
 
   perthread_state = ThreadState()
 
   def __init__(
-      self, name=None, signals=None, handle_signal=None, verbose=False
+      self,
+      name=None,
+      signals=None,
+      handle_signal=None,
+      poll_cancel: Optional[Callable] = None,
+      verbose=False,
   ):
     self.name = name
     self.verbose = verbose
     self._started_from = None
     self._signals = tuple(signals) if signals else ()
     self._sigstack = None
     self._sighandler = handle_signal or self.handle_signal
     # core state
     self._running = False
-    self.cancelled = False
+    self._cancelled = False
+    self.poll_cancel = poll_cancel
     # timing state
     self.start_time = None
     self.stop_time = None
     self.total_time = 0
     # callbacks
     self.notify_start = set()
     self.notify_cancel = set()
@@ -660,14 +666,32 @@
     '''
     self.running = False
 
   # compatibility
   end = stop
 
   @property
+  def cancelled(self):
+    ''' Test the .cancelled attribute, including a poll if supplied.
+    '''
+    if self._cancelled:
+      return True
+    if self.poll_cancel:
+      if self.poll_cancel():
+        self._cancelled = True
+        return True
+    return False
+
+  @cancelled.setter
+  def cancelled(self, cancel_status):
+    ''' Set the .cancelled attribute.
+    '''
+    self._cancelled = cancel_status
+
+  @property
   def running(self):
     ''' Property expressing whether the task is running.
     '''
     return self._running
 
   @running.setter
   def running(self, status):
```

### Comparing `cs.resources-20230331/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20230503/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20230331
+Version: 20230503
 Summary: Resource management classes and functions.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,18 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20230331*:
-* @uses_runstate: use the prevailing RunState or create one.
-* MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
-* bugfix: _mom_state.open: only set self._teardown when opens==1.
+*Latest release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
 
 ## Class `ClosedError(builtins.Exception, builtins.BaseException)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
 
@@ -182,14 +180,17 @@
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
 # Release Log
 
 
 
+*Release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
+
 *Release 20230331*:
 * @uses_runstate: use the prevailing RunState or create one.
 * MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
 * bugfix: _mom_state.open: only set self._teardown when opens==1.
 
 *Release 20230217*:
 MultiOpenMixin: __repr__ for the state object.
```

### Comparing `cs.resources-20230331/pyproject.toml` & `cs.resources-20230503/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,30 +24,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230331"
+version = "20230503"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Resource management classes and functions.
 
-*Latest release 20230331*:
-* @uses_runstate: use the prevailing RunState or create one.
-* MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
-* bugfix: _mom_state.open: only set self._teardown when opens==1.
+*Latest release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
 
 ## Class `ClosedError(builtins.Exception, builtins.BaseException)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
 
@@ -203,14 +201,17 @@
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
 # Release Log
 
 
 
+*Release 20230503*:
+RunState: new optional poll_cancel Callable parameter, make .cancelled a property.
+
 *Release 20230331*:
 * @uses_runstate: use the prevailing RunState or create one.
 * MultiOpenMixin: move all the open/close counting logic to the _mom_state class, make several attributes public, drop separate finalise() method and associated Condition.
 * bugfix: _mom_state.open: only set self._teardown when opens==1.
 
 *Release 20230217*:
 MultiOpenMixin: __repr__ for the state object.
```

### Comparing `cs.resources-20230331/setup.cfg` & `cs.resources-20230503/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.resources
-version = 20230331
+version = 20230503
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Resource management classes and functions.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

