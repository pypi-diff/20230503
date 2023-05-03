# Comparing `tmp/frida-tools-9.2.4.tar.gz` & `tmp/frida-tools-9.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/frida-tools-9.2.4.tar", last modified: Thu Apr 15 09:27:22 2021, max compression
+gzip compressed data, was "dist/frida-tools-9.2.5.tar", last modified: Thu May 27 23:25:46 2021, max compression
```

## Comparing `frida-tools-9.2.4.tar` & `frida-tools-9.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-04-15 09:27:22.321757 frida-tools-9.2.4/
--rw-r--r--   0 oleavr     (501) staff       (20)     1500 2021-04-15 09:27:22.321635 frida-tools-9.2.4/PKG-INFO
--rw-r--r--   0 oleavr     (501) staff       (20)      568 2021-03-25 21:39:15.000000 frida-tools-9.2.4/README.md
-drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-04-15 09:27:22.320727 frida-tools-9.2.4/frida_tools/
--rw-r--r--   0 oleavr     (501) staff       (20)       24 2021-03-02 23:18:49.000000 frida-tools-9.2.4/frida_tools/__init__.py
--rw-r--r--   0 oleavr     (501) staff       (20)    23173 2021-04-15 09:24:53.000000 frida-tools-9.2.4/frida_tools/application.py
--rw-r--r--   0 oleavr     (501) staff       (20)     6356 2021-04-15 09:24:53.000000 frida-tools-9.2.4/frida_tools/creator.py
--rw-r--r--   0 oleavr     (501) staff       (20)     7062 2021-03-02 23:18:49.000000 frida-tools-9.2.4/frida_tools/discoverer.py
--rw-r--r--   0 oleavr     (501) staff       (20)     1085 2021-04-15 09:24:53.000000 frida-tools-9.2.4/frida_tools/kill.py
--rw-r--r--   0 oleavr     (501) staff       (20)     3084 2021-03-02 23:18:49.000000 frida-tools-9.2.4/frida_tools/lsd.py
--rw-r--r--   0 oleavr     (501) staff       (20)     2381 2021-03-02 23:18:49.000000 frida-tools-9.2.4/frida_tools/model.py
--rw-r--r--   0 oleavr     (501) staff       (20)     6958 2021-03-30 21:24:07.000000 frida-tools-9.2.4/frida_tools/ps.py
--rw-r--r--   0 oleavr     (501) staff       (20)    39968 2021-03-25 21:39:27.000000 frida-tools-9.2.4/frida_tools/repl.py
--rw-r--r--   0 oleavr     (501) staff       (20)    29015 2021-03-02 23:18:49.000000 frida-tools-9.2.4/frida_tools/tracer.py
--rw-r--r--   0 oleavr     (501) staff       (20)    25315 2021-04-15 09:27:14.000000 frida-tools-9.2.4/frida_tools/tracer_agent.js
-drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-04-15 09:27:22.321482 frida-tools-9.2.4/frida_tools.egg-info/
--rw-r--r--   0 oleavr     (501) staff       (20)     1500 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/PKG-INFO
--rw-r--r--   0 oleavr     (501) staff       (20)      508 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/SOURCES.txt
--rw-r--r--   0 oleavr     (501) staff       (20)        1 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/dependency_links.txt
--rw-r--r--   0 oleavr     (501) staff       (20)      278 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/entry_points.txt
--rw-r--r--   0 oleavr     (501) staff       (20)       97 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/requires.txt
--rw-r--r--   0 oleavr     (501) staff       (20)       12 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/top_level.txt
--rw-r--r--   0 oleavr     (501) staff       (20)        1 2021-04-15 09:27:22.000000 frida-tools-9.2.4/frida_tools.egg-info/zip-safe
--rw-r--r--   0 oleavr     (501) staff       (20)       38 2021-04-15 09:27:22.321793 frida-tools-9.2.4/setup.cfg
--rwxr-xr-x   0 oleavr     (501) staff       (20)     2556 2021-04-15 09:26:24.000000 frida-tools-9.2.4/setup.py
+drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-05-27 23:25:46.606449 frida-tools-9.2.5/
+-rw-r--r--   0 oleavr     (501) staff       (20)     1500 2021-05-27 23:25:46.606333 frida-tools-9.2.5/PKG-INFO
+-rw-r--r--   0 oleavr     (501) staff       (20)      568 2021-03-25 21:39:15.000000 frida-tools-9.2.5/README.md
+drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-05-27 23:25:46.605378 frida-tools-9.2.5/frida_tools/
+-rw-r--r--   0 oleavr     (501) staff       (20)       24 2021-03-02 23:18:49.000000 frida-tools-9.2.5/frida_tools/__init__.py
+-rw-r--r--   0 oleavr     (501) staff       (20)    23173 2021-05-27 23:24:15.000000 frida-tools-9.2.5/frida_tools/application.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     6356 2021-05-27 23:24:15.000000 frida-tools-9.2.5/frida_tools/creator.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     7062 2021-03-02 23:18:49.000000 frida-tools-9.2.5/frida_tools/discoverer.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     1085 2021-05-27 23:24:15.000000 frida-tools-9.2.5/frida_tools/kill.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     3084 2021-03-02 23:18:49.000000 frida-tools-9.2.5/frida_tools/lsd.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     2381 2021-03-02 23:18:49.000000 frida-tools-9.2.5/frida_tools/model.py
+-rw-r--r--   0 oleavr     (501) staff       (20)     6958 2021-03-30 21:24:07.000000 frida-tools-9.2.5/frida_tools/ps.py
+-rw-r--r--   0 oleavr     (501) staff       (20)    40321 2021-05-27 23:24:18.000000 frida-tools-9.2.5/frida_tools/repl.py
+-rw-r--r--   0 oleavr     (501) staff       (20)    29033 2021-05-27 23:24:18.000000 frida-tools-9.2.5/frida_tools/tracer.py
+-rw-r--r--   0 oleavr     (501) staff       (20)    25315 2021-05-27 23:24:30.000000 frida-tools-9.2.5/frida_tools/tracer_agent.js
+drwxr-xr-x   0 oleavr     (501) staff       (20)        0 2021-05-27 23:25:46.606164 frida-tools-9.2.5/frida_tools.egg-info/
+-rw-r--r--   0 oleavr     (501) staff       (20)     1500 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/PKG-INFO
+-rw-r--r--   0 oleavr     (501) staff       (20)      508 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 oleavr     (501) staff       (20)        1 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 oleavr     (501) staff       (20)      278 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/entry_points.txt
+-rw-r--r--   0 oleavr     (501) staff       (20)       97 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/requires.txt
+-rw-r--r--   0 oleavr     (501) staff       (20)       12 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/top_level.txt
+-rw-r--r--   0 oleavr     (501) staff       (20)        1 2021-05-27 23:25:46.000000 frida-tools-9.2.5/frida_tools.egg-info/zip-safe
+-rw-r--r--   0 oleavr     (501) staff       (20)       38 2021-05-27 23:25:46.606485 frida-tools-9.2.5/setup.cfg
+-rwxr-xr-x   0 oleavr     (501) staff       (20)     2556 2021-05-27 23:24:56.000000 frida-tools-9.2.5/setup.py
```

### Comparing `frida-tools-9.2.4/PKG-INFO` & `frida-tools-9.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-tools
-Version: 9.2.4
+Version: 9.2.5
 Summary: Frida CLI tools
 Home-page: https://frida.re
 Author: Frida Developers
 Author-email: oleavr@frida.re
 License: wxWindows Library Licence, Version 3.1
 Description: CLI tools for [Frida](https://frida.re).
 Keywords: frida debugger dynamic instrumentation inject javascript windows macos linux ios iphone ipad android qnx
```

### Comparing `frida-tools-9.2.4/README.md` & `frida-tools-9.2.5/README.md`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/application.py` & `frida-tools-9.2.5/frida_tools/application.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/creator.py` & `frida-tools-9.2.5/frida_tools/creator.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/discoverer.py` & `frida-tools-9.2.5/frida_tools/discoverer.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/kill.py` & `frida-tools-9.2.5/frida_tools/kill.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/lsd.py` & `frida-tools-9.2.5/frida_tools/lsd.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/model.py` & `frida-tools-9.2.5/frida_tools/model.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/ps.py` & `frida-tools-9.2.5/frida_tools/ps.py`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools/repl.py` & `frida-tools-9.2.5/frida_tools/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
                     ("completion-menu.completion.current", "bg:#ef6456 #3d3d3d"),
                 ])
                 history = FileHistory(os.path.join(config_dir, 'history'))
                 self._cli = PromptSession(lexer=PygmentsLexer(JavascriptLexer),
                                           style=style,
                                           history=history,
                                           completer=self._completer,
-                                          complete_in_thread=True)
+                                          complete_in_thread=True,
+                                          enable_open_in_editor=True,
+                                          tempfile_suffix=".js")
                 self._dumb_stdin_reader = None
             else:
                 self._cli = None
                 self._dumb_stdin_reader = DumbStdinReader(valid_until=self._stopping.is_set)
 
             if not self._have_terminal:
                 self._rpc_complete_server = start_completion_thread(self)
