# Comparing `tmp/esd_services_api_client-0.6.1.tar.gz` & `tmp/esd_services_api_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-0.6.1.tar", max compression
+gzip compressed data, was "esd_services_api_client-0.7.0.tar", max compression
```

## Comparing `esd_services_api_client-0.6.1.tar` & `esd_services_api_client-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10693 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/LICENSE
--rw-r--r--   0        0        0      120 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/README.md
--rw-r--r--   0        0        0      598 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2023-04-24 15:55:57.578765 esd_services_api_client-0.6.1/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      791 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/__init__.py
--rw-r--r--   0        0        0     1163 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_api_versions.py
--rw-r--r--   0        0        0     7197 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_connector.py
--rw-r--r--   0        0        0     5919 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_models.py
--rw-r--r--   0        0        0      743 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0     2666 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_auth.py
--rw-r--r--   0        0        0    10369 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_connector.py
--rw-r--r--   0        0        0     9442 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_models.py
--rw-r--r--   0        0        0     2221 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      780 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     5214 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      976 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8272 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1736 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_helpers.py
--rw-r--r--   0        0        0     3105 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      598 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      787 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      832 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0     9493 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4025 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0      949 2023-04-24 15:55:57.578765 esd_services_api_client-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 esd_services_api_client-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/LICENSE
+-rw-r--r--   0        0        0      120 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/README.md
+-rw-r--r--   0        0        0      598 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-03 15:02:41.141281 esd_services_api_client-0.7.0/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      791 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_api_versions.py
+-rw-r--r--   0        0        0     6934 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_connector.py
+-rw-r--r--   0        0        0     5703 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_models.py
+-rw-r--r--   0        0        0      743 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_auth.py
+-rw-r--r--   0        0        0    10369 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_connector.py
+-rw-r--r--   0        0        0     9442 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_models.py
+-rw-r--r--   0        0        0     2221 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      780 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     5214 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      976 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8272 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1736 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_helpers.py
+-rw-r--r--   0        0        0     3105 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      598 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0     9493 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4025 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0      949 2023-05-03 15:02:41.141281 esd_services_api_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 esd_services_api_client-0.7.0/PKG-INFO
```

### Comparing `esd_services_api_client-0.6.1/LICENSE` & `esd_services_api_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/arcane/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/arcane/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_api_versions.py` & `esd_services_api_client-0.7.0/esd_services_api_client/arcane/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_connector.py` & `esd_services_api_client-0.7.0/esd_services_api_client/arcane/_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,27 @@
         info = self.http.post(
             f"{self.base_url}/stream/restart/{source}/{stream_id}", json=conf
         )
         info.raise_for_status()
 
         return StreamInfo.from_dict(info.json())
 
+    def reload_stream(self, source: str, stream_id: str) -> Optional[StreamInfo]:
+        """
+          Requests a stream restart with a new configuration.
+
+        :param source: Source for this stream.
+        :param stream_id: Stream identifier.
+        :return:
+        """
+        info = self.http.post(f"{self.base_url}/stream/reload/{source}/{stream_id}")
+        info.raise_for_status()
+
+        return StreamInfo.from_dict(info.json())
+
     def stop_stream(self, source: str, stream_id: str) -> Optional[StreamInfo]:
         """
           Requests a stream stop.
 
         :param source: Source for this stream.
         :param stream_id: Stream identifier.
         :return:
@@ -177,38 +190,14 @@
         for active_stream in active_streams:
             info = self.http.post(
                 f"{self.base_url}/stream/stop/{source}/{active_stream.id}"
             )
             if info.status_code == 202:
                 yield info.json()
 
-    def transfer_stream(
-        self, source: str, stream_id: str, new_owner: str
-    ) -> Optional[StreamInfo]:
-        """
-          Requests a stream transfer to another host.
-
-        :param source: Source for this stream.
-        :param stream_id: Stream identifier.
-        :param new_owner: A new host that should run this stream.
-        :return:
-        """
-
-        transfer_response = self.http.post(
-            f"{self.base_url}/stream/transfer/{source}/{stream_id}/{new_owner}"
-        )
-
-        transfer_response.raise_for_status()
-
-        try:
-            return StreamInfo.from_dict(transfer_response.json())
-        except ValueError as ex:
-            print(ex)
-            return None
-
     def update_stream(self, source: str, stream_id: str, request: StreamInfo):
         """
         Update stream metadata
 
         :param source:
         :param stream_id:
         :param request:
```

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_models.py` & `esd_services_api_client-0.7.0/esd_services_api_client/arcane/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,46 +167,33 @@
             "PartitionColumnNameFormat": self.partition_column_name_format,
             "ClientTag": self.client_tag,
         }
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
-class StreamError(DataClassJsonMixin):
-    """
-    Arcane stream failure information.
-    """
-
-    error_type: str
-    error_message: str
-    error_stack: str
-
-
-@dataclass_json(letter_case=LetterCase.CAMEL)
-@dataclass
 class StreamInfo(DataClassJsonMixin):
     """
     Arcane stream information.
     """
 
     id: str  # pylint: disable=C0103
     stream_source: str
     started_at: str
-    owner: str
     tag: str
     stream_configuration: str
     stream_metadata: str
     stream_state: str
-    error: StreamError
     stopped_at: Optional[str] = None
 
 
 class StreamState(Enum):
     """
     Stream states in Arcane.
     """
 
     RUNNING = "RUNNING"
     STOPPED = "STOPPED"
     TERMINATING = "TERMINATING"
     RESTARTING = "RESTARTING"
     FAILED = "FAILED"
+    SCHEMA_MISMATCH = "SCHEMA_MISMATCH"
```

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/beast/_auth.py` & `esd_services_api_client-0.7.0/esd_services_api_client/beast/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/beast/_connector.py` & `esd_services_api_client-0.7.0/esd_services_api_client/beast/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/beast/_models.py` & `esd_services_api_client-0.7.0/esd_services_api_client/beast/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/README.md` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_helpers.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_helpers.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/common/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-0.7.0/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-0.7.0/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-0.7.0/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-0.7.0/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.1/pyproject.toml` & `esd_services_api_client-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "0.6.1"
+version = "0.7.0"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-0.6.1/PKG-INFO` & `esd_services_api_client-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

