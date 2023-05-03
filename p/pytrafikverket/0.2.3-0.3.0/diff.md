# Comparing `tmp/pytrafikverket-0.2.3.tar.gz` & `tmp/pytrafikverket-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrafikverket-0.2.3.tar", last modified: Sat Jan 21 12:28:36 2023, max compression
+gzip compressed data, was "pytrafikverket-0.3.0.tar", last modified: Wed May  3 20:20:24 2023, max compression
```

## Comparing `pytrafikverket-0.2.3.tar` & `pytrafikverket-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-01-21 12:28:36.428039 pytrafikverket-0.2.3/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2022-09-16 18:25:00.000000 pytrafikverket-0.2.3/LICENSE
--rw-r--r--   0 gjo       (1000) gjo       (1000)      287 2023-01-21 12:28:36.428039 pytrafikverket-0.2.3/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2098 2023-01-21 12:28:11.000000 pytrafikverket-0.2.3/README.md
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-01-21 12:28:36.428039 pytrafikverket-0.2.3/pytrafikverket/
--rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2022-10-08 12:23:24.000000 pytrafikverket-0.2.3/pytrafikverket/__init__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     6386 2023-01-21 12:28:11.000000 pytrafikverket-0.2.3/pytrafikverket/__main__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     7774 2022-09-16 18:25:00.000000 pytrafikverket-0.2.3/pytrafikverket/trafikverket.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     3495 2022-10-08 12:23:24.000000 pytrafikverket-0.2.3/pytrafikverket/trafikverket_camera.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     9187 2022-09-16 18:25:00.000000 pytrafikverket-0.2.3/pytrafikverket/trafikverket_ferry.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)    11588 2023-01-21 12:28:11.000000 pytrafikverket-0.2.3/pytrafikverket/trafikverket_train.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     4489 2022-10-08 09:45:40.000000 pytrafikverket-0.2.3/pytrafikverket/trafikverket_weather.py
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-01-21 12:28:36.428039 pytrafikverket-0.2.3/pytrafikverket.egg-info/
--rw-r--r--   0 gjo       (1000) gjo       (1000)      287 2023-01-21 12:28:36.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)      494 2023-01-21 12:28:36.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/SOURCES.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-01-21 12:28:36.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/dependency_links.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-01-21 12:28:36.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/requires.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-01-21 12:28:36.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/top_level.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2022-10-08 12:25:41.000000 pytrafikverket-0.2.3/pytrafikverket.egg-info/zip-safe
--rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-01-21 12:28:36.428039 pytrafikverket-0.2.3/setup.cfg
--rw-r--r--   0 gjo       (1000) gjo       (1000)      566 2023-01-21 12:28:11.000000 pytrafikverket-0.2.3/setup.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.0/LICENSE
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.0/README.md
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/pytrafikverket/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.0/pytrafikverket/__init__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/__main__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/pytrafikverket/exceptions.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/py.typed
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_camera.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_ferry.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)    12091 2023-05-03 20:07:04.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_train.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     7315 2023-05-03 20:07:04.000000 pytrafikverket-0.3.0/pytrafikverket/trafikverket_weather.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/pytrafikverket.egg-info/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/SOURCES.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/dependency_links.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/requires.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/top_level.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.0/pytrafikverket.egg-info/zip-safe
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-03 20:20:24.230394 pytrafikverket-0.3.0/setup.cfg
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-03 20:18:05.000000 pytrafikverket-0.3.0/setup.py
```

### Comparing `pytrafikverket-0.2.3/LICENSE` & `pytrafikverket-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.2.3/README.md` & `pytrafikverket-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # pytrafikverket
 python module for communicating with the swedish trafikverket api
 
+Development and testing done with 3.10
+
 ## Code example
 ```python
 from pytrafikverket import TrafikverketTrain, StationInfo
 import aiohttp
 import asyncio
 import async_timeout
 from datetime import datetime
```

### Comparing `pytrafikverket-0.2.3/pytrafikverket/__init__.py` & `pytrafikverket-0.3.0/pytrafikverket/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.2.3/pytrafikverket/__main__.py` & `pytrafikverket-0.3.0/pytrafikverket/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """CLI enabler for pytrafikverket."""
+from __future__ import annotations
+
 import argparse
 import asyncio
 from datetime import datetime
+from typing import Any
 
+import json
 import aiohttp
 import async_timeout
 
 from pytrafikverket.trafikverket_train import TrafikverketTrain
 from pytrafikverket.trafikverket_weather import TrafikverketWeather
 from pytrafikverket.trafikverket_ferry import TrafikverketFerry
-import json
 
 SEARCH_FOR_STATION = "search-for-station"
 GET_TRAIN_STOP = "get-train-stop"
 GET_NEXT_TRAIN_STOP = "get-next-train-stop"
 GET_WEATHER = "get-weather"
 GET_FERRY_ROUTE = "get-ferry-route"
 SEARCH_FOR_FERRY_ROUTE = "search-for-ferry-route"
 GET_NEXT_FERRY_STOP = "get-next-ferry-stop"
 DATE_TIME_INPUT = "%Y-%m-%dT%H:%M:%S"
 
 
