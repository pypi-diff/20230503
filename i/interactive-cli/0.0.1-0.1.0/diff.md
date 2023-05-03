# Comparing `tmp/interactive_cli-0.0.1.tar.gz` & `tmp/interactive_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactive_cli-0.0.1.tar", max compression
+gzip compressed data, was "interactive_cli-0.1.0.tar", max compression
```

## Comparing `interactive_cli-0.0.1.tar` & `interactive_cli-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1094 2023-04-29 11:29:41.779890 interactive_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0      374 2023-05-01 17:05:12.988203 interactive_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2189 2023-05-02 06:29:17.948332 interactive_cli-0.0.1/README.md
--rw-r--r--   0        0        0       78 2023-04-29 11:31:34.692923 interactive_cli-0.0.1/src/interactive_cli/__init__.py
--rw-r--r--   0        0        0       86 2023-05-01 17:12:18.454730 interactive_cli-0.0.1/src/interactive_cli/async_cli_app.py
--rw-r--r--   0        0        0      443 2023-05-01 18:07:00.971969 interactive_cli-0.0.1/src/interactive_cli/blocking_cli_app.py
--rw-r--r--   0        0        0     6625 2023-05-02 06:23:53.785771 interactive_cli-0.0.1/src/interactive_cli/cli_app.py
--rw-r--r--   0        0        0     1888 2023-05-01 18:08:22.270131 interactive_cli-0.0.1/src/interactive_cli/cli_command.py
--rw-r--r--   0        0        0     1903 2023-05-01 16:50:03.002555 interactive_cli-0.0.1/src/interactive_cli/cli_print_context.py
--rw-r--r--   0        0        0       26 2023-04-29 12:09:06.141619 interactive_cli-0.0.1/src/interactive_cli/static.py
--rw-r--r--   0        0        0      246 2023-05-01 16:55:55.161927 interactive_cli-0.0.1/src/interactive_cli/utils.py
--rw-r--r--   0        0        0        5 2023-04-29 11:29:41.779890 interactive_cli-0.0.1/src/interactive_cli/VERSION
--rw-r--r--   0        0        0      254 2023-04-29 11:29:41.779890 interactive_cli-0.0.1/src/interactive_cli/version.py
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 interactive_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-04-29 11:29:41.779890 interactive_cli-0.1.0/LICENSE
+-rw-r--r--   0        0        0      374 2023-05-03 07:42:08.621733 interactive_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2108 2023-05-03 07:44:01.595023 interactive_cli-0.1.0/README.md
+-rw-r--r--   0        0        0       78 2023-04-29 11:31:34.692923 interactive_cli-0.1.0/src/interactive_cli/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-03 07:40:14.007383 interactive_cli-0.1.0/src/interactive_cli/async_cli_app.py
+-rw-r--r--   0        0        0      316 2023-05-02 10:29:15.371777 interactive_cli-0.1.0/src/interactive_cli/blocking_cli_app.py
+-rw-r--r--   0        0        0     5997 2023-05-03 07:28:16.167858 interactive_cli-0.1.0/src/interactive_cli/cli_app.py
+-rw-r--r--   0        0        0     1221 2023-05-02 10:12:06.121830 interactive_cli-0.1.0/src/interactive_cli/cli_command.py
+-rw-r--r--   0        0        0     8330 2023-05-03 07:02:43.583324 interactive_cli-0.1.0/src/interactive_cli/cli_page.py
+-rw-r--r--   0        0        0     3845 2023-05-03 07:39:09.951836 interactive_cli-0.1.0/src/interactive_cli/cli_print_context.py
+-rw-r--r--   0        0        0      243 2023-05-03 07:39:09.859413 interactive_cli-0.1.0/src/interactive_cli/static.py
+-rw-r--r--   0        0        0      246 2023-05-01 16:55:55.161927 interactive_cli-0.1.0/src/interactive_cli/utils.py
+-rw-r--r--   0        0        0        5 2023-05-03 07:42:19.534036 interactive_cli-0.1.0/src/interactive_cli/VERSION
+-rw-r--r--   0        0        0      254 2023-04-29 11:29:41.779890 interactive_cli-0.1.0/src/interactive_cli/version.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 interactive_cli-0.1.0/PKG-INFO
```

### Comparing `interactive_cli-0.0.1/LICENSE` & `interactive_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactive_cli-0.0.1/README.md` & `interactive_cli-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 
 This module allows to create programs that show an interactive command line interface. The program waits for the user input and then acts on user interaction.
 
 Example:
 
 ```python
 from interactive_cli.blocking_cli_app import BlockingCLIApp
-from interactive_cli.cli_app import CLIApp
 from interactive_cli.cli_command import CLICommand
 
 
-def _hello_world(app: CLIApp) -> None:
-    app.print("Hello world!")
-
-
 if __name__ == "__main__":
-    app = BlockingCLIApp("Hello world CLI", "flow")
-    app.add_command(CLICommand("say hello world", _hello_world))
+    app = BlockingCLIApp("Hello world CLI")
+    app.add_command(
+        CLICommand("say hello world", lambda app, page: app.print("Hello world"))
+    )
 
     app.start()
 ```
 
 results in
 
 ```txt
```

### Comparing `interactive_cli-0.0.1/PKG-INFO` & `interactive_cli-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactive-cli
-Version: 0.0.1
+Version: 0.1.0
 Summary: 
 Author: miile7
 Author-email: miile7@gmx.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,25 +19,22 @@
 
 This module allows to create programs that show an interactive command line interface. The program waits for the user input and then acts on user interaction.
 
 Example:
 
 ```python
 from interactive_cli.blocking_cli_app import BlockingCLIApp
-from interactive_cli.cli_app import CLIApp
 from interactive_cli.cli_command import CLICommand
 
 
-def _hello_world(app: CLIApp) -> None:
-    app.print("Hello world!")
-
-
 if __name__ == "__main__":
-    app = BlockingCLIApp("Hello world CLI", "flow")
-    app.add_command(CLICommand("say hello world", _hello_world))
+    app = BlockingCLIApp("Hello world CLI")
+    app.add_command(
+        CLICommand("say hello world", lambda app, page: app.print("Hello world"))
+    )
 
     app.start()
 ```
 
 results in
 
 ```txt
```

