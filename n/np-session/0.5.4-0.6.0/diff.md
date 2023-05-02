# Comparing `tmp/np-session-0.5.4.tar.gz` & `tmp/np-session-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.5.4.tar", last modified: Thu Apr 27 01:08:25 2023, max compression
+gzip compressed data, was "np-session-0.6.0.tar", last modified: Tue May  2 22:27:47 2023, max compression
```

## Comparing `np-session-0.5.4.tar` & `np-session-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0     2217 2023-04-27 01:08:21.001459 np-session-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.4/README.md
--rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.4/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.4/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8069 2023-04-27 00:58:03.330699 np-session-0.5.4/src/np_session/components/info.py
--rw-r--r--   0        0        0     8823 2023-04-27 00:05:53.424367 np-session-0.5.4/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.4/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.4/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.4/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.4/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.4/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.4/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.4/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.4/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.4/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.4/src/np_session/databases/sql_alchemy.py
--rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.4/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.4/src/np_session/jobs/find_missing_files.py
--rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.4/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.4/src/np_session/jobs/probes.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.4/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.4/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0    26133 2023-04-26 15:19:15.269851 np-session-0.5.4/src/np_session/session.py
--rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.4/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.4/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.4/tests/test_platform_json.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-05-02 22:27:34.652197 np-session-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.0/README.md
+-rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.0/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.0/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.0/src/np_session/components/info.py
+-rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.0/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.0/src/np_session/components/mixins.py
+-rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.0/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.0/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.0/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.0/src/np_session/components/state.py
+-rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.0/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.0/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.0/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.0/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.0/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.0/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.0/src/np_session/exceptions.py
+-rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.0/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.0/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.0/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.0/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0     8531 2023-05-02 22:25:42.888002 np-session-0.6.0/src/np_session/session.py
+-rw-r--r--   0        0        0      181 2023-05-02 22:19:28.306490 np-session-0.6.0/src/np_session/subclasses/__init__.py
+-rw-r--r--   0        0        0     4586 2023-05-02 22:17:18.896118 np-session-0.6.0/src/np_session/subclasses/dynamic_routing_pilot.py
+-rw-r--r--   0        0        0    20527 2023-05-02 22:17:19.652824 np-session-0.6.0/src/np_session/subclasses/pipeline.py
+-rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.0/src/np_session/tasks.py
+-rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.0/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.0/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.0/tests/test_platform_json.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.0/PKG-INFO
```

### Comparing `np-session-0.5.4/pyproject.toml` & `np-session-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [project]
 name = "np-session"
-version = "0.5.4"
+version = "0.6.0"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 dependencies = [
+    "np_logging>=0.3.8",
+    "np_config>=0.4.17",
+    "np-tools>=0.1.6",
     "typing-extensions>=4",
     "psycopg2-binary>=2",
     "requests>=2",
-    "np_logging>=0.3.8",
-    "np_config>=0.4.17",
     "backports.cached-property",
     "firebase-admin>=6.1.0",
-    "redis>=4.5.1",
     "pydantic>=1.10.5",
-    "np-tools>=0.1.4",
+    "redis<=4.1.4",
 ]
 
 [project.urls]
 Repository = "https://github.com/alleninstitute/np_session"
 "Bug Tracker" = "https://github.com/alleninstitute/np_session/issues"
 
 [project.optional-dependencies]
@@ -106,12 +106,15 @@
 source = [
     "np_session",
 ]
 
 [tool.coverage.report]
 show_missing = true
 
+[tool.ruff]
+ignore-init-module-imports = true
+
 [build-system]
 requires = [
     "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `np-session-0.5.4/src/np_session/components/info.py` & `np-session-0.6.0/src/np_session/components/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,240 +5,265 @@
 import enum
 import functools
 import time
 from typing import Any, ClassVar, MutableMapping, Optional
 
 import np_logging
 from backports.cached_property import cached_property
-from typing_extensions import Literal
+from typing_extensions import Literal, Protocol, runtime_checkable
 
 from np_session.databases import State
-from np_session.databases.lims2 import (LIMS2MouseInfo, LIMS2ProjectInfo,
-                                        LIMS2UserInfo)
+from np_session.databases.lims2 import (
+    LIMS2MouseInfo,
+    LIMS2ProjectInfo,
+    LIMS2UserInfo,
+)
 from np_session.databases.mtrain import MTrain
 
 logger = np_logging.getLogger(__name__)
 
+
 class InfoBaseClass(abc.ABC):
-    "Store details for an object from various databases. The commonly-used format of its name, e.g. '366122' for a mouse ID, can be obtained by converting to str()."
+    """Store details for an object from various databases. The commonly-used format of its name, e.g. '366122' for a mouse ID, can be obtained by converting to str()."""
 
     id: int | str
     "Commonly-used format of the object's value among the neuropixels team e.g. for a mouse -> the labtracks ID (366122)."
 
     def __str__(self) -> str:
         return str(self.id)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.id!r})"
+        return f'{self.__class__.__name__}({self.id!r})'
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, (int, str, InfoBaseClass)):
             return NotImplemented
         if isinstance(other, Mouse):
             return self.id == other.id
         return str(self) == str(other) or str(self.id) == str(other)
-    
+
     def __hash__(self) -> int:
         return hash(self.id) ^ hash(self.__class__.__name__)
-    
 
-class Mouse(InfoBaseClass):
+
+@runtime_checkable
+class WithLims(Protocol):
+    """Potocol for types that have a `lims` attribute for accessing relevant
+    lims2 data.
+    """
+
+    id: int | str
+    """Lims2 ID for the object."""
+
+    lims: dict = {}
+    """lims2 data as a dict (may be empty)."""
+
+
+@runtime_checkable
+class WithState(Protocol):
+    """Protocol for types that have a `state` attribute for persisting
+    metadata. Can also be used as a mixin to provide basic state implementation.
+    """
+
+    id: int | str
+    """Unique identifier for the object. This is used as the key for the object's state in the database."""
+
+    @property
+    def state(self) -> MutableMapping[str, Any]:
+        try:
+            return State(self.id)
+        except Exception as exc:
+            logger.error('Failed to load `%r.state`: %r', self, exc)
+        return {}
+
+
+class Mouse(WithLims, WithState, InfoBaseClass):
     def __init__(self, labtracks_mouse_id: str | int):
         self.id = int(labtracks_mouse_id)
 
     @property
     def lims(self) -> LIMS2MouseInfo | dict:
-        "Lims info for the mouse."
-        if not hasattr(self, "_lims"):
+        """Lims info for the mouse."""
+        if not hasattr(self, '_lims'):
             try:
                 self._lims = LIMS2MouseInfo(self.id)
             except ValueError:
                 self._lims = {}
         return self._lims
 
     @cached_property
     def mtrain(self) -> MTrain:
-        "Lims info for the mouse."
+        """Lims info for the mouse."""
         return MTrain(self.id)
 
     @property
     def project(self) -> str | None:
-        "Project associated with the mouse."
+        """Project associated with the mouse."""
         return self.lims.project_name if self.lims else None
-    
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        try:
-            return State(self.id)
-        except Exception as exc:
-            logger.error("Failed to load `%r.state`: %r", self, exc)
-        return {}
-    
-class User(InfoBaseClass):
+
+
+class User(WithState, InfoBaseClass):
     def __init__(self, lims_user_id: str):
         self.id = str(lims_user_id)
 
     @cached_property
     def lims(self) -> LIMS2UserInfo | dict:
-        "Lims info for the user."
-        if not hasattr(self, "_lims"):
+        """Lims info for the user."""
+        if not hasattr(self, '_lims'):
             try:
                 self._lims = LIMS2UserInfo(self.id)
             except ValueError:
                 self._lims = {}
         return self._lims
-    
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        try:
-            return State(self.id)
-        except Exception as exc:
-            logger.error("Failed to load `%r.state`: %r", self, exc)
-        return {}
+
+
+# class ProjectsEnum(abc.ABCMeta, enum.EnumMeta, type):
+#     pass
 
 
 class Projects(enum.Enum):
-    "All specific project names (used on lims) associated with each umbrella project."
+    """All specific project names (used on lims) associated with each umbrella project."""
 
     VAR = (
-        "VariabilitySpontaneous",
-        "VariabilityAim1",
+        'VariabilitySpontaneous',
+        'VariabilityAim1',
     )
-    GLO = ("OpenScopeGlobalLocalOddball",)
-    ILLUSION = ("OpenScopeIllusion",)
+    GLO = ('OpenScopeGlobalLocalOddball',)
+    ILLUSION = ('OpenScopeIllusion',)
     DRDG = (
-        "DynamicRoutingSurgicalDevelopment",
-        "DynamicRoutingDynamicGating",
-        "DynamicRoutingTask1Production",
+        'DynamicRoutingSurgicalDevelopment',
+        'DynamicRoutingDynamicGating',
+        'DynamicRoutingTask1Production',
     )
     """Dynamic Gating subset of DR."""
-    DR = DRDG
-    """All Dynamic Routing, including Dynamic Gating."""
-    VB = ("NeuropixelVisualBehavior",)
+    DRPILOT = ('DRPilot',)
+    DR = DRDG + DRPILOT
+    """All Dynamic Routing, including Dynamic Gating & DRpilot."""
+    VB = ('NeuropixelVisualBehavior',)
     TTN = ('TaskTrainedNetworksNeuropixel',)
     NP = ('NeuropixelPlatformDevelopment',)
-    
-    def get_latest_session(self, session_type: Literal['ephys', 'hab', 'behavior'] = 'ephys') -> int | None:
-        "Lims session id for latest session for all child projects."
-        for _ in self.value:
-            session_id = Project(_).state.get(f'latest_{session_type}')
-            if session_id:
-                return session_id
-        return None
-    
-    get_latest_ephys = functools.partialmethod(get_latest_session, 'ephys')
-    get_latest_hab = functools.partialmethod(get_latest_session, 'hab')
-    get_latest_behavior = functools.partialmethod(get_latest_session, 'behavior')
-    
+
+    @property
+    def id(self) -> str:
+        return str(self.name)
+
     @property
     def state(self) -> MutableMapping[str, Any]:
         try:
-            return State(str(self.name))
+            return State(self.id)
         except Exception as exc:
-    
-            logger.error("Failed to load `%r.state`: %r", self, exc)
+            logger.error('Failed to load `%r.state`: %r', self, exc)
         return {}
-    
-    
-class Project(InfoBaseClass):
-    
+
+    @property
+    def latest_session(
+        self, session_type: Literal['ephys', 'hab', 'behavior'] = 'ephys'
+    ) -> int | None:
+        """Lims session id for latest session for all child projects."""
+        for _ in self.value:
+            session_id = Project(_).state.get(f'latest_{session_type}')
+            if session_id:
+                return session_id
+        return None
+
+    @latest_session.setter
+    def latest_session(self, session_id: int) -> None:
+        for _ in self.value:
+            Project(_).state['latest_session'] = session_id
+
+    latest_ephys = functools.partialmethod(latest_session, 'ephys')
+    latest_hab = functools.partialmethod(latest_session, 'hab')
+    latest_behavior = functools.partialmethod(latest_session, 'behavior')
+
+
+class Project(WithState, InfoBaseClass):
     def __init__(self, lims_project_name: str):
         self.id = str(lims_project_name)
 
     @cached_property
     def lims(self) -> LIMS2ProjectInfo:
-        "Lims info for the project."
+        """Lims info for the project."""
         return LIMS2ProjectInfo(self.id)
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Projects):
             return self.id in other.value
         return super().__eq__(other)
-    
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        try:
-            return State(self.id)
-        except Exception as exc:
-            logger.error("Failed to load `%r.state`: %r", self, exc)
-        return {}
-    
+
     @property
     def parent(self) -> Projects | None:
-        "Parent project if it exists."
+        """Parent project if it exists."""
         for _ in Projects:
             if self.id in _.value:
                 return _
         return None
 
-class WithState:
-    "Mixin for classes that have a `state` attribute for persisting metadata."
-    
-    id: int | str
-    """Unique identifier for the object. This is used as the key for the object's state in the database."""
-    
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        try:
-            return State(self.id)
-        except Exception as exc:
-            logger.error("Failed to load `%r.state`: %r", self, exc)
-        return {}
-    
+
 class Dye(WithState):
     """Info about a DiI or DiO dye.
-    
+
     >>> dye = Dye(1)
     >>> dye.description
     'CM-DiI 100%'
     >>> dye.previous_uses = 0
     >>> dye.record_first_use(time.time())
     >>> dye.increment_uses()
     >>> dye.previous_uses
     1
     """
-    
+
     descriptions: ClassVar = ('CM-DiI 100%', 'DiO')
-    
+
     def __init__(self, dye_id: int) -> None:
         self.id = int(dye_id)
-        
+
     @property
     def previous_uses(self) -> int:
         return self.state.setdefault('previous_uses', 0)
-    
+
     @previous_uses.setter
     def previous_uses(self, value: int) -> None:
         self.state['previous_uses'] = int(value)
-    
+
     @property
     def description(self) -> Literal['CM-DiI` 100%', 'DiO']:
         return self.state.setdefault('description', self.descriptions[0])
-    
+
     @description.setter
     def description(self, value: Literal['CM-DiI 100%', 'DiO']) -> None:
         self.state['description'] = value
-    
+
     @property
     def first_use(self) -> datetime.datetime | None:
         first_use: float | None = self.state.get('first_use')
-        return datetime.datetime.fromtimestamp(first_use) if first_use else None
-    
-    def record_first_use(self, timestamp: Optional[datetime.datetime | float] = None) -> None:
+        return (
+            datetime.datetime.fromtimestamp(first_use) if first_use else None
+        )
+
+    def record_first_use(
+        self, timestamp: Optional[datetime.datetime | float] = None
+    ) -> None:
         """Record the time this dye was first used.
-        
+
         Supply a `time.time()`, else the current time will be recorded.
         """
-        timestamp = timestamp.timestamp() if isinstance(timestamp, datetime.datetime) else timestamp
-        self.state['first_use'] = time.time() if timestamp is None else timestamp
-    
+        timestamp = (
+            timestamp.timestamp()
+            if isinstance(timestamp, datetime.datetime)
+            else timestamp
+        )
+        self.state['first_use'] = (
+            time.time() if timestamp is None else timestamp
+        )
+
     def increment_uses(self):
         """Increment the number of times this dye has been used."""
         previous_uses = self.previous_uses
         if previous_uses == 0:
             self.record_first_use()
         self.previous_uses = self.previous_uses + 1
-        
-        
+
+
 if __name__ == '__main__':
     import doctest
-    doctest.testmod(verbose=True, optionflags=doctest.IGNORE_EXCEPTION_DETAIL)
+
+    doctest.testmod(verbose=True, optionflags=doctest.IGNORE_EXCEPTION_DETAIL)
```

### Comparing `np-session-0.5.4/src/np_session/components/lims_manifests.py` & `np-session-0.6.0/src/np_session/components/lims_manifests.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,205 +5,239 @@
 from typing import Optional
 
 from typing_extensions import Literal
 from backports.cached_property import cached_property
 
 import np_config
 import np_logging
-import pydantic
 
 import np_session.session
 import np_session.components.info
 
 logger = np_logging.getLogger(__name__)
 
 SESSION_TYPES = ('D0', 'D1', 'D2', 'hab')
-MANIFESTS: dict[str, dict] = (
-    np_config.from_zk(f'projects/np_session/manifests')
-)
-        
+MANIFESTS: dict[str, dict] = np_config.from_zk('projects/np_session/manifests')
+
+
 class Manifest:
     # class Config:
     #     # validate_assignment = True # coerce types on assignment
     #     # extra = 'allow' # 'forbid' = properties must be defined in the model
     #     fields = {'names': {'exclude': True}, 'globs': {'exclude': True},  'types': {'exclude': True}}
     #     arbitrary_types_allowed = True
-        
+
     session: Optional[np_session.session.Session] = None
     """`np_session.Session` object"""
     project: Optional[str] = None
     """Umbrella project abbrv/acronym (DR, TTN, GLO)."""
     session_type: Optional[Literal['D0', 'D1', 'D2', 'hab']] = None
     """Type of manifest for a specific session upload, e.g. `D1` for D1 upload."""
     path: Optional[str | pathlib.Path] = None
     """Session folder path, to be used with `globs`."""
-    
+
     names: tuple[str, ...]
     """Descriptive lims names for each file in manifest, in order, e.g. `synchronization_data`."""
     globs: tuple[str, ...]
-    """Globbable filename patterns relative to session folder for each file in manifest, in order, e.g. `.sync`."""""
+    """Globbable filename patterns relative to session folder for each file in manifest, in order, e.g. `.sync`.""" ''
     types: tuple[Literal['filename', 'directory_name'], ...]
     """`filename` or `directory_name` for each file in manifest, in order."""
-    
-    def __init__(self, *args, **kwargs) -> None:      
-        
+
+    def __init__(self, *args, **kwargs) -> None:
+
         self.__dict__.update(kwargs)
-        
+
         self.parse_input_args(*args, **kwargs)
-        
+
         if self.session:
             self.assign_props_from_session()
         elif self.session_type is None:
             self.session_type = 'D1'
-            
+
         self.fetch_from_zk()
