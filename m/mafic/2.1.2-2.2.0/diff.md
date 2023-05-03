# Comparing `tmp/mafic-2.1.2.tar.gz` & `tmp/mafic-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.1.2.tar", max compression
+gzip compressed data, was "mafic-2.2.0.tar", max compression
```

## Comparing `mafic-2.1.2.tar` & `mafic-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-04-30 15:55:28.846659 mafic-2.1.2/LICENSE
--rw-r--r--   0        0        0     3315 2023-04-30 15:55:28.846659 mafic-2.1.2/README.md
--rw-r--r--   0        0        0      886 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/__main__.py
--rw-r--r--   0        0        0     4447 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/errors.py
--rw-r--r--   0        0        0     5609 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/ip.py
--rw-r--r--   0        0        0    35580 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/node.py
--rw-r--r--   0        0        0    23615 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/player.py
--rw-r--r--   0        0        0      929 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/plugin.py
--rw-r--r--   0        0        0     8150 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/search_type.py
--rw-r--r--   0        0        0     3378 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/strategy.py
--rw-r--r--   0        0        0     4149 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/track.py
--rw-r--r--   0        0        0      747 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2817 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/common.py
--rw-r--r--   0        0        0     4018 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/http.py
--rw-r--r--   0        0        0     1968 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/incoming.py
--rw-r--r--   0        0        0      524 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/misc.py
--rw-r--r--   0        0        0     1152 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      139 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/utils/classproperty.py
--rw-r--r--   0        0        0     4987 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/utils/decode.py
--rw-r--r--   0        0        0      710 2023-04-30 15:55:28.846659 mafic-2.1.2/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-04-30 15:55:28.846659 mafic-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-03 20:48:25.093886 mafic-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-05-03 20:48:25.093886 mafic-2.2.0/README.md
+-rw-r--r--   0        0        0      886 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/ip.py
+-rw-r--r--   0        0        0    38923 2023-05-03 20:48:25.093886 mafic-2.2.0/mafic/node.py
+-rw-r--r--   0        0        0    24313 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/player.py
+-rw-r--r--   0        0        0      929 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/plugin.py
+-rw-r--r--   0        0        0     8715 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3378 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2953 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-05-03 20:48:25.097886 mafic-2.2.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-05-03 20:48:25.097886 mafic-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.2.0/PKG-INFO
```

### Comparing `mafic-2.1.2/LICENSE` & `mafic-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/README.md` & `mafic-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/__init__.py` & `mafic-2.2.0/mafic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.1.2/mafic/__libraries.py` & `mafic-2.2.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/__main__.py` & `mafic-2.2.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/errors.py` & `mafic-2.2.0/mafic/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
     Attributes
     ----------
     message: :class:`str`
         The message returned by the node.
     severity: :data:`~typing.Literal`\[``"COMMON"``, ``"SUSPICIOUS"``, ``"FATAL"``]
         The severity of the error.
+
+        This is lowercase in Lavalink v4.
     cause: :class:`str`
         The cause of the error.
     """
 
     def __init__(
         self, *, message: str, severity: ExceptionSeverity, cause: str
     ) -> None:
```

### Comparing `mafic-2.1.2/mafic/events.py` & `mafic-2.2.0/mafic/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     __slots__ = ("track", "reason", "player")
 
     def __init__(
         self, *, track: Track, payload: TrackEndEventPayload, player: PlayerT
     ) -> None:
         self.track: Track = track
-        self.reason: EndReason = EndReason(payload["reason"])
+        self.reason: EndReason = EndReason(payload["reason"].upper())
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
         """Get a string representation of the event."""
         return f"<TrackEndEvent track={self.track!r} reason={self.reason!r}>"
```

### Comparing `mafic-2.1.2/mafic/filter.py` & `mafic-2.2.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/ip.py` & `mafic-2.2.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/node.py` & `mafic-2.2.0/mafic/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         Player as PlayerPayload,
         PluginData,
         RoutePlannerStatus as RoutePlannerStatusPayload,
         TrackInfo,
         TrackLoadingResult,
         UpdatePlayerParams,
         UpdatePlayerPayload,
+        UpdateSessionPayload,
     )
 
 _log = getLogger(__name__)
 URL_REGEX = re.compile(r"https?://")
 
 __all__ = ("Node",)
 
@@ -137,20 +138,33 @@
         error.
     session: :data:`~typing.Optional`\[:class:`aiohttp.ClientSession`]
         The session to use for the node.
         If not provided, a new session will be created.
     resume_key:
         The key to use when resuming the node.
         If not provided, the key will be generated from the host, port and label.
+
+        .. warning::
+
+            This is ignored in lavalink V4, use ``resuming_session_id`` instead.
     regions:
         The voice regions that the node can be used in.
         This is used to determine when to use this node.
     shard_ids:
         The shard IDs that the node can be used in.
         This is used to determine when to use this node.
+    resuming_session_id:
+        The session ID to use when resuming the node.
+        If not provided, the node will not resume.
+
+        This should be stored from :func:`~mafic.on_node_ready` with :attr:`session_id`
+        to resume the session and gain control of the players. If the node is not
+        resuming, players will be destroyed if Lavalink loses connection to us.
+
+        .. versionadded:: 2.2
 
     Attributes
     ----------
     regions: :data:`~typing.Optional`\[:class:`list`\[:class:`~.VoiceRegion`]]
         The regions that the node can be used in.
         This is used to determine when to use this node.
     shard_ids: :data:`~typing.Optional`\[:class:`list`\[:class:`int`]]
@@ -158,29 +172,32 @@
         This is used to determine when to use this node.
     """
 
     __slots__ = (
         "__password",
         "__session",
         "_available",
+        "_checked_version",
         "_client",
         "_connect_task",
         "_heartbeat",
         "_host",
         "_label",
         "_msg_tasks",
         "_players",
         "_port",
         "_resume_key",
         "_secure",
         "_timeout",
         "_ready",
         "_rest_uri",
+        "_resuming_session_id",
         "_session_id",
         "_stats",
+        "_version",
         "_ws",
         "_ws_uri",
         "_ws_task",
         "regions",
         "shard_ids",
     )
 
