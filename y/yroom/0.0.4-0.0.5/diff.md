# Comparing `tmp/yroom-0.0.4.tar.gz` & `tmp/yroom-0.0.5.tar.gz`

## Comparing `yroom-0.0.4.tar` & `yroom-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.4/Cargo.toml
--rw-r--r--   0     1001      123     2772 2023-04-30 12:23:26.000000 yroom-0.0.4/.github/workflows/release.yml
--rw-r--r--   0     1001      123     1174 2023-04-30 12:23:26.000000 yroom-0.0.4/.github/workflows/test.yml
--rw-r--r--   0     1001      123       40 2023-04-30 12:23:26.000000 yroom-0.0.4/.gitignore
--rw-r--r--   0     1001      123     1083 2023-04-30 12:23:26.000000 yroom-0.0.4/LICENSE
--rw-r--r--   0     1001      123      141 2023-04-30 12:23:26.000000 yroom-0.0.4/README.md
--rw-r--r--   0     1001      123       10 2023-04-30 12:24:29.000000 yroom-0.0.4/dist/yroom-0.0.4.tar.gz
--rw-r--r--   0     1001      123      746 2023-04-30 12:23:26.000000 yroom-0.0.4/pyproject.toml
--rw-r--r--   0     1001      123      272 2023-04-30 12:23:26.000000 yroom-0.0.4/src/lib.rs
--rw-r--r--   0     1001      123    21486 2023-04-30 12:23:26.000000 yroom-0.0.4/src/roomsync.rs
--rw-r--r--   0     1001      123     6485 2023-04-30 12:23:26.000000 yroom-0.0.4/tests/test_yroom.py
--rw-r--r--   0     1001      123     3889 2023-04-30 12:23:26.000000 yroom-0.0.4/yroom.pyi
--rw-r--r--   0     1001      123    13697 2023-04-30 12:23:26.000000 yroom-0.0.4/Cargo.lock
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 yroom-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      123     2772 2023-05-03 08:01:56.000000 yroom-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1174 2023-05-03 08:01:56.000000 yroom-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0     1001      123       40 2023-05-03 08:01:56.000000 yroom-0.0.5/.gitignore
+-rw-r--r--   0     1001      123     1083 2023-05-03 08:01:56.000000 yroom-0.0.5/LICENSE
+-rw-r--r--   0     1001      123      442 2023-05-03 08:01:56.000000 yroom-0.0.5/README.md
+-rw-r--r--   0     1001      123       10 2023-05-03 08:03:01.000000 yroom-0.0.5/dist/yroom-0.0.5.tar.gz
+-rw-r--r--   0     1001      123      746 2023-05-03 08:01:56.000000 yroom-0.0.5/pyproject.toml
+-rw-r--r--   0     1001      123      272 2023-05-03 08:01:56.000000 yroom-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      123    21727 2023-05-03 08:01:56.000000 yroom-0.0.5/src/roomsync.rs
+-rw-r--r--   0     1001      123     6492 2023-05-03 08:01:56.000000 yroom-0.0.5/tests/test_yroom.py
+-rw-r--r--   0     1001      123     3889 2023-05-03 08:01:56.000000 yroom-0.0.5/yroom.pyi
+-rw-r--r--   0     1001      123    13697 2023-05-03 08:01:56.000000 yroom-0.0.5/Cargo.lock
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 yroom-0.0.5/PKG-INFO
```

### Comparing `yroom-0.0.4/.github/workflows/release.yml` & `yroom-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `yroom-0.0.4/.github/workflows/test.yml` & `yroom-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `yroom-0.0.4/LICENSE` & `yroom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yroom-0.0.4/pyproject.toml` & `yroom-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "yroom"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">=3.7"
 description = "Yjs sync and awareness protocol handler for a non-editing client (e.g. server)"
 authors = [
     { name = "Stefan Wehrmeyer", email = "mail@stefanwehrmeyer.com" }
 ]
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `yroom-0.0.4/src/roomsync.rs` & `yroom-0.0.5/src/roomsync.rs`

 * *Files 6% similar despite different names*