-        self.remove_non_inserted_probes() # does nothing if no self.session 
-    
+        self.remove_non_inserted_probes()   # does nothing if no self.session
+
     def remove_non_inserted_probes(self) -> None:
         if self.session is None:
             return
         probes_inserted = self.session.probes_inserted
         include_idx = tuple(
-                i
-                for i, name in enumerate(self.names)
-                if (
-                    'probe_' not in name # not a probe field - skip
-                    or any(f'probe_{letter.upper()}' in name for letter in probes_inserted)
+            i
+            for i, name in enumerate(self.names)
+            if (
+                'probe_' not in name  # not a probe field - skip
+                or any(
+                    f'probe_{letter.upper()}' in name
+                    for letter in probes_inserted
                 )
             )
-        self.names, self.globs, self.types = (tuple(_[i] for i in include_idx) for _ in (self.names, self.globs, self.types))
+        )
+        self.names, self.globs, self.types = (
+            tuple(_[i] for i in include_idx)
+            for _ in (self.names, self.globs, self.types)
+        )
 
-                
     @property
     def files(self) -> dict[str, dict[str, str]]:
         """Upload manifest for platform json: `{name: {type: session + glob}}, ...}`"""
         if not self.session:
-            return {k: {v: g} for k, v, g in zip(self.names, self.types, self.globs)}
-        return {k: {v: (p.name if p else None)} for k, v, p in zip(self.names, self.types, self.paths)}
-    
+            return {
+                k: {v: g}
+                for k, v, g in zip(self.names, self.types, self.globs)
+            }
+        return {
+            k: {v: (p.name if p else None)}
+            for k, v, p in zip(self.names, self.types, self.paths)
+        }
+
     @cached_property
     def paths(self) -> tuple[pathlib.Path | None, ...]:
         """First session npexp folder + glob match, if any exist, for each file in manifest,
         in order. `None` if no matches in filesystem.
-        
+
         If `self.path` is set, use that as the session folder path.
-        
+
         See `missing` for files that do not exist.
         """
         if self.path:
             path = pathlib.Path(self.path)
         elif self.session:
             path = self.session.npexp_path
         else:
-            raise ValueError(f'Must provide either `path` or `session` as {self.__class__} property to return paths.')
+            raise ValueError(
+                f'Must provide either `path` or `session` as {self.__class__} property to return paths.'
+            )
         paths = []
         for _ in self.globs:
             hits = tuple(path.glob(_))
             if len(hits) == 0:
                 logger.debug(f'No files found for glob: {path / _}')
             if len(hits) > 1:
-                logger.debug(f'Multiple files found for glob: {path / _} - {hits} - using first.')
-            
+                logger.debug(
+                    f'Multiple files found for glob: {path / _} - {hits} - using first.'
+                )
+
             paths.append(hits[0] if hits else None)
-        
+
         return tuple(paths)
-    
+
     @property
     def missing(self) -> tuple[str, ...]:
         return tuple(n for n, p in zip(self.names, self.paths) if p is None)
-    
-    
+
     def get_sorted_data(self) -> None:
         self._names_sorted_data = []
         self._paths_sorted_data = []
         self._globs_sorted_data = []
-        for probe in ('ABCDEF' if self.session is None else self.session.probes_inserted):
+        for probe in (
+            'ABCDEF' if self.session is None else self.session.probes_inserted
+        ):
             for name, glob in MANIFESTS['_name_glob']['sorted_data'].items():
-                probe_glob =f'*_probe{probe}{glob}'
+                probe_glob = f'*_probe{probe}{glob}'
                 self._globs_sorted_data.append(probe_glob)
                 self._names_sorted_data.append(f'{name}_probe{probe}')
                 if self.session is None:
-                    logger.warning(f'No session provided to {self.__class__} - cannot get sorted data paths.')
+                    logger.warning(
+                        f'No session provided to {self.__class__} - cannot get sorted data paths.'
+                    )
                     return
                 hits = tuple(self.session.npexp_path.glob(probe_glob))
                 if len(hits) == 0:
-                    logger.debug(f'No files found for glob: {self.session.npexp_path / probe_glob}')
+                    logger.debug(
+                        f'No files found for glob: {self.session.npexp_path / probe_glob}'
+                    )
                 if len(hits) > 1:
-                    logger.debug(f'Multiple files found for glob: {self.session.npexp_path / probe_glob} - {hits} - using first.')
+                    logger.debug(
+                        f'Multiple files found for glob: {self.session.npexp_path / probe_glob} - {hits} - using first.'
+                    )
                 self._paths_sorted_data.append(hits[0] if hits else None)
-        
+
     @property
     def names_sorted_data(self) -> tuple[str, ...]:
         with contextlib.suppress(AttributeError):
             return tuple(self._names_sorted_data)
         self.get_sorted_data()
         return self.names_sorted_data
-    
-    @property    
+
+    @property
     def paths_sorted_data(self) -> tuple[pathlib.Path | None, ...]:
         with contextlib.suppress(AttributeError):
             return tuple(self._paths_sorted_data)
         self.get_sorted_data()
         return self.paths_sorted_data
-    
-    @property    
+
+    @property
     def globs_sorted_data(self) -> tuple[str, ...]:
         with contextlib.suppress(AttributeError):
             return tuple(self._globs_sorted_data)
         self.get_sorted_data()
         return self.globs_sorted_data
-    
+
     @property
     def missing_sorted_data(self) -> tuple[str]:
         if self.session is None:
-            logger.warning(f'No session provided to {self.__class__} - cannot get sorted data paths.')
+            logger.warning(
+                f'No session provided to {self.__class__} - cannot get sorted data paths.'
+            )
             return tuple()
-        return tuple(n for n, p in zip(self.names_sorted_data, self.paths_sorted_data) if p is None)
-    
+        return tuple(
+            n
+            for n, p in zip(self.names_sorted_data, self.paths_sorted_data)
+            if p is None
+        )
+
     def parse_input_args(self, *args, **kwargs) -> None:
         for _ in (*args, *kwargs.values()):
             if isinstance(_, np_session.session.Session):
                 self.session = _
                 break
             elif isinstance(_, int):
                 self.session = np_session.session.Session(_)
                 break
             elif isinstance(_, str):
                 with contextlib.suppress(ValueError):
                     self.session = np_session.session.Session(_)
                     break
-        
+
         for _ in SESSION_TYPES:
             if _ in (*args, *kwargs.values()):
                 self.session_type = _
                 break
-            
+
         for _ in (*args, *kwargs.values()):
             if _ in np_session.session.Projects.__members__:
                 self.project = _
                 break
-    
-    
+
     def assign_props_from_session(self) -> None:
         if self.project is None:
             self.project = self.session.project.parent.name
-            logger.debug(f'No project provided, using {self.project} for {self.session}')
+            logger.debug(
+                f'No project provided, using {self.project} for {self.session}'
+            )
         if self.session_type is None:
             self.session_type = 'hab' if self.session.is_hab else 'D1'
-            logger.debug(f'No session_type provided, using {self.session_type} for {self.session}')
-        
+            logger.debug(
+                f'No session_type provided, using {self.session_type} for {self.session}'
+            )
+
     def fetch_from_zk(self) -> None:
         """Fetch names, file globs and file/dir types from zookeeper."""
         project = 'default' if self.project is None else self.project
         default = MANIFESTS[self.session_type]['default']
         if project not in MANIFESTS[self.session_type]:
-            logger.debug(f'No manifest found for {project} in {self.session_type} manifests on ZK - using default.')
-        name_glob: dict[str, str] = MANIFESTS[self.session_type].get(project, default)
-        
-        self.names, self.globs = tuple(name_glob.keys()), tuple(name_glob.values())
-        
+            logger.debug(
+                f'No manifest found for {project} in {self.session_type} manifests on ZK - using default.'
+            )
+        name_glob: dict[str, str] = MANIFESTS[self.session_type].get(
+            project, default
+        )
+
+        self.names, self.globs = tuple(name_glob.keys()), tuple(
+            name_glob.values()
+        )
+
         name_type: dict[str, str] = MANIFESTS['_name_type']
         self.types = tuple(name_type[_] for _ in self.names)
 
     def __repr__(self) -> str:
         return repr(self.files)
-
```

### Comparing `np-session-0.5.4/src/np_session/components/paths.py` & `np-session-0.6.0/src/np_session/components/paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import pathlib
 
 # if any of these are changing regularly we could get them from zk, e.g.:
 # np_config.from_zk('/np_defaults/configuration').get('lims_incoming_root')
 
-NPEXP_ROOT = pathlib.Path("//allen/programs/mindscope/workgroups/np-exp")
+NPEXP_ROOT = pathlib.Path('//allen/programs/mindscope/workgroups/np-exp')
 INCOMING_ROOT = pathlib.Path(
-    "//allen/programs/braintv/production/incoming/neuralcoding"
+    '//allen/programs/braintv/production/incoming/neuralcoding'
 )
 
 TEMPLATES_ROOT = pathlib.Path(
-    "//allen/programs/mindscope/workgroups/dynamicrouting/ben/npexp_data_manifests"
+    '//allen/programs/mindscope/workgroups/dynamicrouting/ben/npexp_data_manifests'
 )
 
-MVR_RELATIVE_PATH = pathlib.Path("c$/ProgramData/AIBS_MPE/mvr/data")
-NEWSCALE_RELATIVE_PATH = pathlib.Path("c$/MPM_data")
-CAMVIEWER_RELATIVE_PATH = pathlib.Path("c$/Users/svc_neuropix/cv3dImages")  # NP.0 only
-CAMSTIM_RELATIVE_PATH = pathlib.Path("c$/ProgramData/AIBS_MPE/camstim/data")
-SYNC_RELATIVE_PATH = pathlib.Path("c$/ProgramData/AIBS_MPE/sync/data")
+MVR_RELATIVE_PATH = pathlib.Path('c$/ProgramData/AIBS_MPE/mvr/data')
+NEWSCALE_RELATIVE_PATH = pathlib.Path('c$/MPM_data')
+CAMVIEWER_RELATIVE_PATH = pathlib.Path(
+    'c$/Users/svc_neuropix/cv3dImages'
+)  # NP.0 only
+CAMSTIM_RELATIVE_PATH = pathlib.Path('c$/ProgramData/AIBS_MPE/camstim/data')
+SYNC_RELATIVE_PATH = pathlib.Path('c$/ProgramData/AIBS_MPE/sync/data')
 
 NEUROPIXELS_DATA_RELATIVE_PATH = pathlib.Path(
-    "c$/ProgramData/AIBS_MPE/neuropixels_data"
+    'c$/ProgramData/AIBS_MPE/neuropixels_data'
 )
-NPEXP_PATH = pathlib.Path("//allen/programs/mindscope/workgroups/np-exp")
+NPEXP_PATH = pathlib.Path('//allen/programs/mindscope/workgroups/np-exp')
 
 QC_PATHS = (
     NPEXP_PATH / 'qc',
     pathlib.Path(
-        "//allen/programs/braintv/workgroups/nc-ophys/corbettb/NP_behavior_pipeline/QC"
+        '//allen/programs/braintv/workgroups/nc-ophys/corbettb/NP_behavior_pipeline/QC'
+    ),
+    pathlib.Path('//allen/programs/mindscope/workgroups/openscope/GLO_QC'),
+    pathlib.Path(
+        '//allen/programs/mindscope/workgroups/openscope/Illusion_QC'
     ),
-    pathlib.Path("//allen/programs/mindscope/workgroups/openscope/GLO_QC"),
-    pathlib.Path("//allen/programs/mindscope/workgroups/openscope/Illusion_QC"),
 )
-"Item 0 is used as default - currently new np-exp/qc folder."
+'Item 0 is used as default - currently new np-exp/qc folder.'
```

### Comparing `np-session-0.5.4/src/np_session/components/platform_json.py` & `np-session-0.6.0/src/np_session/components/platform_json.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,276 +1,294 @@
 from __future__ import annotations
 
-import abc
 import contextlib
 import copy
-import csv
 import datetime
-import functools
 import json
 import pathlib
-import re
-import tempfile
 import time
-from typing import (Any, ClassVar, Dict, ForwardRef, Generator, Iterable, List, Mapping,
-                    Optional, Sequence, Union)
+from typing import Any, ClassVar, Dict, Generator, List, Optional, Union
 
 import np_config
 import np_logging
 import pydantic
-from typing_extensions import Literal
 
 logger = np_logging.getLogger(__name__)
 
 
-
 class PlatformJsonDateTime(datetime.datetime):
-    """
-
-    """
+    """ """
 
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
-        
+
     @classmethod
     def __modify_schema__(cls, field_schema):
         # __modify_schema__ should mutate the dict it receives in place,
         # the returned value will be ignored
         field_schema.update(
             pattern='[0-9]{14}',
             # some example postcodes
             examples=['20220414134738'],
         )
+
     # def __init__(self, v) -> None:
     #     super().__init__(*self.str2components(np_config.normalize_time(v)))
-        
+
     @classmethod
     def validate(cls, v):
         if not v:
-            return None 
+            return None
         if not isinstance(v, str) and len(v) != 14:
             raise TypeError('14-digit string required')
         return cls(*cls.str2components(np_config.normalize_time(v)))
 
     @staticmethod
     def str2components(v: str) -> tuple[int, int, int, int, int, int, int]:
-        return (int(v[:4]), *(int(v[_:_+2]) for _ in range(4, 14, 2)))
-    
+        return (int(v[:4]), *(int(v[_ : _ + 2]) for _ in range(4, 14, 2)))
+
     def __str__(self):
         return np_config.normalize_time(self)
-    
+
     def isoformat(self, *args, **kwargs) -> str:
         return str(self)
-    
+
+
 class PlatformJson(pydantic.BaseModel):
     """Writes D1 platform json for lims upload. Just requires a path (dir or dir+filename)."""
 
     # ------------------------------------------------------------------------------------- #
     # required kwargs on init (any property without a default value or leading underscore)
-    
+
     path: pathlib.Path
-    "Typically the storage directory for the session. Will be modified on assignment."
-    
+    'Typically the storage directory for the session. Will be modified on assignment.'
+
     # ------------------------------------------------------------------------------------- #
-    
+
     file_sync: bool = True
-    
+
     @contextlib.contextmanager
-    def sync_disabled(self)  -> Generator[None, None, None]:
-        "Context manager to temporarily disable writing to file when a property is updated."
+    def sync_disabled(self) -> Generator[None, None, None]:
+        """Context manager to temporarily disable writing to file when a property is updated."""
         self.file_sync = False
         yield
         self.file_sync = True
-        
+
     class Config:
-        validate_assignment = True # coerce types on assignment
-        extra = 'allow' # 'forbid' = properties must be defined in the model
+        validate_assignment = True   # coerce types on assignment
+        extra = 'allow'   # 'forbid' = properties must be defined in the model
         fields = {'path': {'exclude': True}, 'file_sync': {'exclude': True}}
         arbitrary_types_allowed = True
-        
-    suffix: ClassVar[str] = "_platformD1.json"
-        
+
+    suffix: ClassVar[str] = '_platformD1.json'
+
     def __init__(self, path: Union[str, pathlib.Path]) -> None:
         super().__init__(path=path)
         if self.path.exists():
-            logger.debug("Loading from existing %s", self.path.name)
+            logger.debug('Loading from existing %s', self.path.name)
         else:
-            logger.debug("Creating new %s", self.path.name)
-            self.platform_json_creation_time = np_config.normalize_time(time.time())
+            logger.debug('Creating new %s', self.path.name)
+            self.platform_json_creation_time = np_config.normalize_time(
+                time.time()
+            )
         self.load_from_existing()
-        
+
     def __str__(self):
         return self.path.as_posix()
-    
+
     def load_from_existing(self) -> None:
-        "Update empty fields with non-empty fields from file."
+        """Update empty fields with non-empty fields from file."""
         with self.sync_disabled():
             if not self.path.exists():
                 return
-            contents = json.loads(self.path.read_text() or "{}")
+            contents = json.loads(self.path.read_text() or '{}')
             for k, v in contents.items():
                 if not v:
                     continue
                 if isinstance(v, (dict, list)) and not all(_ for _ in v):
                     continue
                 setattr(self, k, v)
-    
+
     def __setattr__(self, name, value):
-        
-        # if field is in non-validated list, just set it 
-        if name in (k for k, v in self.Config.fields.items() if v.get('exclude')):
+
+        # if field is in non-validated list, just set it
+        if name in (
+            k for k, v in self.Config.fields.items() if v.get('exclude')
+        ):
             return super().__setattr__(name, value)
-        
+
         if self.file_sync:
             # fetch fields from disk before writing, in case another process updated the
             # file since we last read it
             self.load_from_existing()
-        
+
         if getattr(self, name, None) == value:
             return
-        
+
         _ = super().__setattr__(name, value)
-        
-        logger.debug("Updated %s.%s = %s", self.path.name, name, value)
-            
+
+        logger.debug('Updated %s.%s = %s', self.path.name, name, value)
+
         if self.file_sync:
             self.write()
-            
+
         return _
-    
-    def write(self): 
+
+    def write(self):
         self.path.parent.mkdir(parents=True, exist_ok=True)
         self.path.touch()
         with self.sync_disabled():
-            self.platform_json_save_time = np_config.normalize_time(time.time())
+            self.platform_json_save_time = np_config.normalize_time(
+                time.time()
+            )
         self.path.write_text(self.json(indent=4))
-        logger.debug("%s wrote to %s", self.__class__.__name__, self.path.as_posix())
-    
-    @pydantic.validator("path", pre=True)
+        logger.debug(
+            '%s wrote to %s', self.__class__.__name__, self.path.as_posix()
+        )
+
+    @pydantic.validator('path', pre=True)
     def normalize_path(cls, v: Union[str, pathlib.Path]) -> pathlib.Path:
         return np_config.normalize_path(v)
-    
-    @pydantic.validator("path")
+
+    @pydantic.validator('path')
     def add_filename_to_path(cls, v: pathlib.Path) -> pathlib.Path:
         name = cls.append_suffix_to_filename(v.name)
         return v / name if v.is_dir() else v.with_name(name)
-    
+
     @classmethod
     def append_suffix_to_filename(cls, v: str) -> str:
-        v = v.split('.json')[0].split('platform')[0].rstrip('_')                                       
+        v = v.split('.json')[0].split('platform')[0].rstrip('_')
         v += cls.suffix
         return v
 
     _foraging_id_re: ClassVar[str] = (
-        r"([0-9,a-f]{8}-[0-9,a-f]{4}-[0-9,a-f]{4}-[0-9,a-f]{4}-[0-9,a-f]{12})" \
-        r"|([0-9,a-f]{8})"
+        r'([0-9,a-f]{8}-[0-9,a-f]{4}-[0-9,a-f]{4}-[0-9,a-f]{4}-[0-9,a-f]{12})'
+        r'|([0-9,a-f]{8})'
     )
-    
+
     # auto-generated / ignored ------------------------------------------------------------- #
     platform_json_save_time: Union[PlatformJsonDateTime, str] = ''
-    "Updated on write."
+    'Updated on write.'
     rig_id: Optional[str] = np_config.Rig().id if np_config.RIG_IDX else None
     wfl_version: float = 0
-    platform_json_creation_time: Union[PlatformJsonDateTime, str] = ""
+    platform_json_creation_time: Union[PlatformJsonDateTime, str] = ''
     # = pydantic.Field(
     #     default_factory=lambda: np_config.normalize_time(time.time()),
     #     validate=PlatformJsonDateTime.validate,
     # )
-    
+
     # pre-experiment
     # ---------------------------------------------------------------------- #
-    workflow_start_time: Union[PlatformJsonDateTime, str] = ""
-    operatorID: Optional[str] = ""
-    sessionID: Optional[Union[str, int]] = ""
-    mouseID: Optional[Union[str, int]] = ""
-    project: Optional[str] = ""
+    workflow_start_time: Union[PlatformJsonDateTime, str] = ''
+    operatorID: Optional[str] = ''
+    sessionID: Optional[Union[str, int]] = ''
+    mouseID: Optional[Union[str, int]] = ''
+    project: Optional[str] = ''
     hab: Optional[bool] = None
-    
+
     DiINotes: Dict[str, Union[str, int]] = dict(
-        EndTime="", StartTime="", dii_description="", times_dipped="", previous_uses="",
+        EndTime='',
+        StartTime='',
+        dii_description='',
+        times_dipped='',
+        previous_uses='',
     )
     HardwareConfiguration: Optional[Dict] = {}
-    probe_A_DiI_depth: str = ""
-    probe_B_DiI_depth: str = ""
-    probe_C_DiI_depth: str = ""
-    probe_D_DiI_depth: str = ""
-    probe_E_DiI_depth: str = ""
-    probe_F_DiI_depth: str = ""
+    probe_A_DiI_depth: str = ''
+    probe_B_DiI_depth: str = ''
+    probe_C_DiI_depth: str = ''
+    probe_D_DiI_depth: str = ''
+    probe_E_DiI_depth: str = ''
+    probe_F_DiI_depth: str = ''
     water_calibration_heights: List[float] = [0.0]
     water_calibration_volumes: List[float] = [0.0]
-    mouse_weight_pre: str = ""
+    mouse_weight_pre: str = ''
     mouse_weight_pre_float: float = 0.0
-    
+
     HeadFrameEntryTime: Union[PlatformJsonDateTime, str] = ''
-    wheel_height: str = ""
+    wheel_height: str = ''
     CartridgeLowerTime: Union[PlatformJsonDateTime, str] = ''
     ProbeInsertionStartTime: Union[PlatformJsonDateTime, str] = ''
     ProbeInsertionCompleteTime: Union[PlatformJsonDateTime, str] = ''
     InsertionNotes: Dict[str, Dict] = pydantic.Field(default_factory=dict)
     ExperimentStartTime: Union[PlatformJsonDateTime, str] = ''
-    stimulus_name: str = ""
-    "MTrain stage (?)."
-    script_name: Union[pathlib.Path, str] = ""
-    "Path to stimulus script."
-    
+    stimulus_name: str = ''
+    'MTrain stage (?).'
+    script_name: Union[pathlib.Path, str] = ''
+    'Path to stimulus script.'
+
     # post-experiment ---------------------------------------------------------------------- #
     ExperimentCompleteTime: Union[PlatformJsonDateTime, str] = ''
     ExperimentNotes: Dict[str, Dict[str, Any]] = dict(
         BleedingOnInsertion={}, BleedingOnRemoval={}
     )
-    foraging_id: str = pydantic.Field(default="", regex=_foraging_id_re)
+    foraging_id: str = pydantic.Field(default='', regex=_foraging_id_re)
     foraging_id_list: List[str] = pydantic.Field(
-        default_factory=lambda: [""], regex=_foraging_id_re
+        default_factory=lambda: [''], regex=_foraging_id_re
     )
     HeadFrameExitTime: Union[PlatformJsonDateTime, str] = ''
-    mouse_weight_post: str = ""
+    mouse_weight_post: str = ''
     water_supplement: float = 0.0
     manifest_creation_time: Union[PlatformJsonDateTime, str] = ''
     workflow_complete_time: Union[PlatformJsonDateTime, str] = ''
-    
-    manipulator_coordinates: Dict[str, Dict[Any, Any]] = pydantic.Field(default_factory=dict)
+
+    manipulator_coordinates: Dict[str, Dict[Any, Any]] = pydantic.Field(
+        default_factory=dict
+    )
 
     files: Dict[str, Dict[str, str]] = pydantic.Field(default_factory=dict)
 
     def update(self, field, new) -> None:
-        
+
         self.load_from_existing()
-        
+
         existing = getattr(self, field)
-        
+
         if (not new and new is not False) or existing == new:
             return
-        
+
         # now merge the new value with the existing value in the file if it's a dict
         with contextlib.suppress(TypeError, AttributeError):
             new = np_config.merge(copy.deepcopy(getattr(self, field)), new)
-            
-        logger.debug('Updating %s %s: %s -> %s', self.path.name, field, existing, new)
+
+        logger.debug(
+            'Updating %s %s: %s -> %s', self.path.name, field, existing, new
+        )
         with self.sync_disabled():
             setattr(self, field, new)
         self.write()
-   
+
+
 def update_from_session(pj: PlatformJson, session) -> None:
-    "Updates fields in a platform json file."
+    """Updates fields in a platform json file."""
     #! careful not to execute Session methods that call this platform json instance in a loop
-    
+
     with pj.sync_disabled():
-        logger.debug("Updating %s with session %s fields, with write disabled", pj.path.name, session.id)
-        pj.update('operatorID', str(session.user)) # don't need to convert here, `update` will compare values with existing
+        logger.debug(
+            'Updating %s with session %s fields, with write disabled',
+            pj.path.name,
+            session.id,
+        )
+        pj.update(
+            'operatorID', str(session.user)
+        )   # don't need to convert here, `update` will compare values with existing
         pj.update('sessionID', str(session.id))
         pj.update('mouseID', str(session.mouse.id))
         pj.update('stimulus_name', session.lims['stimulus_name'])
         if pj.script_name:
             with contextlib.suppress(Exception):
                 if session.rig.stim not in pj.script_name.as_posix():
-                    pj.update('script_name', np_config.local_to_unc(session.rig.stim, pj.script_name).as_posix())
+                    pj.update(
+                        'script_name',
+                        np_config.local_to_unc(
+                            session.rig.stim, pj.script_name
+                        ).as_posix(),
+                    )
         pj.update('foraging_id', session.foraging_id)
         pj.update('project', session.project.id)
         pj.update('hab', session.is_hab)
-        
-    pj.write()
-
 
+    pj.write()
```

### Comparing `np-session-0.5.4/src/np_session/components/settings_xml.py` & `np-session-0.6.0/src/np_session/components/settings_xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,26 @@
 import pathlib
 import xml.etree.ElementTree as ET
 
 
 @dataclasses.dataclass
 class SettingsXmlInfo:
     """Info from a settings.xml file from an Open Ephys recording."""
+
     path: pathlib.Path
     probe_serial_numbers: tuple[int, ...]
     probe_types: tuple[str, ...]
     probe_letters: tuple[str, ...]
     hostname: str
     date: datetime.date
     start_time: datetime.time
     open_ephys_version: str
     settings_xml_md5: str
 
+
 def settings_xml_info_from_path(path: str | pathlib.Path) -> SettingsXmlInfo:
     """Info from a settings.xml file from an Open Ephys recording."""
     path = pathlib.Path(path)
     et = ET.parse(path)
     return SettingsXmlInfo(
         path=path,
         probe_serial_numbers=probe_serial_numbers(et),
@@ -53,83 +55,111 @@
         probe_letters=probe_letters(et),
         hostname=hostname(et),
         date=date_time(et)[0],
         start_time=date_time(et)[1],
         open_ephys_version=open_ephys_version(et),
         settings_xml_md5=settings_xml_md5(path),
     )
-    
+
+
 def get_tag_text(et: ET.ElementTree, tag: str) -> str | None:
-    result = [element.text for element in et.getroot().iter() if element.tag == tag.upper()]
+    result = [
+        element.text
+        for element in et.getroot().iter()
+        if element.tag == tag.upper()
+    ]
     if not (result and any(result)):
-        result = [element.attrib.get(tag.lower()) for element in et.getroot().iter()]
+        result = [
+            element.attrib.get(tag.lower()) for element in et.getroot().iter()
+        ]
     return str(result[0]) if (result and any(result)) else None
 
+
 def get_tag_attrib(et: ET.ElementTree, tag: str, attrib: str) -> str | None:
-    result = [element.attrib.get(attrib) for element in et.getroot().iter() if element.tag == tag.upper()]
+    result = [
+        element.attrib.get(attrib)
+        for element in et.getroot().iter()
+        if element.tag == tag.upper()
+    ]
     return str(result[0]) if (result and any(result)) else None
 
+
 def hostname(et: ET.ElementTree) -> str:
     result = (
         # older, pre-0.6.x:
         get_tag_text(et, 'machine')
         # newer, 0.6.x:
         or get_tag_attrib(et, 'MACHINE', 'name')
     )
     if not result:
         raise LookupError(f'No hostname: {result!r}')
     return result
 
+
 @functools.lru_cache(maxsize=None)
 def date_time(et: ET.ElementTree) -> tuple[datetime.date, datetime.time]:
     """Date and recording start time."""
     result = get_tag_text(et, 'date')
     if not result:
         raise LookupError(f'No datetime found: {result!r}')
     dt = datetime.datetime.strptime(result, '%d %b %Y %H:%M:%S')
     return dt.date(), dt.time()
 
+
 @functools.lru_cache(maxsize=None)
 def probe_attrib_dicts(et: ET.ElementTree) -> tuple[dict[str, str], ...]:
     return tuple(
         probe_dict.attrib
         for probe_dict in et.getroot().iter()
         if 'probe_serial_number' in probe_dict.attrib
     )
 
+
 def probe_attrib(et: ET.ElementTree, attrib: str) -> tuple[str, ...]:
     return tuple(probe[attrib] for probe in probe_attrib_dicts(et))
 
+
 def probe_serial_numbers(et: ET.ElementTree) -> tuple[int, ...]:
     return tuple(int(_) for _ in probe_attrib(et, 'probe_serial_number'))
 
+
 def probe_types(et: ET.ElementTree) -> tuple[str, ...]:
     try:
         return probe_attrib(et, 'probe_name')
     except KeyError:
         return tuple('unknown' for _ in probe_attrib_dicts(et))
-    
+
+
 def probe_idx(et: ET.ElementTree) -> tuple[int, ...]:
     """Try to reconstruct index from probe slot and port.
-    
+
     Normally 2 slots: each with 3 ports in use.
     """
     slots, ports = probe_attrib(et, 'slot'), probe_attrib(et, 'port')
-    result = tuple((int(s) - int(min(slots))) * len(set(ports)) + int(p) - 1 for s, p in zip(slots, ports))
+    result = tuple(
+        (int(s) - int(min(slots))) * len(set(ports)) + int(p) - 1
+        for s, p in zip(slots, ports)
+    )
     if not all(idx in range(6) for idx in result):
-        raise ValueError(f'probe_idx: {result!r}, slots: {slots}, ports: {ports}')
+        raise ValueError(
+            f'probe_idx: {result!r}, slots: {slots}, ports: {ports}'
+        )
     return result
 
+
 def probe_letters(et: ET.ElementTree) -> tuple[str, ...]:
     return tuple('ABCDEF'[idx] for idx in probe_idx(et))
 
+
 def open_ephys_version(et: ET.ElementTree) -> str:
     result = get_tag_text(et, 'version')
     if not result:
         raise LookupError(f'No version found: {result!r}')
     return result
 
+
 def settings_xml_md5(path: str | pathlib.Path) -> str:
     return hashlib.md5(pathlib.Path(path).read_bytes()).hexdigest()
 
+
 if __name__ == '__main__':
-    doctest.testmod(verbose=True)
+    doctest.testmod(verbose=True)
```

### Comparing `np-session-0.5.4/src/np_session/databases/data_getters.py` & `np-session-0.6.0/src/np_session/databases/data_getters.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,59 +12,60 @@
 import os
 import pathlib
 from typing import ClassVar
 
 import psycopg2
 import psycopg2.extras
 
+
 class NoBehaviorSessionError(Exception):
     pass
 
 
 class MultipleBehaviorSessionsError(Exception):
     pass
 
 
 def get_foraging_id_from_behavior_session(
     mouse_id: int | str, start: datetime.datetime, end: datetime.datetime
 ) -> str:
-    fmt = "%Y-%m-%d %H:%M"
+    fmt = '%Y-%m-%d %H:%M'
     query = f"""
             SELECT foraging_id
             FROM behavior_sessions bs
                 JOIN specimens sp ON sp.donor_id = bs.donor_id
             WHERE date_of_acquisition between '{start.strftime(fmt)}' and '{end.strftime(fmt)}'
             and external_specimen_name = '{mouse_id}'
             """
     cur = get_psql_cursor()
     cur.execute(query)
     info_list = []
     if cur.rowcount == 0:
         raise NoBehaviorSessionError(
-            f"No behavior session found for MID {mouse_id} between {start} and {end}"
+            f'No behavior session found for MID {mouse_id} between {start} and {end}'
         )
     elif cur.rowcount != 0:
         info_list = cur.fetchall()
         if len(info_list) > 1:
             raise MultipleBehaviorSessionsError(
-                f"Multiple behavior sessions found for MID {mouse_id} between {start} and {end}"
+                f'Multiple behavior sessions found for MID {mouse_id} between {start} and {end}'
             )
         elif info_list == []:
             raise NoBehaviorSessionError(
-                f"No behavior session found for MID {mouse_id} between {start} and {end}"
+                f'No behavior session found for MID {mouse_id} between {start} and {end}'
             )
         elif len(info_list) == 1 and isinstance(info_list[0], tuple):
             foraging_id = info_list[0][0]
             return foraging_id
         elif len(info_list) == 1 and isinstance(info_list[0], dict):
             foraging_id = info_list[0]['foraging_id']
             return foraging_id
         else:
             raise Exception(
-                f"Unexpected behavior session info for MID {mouse_id} between {start} and {end}: {info_list}"
+                f'Unexpected behavior session info for MID {mouse_id} between {start} and {end}: {info_list}'
             )
 
 
 # functions from Ahad ------------------------------------------------------------------ #
 
 
 def get_sess_probes(session_id):
@@ -95,40 +96,42 @@
     WHERE ep.id = {}
     """
     cur = get_psql_cursor(get_cred_location())
     lims_query = EPHYS_PROBE_QRY.format(session_id)
     cur.execute(lims_query)
     info_list = []
     if cur.rowcount == 0:
-        raise Exception("No data was found for ID {}".format(session_id))
+        raise Exception('No data was found for ID {}'.format(session_id))
     elif cur.rowcount != 0:
         info_list = cur.fetchall()
         probes_list = []
         probes_id_list = info_list[0][1]
         return probes_id_list
         # returning probe IDs early - need to know only if they exist
         for probe_id in probes_id_list:
             print(probe_id)
             probe_query = PROBE_ID_QRY.format(probe_id)
             cur.execute(probe_query)
             if cur.rowcount == 0:
-                raise Exception("No data was found for ID {}".format(session_id))
+                raise Exception(
+                    'No data was found for ID {}'.format(session_id)
+                )
             else:
                 probe_name_status = cur.fetchall()
                 probe_status = probe_name_status[0][1]
                 probe_name = probe_name_status[0][0]
                 probe_storage = probe_name_status[0][2]
                 print(probe_storage)
                 if (
-                    probe_status == "passed" or probe_status == "created"
+                    probe_status == 'passed' or probe_status == 'created'
                 ) and probe_storage is not None:
-                    if (probe_status) == "passed":
+                    if (probe_status) == 'passed':
                         print(probe_name)
                     else:
-                        print(probe_name + " is created, but not passed")
+                        print(probe_name + ' is created, but not passed')
                     probes_list.append(probe_name)
         return probes_list
 
 
 def get_cred_location():
     """Gets content of firebase credential file
     Files are ignored and not committed to the repository
@@ -136,15 +139,15 @@
     ----------
     Returns
     -------
     cred_json: str
     path to json file storing credential information
     """
     dir = os.path.dirname(__file__)
-    cred_json = os.path.join(dir, ".cred", "post_gres.json")
+    cred_json = os.path.join(dir, '.cred', 'post_gres.json')
     return cred_json
 
 
 def get_psql_cursor(as_dict=True):
     """Initializes a connection to the postgres database
     Parameters
     ----------
@@ -162,35 +165,38 @@
     The port to connect to
     Returns
     -------
     con: connect
     A connection to the postgres database
     """
 
-    dbname = "lims2"
-    user = "limsreader"
-    host = "limsdb2"
-    password = "limsro"
+    dbname = 'lims2'
+    user = 'limsreader'
+    host = 'limsdb2'
+    password = 'limsro'
     port = 5432
     con = psycopg2.connect(
         dbname=dbname, user=user, host=host, password=password, port=port
     )
     con.set_session(readonly=True, autocommit=True)
     if as_dict:
-        return con.cursor(cursor_factory=psycopg2.extras.RealDictCursor,)
+        return con.cursor(
+            cursor_factory=psycopg2.extras.RealDictCursor,
+        )
     return con.cursor()
 
 
 # functions from Corbett --------------------------------------------------------------- #
 class data_getter:
     """parent class for data getter, should be able to
     1) connect to data source
     2) grab experiment data
     3) grab probe data
     """
+
     def __init__(self, exp_id=None, base_dir=None, cortical_sort=False):
         self.data_dict = {}
         self.cortical_sort = cortical_sort
         self.connect(exp_id, base_dir)
         self.get_exp_data()
         self.get_probe_data()
         self.get_image_data()
@@ -206,32 +212,33 @@
         pass
 
     def get_image_data(self):
         pass
 
 
 class lims_data_getter(data_getter):
-    
+
     con: ClassVar[psycopg2.connection]
     cursor: ClassVar[psycopg2.cursor]
+
     def connect(self, exp_id, base_dir):
         # set up connection to lims
-        if not hasattr(self.__class__, "con"):
+        if not hasattr(self.__class__, 'con'):
             self.__class__.con = psycopg2.connect(
-                dbname="lims2",
-                user="limsreader",
-                host="limsdb2",
-                password="limsro",
+                dbname='lims2',
+                user='limsreader',
+                host='limsdb2',
+                password='limsro',
                 port=5432,
             )
             self.con.set_session(
                 readonly=True,
                 autocommit=True,
             )
-        if not hasattr(self.__class__, "cursor"):
+        if not hasattr(self.__class__, 'cursor'):
             self.__class__.cursor = self.con.cursor(
                 cursor_factory=psycopg2.extras.RealDictCursor,
             )
 
         self.lims_id = exp_id
 
     def get_exp_data(self):
@@ -272,33 +279,35 @@
         exp_data = self.cursor.fetchall()
         if not exp_data:
             return
         self.data_dict.update(
             exp_data[0]
         )  # update data_dict to have all the experiment metadata
         [
-            self.data_dict.pop(key) for key in ["wkft", "wkf_path"]
+            self.data_dict.pop(key) for key in ['wkft', 'wkf_path']
         ]  # ...but remove the wkf stuff
 
         for e in exp_data:
-            wkft = e["wkft"]
-            wkf_path = e["wkf_path"]
+            wkft = e['wkft']
+            wkf_path = e['wkf_path']
             self.data_dict[wkft] = convert_lims_path(wkf_path)
 
         self.translate_wkf_names()
 
-        behavior_dir = convert_lims_path(self.data_dict["behavior_dir"])
-        self.data_dict["behavior_pkl"] = glob_file(os.path.join(behavior_dir, "*.pkl"))
-        if self.data_dict["date_of_acquisition"] is not None:
-            self.data_dict["datestring"] = self.data_dict[
-                "date_of_acquisition"
-            ].strftime("%Y%m%d")
+        behavior_dir = convert_lims_path(self.data_dict['behavior_dir'])
+        self.data_dict['behavior_pkl'] = glob_file(
+            os.path.join(behavior_dir, '*.pkl')
+        )
+        if self.data_dict['date_of_acquisition'] is not None:
+            self.data_dict['datestring'] = self.data_dict[
+                'date_of_acquisition'
+            ].strftime('%Y%m%d')
         else:
-            self.data_dict["datestring"] = ""
-        self.data_dict["es_id"] = str(self.data_dict["es_id"])
+            self.data_dict['datestring'] = ''
+        self.data_dict['es_id'] = str(self.data_dict['es_id'])
 
     def get_image_data(self):
         """Get all the images associated with this experiment"""
 
         IMAGE_QRY = """
             SELECT es.id AS es_id, es.name AS es, imt.name AS image_type, es.storage_directory || im.jp2 AS image_path
             FROM ecephys_sessions es
