# Comparing `tmp/pygments_pasp-0.0.2.tar.gz` & `tmp/pygments_pasp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_pasp-0.0.2.tar", last modified: Thu Feb 23 00:19:08 2023, max compression
+gzip compressed data, was "pygments_pasp-0.0.3.tar", last modified: Wed May  3 19:58:49 2023, max compression
```

## Comparing `pygments_pasp-0.0.2.tar` & `pygments_pasp-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-02-23 00:19:08.798301 pygments_pasp-0.0.2/
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      826 2023-02-23 00:19:08.798301 pygments_pasp-0.0.2/PKG-INFO
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      241 2023-02-22 23:33:35.000000 pygments_pasp-0.0.2/README.md
-drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-02-23 00:19:08.798301 pygments_pasp-0.0.2/pygments_pasp/
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        0 2023-02-22 23:31:14.000000 pygments_pasp-0.0.2/pygments_pasp/__init__.py
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)     4801 2023-02-22 23:55:00.000000 pygments_pasp-0.0.2/pygments_pasp/pasp.py
-drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-02-23 00:19:08.798301 pygments_pasp-0.0.2/pygments_pasp.egg-info/
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      826 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/PKG-INFO
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      305 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/SOURCES.txt
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        1 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/dependency_links.txt
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       59 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/entry_points.txt
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        9 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/requires.txt
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       14 2023-02-23 00:19:08.000000 pygments_pasp-0.0.2/pygments_pasp.egg-info/top_level.txt
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      804 2023-02-23 00:18:16.000000 pygments_pasp-0.0.2/pyproject.toml
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       38 2023-02-23 00:19:08.798301 pygments_pasp-0.0.2/setup.cfg
--rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       70 2023-02-23 00:17:23.000000 pygments_pasp-0.0.2/setup.py
+drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-05-03 19:58:49.977682 pygments_pasp-0.0.3/
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      826 2023-05-03 19:58:49.977682 pygments_pasp-0.0.3/PKG-INFO
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      241 2023-02-22 23:33:35.000000 pygments_pasp-0.0.3/README.md
+drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-05-03 19:58:49.977682 pygments_pasp-0.0.3/pygments_pasp/
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        0 2023-02-22 23:31:14.000000 pygments_pasp-0.0.3/pygments_pasp/__init__.py
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)     4872 2023-04-28 00:56:17.000000 pygments_pasp-0.0.3/pygments_pasp/pasp.py
+drwxr-xr-x   0 renatogeh  (1000) renatogeh  (1000)        0 2023-05-03 19:58:49.977682 pygments_pasp-0.0.3/pygments_pasp.egg-info/
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      826 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/PKG-INFO
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      305 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/SOURCES.txt
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        1 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/dependency_links.txt
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       59 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/entry_points.txt
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)        9 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/requires.txt
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       14 2023-05-03 19:58:49.000000 pygments_pasp-0.0.3/pygments_pasp.egg-info/top_level.txt
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)      804 2023-05-03 19:58:28.000000 pygments_pasp-0.0.3/pyproject.toml
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       38 2023-05-03 19:58:49.977682 pygments_pasp-0.0.3/setup.cfg
+-rw-r--r--   0 renatogeh  (1000) renatogeh  (1000)       70 2023-02-23 00:17:23.000000 pygments_pasp-0.0.3/setup.py
```

### Comparing `pygments_pasp-0.0.2/PKG-INFO` & `pygments_pasp-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments_pasp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pygments package for pasp
 Author-email: Renato Lui Geh <renatogeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/RenatoGeh/pygments_pasp
 Project-URL: Issues, https://github.com/RenatoGeh/pygments_pasp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygments_pasp-0.0.2/pygments_pasp/pasp.py` & `pygments_pasp-0.0.3/pygments_pasp/pasp.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                      Text, # space
                      using(lexer),
                      Keyword, # end
                      Text, # space
                      Punctuation), # .)
             '#pop')
 
-def _torch_lexer(lexer):
+def _python_lexer(lexer):
     return (rf'(?s)(\s*)(.*)(#end)(\s*)(\.)',
             bygroups(Text, # space
                      using(lexer),
                      Keyword, # end
                      Text, # space
                      Punctuation), # .)
             '#pop')
@@ -67,37 +67,38 @@
             (r'@[a-zA-Z][a-zA-Z0-9_]*', Name.Function),
             (r'[\[\](){}]', Punctuation),
             (r'((?<!:):-|(?<!:):~|\.(?!\.)|,(?!;)|;(?!;)|:(?!:))', Punctuation),
             (r'\&[_]*[a-z][a-zA-Z_]*', Keyword),
             (r'[/<=>+\-*\\?&@|:;~k.!]+', Operator),
             (r'(#count|#sum|#min|#max|#show|#const|#edge|#minimize|#maximize|'
              r'#defined|#heuristic|#project|#program|'
-             r'#external|#theory|#end|not|#query|undef|as|in|at|with|\?|\!)\b', Keyword),
+             r'#external|#theory|#end|not|#query|#learn|#semantics|undef|as|in|on|at|with|\?|\!)\b', Keyword),
             (r'#script', Keyword, 'script'),
-            (r'#torch', Keyword, 'torch'),
+            (r'#python', Keyword, 'python'),
             (r'#include\b', Keyword, 'include'),
             (r'(#inf|#sup|#true|#false)\b', Keyword.Constant),
             (r"[_']*[A-Z][0-9a-zA-Z'_]*", Name.Variable),
             (r'_', Name.Variable),
             (r"[_']*[a-z][0-9a-zA-Z'_]*", Text),
             (r'\s', Text),
+            (r"(test|train)", Name.Builtin),
         ],
         'include': [
             (r'<(\\>|\\"|\\\\|[^\\>])*>', String.Double, "#pop"),
             (r'"(\\n|\\"|\\\\|[^\\"])*"', String.Double, "#pop"),
             (r'\s', Text),
             ('', Text, '#pop'), # fallback to normal parsing
         ],
         'script': [
             _script_lexer('python', PythonLexer),
             _script_lexer('lua', LuaLexer),
             ('', Text, '#pop'), # fallback to normal parsing
         ],
-        'torch': [
-            _torch_lexer(PythonLexer),
+        'python': [
+            _python_lexer(PythonLexer),
             ('', Text, '#pop'), # fallback to normal parsing
         ],
         'nested-comment': [
             (r'\*%', Comment.Multiline, '#pop'),
             (r'%\*', Comment.Multiline, '#push'),
             (r'[^*%]+', Comment.Multiline),
             (r'[*%]', Comment.Multiline),
```

### Comparing `pygments_pasp-0.0.2/pygments_pasp.egg-info/PKG-INFO` & `pygments_pasp-0.0.3/pygments_pasp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-pasp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pygments package for pasp
 Author-email: Renato Lui Geh <renatogeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/RenatoGeh/pygments_pasp
 Project-URL: Issues, https://github.com/RenatoGeh/pygments_pasp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygments_pasp-0.0.2/pyproject.toml` & `pygments_pasp-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.6.3", "pygments"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygments_pasp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name = "Renato Lui Geh", email = "renatogeh@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = ["pygments"]
```