```diff
@@ -22,53 +22,53 @@
         decoder::{Decode, DecoderV1, DecoderV2},
         encoder::{Encode, Encoder, EncoderV1, EncoderV2},
     },
     GetString, ReadTxn, StateVector, Transact, Update,
 };
 
 #[derive(Clone, Default, Debug)]
-enum WireVersion {
+enum ProtocolVersion {
     #[default]
     V1,
     V2,
 }
 
 struct EncoderWrapper {
-    wire_version: WireVersion,
+    protocol_version: ProtocolVersion,
     messages: Vec<Message>,
     prefix: Option<String>,
 }
 
 impl EncoderWrapper {
-    fn new(wire_version: &WireVersion, prefix: Option<String>) -> Self {
+    fn new(protocol_version: &ProtocolVersion, prefix: Option<String>) -> Self {
         EncoderWrapper {
-            wire_version: wire_version.clone(),
+            protocol_version: protocol_version.clone(),
             messages: Vec::default(),
             prefix,
         }
     }
     fn push(&mut self, message: Message) {
         self.messages.push(message);
     }
     fn to_vec(&self) -> Vec<u8> {
-        match self.wire_version {
-            WireVersion::V1 => {
+        match self.protocol_version {
+            ProtocolVersion::V1 => {
                 if self.messages.is_empty() {
                     return Vec::new();
                 }
                 let mut encoder = EncoderV1::new();
                 if let Some(prefix) = &self.prefix {
                     encoder.write_string(prefix);
                 }
                 self.messages.iter().for_each(|message| {
                     message.encode(&mut encoder);
                 });
                 encoder.to_vec()
             }
-            WireVersion::V2 => {
+            ProtocolVersion::V2 => {
                 if self.messages.is_empty() {
                     return Vec::new();
                 }
                 let mut encoder = EncoderV2::new();
                 if let Some(prefix) = &self.prefix {
                     encoder.write_string(prefix);
                 }
@@ -78,116 +78,116 @@
                 encoder.to_vec()
             }
         }
     }
 }
 
 struct DecoderWrapper<'a> {
-    wire_version: WireVersion,
+    protocol_version: ProtocolVersion,
     decoder_v1: Option<DecoderV1<'a>>,
     decoder_v2: Option<DecoderV2<'a>>,
     pub document_name: Option<String>,
 }
 
 impl<'a> DecoderWrapper<'a> {
     fn new(
-        wire_version: &WireVersion,
+        protocol_version: &ProtocolVersion,
         cursor: Cursor<'a>,
-        name_prefixed: bool,
+        name_prefix: bool,
     ) -> Result<Self, lib0::error::Error> {
         let mut document_name = None;
-        match wire_version {
-            WireVersion::V1 => {
+        match protocol_version {
+            ProtocolVersion::V1 => {
                 let mut decoder = DecoderV1::new(cursor);
-                if name_prefixed {
+                if name_prefix {
                     document_name = Some(decoder.read_string()?.to_string());
                 }
                 Ok(DecoderWrapper {
-                    wire_version: wire_version.clone(),
+                    protocol_version: protocol_version.clone(),
                     decoder_v1: Some(decoder),
                     decoder_v2: None,
                     document_name,
                 })
             }
-            WireVersion::V2 => match DecoderV2::new(cursor) {
+            ProtocolVersion::V2 => match DecoderV2::new(cursor) {
                 Ok(mut decoder) => {
-                    if name_prefixed {
+                    if name_prefix {
                         document_name = Some(decoder.read_string()?.to_string());
                     }
                     Ok(DecoderWrapper {
-                        wire_version: wire_version.clone(),
+                        protocol_version: protocol_version.clone(),
                         decoder_v1: None,
                         decoder_v2: Some(decoder),
                         document_name,
                     })
                 }
                 Err(err) => Err(err),
             },
         }
     }
 }
 
 impl Iterator for DecoderWrapper<'_> {
     type Item = Result<Message, lib0::error::Error>;
     fn next(&mut self) -> Option<Self::Item> {
-        match self.wire_version {
-            WireVersion::V1 => MessageReader::new(self.decoder_v1.as_mut().unwrap()).next(),
-            WireVersion::V2 => MessageReader::new(self.decoder_v2.as_mut().unwrap()).next(),
+        match self.protocol_version {
+            ProtocolVersion::V1 => MessageReader::new(self.decoder_v1.as_mut().unwrap()).next(),
+            ProtocolVersion::V2 => MessageReader::new(self.decoder_v2.as_mut().unwrap()).next(),
         }
     }
 }
 
-impl From<u8> for WireVersion {
+impl From<u8> for ProtocolVersion {
     fn from(version: u8) -> Self {
         match version {
-            1 => WireVersion::V1,
-            2 => WireVersion::V2,
+            1 => ProtocolVersion::V1,
+            2 => ProtocolVersion::V2,
             // TODO: make this more graceful
             _ => panic!("Invalid encoder version"),
         }
     }
 }
 
 #[derive(Clone, Debug)]
 struct YRoomSettings {
-    pub wire_version: WireVersion,
-    pub name_prefixed: bool,
+    pub protocol_version: ProtocolVersion,
+    pub name_prefix: bool,
     pub server_start_sync: bool,
 }
 
 impl Default for YRoomSettings {
     fn default() -> Self {
         YRoomSettings {
-            wire_version: WireVersion::V1,
-            name_prefixed: false,
+            protocol_version: ProtocolVersion::V1,
+            name_prefix: false,
             server_start_sync: true,
         }
     }
 }
 
 impl FromPyObject<'_> for YRoomSettings {
     fn extract(ob: &PyAny) -> PyResult<Self> {
         let settings = ob.downcast::<PyDict>()?;
 
-        let wire_version: WireVersion = match settings.get_item("wire_version") {
-            Some(wire_version) => wire_version.extract::<u8>()?.into(),
-            None => WireVersion::V1,
+        let protocol_version: ProtocolVersion = match settings.get_item("PROTOCOL_VERSION") {
+            Some(protocol_version) => protocol_version.extract::<u8>()?.into(),
+            None => ProtocolVersion::V1,
         };
-        let name_prefixed = match settings.get_item("name_prefixed") {
-            Some(name_prefixed) => name_prefixed.extract::<bool>()?,
+        let name_prefix = match settings.get_item("PROTOCOL_NAME_PREFIX") {
+            Some(name_prefix) => name_prefix.extract::<bool>()?,
             None => false,
         };
-        let server_start_sync = match settings.get_item("server_start_sync") {
+        let server_start_sync = match settings.get_item("SERVER_START_SYNC") {
             Some(server_start_sync) => server_start_sync.extract::<bool>()?,
             None => true,
         };
 
         Ok(YRoomSettings {
-            wire_version,
-            name_prefixed,
+            protocol_version,
+            name_prefix,
             server_start_sync,
         })
     }
 }
 
 #[pyclass]
 pub struct YRoomMessage {
@@ -451,15 +451,15 @@
     fn connect(&mut self, conn_id: u64) -> YRoomMessage {
         let connections = self.connections.lock();
         connections
             .unwrap()
             .entry(conn_id)
             .or_insert_with(HashSet::new);
 
-        let mut encoder = EncoderWrapper::new(&self.settings.wire_version, None);
+        let mut encoder = EncoderWrapper::new(&self.settings.protocol_version, None);
 
         if self.settings.server_start_sync {
             let sv = self.awareness.doc().transact().state_vector();
             encoder.push(Message::Sync(SyncMessage::SyncStep1(sv)));
             if !self.awareness.clients().is_empty() {
                 if let Ok(awareness_update) = self.awareness.update() {
                     encoder.push(Message::Awareness(awareness_update));
@@ -473,54 +473,58 @@
         })
     }
 
     pub fn handle_message(&mut self, conn_id: u64, payload: Vec<u8>) -> YRoomMessage {
         log::debug!("message: {:?}", payload);
         let cursor = Cursor::new(&payload);
         let decoder = match DecoderWrapper::new(
-            &self.settings.wire_version,
+            &self.settings.protocol_version,
             cursor,
-            self.settings.name_prefixed,
+            self.settings.name_prefix,
         ) {
             Ok(decoder) => decoder,
             Err(e) => {
                 log::error!("Error decoding message: {}", e);
                 // TODO: return error message
                 return Python::with_gil(|py| YRoomMessage {
                     payload: PyBytes::new(py, &[]).into(),
                     broadcast_payload: PyBytes::new(py, &[]).into(),
                 });
             }
         };
 
-        let mut sync_encoder =
-            EncoderWrapper::new(&self.settings.wire_version, decoder.document_name.clone());
-        let mut update_encoder =
-            EncoderWrapper::new(&self.settings.wire_version, decoder.document_name.clone());
+        let mut sync_encoder = EncoderWrapper::new(
+            &self.settings.protocol_version,
+            decoder.document_name.clone(),
+        );
+        let mut update_encoder = EncoderWrapper::new(
+            &self.settings.protocol_version,
+            decoder.document_name.clone(),
+        );
 
         decoder.for_each(|message_result| match message_result {
             Ok(message) => match message {
                 Message::Sync(SyncMessage::SyncStep1(sv)) => {
                     let txn = self.awareness.doc_mut().transact_mut();
-                    let data = match self.settings.wire_version {
-                        WireVersion::V1 => txn.encode_diff_v1(&sv),
-                        WireVersion::V2 => {
+                    let data = match self.settings.protocol_version {
+                        ProtocolVersion::V1 => txn.encode_diff_v1(&sv),
+                        ProtocolVersion::V2 => {
                             let mut enc = EncoderV2::new();
                             txn.encode_diff(&sv, &mut enc);
                             enc.to_vec()
                         }
                     };
                     log::debug!("message: {:?}", data);
                     let message = Message::Sync(SyncMessage::SyncStep2(data));
                     sync_encoder.push(message);
                 }
                 Message::Sync(SyncMessage::SyncStep2(data)) => {
-                    let update = match self.settings.wire_version {
-                        WireVersion::V1 => Update::decode_v1(&data),
-                        WireVersion::V2 => Update::decode_v2(&data),
+                    let update = match self.settings.protocol_version {
+                        ProtocolVersion::V1 => Update::decode_v1(&data),
+                        ProtocolVersion::V2 => Update::decode_v2(&data),
                     };
                     match update {
                         Ok(update) => {
                             let mut txn = self.awareness.doc_mut().transact_mut();
                             txn.apply_update(update);
                         }
                         Err(e) => log::error!("Error decoding sync step 2: {}", e),
@@ -599,26 +603,26 @@
                 client_ids.iter().for_each(|client_id| {
                     self.awareness.remove_state(*client_id);
                 });
             }
             connections.remove(&conn_id);
         }
         // FIXME: Can't give possibly necessary name prefix on disconnect
-        let mut encoder = EncoderWrapper::new(&self.settings.wire_version, None);
+        let mut encoder = EncoderWrapper::new(&self.settings.protocol_version, None);
         if let Ok(awareness_update) = self.awareness.update() {
             encoder.push(Message::Awareness(awareness_update));
         }
         encoder.to_vec()
     }
 
     pub fn serialize(&self) -> Vec<u8> {
         let txn = self.awareness.doc().transact();
-        match self.settings.wire_version {
-            WireVersion::V1 => txn.encode_state_as_update_v1(&StateVector::default()),
-            WireVersion::V2 => txn.encode_state_as_update_v2(&StateVector::default()),
+        match self.settings.protocol_version {
+            ProtocolVersion::V1 => txn.encode_state_as_update_v1(&StateVector::default()),
+            ProtocolVersion::V2 => txn.encode_state_as_update_v2(&StateVector::default()),
         }
     }
 
     pub fn is_alive(&self) -> bool {
         !self.connections.lock().unwrap().is_empty()
     }
 }
```