@@ -312,16 +321,16 @@
         self.cursor.execute(IMAGE_QRY.format(self.lims_id))
         image_data = self.cursor.fetchall()
 
         # FOR NOW JUST ASSUME IMAGES ARE IN THE D1 UPLOAD DIRECTORY
         # get D1 directory (assume this is where the sync file is)
 
         for im in image_data:
-            name = im["image_type"]
-            path = convert_lims_path(im["image_path"])
+            name = im['image_type']
+            path = convert_lims_path(im['image_path'])
             # self.data_dict[name] = convert_lims_path(path)
             self.data_dict[name] = path
 
     def get_probe_data(self):
         """Get sorted ephys data for each probe
 
         TODO: make this actually use the well known file types,
@@ -342,211 +351,232 @@
                 LEFT JOIN well_known_file_types wkft ON wkft.id=wkf.well_known_file_type_id
             WHERE es.id = {} 
             ORDER BY es.id, ep.name;
             """
         self.cursor.execute(WKF_PROBE_QRY.format(self.lims_id))
         probe_data = self.cursor.fetchall()
 
-        p_info = [p for p in probe_data if p["wkft"] == "EcephysSortedAmplitudes"]
+        p_info = [
+            p for p in probe_data if p['wkft'] == 'EcephysSortedAmplitudes'
+        ]
+
+        def getnesteddir(x):
+            return os.path.dirname(os.path.dirname(os.path.dirname(x)))
 
-        getnesteddir = lambda x: os.path.dirname(os.path.dirname(os.path.dirname(x)))
-        probe_bases = [convert_lims_path(getnesteddir(pi["wkf_path"])) for pi in p_info]
+        probe_bases = [
+            convert_lims_path(getnesteddir(pi['wkf_path'])) for pi in p_info
+        ]
         # probe_bases = [convert_lims_path(os.path.dirname(pi['wkf_path'])) for pi in p_info]
 
-        self.data_dict["data_probes"] = []
+        self.data_dict['data_probes'] = []
         for pb in probe_bases:
             probeID = pb[-1]
-            self.data_dict["data_probes"].append(probeID)
-            self.data_dict["probe" + probeID] = pb
-            self.data_dict["lfp" + probeID] = pb
-            info_json = glob_file(os.path.join(pb, "*probe_info*json"))
-            self.data_dict["probe" + probeID + "_info"] = info_json
+            self.data_dict['data_probes'].append(probeID)
+            self.data_dict['probe' + probeID] = pb
+            self.data_dict['lfp' + probeID] = pb
+            info_json = glob_file(os.path.join(pb, '*probe_info*json'))
+            self.data_dict['probe' + probeID + '_info'] = info_json
 
-        raw = [p for p in probe_data if p["wkft"] == "EcephysProbeRawData"]
+        raw = [p for p in probe_data if p['wkft'] == 'EcephysProbeRawData']
         name_suffix = {
-            "probeA": "ABC",
-            "probeB": "ABC",
-            "probeC": "ABC",
-            "probeD": "DEF",
-            "probeE": "DEF",
-            "probeF": "DEF",
+            'probeA': 'ABC',
+            'probeB': 'ABC',
+            'probeC': 'ABC',
+            'probeD': 'DEF',
+            'probeE': 'DEF',
+            'probeF': 'DEF',
         }
         for r in raw:
-            probeID = r["ep"]
-            name = r["wkft"] + name_suffix[probeID]
-            path = convert_lims_path(r["wkf_path"])
+            probeID = r['ep']
+            name = r['wkft'] + name_suffix[probeID]
+            path = convert_lims_path(r['wkf_path'])
 
             if (
-                not name + "_settings" in self.data_dict
-                or self.data_dict[name + "_settings"] is None
+                name + '_settings' not in self.data_dict
+                or self.data_dict[name + '_settings'] is None
             ):
-                self.data_dict[name + "_settings"] = path
+                self.data_dict[name + '_settings'] = path
 
-            npx2_path = glob_file(os.path.join(os.path.dirname(path), "*npx2"))
-            if not name in self.data_dict or self.data_dict[name] is None:
+            npx2_path = glob_file(os.path.join(os.path.dirname(path), '*npx2'))
+            if name not in self.data_dict or self.data_dict[name] is None:
                 self.data_dict[name] = npx2_path
 
         self.probe_data = probe_data
 
     def storage_directory(self) -> str | None:
         """Get the storage directory for this experiment"""
         if self.data_dict:
-            return "/" + self.data_dict["storage_directory"]
+            return '/' + self.data_dict['storage_directory']
         WKF_QRY = """
             SELECT es.storage_directory
             FROM ecephys_sessions es
             WHERE es.id = {}
             """
         self.cursor.execute(WKF_QRY.format(self.lims_id))
         exp_data = self.cursor.fetchall()
-        if exp_data and exp_data[0]["storage_directory"]:
-            return "/" + exp_data[0]["storage_directory"]
+        if exp_data and exp_data[0]['storage_directory']:
+            return '/' + exp_data[0]['storage_directory']
         return None
 
     def translate_wkf_names(self):
         wkf_dict = {
-            "MappingPickle": "mapping_pkl",
-            "EcephysReplayStimulus": "replay_pkl",
-            "EcephysRigSync": "sync_file",
-            "OptoPickle": "opto_pkl",
+            'MappingPickle': 'mapping_pkl',
+            'EcephysReplayStimulus': 'replay_pkl',
+            'EcephysRigSync': 'sync_file',
+            'OptoPickle': 'opto_pkl',
         }
 
         for wkf in wkf_dict:
             if wkf in self.data_dict:
                 self.data_dict[wkf_dict[wkf]] = self.data_dict[wkf]
 
 
 class local_data_getter(data_getter):
     def connect(self, exp_id, base_dir):
         if os.path.exists(base_dir):
             self.base_dir = base_dir
         else:
-            print("Invalid base directory: " + base_dir)
+            print('Invalid base directory: ' + base_dir)
 
     def get_exp_data(self):
         file_glob_dict = {
-            "mapping_pkl": ["*mapping*.pkl", "*stim.pkl"],
-            "replay_pkl": "*replay*.pkl",
-            "behavior_pkl": "*behavior*.pkl",
-            "opto_pkl": "*opto*.pkl",
-            "sync_file": "*.sync",
-            "RawEyeTrackingVideo": ["*.eye.avi", "*eye.mp4"],
-            "RawBehaviorTrackingVideo": ["*behavior.avi", "*behavior.mp4"],
-            "RawFaceTrackingVideo": ["*face.avi", "*face.mp4"],
-            "RawEyeTrackingVideoMetadata": "*eye.json",
-            "RawBehaviorTrackingVideoMetadata": "*behavior.json",
-            "RawFaceTrackingVideoMetadata": "*face.json",
-            "EcephysPlatformFile": "*platformD1.json",
-            "NewstepConfiguration": "*motor-locs.csv",
+            'mapping_pkl': ['*mapping*.pkl', '*stim.pkl'],
+            'replay_pkl': '*replay*.pkl',
+            'behavior_pkl': '*behavior*.pkl',
+            'opto_pkl': '*opto*.pkl',
+            'sync_file': '*.sync',
+            'RawEyeTrackingVideo': ['*.eye.avi', '*eye.mp4'],
+            'RawBehaviorTrackingVideo': ['*behavior.avi', '*behavior.mp4'],
+            'RawFaceTrackingVideo': ['*face.avi', '*face.mp4'],
+            'RawEyeTrackingVideoMetadata': '*eye.json',
+            'RawBehaviorTrackingVideoMetadata': '*behavior.json',
+            'RawFaceTrackingVideoMetadata': '*face.json',
+            'EcephysPlatformFile': '*platformD1.json',
+            'NewstepConfiguration': '*motor-locs.csv',
         }
 
         for fn in file_glob_dict:
             if isinstance(file_glob_dict[fn], list):
                 paths = [
                     glob_file(os.path.join(self.base_dir, f))
                     for f in file_glob_dict[fn]
                 ]
-                path = [p for p in paths if not p is None]
+                path = [p for p in paths if p is not None]
                 if len(path) > 0:
                     self.data_dict[fn] = path[0]
             else:
-                filepath = glob_file(os.path.join(self.base_dir, file_glob_dict[fn]))
+                filepath = glob_file(
+                    os.path.join(self.base_dir, file_glob_dict[fn])
+                )
                 if filepath is not None:
                     self.data_dict[fn] = filepath
 
         basename = os.path.basename(self.base_dir)
-        self.data_dict["es_id"] = basename.split("_")[0]
-        self.data_dict["external_specimen_name"] = basename.split("_")[1]
-        self.data_dict["datestring"] = basename.split("_")[2]
-        self.data_dict["rig"] = self.get_rig_from_platform()
+        self.data_dict['es_id'] = basename.split('_')[0]
+        self.data_dict['external_specimen_name'] = basename.split('_')[1]
+        self.data_dict['datestring'] = basename.split('_')[2]
+        self.data_dict['rig'] = self.get_rig_from_platform()
 
     def get_platform_info(self):
-        platform_file = self.data_dict["EcephysPlatformFile"]
-        with open(platform_file, "r") as file:
+        platform_file = self.data_dict['EcephysPlatformFile']
+        with open(platform_file, 'r') as file:
             self.platform_info = json.load(file)
 
     def get_rig_from_platform(self):
-        if not hasattr(self, "platform_info"):
+        if not hasattr(self, 'platform_info'):
             self.get_platform_info()
 
-        return self.platform_info["rig_id"]
+        return self.platform_info['rig_id']
 
     def get_probe_data(self):
-        self.data_dict["data_probes"] = []
+        self.data_dict['data_probes'] = []
 
         # get probe dirs
-        for probeID in "ABCDEF":
+        for probeID in 'ABCDEF':
             if self.cortical_sort:
                 probe_base = glob_file(
-                    os.path.join(self.base_dir, "cortical*probe" + probeID + "_sorted")
+                    os.path.join(
+                        self.base_dir, 'cortical*probe' + probeID + '_sorted'
+                    )
                 )
                 lfp_base = glob_file(
-                    os.path.join(self.base_dir, "*probe" + probeID + "_sorted")
+                    os.path.join(self.base_dir, '*probe' + probeID + '_sorted')
                 )
             else:
                 probe_base = glob_file(
-                    os.path.join(self.base_dir, "*probe" + probeID + "_sorted")
+                    os.path.join(self.base_dir, '*probe' + probeID + '_sorted')
                 )
                 lfp_base = probe_base
 
             if probe_base is not None:
-                self.data_dict["data_probes"].append(probeID)
-                self.data_dict["probe" + probeID] = probe_base
+                self.data_dict['data_probes'].append(probeID)
+                self.data_dict['probe' + probeID] = probe_base
 
                 metrics_file = glob_file(
                     os.path.join(
-                        probe_base, r"continuous\Neuropix-PXI-100.0\metrics.csv"
+                        probe_base,
+                        r'continuous\Neuropix-PXI-100.0\metrics.csv',
                     )
                 )
-                self.data_dict["probe" + probeID + "_metrics"] = metrics_file
+                self.data_dict['probe' + probeID + '_metrics'] = metrics_file
 
-                info_json = glob_file(os.path.join(probe_base, "*probe_info*json"))
-                self.data_dict["probe" + probeID + "_info"] = info_json
+                info_json = glob_file(
+                    os.path.join(probe_base, '*probe_info*json')
+                )
+                self.data_dict['probe' + probeID + '_info'] = info_json
 
                 channel_map = glob_file(
                     os.path.join(
-                        probe_base, r"continuous\Neuropix-PXI-100.0\channel_map.npy"
+                        probe_base,
+                        r'continuous\Neuropix-PXI-100.0\channel_map.npy',
                     )
                 )
-                self.data_dict["probe" + probeID + "_channel_map"] = channel_map
+                self.data_dict[
+                    'probe' + probeID + '_channel_map'
+                ] = channel_map
 
             if lfp_base is not None:
-                self.data_dict["lfp" + probeID] = lfp_base
+                self.data_dict['lfp' + probeID] = lfp_base
 
     def get_image_data(self):
         # GET PROBE DEPTH IMAGES
-        for probeID in self.data_dict["data_probes"]:
-            probe_base = self.data_dict["probe" + probeID]
-            probe_depth_image = glob_file(os.path.join(probe_base, "probe_depth*.png"))
+        for probeID in self.data_dict['data_probes']:
+            probe_base = self.data_dict['probe' + probeID]
+            probe_depth_image = glob_file(
+                os.path.join(probe_base, 'probe_depth*.png')
+            )
             if probe_depth_image is not None:
-                self.data_dict["probe_depth_" + probeID] = probe_depth_image
+                self.data_dict['probe_depth_' + probeID] = probe_depth_image
 
         # GET OTHER IMAGE FILES
         # image_files = [k for k in D1_local if 'image' in k]
         image_files = [
-            "EcephysPostExperimentLeft",
-            "EcephysPostExperimentRight",
-            "EcephysPostInsertionLeft",
-            "EcephysPostInsertionRight",
-            "EcephysPostStimulusLeft",
-            "EcephysPostStimulusRight",
-            "EcephysPreExperimentLeft",
-            "EcephysPreExperimentRight",
-            "EcephysPreInsertionLeft",
-            "EcephysPreInsertionRight",
-            "EcephysInsertionLocationImage",
-            "EcephysOverlayImage",
-            "EcephysBrainSurfaceLeft",
-            "EcephysBrainSurfaceRight",
+            'EcephysPostExperimentLeft',
+            'EcephysPostExperimentRight',
+            'EcephysPostInsertionLeft',
+            'EcephysPostInsertionRight',
+            'EcephysPostStimulusLeft',
+            'EcephysPostStimulusRight',
+            'EcephysPreExperimentLeft',
+            'EcephysPreExperimentRight',
+            'EcephysPreInsertionLeft',
+            'EcephysPreInsertionRight',
+            'EcephysInsertionLocationImage',
+            'EcephysOverlayImage',
+            'EcephysBrainSurfaceLeft',
+            'EcephysBrainSurfaceRight',
         ]
         from np_session.components.lims_manifests import Manifest, MANIFESTS
+
         manifest = Manifest(self.base_dir)
-        
+
         for im in image_files:
-            rel_path = manifest.globs[manifest.names.index(MANIFESTS['_lims_name'][im])]
+            rel_path = manifest.globs[
+                manifest.names.index(MANIFESTS['_lims_name'][im])
+            ]
             im_file = glob_file(os.path.join(self.base_dir, rel_path))
 
             self.data_dict[im] = im_file
 
 
 def glob_file(file_path):
     f = glob.glob(file_path)
@@ -554,17 +584,17 @@
         return f[0]
     else:
         return None
 
 
 def convert_lims_path(path):
     if path is not None:
-        new_path = r"\\" + os.path.normpath(path)[1:]
+        new_path = r'\\' + os.path.normpath(path)[1:]
     else:
-        new_path = ""
+        new_path = ''
 
     return new_path
 
 
 def convert_path_str_to_pathlib(data_dict_orig) -> dict:
     """
     >>> orig = {0: '\\\\allen\\programs\\mindscope'}
@@ -577,18 +607,19 @@
 
     >>> test = convert_path_str_to_pathlib({1: '/allen/programs/mindscope'})
     >>> test[1].as_posix()
     '//allen/programs/mindscope'
     """
     data_dict = data_dict_orig.copy()
     for k, v in data_dict.items():
-        if isinstance(v, str) and (v.startswith("/") or v.startswith("\\")):
-            v = v.replace("\\", "/")
-            if v[:2] != "//":
-                v = "/" + v
+        if isinstance(v, str) and (v.startswith('/') or v.startswith('\\')):
+            v = v.replace('\\', '/')
+            if v[:2] != '//':
+                v = '/' + v
             data_dict[k] = pathlib.Path(v)
     return data_dict
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     import doctest
+
     doctest.testmod()
```

### Comparing `np-session-0.5.4/src/np_session/databases/firebase_state.py` & `np-session-0.6.0/src/np_session/databases/firebase_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import doctest
 import pathlib
 from collections.abc import MutableMapping
 from typing import ClassVar, Iterator, Union
 
 import firebase_admin
 import firebase_admin.firestore as firestore
-import np_logging
 
 AcceptedType = Union[str, int, float, bool, list, None]
 
+
 class State(MutableMapping):
     """Get and set session state in Firebase via a dict interface.
-    
+
     - dict interface provides `keys`, `get`, `setdefault`, `pop`, etc.
     - accepted value types are str, int, float, bool, None
 
     >>> test_id = 123456
     >>> state = State(test_id)
     >>> state['new'] = 1.0
     >>> state['new']
@@ -31,34 +31,36 @@
     'new'
     >>> state.pop('new')
     'new'
     >>> del state['new']
     >>> state.get('new') is None
     True
     """
-    
+
     db: ClassVar
-    
+
     def __init__(self, id: int | str) -> None:
         self.id = str(id)
         try:
             _ = self.db
         except AttributeError:
             self.__class__.connect()
 
     def __repr__(self) -> str:
         return repr(self.session_doc.get().to_dict())
-    
+
     @classmethod
     def connect(cls) -> None:
-        key_path = pathlib.Path('//allen/scratch/aibstemp/arjun.sridhar/db_key.json')
+        key_path = pathlib.Path(
+            '//allen/scratch/aibstemp/arjun.sridhar/db_key.json'
+        )
         cred = firebase_admin.credentials.Certificate(key_path)
         cls.app = firebase_admin.initialize_app(cred)
-        cls.db = firestore.client().collection(u'session_state')
-        #cls.ref = cls.db.reference('/session_state') # root user, can create users and add them also if needed
+        cls.db = firestore.client().collection('session_state')
+        # cls.ref = cls.db.reference('/session_state') # root user, can create users and add them also if needed
 
     @property
     def session_doc(self):
         """
         returns document snapshot
         """
         doc = self.db.document(str(self.id))
@@ -82,11 +84,11 @@
         """
         updates the database with the key value item
         """
         return self.session_doc.update({key: value})
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.session_doc.get().to_dict())
-    
+
+
 if __name__ == '__main__':
     doctest.testmod(verbose=True)
-
```

### Comparing `np-session-0.5.4/src/np_session/databases/lims2.py` & `np-session-0.6.0/src/np_session/databases/lims2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Critical components of an NP experiment workflow that come from lims2.
 
 - user/operator info
-- mouse info 
+- mouse info
     - isi experiment
     - project name
 
 Combined, these are sufficient to create a new ecephys session entry in lims2.
 
 Tools are also provided to construct commonly used abbreviations or folder names, and to
 reverse these 'NP' formats to reconstruct the Info objects used during an
 experiment workflow.
-
 """
 from __future__ import annotations
 
 import abc
 import collections
 import datetime
 import doctest
@@ -30,32 +29,39 @@
 from typing_extensions import Literal
 
 logger = np_logging.getLogger(__name__)
 
 
 def requester(url: str, *args) -> dict:
     request = url.format(*args)  # .replace(";", "%3B")
-    logger.debug(f"Requesting {request}")
+    logger.debug(f'Requesting {request}')
     response = requests.get(request)
     if response.status_code != 200:
-        raise ValueError(f"Bad response from {request}: {response.status_code}")
+        raise ValueError(
+            f'Bad response from {request}: {response.status_code}'
+        )
     return response.json()
 
 
-request = lambda url: functools.partial(requester, url)
-donor_info = request("http://lims2/donors/info/details.json?external_donor_name={}")
-user_info = request("http://lims2/users.json?login={}")
-ecephys_info = request("http://lims2/ecephys_sessions.json?id={}")
-behavior_info = request("http://lims2/behavior_sessions.json?id={}")
-isi_info = request("http://lims2/specimens/isi_experiment_details/{}.json")
-project_info = request("http://lims2/projects.json?code={}")
+def request(url):
+    return functools.partial(requester, url)
+
+
+donor_info = request(
+    'http://lims2/donors/info/details.json?external_donor_name={}'
+)
+user_info = request('http://lims2/users.json?login={}')
+ecephys_info = request('http://lims2/ecephys_sessions.json?id={}')
+behavior_info = request('http://lims2/behavior_sessions.json?id={}')
+isi_info = request('http://lims2/specimens/isi_experiment_details/{}.json')
+project_info = request('http://lims2/projects.json?code={}')
 
 
 class LIMS2InfoBaseClass(collections.UserDict, abc.ABC):
-    "Store details for an object in a dict-like. The commonly-used format of its name, e.g. '366122' for a mouse ID, can be obtained by converting to str()."
+    """Store details for an object in a dict-like. The commonly-used format of its name, e.g. '366122' for a mouse ID, can be obtained by converting to str()."""
 
     np_id: int | str
     "Commonly-used format of the object's value among the neuropixels team e.g. for a mouse -> the labtracks ID (366122)."
 
     _type: Type = NotImplemented
     _get_info: Callable[[str | int], dict] = NotImplemented
 
@@ -67,61 +73,61 @@
         self.fetch()
         return super().__getitem__(key)
 
     def __str__(self):
         return str(self.np_id)
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self.np_id!r})"
+        return f'{self.__class__.__name__}({self.np_id!r})'
 
     def __bool__(self):
         try:
             self.info_from_lims()
         except ValueError:
             return False
         else:
             return True
 
     def info_from_lims(self) -> dict[str, Any]:
-        "Return the object's info from lims database or raises a ValueError if not found."
+        """Return the object's info from lims database or raises a ValueError if not found."""
         try:
             return self._get_info(self.np_id)[0]
         except IndexError:
             raise ValueError(
-                f"Could not find {self.__class__.__name__} {self.np_id} in lims"
+                f'Could not find {self.__class__.__name__} {self.np_id} in lims'
             ) from None
 
     def fetch(self):
-        "Fetch the object's info from lims once."
+        """Fetch the object's info from lims once."""
         if not self.data:
             try:
                 info = self.info_from_lims()
             except ValueError:
                 self.data = {}
             else:
                 self.data = dict(**info)
 
     def keys(self):
-        "Fetch before returning keys."
+        """Fetch before returning keys."""
         self.fetch()
         return self.data.keys()
 
     def items(self):
-        "Fetch before returning keys."
+        """Fetch before returning keys."""
         self.fetch()
         return self.data.items()
 
     def values(self):
-        "Fetch before returning keys."
+        """Fetch before returning keys."""
         self.fetch()
         return self.data.values()
 
     @abc.abstractproperty
     def lims_id(self):
-        "LIMS2 ID for the object, usually different to the np_id."
+        """LIMS2 ID for the object, usually different to the np_id."""
         return NotImplemented
 
     @property
     def id(self) -> str | int:
         return self.lims_id
 
     # end of baseclass properties & methods ------------------------------ #
@@ -144,92 +150,94 @@
     """
 
     _type = int
     _get_info = donor_info
 
     @property
     def lims_id(self) -> int:
-        return self["specimens"][0]["id"]
+        return self['specimens'][0]['id']
 
     @property
     def isi_info(self) -> dict | None:
-        "Info from lims about the mouse's ISI experiments."
-        if not hasattr(self, "_isi_info"):
+        """Info from lims about the mouse's ISI experiments."""
+        if not hasattr(self, '_isi_info'):
             response = isi_info(str(self.np_id))
             if response:
                 self._isi_info = response[0]
             else:
                 self._isi_info = None
         return self._isi_info
 
     @property
     def isi_id(self) -> int | None:
-        "ID of the mouse's most recent ISI experiment not marked `failed`."
-        exps: list = self.isi_info["isi_experiments"]
-        exps.sort(key=lambda x: x["id"], reverse=True)
+        """ID of the mouse's most recent ISI experiment not marked `failed`."""
+        exps: list = self.isi_info['isi_experiments']
+        exps.sort(key=lambda x: x['id'], reverse=True)
         for exp in exps:
-            if exp["workflow_state"] != "failed":
-                return exp["id"]
+            if exp['workflow_state'] != 'failed':
+                return exp['id']
         return None
 
     @property
     def isi_targets(self) -> tuple[dict[Literal['x', 'y'], float], ...] | None:
-        "List of targets in image space for the mouse's most recent ISI experiment not marked `failed`."
+        """List of targets in image space for the mouse's most recent ISI experiment not marked `failed`."""
         if self.isi_info:
-            for isi_exp in self.isi_info["isi_experiments"]:
-                if isi_exp["id"] == self.isi_id:
-                    return tuple(isi_exp['targets']['insertion_targets']['image_space'])
+            for isi_exp in self.isi_info['isi_experiments']:
+                if isi_exp['id'] == self.isi_id:
+                    return tuple(
+                        isi_exp['targets']['insertion_targets']['image_space']
+                    )
         return None
-    
+
     @property
     def project_id(self) -> int:
-        "ID of the the project the mouse belongs to."
-        return self["specimens"][0]["project_id"]
+        """ID of the the project the mouse belongs to."""
+        return self['specimens'][0]['project_id']
 
     @property
     def project_name(self) -> str:
-        "PascalCase name of the project the mouse belongs to."
-        return self["specimens"][0]["project"]["code"]
+        """PascalCase name of the project the mouse belongs to."""
+        return self['specimens'][0]['project']['code']
 
     @property
     def path(self) -> pathlib.Path:
-        "Allen network dir where the mouse's sessions are stored."
-        return pathlib.Path(self["specimens"][0]["storage_directory"])
+        """Allen network dir where the mouse's sessions are stored."""
+        return pathlib.Path(self['specimens'][0]['storage_directory'])
 
 
 class LIMS2UserInfo(LIMS2InfoBaseClass):
-    "Store details for a user/operator."
+    """Store details for a user/operator."""
 
     _type = str
     _get_info = user_info
 
     @property
     def lims_id(self) -> int:
-        return self["id"]
+        return self['id']
 
 
 class LIMS2ProjectInfo(LIMS2InfoBaseClass):
-    "Store details for a project."
+    """Store details for a project."""
 
     _type = str
     _get_info = project_info
 
     @property
     def lims_id(self) -> int:
-        return self["id"]
+        return self['id']
 
 
 class LIMS2SessionInfo(LIMS2InfoBaseClass):
-    "Store details for an ecephys or behavior session."
+    """Store details for an ecephys or behavior session."""
 
     _type = int
     _get_info = ecephys_info  # default - behavior_info may be used instead
 
     def __str__(self):
-        return f"{self.np_id}"
+        return f'{self.np_id}'
 
     @property
     def lims_id(self) -> int:
         return self.np_id
 
     @property
     def session(self) -> str:
@@ -244,132 +252,134 @@
     def info_from_lims(self) -> dict:
         try:
             data = super().info_from_lims()  # with ecephys_info
         except ValueError:
             response = behavior_info(self.np_id)  # try behavior_info instead
             if not response:
                 raise
-            self._session = "behavior"
+            self._session = 'behavior'
             data = response[0]
         else:
-            self._session = "ecephys"
+            self._session = 'ecephys'
         self.cast()
         return data
 
     def cast(self):
-        if not hasattr(self, "_session"):
+        if not hasattr(self, '_session'):
             _ = self.fetch()  # trigger fetching data from lims
         self.__class__ = (
             LIMS2EcephysSessionInfo
-            if self._session == "ecephys"
+            if self._session == 'ecephys'
             else LIMS2BehaviorSessionInfo
         )
 
 
 class LIMS2EcephysSessionInfo(LIMS2SessionInfo):
-    "Don't instantiate directly, use LIMS2SessionInfo and class will be converted after info fetched from lims."
+    """Don't instantiate directly, use LIMS2SessionInfo and class will be converted after info fetched from lims."""
 
     def get_folder(self) -> str:
         return f"{self.np_id}_{self['specimen']['external_specimen_name']}_{self['name'].replace('HAB_', '')[:8]}"
 
     def __repr__(self):
-        return f"{__class__.__bases__[0].__name__}({self.np_id!r})"
+        return f'{__class__.__bases__[0].__name__}({self.np_id!r})'
 
 
 class LIMS2BehaviorSessionInfo(LIMS2SessionInfo):
-    "Don't instantiate directly, use LIMS2SessionInfo and class will be converted after info fetched from lims."
+    """Don't instantiate directly, use LIMS2SessionInfo and class will be converted after info fetched from lims."""
 
     def get_folder(self) -> str:
         return f"{self.np_id}_{self['donor']['name'].split('-')[-1]}_{self['ecephys_session']['name'][:8]}"
 
     def __repr__(self):
-        return f"{__class__.__bases__[0].__name__}({self.np_id!r})"
+        return f'{__class__.__bases__[0].__name__}({self.np_id!r})'
 
 
 # end of classes ----------------------------------------------------------------------- #
 
 
 def generate_ephys_session(
     mouse: str | int | LIMS2MouseInfo,
     user: str | LIMS2UserInfo,
 ) -> LIMS2SessionInfo:
-    "Create a new session and return an object instance with its info."
+    """Create a new session and return an object instance with its info."""
 
     if not isinstance(mouse, LIMS2MouseInfo):
         mouse = LIMS2MouseInfo(mouse)
     if not isinstance(user, LIMS2UserInfo):
         user = LIMS2UserInfo(user)
 
-    timestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
+    timestamp = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
     request_json = {
-        "specimen_id": mouse.lims_id,
-        "project_id": mouse.project_id,
-        "isi_experiment_id": mouse.isi_id,
-        "name": f"{timestamp}_{user.lims_id}",
-        "operator_id": user.lims_id,
+        'specimen_id': mouse.lims_id,
+        'project_id': mouse.project_id,
+        'isi_experiment_id': mouse.isi_id,
+        'name': f'{timestamp}_{user.lims_id}',
+        'operator_id': user.lims_id,
     }
-    url = "http://lims2/observatory/ecephys_session/create"
+    url = 'http://lims2/observatory/ecephys_session/create'
     response = requests.post(url, json=request_json)
-    decoded_dict = json.loads(response.content.decode("utf-8"))
-    new_session_id = decoded_dict["id"]
+    decoded_dict = json.loads(response.content.decode('utf-8'))
+    new_session_id = decoded_dict['id']
     if not new_session_id:
-        raise ValueError(f"Failed to create session: {decoded_dict}")
+        raise ValueError(f'Failed to create session: {decoded_dict}')
     return LIMS2SessionInfo(new_session_id)
 
 
 def generate_hab_session(
     mouse: str | int | LIMS2MouseInfo,
     user: str | LIMS2UserInfo,
 ) -> LIMS2SessionInfo:
-    "Create a new session and return an object instance with its info."
+    """Create a new session and return an object instance with its info."""
 
     if not isinstance(mouse, LIMS2MouseInfo):
         mouse = LIMS2MouseInfo(mouse)
     if not isinstance(user, LIMS2UserInfo):
         user = LIMS2UserInfo(user)
 
-    timestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
+    timestamp = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
     request_json = {
-        "specimen_id": mouse.lims_id,
-        "project_id": mouse.project_id,
-        "isi_experiment_id": mouse.isi_id,
-        "name": f"HAB_{timestamp}_{user.lims_id}",
-        "operator_id": user.lims_id,
+        'specimen_id': mouse.lims_id,
+        'project_id': mouse.project_id,
+        'isi_experiment_id': mouse.isi_id,
+        'name': f'HAB_{timestamp}_{user.lims_id}',
+        'operator_id': user.lims_id,
     }
-    url = "http://lims2/observatory/ecephys_session/create"
+    url = 'http://lims2/observatory/ecephys_session/create'
     response = requests.post(url, json=request_json)
-    decoded_dict = json.loads(response.content.decode("utf-8"))
-    new_session_id = decoded_dict["id"]
+    decoded_dict = json.loads(response.content.decode('utf-8'))
+    new_session_id = decoded_dict['id']
     if not new_session_id:
-        raise ValueError(f"Failed to create session: {decoded_dict}")
+        raise ValueError(f'Failed to create session: {decoded_dict}')
     return LIMS2SessionInfo(new_session_id)
 
+
 def find_session_folder_string(path: str | pathlib.Path) -> str | None:
     """Extract [8+digit session ID]_[6-digit mouse ID]_[6-digit date
     str] from a file or folder path"""
-    session_reg_exp = r"[0-9]{8,}_[0-9]{6}_[0-9]{8}"
+    session_reg_exp = r'[0-9]{8,}_[0-9]{6}_[0-9]{8}'
     session_folders = re.findall(session_reg_exp, str(path))
     if session_folders:
         if not all(s == session_folders[0] for s in session_folders):
             raise ValueError(
-                f"Mismatch between session folder strings - file may be in the wrong folder: {path}"
+                f'Mismatch between session folder strings - file may be in the wrong folder: {path}'
             )
         return session_folders[0]
     return None
 
+
 def info_classes_from_session_folder(
     session_folder: str,
 ) -> tuple[LIMS2SessionInfo, LIMS2MouseInfo, LIMS2UserInfo]:
-    "Reconstruct Info objects from a session folder string."
+    """Reconstruct Info objects from a session folder string."""
     folder = find_session_folder_string(session_folder)
     if not folder:
-        raise ValueError(f"{session_folder} is not a valid session folder")
+        raise ValueError(f'{session_folder} is not a valid session folder')
 
-    session = LIMS2SessionInfo(folder.split("_")[0])
-    mouse = LIMS2MouseInfo(folder.split("_")[1])
-    user = LIMS2UserInfo(session["operator"]["login"])
+    session = LIMS2SessionInfo(folder.split('_')[0])
+    mouse = LIMS2MouseInfo(folder.split('_')[1])
+    user = LIMS2UserInfo(session['operator']['login'])
 
     return (session, mouse, user)
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     doctest.testmod()
```

### Comparing `np-session-0.5.4/src/np_session/databases/mtrain.py` & `np-session-0.6.0/src/np_session/databases/mtrain.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,63 +9,66 @@
 
 
 class MouseNotInMTrainError(Exception):
     pass
 
 
 class MTrain:
-    server = "http://mtrain:5000"
+    server = 'http://mtrain:5000'
 
     @classmethod
     def connected(cls) -> bool:
         response = requests.get(cls.server)
         return True if response.status_code == 200 else False
 
     def __init__(self, mouse_id: Optional[int | str] = None):
         # we'll only allow mouse_id to be set once per instance
         # but it doesn't necessarily have to be set on init
         if mouse_id:
             self.mouse_id = mouse_id
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self.mouse_id!r})"
+        return f'{self.__class__.__name__}({self.mouse_id!r})'
 
     def session(self):
         session = requests.session()
         session.post(
             self.server,
             data={
-                "username": "chrism",
-                "password": "password",
+                'username': 'chrism',
+                'password': 'password',
             },
         )
         return session
 
     @property
     def mouse_id(self) -> str:
         return self._mouse_id
 
     @mouse_id.setter
     def mouse_id(self, value: int | str):
-        if hasattr(self, "_mouse_id") and self._mouse_id is not None:
-            raise ValueError("Mouse ID can only be set once per instance.")
+        if hasattr(self, '_mouse_id') and self._mouse_id is not None:
+            raise ValueError('Mouse ID can only be set once per instance.')
         response = requests.get(
-            f"{self.server}/get_script/", data=json.dumps({"LabTracks_ID": str(value)})
+            f'{self.server}/get_script/',
+            data=json.dumps({'LabTracks_ID': str(value)}),
         )
         if response.status_code == 200:
             self._mouse_id = str(value)
         else:
-            raise MouseNotInMTrainError(f"Mouse ID {value} not found in MTrain")
+            raise MouseNotInMTrainError(
+                f'Mouse ID {value} not found in MTrain'
+            )
 
     @property
     def state(self) -> dict[str, int]:
         """Returns dict with values 'id', 'regimen_id', 'stage_id' - all ints"""
-        return requests.get(f"{self.server}/api/v1/subjects/{self.mouse_id}").json()[
-            "state"
-        ]
+        return requests.get(
+            f'{self.server}/api/v1/subjects/{self.mouse_id}'
+        ).json()['state']
 
     @state.setter
     def state(self, value: dict | int | str):
         """Allows switching to one of the states in the current regimen.
 
         To change regimen, use set_regimen_and_stage()
 
@@ -73,84 +76,84 @@
         """
         valid_dict = valid_id = None
 
         if isinstance(value, dict):
             if value in self.states:
                 valid_dict = value
             elif (
-                hasattr(value, "regimen_id")
-                and (str(value["regimen_id"]) in self.all_regimens().keys())
-                and not (value["regimen_id"] == self.regimen["id"])
+                hasattr(value, 'regimen_id')
+                and (str(value['regimen_id']) in self.all_regimens().keys())
+                and not (value['regimen_id'] == self.regimen['id'])
             ):
                 warnings.warn(
                     "Trying to change regimen via set state method: use 'obj.regimen=...' instead"
                 )
                 return
 
         elif isinstance(value, int) or value.isdigit():
             # check if input matches a state id
             valid_id = (
                 int(value)
-                if str(value) in [str(s["id"]) for s in self.states]
+                if str(value) in [str(s['id']) for s in self.states]
                 else None
             )
 
         elif isinstance(value, str) and value.lower() in [
-            str(s["name"]).lower() for s in self.stages
+            str(s['name']).lower() for s in self.stages
         ]:
             # check if input matches a stage name
-            valid_id = [s["id"] for s in self.stages if s["name"] == value][0]
+            valid_id = [s['id'] for s in self.stages if s['name'] == value][0]
 
         if not any([valid_dict, valid_id]):
             warnings.warn(
                 f"No matching state found in regimen {self.regimen['name']}. Check obj.states"
             )
             return
 
         if valid_id and not valid_dict:
-            value = [s for s in self.states if s["id"] == value][0]
+            value = [s for s in self.states if s['id'] == value][0]
 
         with self.session() as s:
             s.post(
-                f"{self.server}/set_state/{self.mouse_id}",
+                f'{self.server}/set_state/{self.mouse_id}',
                 data={
-                    "state": json.dumps(value),
+                    'state': json.dumps(value),
                 },
             )
-        assert self.state == value, "set state failed!"
+        assert self.state == value, 'set state failed!'
 
     @property
     def states(self):
-        return self.regimen["states"]
+        return self.regimen['states']
 
     @property
     def regimen(self) -> dict:
         """Returns dictionary containing 'id', 'name', 'stages', 'states'"""
         return requests.get(
             f"{self.server}/api/v1/regimens/{self.state['regimen_id']}"
         ).json()
 
     @property
     def all_behavior_sessions(self) -> dict:
         """Returns dictionary containing details of all behavior sessions for mouse_id"""
         result = requests.get(
-            f"{self.server}/get_behavior_sessions/",
-            data=json.dumps({"LabTracks_ID": str(self.mouse_id)}),
+            f'{self.server}/get_behavior_sessions/',
+            data=json.dumps({'LabTracks_ID': str(self.mouse_id)}),
         )
 
         if result:
-            return result.json()["results"]
+            return result.json()['results']
         return None
 
     def last_behavior_session_on(self, query_date: datetime.date) -> dict:
         all_behavior_sessions = self.all_behavior_sessions
         matching_sessions = []
         for session in all_behavior_sessions:
             session_datetime = datetime.datetime.strptime(
-                session["date"], "%a, %d %b %Y %H:%M:%S %Z"
+                session['date'], '%a, %d %b %Y %H:%M:%S %Z'
             )
             if session_datetime.date() == query_date:
                 matching_sessions.append(session)
 
         if matching_sessions:
             return matching_sessions[-1]
         return {}
@@ -166,109 +169,117 @@
         regimen: Optional[dict | int | str] = None,
         stage: Optional[dict | int | str] = None,
     ):
         """Requires a regimen dict, id (str/int) or name (str), plus stage dict, id (str/int) or name (str)"""
 
         def warn_and_return():
             warnings.warn(
-                "Regimen not changed: invalid input. Provide an identifier for both a regimen and a stage."
+                'Regimen not changed: invalid input. Provide an identifier for both a regimen and a stage.'
             )
             return
 
         if not regimen and stage:
             warn_and_return()
 
         # we're not setting the regimen directly - we just need some info to set a valid state
         regimen_id: int = None
         stage_id: int = None
 
         if isinstance(regimen, dict):
-            if regimen in self.get_all("regimens"):
+            if regimen in self.get_all('regimens'):
                 # valid dict provided
-                regimen_id = regimen["id"]
+                regimen_id = regimen['id']
             else:
                 warn_and_return()
 
         elif str(regimen) in self.all_regimens().keys():
             # valid id provided
             regimen_id = int(regimen)
 
-        elif any(str(regimen) == s.lower() for s in self.all_regimens().values()):
+        elif any(
+            str(regimen) == s.lower() for s in self.all_regimens().values()
+        ):
             # valid name provided
             regimen_id = [
-                s["id"]
-                for s in self.get_all("regimens")
-                if s["name"].lower() == str(regimen).lower()
+                s['id']
+                for s in self.get_all('regimens')
+                if s['name'].lower() == str(regimen).lower()
             ][0]
 
         else:
             warn_and_return()
 
         # get the stages available in the new regimen, without setting anything yet
         # new_regimen = self.get_all("regimens")['id'==regimen_id]
-        new_regimen = [s for s in self.get_all("regimens") if s["id"] == regimen_id][0]
-        new_stages = new_regimen["stages"]
+        new_regimen = [
+            s for s in self.get_all('regimens') if s['id'] == regimen_id
+        ][0]
+        new_stages = new_regimen['stages']
 
         if isinstance(stage, dict):
             if stage in new_stages:
-                stage_id = stage["id"]  # valid dict provided
+                stage_id = stage['id']  # valid dict provided
             else:
                 warn_and_return()
 
-        elif str(stage) in [str(s["id"]) for s in new_stages]:
+        elif str(stage) in [str(s['id']) for s in new_stages]:
             stage_id = int(stage)  # valid id provided
 
-        elif str(stage).lower() in [str(s["name"]).lower() for s in new_stages]:
-            stage_id = [s["id"] for s in new_stages if s["name"] == stage][
+        elif str(stage).lower() in [
+            str(s['name']).lower() for s in new_stages
+        ]:
+            stage_id = [s['id'] for s in new_stages if s['name'] == stage][
                 0
             ]  # valid name provided
 
         else:
             warn_and_return()
 
         # look for corresponding state
         state_match = [
             s
-            for s in new_regimen["states"]
-            if s["regimen_id"] == regimen_id and s["stage_id"] == stage_id
+            for s in new_regimen['states']
+            if s['regimen_id'] == regimen_id and s['stage_id'] == stage_id
         ]
         if not state_match or len(state_match) != 1:
             warn_and_return()
         new_state = state_match[0]
 
         # set directly instead of using state set method (which intentionally blocks setting a state dict with a new regimen)
         with self.session() as s:
             s.post(
-                f"{self.server}/set_state/{self.mouse_id}",
+                f'{self.server}/set_state/{self.mouse_id}',
                 data={
-                    "state": json.dumps(new_state),
+                    'state': json.dumps(new_state),
                 },
             )
-        assert self.state == new_state, "set regimen and stage failed!"
+        assert self.state == new_state, 'set regimen and stage failed!'
 
     @property
     def stage(self):
         for item in self.stages:
-            if item["id"] == self.state["stage_id"]:
+            if item['id'] == self.state['stage_id']:
                 return item
 
     @stage.setter
     def stage(self, value: str | int):
         """Accepts stage id (int/str) or name (str)"""
 
         state_match = None
 
         if isinstance(value, int) or value.isdigit():
             value = int(value)
-            state_match = [s for s in self.states if s["stage_id"] == value]
+            state_match = [s for s in self.states if s['stage_id'] == value]
 
         if isinstance(value, str):
-            stage_match = [s for s in self.stages if s["name"].lower() == value.lower()]
+            stage_match = [
+                s for s in self.stages if s['name'].lower() == value.lower()
+            ]
             state_match = [
-                s for s in self.states if s["stage_id"] == stage_match[0]["id"]
+                s for s in self.states if s['stage_id'] == stage_match[0]['id']
             ]
 
         if not state_match or len(state_match) != 1:
             warnings.warn(
                 f'No state with stage name or id {value} found in regimen {self.regimen["name"]}. Check obj.stages or obj.states'
             )
             return
@@ -285,87 +296,89 @@
         """Accepts stage id (int/str) or name (str)
         Re-routes to stage property
         """
         self.stage = value
 
     @property
     def stages(self):
-        return self.regimen["stages"]
+        return self.regimen['stages']
 
     @classmethod
     def paginated_get(cls, route, page_size=10, offset=0):
         page_number = offset + 1  # page number is 1 based, offset is page
         result = requests.get(
-            f"{route}?results_per_page={page_size}&page={page_number}"
+            f'{route}?results_per_page={page_size}&page={page_number}'
         ).json()
-        total_pages = result["total_pages"]
+        total_pages = result['total_pages']
         if page_number == total_pages:
             new_offset = None
             has_more = False
         else:
             new_offset = offset + 1
             has_more = True
 
-        return result["objects"], has_more, new_offset
+        return result['objects'], has_more, new_offset
 
     @classmethod
     def get_all(cls, endpoint: str):
         # page_size = 200 is over the actual page size limit for the api but we don't appear to know what that value is
         # ? 'total_pages': 18
-        if endpoint not in ["regimens", "states", "stages", "subjects"]:
-            raise ValueError(f"Endpoint {endpoint} not recognized")
+        if endpoint not in ['regimens', 'states', 'stages', 'subjects']:
+            raise ValueError(f'Endpoint {endpoint} not recognized')
         all = []
         max_fetch = 100
         page_size = 200
         offset = 0
         for _ in range(max_fetch):
             results, has_more, new_offset = cls.paginated_get(
-                f"{cls.server}/api/v1/{endpoint}", page_size, offset
+                f'{cls.server}/api/v1/{endpoint}', page_size, offset
             )
             all.extend(results)
             if not has_more:
                 break
             offset = new_offset
         else:
-            warnings.warn(f"Failed to get full list of {endpoint}.")
+            warnings.warn(f'Failed to get full list of {endpoint}.')
         return all
 
     @classmethod
     def all_regimens(cls) -> dict:
         """List of dicts {str(regimen['id']):regimen['name']}"""
         d = {}
-        for val in cls.get_all("regimens"):
-            d.update({str(val["id"]): val["name"]})
+        for val in cls.get_all('regimens'):
+            d.update({str(val['id']): val['name']})
         return d
 
     # the two methods below were added after the others above:
     # other functions could be re-written to use them for cleaner code
 
     @classmethod
     def all_states(cls) -> dict:
         """dict containing {str(state['id']):{'id':int,'regimen_id':int,'stage_id':int}}"""
         d = {}
-        for val in cls.get_all("states"):
-            d.update({str(val["id"]): val})
+        for val in cls.get_all('states'):
+            d.update({str(val['id']): val})
         return d
 
     @classmethod
     def all_stages(cls) -> dict:
         """Takes a while. dict containing {str(stage['id']):stage['name']}"""
         d = {}
-        for val in cls.get_all("stages"):
-            d.update({str(val["id"]): val["name"]})
+        for val in cls.get_all('stages'):
+            d.update({str(val['id']): val['name']})
         return d
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     # print(MTrain.connected())
-    x = MTrain("632296")
+    x = MTrain('632296')
     x.last_behavior_session_on(query_date=datetime.date(2022, 9, 27))
-    x.state = x.regimen["states"][0]
+    x.state = x.regimen['states'][0]
     x.state = 1734
     x.stage = 1751
-    illusion_regimens = [r for r in x.get_all("regimens") if "Illusion" in r["name"]]
+    illusion_regimens = [
+        r for r in x.get_all('regimens') if 'Illusion' in r['name']
+    ]
     # x.regimen = x.get_all("regimens")[4]
     x.all_stages()
     x.all_states()
     # x.set_regimen_and_stage(illusion_regimens[4], illusion_regimens[4]['stages'][4])
```

### Comparing `np-session-0.5.4/src/np_session/databases/redis_state.py` & `np-session-0.6.0/src/np_session/databases/redis_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 Redis connection for persisting np_session state.
-
-
 """
 from __future__ import annotations
 
 import collections.abc
 import contextlib
 import doctest
 import pathlib
@@ -13,30 +11,30 @@
 
 import np_logging
 import redis
 
 logger = np_logging.getLogger(__name__)
 
 password_file = pathlib.Path(
-        "//allen/scratch/aibstemp/arjun.sridhar/redis_db.txt"
+    '//allen/scratch/aibstemp/arjun.sridhar/redis_db.txt'
 )
 
 # AcceptedType will be coerced to RedisType before being stored in Redis:
 RedisType = Union[str, int, float]
 """Can be stored in Redis directly, or returned from Redis."""
 AcceptedType = Union[RedisType, bool, None]
 """Can be stored in Redis after using `encode(value: AcceptedType)`."""
 
 
 class State(collections.abc.MutableMapping):
     """Get and set session state in Redis via a dict interface.
 
     - dict interface provides `keys`, `get`, `setdefault`, `pop`, etc.
     - accepted value types are str, int, float, bool, None
-    
+
     >>> test_id = 0
     >>> state = State(test_id)
     >>> state['test'] = 1.0
     >>> state['test']
     1.0
     >>> state['test'] = 'test'
     >>> state['test']
@@ -59,65 +57,70 @@
         try:
             _ = self.db
         except AttributeError:
             self.__class__.connect()
 
     def __repr__(self) -> str:
         return self.data.__repr__()
-    
+
     @classmethod
     def connect(cls) -> None:
         password = password_file.read_text().strip()
         cls.db = redis.Redis(
-            host="redis-11877.c1.us-west-2-2.ec2.cloud.redislabs.com",
+            host='redis-11877.c1.us-west-2-2.ec2.cloud.redislabs.com',
             port=11877,
             password=password,
         )
         if cls.db.ping():
-            logger.debug("Connected to Redis database: %s", cls.db)
+            logger.debug('Connected to Redis database: %s', cls.db)
         else:
-            logger.error("Failed to connect to Redis database")
-            
+            logger.error('Failed to connect to Redis database')
+
     @property
     def data(self) -> dict[str, AcceptedType]:
-        return {k.decode(): decode(v) for k, v in self.db.hgetall(self.name).items()}
+        return {
+            k.decode(): decode(v)
+            for k, v in self.db.hgetall(self.name).items()
+        }
 
     def __getitem__(self, key: str) -> AcceptedType:
         _ = decode(self.db.hget(self.name, key))
         if _ is None:
-            raise KeyError(f"{key!r} not found in Redis db entry {self!r}")
+            raise KeyError(f'{key!r} not found in Redis db entry {self!r}')
         return _
-    
+
     def __setitem__(self, key: str, value: AcceptedType) -> None:
         self.db.hset(self.name, key, encode(value))
 
     def __delitem__(self, key: str) -> None:
         self.db.hdel(self.name, key)
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.data)
 
     def __len__(self) -> int:
         return len(self.data)
 
