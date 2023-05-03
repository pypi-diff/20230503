# Comparing `tmp/foxplot-0.0.1.tar.gz` & `tmp/foxplot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxplot-0.0.1.tar", last modified: Tue Apr 25 15:12:23 2023, max compression
+gzip compressed data, was "foxplot-0.0.2.tar", last modified: Wed May  3 10:10:49 2023, max compression
```

## Comparing `foxplot-0.0.1.tar` & `foxplot-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,38 @@
--rw-r--r--   0        0        0     2753 2023-01-26 08:59:41.538467 foxplot-0.0.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0       49 2023-01-26 08:59:41.538467 foxplot-0.0.1/.gitignore
--rw-r--r--   0        0        0      314 2023-04-25 15:09:21.743404 foxplot-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-01-26 08:59:41.542467 foxplot-0.0.1/LICENSE
--rw-r--r--   0        0        0       30 2023-01-26 08:59:41.542467 foxplot-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     1503 2023-04-25 15:11:35.289610 foxplot-0.0.1/README.md
--rw-r--r--   0        0        0     1073 2023-04-25 14:58:06.539529 foxplot-0.0.1/examples/plot_robot_data.py
--rw-r--r--   0        0        0   128378 2023-04-25 14:37:52.909959 foxplot-0.0.1/examples/robot_data.json
--rw-r--r--   0        0        0      747 2023-04-25 14:46:18.345520 foxplot-0.0.1/foxplot/__init__.py
--rw-r--r--   0        0        0     2971 2023-04-25 15:05:08.783198 foxplot-0.0.1/foxplot/cli.py
--rw-r--r--   0        0        0     1442 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/color_picker.py
--rw-r--r--   0        0        0      719 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/decoders/__init__.py
--rw-r--r--   0        0        0     1469 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/decoders/json.py
--rw-r--r--   0        0        0      736 2023-04-24 09:36:48.809711 foxplot-0.0.1/foxplot/exceptions.py
--rw-r--r--   0        0        0     4806 2023-04-25 15:08:48.451871 foxplot-0.0.1/foxplot/fox.py
--rw-r--r--   0        0        0     8177 2023-04-25 14:54:35.265360 foxplot-0.0.1/foxplot/generate_html.py
--rw-r--r--   0        0        0     1597 2023-04-25 14:56:10.622539 foxplot-0.0.1/foxplot/indexed_series.py
--rw-r--r--   0        0        0     3231 2023-04-25 14:56:38.401779 foxplot-0.0.1/foxplot/node.py
--rw-r--r--   0        0        0   120184 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/uPlot/uPlot.iife.js
--rw-r--r--   0        0        0     1839 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/uPlot/uPlot.min.css
--rw-r--r--   0        0        0     4543 2023-04-12 16:50:56.668776 foxplot-0.0.1/foxplot/uPlot/uPlot.mousewheel.js
--rw-r--r--   0        0        0     1205 2023-04-25 14:19:33.129645 foxplot-0.0.1/foxplot/write_tmpfile.py
--rw-r--r--   0        0        0     1529 2023-04-24 12:26:58.318170 foxplot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-01-26 08:59:41.542467 foxplot-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-04 12:24:42.147920 foxplot-0.0.1/tests/test_color_picker.py
--rw-r--r--   0        0        0     1318 2023-04-04 12:24:42.147920 foxplot-0.0.1/tests/test_decoders.py
--rw-r--r--   0        0        0     6603 2023-04-24 12:24:53.005389 foxplot-0.0.1/tests/test_fox.py
--rw-r--r--   0        0        0     1074 2023-04-24 11:57:18.540637 foxplot-0.0.1/tests/test_generate_html.py
--rw-r--r--   0        0        0      674 2023-01-26 08:59:41.542467 foxplot-0.0.1/tox.ini
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 foxplot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2700 2023-05-03 10:05:19.625704 foxplot-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1270 2023-05-03 10:05:32.381708 foxplot-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       62 2023-05-03 10:05:19.625704 foxplot-0.0.2/.gitignore
+-rw-r--r--   0        0        0      373 2023-05-03 09:37:34.286589 foxplot-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-01-26 08:59:41.542467 foxplot-0.0.2/LICENSE
+-rw-r--r--   0        0        0       30 2023-01-26 08:59:41.542467 foxplot-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     2262 2023-05-03 10:05:19.625704 foxplot-0.0.2/README.md
+-rw-r--r--   0        0        0       51 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/api.rst
+-rw-r--r--   0        0        0     9358 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0      204 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/environment.yml
+-rw-r--r--   0        0        0      253 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/index.rst
+-rw-r--r--   0        0        0      202 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/installation.rst
+-rw-r--r--   0        0        0     1003 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/usage.rst
+-rw-r--r--   0        0        0     1073 2023-04-25 14:58:06.539529 foxplot-0.0.2/examples/plot_robot_data.py
+-rw-r--r--   0        0        0   128378 2023-04-25 14:37:52.909959 foxplot-0.0.2/examples/robot_data.json
+-rw-r--r--   0        0        0      747 2023-05-03 09:37:39.262562 foxplot-0.0.2/foxplot/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/cli.py
+-rw-r--r--   0        0        0     1442 2023-05-02 15:36:42.759188 foxplot-0.0.2/foxplot/color_picker.py
+-rw-r--r--   0        0        0      777 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/decoders/__init__.py
+-rw-r--r--   0        0        0     1469 2023-05-02 15:36:46.319031 foxplot-0.0.2/foxplot/decoders/json.py
+-rw-r--r--   0        0        0     1302 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/decoders/msgpack.py
+-rw-r--r--   0        0        0      736 2023-05-02 15:36:38.119141 foxplot-0.0.2/foxplot/exceptions.py
+-rw-r--r--   0        0        0     5667 2023-05-03 09:37:04.510756 foxplot-0.0.2/foxplot/fox.py
+-rw-r--r--   0        0        0     8177 2023-05-02 15:36:35.263076 foxplot-0.0.2/foxplot/generate_html.py
+-rw-r--r--   0        0        0     1597 2023-04-25 14:56:10.622539 foxplot-0.0.2/foxplot/indexed_series.py
+-rw-r--r--   0        0        0     3231 2023-04-25 14:56:38.401779 foxplot-0.0.2/foxplot/node.py
+-rw-r--r--   0        0        0   120184 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.iife.js
+-rw-r--r--   0        0        0     1839 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.min.css
+-rw-r--r--   0        0        0     4543 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.mousewheel.js
+-rw-r--r--   0        0        0     1205 2023-04-25 14:19:33.129645 foxplot-0.0.2/foxplot/write_tmpfile.py
+-rw-r--r--   0        0        0     1529 2023-04-24 12:26:58.318170 foxplot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-01-26 08:59:41.542467 foxplot-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-04 12:24:42.147920 foxplot-0.0.2/tests/test_color_picker.py
+-rw-r--r--   0        0        0     1739 2023-05-03 09:37:04.510756 foxplot-0.0.2/tests/test_decoders.py
+-rw-r--r--   0        0        0     6603 2023-04-24 12:24:53.005389 foxplot-0.0.2/tests/test_fox.py
+-rw-r--r--   0        0        0     1074 2023-04-24 11:57:18.540637 foxplot-0.0.2/tests/test_generate_html.py
+-rw-r--r--   0        0        0      739 2023-05-03 09:37:04.510756 foxplot-0.0.2/tox.ini
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 foxplot-0.0.2/PKG-INFO
```

### Comparing `foxplot-0.0.1/.github/workflows/CI.yml` & `foxplot-0.0.2/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,26 @@
         name: "Code style"
         runs-on: ubuntu-latest
 
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v3
 