### Comparing `yroom-0.0.4/tests/test_yroom.py` & `yroom-0.0.5/tests/test_yroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     d1 = Y.YDoc()
     text = d1.get_text("test")
     with d1.begin_transaction() as txn:
         text.extend(txn, "hello world!")
 
     room_name = "test"
     client_id = 1
-    manager = YRoomManager({room_name: {"server_start_sync": False}})
+    manager = YRoomManager({room_name: {"SERVER_START_SYNC": False}})
     message = manager.connect(room_name, client_id)
     assert message.payload == b""
     assert message.broadcast_payload == b""
 
     state_vector = Y.encode_state_vector(d1)
     sv_len = len(state_vector).to_bytes(1, "big")
     client_sync_step1_payload = b"".join(
@@ -182,16 +182,16 @@
         text.extend(txn, "hello world!")
 
     room_name = "test"
     client_id = 1
     manager = YRoomManager(
         {
             room_name: {
-                "server_start_sync": False,
-                "name_prefixed": True,
+                "SERVER_START_SYNC": False,
+                "PROTOCOL_NAME_PREFIX": True,
             }
         }
     )
     message = manager.connect(room_name, client_id)
     assert message.payload == b""
     assert message.broadcast_payload == b""
```

### Comparing `yroom-0.0.4/yroom.pyi` & `yroom-0.0.5/yroom.pyi`

 * *Files identical despite different names*

### Comparing `yroom-0.0.4/Cargo.lock` & `yroom-0.0.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
  "lib0",
  "thiserror",
  "yrs",
 ]
 
 [[package]]
 name = "yroom"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
  "lib0",
  "log",
  "pyo3",
  "pyo3-log",
  "y-sync",
  "yrs",
```

