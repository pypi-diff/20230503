# Comparing `tmp/crelm-0.0.30a2.tar.gz` & `tmp/crelm-0.0.30a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crelm-0.0.30a2.tar", max compression
+gzip compressed data, was "crelm-0.0.30a3.tar", max compression
```

## Comparing `crelm-0.0.30a2.tar` & `crelm-0.0.30a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-03-20 17:24:58.163553 crelm-0.0.30a2/LICENSE
--rw-r--r--   0        0        0      582 2023-03-29 17:17:37.948852 crelm-0.0.30a2/README.md
--rw-r--r--   0        0        0      181 2023-03-20 17:24:58.163553 crelm-0.0.30a2/crelm/__init__.py
--rw-r--r--   0        0        0     2976 2023-04-04 12:56:00.776271 crelm-0.0.30a2/crelm/factory.py
--rw-r--r--   0        0        0      380 2023-03-20 17:24:58.163553 crelm-0.0.30a2/crelm/libcrelm.py
--rw-r--r--   0        0        0   103701 2023-03-20 17:24:58.163553 crelm-0.0.30a2/crelm/makeheaders.c
--rw-r--r--   0        0        0     1900 2023-03-20 17:24:58.163553 crelm-0.0.30a2/crelm/makeheaders_crelm.c
--rw-r--r--   0        0        0    12752 2023-04-06 18:25:49.477305 crelm-0.0.30a2/crelm/tube.py
--rw-r--r--   0        0        0      748 2023-04-06 18:25:54.617295 crelm-0.0.30a2/pyproject.toml
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 crelm-0.0.30a2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-06 18:21:20.719078 crelm-0.0.30a3/LICENSE
+-rw-r--r--   0        0        0      600 2023-04-06 18:21:20.719078 crelm-0.0.30a3/README.md
+-rw-r--r--   0        0        0      187 2023-04-06 18:21:20.719078 crelm-0.0.30a3/crelm/__init__.py
+-rw-r--r--   0        0        0     3071 2023-04-06 18:21:20.719078 crelm-0.0.30a3/crelm/factory.py
+-rw-r--r--   0        0        0      391 2023-04-06 18:21:20.720078 crelm-0.0.30a3/crelm/libcrelm.py
+-rw-r--r--   0        0        0   107326 2023-04-06 18:21:20.721078 crelm-0.0.30a3/crelm/makeheaders.c
+-rw-r--r--   0        0        0     1987 2023-04-06 18:21:20.721078 crelm-0.0.30a3/crelm/makeheaders_crelm.c
+-rw-r--r--   0        0        0    13575 2023-05-03 16:52:52.748523 crelm-0.0.30a3/crelm/tube.py
+-rw-r--r--   0        0        0      778 2023-05-03 16:56:20.327627 crelm-0.0.30a3/pyproject.toml
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 crelm-0.0.30a3/PKG-INFO
```

### Comparing `crelm-0.0.30a2/LICENSE` & `crelm-0.0.30a3/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Wide Open Technical Services Ltd
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Wide Open Technical Services Ltd
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `crelm-0.0.30a2/README.md` & `crelm-0.0.30a3/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Crelm
-The Crelm package provides a relatively simple API around the CFFI system. Give it C code or source files, it gives you a package with bindings to functions and `struct`s. Easiest way to get started is hack up the examples in [the repo](https://github.com/wideopensource/crelm/tree/main/examples).
-
-### Installation
-
-pip3 install crelm
-
-### Simple Demo
-
-```
-from crelm import Factory
-
-paste = Factory(debug=False, verbose=True).create_Tube('add2') \
-    .add_source_text('int add2(int a, int b) { return a + b; }') \
-    .squeeze()
-
-print(f'2 + 3 = {paste.add2(2, 3)}')
-```
+# Crelm
+The Crelm package provides a relatively simple API around the CFFI system. Give it C code or source files, it gives you a package with bindings to functions and `struct`s. Easiest way to get started is hack up the examples in [the repo](https://github.com/wideopensource/crelm/tree/main/examples).
+
+### Installation
+
+pip3 install crelm
+
+### Simple Demo
+
+```
+from crelm import Factory
+
+paste = Factory(debug=False, verbose=True).create_Tube('add2') \
+    .add_source_text('int add2(int a, int b) { return a + b; }') \
+    .squeeze()
+
+print(f'2 + 3 = {paste.add2(2, 3)}')
+```
```