-async def async_main(loop):
+async def async_main(loop: Any) -> None:
     """Set up function to handle input and get data to present."""
     async with aiohttp.ClientSession(loop=loop) as session:
         parser = argparse.ArgumentParser(
             description="CLI used to get data from trafikverket"
         )
         parser.add_argument("-key", type=str, required=True)
         parser.add_argument(
@@ -69,16 +72,16 @@
                 for station in stations:
                     print_values(station)
             elif args.method == GET_TRAIN_STOP:
                 from_station = await train_api.async_get_train_station(
                     args.from_station
                 )
                 to_station = await train_api.async_get_train_station(args.to_station)
-                print("from_station_signature: " + from_station.signature)
-                print("to_station_signature:   " + to_station.signature)
+                print(f"from_station_signature: {from_station.signature}")
+                print(f"to_station_signature:   {to_station.signature}")
 
                 time = datetime.strptime(args.date_time, DATE_TIME_INPUT)
 
                 train_stop = await train_api.async_get_train_stop(
                     from_station,
                     to_station,
                     time,
@@ -88,16 +91,16 @@
                 print_values(train_stop)
 
             elif args.method == GET_NEXT_TRAIN_STOP:
                 from_station = await train_api.async_get_train_station(
                     args.from_station
                 )
                 to_station = await train_api.async_get_train_station(args.to_station)
-                print("from_station_signature: " + from_station.signature)
-                print("to_station_signature:   " + to_station.signature)
+                print(f"from_station_signature: {from_station.signature}")
+                print(f"to_station_signature:   {to_station.signature}")
 
                 if args.date_time is not None:
                     time = datetime.strptime(args.date_time, DATE_TIME_INPUT)
                 else:
                     time = datetime.now()
                 train_stop = await train_api.async_get_next_train_stop(
                     from_station,
@@ -128,15 +131,15 @@
 
             elif args.method == SEARCH_FOR_FERRY_ROUTE:
                 if args.route is None:
                     raise ValueError("-route is required")
                 routes = await ferry_api.async_search_ferry_routes(args.route)
                 for route in routes:
                     print_values(route)
-                    print(route.name + " " + route.id)
+                    print(f"{route.name} {route.id}")
 
             elif args.method == GET_NEXT_FERRY_STOP:
                 if args.from_harbor is None:
                     raise ValueError(
                         '-from-harbor is required with name of Ferry harbor\
                          (ex. -from-harbor "Ekerö")'
                     )
@@ -147,16 +150,16 @@
 
                 ferry_stop = await ferry_api.async_get_next_ferry_stop(
                     args.from_harbor, args.to_harbor, time
                 )
                 print_values(ferry_stop)
 
 
-def print_values(object):
+def print_values(result: Any) -> None:
     """Print out values for all object members."""
-    print(json.dumps(object.__dict__, indent=4, ensure_ascii=False))
+    print(json.dumps(result.__dict__, indent=4, ensure_ascii=False))
 
 
-def main():
+def main() -> None:
     """Initialize the loop."""
     loop = asyncio.get_event_loop()
     loop.run_until_complete(async_main(loop))
```

### Comparing `pytrafikverket-0.2.3/pytrafikverket/trafikverket.py` & `pytrafikverket-0.3.0/pytrafikverket/trafikverket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,161 +1,163 @@
 """Module for communication with Trafikverket official API."""
-import typing
+from __future__ import annotations
+
+from typing import Any, cast
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 from enum import Enum
 
 import aiohttp
 from lxml import etree
 
+from .exceptions import InvalidAuthentication, UnknownError
 
 class FilterOperation(Enum):
     """Contains all field filter operations."""
 
-    equal = "EQ"
-    exists = "EXISTS"
-    greater_than = "GT"
-    greater_than_equal = "GTE"
-    less_than = "LT"
-    less_than_equal = "LTE"
-    not_equal = "NE"
-    like = "LIKE"
-    not_like = "NOTLIKE"
-    #    in = "IN"
-    not_in = "NOTIN"
-    with_in = "WITHIN"
+    EQUAL = "EQ"
+    EXISTS = "EXISTS"
+    GREATER_THAN = "GT"
+    GREATER_THAN_EQUAL = "GTE"
+    LESS_THAN = "LT"
+    LESS_THAN_EQUAL = "LTE"
+    NOT_EQUAL = "NE"
+    LIKE = "LIKE"
+    NOT_LIKE = "NOTLIKE"
+    #    IN = "IN"
+    NOT_IN = "NOTIN"
+    WITH_IN = "WITHIN"
 
 
 class SortOrder(Enum):
     """Specifies how rows of data are sorted."""
 
-    ascending = "asc"
-    decending = "desc"
+    ASCENDING = "asc"
+    DECENDING = "desc"
 
 
 class FieldSort:
     """What field and how to sort on it."""
 
-    def __init__(self, field: str, sort_order: SortOrder):
+    def __init__(self, field: str, sort_order: SortOrder) -> None:
         """Initialize the class."""
         self._field = field
         self._sort_order = sort_order
 
-    def to_string(self):
+    def to_string(self) -> str:
         """Sort_order as string."""
         return self._field + " " + self._sort_order.value
 
 
 class Filter:
     """Base class for all filters."""
 
     __metaclass__ = ABCMeta
 
     @abstractmethod
-    def generate_node(self, parent_node):
+    def generate_node(self, parent_node: Any) -> Any:
         """Generate node."""
-        pass
 
 
 class FieldFilter(Filter):
     """Used to filter on one field."""
 
-    def __init__(self, operation: FilterOperation, name, value):
+    def __init__(self, operation: FilterOperation, name: str, value: Any) -> None:
         """Initialize the class."""
         self.operation = operation
         self.name = name
         self.value = value
 
-    def generate_node(self, parent_node):
+    def generate_node(self, parent_node: Any) -> Any:
         """Return element node for field filter."""
         filter_node = etree.SubElement(parent_node, self.operation.value)
         filter_node.attrib["name"] = self.name
         filter_node.attrib["value"] = self.value
         return filter_node
 
 
 class OrFilter(Filter):
     """Used to create a Or filter."""
 
-    def __init__(self, filters: typing.List[Filter]):
+    def __init__(self, filters: list[Filter]) -> None:
         """Initialize the class."""
         self.filters = filters
 
-    def generate_node(self, parent_node):
+    def generate_node(self, parent_node: Any) -> Any:
         """Return element node for filter."""
         or_node = etree.SubElement(parent_node, "OR")
         for sub_filter in self.filters:
             sub_filter.generate_node(or_node)
         return or_node
 
 
 class AndFilter(Filter):
     """Used to create a And filter."""
 
-    def __init__(self, filters: typing.List[Filter]):
+    def __init__(self, filters: list[Filter]) -> None:
         """Initialize the class."""
         self.filters = filters
 
-    def generate_node(self, parent_node):
+    def generate_node(self, parent_node: Any) -> Any:
         """Return element node for filter."""
         or_node = etree.SubElement(parent_node, "AND")
         for sub_filter in self.filters:
             sub_filter.generate_node(or_node)
         return or_node
 
 
-class Trafikverket(object):
+class Trafikverket:
     """Class used to communicate with trafikverket api."""
 
     _api_url = "https://api.trafikinfo.trafikverket.se/v2/data.xml"
     date_time_format = "%Y-%m-%dT%H:%M:%S.%f%z"
     date_time_format_for_modified = "%Y-%m-%dT%H:%M:%S.%fZ"
 
-    def __init__(self, client_session: aiohttp.ClientSession, api_key: str):
+    def __init__(self, client_session: aiohttp.ClientSession, api_key: str) -> None:
         """Initialize TrafikInfo object."""
         self._client_session = client_session
         self._api_key = api_key
 
     def _generate_request_data(
         self,
         objecttype: str,
         schemaversion: str,
-        includes: typing.List[str],
-        filters: typing.List[Filter],
-        limit: int = None,
-        sorting: typing.List[FieldSort] = None,
-    ):
+        includes: list[str],
+        filters: list[Filter],
+        limit: int | None = None,
+        sorting: list[FieldSort] | None = None,
+    ) -> Any:
         root_node = etree.Element("REQUEST")
         login_node = etree.SubElement(root_node, "LOGIN")
         login_node.attrib["authenticationkey"] = self._api_key
         query_node = etree.SubElement(root_node, "QUERY")
         query_node.attrib["objecttype"] = objecttype
         query_node.attrib["schemaversion"] = schemaversion
         if limit is not None:
             query_node.attrib["limit"] = str(limit)
         if sorting is not None and len(sorting) > 0:
             query_node.attrib["orderby"] = ", ".join([fs.to_string() for fs in sorting])
         for include in includes:
             include_node = etree.SubElement(query_node, "INCLUDE")
             include_node.text = include
         filters_node = etree.SubElement(query_node, "FILTER")
-        for filter in filters:
-            filter.generate_node(filters_node)
+        for _filter in filters:
+            _filter.generate_node(filters_node)
 
         return root_node
 
     async def async_make_request(
         self,
         objecttype: str,
         schemaversion: str,
-        includes: typing.List[str],
-        filters: typing.List[Filter],
-        limit: int = None,
-        sorting: typing.List[FieldSort] = None,
-    ):
+        includes: list[str],
+        filters: list[Filter | FieldFilter],
+        limit: int | None = None,
+        sorting: list[FieldSort] | None = None,
+    ) -> Any:
         """Send request to trafikverket api and return a element node."""
         request_data = self._generate_request_data(
             objecttype, schemaversion, includes, filters, limit, sorting
         )
         request_data_text = etree.tostring(request_data, pretty_print=False)
         headers = {"content-type": "text/xml"}
         async with self._client_session.post(
@@ -164,48 +166,63 @@
             content = await response.text()
             error_nodes = etree.fromstring(content).xpath("/RESPONSE/RESULT/ERROR")
             if len(error_nodes) > 0:
                 error_node = error_nodes[0]
                 helper = NodeHelper(error_node)
                 source = helper.get_text("SOURCE")
                 message = helper.get_text("MESSAGE")
-                raise ValueError("Source: " + source + ", message: " + message)
+                if response.status == 401:
+                    raise InvalidAuthentication(f"Source: {source}, message: {message}, status: {response.status}")
+                raise UnknownError(f"Source: {source}, message: {message}, status: {response.status}")
 
             return etree.fromstring(content).xpath("/RESPONSE/RESULT/" + objecttype)
 
 
-class NodeHelper(object):
+class NodeHelper:
     """Helper class to get node content."""
 
-    def __init__(self, node):
+    def __init__(self, node: Any) -> None:
         """Initialize the class."""
         self._node = node
 
-    def get_text(self, field):
+    def get_text(self, field: str) -> str | None:
         """Return the text in 'field' from the node or None if not found."""
         nodes = self._node.xpath(field)
         if nodes is None:
             return None
         if len(nodes) == 0:
             return None
         if len(nodes) > 1:
             raise ValueError("Found multiple nodes should only 0 or 1 is allowed")
-        return nodes[0].text
+        value = nodes[0].text
+        return cast(str, value)
+
+    def get_number(self, field: str) -> float | None:
+        """Return the number in 'field' from the node or None if not found."""
+        nodes = self._node.xpath(field)
+        if nodes is None:
+            return None
+        if len(nodes) == 0:
+            return None
+        if len(nodes) > 1:
+            raise ValueError("Found multiple nodes should only 0 or 1 is allowed")
+        value = nodes[0].text
+        return cast(float, value)
 
-    def get_texts(self, field):
+    def get_texts(self, field: str) -> list[str] | None:
         """Return a list of texts from the node selected by 'field' or None."""
         nodes = self._node.xpath(field)
         if nodes is None:
             return None
-        result = [str] * 0
+        result = []
         for line in nodes:
             result.append(line.text)
         return result
 
-    def get_datetime_for_modified(self, field):
+    def get_datetime_for_modified(self, field: str) -> datetime | None:
         """Return datetime object from node, selected by 'field'.
 
         Format of the text is expected to be modifiedTime-format.
         """
         nodes = self._node.xpath(field)
         if nodes is None:
             return None
@@ -213,28 +230,29 @@
             return None
         if len(nodes) > 1:
             raise ValueError("Found multiple nodes should only 0 or 1 is allowed")
         return datetime.strptime(
             nodes[0].text, Trafikverket.date_time_format_for_modified
         )
 
-    def get_datetime(self, field):
+    def get_datetime(self, field: str) -> datetime | None:
         """Return a datetime object from node, selected by 'field'."""
         nodes = self._node.xpath(field)
         if nodes is None:
             return None
         if len(nodes) == 0:
             return None
         if len(nodes) > 1:
             raise ValueError("Found multiple nodes should only 0 or 1 is allowed")
         return datetime.strptime(nodes[0].text, Trafikverket.date_time_format)
 
-    def get_bool(self, field):
+    def get_bool(self, field: str) -> bool:
         """Return True if value selected by field is 'true' else returns False."""
-        nodes = self._node.xpath(field)
+        nodes: etree.XPath = self._node.xpath(field)
         if nodes is None:
             return False
         if len(nodes) == 0:
             return False
         if len(nodes) > 1:
             raise ValueError("Found multiple nodes should only 0 or 1 is allowed")
-        return nodes[0].text.lower() == "true"
+        value = nodes[0].text.lower() == "true"
+        return cast(bool, value)
```

### Comparing `pytrafikverket-0.2.3/pytrafikverket/trafikverket_camera.py` & `pytrafikverket-0.3.0/pytrafikverket/trafikverket_camera.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Retrieve camera data from Trafikverket API."""
+from __future__ import annotations
+
+from typing import Any
 
 from datetime import datetime
 import aiohttp
 from pytrafikverket.trafikverket import (
     FieldFilter,
     FilterOperation,
     NodeHelper,
     Trafikverket,
 )
 
+from .exceptions import NoCameraFound, MultipleCamerasFound
+
 
 class CameraInfo:
     """Fetch Camera data."""
 
     _required_fields = [
         "Name",
         "Id",
@@ -27,27 +32,27 @@
         "PhotoUrl",
         "Status",
         "Type",
     ]
 
     def __init__(
         self,
-        camera_name: str,
-        camera_id: str,
+        camera_name: str | None,
+        camera_id: str | None,
         active: bool,
         deleted: bool,
-        description: str,
-        direction: str,
+        description: str | None,
+        direction: str | None,
         fullsizephoto: bool,
-        location: str,
-        modified: datetime,
-        phototime: datetime,
-        photourl: str,
-        status: str,
-        camera_type: str,
+        location: str | None,
+        modified: datetime | None,
+        phototime: datetime | None,
+        photourl: str | None,
+        status: str | None,
+        camera_type: str | None,
     ) -> None:
         """Initialize the class."""
         self.camera_name = camera_name
         self.camera_id = camera_id
         self.active = active
         self.deleted = deleted
         self.description = description
@@ -57,15 +62,15 @@
         self.modified = modified
         self.phototime = phototime
         self.photourl = photourl
         self.status = status
         self.camera_type = camera_type
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> CameraInfo:
         """Map XML path for values."""
         node_helper = NodeHelper(node)
         camera_name = node_helper.get_text("Name")
         camera_id = node_helper.get_text("Id")
         active = node_helper.get_bool("Active")
         deleted = node_helper.get_bool("Deleted")
         description = node_helper.get_text("Description")
@@ -103,15 +108,15 @@
 
     async def async_get_camera(self, location_name: str) -> CameraInfo:
         """Retrieve camera from API."""
         cameras = await self._api.async_make_request(
             "Camera",
             "1.0",
             CameraInfo._required_fields,  # pylint: disable=protected-access
-            [FieldFilter(FilterOperation.equal, "Name", location_name)],
+            [FieldFilter(FilterOperation.EQUAL, "Name", location_name)],
         )
         if len(cameras) == 0:
-            raise ValueError("Could not find a camera with the specified name")
+            raise NoCameraFound("Could not find a camera with the specified name")
         if len(cameras) > 1:
-            raise ValueError("Found multiple camera with the specified name")
+            raise MultipleCamerasFound("Found multiple camera with the specified name")
 
         return CameraInfo.from_xml_node(cameras[0])
```

### Comparing `pytrafikverket-0.2.3/pytrafikverket/trafikverket_ferry.py` & `pytrafikverket-0.3.0/pytrafikverket/trafikverket_ferry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,104 +1,122 @@
 """Enables retreival of ferry departure information from Trafikverket API."""
+from __future__ import annotations
+
+from typing import Any
 
-import typing
 from datetime import datetime
 from enum import Enum
-from typing import List
 
 import aiohttp
 from pytrafikverket.trafikverket import (
+    Filter,
     FieldFilter,
     FieldSort,
     FilterOperation,
     NodeHelper,
     SortOrder,
     Trafikverket,
 )
 
+from .exceptions import (
+    NoRouteFound,
+    MultipleRoutesFound,
+    NoFerryFound,
+    NoDeviationFound,
+    MultipleDeviationsFound,
+)
+
+# pylint: disable=W0622, C0103
 
-class RouteInfo(object):
+
+class RouteInfo:
     """Contains information about a FerryRoute."""
 
     _required_fields = ["Id", "Name", "Shortname", "Type.Name"]
 
-    def __init__(self, id: str, name: str, short_name: str, route_type: str):
+    def __init__(
+        self,
+        id: str | None,
+        name: str | None,
+        short_name: str | None,
+        route_type: str | None,
+    ) -> None:
         """Initialize RouteInfo class."""
         self.id = id
         self.name = name
         self.short_name = short_name
         self.route_type = route_type
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> RouteInfo:
         """Map route information in XML data."""
         node_helper = NodeHelper(node)
         id = node_helper.get_text("Id")
         name = node_helper.get_text("Name")
         short_name = node_helper.get_text("Shortname")
         route_type = node_helper.get_text("Type/Name")
 
         return cls(id, name, short_name, route_type)
 
 
-class DeviationInfo(object):
+class DeviationInfo:
     """Contains information about a Situation/Deviation."""
 
     _required_fields = [
         "Deviation.Id",
         "Deviation.Header",
         "Deviation.EndTime",
         "Deviation.StartTime",
         "Deviation.Message",
         "Deviation.IconId",
         "Deviation.LocationDescriptor",
     ]
 
     def __init__(
         self,
-        id: str,
-        header: str,
-        message: str,
-        start_time: datetime,
-        end_time: datetime,
-        icon_id: str,
-        location_desc: str,
-    ):
+        id: str | None,
+        header: str | None,
+        message: str | None,
+        start_time: datetime | None,
+        end_time: datetime | None,
+        icon_id: str | None,
+        location_desc: str | None,
+    ) -> None:
         """Initialize DeviationInfo class."""
         self.id = id
         self.header = header
         self.message = message
         self.start_time = start_time
         self.end_time = end_time
         self.icon_id = icon_id
         self.location_desc = location_desc
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> DeviationInfo:
         """Map deviation information in XML data."""
         node_helper = NodeHelper(node)
         id = node_helper.get_text("Deviation/Id")
         header = node_helper.get_text("Deviation/Header")
         message = node_helper.get_text("Deviation/Message")
-        start_time = node_helper.get_text("Deviation/StartTime")
-        end_time = node_helper.get_text("Deviation/EndTime")
+        start_time = node_helper.get_datetime("Deviation/StartTime")
+        end_time = node_helper.get_datetime("Deviation/EndTime")
         icon_id = node_helper.get_text("Deviation/IconId")
         location_desc = node_helper.get_text("Deviation/LocationDescriptor")
-        return cls(id, header, message, start_time, end_time,
-                   icon_id, location_desc)
+        return cls(id, header, message, start_time, end_time, icon_id, location_desc)
 
 
 class FerryStopStatus(Enum):
     """Contain the different ferry stop statuses."""
 
-    on_time = "scheduled to arrive on schedule"
-    canceled = "canceled"
+    ON_TIME = "on_time"
+    CANCELED = "canceled"
+    DELETED = "deleted"
 
 
-class FerryStop(object):
+class FerryStop:
     """Contain information about a ferry departure."""
 
     _required_fields = [
         "Id",
         "Deleted",
         "DepartureTime",
         "Route.Name",
@@ -107,41 +125,41 @@
         "FromHarbor",
         "ToHarbor",
         "Info",
     ]
 
     def __init__(
         self,
-        id,
+        id: str | None,
         deleted: bool,
-        departure_time: datetime,
-        other_information: typing.List[str],
-        deviation_id: str,
-        modified_time: datetime,
-        from_harbor_name: str,
-        to_harbor_name: str,
-    ):
+        departure_time: datetime | None,
+        other_information: list[str] | None,
+        deviation_id: list[str] | None,
+        modified_time: datetime | None,
+        from_harbor_name: str | None,
+        to_harbor_name: str | None,
+    ) -> None:
         """Initialize FerryStop."""
         self.id = id
         self.deleted = deleted
         self.departure_time = departure_time
         self.other_information = other_information
         self.deviation_id = deviation_id
         self.modified_time = modified_time
         self.from_harbor_name = from_harbor_name
         self.to_harbor_name = to_harbor_name
 
     def get_state(self) -> FerryStopStatus:
         """Retrieve the state of the departure."""
         if self.deleted:
-            return FerryStopStatus.deleted
-        return FerryStopStatus.on_time
+            return FerryStopStatus.DELETED
+        return FerryStopStatus.ON_TIME
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> FerryStop:
         """Map the path in the return XML data."""
         node_helper = NodeHelper(node)
         id = node_helper.get_text("Id")
         deleted = node_helper.get_bool("Deleted")
         departure_time = node_helper.get_datetime("DepartureTime")
         other_information = node_helper.get_texts("Info")
         deviation_id = node_helper.get_texts("DeviationId")
@@ -157,102 +175,102 @@
             deviation_id,
             modified_time,
             from_harbor_name,
             to_harbor_name,
         )
 
 
-class TrafikverketFerry(object):
+class TrafikverketFerry:
     """Class used to communicate with trafikverket's ferry route api."""
 
-    def __init__(self, client_session: aiohttp.ClientSession, api_key: str):
+    def __init__(self, client_session: aiohttp.ClientSession, api_key: str) -> None:
         """Initialize FerryInfo object."""
         self._api = Trafikverket(client_session, api_key)
 
     async def async_get_ferry_route(self, route_name: str) -> RouteInfo:
         """Retreive ferry route id based on name."""
         routes = await self._api.async_make_request(
             "FerryRoute",
             "1.2",
-            RouteInfo._required_fields,
-            [FieldFilter(FilterOperation.equal, "Name", route_name)],
+            RouteInfo._required_fields,  # pylint: disable=protected-access
+            [FieldFilter(FilterOperation.EQUAL, "Name", route_name)],
         )
         if len(routes) == 0:
-            raise ValueError("Could not find a route with the specified name")
+            raise NoRouteFound("Could not find a route with the specified name")
         if len(routes) > 1:
-            raise ValueError("Found multiple routes with the specified name")
+            raise MultipleRoutesFound("Found multiple routes with the specified name")
 
         return RouteInfo.from_xml_node(routes[0])
 
     async def async_get_ferry_route_id(self, route_id: int) -> RouteInfo:
         """Retreive ferry route id based on routeId."""
         routes = await self._api.async_make_request(
             "FerryRoute",
             "1.2",
-            RouteInfo._required_fields,
-            [FieldFilter(FilterOperation.equal, "Id", str(route_id))],
+            RouteInfo._required_fields,  # pylint: disable=protected-access
+            [FieldFilter(FilterOperation.EQUAL, "Id", str(route_id))],
         )
         if len(routes) == 0:
-            raise ValueError("Could not find a route with the specified name")
+            raise NoRouteFound("Could not find a route with the specified name")
         if len(routes) > 1:
-            raise ValueError("Found multiple routes with the specified name")
+            raise MultipleRoutesFound("Found multiple routes with the specified name")
 
         return RouteInfo.from_xml_node(routes[0])
 
-    async def async_search_ferry_routes(self, name: str) -> typing.List[RouteInfo]:
+    async def async_search_ferry_routes(self, name: str) -> list[RouteInfo]:
         """Search for ferry routes based on the route name."""
         routes = await self._api.async_make_request(
             "FerryRoute",
             "1.2",
-            RouteInfo._required_fields,
-            [FieldFilter(FilterOperation.like, "Name", name)],
+            RouteInfo._required_fields,  # pylint: disable=protected-access
+            [FieldFilter(FilterOperation.LIKE, "Name", name)],
         )
         if len(routes) == 0:
-            raise ValueError("Could not find a ferry route with the specified name")
+            raise NoRouteFound("Could not find a ferry route with the specified name")
 
-        result = [RouteInfo] * 0
+        result = []
 
         for route in routes:
             result.append(RouteInfo.from_xml_node(route))
 
         return result
 
     async def async_get_next_ferry_stops(
         self,
         from_harbor_name: str,
         to_harnbor_name: str = "",
         after_time: datetime = datetime.now(),
         number_of_stops: int = 1,
-    ) -> List[FerryStop]:
+    ) -> list[FerryStop]:
         """Enable retreival of next departures."""
         date_as_text = after_time.strftime(Trafikverket.date_time_format)
 
-        filters = [
-            FieldFilter(FilterOperation.equal, "FromHarbor.Name", from_harbor_name),
+        filters: list[FieldFilter | Filter] = [
+            FieldFilter(FilterOperation.EQUAL, "FromHarbor.Name", from_harbor_name),
             FieldFilter(
-                FilterOperation.greater_than_equal, "DepartureTime", date_as_text
+                FilterOperation.GREATER_THAN_EQUAL, "DepartureTime", date_as_text
             ),
         ]
         if to_harnbor_name:
             filters.append(
-                FieldFilter(FilterOperation.equal, "ToHarbor.Name", to_harnbor_name)
+                FieldFilter(FilterOperation.EQUAL, "ToHarbor.Name", to_harnbor_name)
             )
 
-        sorting = [FieldSort("DepartureTime", SortOrder.ascending)]
+        sorting = [FieldSort("DepartureTime", SortOrder.ASCENDING)]
         ferry_announcements = await self._api.async_make_request(
             "FerryAnnouncement",
             "1.2",
-            FerryStop._required_fields,
+            FerryStop._required_fields,  # pylint: disable=protected-access
             filters,
             number_of_stops,
             sorting,
         )
 
         if len(ferry_announcements) == 0:
-            raise ValueError("No FerryAnnouncement found")
+            raise NoFerryFound("No FerryAnnouncement found")
 
         stops = []
         for announcement in ferry_announcements:
             stops.append(FerryStop.from_xml_node(announcement))
         return stops
 
     async def async_get_next_ferry_stop(
@@ -265,19 +283,24 @@
         stops = await self.async_get_next_ferry_stops(
             from_harbor_name, to_harnbor_name, after_time, 1
         )
         return stops[0]
 
     async def async_get_deviation(self, id: str) -> DeviationInfo:
         """Retreive deviation info from Deviation Id."""
-        filters = [FieldFilter(FilterOperation.equal, "Deviation.Id", id)]
+        filters: list[FieldFilter | Filter] = [
+            FieldFilter(FilterOperation.EQUAL, "Deviation.Id", id)
+        ]
         deviations = await self._api.async_make_request(
-            "Situation", "1.5", DeviationInfo._required_fields, filters
+            "Situation",
+            "1.5",
+            DeviationInfo._required_fields,  # pylint: disable=protected-access
+            filters,
         )
 
         if len(deviations) == 0:
-            raise ValueError("No Deviation found")
+            raise NoDeviationFound("No Deviation found")
         if len(deviations) > 1:
-            raise ValueError("Multiple Deviations found")
+            raise MultipleDeviationsFound("Multiple Deviations found")
 
         deviation = deviations[0]
         return DeviationInfo.from_xml_node(deviation)
```

### Comparing `pytrafikverket-0.2.3/pytrafikverket/trafikverket_train.py` & `pytrafikverket-0.3.0/pytrafikverket/trafikverket_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 """Enables retreival of train departure information from Trafikverket API."""
-import typing
+from __future__ import annotations
+
+from typing import Any
+
 from datetime import datetime, timedelta
 from enum import Enum
 
 import aiohttp
 from pytrafikverket.trafikverket import (
     FieldFilter,
     FieldSort,
     FilterOperation,
     NodeHelper,
     OrFilter,
     SortOrder,
     Trafikverket,
 )
 
+from .exceptions import (
+    NoTrainStationFound,
+    MultipleTrainStationsFound,
+    NoTrainAnnouncementFound,
+    MultipleTrainAnnouncementFound,
+)
+
+# pylint: disable=W0622, C0103
+
 
-class StationInfo(object):
+class StationInfo:
     """Contains information about a train station."""
 
     _required_fields = ["LocationSignature", "AdvertisedLocationName"]
 
-    def __init__(self, signature: str, name: str, advertised: str):
+    def __init__(
+        self, signature: str | None, name: str | None, advertised: str | None
+    ) -> None:
         """Initialize StationInfo class."""
         self.signature = signature
         self.name = name
         self.advertised = advertised
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> StationInfo:
         """Map station information in XML data."""
         node_helper = NodeHelper(node)
         location_signature = node_helper.get_text("LocationSignature")
         advertised_location_name = node_helper.get_text("AdvertisedLocationName")
         location_advertised = node_helper.get_text("Advertised")
         return cls(location_signature, advertised_location_name, location_advertised)
 
 
 class TrainStopStatus(Enum):
     """Contain the different train stop statuses."""
 
-    on_time = "scheduled to arrive on schedule"
-    delayed = "delayed"
-    canceled = "canceled"
+    ON_TIME = "scheduled to arrive on schedule"
+    DELAYED = "delayed"
+    CANCELED = "canceled"
 
 
-class TrainStop(object):
+class TrainStop:
     """Contain information about a train stop."""
 
     _required_fields = [
         "ActivityId",
         "Canceled",
         "AdvertisedTimeAtLocation",
         "EstimatedTimeAtLocation",
@@ -57,54 +71,54 @@
         "Deviation",
         "ModifiedTime",
         "ProductInformation",
     ]
 
     def __init__(
         self,
-        id,
+        id: str | None,
         canceled: bool,
-        advertised_time_at_location: datetime,
-        estimated_time_at_location: datetime,
-        time_at_location: datetime,
-        other_information: typing.List[str],
-        deviations: typing.List[str],
-        modified_time: datetime,
-        product_description: str,
-    ):
+        advertised_time_at_location: datetime | None,
+        estimated_time_at_location: datetime | None,
+        time_at_location: datetime | None,
+        other_information: list[str] | None,
+        deviations: list[str] | None,
+        modified_time: datetime | None,
+        product_description: list[str] | None,
+    ) -> None:
         """Initialize TrainStop."""
         self.id = id
         self.canceled = canceled
         self.advertised_time_at_location = advertised_time_at_location
         self.estimated_time_at_location = estimated_time_at_location
         self.time_at_location = time_at_location
         self.other_information = other_information
         self.deviations = deviations
         self.modified_time = modified_time
         self.product_description = product_description
 
     def get_state(self) -> TrainStopStatus:
         """Retrieve the state of the departure."""
         if self.canceled:
-            return TrainStopStatus.canceled
+            return TrainStopStatus.CANCELED
         if (
             self.advertised_time_at_location is not None
             and self.time_at_location is not None
             and self.advertised_time_at_location != self.time_at_location
         ):
-            return TrainStopStatus.delayed
+            return TrainStopStatus.DELAYED
         if (
             self.advertised_time_at_location is not None
             and self.estimated_time_at_location is not None
             and self.advertised_time_at_location != self.estimated_time_at_location
         ):
-            return TrainStopStatus.delayed
-        return TrainStopStatus.on_time
+            return TrainStopStatus.DELAYED
+        return TrainStopStatus.ON_TIME
 
-    def get_delay_time(self) -> timedelta:
+    def get_delay_time(self) -> timedelta | None:
         """Calculate the delay of a departure."""
         if self.canceled:
             return None
         if (
             self.advertised_time_at_location is not None
             and self.time_at_location is not None
             and self.advertised_time_at_location != self.time_at_location
@@ -115,15 +129,15 @@
             and self.estimated_time_at_location is not None
             and self.advertised_time_at_location != self.estimated_time_at_location
         ):
             return self.estimated_time_at_location - self.advertised_time_at_location
         return None
 
     @classmethod
-    def from_xml_node(cls, node):
+    def from_xml_node(cls, node: Any) -> TrainStop:
         """Map the path in the return XML data."""
         node_helper = NodeHelper(node)
         activity_id = node_helper.get_text("ActivityId")
         canceled = node_helper.get_bool("Canceled")
         advertised_time_at_location = node_helper.get_datetime(
             "AdvertisedTimeAtLocation"
         )
@@ -142,194 +156,196 @@
             other_information,
             deviations,
             modified_time,
             product_description,
         )
 
 
-class TrafikverketTrain(object):
+class TrafikverketTrain:
     """Class used to communicate with trafikverket's train api."""
 
-    def __init__(self, client_session: aiohttp.ClientSession, api_key: str):
+    def __init__(self, client_session: aiohttp.ClientSession, api_key: str) -> None:
         """Initialize TrainInfo object."""
         self._api = Trafikverket(client_session, api_key)
 
     async def async_get_train_station(self, location_name: str) -> StationInfo:
         """Retreive train station id based on name."""
         train_stations = await self._api.async_make_request(
             "TrainStation",
             "1.4",
-            StationInfo._required_fields,
+            StationInfo._required_fields,  # pylint: disable=protected-access
             [
                 FieldFilter(
-                    FilterOperation.equal, "AdvertisedLocationName", location_name
+                    FilterOperation.EQUAL, "AdvertisedLocationName", location_name
                 ),
-                FieldFilter(FilterOperation.equal, "Advertised", "true"),
+                FieldFilter(FilterOperation.EQUAL, "Advertised", "true"),
             ],
         )
         if len(train_stations) == 0:
-            raise ValueError("Could not find a station with the specified name")
+            raise NoTrainStationFound(
+                "Could not find a station with the specified name"
+            )
         if len(train_stations) > 1:
-            raise ValueError("Found multiple stations with the specified name")
+            raise MultipleTrainStationsFound(
+                "Found multiple stations with the specified name"
+            )
 
         return StationInfo.from_xml_node(train_stations[0])
 
     async def async_search_train_stations(
         self, location_name: str
-    ) -> typing.List[StationInfo]:
+    ) -> list[StationInfo]:
         """Search for train stations."""
         train_stations = await self._api.async_make_request(
             "TrainStation",
             "1.4",
             ["AdvertisedLocationName", "LocationSignature", "Advertised", "Deleted"],
             [
                 FieldFilter(
-                    FilterOperation.like, "AdvertisedLocationName", location_name
+                    FilterOperation.LIKE, "AdvertisedLocationName", location_name
                 ),
-                FieldFilter(FilterOperation.equal, "Advertised", "true"),
+                FieldFilter(FilterOperation.EQUAL, "Advertised", "true"),
             ],
         )
         if len(train_stations) == 0:
-            raise ValueError("Could not find a station with the specified name")
+            raise NoTrainStationFound(
+                "Could not find a station with the specified name"
+            )
 
-        result = [StationInfo] * 0
+        result = []
 
         for train_station in train_stations:
             result.append(StationInfo.from_xml_node(train_station))
 
         return result
 
     async def async_get_train_stop(
         self,
         from_station: StationInfo,
         to_station: StationInfo,
         time_at_location: datetime,
-        product_description: typing.Optional[str] = None,
+        product_description: str | None = None,
         exclude_canceled: bool = False,
     ) -> TrainStop:
         """Retrieve the train stop."""
         date_as_text = time_at_location.strftime(Trafikverket.date_time_format)
 
         filters = [
-            FieldFilter(FilterOperation.equal, "ActivityType", "Avgang"),
+            FieldFilter(FilterOperation.EQUAL, "ActivityType", "Avgang"),
             FieldFilter(
-                FilterOperation.equal, "LocationSignature", from_station.signature
+                FilterOperation.EQUAL, "LocationSignature", from_station.signature
             ),
             FieldFilter(
-                FilterOperation.equal, "AdvertisedTimeAtLocation", date_as_text
+                FilterOperation.EQUAL, "AdvertisedTimeAtLocation", date_as_text
             ),
             OrFilter(
                 [
                     FieldFilter(
-                        FilterOperation.equal,
+                        FilterOperation.EQUAL,
                         "ViaToLocation.LocationName",
                         to_station.signature,
                     ),
                     FieldFilter(
-                        FilterOperation.equal,
+                        FilterOperation.EQUAL,
                         "ToLocation.LocationName",
                         to_station.signature,
                     ),
                 ]
             ),
         ]
 
         if product_description:
             filters.append(
                 FieldFilter(
-                    FilterOperation.equal,
+                    FilterOperation.EQUAL,
                     "ProductInformation.Description",
                     product_description,
                 )
             )
 
         if exclude_canceled:
-            filters.append(
-                FieldFilter(
-                    FilterOperation.equal,
-                    "Canceled",
-                    "false"
-                )
-            )
+            filters.append(FieldFilter(FilterOperation.EQUAL, "Canceled", "false"))
 
         train_announcements = await self._api.async_make_request(
-            "TrainAnnouncement", "1.6", TrainStop._required_fields, filters
+            "TrainAnnouncement",
+            "1.6",
+            TrainStop._required_fields,  # pylint: disable=protected-access
+            filters,
         )
 
         if len(train_announcements) == 0:
-            raise ValueError("No TrainAnnouncement found")
+            raise NoTrainAnnouncementFound("No TrainAnnouncement found")
 
         if len(train_announcements) > 1:
-            raise ValueError("Multiple TrainAnnouncements found")
+            raise MultipleTrainAnnouncementFound("Multiple TrainAnnouncements found")
 
         train_announcement = train_announcements[0]
         return TrainStop.from_xml_node(train_announcement)
 
     async def async_get_next_train_stop(
         self,
         from_station: StationInfo,
         to_station: StationInfo,
         after_time: datetime,
-        product_description: typing.Optional[str] = None,
+        product_description: str | None = None,
         exclude_canceled: bool = False,
     ) -> TrainStop:
         """Enable retreival of next departure."""
         date_as_text = after_time.strftime(Trafikverket.date_time_format)
 
         filters = [
-            FieldFilter(FilterOperation.equal, "ActivityType", "Avgang"),
+            FieldFilter(FilterOperation.EQUAL, "ActivityType", "Avgang"),
             FieldFilter(
-                FilterOperation.equal, "LocationSignature", from_station.signature
+                FilterOperation.EQUAL, "LocationSignature", from_station.signature
             ),
             FieldFilter(
-                FilterOperation.greater_than_equal,
+                FilterOperation.GREATER_THAN_EQUAL,
                 "AdvertisedTimeAtLocation",
                 date_as_text,
             ),
             OrFilter(
                 [
                     FieldFilter(
-                        FilterOperation.equal,
+                        FilterOperation.EQUAL,
                         "ViaToLocation.LocationName",
                         to_station.signature,
                     ),
                     FieldFilter(
-                        FilterOperation.equal,
+                        FilterOperation.EQUAL,
                         "ToLocation.LocationName",
                         to_station.signature,
                     ),
                 ]
             ),
         ]
 
         if product_description:
             filters.append(
                 FieldFilter(
-                    FilterOperation.equal,
+                    FilterOperation.EQUAL,
                     "ProductInformation.Description",
                     product_description,
                 )
             )
 
         if exclude_canceled:
-            filters.append(
-                FieldFilter(
-                    FilterOperation.equal,
-                    "Canceled",
-                    "false"
-                )
-            )
+            filters.append(FieldFilter(FilterOperation.EQUAL, "Canceled", "false"))
 
-        sorting = [FieldSort("AdvertisedTimeAtLocation", SortOrder.ascending)]
+        sorting = [FieldSort("AdvertisedTimeAtLocation", SortOrder.ASCENDING)]
         train_announcements = await self._api.async_make_request(
-            "TrainAnnouncement", "1.6", TrainStop._required_fields, filters, 1, sorting
+            "TrainAnnouncement",
+            "1.6",
+            TrainStop._required_fields,  # pylint: disable=protected-access
+            filters,
+            1,
+            sorting,
         )
 
         if len(train_announcements) == 0:
-            raise ValueError("No TrainAnnouncement found")
+            raise NoTrainAnnouncementFound("No TrainAnnouncement found")
 
         if len(train_announcements) > 1:
-            raise ValueError("Multiple TrainAnnouncements found")
+            raise MultipleTrainAnnouncementFound("Multiple TrainAnnouncements found")
 
         train_announcement = train_announcements[0]
 
         return TrainStop.from_xml_node(train_announcement)
```