@@ -195,14 +212,15 @@
         secure: bool = False,
         heartbeat: int = 30,
         timeout: float = 10,
         session: aiohttp.ClientSession | None = None,
         resume_key: str | None = None,
         regions: Sequence[Group | Region | VoiceRegion] | None = None,
         shard_ids: Sequence[int] | None = None,
+        resuming_session_id: str | None = None,
     ) -> None:
         self._host = host
         self._port = port
         self._label = label
         self.__password = password
         self._secure = secure
         self._heartbeat = heartbeat
@@ -213,14 +231,15 @@
         self.regions: list[VoiceRegion] | None = _wrap_regions(regions)
 
         self._rest_uri = yarl.URL.build(
             scheme=f"http{'s'*secure}", host=host, port=port
         )
         self._ws_uri = yarl.URL.build(scheme=f"ws{'s'*secure}", host=host, port=port)
         self._resume_key = resume_key or f"{host}:{port}:{label}"
+        self._resuming_session_id: str = resuming_session_id or ""
 
         self._ws: ClientWebSocketResponse | None = None
         self._ws_task: Task[None] | None = None
 
         self._available = False
         self._ready = Event()
 
@@ -228,14 +247,17 @@
 
         self._stats: NodeStats | None = None
         self._session_id: str | None = None
 
         self._msg_tasks: set[Task[None]] = set()
         self._connect_task: Task[None] | None = None
 
+        self._checked_version: bool = False
+        self._version: int = 3
+
     @property
     def host(self) -> str:
         """The host of the node."""
         return self._host
 
     @property
     def port(self) -> int:
@@ -361,14 +383,35 @@
 
         .. versionchanged:: 2.0
 
             This is now a list.
         """
         return [*self._players.values()]
 
+    @property
+    def session_id(self) -> str | None:
+        """The session ID of the node.
+
+        This is ``None`` if the node is not connected.
+
+        .. versionadded:: 2.2
+        """
+        return self._session_id
+
+    @property
+    def version(self) -> int:
+        """The major semver version of the node.
+
+        This is ``3`` if the node is not connected.
+        This is mostly used in :class:`Player` for version checks.
+
+        .. versionadded:: 2.2
+        """
+        return self._version
+
     def get_player(self, guild_id: int) -> Player[ClientT] | None:
         r"""Get a player from the node.
 
         Parameters
         ----------
         guild_id:
             The guild ID to get the player for.
@@ -403,66 +446,81 @@
         Parameters
         ----------
         guild_id:
             The guild ID to remove the player for.
         """
         self._players.pop(guild_id, None)
 
-    async def _check_version(self) -> None:
-        """Check the version of the node.
+    async def _check_version(self) -> int:
+        """:class:`int`: The major version of the node.
+
+        This also does checks based on if that is supported.
 
         Raises
         ------
         :exc:`RuntimeError`
             If the
-            - major version is not 3
-            - minor version is less than 7
+            - major version is not in (3, 4)
+            - minor version is less than 7 when the major version is 3
 
-            This is because the rest api is in 3.7, and v4 will have breaking changes.
+            This is because the rest api is in 3.7, and v5 will have breaking changes.
 
         Warns
         -----
         :class:`UnsupportedVersionWarning`
-            If the minor version is greater than 7.
+            If the
+            - major version is 3 and the minor version is more than 7
+            - major version is 4 and the minor version is more than 0
             Some features may not work.
         """
