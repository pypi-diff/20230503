# Comparing `tmp/gridworks_debug_cli-0.2.5.tar.gz` & `tmp/gridworks_debug_cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_debug_cli-0.2.5.tar", max compression
+gzip compressed data, was "gridworks_debug_cli-0.2.6.tar", max compression
```

## Comparing `gridworks_debug_cli-0.2.5.tar` & `gridworks_debug_cli-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/LICENSE
--rw-r--r--   0        0        0     4476 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/README.md
--rw-r--r--   0        0        0     2375 2023-04-03 15:05:54.146893 gridworks_debug_cli-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       27 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/__init__.py
--rw-r--r--   0        0        0      467 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/__main__.py
--rw-r--r--   0        0        0       63 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/csv/__init__.py
--rw-r--r--   0        0        0     2880 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/csv/__main__.py
--rw-r--r--   0        0        0    11313 2023-04-03 15:05:54.146893 gridworks_debug_cli-0.2.5/src/gwdcli/csv/egauge_download.py
--rw-r--r--   0        0        0     3939 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/csv/settings.py
--rw-r--r--   0        0        0       66 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/events/__init__.py
--rw-r--r--   0        0        0     4912 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/events/__main__.py
--rw-r--r--   0        0        0     9132 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/events/models.py
--rw-r--r--   0        0        0     4578 2023-04-03 15:05:36.113653 gridworks_debug_cli-0.2.5/src/gwdcli/events/mqtt.py
--rw-r--r--   0        0        0     1429 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/events/queue_loop.py
--rw-r--r--   0        0        0     3676 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/events/settings.py
--rw-r--r--   0        0        0     1936 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/events/show_dir.py
--rw-r--r--   0        0        0     5768 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/events/sync.py
--rw-r--r--   0        0        0    18071 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/events/tui.py
--rw-r--r--   0        0        0        0 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/py.typed
--rw-r--r--   0        0        0        0 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/utils/__init__.py
--rw-r--r--   0        0        0      509 2023-04-03 15:05:36.117654 gridworks_debug_cli-0.2.5/src/gwdcli/utils/settings.py
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4476 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/README.md
+-rw-r--r--   0        0        0     2375 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/__main__.py
+-rw-r--r--   0        0        0       63 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/__main__.py
+-rw-r--r--   0        0        0    11313 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/egauge_download.py
+-rw-r--r--   0        0        0     3939 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/settings.py
+-rw-r--r--   0        0        0       66 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/__init__.py
+-rw-r--r--   0        0        0     5553 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/__main__.py
+-rw-r--r--   0        0        0     9199 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/models.py
+-rw-r--r--   0        0        0     4578 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/mqtt.py
+-rw-r--r--   0        0        0     1429 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/queue_loop.py
+-rw-r--r--   0        0        0     3703 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/settings.py
+-rw-r--r--   0        0        0     1936 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/show_dir.py
+-rw-r--r--   0        0        0     5768 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/sync.py
+-rw-r--r--   0        0        0    18985 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/tui.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/py.typed
+-rw-r--r--   0        0        0        0 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/utils/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/utils/settings.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.6/PKG-INFO
```

### Comparing `gridworks_debug_cli-0.2.5/LICENSE` & `gridworks_debug_cli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/README.md` & `gridworks_debug_cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/pyproject.toml` & `gridworks_debug_cli-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-debug-cli"
-version = "0.2.5"
+version = "0.2.6"
 description = "Gridworks Debug Cli"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-debug-cli"
 repository = "https://github.com/anschweitzer/gridworks-debug-cli"
 documentation = "https://gridworks-debug-cli.readthedocs.io"
```

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/csv/__main__.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/csv/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/csv/egauge_download.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/csv/egauge_download.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/csv/settings.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/csv/settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/__main__.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,30 @@
 typer_click_object = typer.main.get_command(app)
 
 
 @app.command()
 def show(
     config_path: Path = Paths().config_path,
     verbose: int = typer.Option(0, "--verbose", "-v", count=True),
-    snap: Optional[List[str]] = typer.Option(None, "--snap"),
+    snap: Optional[List[str]] = typer.Option(
+        None,
+        "--snap",
+        help=(
+            "Scadas whose [bold]snapshots[/bold] to show. May be specified multiple times. If present, "
+            "a snapshot message Src must contain one of these values to be displayed."
+        ),
+    ),
+    scada: Optional[List[str]] = typer.Option(
+        None,
+        "--scada",
+        help=(
+            "Scadas whose [bold]events[/bold] to show. May be specified multiple times. If present, "
+            "an event message Src must contain one of these values to be displayed."
+        ),
+    ),
     clean: bool = typer.Option(  # noqa
         False, "-c", "--clean", help="Delete the entire data directory."
     ),
     no_sync: bool = typer.Option(
         False,
         "--no-sync",
         help="Skip downloading data from S3. Only mqtt data will be monitored.",
@@ -51,15 +66,18 @@
         "--no-mqtt",
         help="Download data from S3 but do no live monitoring of mqtt.",
     ),
 ):
     """Live display of incoming scada events and status"""
     settings = EventsSettings.load(config_path)
     settings.verbosity += verbose
+    settings.scadas += scada
     settings.snaps += snap
+    if not settings.snaps:
+        settings.snaps = settings.scadas[:]
     if clean:
         rich.print(f"Deleting {settings.paths.data_dir}")
         shutil.rmtree(settings.paths.data_dir)
     run(show_main, settings, Console(), not no_sync, not no_mqtt)
 
 
 @app.command()
```

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/models.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 
 class AnyEvent(EventBase, extra=Extra.allow):
     TypeName: str
     _message_src: str = ""
 
     def other_fields(self) -> dict:
-        return self.dict(exclude=EventBase.__fields__.keys())
+        exclude = set(EventBase.__fields__.keys())
+        exclude.add("_message_src")
+        return self.dict(exclude=exclude)
 
     def as_pandas_record(
         self,
         collapse_other_fields: bool = True,
         other_field_name: str = "other_fields",
         explicit_summary: str = "",
         interpolate_summary: bool = False,
```

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/mqtt.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/queue_loop.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/queue_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/settings.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     max_other_fields_width: int = 90
     c_to_f: bool = True
 
 
 class EventsSettings(BaseSettings):
     verbosity: int = 0
     snaps: list[str] = []
+    scadas: list[str] = []
     paths: Paths = Paths()
     sync: SyncSettings = SyncSettings()
     mqtt: MQTTClient = MQTTClient()
     tui: TUISettings = TUISettings()
 
     @classmethod
     def load(
```

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/show_dir.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/show_dir.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/sync.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.5/src/gwdcli/events/tui.py` & `gridworks_debug_cli-0.2.6/src/gwdcli/events/tui.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from pathlib import Path
 from typing import Any
+from typing import Optional
+from typing import Sequence
 
 import pandas as pd
 from anyio import to_thread
 from gwproto import Message
 from gwproto.enums import TelemetryName
 from gwproto.gs import GsPwr
 from gwproto.messages import EventBase
@@ -123,15 +125,15 @@
         else:
             self.df = pd.DataFrame(
                 index=pd.DatetimeIndex([], name="TimeNS"),
                 columns=["MessageId", "Src", "TypeName", "other_fields"],
             )
         self.df.drop_duplicates("MessageId", inplace=True)
         self.live_history_df = self.df.head(0)
-        self.display_df = self.df.tail(self.settings.tui.displayed_events)
+        self.display_df = self.extract_display_df()
         self.queue = queue.Queue()
         self.gwd_text = Text()
         self.sync_spinners = SyncSpinners()
         # noinspection PyTypeChecker
         self.local_tz = datetime.now(timezone(timedelta(0))).astimezone().tzinfo
         self.event_table = self.make_event_table()
         self.load_snaps()
@@ -168,24 +170,36 @@
 
     def load_statuses(self):
         self._load_latest("status", "statuses", GtShStatus_Maker)
 
     def load_snaps(self):
         self._load_latest("snap", "snaps", SnapshotSpaceheat_Maker)
 
+    def extract_display_df(self) -> pd.DataFrame:
+        if self.settings.scadas:
+            srcs_used = [
+                src
+                for src in self.df["Src"].unique()
+                if any(scada in src for scada in self.settings.scadas)
+            ]
+            filtered_df = self.df[self.df["Src"].isin(srcs_used)]
+        else:
+            filtered_df = self.df
+        return filtered_df.tail(self.settings.tui.displayed_events)
+
     def reload_dfs(self):
         self.df = pd.read_csv(
             self.settings.paths.csv_path,
             index_col="TimeNS",
             parse_dates=True,
             date_parser=functools.partial(pd.to_datetime, utc=True),
         )
         self.df = pd.concat([self.df, self.live_history_df]).sort_index()
         self.df.drop_duplicates("MessageId", inplace=True)
-        self.display_df = self.df.tail(self.settings.tui.displayed_events)
+        self.display_df = self.extract_display_df()
 
     def make_layout(self):
         self.layout = Layout(name="root")
         self.layout.split(
             Layout(name="header", size=3),
             Layout(name="main", ratio=1),
             Layout(name="footer", size=10),
@@ -198,15 +212,15 @@
             Layout(name="snap0"),
             Layout(name="snap1"),
         )
         self.layout["footer"].split_row(
             Layout(name="GWDEvents", minimum_size=100, ratio=2),
             Layout(name="sync"),
         )
-        self.layout["header"].update(Header())
+        self.layout["header"].update(Header(self.settings.scadas))
         self.layout["events"].update(self.event_table)
         self.layout["GWDEvents"].update(
             Panel(self.gwd_text, title="[b]GWDEvents", border_style="green")
         )
         self.layout["snap0"].update(self.make_snapshot(self.scadas_to_snap[0]))
         self.layout["snap1"].update(self.make_snapshot(self.scadas_to_snap[1]))
         self.layout["sync"].update(self.sync_spinners.panel())
@@ -457,19 +471,34 @@
                 self.check_sync_queue()
 
     async def tui_task(self):
         await to_thread.run_sync(self.loop)
 
 
 class Header:
+    scadas: Sequence[str]
+
     """Display header with clock."""
 
+    def __init__(self, scadas: Optional[Sequence[str]] = None):
+        if scadas:
+            self.scadas = scadas[:]
+        else:
+            self.scadas = []
+
     # noinspection PyMethodMayBeStatic
     def __rich__(self) -> Panel:
         grid = Table.grid(expand=True)
         grid.add_column(justify="center", ratio=1)
         grid.add_column(justify="right")
+        title = "[b]Gridworks Events"
+        if self.scadas:
+            title += " from Scadas: "
+            for i, scada in enumerate(self.scadas):
+                title += scada
+                if i < len(self.scadas) - 1:
+                    title += ", "
         grid.add_row(
-            "[b]Gridworks Events",
+            title,
             datetime.now().ctime().replace(":", "[blink]:[/]"),
         )
         return Panel(grid, style="white on blue")
```

### Comparing `gridworks_debug_cli-0.2.5/PKG-INFO` & `gridworks_debug_cli-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-debug-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Gridworks Debug Cli
 Home-page: https://github.com/anschweitzer/gridworks-debug-cli
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

