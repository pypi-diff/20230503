# Comparing `tmp/interval_sdk-1.1.0.tar.gz` & `tmp/interval_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.1.0.tar", max compression
+gzip compressed data, was "interval_sdk-1.2.0.tar", max compression
```

## Comparing `interval_sdk-1.1.0.tar` & `interval_sdk-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.1.0/README.md
--rw-r--r--   0        0        0     1890 2023-04-24 18:28:48.134160 interval_sdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7024 2023-04-20 18:40:02.490552 interval_sdk-1.1.0/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    57635 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8151 2023-04-20 18:40:02.490552 interval_sdk-1.1.0/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.1.0/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     7891 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1290 2023-04-14 17:16:59.713107 interval_sdk-1.1.0/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.1.0/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.1.0/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.1.0/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    15208 2023-04-24 17:30:45.828290 interval_sdk-1.1.0/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25774 2023-04-24 17:47:34.107311 interval_sdk-1.1.0/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    65147 2023-04-24 18:36:10.017979 interval_sdk-1.1.0/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-14 17:16:59.716440 interval_sdk-1.1.0/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7193 2023-04-14 17:16:59.716440 interval_sdk-1.1.0/src/interval_sdk/util.py
--rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.1.0/setup.py
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/README.md
+-rw-r--r--   0        0        0     1890 2023-05-03 17:16:14.766804 interval_sdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7151 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    60224 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8178 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.2.0/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     7891 2023-04-24 17:19:39.837392 interval_sdk-1.2.0/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.2.0/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.2.0/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.2.0/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.2.0/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15318 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25838 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    65727 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.2.0/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.2.0/setup.py
+-rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.2.0/PKG-INFO
```

### Comparing `interval_sdk-1.1.0/pyproject.toml` & `interval_sdk-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.1.0"
+version = "1.2.0"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/component.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,34 +133,40 @@
             print("[Interval] Received invalid return value:", err, file=sys.stderr)
             self._fut.set_exception(err)
 
     async def set_state(self, value: Any):
         try:
             parsed = parse_obj_as(self.schema.state, dict_keys_to_snake(value))
             if self._handle_state_change:
-                self.instance.props = await self._handle_state_change(
-                    parsed,
-                    parse_obj_as(
-                        self.schema.props,
-                        dict_keys_to_snake(self.instance.props),
-                    ),
+                await self.set_props(
+                    await self._handle_state_change(
+                        parsed,
+                        parse_obj_as(
+                            self.schema.props,
+                            dict_keys_to_snake(self.instance.props),
+                        ),
+                    )
                 )
             elif parsed is not None:
                 print(
                     "[Interval] Received state, but no method was defined to handle.",
                     file=sys.stderr,
                 )
 
-            if self.on_state_change is not None:
-                # This is definitely callable?
-                # pylint: disable-next=not-callable
-                await self.on_state_change()
         except ValidationError as err:
             print("[Interval] Received invalid state:", value, err, file=sys.stderr)
 
+    async def set_props(self, value: Any):
+        self.instance.props = value
+
+        if self.on_state_change is not None:
+            # This is definitely callable?
+            # pylint: disable-next=not-callable
+            await self.on_state_change()
+
     def parse_return_value(self, value: Any):
         return_schema = self.schema.returns
         if self.instance.is_multiple:
             return_schema = list[return_schema]
         if self.instance.is_optional:
             return_schema = Optional[return_schema]
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/io.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import base64
+from inspect import isawaitable
 import sys
 from dataclasses import dataclass
 from datetime import date, datetime, time
 from typing import (
     Iterable,
     Mapping,
     Optional,
@@ -14,14 +15,19 @@
     Any,
     Callable,
     Awaitable,
 )
 from typing_extensions import Never
 from urllib.parse import ParseResult, urlparse
 
+from pydantic.fields import Undefined
+
+from interval_sdk.classes.logger import Logger
+from interval_sdk.superjson.transformer import UNDEFINED
+
 from ..io_schema import (
     ButtonItem,
     ButtonItemModel,
     CurrencyCode,
     DeserializableRecordModel,
     DisplayGridProps,
     DisplayGridState,
@@ -140,14 +146,15 @@
 MAX_FILE_SIZE_MB = 50
 
 
 class IO:
     @dataclass
     class Input:
         _renderer: ComponentRenderer
+        _logger: Logger
         _display_resolves_immediately: Optional[bool]
 
         def text(
             self,
             label: str,
             *,
             help_text: Optional[str] = None,
@@ -532,14 +539,15 @@
             return MultipleableIOPromise(
                 c, renderer=self._renderer, get_value=get_value
             )
 
     @dataclass
     class Select:
         _renderer: ComponentRenderer
+        _logger: Logger
         _display_resolves_immediately: Optional[bool]
 
         def table(
             self,
             label: str,
             *,
             data: Iterable[TR],
@@ -859,14 +867,15 @@
                 return [option_map[item.value] for item in val]
 
             return InputIOPromise(c, renderer=self._renderer, get_value=get_value)
 
     @dataclass
     class Display:
         _renderer: ComponentRenderer
+        _logger: Logger
         _display_resolves_immediately: Optional[bool]
 
         def code(
             self,
             label: str,
             *,
             code: str,
@@ -942,23 +951,74 @@
         def metadata(
             self,
             label: str,
             *,
             data: Iterable[MetaItemDefinition],
             layout: MetadataLayout = "grid",
         ) -> DisplayIOPromise[Literal["DISPLAY_METADATA"], None]:
+            eventual_props = ["value", "url", "image", "route", "params"]
+
+            new_data: list[MetaItemDefinition] = []
+            model_data: list[MetaItemDefinitionModel] = []
+
+            for item in data:
+                new_item: MetaItemDefinition = {"label": item["label"]}
+                model_item = MetaItemDefinitionModel(label=item["label"])
+
+                for prop in eventual_props:
+                    if prop in item:
+                        prop_val = item[prop]
+                        if callable(prop_val):
+                            prop_val = prop_val()
+
+                        new_item[prop] = prop_val
+
+                        if isawaitable(prop_val):
+                            model_item.__setattr__(prop, UNDEFINED)
+                        elif prop_val is not None:
+                            model_item.__setattr__(prop, prop_val)
+
+                new_data.append(new_item)
+                model_data.append(model_item)
+
             c = Component(
                 method_name="DISPLAY_METADATA",
                 label=label,
                 initial_props=DisplayMetadataProps(
                     layout=layout,
-                    data=[MetaItemDefinitionModel.parse_obj(item) for item in data],
+                    data=model_data,
                 ),
                 display_resolves_immediately=self._display_resolves_immediately,
             )
+
+            loop = asyncio.get_running_loop()
+            for i, item in enumerate(new_data):
+                for prop in eventual_props:
+                    if prop in item and isawaitable(item[prop]):
+
+                        async def handle_wait(
+                            item: MetaItemDefinition,
+                            prop: str,
+                            i: int,
+                        ):
+                            try:
+                                value = await item[prop]
+                                item[prop] = value
+                                model_data[i].__setattr__(prop, value)
+                                await c.set_props(
+                                    DisplayMetadataProps(layout=layout, data=model_data)
+                                )
+                            except Exception as err:
+                                self._logger.error(
+                                    f'Error updating metadata field "{prop}" with result from async task:',
+                                    err,
+                                )
+
+                        _task = loop.create_task(handle_wait(item, prop, i))
+
             return DisplayIOPromise(c, renderer=self._renderer)
 
         def object(
             self,
             label: str,
             *,
             data: KeyValueObject,
@@ -1285,14 +1345,15 @@
                 display_resolves_immediately=self._display_resolves_immediately,
             )
             return DisplayIOPromise(c, renderer=self._renderer)
 
     @dataclass
     class Experimental:
         _renderer: ComponentRenderer
+        _logger: Logger
         _display_resolves_immediately: Optional[bool]
 
         def spreadsheet(
             self,
             label: str,
             columns: dict[str, TypeValue],
             help_text: Optional[str] = None,
@@ -1310,40 +1371,51 @@
                     if default_value is not None
                     else None,
                 ),
                 display_resolves_immediately=self._display_resolves_immediately,
             )
             return InputIOPromise(c, renderer=self._renderer)
 
+    _logger: Logger
     _renderer: ComponentRenderer
     _display_resolves_immediately: Optional[bool]
     input: Input
     select: Select
     display: Display
     experimental: Experimental
 
     def __init__(
         self,
         renderer: ComponentRenderer,
         *,
+        logger: Logger,
         display_resolves_immediately: Optional[bool] = None,
     ):
+        self._logger = logger
         self._renderer = renderer
         self._display_resolves_immediately = display_resolves_immediately
         self.input = self.Input(
-            renderer, _display_resolves_immediately=display_resolves_immediately
+            renderer,
+            _logger=logger,
+            _display_resolves_immediately=display_resolves_immediately,
         )
         self.select = self.Select(
-            renderer, _display_resolves_immediately=display_resolves_immediately
+            renderer,
+            _logger=logger,
+            _display_resolves_immediately=display_resolves_immediately,
         )
         self.display = self.Display(
-            renderer, _display_resolves_immediately=display_resolves_immediately
+            renderer,
+            _logger=logger,
+            _display_resolves_immediately=display_resolves_immediately,
         )
         self.experimental = self.Experimental(
-            renderer, _display_resolves_immediately=display_resolves_immediately
+            renderer,
+            _logger=logger,
+            _display_resolves_immediately=display_resolves_immediately,
         )
 
     def confirm(
         self,
         label: str,
         help_text: Optional[str] = None,
     ) -> ExclusiveIOPromise[Literal["CONFIRM"], bool]:
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/io_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ):
         self._logger = logger
         self._send = send
         self._on_response_handlers = {}
 
         self.io = IO(
             self.render_components,
+            logger=logger,
             display_resolves_immediately=display_resolves_immediately,
         )
 
     @property
     def is_canceled(self) -> bool:
         return self._is_canceled
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/isocket.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/layout.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/layout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import json
 from dataclasses import dataclass
-from typing import Any, Callable, Optional, Union
+from typing import Optional
 
-from typing_extensions import Literal, TypeAlias, Awaitable
+from typing_extensions import Literal, TypeAlias
 
 from pydantic import Field
 
 from ..classes.io_promise import DisplayIOPromise
 from ..types import BaseModel
 from ..io_schema import ButtonItem, ButtonItemModel, IORender
-from ..util import dump_snake_obj, json_loads_camel, snake_to_camel
+from ..util import Eventual
 
 PageLayoutKey = Literal["title", "description", "children", "menuItems"]
 
 
 class PageError(BaseModel):
     layout_key: PageLayoutKey
     error: str
     message: str
     cause: Optional[str] = None
     stack: Optional[str] = None
 
 
-EventualStr: TypeAlias = Union[str, Awaitable[str], Callable[[], Awaitable[str]]]
+EventualStr: TypeAlias = Eventual[str]
 
 
 @dataclass
 class BasicLayout:
     kind: Literal["BASIC"] = "BASIC"
     title: Optional[EventualStr] = None
     description: Optional[EventualStr] = None
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/logger.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/page.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.2.0/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/components/grid.py` & `interval_sdk-1.2.0/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/components/table.py` & `interval_sdk-1.2.0/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/handlers.py` & `interval_sdk-1.2.0/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.2.0/src/interval_sdk/internal_rpc_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,14 +495,15 @@
 
 class PageContext:
     environment: ActionEnvironment
     user: ContextUser
     params: SerializableRecord
     organization: OrganizationDef
     page: PageInfo
+    loading: TransactionLoadingState
 
     _page_key: str
     _logger: Logger
     _send_redirect: Callable[[SendRedirectInputs], Awaitable[None]]
 
     def __init__(
         self,
@@ -510,24 +511,26 @@
         logger: Logger,
         environment: ActionEnvironment,
         user: ContextUser,
         params: SerializableRecord,
         organization: OrganizationDef,
         page: PageInfo,
         send_redirect: Callable[[SendRedirectInputs], Awaitable[None]],
+        loading: TransactionLoadingState,
     ):
         self._page_key = page_key
         self._logger = logger
         self._send_redirect = send_redirect
 
         self.environment = environment
         self.user = user
         self.params = params
         self.organization = organization
         self.page = page
+        self.loading = loading
 
     async def redirect(
         self,
         url: Optional[str] = None,
         route: Optional[str] = None,
         params: Optional[SerializableRecord] = None,
         replace: Optional[bool] = None,
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/io_schema.py` & `interval_sdk-1.2.0/src/interval_sdk/io_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from pydantic.fields import ModelField
 
 from .types import (
     BaseModel,
     GenericModel,
 )
 from .util import (
+    Eventual,
     ObjectLiteral,
     json_dumps_strip_none,
     json_loads_strip_none,
     Serializable,
     SerializableRecord,
 )
 
@@ -672,19 +673,19 @@
 
 
 MetadataLayout: TypeAlias = Literal["card", "list", "grid"]
 
 
 class MetaItemDefinition(TypedDict):
     label: str
-    value: NotRequired[Optional[ObjectLiteral]]
-    url: NotRequired[str]
-    image: NotRequired[ImageDefinition]
-    route: NotRequired[str]
-    params: NotRequired[SerializableRecord]
+    value: NotRequired[Optional[Eventual[ObjectLiteral]]]
+    url: NotRequired[Eventual[str]]
+    image: NotRequired[Eventual[ImageDefinition]]
+    route: NotRequired[Eventual[str]]
+    params: NotRequired[Eventual[SerializableRecord]]
 
 
 class MetaItemDefinitionModel(BaseModel):
     label: str
     value: Optional[ObjectLiteral] = None
     url: Optional[str] = None
     image: Optional[ImageDefinitionModel] = None
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/main.py` & `interval_sdk-1.2.0/src/interval_sdk/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1057,27 +1057,41 @@
 
             try:
                 page_handler = self._page_handlers[inputs.page.slug]
             except KeyError:
                 self._logger.error("No page handler found for slug", inputs.page.slug)
                 return OpenPageReturnsError(message="No page handler found.")
 
+            async def send_loading_state(loading_state: LoadingState):
+                self._transaction_loading_states[inputs.page_key] = loading_state
+                await self._send(
+                    "SEND_LOADING_CALL",
+                    SendLoadingCallInputs(
+                        transaction_id=inputs.page_key,
+                        **loading_state.dict(),
+                    ).dict(),
+                )
+
             params = inputs.params
             if params is not None and inputs.params_meta is not None:
                 params = superjson.deserialize(params, inputs.params_meta)
 
             page_ctx = PageContext(
                 page_key=inputs.page_key,
                 logger=self._logger,
                 user=inputs.user,
                 params=deserialize_dates(inputs.params),
                 environment=inputs.environment,
                 organization=self.organization,
                 page=inputs.page,
                 send_redirect=self._send_redirect,
+                loading=TransactionLoadingState(
+                    logger=self._logger,
+                    sender=send_loading_state,
+                ),
             )
 
             page: Optional[Layout] = None
             menu_items: Optional[list[ButtonItemModel]] = None
             render_instruction: Optional[IORender] = None
             errors: list[PageError] = []
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/superjson/main.py` & `interval_sdk-1.2.0/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.2.0/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.2.0/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.2.0/src/interval_sdk/superjson/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math, re
 from datetime import date, time, datetime, timezone
 from typing import Any, Callable, Union
 from typing_extensions import TypeAlias, Literal
 
-LeafTypeAnnotation: TypeAlias = Literal["number", "Date", "regexp", "set", "map"]
+LeafTypeAnnotation: TypeAlias = Literal[
+    "number", "Date", "regexp", "set", "map", "undefined"
+]
 
 CustomTypeAnnotation: TypeAlias = tuple[Literal["custom"], str]
 
 CompositeTypeAnnotation: TypeAlias = CustomTypeAnnotation
 
 TypeAnnotation: TypeAlias = Union[LeafTypeAnnotation, CompositeTypeAnnotation]
 
@@ -15,15 +17,24 @@
 
 REGEXP_FLAGS = {
     "i": re.I,
     "m": re.M,
 }
 
 
+class Undefined:
+    pass
+
+
+UNDEFINED = Undefined()
+
+
 def transform_value(value: Any) -> Union[tuple[Any, TypeAnnotation], None]:
+    if isinstance(value, Undefined):
+        return (None, "undefined")
     if isinstance(value, float):
         if math.isinf(value):
             return ("Infinity", "number")
         if math.isnan(value):
             return ("NaN", "number")
 
     if isinstance(value, re.Pattern):
```

### Comparing `interval_sdk-1.1.0/src/interval_sdk/types.py` & `interval_sdk-1.2.0/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.1.0/src/interval_sdk/util.py` & `interval_sdk-1.2.0/src/interval_sdk/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 import json, re
-from typing import Any, Iterable, Mapping, Optional, Tuple, Callable, Union, cast
+from typing import (
+    Any,
+    Awaitable,
+    Iterable,
+    Mapping,
+    Optional,
+    Tuple,
+    Callable,
+    Union,
+    cast,
+)
 from datetime import date, time, datetime
 from typing_extensions import TypeAlias, TypeVar
 from time import time_ns
 
 from pydantic import StrictBool, StrictFloat, StrictInt
 
 
@@ -170,14 +180,18 @@
 
 
 def json_loads_strip_none(*args, **kwargs) -> Any:
     obj = json.loads(*args, **kwargs)
     return dict_strip_none(obj)
 
 
+Eventual: TypeAlias = Union[
+    T, Awaitable[T], Callable[[], T], Callable[[], Awaitable[T]]
+]
+
 Deserializable: TypeAlias = Union[int, float, bool, None, str]
 DeserializableRecord: TypeAlias = Mapping[str, Deserializable]
 Serializable: TypeAlias = Union[bool, int, float, datetime, date, time, str, None]
 SerializableRecord: TypeAlias = Mapping[str, Serializable]
 
 ObjectLiteral: TypeAlias = Union[
     StrictInt, StrictFloat, StrictBool, datetime, date, time, None, str
```