+
 def encode(value: AcceptedType) -> RedisType:
     """Redis can't store bools: convert to something compatible before entering."""
     if value in (True, False, None):
         return str(value)
     return value
 
+
 def decode(value: bytes | None) -> AcceptedType:
     """Redis stores everything as bytes: convert back to our original python datatype."""
     if value is None:
         return None
     decoded_value: str = value.decode()
     if decoded_value.isnumeric():
         return int(decoded_value)
     with contextlib.suppress(ValueError):
         return float(decoded_value)
     if decoded_value.capitalize() in (str(_) for _ in (True, False, None)):
         return eval(decoded_value.capitalize())
     return decoded_value
 
 
-if __name__ == "__main__":
-    doctest.testmod(verbose=True)
+if __name__ == '__main__':
+    doctest.testmod(verbose=True)
```

### Comparing `np-session-0.5.4/src/np_session/jobs/sessions.json` & `np-session-0.6.0/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.5.4/src/np_session/jobs/sync_states.py` & `np-session-0.6.0/src/np_session/jobs/sync_states.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from np_session.databases.firebase_state import State as Firebase
 from np_session.databases.redis_state import State as Redis
 
 logger = np_logging.getLogger(__name__)
 
 
-def sync_redis_to_firebase(
-) -> None:
+def sync_redis_to_firebase() -> None:
     """Sync Redis state to Firebase state."""
     for id in Redis.db.keys():
-        id = id.decode() # Redis keys are bytes
+        id = id.decode()   # Redis keys are bytes
         Firebase(id).update(Redis(id))
-        logger.debug(f"Synced {id} from Redis to Firebase.")
+        logger.debug(f'Synced {id} from Redis to Firebase.')
 
-if __name__ == "__main__":
+
+if __name__ == '__main__':
     Firebase.connect()
     Redis.connect()