-            - name: "Set up Python ${{ matrix.python-version }}"
+            - name: "Set up Python 3.9"
               uses: actions/setup-python@v4
               with:
-                  python-version: "${{ matrix.python-version }}"
+                  python-version: "3.9"
 
             - name: "Install dependencies"
               run: |
                   python -m pip install --upgrade pip
                   # tox version: https://github.com/tox-dev/tox/issues/2778
                   python -m pip install tox==3.28.0
 
-            - name: "Test with tox for ${{ matrix.os }}"
+            - name: "Test with tox for ubuntu-latest"
               run: |
                   tox -e lint
               env:
                   PLATFORM: ubuntu-latest
 
     coverage:
         name: "Coverage"
```

### Comparing `foxplot-0.0.1/LICENSE` & `foxplot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/examples/plot_robot_data.py` & `foxplot-0.0.2/examples/plot_robot_data.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/examples/robot_data.json` & `foxplot-0.0.2/examples/robot_data.json`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/__init__.py` & `foxplot-0.0.2/foxplot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Plot time-series data from line-delimited JSON."""
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from .fox import Fox
 
 __all__ = ["Fox"]
```

### Comparing `foxplot-0.0.1/foxplot/cli.py` & `foxplot-0.0.2/foxplot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 def main() -> None:
     """Entry point for command-line execution."""
     args = parse_command_line_arguments()
 
     fox = Fox(from_file=args.file, time=args.time)
     if args.file is None:
-        fox.read_from_file(sys.stdin)
+        fox.read_from_json(sys.stdin)
 
     if args.interactive:
         __import__("IPython").embed()
     else:  # not args.interactive
         left_labels = args.left if args.left else []
         right_labels = args.right if args.right else []
         left_series = [fox.get_series(label) for label in left_labels]