-        if self._rest_uri.path.endswith("/v3") or self._ws_uri.path.endswith(
-            "/websocket"
-        ):
+        if self._checked_version:
             # This process was already ran likely.
-            return
+            return self._version
 
         if self.__session is None:
             self.__session = await self._create_session()
 
         async with self.__session.get(
             self._rest_uri / "version",
             headers={"Authorization": self.__password},
         ) as resp:
             # Only the major and minor are needed.
             version = await resp.text()
 
             try:
                 major, minor, _ = version.split(".", maxsplit=2)
             except ValueError:
-                message = UnknownVersionWarning.message
-                warnings.warn(message, UnknownVersionWarning)
+                if version.endswith("-SNAPSHOT"):
+                    major = 4
+                    minor = 0
+                else:
+                    major = 3
+                    minor = 7
+                    message = UnknownVersionWarning.message
+                    warnings.warn(message, UnknownVersionWarning)
             else:
                 major = int(major)
                 minor = int(minor)
 
-                if major != 3 or minor < 7:
-                    msg = f"Unsupported lavalink version {version} (expected 3.7.x)"
+                if major not in (3, 4) or (major == 3 and minor < 7):
+                    msg = (
+                        f"Unsupported lavalink version {version} "
+                        "(expected 3.7.x or 4.x.x)"
+                    )
                     raise RuntimeError(msg)
-                elif minor > 7:
+                elif (major == 3 and minor > 7) or (major == 4 and minor > 0):
                     message = UnsupportedVersionWarning.message
                     warnings.warn(message, UnsupportedVersionWarning)
 
-            self._rest_uri /= "v3"
-            self._ws_uri /= "v3/websocket"
+            self._rest_uri /= f"v{major}"
+            self._ws_uri /= f"v{major}/websocket"
+
+            self._version = major
+            self._checked_version = True
+            return major
 
     async def _connect_to_websocket(
         self, headers: dict[str, str], session: aiohttp.ClientSession
     ) -> None:
         """Connect to the websocket of the node.
 
         Parameters
@@ -518,23 +576,28 @@
             raise RuntimeError(msg)
 
         if self.__session is None:
             self.__session = await self._create_session()
 
         session = self.__session
 
+        _log.debug("Checking lavalink version...", extra={"label": self._label})
+        version = await self._check_version()
+
         headers: dict[str, str] = {
             "Authorization": self.__password,
             "User-Id": str(self._client.user.id),
             "Client-Name": f"Mafic/{__import__('mafic').__version__}",
-            "Resume-Key": self._resume_key,
         }
 
-        _log.debug("Checking lavalink version...", extra={"label": self._label})
-        await self._check_version()
+        # V4 uses session ID resuming
+        if version == 3:
+            headers["Resume-Key"] = self._resume_key
+        else:
+            headers["Session-Id"] = self._resuming_session_id
 
         _log.info(
             "Connecting to lavalink at %s...",
             self._rest_uri,
             extra={"label": self._label},
         )
         try:
@@ -586,14 +649,15 @@
             raise
         else:
             _log.info(
                 "Node %s is now available.", self._label, extra={"label": self._label}
             )
             await self.sync_players()
             self._available = True
+            self._client.dispatch("node_ready", self)
 
     async def _ws_listener(self) -> None:
         """Listen for messages from the websocket."""
         backoff = ExponentialBackoff()
 
         if self._ws is None:
             _log.error(
@@ -606,17 +670,15 @@
         # To catch closing messages, we cannot use async for.
         while True:
             msg = await self._ws.receive()
 
             _log.debug("Received message from websocket.", extra={"label": self._label})
 
             # Please aiohttp, fix your typehints.
-            _type: aiohttp.WSMsgType = (
-                msg.type
-            )  # pyright: ignore[reportUnknownMemberType]
+            _type: aiohttp.WSMsgType = msg.type  # pyright: ignore
 
             if _type is aiohttp.WSMsgType.CLOSED:
                 self._available = False
                 close_code = self._ws.close_code
                 self._ws = None
 
                 wait_time = backoff.delay()
@@ -652,16 +714,16 @@
         """Handle a message from the websocket.
 
         Parameters
         ----------
         data:
             The data to handle.
         """
-        _log.debug("Received event with op %s", data["op"])
         _log.debug("Event data: %s", data)
+        _log.debug("Received event with op %s", data["op"])
 
         if data["op"] == "playerUpdate":
             guild_id = int(data["guildId"])
             player = self.get_player(guild_id)
 
             if player is None:
                 if data["state"]["connected"] is True:
@@ -688,19 +750,26 @@
 
             if resumed:
                 _log.info(
                     "Successfully resumed connection with lavalink.",
                     extra={"label": self._label},
                 )
             else:
-                _log.debug(
-                    "Sending configuration to resume with key %s",
-                    self._resume_key,
-                    extra={"label": self._label},
-                )
+                if self._version == 3:
+                    _log.debug(
+                        "Sending configuration to resume with key %s",
+                        self._resume_key,
+                        extra={"label": self._label},
+                    )
+                else:
+                    _log.debug(
+                        "Sending configuration to resume with session ID %s",
+                        self._session_id,
+                        extra={"label": self._label},
+                    )
                 await self.configure_resuming()
 
             self._ready.set()
         else:
             # Of course pyright considers this to be `Never`, so this is to keep types.
             op = cast(str, data["op"])
             _log.warn("Unknown incoming message op code %s", op)
@@ -761,27 +830,40 @@
                     "token": data["token"],
                 },
             },
         )
 
     def configure_resuming(self) -> Coro[None]:
         """Configure the node to resume."""
-        _log.info(
-            "Sending resume configuration to lavalink with resume key %s.",
-            self._resume_key,
-            extra={"label": self._label},
-        )
+        data: UpdateSessionPayload
+        if self._version == 3:
+            _log.info(
+                "Sending resume configuration to lavalink with resume key %s.",
+                self._resume_key,
+                extra={"label": self._label},
+            )
+            data = {
+                "resumingKey": self._resume_key,
+                "timeout": 60,
+            }
+        else:
+            _log.info(
+                "Sending resume configuration to lavalink with session ID %s.",
+                self._session_id,
+                extra={"label": self._label},
+            )
+            data = {
+                "resuming": True,
+                "timeout": 60,
+            }
 
         return self.__request(
             "PATCH",
             f"sessions/{self._session_id}",
-            {
-                "resumingKey": self._resume_key,
-                "timeout": 60,
-            },
+            data,
         )
 
     def destroy(self, guild_id: int) -> Coro[None]:
         """Destroy a player.
 
         Parameters
         ----------
