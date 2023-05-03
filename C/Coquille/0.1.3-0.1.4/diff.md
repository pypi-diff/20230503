# Comparing `tmp/Coquille-0.1.3.tar.gz` & `tmp/Coquille-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-0.1.3.tar", last modified: Tue May  2 21:50:24 2023, max compression
+gzip compressed data, was "Coquille-0.1.4.tar", last modified: Wed May  3 12:15:11 2023, max compression
```

## Comparing `Coquille-0.1.3.tar` & `Coquille-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.3/.gitignore
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.3/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-02 21:50:24.454930 Coquille-0.1.3/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2515 2023-05-02 21:48:53.000000 Coquille-0.1.3/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.451597 Coquille-0.1.3/examples/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/examples/coquille_context/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.3/examples/coquille_context/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.3/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/examples/coquille_print/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/output.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    35689 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/screenshot.png
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 21:50:18.000000 Coquille-0.1.3/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 21:50:24.454930 Coquille-0.1.3/setup.cfg
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.3/setup.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.451597 Coquille-0.1.3/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/src/Coquille.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/src/coquille/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.3/src/coquille/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5731 2023-05-02 21:36:06.000000 Coquille-0.1.3/src/coquille/coquille.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.3/src/coquille/sequences.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.3/src/coquille/typeshed.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/tests/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/coquille_test.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/sequences_test.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.4/.gitignore
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.4/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-03 12:15:11.740973 Coquille-0.1.4/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2515 2023-05-03 12:04:51.000000 Coquille-0.1.4/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/examples/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/examples/coquille_context/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.4/examples/coquille_context/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.4/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/examples/coquille_write/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/output.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    44980 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/screenshot.png
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-03 12:14:56.000000 Coquille-0.1.4/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-03 12:15:11.740973 Coquille-0.1.4/setup.cfg
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.4/setup.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/src/Coquille.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/src/coquille/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.4/src/coquille/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     6283 2023-05-03 12:14:29.000000 Coquille-0.1.4/src/coquille/coquille.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.4/src/coquille/sequences.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.4/src/coquille/typeshed.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/tests/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/coquille_test.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/sequences_test.py
```

### Comparing `Coquille-0.1.3/.gitignore` & `Coquille-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/.pre-commit-config.yaml` & `Coquille-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/LICENSE` & `Coquille-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/PKG-INFO` & `Coquille-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.3
+Version: 0.1.4
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -73,29 +73,29 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.print()
+### Coquille.write()
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.print("Hello World, but in magenta and italic!", fg_magenta, italic)
+Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
 
-with open("examples/coquille_print/output.txt", "w") as my_file:
-    Coquille.print("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+with open("examples/coquille_write/output.txt", "w") as my_file:
+    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
 
 ```
 
-![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_print/screenshot.png)
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
-Source code: [examples/coquille_print/](https://github.com/qexat/Coquille/blob/main/examples/coquille_print/__main__.py)
+Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
 
 ## Documentation
 
 Coming soon! 🚧
```

### Comparing `Coquille-0.1.3/README.md` & `Coquille-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -60,29 +60,29 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.print()
+### Coquille.write()
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.print("Hello World, but in magenta and italic!", fg_magenta, italic)
+Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
 
-with open("examples/coquille_print/output.txt", "w") as my_file:
-    Coquille.print("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+with open("examples/coquille_write/output.txt", "w") as my_file:
+    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
 
 ```
 
-![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_print/screenshot.png)
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
-Source code: [examples/coquille_print/](https://github.com/qexat/Coquille/blob/main/examples/coquille_print/__main__.py)
+Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
 
 ## Documentation
 
 Coming soon! 🚧
```

### Comparing `Coquille-0.1.3/examples/coquille_context/screenshot.png` & `Coquille-0.1.4/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/src/Coquille.egg-info/PKG-INFO` & `Coquille-0.1.4/src/Coquille.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.3
+Version: 0.1.4
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -73,29 +73,29 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.print()
+### Coquille.write()
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.print("Hello World, but in magenta and italic!", fg_magenta, italic)
+Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
 
-with open("examples/coquille_print/output.txt", "w") as my_file:
-    Coquille.print("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+with open("examples/coquille_write/output.txt", "w") as my_file:
+    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
 
 ```
 
-![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_print/screenshot.png)
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
-Source code: [examples/coquille_print/](https://github.com/qexat/Coquille/blob/main/examples/coquille_print/__main__.py)
+Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
 
 ## Documentation
 
 Coming soon! 🚧
```

### Comparing `Coquille-0.1.3/src/Coquille.egg-info/SOURCES.txt` & `Coquille-0.1.4/src/Coquille.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.py
 examples/coquille_context/__main__.py
 examples/coquille_context/screenshot.png
-examples/coquille_print/__main__.py
-examples/coquille_print/output.txt
-examples/coquille_print/screenshot.png
+examples/coquille_write/__main__.py
+examples/coquille_write/output.txt
+examples/coquille_write/screenshot.png
 src/Coquille.egg-info/PKG-INFO
 src/Coquille.egg-info/SOURCES.txt
 src/Coquille.egg-info/dependency_links.txt
 src/Coquille.egg-info/requires.txt
 src/Coquille.egg-info/top_level.txt
 src/coquille/__init__.py
 src/coquille/coquille.py
```

### Comparing `Coquille-0.1.3/src/coquille/coquille.py` & `Coquille-0.1.4/src/coquille/coquille.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,14 +130,34 @@
     def reset(self) -> None:
         """
         Reset the currently active escape sequences of the `with` block.
         """
 
         apply(soft_reset, self.file)
 
+    def print(
+        self,
+        *values: object,
+        sep: str | None = None,
+        end: str | None = "\n",
+    ) -> None:
+        """
+        Convenient function to print in the same file as the coquille's one.
+
+        ## Example
+
+        ```py
+        >>> with Coquille.new(bold, fg_red, file=sys.stderr) as coquille:
+        ...     # same as: print("My pretty error message", file=coquille.file)
+        ...     coquille.print("My pretty error message")
+        ```
+        """
+
+        print(*values, sep=sep, end=end, file=self.file)
+
 
 @dataclass(slots=True)
 class Coquille:
     sequences: list[EscapeSequence]
     file: SupportsWrite[str] | None
 
     @overload
@@ -163,29 +183,29 @@
         """
         Convenient constructor for a Coquille.
         """
 
         return cls(list(sequences), file)
 
     @staticmethod
-    def print(
+    def write(
         text: str,
         *sequences: EscapeSequence,
         end: str | None = "\n",
         file: SupportsWrite[str] | None = None,
     ) -> None:
         """
         A function relatively similar to built-in `print`, but with
         support of escape sequences that are prepended to the printed
         text.
 
         Example:
         ```py
         >>> from coquille.sequences import fg_magenta, italic
-        >>> Coquille.print("Hello World!", fg_magenta, italic)
+        >>> Coquille.write("Hello World!", fg_magenta, italic)
         Hello World!
         ```
         Here, "Hello World!" is printed in italic and magenta, but this
         cannot be reproduced exactly in docstrings.
 
         The previous example is roughly the same as doing:
         ```py
```

### Comparing `Coquille-0.1.3/src/coquille/sequences.py` & `Coquille-0.1.4/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/tests/coquille_test.py` & `Coquille-0.1.4/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.3/tests/sequences_test.py` & `Coquille-0.1.4/tests/sequences_test.py`

 * *Files identical despite different names*