-    sync_redis_to_firebase()
+    sync_redis_to_firebase()
```

### Comparing `np-session-0.5.4/src/np_session/session.py` & `np-session-0.6.0/src/np_session/subclasses/pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,667 +1,587 @@
-from __future__ import annotations
-
-import contextlib
-import copy
-import datetime
-import doctest
-import functools
-import itertools
-import os
-import pathlib
-import shutil
-from typing import Any, Callable, Generator, Iterable, MutableMapping, Optional, Union
-
-import np_config
-import np_logging
-from backports.cached_property import cached_property
-from typing_extensions import Literal
-
-from np_session.components.info import Mouse, Project, Projects, User
-from np_session.components.paths import *
-from np_session.components.platform_json import *
-from np_session.components.lims_manifests import Manifest
-from np_session.databases import State
-from np_session.databases import data_getters as dg
-from np_session.databases import lims2 as lims
-from np_session.databases import mtrain
-from np_session.utils import *
-
-logger = np_logging.getLogger(__name__)
-
-PathLike = Union[str, bytes, os.PathLike, pathlib.Path]
-# https://peps.python.org/pep-0519/#provide-specific-type-hinting-support
-# PathLike inputs are converted to pathlib.Path objects for os-agnostic filesystem operations.
-# os.fsdecode(path: PathLike) is used where only a string is required.
-
-
-class SessionError(ValueError):
-    """Raised when a session folder string ([lims-id]_[mouse-id]_[date]) can't be found in a
-    filepath"""
-
-    pass
-
-
-class FilepathIsDirError(ValueError):
-    """Raised when a directory is specified but a filepath is required"""
-
-    pass
-
-
-class Session:
-    """Session information from any string or PathLike containing a lims session ID.
-
-    Note: lims/mtrain properties may be empty or None if mouse/session isn't in db.
-    Note: `is_ecephys_session` checks ecephys vs behavior. habs are ecephys sessions in lims. 
-    
-    Quick access to useful properties:
-    >>> session = Session('c:/1116941914_surface-image1-left.png')
-    >>> session.lims.id
-    1116941914
-    >>> session.folder
-    '1116941914_576323_20210721'
-    >>> session.project.lims.id
-    714916854
-    >>> session.is_hab
-    False
-    >>> session.rig.acq # hostnames reflect the computers used during the session, not necessarily the current machines
-    'W10DT05515'
-
-    Some properties are returned as objects with richer information:
-    - `pathlib` objects for filesystem paths:
-    >>> session.lims_path.as_posix()
-    '//allen/programs/braintv/production/visualbehavior/prod0/specimen_1098595957/ecephys_session_1116941914'
-    >>> session.data_dict['storage_directory'].as_posix()
-    '//allen/programs/braintv/production/visualbehavior/prod0/specimen_1098595957/ecephys_session_1116941914'
-
-
-    - `datetime` objects for easy date manipulation:
-    >>> session.date
-    datetime.date(2021, 7, 21)
-
-    - dictionaries from lims (loaded lazily):
-    >>> session.mouse
-    Mouse(576323)
-    >>> session.mouse.lims
-    LIMS2MouseInfo(576323)
-    >>> session.mouse.lims.id
-    1098595957
-    >>> session.mouse.lims['full_genotype']
-    'wt/wt'
-
-    ...with a useful string representation:
-    >>> str(session.mouse)
-    '576323'
-    >>> str(session.project)
-    'NeuropixelVisualBehavior'
-    >>> str(session.rig)        # see np_config.Rig
-    'NP.0'
-    """
-
-    def __lt__(self, other: Session) -> bool:
-        if not hasattr(other, "date"):
-            return NotImplemented
-        return self.date < other.date
-    
-    def __eq__(self, other: Any) -> bool:
-        if not isinstance(other, (int, str, Session)):
-            return NotImplemented
-        if isinstance(other, Session):
-            return self.id == other.id
-        return str(self) == str(other) or str(self.id) == str(other) or self.folder == other
-    
-    def __hash__(self) -> int:
-        return hash(self.id) ^ hash(self.__class__.__name__)
-    
-    def __str__(self) -> str:
-        return self.folder
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.folder!r})"
-
-    def __init__(self, path_or_session: PathLike | int | LIMS2SessionInfo):
-        path_or_session = str(path_or_session)
-
-        path_or_session = pathlib.Path(path_or_session)
-
-        np_folder = folder(path_or_session)
-
-        if not np_folder:
-            np_folder = folder_from_lims_id(path_or_session)
-
-        if np_folder is None:
-            raise SessionError(
-                f"{path_or_session} does not contain a valid lims session id or session folder string"
-            )
-
-        self.folder = np_folder
-        self.id = int(self.folder.split("_")[0])
-
-        if isinstance(path_or_session, LIMS2SessionInfo):
-            self._lims = path_or_session
-
-    @property
-    def lims(self) -> lims.LIMS2SessionInfo | dict:
-        """
-        >>> info = Session(1116941914).lims
-        >>> info['stimulus_name']
-        'EPHYS_1_images_H_3uL_reward'
-        >>> info['operator']['login']
-        'taminar'
-
-        >>> Session(1116941914).lims
-        LIMS2SessionInfo(1116941914)
-        >>> str(Session(1116941914).lims)
-        '1116941914'
-        """
-        if not hasattr(self, "_lims"):
-            try:
-                self._lims = lims.LIMS2SessionInfo(self.id)
-            except ValueError:
-                self._lims = {}
-        return self._lims
-
-    @property
-    def mouse(self) -> Mouse:
-        if not hasattr(self, "_mouse"):
-            self._mouse = Mouse(self.folder.split("_")[1])
-        return self._mouse
-
-    @property
-    def user(self) -> User | None:
-        if not hasattr(self, "_user"):
-            lims_user_id = self.lims.get("operator", {}).get("login", "")
-            if lims_user_id:
-                self._user = User(lims_user_id)
-            else:
-                self._user = None
-        return self._user
-
-    @cached_property
-    def date(self) -> datetime.date:
-        d = self.folder.split("_")[2]
-        date = datetime.date(year=int(d[:4]), month=int(d[4:6]), day=int(d[6:]))
-        return date
-
-    @property
-    def rig(self) -> np_config.Rig | None:
-        "Rig object with computer info and paths, can also be used as a string."
-        if not hasattr(self, "_rig"):
-            self._rig = None
-            while not self.rig:
-                # try from current rig first
-                with contextlib.suppress(ValueError):
-                    self.rig = np_config.Rig()
-                    continue
-
-                # try from platform json
-                with contextlib.suppress(Exception):
-                    self.rig = np_config.Rig(self.platform_json.rig_id)
-                # try from lims
-                rig_id: str | None = self.data_dict.get("rig")
-                if rig_id:
-                    self.rig = np_config.Rig(rig_id)
-                    continue
-
-                break
-        return self._rig
-
-    @rig.setter
-    def rig(self, value: np_config.Rig) -> None:
-        if not isinstance(value, np_config.Rig):
-            raise TypeError(
-                f"Expected `rig` to be an instance of `np_config.Rig`, not {type(value)}"
-            )
-        self._rig = value
-        self.update_hostnames_for_replaced_computers()
-
-    def update_hostnames_for_replaced_computers(self) -> None:
-        if not self._rig:
-            return
-        for comp in ("sync", "stim", "mon", "acq"):
-            replaced = old_hostname(f"{self._rig.id}-{comp.capitalize()}", self.date)
-            if replaced:
-                setattr(self._rig, f"_{comp}", replaced)
-
-    @property
-    def is_ecephys_session(self) -> bool | None:
-        """False if behavior session in lims, None if unsure.
-        
-        Note that habs are classed as ecephys sessions: use `is_hab`.
-        """
-        if not self.lims or not self.lims.get("ecephys_session"):
-            return None
-        return "ecephys_session" in self.lims['ecephys_session']
-
-    @property
-    def is_hab(self) -> bool | None:
-        """False if hab session, None if unsure."""
-        if not self.lims:
-            return None
-        return self.lims.get('name', '').startswith('HAB')
-    
-    @property
-    def npexp_path(self) -> pathlib.Path:
-        """np-exp root / folder (may not exist)"""
-        return NPEXP_ROOT / 'habituation' / self.folder if self.is_hab else NPEXP_ROOT / self.folder
-    
-    @property
-    def lims_path(self) -> pathlib.Path | None:
-        """Corresponding directory in lims, if one can be found"""
-        if not hasattr(self, "_lims_path"):
-            path: str = self.lims.get("storage_directory", "")
-            if not path:
-                logger.debug(
-                    "lims checked successfully, but no folder uploaded for %s", self.id
-                )
-                self._lims_path = None
-            else:
-                self._lims_path = pathlib.Path("/" + path)
-        return self._lims_path
-
-    @property
-    def z_path(self) -> pathlib.Path:
-        "Path in Sync neuropixels_data (aka Z:) (may not exist))"
-        return (
-            np_config.local_to_unc(self.rig.sync, NEUROPIXELS_DATA_RELATIVE_PATH)
-            / self.folder
-        )
-
-    @property
-    def qc_path(self) -> pathlib.Path:
-        "Expected default path, or alternative if one exists - see `qc_paths` for all available"
-        return self.qc_paths[0] if self.qc_paths else QC_PATHS[0] / self.folder
-
-    @cached_property
-    def qc_paths(self) -> list[pathlib.Path]:
-        "Any QC folders that exist"
-        return [
-            path / self.folder for path in QC_PATHS if (path / self.folder).exists()
-        ]
-
-    @property
-    def project(self) -> Project | None:
-        if not hasattr(self, "_project"):
-            lims_project_name = self.lims.get("project", {}).get("code", "")
-            if lims_project_name:
-                self._project = Project(lims_project_name)
-            else:
-                self._project = None
-        return self._project
-
-    @cached_property
-    def lims_data_getter(self) -> dg.data_getter | None:
-        try:
-            return dg.lims_data_getter(self.id)
-        except ConnectionError:
-            logger.debug("Connection to lims failed", exc_info=True)
-            return None
-        except:
-            raise
-
-    @property
-    def data_dict(self) -> dict:
-        if not hasattr(self, "_data_dict"):
-            data_getter = self.lims_data_getter
-            if not data_getter:
-                self._data_dict = {}
-            else:
-                self._data_dict_orig = data_getter.data_dict  # str paths
-                self._data_dict = data_getter.data_dict_pathlib  # pathlib paths
-        return self._data_dict
-
-    @property
-    def mtrain(self) -> mtrain.MTrain | dict:
-        """Info from MTrain on the last behavior session for the mouse on the experiment day"""
-        if not hasattr(self, "_mtrain"):
-            if not is_connected("mtrain"):
-                return {}
-            try:
-                _ = self.mouse.mtrain
-            except mtrain.MouseNotInMTrainError:
-                self._mtrain = {}
-            except:
-                raise
-            else:
-                self._mtrain = self.mouse.mtrain.last_behavior_session_on(self.date)
-        return self._mtrain
-
-    @property
-    def foraging_id(self) -> str | None:
-        "From lims, mtrain, or platform json, in that order."
-        if not hasattr(self, "_foraging_id"):
-            self._foraging_id = self.foraging_id_lims or self.foraging_id_mtrain or (
-                self.platform_json.foraging_id if self.platform_json.file_sync else None
-                )
-        return self._foraging_id
-    
-    @foraging_id.setter
-    def foraging_id(self, value: str) -> None:
-        self.platform_json.foraging_id = value # validates uuid
-        self._foraging_id = value
-        
-    @cached_property
-    def foraging_id_mtrain(self) -> str | None:
-        """Foraging ID from MTrain (if an MTrain session is found)."""
-        return self.mtrain.get("id", None)
-    
-    @cached_property
-    def foraging_id_lims(self) -> str | None:
-        """Foraging ID from lims based on start/stop time of experiment and mouse ID
-        (from platform json), obtained from the behavior session that ran at the time. 
-        
-        Not all mice have foraging IDs (e.g. variability project)"""
-        try:
-            from_lims = dg.get_foraging_id_from_behavior_session(
-                self.mouse.id,
-                self.experiment_start,
-                self.experiment_end,
-            )
-        except (dg.MultipleBehaviorSessionsError, dg.NoBehaviorSessionError):
-            return None
-        else:
-            return from_lims
-    
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        try:
-            return State(self.id)
-        except Exception as exc:
-            logger.error("Failed to load `%r.state`: %r", self, exc)
-        return {}
-    
-    def find_platform_json(self) -> pathlib.Path | None:
-        """Find the platform.json file for this session, if it exists."""
-        path = (
-            self.data_dict.get('EcephysPlatformFile') 
-            or next(self.npexp_path.glob('*platformD1*.json'), None)
-            )
-        if path and 'platformD1' in path.name:
-            return np_config.normalize_path(path)
-        
-    def find_settings_xml(self) -> pathlib.Path | None:
-        """Find one of the settings.xml files for this session.
-        
-        Files associated with probes ABC and DEF are identical, so return either.
-        """
-        path = (
-            self.data_dict.get('EcephysProbeRawDataABC_settings') 
-            or self.data_dict.get('EcephysProbeRawDataDEF_settings')
-        )
-        if (not path or path.suffix != '.xml') and self.npexp_path.exists():
-            path = next(self.npexp_path.glob('*_probe???/settings*.xml'), None)
-        return np_config.normalize_path(path) if path else None
-    
-    @property
-    def D0(self) -> Manifest:
-        """D0 upload manifest for platform json, plus extra methods for finding missing files."""
-        with contextlib.suppress(AttributeError):
-            return self._D0
-        self._D0 = Manifest(self, 'D0')
-        return self.D0
-    
-    @property
-    def D1(self) -> Manifest:
-        """D1 upload manifest for platform json, plus extra methods for finding missing files."""
-        with contextlib.suppress(AttributeError):
-            return self._D1
-        self._D1 = Manifest(self, 'D1')
-        return self.D1
-    
-    @property
-    def D2(self) -> Manifest:
-        """D2 upload manifest for platform json, plus extra methods for finding missing files."""
-        with contextlib.suppress(AttributeError):
-            return self._D2
-        self._D2 = Manifest(self, 'D2')
-        return self.D2
-    
-    def get_missing_files(self) -> tuple[str, ...]:
-        """Globs for D1 & D2 files that are missing from npexp"""
-        missing_globs = [self.D1.globs[self.D1.names.index(_)] for _ in self.D1.missing]
-        missing_globs.extend(self.D2.globs[self.D2.names.index(_)] for _ in self.D2.missing)
-        missing_globs.extend(self.D2.globs_sorted_data[self.D2.names_sorted_data.index(_)] for _ in self.D2.missing_sorted_data
-                             if not any(f'probe_{_[-1]}' in __ for __ in self.D2.missing)
-                             ) # don't add each individual missing sorted file if we already added their parent probeX_sorted folder
-        return tuple(dict.fromkeys(missing_globs))
-    
-    @cached_property
-    def metrics_csv(self) -> tuple[pathlib.Path, ...]:
-        probe_letters = self.data_dict.get('data_probes')
-        probe_paths = [self.data_dict.get(f'probe{letter}') for letter in probe_letters]
-        if any(probe_paths):
-            csv_paths = [_ / 'metrics.csv' for _ in probe_paths if _ and (_/ 'metrics.csv').exists()]
-            if csv_paths:
-                return tuple(csv_paths)
-        if self.npexp_path.exists():
-            return tuple(self.npexp_path.glob('*/*/*/metrics.csv'))
-    
-    @cached_property
-    def probe_letter_to_metrics_csv_path(self) -> dict[str, pathlib.Path]:
-        csv_paths = self.metrics_csv
-        if not csv_paths:
-            return {}
-        letter = lambda x: re.findall('(?<=_probe)[A-F]', str(x))
-        probe_letters = [_[-1] for _ in map(letter, csv_paths) if _]
-        if probe_letters:
-            return dict(zip(probe_letters, csv_paths))
-        return {}
-    
-    @property
-    def platform_json(self) -> PlatformJson:
-        """Platform D1 json on npexp."""
-        with contextlib.suppress(AttributeError):
-            self._platform_json.load_from_existing()
-            return self._platform_json
-        self._platform_json = PlatformJson(self.npexp_path)
-        update_from_session(self._platform_json, self)
-        return self._platform_json
-    
-    def fix_platform_json(self, path_or_obj: Optional[pathlib.Path | PlatformJson] = None):
-        if not path_or_obj:
-            path_or_obj = self.platform_json
-        if isinstance(path_or_obj, pathlib.Path):
-            path_or_obj = PlatformJson(path_or_obj)
-        pj = path_or_obj
-        # TODO get files dict, fetch files
-    
-    @cached_property
-    def experiment_start(self) -> datetime.datetime:
-        """Start time estimated from platform.json, for finding files created during
-        experiment. Not relevant for D2 files.
-        
-        In the event that the platform.json file does not contain a time, we use the start
-        of the day of the session.       
-        """
-        if self.platform_json.file_sync:
-            fields_to_try = ('ExperimentStartTime', 'ProbeInsertionStartTime', 'CartridgeLowerTime', 'HeadFrameEntryTime', 'workflow_start_time',)
-            for _ in fields_to_try:
-                time = getattr(self.platform_json, _)
-                if isinstance(time, datetime.datetime):
-                    return time
-            logger.debug('Could not find experiment start time in %s: using start of day instead', self.platform_json)
-        return datetime.datetime(*self.date.timetuple()[:5])
-    
-    @cached_property
-    def experiment_end(self) -> datetime.datetime:
-        """End time estimated from platform.json, for finding files created during
-        experiment. Not relevant for D2 files.
-        
-        In the event that the platform.json file does not contain a time, we use the end
-        of the day of the session.       
-        """
-        if self.platform_json.file_sync:
-            fields_to_try = ('workflow_complete_time', 'ExperimentCompleteTime', 'HeadFrameExitTime',)
-            for _ in fields_to_try:
-                time = getattr(self.platform_json, _)
-                if isinstance(time, datetime.datetime):
-                    return time
-            logger.debug('Could not find experiment end time in %s: using end of day instead', self.platform_json)
-        return datetime.datetime(*self.date.timetuple()[:5]) + datetime.timedelta(days=1) - datetime.timedelta(seconds=1)
-    
-    @property
-    def probes_inserted(self) -> tuple[Literal['A', 'B', 'C', 'D', 'E', 'F'], ...]:
-        probes = 'ABCDEF'
-        notes: dict = self.platform_json.InsertionNotes
-        # assume that no notes means probe was inserted
-        return tuple(_ for _ in probes if (f'Probe{_}' not in notes) or (notes[f'Probe{_}'].get('FailedToInsert') == 0))
-        
-    @probes_inserted.setter
-    def probes_inserted(self, inserted: str | Iterable[Literal['A', 'B', 'C', 'D', 'E', 'F']]):
-        probes = 'ABCDEF'
-        inserted = "".join(_.upper() for _ in inserted)
-        if not all(_ in probes for _ in inserted):
-            raise ValueError(f"Probes must be a sequence of letters A-F, got {inserted}")
-        notes = copy.deepcopy(self.platform_json.InsertionNotes)
-        for _ in probes:
-            probe = f'Probe{_}'
-            if probe in notes and _ in inserted:
-                notes[probe]['FailedToInsert'] = 0
-            if probe not in notes and _ not in inserted:
-                notes[probe] = {'FailedToInsert': 1}
-        self.platform_json.InsertionNotes = notes
-        logger.debug('Updated %s InsertionNotes: %s', self.platform_json, self.platform_json.InsertionNotes)
-        
-    @cached_property
-    def probe_letter_to_serial_number_from_probe_info(self) -> dict[str, int | None]:
-        """Probe letter to serial number, if they can be found from `probe_info.json`.
-        
-        Not a tuple because we might not find a serial number for all probes.
-        """
-        probe_letters: list[str] = self.data_dict.get('data_probes')
-        probe_info = [self.data_dict.get(f'probe{letter}_info') for letter in probe_letters]
-        if not any(probe_info):
-            return {}
-        mapping = dict().fromkeys(probe_letters, None)
-        for letter, info in zip(probe_letters, probe_info):
-            result = json.loads(pathlib.Path(info).read_bytes()).get('probe', {}).get('serial number')
-            mapping[letter] = int(result) if result else None
-            
-def generate_session(
-    mouse: str | int | Mouse,
-    user: str | User,
-    session_type: Literal["ephys", "hab", "behavior"] = "ephys",
-) -> Session:
-    if not isinstance(mouse, Mouse):
-        mouse = Mouse(mouse)
-    if not isinstance(user, User):
-        user = User(user)
-    if "ephys" in session_type: # maintain backwards compatibility with 'ecephys'
-        lims_session = lims.generate_ephys_session(mouse=mouse.lims, user=user.lims)
-    elif session_type == "hab":
-        lims_session = lims.generate_hab_session(mouse=mouse.lims, user=user.lims)
-    elif session_type == "behavior":
-        raise ValueError("Generating behavior sessions is not yet supported")
-    session = Session(lims_session)
-    # assign instances with data already fetched from lims:
-    session._mouse = mouse
-    session._user = user
-    return session
-
-
-def sessions(
-    project: Optional[str | Projects] = None,
-    root: str | pathlib.Path = NPEXP_ROOT,
-    session_type: Literal["ephys", "hab", "behavior"] = "ephys",
-) -> Generator[Session, None, None]:
-    """Find Session folders in a directory.
-
-    - `project` is the acronym used by the NP-ops team for the umbrella project:
-        'DR', 'GLO', 'VAR', 'ILLUSION', 'TTN'
-    - a `Projects` enum can also be used directly
-    """
-    root = pathlib.Path(root)
-    
-    if isinstance(project, str):
-        project = getattr(Projects, project)
-
-    for path in root.iterdir():
-        if not path.is_dir():
-            continue
-        try:
-            session = Session(path)
-        except (SessionError, FilepathIsDirError):
-            continue
-        
-        if (
-            (session_type == "behavior") and (session.is_ecephys_session in (True, None) or session.is_hab)
-        ): # watch out: is_ecephys_session is None if unsure. assumed to be ecephys here
-            continue
-        
-        if (
-            (session_type != "hab") and (session.is_hab)
-        ): # watch out: is_hab is None if unsure
-            continue
-
-        if project and session.project not in project.value:
-            continue
-
-        if session.is_ecephys_session is None:
-            logger.debug("Unsure if %s is an ecephys or behavior session on lims, but it's included in results", session)
-        if session.is_hab is None:
-            logger.debug("Unsure if %s is a hab or ephys session, but it's included in results", session)
-            
-        yield session
-
-def cleanup_npexp():
-    """Remove empty dirs, 366122 dirs, move habs"""
-    def remove_non_empty_dir(path: pathlib.Path):
-        shutil.rmtree(path, ignore_errors=True)
-        if not path.exists():
-            logger.info("Removed %s", path.name)
-        
-    for _ in itertools.chain(NPEXP_ROOT.iterdir(), (NPEXP_ROOT / "habituation").iterdir()):
-        if not _.is_dir():
-            continue
-        with contextlib.suppress(Exception):
-            _.rmdir()
-            logger.info("Removed empty dir %s", _.name)
-            continue
-        if '_366122_' in _.name:
-            remove_non_empty_dir(_)
-            continue
-        contents = tuple(_.iterdir())
-        if len(contents) == 1 and contents[0].suffix == ".json" and "platform" in contents[0].name:
-            remove_non_empty_dir(_)
-            continue
-        try:
-            session = Session(_)
-        except SessionError:
-            continue
-        if session.is_hab and _.parent == NPEXP_ROOT:
-            try:
-                _.replace(NPEXP_ROOT / "habituation" / "backup" / _.name)
-            except OSError as exc:
-                logger.error("Moving hab failed: %r", exc)
-            else:
-                logger.info("Moved %s to habituation/backup", _.name)
-                
-                
-def latest_session(
-        project: str | Project | Projects,
-        session_type: Literal["ephys", "hab", "behavior"] = "ephys"
-    ) -> Session | None:
-    
-    if isinstance(project, str):
-        if project.upper() in Projects.__members__:
-            project = Projects[project.upper()]
-            
-    session: int | None = None
-    if isinstance(project, Projects):
-        session = project.get_latest_session(session_type)
-    if isinstance(project, Project):
-        session = project.state.get(f'latest_{session_type}')
-    if session is None:
-        logger.info("No latest session found for %s", project)
-        return None
-    
-    return Session(session)
-
-if __name__ == "__main__":
-    np_logging.getLogger()
-    cleanup_npexp()
-    if is_connected("lims2"):
-        doctest.testmod(verbose=True)
-        # optionflags=(doctest.ELLIPSIS, doctest.NORMALIZE_WHITESPACE,
-        # doctest.IGNORE_EXCEPTION_DETAIL)
-    else:
-        print("LIMS not connected - skipping doctests")
+from __future__ import annotations
+
+import contextlib
+import copy
+import datetime
+import doctest
+import pathlib
+from typing import Iterable, Optional
+
+import np_config
+import np_logging
+from backports.cached_property import cached_property
+from typing_extensions import Literal
+
+from np_session.components.info import Project, User
+from np_session.components.lims_manifests import Manifest
+from np_session.components.paths import *
+from np_session.components.platform_json import *
+from np_session.databases import data_getters as dg
+from np_session.databases import lims2 as lims
+from np_session.databases import mtrain
+from np_session.utils import *
+from np_session.session import Session
+
+logger = np_logging.getLogger(__name__)
+
+
+class PipelineSession(Session):
+    """Session information from any string or PathLike containing a session ID.
+
+    Note: lims/mtrain properties may be empty or None if mouse/session isn't in db.
+    Note: `is_ecephys` checks ecephys vs behavior: habs are ecephys sessions, as in lims.
+
+    Quick access to useful properties:
+    >>> session = PipelineSession('c:/1116941914_surface-image1-left.png')
+    >>> session.lims.id
+    1116941914
+    >>> session.folder
+    '1116941914_576323_20210721'
+    >>> session.project.lims.id
+    714916854
+    >>> session.is_hab
+    False
+    >>> session.rig.acq # hostnames reflect the computers used during the session, not necessarily the current machines
+    'W10DT05515'
+
+    Some properties are returned as objects with richer information:
+    - `pathlib` objects for filesystem paths:
+    >>> session.lims_path.as_posix()
+    '//allen/programs/braintv/production/visualbehavior/prod0/specimen_1098595957/ecephys_session_1116941914'
+    >>> session.data_dict['storage_directory'].as_posix()
+    '//allen/programs/braintv/production/visualbehavior/prod0/specimen_1098595957/ecephys_session_1116941914'
+
+
+    - `datetime` objects for easy date manipulation:
+    >>> session.date
+    datetime.date(2021, 7, 21)
+
+    - dictionaries from lims (loaded lazily):
+    >>> session.mouse
+    Mouse(576323)
+    >>> session.mouse.lims
+    LIMS2MouseInfo(576323)
+    >>> session.mouse.lims.id
+    1098595957
+    >>> session.mouse.lims['full_genotype']
+    'wt/wt'
+
+    ...with a useful string representation:
+    >>> str(session.mouse)
+    '576323'
+    >>> str(session.project)
+    'NeuropixelVisualBehavior'
+    >>> str(session.rig)        # see np_config.Rig
+    'NP.0'
+    """
+
+    @staticmethod
+    def get_folder(value: int | str | PathLike) -> str | None:
+        return get_lims_session_folder(value)
+
+    @property
+    def folder(self) -> str:
+        """Folder name, e.g. `[lims session ID]_[labtracks ID]_[8-digit date]`."""
+        return self._folder
+
+    @folder.setter
+    def folder(self, value: str | PathLike) -> None:
+        folder = self.get_folder(value)
+        if folder is None:
+            raise ValueError(
+                f'Session folder must be in the format `[lims session ID]_[6-digit mouse ID]_[8-digit date str]`: {value}'
+            )
+        self._folder = folder
+
+    @property
+    def id(self) -> int:
+        """LIMS session ID (ephys for ecephys/hab, behavior for behavior)"""
+        return int(self.folder.split('_')[0])
+
+    @property
+    def lims(self) -> lims.LIMS2SessionInfo | dict:
+        """
+        >>> info = Session(1116941914).lims
+        >>> info['stimulus_name']
+        'EPHYS_1_images_H_3uL_reward'
+        >>> info['operator']['login']
+        'taminar'
+
+        >>> Session(1116941914).lims
+        LIMS2SessionInfo(1116941914)
+        >>> str(Session(1116941914).lims)
+        '1116941914'
+        """
+        if not hasattr(self, '_lims'):
+            try:
+                self._lims = lims.LIMS2SessionInfo(self.id)
+            except ValueError:
+                self._lims = {}
+        return self._lims
+
+    @lims.setter
+    def lims(self, value: lims.LIMS2SessionInfo):
+        if not isinstance(value, lims.LIMS2SessionInfo):
+            raise TypeError(
+                f'Expected `lims` to be an instance of `lims.LIMS2SessionInfo`, not {type(value)}'
+            )
+        self._lims = value
+
+    @property
+    def user(self) -> User | None:
+        if not hasattr(self, '_user'):
+            lims_user_id = self.lims.get('operator', {}).get('login', '')
+            if lims_user_id:
+                self._user = User(lims_user_id)
+            else:
+                self._user = None
+        return self._user
+
+    @property
+    def rig(self) -> np_config.Rig | None:
+        """Rig object with computer info and paths, can also be used as a string."""
+        if not hasattr(self, '_rig'):
+            self._rig = None
+            while not self.rig:
+                # try from current rig first
+                with contextlib.suppress(ValueError):
+                    self.rig = np_config.Rig()
+                    continue
+
+                # try from platform json
+                with contextlib.suppress(Exception):
+                    self.rig = np_config.Rig(self.platform_json.rig_id)
+                # try from lims
+                rig_id: str | None = self.data_dict.get('rig')
+                if rig_id:
+                    self.rig = np_config.Rig(rig_id)
+                    continue
+
+                break
+        return self._rig
+
+    @rig.setter
+    def rig(self, value: np_config.Rig) -> None:
+        if not isinstance(value, np_config.Rig):
+            raise TypeError(
+                f'Expected `rig` to be an instance of `np_config.Rig`, not {type(value)}'
+            )
+        self._rig = value
+        self.update_hostnames_for_replaced_computers()
+
+    def update_hostnames_for_replaced_computers(self) -> None:
+        if not self._rig:
+            return
+        for comp in ('sync', 'stim', 'mon', 'acq'):
+            replaced = old_hostname(
+                f'{self._rig.id}-{comp.capitalize()}', self.date
+            )
+            if replaced:
+                setattr(self._rig, f'_{comp}', replaced)
+
+    @property
+    def is_ecephys(self) -> bool | None:
+        """False if behavior session in lims, None if unsure.
+
+        Note that habs are classed as ecephys sessions: use `is_hab`.
+        """
+        if not self.lims or not self.lims.get('ecephys_session'):
+            return None
+        return 'ecephys_session' in self.lims['ecephys_session']
+
+    is_ecephys_session = is_ecephys   # for backwards compatibility
+
+    @property
+    def is_hab(self) -> bool | None:
+        """False if hab session, None if unsure."""
+        if not self.lims:
+            return None
+        return self.lims.get('name', '').startswith('HAB')
+
+    @property
+    def npexp_path(self) -> pathlib.Path:
+        """np-exp root / folder (may not exist)"""
+        return (
+            NPEXP_ROOT / 'habituation' / self.folder
+            if self.is_hab
+            else NPEXP_ROOT / self.folder
+        )
+
+    @property
+    def lims_path(self) -> pathlib.Path | None:
+        """Corresponding directory in lims, if one can be found"""
+        if not hasattr(self, '_lims_path'):
+            path: str = self.lims.get('storage_directory', '')
+            if not path:
+                logger.debug(
+                    'lims checked successfully, but no folder uploaded for %s',
+                    self.id,
+                )
+                self._lims_path = None
+            else:
+                self._lims_path = pathlib.Path('/' + path)
+        return self._lims_path
+
+    @property
+    def z_path(self) -> pathlib.Path:
+        """Path in Sync neuropixels_data (aka Z:) (may not exist))"""
+        return (
+            np_config.local_to_unc(
+                self.rig.sync, NEUROPIXELS_DATA_RELATIVE_PATH
+            )
+            / self.folder
+        )
+
+    @property
+    def qc_path(self) -> pathlib.Path:
+        """Expected default path, or alternative if one exists - see `qc_paths` for all available"""
+        return self.qc_paths[0] if self.qc_paths else QC_PATHS[0] / self.folder
+
+    @cached_property
+    def qc_paths(self) -> list[pathlib.Path]:
+        """Any QC folders that exist"""
+        return [
+            path / self.folder
+            for path in QC_PATHS
+            if (path / self.folder).exists()
+        ]
+
+    @property
+    def project(self) -> Project | None:
+        if not hasattr(self, '_project'):
+            lims_project_name = self.lims.get('project', {}).get('code', '')
+            if lims_project_name:
+                self._project = Project(lims_project_name)
+            else:
+                self._project = None
+        return self._project
+
+    @cached_property
+    def lims_data_getter(self) -> dg.data_getter | None:
+        try:
+            return dg.lims_data_getter(self.id)
+        except ConnectionError:
+            logger.debug('Connection to lims failed', exc_info=True)
+            return None
+        except:
+            raise
+
+    @property
+    def data_dict(self) -> dict:
+        if not hasattr(self, '_data_dict'):
+            data_getter = self.lims_data_getter
+            if not data_getter:
+                self._data_dict = {}
+            else:
+                self._data_dict_orig = data_getter.data_dict  # str paths
+                self._data_dict = (
+                    data_getter.data_dict_pathlib
+                )  # pathlib paths
+        return self._data_dict
+
+    @property
+    def mtrain(self) -> mtrain.MTrain | dict:
+        """Info from MTrain on the last behavior session for the mouse on the experiment day"""
+        if not hasattr(self, '_mtrain'):
+            if not is_connected('mtrain'):
+                return {}
+            try:
+                _ = self.mouse.mtrain
+            except mtrain.MouseNotInMTrainError:
+                self._mtrain = {}
+            except:
+                raise
+            else:
+                self._mtrain = self.mouse.mtrain.last_behavior_session_on(
+                    self.date
+                )
+        return self._mtrain
+
+    @property
+    def foraging_id(self) -> str | None:
+        """From lims, mtrain, or platform json, in that order."""
+        if not hasattr(self, '_foraging_id'):
+            self._foraging_id = (
+                self.foraging_id_lims
+                or self.foraging_id_mtrain
+                or (
+                    self.platform_json.foraging_id
+                    if self.platform_json.file_sync
+                    else None
+                )
+            )
+        return self._foraging_id
+
+    @foraging_id.setter
+    def foraging_id(self, value: str) -> None:
+        self.platform_json.foraging_id = value   # validates uuid
+        self._foraging_id = value
+
+    @cached_property
+    def foraging_id_mtrain(self) -> str | None:
+        """Foraging ID from MTrain (if an MTrain session is found)."""
+        return self.mtrain.get('id', None)
+
+    @cached_property
+    def foraging_id_lims(self) -> str | None:
+        """Foraging ID from lims based on start/stop time of experiment and mouse ID
+        (from platform json), obtained from the behavior session that ran at the time.
+
+        Not all mice have foraging IDs (e.g. variability project)"""
+        try:
+            from_lims = dg.get_foraging_id_from_behavior_session(
+                self.mouse.id,
+                self.start,
+                self.end,
+            )
+        except (dg.MultipleBehaviorSessionsError, dg.NoBehaviorSessionError):
+            return None
+        else:
+            return from_lims
+
+    def find_platform_json(self) -> pathlib.Path | None:
+        """Find the platform.json file for this session, if it exists."""
+        path = self.data_dict.get('EcephysPlatformFile') or next(
+            self.npexp_path.glob('*platformD1*.json'), None
+        )
+        if path and 'platformD1' in path.name:
+            return np_config.normalize_path(path)
+
+    def find_settings_xml(self) -> pathlib.Path | None:
+        """Find one of the settings.xml files for this session.
+
+        Files associated with probes ABC and DEF are identical, so return either.
+        """
+        path = self.data_dict.get(
+            'EcephysProbeRawDataABC_settings'
+        ) or self.data_dict.get('EcephysProbeRawDataDEF_settings')
+        if (not path or path.suffix != '.xml') and self.npexp_path.exists():
+            path = next(self.npexp_path.glob('*_probe???/settings*.xml'), None)
+        return np_config.normalize_path(path) if path else None
+
+    @property
+    def D0(self) -> Manifest:
+        """D0 upload manifest for platform json, plus extra methods for finding missing files."""
+        with contextlib.suppress(AttributeError):
+            return self._D0
+        self._D0 = Manifest(self, 'D0')
+        return self.D0
+
+    @property
+    def D1(self) -> Manifest:
+        """D1 upload manifest for platform json, plus extra methods for finding missing files."""
+        with contextlib.suppress(AttributeError):
+            return self._D1
+        self._D1 = Manifest(self, 'D1')
+        return self.D1
+
+    @property
+    def D2(self) -> Manifest:
+        """D2 upload manifest for platform json, plus extra methods for finding missing files."""
+        with contextlib.suppress(AttributeError):
+            return self._D2
+        self._D2 = Manifest(self, 'D2')
+        return self.D2
+
+    def get_missing_files(self) -> tuple[str, ...]:
+        """Globs for D1 & D2 files that are missing from npexp"""
+        missing_globs = [
+            self.D1.globs[self.D1.names.index(_)] for _ in self.D1.missing
+        ]
+        missing_globs.extend(
+            self.D2.globs[self.D2.names.index(_)] for _ in self.D2.missing
+        )
+        missing_globs.extend(
+            self.D2.globs_sorted_data[self.D2.names_sorted_data.index(_)]
+            for _ in self.D2.missing_sorted_data
+            if not any(f'probe_{_[-1]}' in __ for __ in self.D2.missing)
+        )   # don't add each individual missing sorted file if we already added their parent probeX_sorted folder
+        return tuple(dict.fromkeys(missing_globs))
+
+    @cached_property
+    def metrics_csv(self) -> tuple[pathlib.Path, ...]:
+        probe_letters = self.data_dict.get('data_probes')
+        probe_paths = [
+            self.data_dict.get(f'probe{letter}') for letter in probe_letters
+        ]
+        if any(probe_paths):
+            csv_paths = [
+                _ / 'metrics.csv'
+                for _ in probe_paths
+                if _ and (_ / 'metrics.csv').exists()
+            ]
+            if csv_paths:
+                return tuple(csv_paths)
+        if self.npexp_path.exists():
+            return tuple(self.npexp_path.glob('*/*/*/metrics.csv'))
+
+    @cached_property
+    def probe_letter_to_metrics_csv_path(self) -> dict[str, pathlib.Path]:
+        csv_paths = self.metrics_csv
+        if not csv_paths:
+            return {}
+
+        def letter(x):
+            return re.findall('(?<=_probe)[A-F]', str(x))
+
+        probe_letters = [_[-1] for _ in map(letter, csv_paths) if _]
+        if probe_letters:
+            return dict(zip(probe_letters, csv_paths))
+        return {}
+
+    @property
+    def platform_json(self) -> PlatformJson:
+        """Platform D1 json on npexp."""
+        with contextlib.suppress(AttributeError):
+            self._platform_json.load_from_existing()
+            return self._platform_json
+        self._platform_json = PlatformJson(self.npexp_path)
+        update_from_session(self._platform_json, self)
+        return self._platform_json
+
+    def fix_platform_json(
+        self, path_or_obj: Optional[pathlib.Path | PlatformJson] = None
+    ):
+        if not path_or_obj:
+            path_or_obj = self.platform_json
+        if isinstance(path_or_obj, pathlib.Path):
+            path_or_obj = PlatformJson(path_or_obj)
+        # TODO get files dict, fetch files
+
+    @cached_property
+    def start(self) -> datetime.datetime:
+        """Start time estimated from platform.json, for finding files created during
+        experiment. Not relevant for D2 files.
+
+        In the event that the platform.json file does not contain a time, we use the start
+        of the day of the session.
+        """
+        if self.platform_json.file_sync:
+            fields_to_try = (
+                'ExperimentStartTime',
+                'ProbeInsertionStartTime',
+                'CartridgeLowerTime',
+                'HeadFrameEntryTime',
+                'workflow_start_time',
+            )
+            for _ in fields_to_try:
+                time = getattr(self.platform_json, _)
+                if isinstance(time, datetime.datetime):
+                    return time
+            logger.debug(
+                'Could not find experiment start time in %s: using start of day instead',
+                self.platform_json,
+            )
+        return super().start
+
+    @cached_property
+    def end(self) -> datetime.datetime:
+        """End time estimated from platform.json, for finding files created during
+        experiment. Not relevant for D2 files.
+
+        In the event that the platform.json file does not contain a time, we use the end
+        of the day of the session.
+        """
+        if self.platform_json.file_sync:
+            fields_to_try = (
+                'workflow_complete_time',
+                'ExperimentCompleteTime',
+                'HeadFrameExitTime',
+            )
+            for _ in fields_to_try:
+                time = getattr(self.platform_json, _)
+                if isinstance(time, datetime.datetime):
+                    return time
+            logger.debug(
+                'Could not find experiment end time in %s: using end of day instead',
+                self.platform_json,
+            )
+        return super().end
+
+    @property
+    def experiment_start(self):
+        """For backwards compatibility with old code.
+        Replace with `self.start`.
+        """
+        return self.start()
+
+    @property
+    def experiment_end(self):
+        """For backwards compatibility with old code.
+        Replace with `self.end`.
+        """
+        return self.end()
+
+    @property
+    def probes_inserted(
+        self,
+    ) -> Optional[tuple[Literal['A', 'B', 'C', 'D', 'E', 'F'], ...]]:
+        probes = 'ABCDEF'
+        notes: dict = self.platform_json.InsertionNotes
+        # assume that no notes means probe was inserted
+        return tuple(
+            _
+            for _ in probes
+            if (f'Probe{_}' not in notes)
+            or (notes[f'Probe{_}'].get('FailedToInsert') == 0)
+        )
+
+    @probes_inserted.setter
+    def probes_inserted(
+        self, inserted: str | Iterable[Literal['A', 'B', 'C', 'D', 'E', 'F']]
+    ):
+        probes = 'ABCDEF'
+        inserted = ''.join(_.upper() for _ in inserted)
+        if not all(_ in probes for _ in inserted):
+            raise ValueError(
+                f'Probes must be a sequence of letters A-F, got {inserted}'
+            )
+        notes = copy.deepcopy(self.platform_json.InsertionNotes)
+        for _ in probes:
+            probe = f'Probe{_}'
+            if probe in notes and _ in inserted:
+                notes[probe]['FailedToInsert'] = 0
+            if probe not in notes and _ not in inserted:
+                notes[probe] = {'FailedToInsert': 1}
+        self.platform_json.InsertionNotes = notes
+        logger.debug(
+            'Updated %s InsertionNotes: %s',
+            self.platform_json,
+            self.platform_json.InsertionNotes,
+        )
+
+    @cached_property
+    def probe_letter_to_serial_number_from_probe_info(
+        self,
+    ) -> dict[str, int | None]:
+        """Probe letter to serial number, if they can be found from `probe_info.json`.
+
+        Not a tuple because we might not find a serial number for all probes.
+        """
+        probe_letters: list[str] = self.data_dict.get('data_probes')
+        probe_info = [
+            self.data_dict.get(f'probe{letter}_info')
+            for letter in probe_letters
+        ]
+        if not any(probe_info):
+            return {}
+        mapping = dict().fromkeys(probe_letters, None)
+        for letter, info in zip(probe_letters, probe_info):
+            result = (
+                json.loads(pathlib.Path(info).read_bytes())
+                .get('probe', {})
+                .get('serial number')
+            )
+            mapping[letter] = int(result) if result else None
+
+
+if __name__ == '__main__':
+    if is_connected('lims2'):
+        doctest.testmod(verbose=True)
+        optionflags = (
+            doctest.ELLIPSIS,
+            doctest.NORMALIZE_WHITESPACE,
+            doctest.IGNORE_EXCEPTION_DETAIL,
+        )
+    else:
+        print('LIMS not connected - skipping doctests')
```

### Comparing `np-session-0.5.4/src/np_session/utils.py` & `np-session-0.6.0/src/np_session/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,42 +13,39 @@
 import os
 import pathlib
 import re
 import subprocess
 import sys
 from typing import Union
 