@@ -771,14 +773,17 @@
                         # so we just use the simplest value with that type
                         if t[0] in Token.Literal.String.subtypes:
                             before_dot = '""' + before_dot
                         elif t[0] in Token.Literal.Number.subtypes:
                             before_dot = '0.0' + before_dot
                         elif t[0] == Token.Punctuation and t[1] == ']':
                             before_dot = '[]' + before_dot
+                        elif t[0] == Token.Punctuation and t[1] == ')':
+                            # we don't know the returned value of the function call so we abort the completion
+                            return
 
                     break
 
             try:
                 if encountered_dot:
                     if before_dot == "" or before_dot.endswith("."):
                         return
```

### Comparing `frida-tools-9.2.4/frida_tools/tracer.py` & `frida-tools-9.2.5/frida_tools/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
             pb = TracerProfileBuilder()
             def process_builder_arg(option, opt_str, value, parser, method, **kwargs):
                 method(value)
             parser.add_option("-I", "--include-module", help="include MODULE", metavar="MODULE",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.include_modules,))
             parser.add_option("-X", "--exclude-module", help="exclude MODULE", metavar="MODULE",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.exclude_modules,))
-            parser.add_option("-i", "--include", help="include FUNCTION", metavar="FUNCTION",
+            parser.add_option("-i", "--include", help="include [MODULE!]FUNCTION", metavar="FUNCTION",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.include,))
-            parser.add_option("-x", "--exclude", help="exclude FUNCTION", metavar="FUNCTION",
+            parser.add_option("-x", "--exclude", help="exclude [MODULE!]FUNCTION", metavar="FUNCTION",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.exclude,))
             parser.add_option("-a", "--add", help="add MODULE!OFFSET", metavar="MODULE!OFFSET",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.include_relative_address,))
             parser.add_option("-T", "--include-imports", help="include program's imports",
                     action='callback', callback=process_builder_arg, callback_args=(pb.include_imports,))
             parser.add_option("-t", "--include-module-imports", help="include MODULE imports", metavar="MODULE",
                     type='string', action='callback', callback=process_builder_arg, callback_args=(pb.include_imports,))
