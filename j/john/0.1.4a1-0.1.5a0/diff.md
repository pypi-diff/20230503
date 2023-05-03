# Comparing `tmp/john-0.1.4a1.tar.gz` & `tmp/john-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "john-0.1.4a1.tar", max compression
+gzip compressed data, was "john-0.1.5a0.tar", max compression
```

## Comparing `john-0.1.4a1.tar` & `john-0.1.5a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.4a1/LICENSE
--rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.4a1/README.md
--rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.4a1/john/__init__.py
--rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.4a1/john/factory.py
--rw-r--r--   0        0        0     1375 2023-04-24 15:49:15.036240 john-0.1.4a1/john/tdd.py
--rw-r--r--   0        0        0     7727 2023-04-24 13:38:05.344784 john-0.1.4a1/john/test_case.py
--rw-r--r--   0        0        0      681 2023-04-24 15:53:18.921369 john-0.1.4a1/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.4a1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.5a0/README.md
+-rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.5a0/john/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.5a0/john/factory.py
+-rw-r--r--   0        0        0     2090 2023-05-03 15:54:44.915729 john-0.1.5a0/john/tdd.py
+-rw-r--r--   0        0        0     7943 2023-05-03 15:55:42.420797 john-0.1.5a0/john/test_case.py
+-rw-r--r--   0        0        0      681 2023-05-03 17:03:16.264584 john-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.5a0/PKG-INFO
```

### Comparing `john-0.1.4a1/LICENSE` & `john-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `john-0.1.4a1/john/test_case.py` & `john-0.1.5a0/john/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,22 @@
         [self._helper.remove_temp_files(x) for x in (
             '*.c', '*.h', '*.so', '*.i', '*.o')]
         return unittest.TestCase.setUp(self)
 
     def writeFile(self, filename: str, text: str) -> str:
         return self._helper.write_file(self.testName, filename=filename, text=text)
 
+class AssertMixin:
+    def assertZero(self, actual, msg=None):
+        assert 0 == actual, msg
 
-# foss: based on https://stackoverflow.com/questions/4319825/python-unittest-opposite-of-assertraises
+    def assertNotZero(self, actual, msg=None):
+        assert 0 != actual, msg
+
+# foss: based on https://stackconfig = overflow.com/questions/4319825/python-unittest-opposite-of-assertraises
 is_micropython = sys.implementation.name == "micropython"
 
 if is_micropython:
     from unittest import AssertRaisesContext
 
     class AssertDoesNotRaiseContext(AssertRaisesContext):
         def __exit__(self, exc_type, exc_value, tb):
@@ -215,12 +221,12 @@
             context = _AssertDoesNotRaiseContext(expected_exception, self)
             try:
                 return context.handle('assertDoesNotRaise', args, kwargs)
             finally:
                 context = None
 
 if is_micropython:
-    class TestCase(TestCaseBase, MicropythonAssertMixin):
+    class TestCase(TestCaseBase, AssertMixin, MicropythonAssertMixin):
         pass
 else:
-    class TestCase(TestCaseBase, AssertRaisesMixin, AssertDoesNotRaiseMixin):
+    class TestCase(TestCaseBase, AssertMixin, AssertRaisesMixin, AssertDoesNotRaiseMixin):
         pass
```

### Comparing `john-0.1.4a1/pyproject.toml` & `john-0.1.5a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "john"
-version = "0.1.4a1"
+version = "0.1.5a0"
 description = "Jeneral Outlying Helper Nuggetoids"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `john-0.1.4a1/PKG-INFO` & `john-0.1.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: john
-Version: 0.1.4a1
+Version: 0.1.5a0
 Summary: Jeneral Outlying Helper Nuggetoids
 Home-page: https://github.com/wideopensource/john
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

