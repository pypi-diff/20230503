# Comparing `tmp/shelllikecui-0.0.1.tar.gz` & `tmp/shelllikecui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelllikecui-0.0.1.tar", last modified: Wed May  3 08:13:01 2023, max compression
+gzip compressed data, was "shelllikecui-0.0.2.tar", last modified: Wed May  3 10:23:45 2023, max compression
```

## Comparing `shelllikecui-0.0.1.tar` & `shelllikecui-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 08:13:01.067037 shelllikecui-0.0.1/
--rw-rw-rw-   0        0        0     1063 2023-05-03 07:50:51.000000 shelllikecui-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1963 2023-05-03 08:13:01.067037 shelllikecui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-05-03 08:10:12.000000 shelllikecui-0.0.1/README.md
--rw-rw-rw-   0        0        0      773 2023-05-03 08:04:48.000000 shelllikecui-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 08:13:01.067037 shelllikecui-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 08:13:01.047631 shelllikecui-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 08:13:01.053633 shelllikecui-0.0.1/src/shelllikecui/
--rw-rw-rw-   0        0        0       86 2023-05-03 07:21:45.000000 shelllikecui-0.0.1/src/shelllikecui/__init__.py
--rw-rw-rw-   0        0        0     1553 2023-05-03 08:07:23.000000 shelllikecui-0.0.1/src/shelllikecui/base.py
--rw-rw-rw-   0        0        0     2210 2023-05-03 07:31:39.000000 shelllikecui-0.0.1/src/shelllikecui/cui.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:13:01.065631 shelllikecui-0.0.1/src/shelllikecui.egg-info/
--rw-rw-rw-   0        0        0     1963 2023-05-03 08:13:01.000000 shelllikecui-0.0.1/src/shelllikecui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-03 08:13:01.000000 shelllikecui-0.0.1/src/shelllikecui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 08:13:01.000000 shelllikecui-0.0.1/src/shelllikecui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 08:13:01.000000 shelllikecui-0.0.1/src/shelllikecui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:23:45.128356 shelllikecui-0.0.2/
+-rw-rw-rw-   0        0        0     1063 2023-05-03 07:50:51.000000 shelllikecui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1963 2023-05-03 10:23:45.128356 shelllikecui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-05-03 08:10:12.000000 shelllikecui-0.0.2/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-03 10:23:07.000000 shelllikecui-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:23:45.128356 shelllikecui-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 10:23:45.111356 shelllikecui-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 10:23:45.117355 shelllikecui-0.0.2/src/shelllikecui/
+-rw-rw-rw-   0        0        0       86 2023-05-03 07:21:45.000000 shelllikecui-0.0.2/src/shelllikecui/__init__.py
+-rw-rw-rw-   0        0        0     1237 2023-05-03 10:00:03.000000 shelllikecui-0.0.2/src/shelllikecui/base.py
+-rw-rw-rw-   0        0        0     2763 2023-05-03 09:58:40.000000 shelllikecui-0.0.2/src/shelllikecui/cui.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:23:45.127356 shelllikecui-0.0.2/src/shelllikecui.egg-info/
+-rw-rw-rw-   0        0        0     1963 2023-05-03 10:23:45.000000 shelllikecui-0.0.2/src/shelllikecui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-03 10:23:45.000000 shelllikecui-0.0.2/src/shelllikecui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:23:45.000000 shelllikecui-0.0.2/src/shelllikecui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 10:23:45.000000 shelllikecui-0.0.2/src/shelllikecui.egg-info/top_level.txt
```

### Comparing `shelllikecui-0.0.1/LICENSE` & `shelllikecui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shelllikecui-0.0.1/PKG-INFO` & `shelllikecui-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelllikecui
-Version: 0.0.1
+Version: 0.0.2
 Summary: shell like CUI
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Elaina
```

### Comparing `shelllikecui-0.0.1/pyproject.toml` & `shelllikecui-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shelllikecui"
-version = "0.0.1"
+version = "0.0.2"
 description = "shell like CUI"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["cui"]
 
 authors = [
```

### Comparing `shelllikecui-0.0.1/src/shelllikecui/base.py` & `shelllikecui-0.0.2/src/shelllikecui/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,52 @@
-import sys
 import shlex
 import subprocess
-
-from .cui import Cui, make_command, _CNF
+from .cui import Cui, make_command
 
 
 def make_cui0() -> Cui:
     return Cui()
 
 
-def _command_not_found(arg: str) -> int:
-    f, arg = arg.split(' ', 1)
-    print('Command Not Found:', f)
-
-
 def _exec(arg: str):
     f, arg = arg.split(' ', 1)
     try:
         exec(arg)
     except Exception as e:
         print(repr(e))
+    return None
 
 
 def _eval(arg: str):
     f, arg = arg.split(' ', 1)
     try:
         print(eval(arg))
     except Exception as e:
         print(repr(e))
-
-def _exit(arg: str):
-    sys.exit(0)
+    return None
 
 
 def make_cui1() -> Cui:
-    a = Cui()
-
-    a.register(make_command(_CNF, _command_not_found, 'cnf',
-               'Command Not Found Exception default function'))
+    a = make_cui0()
+    a.register(make_command('exec', _exec, list(), 'exec by Python'))
+    a.register(make_command('eval', _eval, list(), 'eval by Python'))
 
     def _cui(arg: str):
         f, arg = arg.split(' ', 1)
         return a.exec(arg)
     a.register(make_command('cui', _cui, list(), 'exec by its Interpreter'))
 
-    a.register(make_command('exec', _exec, list(), 'exec by Python'))
-    a.register(make_command('eval', _eval, list(), 'eval by Python'))
-    a.register(make_command('exit', _exit, list(), 'exit by Python'))
-
     def _sh(arg: str):
         f, arg = arg.split(' ', 1)
         p = subprocess.Popen(
             shlex.split(arg),
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
         while p.poll() is None:
             a.slp()
         print(p.stdout.read().decode('utf8'))
+        return None
     a.register(make_command('sh', _sh, 'shell', 'exec by Shell'))
 
     return a
```

### Comparing `shelllikecui-0.0.1/src/shelllikecui/cui.py` & `shelllikecui-0.0.2/src/shelllikecui/cui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Union, Callable, Iterable
+import sys
 import time
+from typing import Union, Callable, Iterable
 
 _CNF = 'command_not_found'
 
 
 class CommandBase:
     def __init__(self, name: str, alias: Union[Iterable[str], str] = (), desc: str = '') -> None:
         self.name = name
@@ -26,24 +27,43 @@
 
 def make_command(name: str, func: Callable, alias: Union[Iterable[str], str] = (), desc: str = '') -> CommandBase:
     a = CommandBase(name, alias, desc)
     a.func = func
     return a
 
 
+def _command_not_found(arg: str) -> int:
+    f, arg = arg.split(' ', 1)
+    print('Command Not Found:', f)
+    return None
+
+
+def _exit(arg: str):
+    sys.exit(0)
+    return None
+
+def _none(arg: str):
+    return None
+
+
 class Cui:
     def __init__(self) -> None:
         # self.pth = './'
         # self.ps1 = 'user@Cui%s%s# '
         # self.ps1_full: bool = False
         self.ps1 = '> '
         self.clk = 0.1
         self.all_cmd = dict()
         self.alias = dict()
 
+        self.register(make_command(_CNF, _command_not_found, 'cnf',
+                                   'Command Not Found Exception default function'))
+        self.register(make_command('exit', _exit, list(), 'exit by Python'))
+        self.register(make_command('', _none, list(), 'nothing'))
+
     def slp(self, i: int = 1) -> None:
         time.sleep(self.clk * i)
 
     def register(self, a: CommandBase, rewrite: bool = False) -> dict:
         res = dict()
         if a.name in self.all_cmd:
             res[a.name] = a.name
@@ -57,17 +77,17 @@
                 if not rewrite:
                     continue
             self.alias[i] = a.name
         return res
 
     def _get_func(self, name: str) -> Callable:
         return self.all_cmd[self.alias.get(name, _CNF)]
-    
-    def exec(self, s:str):
-        s += ' '
+
+    def exec(self, s: str):
+        s = s.strip() + ' '
         name = s.split(' ', 1)[0]
         return self._get_func(name)(s)
 
     def cmd(self, s: str):
         code = self.exec(s)
         print(self.ps1, end='', flush=True)
         return code
```

### Comparing `shelllikecui-0.0.1/src/shelllikecui.egg-info/PKG-INFO` & `shelllikecui-0.0.2/src/shelllikecui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelllikecui
-Version: 0.0.1
+Version: 0.0.2
 Summary: shell like CUI
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Elaina
```