```

### Comparing `frida-tools-9.2.4/frida_tools/tracer_agent.js` & `frida-tools-9.2.5/frida_tools/tracer_agent.js`

 * *Files identical despite different names*

### Comparing `frida-tools-9.2.4/frida_tools.egg-info/PKG-INFO` & `frida-tools-9.2.5/frida_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-tools
-Version: 9.2.4
+Version: 9.2.5
 Summary: Frida CLI tools
 Home-page: https://frida.re
 Author: Frida Developers
 Author-email: oleavr@frida.re
 License: wxWindows Library Licence, Version 3.1
 Description: CLI tools for [Frida](https://frida.re).
 Keywords: frida debugger dynamic instrumentation inject javascript windows macos linux ios iphone ipad android qnx
```

### Comparing `frida-tools-9.2.4/setup.py` & `frida-tools-9.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 pkg_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), "frida_tools"))
 
 agents = glob.glob(os.path.join(pkg_dir, "*_agent.*"))
 assert len(agents) > 0, "Agents not compiled; run “npm install” in agents/"
 
 setup(
     name="frida-tools",
-    version="9.2.4",
+    version="9.2.5",
     description="Frida CLI tools",
     long_description="CLI tools for [Frida](https://frida.re).",
     long_description_content_type="text/markdown",
     author="Frida Developers",
     author_email="oleavr@frida.re",
     url="https://frida.re",
     install_requires=[
```