-from typing_extensions import Literal
-from backports.cached_property import cached_property
-
 import np_logging
 import requests
+from typing_extensions import Literal
 
 import np_session.components.paths as paths
-from np_session.databases.data_getters import lims_data_getter
 from np_session.databases.lims2 import LIMS2SessionInfo
 
 logger = np_logging.getLogger(__name__)
 
 PathLike = Union[str, bytes, os.PathLike, pathlib.Path]
 # https://peps.python.org/pep-0519/#provide-specific-type-hinting-support
 # PathLike inputs are converted to pathlib.Path objects for os-agnostic filesystem operations
 # os.fsdecode(path: PathLike) is used where only a string is required
 
-RE_SESSION_ID = re.compile("[0-9]{8,}")
-RE_FOLDER = re.compile("[0-9]{8,}_[0-9]{6}_[0-9]{8}")
-RE_PROBES = re.compile("(?<=_probe)_?(([A-F]+)|([0-5]))")
+RE_SESSION_ID = re.compile('[0-9]{8,}')
+RE_FOLDER = re.compile('[0-9]{8,}_[0-9]{6}_[0-9]{8}')
+RE_PROBES = re.compile('(?<=_probe)_?(([A-F]+)|([0-5]))')
 
 REPLACED_COMP_ID: dict[str, tuple[datetime.date, str]] = {
-    "NP.0-Acq": (datetime.date(2022, 10, 18), "W10DT05515"),
-    "NP.1-Acq": (datetime.date(2022, 10, 27), "W10DT05501"),
-    "NP.2-Acq": (datetime.date(2022, 7, 14), "W10DT05517"),
-    "NP.0-Stim": (datetime.date(2023, 2, 7), "W10DTSM112721"),
-    "NP.1-Stim": (datetime.date(2023, 1, 19), "W10DTSM118294"),
-    "NP.2-Stim": (datetime.date(2023, 3, 15), "W10DTSM118295"),
+    'NP.0-Acq': (datetime.date(2022, 10, 18), 'W10DT05515'),
+    'NP.1-Acq': (datetime.date(2022, 10, 27), 'W10DT05501'),
+    'NP.2-Acq': (datetime.date(2022, 7, 14), 'W10DT05517'),
+    'NP.0-Stim': (datetime.date(2023, 2, 7), 'W10DTSM112721'),
+    'NP.1-Stim': (datetime.date(2023, 1, 19), 'W10DTSM118294'),
+    'NP.2-Stim': (datetime.date(2023, 3, 15), 'W10DTSM118295'),
 }
 
 
 def old_hostname(comp_id: str, date: datetime.date) -> str | None:
     """Return the hostname for a computer that was replaced, if `date` predates the switchover.
 
     For a date before the hostname changed:
@@ -63,36 +60,38 @@
     if replaced is None:
         return
     if date < replaced[0]:
         return replaced[1]
 
 
 class Host(enum.Enum):
-    LIMS = "lims2"
-    MTRAIN = "mtrain"
-    MINDSCOPE_SERVER = ZK = "eng-mindscope"
-    MPE_SERVER = "aibspi"
+    LIMS = 'lims2'
+    MTRAIN = 'mtrain'
+    MINDSCOPE_SERVER = ZK = 'eng-mindscope'
+    MPE_SERVER = 'aibspi'
 
 
 def is_connected(host: str | Host) -> bool:
-    "Use OS's `ping` cmd to check if `host` is connected."
-    command = ["ping", "-n" if "win" in sys.platform else "-c", "1", str(host)]
+    """Use OS's `ping` cmd to check if `host` is connected."""
+    command = ['ping', '-n' if 'win' in sys.platform else '-c', '1', str(host)]
     try:
-        return subprocess.call(command, stdout=subprocess.PIPE, timeout=0.1) == 0
+        return (
+            subprocess.call(command, stdout=subprocess.PIPE, timeout=0.1) == 0
+        )
     except subprocess.TimeoutExpired:
         return False
 
 
 def is_lims_path(path: PathLike) -> bool:
     """
     >>> is_lims_path('//allen/programs/mindscope/production/dynamicrouting/prod0/specimen_1200280254/ecephys_session_1234028213')
     True
     """
     parts = pathlib.Path(path).parts
-    return "production" in parts and "incoming" not in parts
+    return 'production' in parts and 'incoming' not in parts
 
 
 def is_valid_session_id(session_id: int | str) -> bool:
     """
     >>> is_valid_session_id('1234028213')
     True
     >>> is_valid_session_id('abcdefg')
@@ -100,47 +99,48 @@
     """
     try:
         _ = int(session_id)
     except ValueError:
         return False
     return bool(LIMS2SessionInfo(session_id))
 
+
 def lims_session_id(path: PathLike) -> str | None:
     """
     Get valid lims ecephys/behavior session id from str or path.
 
     >>> lims_session_id('//allen/programs/mindscope/production/dynamicrouting/prod0/specimen_1200280254/ecephys_session_1234028213')
     '1234028213'
     """
 
-    path = os.fsdecode(path)
+    path = str(path)
     if is_lims_path(path):
-        from_lims_path = re.search("(?<=_session_)\\d+", os.fsdecode(path))
+        from_lims_path = re.search('(?<=_session_)\\d+', os.fsdecode(path))
         if from_lims_path:
             return from_lims_path.group(0)
     for i in RE_SESSION_ID.findall(path):
         if is_valid_session_id(i):
             return i
 
 
-def folder(path: PathLike) -> str | None:
+def get_lims_session_folder(path: int | PathLike) -> str | None:
     """
     Extract [8+digit lims session ID]_[6-digit labtracks mouse ID]_[6-digit datestr] from a str or path.
 
-    >>> folder('//allen/programs/mindscope/workgroups/np-exp/1234028213_640887_20221219/image.png')
+    >>> get_lims_session_folder('//allen/programs/mindscope/workgroups/np-exp/1234028213_640887_20221219/image.png')
     '1234028213_640887_20221219'
     """
 
-    session_folders = RE_FOLDER.findall(os.fsdecode(path))
+    session_folders = RE_FOLDER.findall(str(path))
 
     if not session_folders:
         return folder_from_lims_id(path)
     if not all(s == session_folders[0] for s in session_folders):
         logger.warning(
-            f"Mismatch between session folder strings - file may be in the wrong folder: {path!r}"
+            f'Mismatch between session folder strings - file may be in the wrong folder: {path!r}'
         )
     return session_folders[0]
 
 
 def folder_from_lims_id(path: PathLike) -> str | None:
     """
     Get the session folder string ([lims-id]_[mouse-id]_[date]) from a string or path containing a possible lims id.
@@ -150,86 +150,71 @@
 
     >>> folder_from_lims_id('1234028213')
     '1234028213_640887_20221219'
     """
     session_id = lims_session_id(path)
     if session_id is None:
         return None
-    lims_data = lims_data_getter(session_id)
-    return ("_").join(
-        [
-            lims_data.lims_id,
-            lims_data.data_dict["external_specimen_name"],
-            lims_data.data_dict["datestring"],
-        ]
-    )
-
-
-def folder_from_lims_id(path: PathLike) -> str | None:
-    """
-    Get the session folder string ([lims-id]_[mouse-id]_[date]) from a string or path containing a possible lims id.
-
-    >>> folder_from_lims_id('//allen/programs/mindscope/production/dynamicrouting/prod0/specimen_1200280254/ecephys_session_1234028213')
-    '1234028213_640887_20221219'
-
-    >>> folder_from_lims_id('1234028213')
-    '1234028213_640887_20221219'
-    """
-    session_id = lims_session_id(path)
-    if session_id is None:
-        return None
     return LIMS2SessionInfo(session_id).folder
 
 
 @functools.lru_cache(maxsize=None)
 def lims_json_content(lims_id: int | str) -> dict | None:
     if not is_valid_session_id(lims_id):
-        raise ValueError(f"{lims_id} is not a valid lims session id")
-    if not is_connected("lims2"):
-        raise ConnectionError("Could not connect to lims")
-    for session_type in ["ecephys_sessions", "behavior_sessions"]:
-        response = requests.get(f"http://lims2/{session_type}/{lims_id}.json?")
+        raise ValueError(f'{lims_id} is not a valid lims session id')
+    if not is_connected('lims2'):
+        raise ConnectionError('Could not connect to lims')
+    for session_type in ['ecephys_sessions', 'behavior_sessions']:
+        response = requests.get(f'http://lims2/{session_type}/{lims_id}.json?')
         if response.status_code == 200:
             return response.json()
-    logger.warning(f"Could not find json content for lims session id {lims_id}")
+    logger.warning(
+        f'Could not find json content for lims session id {lims_id}'
+    )
     return None
 
 
 def is_new_ephys_folder(path: PathLike) -> bool:
-    "Contains subfolders with raw data from OpenEphys v0.6.0+ (format switched 2022 on NP.0,1,2)"
+    """Contains subfolders with raw data from OpenEphys v0.6.0+ (format switched 2022 on NP.0,1,2)"""
     path = pathlib.Path(path)
-    if path.match("_probe*"):
-        return path.match("Record Node*") or path.rglob("Record Node*")
-    return bool(list(path.glob("*_probe*/Record Node*")))
+    if path.match('_probe*'):
+        return path.match('Record Node*') or path.rglob('Record Node*')
+    return bool(list(path.glob('*_probe*/Record Node*')))
 
 
 def get_files_manifest(
     project_name: str,
-    session_str: str = "",
-    session_type: Literal["D0", "D1", "D2", "habituation"] = "D1",
+    session_str: str = '',
+    session_type: Literal['D0', 'D1', 'D2', 'habituation'] = 'D1',
 ) -> dict[Literal['files'], dict[str, dict[str, str]]]:
     """Return a dict that could be entered directly into a platform json `files` key.
     - project_name: corresponds to a manifet template
     - session_str: [lims_id]_[mouse_id]_[session_id], will replace a placeholder in a manifest template
     """
     if session_type == 'D0':
-        return {'files': {f'ephys_raw_data_probe_{letter}': 
-        {'directory_name': f'{session_str}_probe{"ABC" if letter in "ABC" else "DEF"}'} for letter in 'ABCDEF'}}
-        
-    if session_type not in ["D1", "habituation", "D2"]:
-        raise ValueError(f"{session_type} is not a valid session type")
+        return {
+            'files': {
+                f'ephys_raw_data_probe_{letter}': {
+                    'directory_name': f'{session_str}_probe{"ABC" if letter in "ABC" else "DEF"}'
+                }
+                for letter in 'ABCDEF'
+            }
+        }
+
+    if session_type not in ['D1', 'habituation', 'D2']:
+        raise ValueError(f'{session_type} is not a valid session type')
 
-    template = paths.TEMPLATES_ROOT / session_type / f"{project_name}.json"
+    template = paths.TEMPLATES_ROOT / session_type / f'{project_name}.json'
 
     x = json.loads(template.read_bytes())
     # convert dict to str
     # replace % with session string
     # switch ' and " so we can convert str back to dict with json.loads()
-    return json.loads(str(x).replace("%", str(session_str)).replace("'", '"'))
+    return json.loads(str(x).replace('%', str(session_str)).replace("'", '"'))
 
 
-if __name__ == "__main__":
-    if is_connected("lims2"):
+if __name__ == '__main__':
+    if is_connected('lims2'):
         doctest.testmod()
         # optionflags=(doctest.ELLIPSIS, doctest.NORMALIZE_WHITESPACE, doctest.IGNORE_EXCEPTION_DETAIL)
     else:
-        print("LIMS not connected - skipping doctests")
+        print('LIMS not connected - skipping doctests')
```

### Comparing `np-session-0.5.4/tests/test_platform_json.py` & `np-session-0.6.0/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.4/PKG-INFO` & `np-session-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.5.4
+Version: 0.6.0
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
@@ -13,25 +13,29 @@
 Description-Content-Type: text/markdown
 
 # np_session
 
 
 ### *For use on internal Allen Institute network*
 
+A lightweight package for handling file paths and metadata associated with
+Mindscope Neuropixels experiments with data on local rig-connected machines or
+the /allen network.
+Provides an interface that can be used by other applications.
 
 ```python
 >>> from np_session import Session
 
 # initialize with a lims session ID or a string containing one: 
 >>> session = Session('c:/1116941914_surface-image1-left.png') 
 >>> session.lims.id
 1116941914
 >>> session.folder
 '1116941914_576323_20210721'
->>> session.is_ecephys_session
+>>> session.is_ecephys
 True
 >>> session.rig.acq # hostnames reflect the computers used during the session, not necessarily the current machines
 'W10DT05515'
 
 # some properties are objects with richer information:
 >>> session.mouse
 Mouse(576323)
```