### Comparing `crelm-0.0.30a2/crelm/makeheaders_crelm.c` & `crelm-0.0.30a3/crelm/makeheaders_crelm.c`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-#include <stdio.h>
-
-// todo foss: tie this in with externla DEBUG macro
-// #define DEBUG (PARSER | DECL_DUMP | TOKENIZER)
-
-#define TEST 2 // foss: semi-hack to disable main() in makeheaders.c
-
-// foss: unmodified from source: https://www.hwaci.com/sw/mkhdr/
-#include "makeheaders.c"
-
-// foss: note that this code is MIT-licensed but makeheaders.c is under
-// the (seemingly compatible) 2-clause BSD license.
-
-// foss: WARNING: makeheaders keeps a lot of global state which makes
-// it awkward to use in a library. Make sure the state is reset between runs.
-
-static int build_declarations(char *header, FILE *log_file) {
-  GenState sState;
-  String outStr;
-  IdentTable includeTable;
-  Decl *pDecl;
-
-  sState.pStr = &outStr;
-  StringInit(&outStr);
-
-  sState.pTable = &includeTable;
-  memset(&includeTable, 0, sizeof(includeTable));
-  sState.zIf = 0;
-  sState.nErr = 0;
-  sState.zFilename = "(all)";
-  sState.flags = 0;
-
-  ResetDeclFlags(0);
-
-  for (pDecl = pDeclFirst; pDecl; pDecl = pDecl->pNext) {
-    DeclareObject(pDecl, &sState, 1);
-  }
-
-  ChangeIfContext(0, &sState);
-  strcpy(header, StringGet(&outStr));
-
-#ifdef DEBUG
-  fprintf(log_file, "emitting decl: '%s'\n", header);
-#endif
-
-  IdentTableReset(&includeTable);
-  StringReset(&outStr);
-  return 0;
-}
-
-int make_header(char const *source, char *header) {
-  Token *pList;
-  FILE *log_file = stdout;
-  IdentTable idTable;
-  int rv = 0;
-
-#ifdef DEBUG
-  debugMask = DEBUG;
-
-  fprintf(log_file, "%s -> %s\n", source, header);
-#endif
-
-  memset(&idTable, 0, sizeof(IdentTable));
-  pDeclFirst = 0;
-  pDeclLast = 0;
-
-#ifdef DEBUG
-  printf("%s", source);
-#endif
-
-  pList = TokenizeFile(source, &idTable);
-
-  if (!pList) {
-    fprintf(log_file, "Errors while processing source\n");
-    return 1;
-  }
-
-  rv = ParseFile(pList, 0);
-  if (!rv) {
-    rv = build_declarations(header, log_file);
-  }
-
-  fflush(log_file);
-  FreeTokenList(pList);
-
-  return rv;
-}
+#include <stdio.h>
+
+// todo foss: tie this in with externla DEBUG macro
+// #define DEBUG (PARSER | DECL_DUMP | TOKENIZER)
+
+#define TEST 2 // foss: semi-hack to disable main() in makeheaders.c
+
+// foss: unmodified from source: https://www.hwaci.com/sw/mkhdr/
+#include "makeheaders.c"
+
+// foss: note that this code is MIT-licensed but makeheaders.c is under
+// the (seemingly compatible) 2-clause BSD license.
+
+// foss: WARNING: makeheaders keeps a lot of global state which makes
+// it awkward to use in a library. Make sure the state is reset between runs.
+
+static int build_declarations(char *header, FILE *log_file) {
+  GenState sState;
+  String outStr;
+  IdentTable includeTable;
+  Decl *pDecl;
+
+  sState.pStr = &outStr;
+  StringInit(&outStr);
+
+  sState.pTable = &includeTable;
+  memset(&includeTable, 0, sizeof(includeTable));
+  sState.zIf = 0;
+  sState.nErr = 0;
+  sState.zFilename = "(all)";
+  sState.flags = 0;
+
+  ResetDeclFlags(0);
+
+  for (pDecl = pDeclFirst; pDecl; pDecl = pDecl->pNext) {
+    DeclareObject(pDecl, &sState, 1);
+  }
+
+  ChangeIfContext(0, &sState);
+  strcpy(header, StringGet(&outStr));
+
+#ifdef DEBUG
+  fprintf(log_file, "emitting decl: '%s'\n", header);
+#endif
+
+  IdentTableReset(&includeTable);
+  StringReset(&outStr);
+  return 0;
+}
+
+int make_header(char const *source, char *header) {
+  Token *pList;
+  FILE *log_file = stdout;
+  IdentTable idTable;
+  int rv = 0;
+
+#ifdef DEBUG
+  debugMask = DEBUG;
+
+  fprintf(log_file, "%s -> %s\n", source, header);
+#endif
+
+  memset(&idTable, 0, sizeof(IdentTable));
+  pDeclFirst = 0;
+  pDeclLast = 0;
+
+#ifdef DEBUG
+  printf("%s", source);
+#endif
+
+  pList = TokenizeFile(source, &idTable);
+
+  if (!pList) {
+    fprintf(log_file, "Errors while processing source\n");
+    return 1;
+  }
+
+  rv = ParseFile(pList, 0);
+  if (!rv) {
+    rv = build_declarations(header, log_file);
+  }
+
+  fflush(log_file);
+  FreeTokenList(pList);
+
+  return rv;
+}
```

### Comparing `crelm-0.0.30a2/pyproject.toml` & `crelm-0.0.30a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[tool.poetry]
-name = "crelm"
-version = "0.0.30a2"
-description = "Utility that automates turning simple C classes into Python objects"
-authors = [
-  "WideOpenTech <foss@wideopentech.co.uk>",
-]
-readme = "README.md"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-repository = "https://github.com/wideopensource/crelm"
-
-[project.urls]
-"Homepage" = "https://github.com/wideopentech-public/crelm"
-"Bug Tracker" = "https://github.com/wideopentech-public/crelm/issues"
-
-
-[tool.poetry.dependencies]
-python = "^3.8"
-cffi = "^1.15.1"
-pexpect = "^4.8.0"
-john = "^0.1.1a2"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "crelm"
+version = "0.0.30a3"
+description = "Utility that automates turning simple C classes into Python objects"
+authors = [
+  "WideOpenTech <foss@wideopentech.co.uk>",
+]
+readme = "README.md"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+repository = "https://github.com/wideopensource/crelm"
+
+[project.urls]
+"Homepage" = "https://github.com/wideopentech-public/crelm"
+"Bug Tracker" = "https://github.com/wideopentech-public/crelm/issues"
+
+
+[tool.poetry.dependencies]
+python = "^3.8"
+cffi = "^1.15.1"
+pexpect = "^4.8.0"
+john = "^0.1.1a2"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `crelm-0.0.30a2/PKG-INFO` & `crelm-0.0.30a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crelm
-Version: 0.0.30a2
+Version: 0.0.30a3
 Summary: Utility that automates turning simple C classes into Python objects
 Home-page: https://github.com/wideopensource/crelm
 Author: WideOpenTech
 Author-email: foss@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