```

### Comparing `foxplot-0.0.1/foxplot/color_picker.py` & `foxplot-0.0.2/foxplot/color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/decoders/__init__.py` & `foxplot-0.0.2/foxplot/decoders/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Decoder functions."""
 
 from .json import decode_json
+from .msgpack import decode_msgpack
 
 __all__ = [
     "decode_json",
+    "decode_msgpack",
 ]
```

### Comparing `foxplot-0.0.1/foxplot/decoders/json.py` & `foxplot-0.0.2/foxplot/decoders/json.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/exceptions.py` & `foxplot-0.0.2/foxplot/exceptions.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/fox.py` & `foxplot-0.0.2/foxplot/fox.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Main class to manipulate dictionary-series data."""
 
+import sys
 import webbrowser
-from typing import List, Optional, TextIO
+from typing import BinaryIO, List, Optional, TextIO
 
 from .decoders.json import decode_json
+from .decoders.msgpack import decode_msgpack
 from .generate_html import generate_html
 from .indexed_series import IndexedSeries
 from .node import Node
 from .write_tmpfile import write_tmpfile
 
 
 class Fox:
@@ -46,16 +48,15 @@
             time: Label of time index in input dictionaries.
         """
         self.__file = from_file
         self.__time = time
         self.data = Node("/")
         self.length = 0
         if from_file:
-            with open(from_file, "r", encoding="utf-8") as file:
-                self.read_from_file(file)
+            self.read_from_file(from_file)
 
     def get_series(self, label: str) -> IndexedSeries:
         """Get time-series data from a given label.
 
         Args:
             label: Label to the data in input dictionaries, for example
                 ``/observation/cpu_temperature``.
@@ -122,23 +123,47 @@
         right_args = ("-r " if right_series else "") + " ".join(
             right_series.keys()
         )
         file = f"{self.__file} " if self.__file is not None else ""
         time = f"-t {self.__time} " if self.__time else ""
         print(f"foxplot {file}{time}-l {left_args} {right_args}")
 
-    def read_from_file(self, file: TextIO) -> None:
+    def read_from_file(self, filename: str) -> None:
         """Process time series data.
 
         Args:
-            file: File to read time series from.
+            filename: Name of a file to read time series from.
+        """
+        if filename == "stdin":
+            self.read_from_json(sys.stdin)
+        elif filename.endswith(".json"):
+            with open(filename, "r", encoding="utf-8") as file:
+                self.read_from_json(file)
+        elif filename.endswith(".mpack"):
+            with open(filename, "rb") as file:
+                self.read_from_msgpack(file)
+
+    def read_from_json(self, file: TextIO) -> None:
+        """Process time series data from a JSON stream.
+
+        Args:
+            file: JSON stream to read time series from.
         """
         for unpacked in decode_json(file=file):
             self.unpack(unpacked)
 
+    def read_from_msgpack(self, file: BinaryIO) -> None:
+        """Process time series data from a MessagePack stream.
+
+        Args:
+            file: MessagePack stream to read time series from.
+        """
+        for unpacked in decode_msgpack(file=file):
+            self.unpack(unpacked)
+
     def set_time(self, time: str):
         """Set label of time index in input dictionaries.
 
         Args:
             time: Label of time index in input dictionaries.
         """
         self.__time = time
```

### Comparing `foxplot-0.0.1/foxplot/generate_html.py` & `foxplot-0.0.2/foxplot/generate_html.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/indexed_series.py` & `foxplot-0.0.2/foxplot/indexed_series.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/node.py` & `foxplot-0.0.2/foxplot/node.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/uPlot/uPlot.iife.js` & `foxplot-0.0.2/foxplot/uPlot/uPlot.iife.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/uPlot/uPlot.min.css` & `foxplot-0.0.2/foxplot/uPlot/uPlot.min.css`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/uPlot/uPlot.mousewheel.js` & `foxplot-0.0.2/foxplot/uPlot/uPlot.mousewheel.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/foxplot/write_tmpfile.py` & `foxplot-0.0.2/foxplot/write_tmpfile.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/pyproject.toml` & `foxplot-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/tests/test_color_picker.py` & `foxplot-0.0.2/tests/test_color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/tests/test_decoders.py` & `foxplot-0.0.2/tests/test_decoders.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,30 +15,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import tempfile
 import unittest
 
-from foxplot.decoders import decode_json
+import msgpack
 
+from foxplot.decoders import decode_json, decode_msgpack
 
-class TestDecoders(unittest.TestCase):
 
+class TestDecoders(unittest.TestCase):
     EXPECTED_DICTS = [
         {"a": 1, "b": 2},
         {"c": 3, "d": 4},
     ]
 
     def setUp(self):
         self.json_file = tempfile.NamedTemporaryFile(mode="w+")
+        self.msgpack_file = tempfile.NamedTemporaryFile(mode="wb+")
         for d in self.EXPECTED_DICTS:
             self.json_file.file.write(json.dumps(d) + "\n")
+            self.msgpack_file.file.write(msgpack.packb(d))
         self.json_file.file.seek(0)
+        self.msgpack_file.file.seek(0)
 
     def tearDown(self):
         self.json_file.close()
 
     def test_decode_json(self):
         read_dicts = list(decode_json(file=self.json_file.file))
         for read, expected in zip(read_dicts, self.EXPECTED_DICTS):
             self.assertDictEqual(read, expected)
+
+    def test_decode_msgpack(self):
+        read_dicts = list(decode_msgpack(file=self.msgpack_file.file))
+        for read, expected in zip(read_dicts, self.EXPECTED_DICTS):
+            self.assertDictEqual(read, expected)
```