@@ -935,15 +1017,15 @@
                 "Received status %s from lavalink from path %s", resp.status, path
             )
 
             json = await resp.json(loads=loads)
             _log.debug("Received raw data %s from %s", json, path)
             return json
 
-    async def fetch_tracks(
+    async def fetch_tracks(  # noqa: PLR0911  # V3/V4 compat.
         self, query: str, *, search_type: str
     ) -> list[Track] | Playlist | None:
         r"""Fetch tracks from the node.
 
         Parameters
         ----------
         query:
@@ -963,16 +1045,24 @@
         if not URL_REGEX.match(query):
             query = f"{search_type}:{query}"
 
         data: TrackLoadingResult = await self.__request(
             "GET", "loadtracks", params={"identifier": query}
         )
 
-        if data["loadType"] == "NO_MATCHES":
+        if data["loadType"] in ("empty", "NO_MATCHES"):
             return []
+        elif data["loadType"] == "track":
+            return [Track.from_data_with_info(data["data"])]
+        elif data["loadType"] == "playlist":
+            return Playlist(info=data["data"]["info"], tracks=data["data"]["tracks"])
+        elif data["loadType"] == "search":
+            return [Track.from_data_with_info(track) for track in data["data"]]
+        elif data["loadType"] == "error":
+            raise TrackLoadException.from_data(data["data"])
         elif data["loadType"] == "TRACK_LOADED":
             return [Track.from_data_with_info(data["tracks"][0])]
         elif data["loadType"] == "PLAYLIST_LOADED":
             return Playlist(info=data["playlistInfo"], tracks=data["tracks"])
         elif data["loadType"] == "SEARCH_RESULT":
             return [Track.from_data_with_info(track) for track in data["tracks"]]
         elif data["loadType"] == "LOAD_FAILED":
```

### Comparing `mafic-2.1.2/mafic/player.py` & `mafic-2.2.0/mafic/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .errors import NoNodesAvailable, PlayerNotConnected
 from .events import *
 from .filter import Filter
 from .pool import NodePool
 from .search_type import SearchType
 from .track import Track
 from .type_variables import ClientT
+from .typings import TrackWithInfo
 
 if TYPE_CHECKING:
     from .__libraries import (
         Connectable,
         Guild,
         GuildVoiceStatePayload,
         VoiceServerUpdatePayload,
@@ -236,56 +237,72 @@
             The event payload to dispatch.
         """
         if data["type"] == "WebSocketClosedEvent":
             event = WebSocketClosedEvent(payload=data, player=self)
             _log.debug("Received websocket closed event: %s", event)
             self.client.dispatch("websocket_closed", event)
         elif data["type"] == "TrackStartEvent":
-            track = self._current
+            track = (
+                self._current
+                if self.node.version == 3
+                else Track.from_data_with_info(cast(TrackWithInfo, data.get("track")))
+            )
 
             if track is None:
                 _log.error(
                     "Received track start event but no track was playing, discarding."
                 )
                 return
 
             event = TrackStartEvent(player=self, track=track)
             self.client.dispatch("track_start", event)
             _log.debug("Received track start event: %s", event)
             self._last_track = track
         elif data["type"] == "TrackEndEvent":
-            track = self._last_track
+            track = (
+                self._last_track
+                if self.node.version == 3
+                else Track.from_data_with_info(cast(TrackWithInfo, data.get("track")))
+            )
 
             if track is None:
                 _log.error(
                     "Received track end event but no track was playing, discarding."
                 )
                 return
 
             event = TrackEndEvent(player=self, track=track, payload=data)
             self.client.dispatch("track_end", event)
             _log.debug("Received track end event: %s", event)
 
             if data["reason"] != "REPLACED":
                 self._current = None
         elif data["type"] == "TrackExceptionEvent":
-            track = self._current
+            track = (
+                self._current
+                if self.node.version == 3
+                else Track.from_data_with_info(cast(TrackWithInfo, data.get("track")))
+            )
 
             if track is None:
                 _log.error(
                     "Received track exception event but no track was playing, "
                     "discarding."
                 )
                 return
 
             event = TrackExceptionEvent(player=self, track=track, payload=data)
             self.client.dispatch("track_exception", event)
             _log.debug("Received track exception event: %s", event)
         elif data["type"] == "TrackStuckEvent":
-            track = self._current
+            track = (
+                self._current
+                if self.node.version == 3
+                else Track.from_data_with_info(cast(TrackWithInfo, data.get("track")))
+            )
 
             if track is None:
                 _log.error(
                     "Received track stuck event but no track was playing, discarding."
                 )
                 return
 
@@ -386,15 +403,15 @@
         self_deaf:
             Whether to deafen the bot on connect.
         """
         if not isinstance(self.channel, (VoiceChannel, StageChannel)):
             msg = "Voice channel must be a VoiceChannel or StageChannel."
             raise TypeError(msg)
 
-        if not NodePool.nodes:
+        if not NodePool.nodes:  # pyright: ignore
             raise NoNodesAvailable
 
         _log.debug("Connecting to voice channel %s", self.channel.id)
 
         await self.channel.guild.change_voice_state(
             channel=self.channel, self_mute=self_mute, self_deaf=self_deaf
         )
```

### Comparing `mafic-2.1.2/mafic/playlist.py` & `mafic-2.2.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/plugin.py` & `mafic-2.2.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/pool.py` & `mafic-2.2.0/mafic/pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 from collections.abc import Sequence
 from functools import partial
 from logging import getLogger
 from random import choice
-from typing import TYPE_CHECKING, Any, Generic, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Generic, List, TypeVar, Union, cast
 
 from .errors import NoNodesAvailable
 from .node import Node
 from .strategy import Strategy, StrategyCallable, call_strategy
 from .type_variables import ClientT
 from .utils import classproperty
 
@@ -104,14 +104,15 @@
         secure: bool = False,
         heartbeat: int = 30,
         timeout: float = 10,
         session: aiohttp.ClientSession | None = None,
         resume_key: str | None = None,
         regions: Sequence[Group | Region | VoiceRegion] | None = None,
         shard_ids: Sequence[int] | None = None,
+        resuming_session_id: str | None = None,
     ) -> Node[ClientT]:
         r"""Create a node and connect it.
 
         The parameters here relate to :class:`Node`.
 
         Parameters
         ----------
@@ -128,25 +129,36 @@
         heartbeat:
             The interval to send heartbeats to the node websocket connection.
         timeout:
             The timeout to use for the node websocket connection.
         session: :data:`~typing.Optional`\[:class:`aiohttp.ClientSession`]
             The session to use for the node websocket connection.
         resume_key:
-            The key to use to resume the node websocket connection.
-            This is used to resume a connection if the connection is lost.
-            Defaults to using the `host`, `port` and `label`.
+            The key to use when resuming the node.
+            If not provided, the key will be generated from the host, port and label.
+
+            .. warning::
+
+                This is ignored in lavalink V4, use ``resuming_session_id`` instead.
         regions:
-            The regions this node is best to connect to.
-            This is used to determine if this is the best node for a connection
-            with :attr:`Strategy.LOCATION`.
+            The voice regions that the node can be used in.
+            This is used to determine when to use this node.
         shard_ids:
-            The shard IDs this node is best to connect to.
-            This is used to determine if this is the best node for a connection
-            with :attr:`Strategy.SHARD`.
+            The shard IDs that the node can be used in.
+            This is used to determine when to use this node.
+        resuming_session_id:
+            The session ID to use when resuming the node.
+            If not provided, the node will not resume.
+
+            This should be stored from :func:`~mafic.on_node_ready` with
+            :attr:`session_id` to resume the session and gain control of the players.
+            If the node is not resuming, players will be destroyed if Lavalink loses
+            connection to us.
+
+            .. versionadded:: 2.2
 
         Returns
         -------
         :class:`Node`
             The created node.
 
         Raises
@@ -167,14 +179,15 @@
             secure=secure,
             heartbeat=heartbeat,
             timeout=timeout,
             session=session,
             resume_key=resume_key,
             regions=regions,
             shard_ids=shard_ids,
+            resuming_session_id=resuming_session_id,
         )
 
         # Add to dictionaries, creating a set or extending it if needed.
         if node.regions:
             for region in node.regions:
                 self._node_regions[region] = {
                     node,
@@ -230,15 +243,16 @@
 
         actual_strategies: Sequence[StrategyCallable[ClientT] | Strategy]
 
         strategies = strategies or cls._default_strategies
 
         actual_strategies = [strategies] if callable(strategies) else strategies
 
-        nodes = cls.nodes
+        # It is a classproperty.
+        nodes = cast(List[Node[ClientT]], cls.nodes)  # pyright: ignore
 
         for strategy in actual_strategies:
             if isinstance(strategy, Strategy):
                 strategy_callable = partial(call_strategy, strategy)
             else:
                 strategy_callable = strategy
```

### Comparing `mafic-2.1.2/mafic/region.py` & `mafic-2.2.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/search_type.py` & `mafic-2.2.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/stats.py` & `mafic-2.2.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/strategy.py` & `mafic-2.2.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/track.py` & `mafic-2.2.0/mafic/track.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,42 +55,56 @@
         Whether the track is a stream.
     seekable: :class:`bool`
         Whether the track is seekable.
     position: :class:`int`
         The current position of the track.
     length: :class:`int`
         The length of the track.
+    artwork_url: :data:`~typing.Optional`\[:class:`str`]
+        The artwork URL of the track.
+        This is always ``None`` if the node does not use Lavalink v4.
+
+        .. versionadded:: 2.2
+    isrc: :data:`~typing.Optional`\[:class:`str`]
+        The ISRC of the track.
+        This is always ``None`` if the node does not use Lavalink v4.
+
+        .. versionadded:: 2.2
     """
 
     __slots__ = (
         "author",
+        "artwork_url",
         "id",
         "identifier",
+        "isrc",
         "length",
         "position",
         "seekable",
         "source",
         "stream",
         "title",
         "uri",
     )
 
     def __init__(
         self,
         *,
         track_id: str,
-        title: str,
-        author: str,
         identifier: str,
-        uri: str | None,
-        source: str,
-        stream: bool,
         seekable: bool,
-        position: int = 0,
+        author: str,
         length: int,
+        stream: bool,
+        position: int = 0,
+        title: str,
+        uri: str | None,
+        artwork_url: str | None,
+        isrc: str | None,
+        source: str,
     ) -> None:
         self.id: str = track_id
 
         self.title: str = title
         self.author: str = author
 
         self.identifier: str = identifier
@@ -100,14 +114,17 @@
         self.stream: bool = stream
 
         self.seekable: bool = seekable
 
         self.position: int = position
         self.length: int = length
 
+        self.artwork_url: str | None = artwork_url
+        self.isrc: str | None = isrc
+
     @classmethod
     def from_data(cls, *, track: str, info: TrackInfo) -> Self:
         """Create a track from the raw data.
 
         Parameters
         ----------
         track:
@@ -127,14 +144,16 @@
             identifier=info["identifier"],
             uri=info["uri"],
             source=info["sourceName"],
             stream=info["isStream"],
             seekable=info["isSeekable"],
             position=info["position"],
             length=info["length"],
+            artwork_url=info.get("artworkUrl"),
+            isrc=info.get("isrc"),
         )
 
     @classmethod
     def from_data_with_info(cls, data: TrackWithInfo) -> Self:
         """Create a track from the raw data, bundled with the track and info.
 
         Parameters
```

### Comparing `mafic-2.1.2/mafic/type_variables.py` & `mafic-2.2.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.2/mafic/typings/common.py` & `mafic-2.2.0/mafic/typings/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,18 @@
     identifier: str
     isSeekable: bool
     author: str
     length: int
     isStream: bool
     position: int
     title: str
-    uri: str
+    uri: str | None
+    # TODO: Remove NotRequired when V3 support removed
+    artworkUrl: NotRequired[str | None]
+    isrc: NotRequired[str | None]
     sourceName: str
 
 
 class TrackWithInfo(TypedDict):
     encoded: str
     info: TrackInfo
```

### Comparing `mafic-2.1.2/mafic/typings/http.py` & `mafic-2.2.0/mafic/typings/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: MIT
 # ruff: noqa: UP013
 # `class` in `TypedDict` does not work as that is a reserved keyword
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Literal, Optional, TypedDict, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, TypedDict, Union
 
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
     from .common import PlaylistInfo, TrackWithInfo
     from .misc import LavalinkException
 
@@ -45,14 +45,17 @@
     "RotatingNanoIPRoutePlanner",
     "BalancingIPRoutePlanner",
     "EmptyRoutePlanner",
     "RoutePlannerStatus",
 )
 
 
+# V3
+
+
 class PlaylistTracks(TypedDict):
     loadType: Literal["PLAYLIST_LOADED"]
     playlistInfo: PlaylistInfo
     tracks: list[TrackWithInfo]
 
 
 class GenericTracks(TypedDict):
@@ -65,15 +68,58 @@
     exception: LavalinkException
 
 
 class NoMatches(TypedDict):
     loadType: Literal["NO_MATCHES"]
 
 
-TrackLoadingResult = Union[PlaylistTracks, GenericTracks, TracksFailed, NoMatches]
+# V4
+
+
+class TrackLoadedV4(TypedDict):
+    loadType: Literal["track"]
+    data: TrackWithInfo
+
+
+class PlaylistLoadedV4(TypedDict):
+    loadType: Literal["playlist"]
+    data: PlaylistDataV4
+
+
+class PlaylistDataV4(TypedDict):
+    info: PlaylistInfo
+    pluginInfo: dict[str, Any]
+    tracks: list[TrackWithInfo]
+
+
+class SearchResultV4(TypedDict):
+    loadType: Literal["search"]
+    data: list[TrackWithInfo]
+
+
+class SearchEmptyV4(TypedDict):
+    loadType: Literal["empty"]
+
+
+class LoadErrorV4(TypedDict):
+    loadType: Literal["error"]
+    data: LavalinkException
+
+
+TrackLoadingResult = Union[
+    PlaylistTracks,
+    GenericTracks,
+    TracksFailed,
+    NoMatches,
+    TrackLoadedV4,
+    PlaylistLoadedV4,
+    SearchResultV4,
+    SearchEmptyV4,
+    LoadErrorV4,
+]
 
 
 class PluginData(TypedDict):
     name: str
     version: str
```

### Comparing `mafic-2.1.2/mafic/typings/incoming.py` & `mafic-2.2.0/mafic/typings/incoming.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypedDict, Union
 
-from .common import Stats
+from .common import Stats, TrackWithInfo
 from .misc import PayloadWithGuild
 
 if TYPE_CHECKING:
     from typing import Literal
 
     from typing_extensions import NotRequired
 
@@ -46,41 +46,60 @@
     reason: str
     byRemote: bool
 
 
 class TrackStartEvent(PayloadWithGuild):
     op: Literal["event"]
     type: Literal["TrackStartEvent"]
-    encodedTrack: str
+    # V3
+    encodedTrack: NotRequired[str]
+    # V4
+    track: NotRequired[TrackWithInfo]
 
 
 class TrackEndEvent(PayloadWithGuild):
     op: Literal["event"]
     type: Literal["TrackEndEvent"]
-    encodedTrack: str
+    # V3
+    encodedTrack: NotRequired[str]
+    # V4
+    track: NotRequired[TrackWithInfo]
     reason: Literal[
+        # V3
         "FINISHED",
         "LOAD_FAILED",
         "STOPPED",
         "REPLACED",
         "CLEANUP",
+        # V4
+        "finished",
+        "loadFailed",
+        "stopped",
+        "replaced",
+        "cleanup",
     ]
 
 
 class TrackExceptionEvent(PayloadWithGuild):
     op: Literal["event"]
     type: Literal["TrackExceptionEvent"]
-    encodedTrack: str
+    # V3
+    encodedTrack: NotRequired[str]
+    # V4
+    track: NotRequired[TrackWithInfo]
     exception: LavalinkException
 
 
 class TrackStuckEvent(PayloadWithGuild):
     op: Literal["event"]
     type: Literal["TrackStuckEvent"]
-    encodedTrack: str
+    # V3
+    encodedTrack: NotRequired[str]
+    # V4
+    track: NotRequired[TrackWithInfo]
     thresholdMs: int
 
 
 class ReadyPayload(TypedDict):
     op: Literal["ready"]
     resumed: bool
     sessionId: str
```

### Comparing `mafic-2.1.2/mafic/typings/misc.py` & `mafic-2.2.0/mafic/typings/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,24 @@
     "LavalinkException",
     "ExceptionSeverity",
     "PayloadWithGuild",
 )
 T = TypeVar("T")
 
 Coro = Coroutine[Any, Any, T]
-ExceptionSeverity = Literal["COMMON", "SUSPICIOUS", "FAULT"]
+ExceptionSeverity = Literal[
+    # V3
+    "COMMON",
+    "SUSPICIOUS",
+    "FAULT",
+    # V4
+    "common",
+    "suspicious",
+    "fault",
+]
 
 
 class LavalinkException(TypedDict):
     severity: ExceptionSeverity
     message: str
     cause: str
```

### Comparing `mafic-2.1.2/mafic/typings/outgoing.py` & `mafic-2.2.0/mafic/typings/outgoing.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     "UpdatePlayerPayload",
     "UpdatePlayerParams",
     "UpdateSessionPayload",
 )
 
 
 class UpdateSessionPayload(TypedDict, total=False):
+    # V3
     resumingKey: str | None
+    # V4
+    resuming: bool
     timeout: int
 
 
 class UpdatePlayerPayload(TypedDict, total=False):
     encodedTrack: str | None
     identifier: str
     position: int
```

### Comparing `mafic-2.1.2/mafic/utils/classproperty.py` & `mafic-2.2.0/mafic/utils/classproperty.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 """Contains a decorator to merge properties and classmethods."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, Type, TypeVar, cast
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 T = TypeVar("T")
+R = TypeVar("R")
 
 __all__ = ("classproperty",)
 
 
