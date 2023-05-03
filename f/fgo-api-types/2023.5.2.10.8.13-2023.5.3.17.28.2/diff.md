# Comparing `tmp/fgo_api_types-2023.5.2.10.8.13.tar.gz` & `tmp/fgo_api_types-2023.5.3.17.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.5.2.10.8.13.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.5.3.17.28.2.tar", max compression
```

## Comparing `fgo_api_types-2023.5.2.10.8.13.tar` & `fgo_api_types-2023.5.3.17.28.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-02 10:07:44.199716 fgo_api_types-2023.5.2.10.8.13/LICENSE
--rw-r--r--   0        0        0      449 2023-05-02 10:07:44.199716 fgo_api_types-2023.5.2.10.8.13/README.md
--rw-r--r--   0        0        0        0 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/common.py
--rw-r--r--   0        0        0    37946 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157289 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74891 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50178 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-05-02 10:08:13.867619 fgo_api_types-2023.5.2.10.8.13/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-05-02 10:08:14.219618 fgo_api_types-2023.5.2.10.8.13/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.2.10.8.13/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-03 17:27:27.774556 fgo_api_types-2023.5.3.17.28.2/LICENSE
+-rw-r--r--   0        0        0      449 2023-05-03 17:27:27.774556 fgo_api_types-2023.5.3.17.28.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37946 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157289 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74966 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50178 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-05-03 17:28:02.758900 fgo_api_types-2023.5.3.17.28.2/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.3.17.28.2/PKG-INFO
```

### Comparing `fgo_api_types-2023.5.2.10.8.13/LICENSE` & `fgo_api_types-2023.5.3.17.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/basic.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/common.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/enums.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/gameenums.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/nice.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2196,15 +2196,17 @@
     call: list[int] = Field([], title="Summon these NPC IDs")
     enemyFieldPosCount: int | None = None
     enemyActCount: int | None = None
     turn: int | None = Field(None, title="Turn countdown")
     limitAct: StageLimitActType | None = Field(
         None, title="Action after turn countdown is over"
     )
+    NoEntryIds: list[int] | None = None
     waveStartMovies: list[NiceStageStartMovie] = []
+    originalScript: dict[str, Any]
     enemies: list[QuestEnemy] = []
 
 
 class NiceQuestMessage(BaseModelORJson):
     idx: int
     message: str
     condType: NiceCondType
```

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/raw.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/rayshift.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/fgo_api_types/search.py` & `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.2.10.8.13/pyproject.toml` & `fgo_api_types-2023.5.3.17.28.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.05.02.10.08.13"
+version = "2023.05.03.17.28.02"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.5.2.10.8.13/PKG-INFO` & `fgo_api_types-2023.5.3.17.28.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.5.2.10.8.13
+Version: 2023.5.3.17.28.2
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

