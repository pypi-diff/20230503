# Comparing `tmp/xt_st_common-0.2.1.tar.gz` & `tmp/xt_st_common-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.2.1.tar", max compression
+gzip compressed data, was "xt_st_common-0.3.0.tar", max compression
```

## Comparing `xt_st_common-0.2.1.tar` & `xt_st_common-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      606 2023-05-02 04:42:32.461250 xt_st_common-0.2.1/README.md
--rw-r--r--   0        0        0     1473 2023-05-02 04:42:32.461250 xt_st_common-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-02 04:42:32.461250 xt_st_common-0.2.1/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5013 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/components.py
--rw-r--r--   0        0        0     1686 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/config.py
--rw-r--r--   0        0        0     7174 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/database.py
--rw-r--r--   0        0        0    14615 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/file_manager.py
--rw-r--r--   0        0        0     5912 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/session.py
--rw-r--r--   0        0        0     4871 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1774 2023-05-02 04:41:54.425447 xt_st_common-0.2.1/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 xt_st_common-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      606 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/README.md
+-rw-r--r--   0        0        0     1508 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5039 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     1699 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     7200 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0    14615 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/file_manager.py
+-rw-r--r--   0        0        0     5938 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     4871 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1774 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 xt_st_common-0.3.0/PKG-INFO
```

### Comparing `xt_st_common-0.2.1/README.md` & `xt_st_common-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.2.1
+# XT-STREAMLIT - 0.3.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

### Comparing `xt_st_common-0.2.1/pyproject.toml` & `xt_st_common-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.2.1"
+version = "0.3.0"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.21.0"
 pydantic = "^1.10.7"
-jwt = "^1.3.1"
+pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 streamlit-js-eval = "^0.1.5"
 minio = { version = "^7.1.14", optional = true }
 odmantic = { version = "^0.9.2", optional = true }
 chardet = "^5.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `xt_st_common-0.2.1/src/xt_st_common/components.py` & `xt_st_common-0.3.0/src/xt_st_common/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import streamlit as st
 
-from xt_st_common.config import Settings
+from xt_st_common.config import StreamlitBaseSettings
 
-settings = Settings()
+settings = StreamlitBaseSettings()
 
 
 def page_header(
     page_title: str | None = None,
     page_logo: str | None = None,
     page_logo_width: int = 250,
     logout_url: str | None = None,
```

### Comparing `xt_st_common-0.2.1/src/xt_st_common/config.py` & `xt_st_common-0.3.0/src/xt_st_common/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseSettings
 from pydantic.color import Color
 
 
-class Settings(BaseSettings):
+class StreamlitBaseSettings(BaseSettings):
     SIGNOUT_URL: Optional[str] = None
     CURRENT_PACKAGE = __name__.split(".")[0]
     BASE_PATH: str = str(Path(PathFinder().find_spec(CURRENT_PACKAGE).origin).parent)  # type: ignore
     DATA_DIR: str = str(Path.cwd() / "appdata")
     """Root directory for storing app data"""
     APP_TAG_TEXT: str = "Development"
     """text that will appear next the application logo"""
```

### Comparing `xt_st_common-0.2.1/src/xt_st_common/database.py` & `xt_st_common-0.3.0/src/xt_st_common/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from pathlib import Path
 from typing import Dict, List, Union
 
 import streamlit as st
 from odmantic import Model, SyncEngine, query
 from pymongo import MongoClient
 
-from .config import Settings
+from .config import StreamlitBaseSettings
 from .storage import FileRef
 
 # from streamlit.runtime.uploaded_file_manager import UploadedFile # FIXME: remove if unneeded?
 
 
 # Initialize connection.
 # Uses st.experimental_singleton to only run once.
 @st.experimental_singleton
 def get_engine():
-    settings = Settings()
+    settings = StreamlitBaseSettings()
     if settings.MONGO_CONNECTION_STRING is None:
         raise ValueError("Can't get mongo engine when connection string is None.")
 
     client = MongoClient(settings.MONGO_CONNECTION_STRING)
     return SyncEngine(client=client, database=settings.DATABASE_NAME)
```

### Comparing `xt_st_common-0.2.1/src/xt_st_common/file_manager.py` & `xt_st_common-0.3.0/src/xt_st_common/file_manager.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.2.1/src/xt_st_common/session.py` & `xt_st_common-0.3.0/src/xt_st_common/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import List
 
 import jwt
 from streamlit.web.server.websocket_headers import _get_websocket_headers
 
-from xt_st_common.config import Settings
+from xt_st_common.config import StreamlitBaseSettings
 
-settings = Settings()
+settings = StreamlitBaseSettings()
 
 
 def get_session_headers():
     """
     Returns the request headers for the current streamlit session
     """
     if settings.DEBUG and settings.DEBUG_MOCK_SESSION:
```

### Comparing `xt_st_common-0.2.1/src/xt_st_common/storage.py` & `xt_st_common-0.3.0/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.2.1/src/xt_st_common/utils.py` & `xt_st_common-0.3.0/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.2.1/PKG-INFO` & `xt_st_common-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.2.1
+Version: 0.3.0
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: databases
 Provides-Extra: storage
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
-Requires-Dist: jwt (>=1.3.1,<2.0.0)
 Requires-Dist: minio (>=7.1.14,<8.0.0) ; extra == "storage"
 Requires-Dist: odmantic (>=0.9.2,<0.10.0) ; extra == "databases"
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.2.1
+# XT-STREAMLIT - 0.3.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