-class _ClassPropertyDescriptor(Generic[T]):
+class _ClassPropertyDescriptor(Generic[T, R]):
     """A descriptor that mimics the behavior of a property, but for classmethods."""
 
-    def __init__(self, fget: classmethod[T] | staticmethod[T]) -> None:
+    def __init__(self, fget: classmethod[T, ..., R] | staticmethod[..., R]) -> None:
         self.fget = fget
 
-    def __get__(self, instance: object, owner: type | None = None) -> T:
+    def __get__(self, instance: T, owner: type[T] | None = None) -> R:
         if owner is None:
-            owner = type(instance)
+            owner = cast(Type[T], type(instance))
         return self.fget.__get__(instance, owner)()
 
 
 def classproperty(
-    func: Callable[..., T] | classmethod[T] | staticmethod[T]
-) -> _ClassPropertyDescriptor[T]:
+    func: Callable[[T], R] | classmethod[T, ..., R] | staticmethod[..., R]
+) -> _ClassPropertyDescriptor[T, R]:
     """Contains a decorator to mimic the behavior of a property, but for classmethods.
 
     Parameters
     ----------
     func:
         The function to decorate.
     """
```

### Comparing `mafic-2.1.2/mafic/warnings.py` & `mafic-2.2.0/mafic/warnings.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 
 
 class UnknownVersionWarning(UserWarning):
     """Represents a warning for an unknown version of Lavalink."""
 
     message: str = (
         "The version of Lavalink you are using is unknown to Mafic. "
-        "It should still work but not all features are supported."
+        "It should still work but not all features are supported. "
+        "Assuming Lavalink v3.7."
     )
```

### Comparing `mafic-2.1.2/pyproject.toml` & `mafic-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.1.2"
+version = "2.2.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
@@ -36,15 +36,15 @@
 orjson = { version = "^3.8.0", optional = true }
 yarl = "^1.0.0"
 
 [tool.poetry.extras]
 speedups = ["orjson"]
 
 [tool.poetry.group.dev.dependencies]
-pyright = "1.1.289"
+pyright = "1.1.306"
 black = "^22.8.0"
 taskipy = "^1.10.3"
 pre-commit = "^2.20.0"
 python-dotenv = "^0.21.0"
 slotscheck = "^0.15.0"
 typing-extensions = "^4.3.0"
 ruff = "^0.0.251"
```

### Comparing `mafic-2.1.2/PKG-INFO` & `mafic-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.1.2
+Version: 2.2.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