### Comparing `foxplot-0.0.1/tests/test_fox.py` & `foxplot-0.0.2/tests/test_fox.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/tests/test_generate_html.py` & `foxplot-0.0.2/tests/test_generate_html.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.1/tox.ini` & `foxplot-0.0.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
 
 [testenv]
 deps =
+    msgpack >=1.0.4
     pytest >=7.1.2
 commands =
     pytest tests
 
 [testenv:coverage]
 deps =
     coverage >=5.5
+    msgpack >=1.0.4
 commands =
     coverage erase
     coverage run -m unittest discover
     coverage report --include="foxplot/**"
 
 [testenv:lint]
 deps =
@@ -33,8 +35,8 @@
     pylint >=2.8.2
     ruff >=0.0.220
     types-setuptools >=65.6.0.2
 commands =
     black --check --diff foxplot
     ruff foxplot
     pylint foxplot --exit-zero --rcfile={toxinidir}/tox.ini
-    mypy foxplot
+    mypy foxplot --ignore-missing-imports
```

### Comparing `foxplot-0.0.1/PKG-INFO` & `foxplot-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxplot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plot time-series data from line-delimited JSON.
 Keywords: json,time,series,plot
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -20,46 +20,57 @@
 Project-URL: Changelog, https://github.com/stephane-caron/foxplot/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/stephane-caron/foxplot
 Project-URL: Tracker, https://github.com/stephane-caron/foxplot/issues
 
 # foxplot
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/CI.yml?branch=main)](https://github.com/stephane-caron/foxplot/actions)
+[![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/foxplot/)
 
 Plot time-series data from [line-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Line-delimited_JSON).
 
 Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case (robotic control loops). Dictionaries are the observation format used in [Vulp](https://github.com/tasts-robots/vulp). Plots are plots :wink:
 
+## Installation
+
+```console
+$ pip install foxplot
+```
+
 ## Usage
 
 ### Interactive mode
 
-```console
-$ foxplot -i robot_data.json
+In interactive mode, you can explore the data in ``fox.data`` (tab completion works) and plot it using the ``fox.plot`` function:
+
+```python
+$ foxplot -i upkie_2023-05-03-103245.mpack
 Python 3.8.10 (default, Mar 13 2023, 10:26:41)
 Type 'copyright', 'credits' or 'license' for more information
-IPython 7.22.0 -- An enhanced Interactive Python. Type '?' for help.
+IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
 
-In [1]: fox.plot(left=[fox.data.observation.cpu_temperature])
+In [1]: fox.plot(
+   ...:     [
+   ...:         fox.data.observation.servo.left_knee.torque,
+   ...:         fox.data.observation.servo.left_wheel.torque,
+   ...:     ],
+   ...:     right=[
+   ...:         fox.data.observation.servo.left_knee.velocity,
+   ...:         fox.data.observation.servo.left_wheel.velocity,
+   ...:     ],
+   ...: )
 New tab opened in your web browser! The command line is to produce it directly is:
 
-foxplot robot_data.json -l /observation/cpu_temperature
+foxplot upkie_2023-05-03-103245.mpack -l /observation/servo/left_knee/torque /observation/servo/left_wheel/torque -r /observation/servo/left_knee/velocity /observation/servo/left_wheel/velocity
 ```
 
-### JSON files
+### Plotting from files
 
-```console
-foxplot robot_data.json -l /observation/cpu_temperature
-```
-
-### MessagePack files
-
-```console
-rq -mJ < my_time_series.mpack | jq '{.my.filters.here}' | foxplot
-```
+- JSON: ``foxplot my_data.json -l /observation/cpu_temperature``
+- MessagePack: ``foxplot my_data.mpack -l /observation/cpu_temperature``
 
 ## Design notes
 
 * Foxplot prioritizes ease-of-use (interactive mode) over performance
 
 ## See also
```

