# Comparing `tmp/ahk-1.0.0b0.tar.gz` & `tmp/ahk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.0.0b0.tar", last modified: Tue May  2 04:34:59 2023, max compression
+gzip compressed data, was "ahk-1.0.1.tar", last modified: Tue May  2 23:45:45 2023, max compression
```

## Comparing `ahk-1.0.0b0.tar` & `ahk-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 04:34:49.000000 ahk-1.0.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.929923 ahk-1.0.0b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169734 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   164017 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 04:34:49.000000 ahk-1.0.0b0/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-02 04:34:49.000000 ahk-1.0.0b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 04:34:49.000000 ahk-1.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 04:34:59.929923 ahk-1.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:34:49.000000 ahk-1.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 23:45:34.000000 ahk-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-02 23:45:45.257030 ahk-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.253030 ahk-1.0.1/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178319 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172602 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 23:45:34.000000 ahk-1.0.1/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 23:45:45.000000 ahk-1.0.1/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 23:45:34.000000 ahk-1.0.1/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:45:45.257030 ahk-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-05-02 23:45:34.000000 ahk-1.0.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 23:45:34.000000 ahk-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 23:45:45.257030 ahk-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:45:34.000000 ahk-1.0.1/setup.py
```

### Comparing `ahk-1.0.0b0/PKG-INFO` & `ahk-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -15,48 +15,49 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: binary
 
 # ahk
 
 A fully typed Python wrapper around AHK.
 
 [![Docs](https://readthedocs.org/projects/ahk/badge/?version=latest)](https://ahk.readthedocs.io/en/latest/?badge=latest)
-[![Build](https://ci.appveyor.com/api/projects/status/2c53x6gglw9nxgj1/branch/master?svg=true)](https://ci.appveyor.com/project/spyoungtech/ahk/branch/master)
+[![Build](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml/badge.svg)](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml)
 [![version](https://img.shields.io/pypi/v/ahk.svg?colorB=blue)](https://pypi.org/project/ahk/)
 [![pyversion](https://img.shields.io/pypi/pyversions/ahk.svg?)](https://pypi.org/project/ahk/)
 [![Coverage](https://coveralls.io/repos/github/spyoungtech/ahk/badge.svg?branch=master)](https://coveralls.io/github/spyoungtech/ahk?branch=master)
 [![Downloads](https://pepy.tech/badge/ahk)](https://pepy.tech/project/ahk)
 
 # Installation
 
 ```
 pip install ahk
 ```
 Requires Python 3.8+
 
-See also [Non-Python dependencies](#non-python-dependencies)
+See also [Non-Python dependencies](#deps)
 
 # Usage
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
 
 ahk.mouse_move(x=100, y=100, blocking=True)  # Blocks until mouse finishes moving (the default)
 ahk.mouse_move(x=150, y=150, speed=10, blocking=True) # Moves the mouse to x, y taking 'speed' seconds to move
 print(ahk.mouse_position)  #  (150, 150)
 ```
 
-![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/master/docs/_static/ahk.gif)
+![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/9d049a327c7a10c9f19dfef89fc63668695023fc/docs/_static/ahk.gif)
 
 # Examples
 
 Non-exhaustive examples of some functions available with this package. Full documentation coming soon!
 
 ## Hotkeys
 
@@ -460,19 +461,36 @@
 This library is fully type-hinted, allowing you to leverage tools like `mypy` to help validate the type-correctness
 of your code. IDEs that implement type-checking features are also able to leverage type hints to help ensure your
 code is safe.
 
 
 ## Run arbitrary AutoHotkey scripts
 
-TBD
+You can also run arbitrary AutoHotkey code either as a `.ahk` script file or as a string containing AHK code.
 
+```python
+from ahk import AHK
+ahk = AHK()
+my_script = '''\
+MouseMove, 100, 100
+; etc...
+'''
+
+ahk.run_script(my_script)
+```
+
+```python
+from ahk import AHK
+ahk = AHK()
+script_path = r'C:\Path\To\myscript.ahk'
+ahk.run_script(script_path)
+```
 
 
-<a name="deps" />
+<a name="deps"></a>
 
 # Non-Python dependencies
 
 To use this package, you need the [AutoHotkey executable](https://www.autohotkey.com/download/). It's expected to be on PATH by default.
 
 Note: this should be AutoHotkey V1. AutoHotkey V2 is not yet supported.
```

### Comparing `ahk-1.0.0b0/ahk/__init__.py` & `ahk-1.0.1/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_async/engine.py` & `ahk-1.0.1/ahk/_async/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,17 +189,15 @@
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
     async def set_title_match_mode(self, title_match_mode: TitleMatchMode, /) -> None:
         """
         Sets the default title match mode
 
-        Has no effect for `Window`/`Control` instance methods (these always use hwnd)
-
-        Does not affect methods called with `blocking=True` (because these run in a separate AHK process)
+        Does not affect methods called with ``blocking=True`` (because these run in a separate AHK process)
 
         Reference: https://www.autohotkey.com/docs/commands/SetTitleMatchMode.htm
 
         :param title_match_mode: the match mode (and/or match speed) to set as the default title match mode. Can be 1, 2, 3, 'Regex', 'Fast', 'Slow' or a tuple of these.
         :return: None
         """
 
@@ -221,36 +219,42 @@
         await self._transport.function_call('AHKSetTitleMatchMode', args)
         return None
 
     async def get_title_match_mode(self) -> str:
         """
         Get the title match mode.
 
-        I.E. the current value of `A_TitleMatchMode`
+        I.E. the current value of ``A_TitleMatchMode``
 
         """
         resp = await self._transport.function_call('AHKGetTitleMatchMode')
         return resp
 
     async def get_title_match_speed(self) -> str:
         """
         Get the title match mode speed.
 
-        I.E. the current value of `A_TitleMatchModeSpeed`
+        I.E. the current value of ``A_TitleMatchModeSpeed``
 
         """
         resp = await self._transport.function_call('AHKGetTitleMatchSpeed')
         return resp
 
     async def set_coord_mode(self, target: CoordModeTargets, relative_to: CoordModeRelativeTo = 'Screen') -> None:
+        """
+        Analog of `CoordMode <https://www.autohotkey.com/docs/commands/CoordMode.htm>`_
+        """
         args = [str(target), str(relative_to)]
         await self._transport.function_call('AHKSetCoordMode', args)
         return None
 
     async def get_coord_mode(self, target: CoordModeTargets) -> str:
+        """
+        Analog for ``A_CoordMode<target>``
+        """
         args = [str(target)]
         resp = await self._transport.function_call('AHKGetCoordMode', args)
         return resp
 
     # fmt: off
     @overload
     async def control_click(self, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', control: str = '', title: str = '', text: str = '', exclude_title: str = '', exclude_text: str = '', *, title_match_mode: Optional[TitleMatchMode] = None, detect_hidden_windows: Optional[bool] = None) -> None: ...
@@ -273,27 +277,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
         """
-
-        :param button: the mouse button to use
-        :param click_count: how many times to click
-        :param options: options -- same meaning as in AutoHotkey
-        :param control: the control to click
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlClick <https://www.autohotkey.com/docs/commands/ControlClick.htm>`_
         """
         args = [control, title, text, str(button), str(click_count), options, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -344,25 +336,15 @@
         exclude_title: str = '',
         exclude_text: str = '',
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, AsyncFutureResult[str]]:
         """
-        Analog to ``ControlGetText``
-
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlGetText <https://www.autohotkey.com/docs/commands/ControlGetText.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -412,25 +394,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Position, AsyncFutureResult[Position]]:
         """
-        Analog to ``ControlGetPos``
-
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog to `ControlGetPos <https://www.autohotkey.com/docs/commands/ControlGetPos.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -482,28 +454,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
         """
-        Analog for ``ControlSend``
-
-        Reference: https://www.autohotkey.com/docs/commands/ControlSend.htm
-
-        :param keys:
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlSend <https://www.autohotkey.com/docs/commands/ControlSend.htm>`_
         """
         args = [control, keys, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -541,25 +500,24 @@
         Start the Autohotkey process for triggering hotkeys
 
         """
         return self._transport.start_hotkeys()
 
     def stop_hotkeys(self) -> None:
         """
-        Stop the Autohotkey process for triggering hotkeys
+        Stop the Autohotkey process for triggering hotkeys/hotstrings
 
         """
         return self._transport.stop_hotkeys()
 
     async def set_detect_hidden_windows(self, value: bool) -> None:
         """
-        Analog for AutoHotkey's `DetectHiddenWindows`
-
-        :param value: The setting value. `True` to turn on hidden window detection, `False` to turn it off.
+        Analog for `DetectHiddenWindows <https://www.autohotkey.com/docs/commands/DetectHiddenWindows.htm>`_
 
+        :param value: The setting value. ``True`` to turn on hidden window detection, ``False`` to turn it off.
         """
 
         if value not in (True, False):
             raise TypeError(f'detect hidden windows must be a boolean, got object of type {type(value)}')
         args = []
         if value is True:
             args.append('On')
@@ -629,23 +587,15 @@
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[List[AsyncWindow], AsyncFutureResult[List[AsyncWindow]]]:
         """
         Enumerate all windows matching the criteria.
 
-
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `WinGet List subcommand <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#List>_`
         """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
@@ -664,46 +614,41 @@
     @overload
     async def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Tuple[int, int], AsyncFutureResult[Tuple[int, int]]]: ...
     # fmt: on
     async def get_mouse_position(
         self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True
     ) -> Union[Tuple[int, int], AsyncFutureResult[Tuple[int, int]]]:
         """
-        Analog for ``MouseGetPos``
-
-        :param coord_mode:
-        :param blocking:
-        :return:
+        Analog for `MouseGetPos <https://www.autohotkey.com/docs/commands/MouseGetPos.htm>`_
         """
         if coord_mode:
             args = [str(coord_mode)]
         else:
             args = []
         resp = await self._transport.function_call('AHKMouseGetPos', args, blocking=blocking)
         return resp
 
     @property
     def mouse_position(self) -> AsyncPropertyReturnTupleIntInt:
         """
-        Convenience property for ``get_mouse_position``
+        Convenience property for :py:meth:`get_mouse_position`
 
-        :return:
+        Setter accepts a tuple of x,y coordinates passed to :py:meth:`mouse_mouse`
         """
         warnings.warn(  # unasync: remove
             _PROPERTY_DEPRECATION_WARNING_MESSAGE.format('mouse_position'), category=DeprecationWarning, stacklevel=2
         )
         return self.get_mouse_position()
 
     @mouse_position.setter
     def mouse_position(self, new_position: Tuple[int, int]) -> None:
         """
         Convenience setter for ``mouse_move``
 
         :param new_position: a tuple of x,y coordinates to move to
-        :return:
         """
         raise RuntimeError('Use of the mouse_position setter is not supported in the async API.')  # unasync: remove
         x, y = new_position
         return self.mouse_move(x=x, y=y, speed=0, relative=False)
 
     # fmt: off
     @overload
@@ -721,22 +666,15 @@
         y: Optional[Union[str, int]] = None,
         *,
         speed: Optional[int] = None,
         relative: bool = False,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
         """
-        Analog for ``MouseMove``
-
-        :param x:
-        :param y:
-        :param speed:
-        :param relative:
-        :param blocking:
-        :return:
+        Analog for `MouseMove <https://www.autohotkey.com/docs/commands/MouseMove.htm>`_
         """
         if relative and (x is None or y is None):
             x = x or 0
             y = y or 0
         elif not relative and (x is None or y is None):
             posx, posy = await self.get_mouse_position()
             x = x or posx
@@ -748,15 +686,15 @@
         if relative:
             args.append('R')
         resp = await self._transport.function_call('AHKMouseMove', args, blocking=blocking)
         return resp
 
     async def a_run_script(self, *args: Any, **kwargs: Any) -> Union[str, AsyncFutureResult[str]]:
         """
-        Deprecated. Use ``run_script`` instead.
+        Deprecated. Use :py:meth:`run_script` instead.
         """
         warnings.warn('a_run_script is deprecated. Use run_script instead.', DeprecationWarning, stacklevel=2)
         return await self.run_script(*args, **kwargs)
 
     # fmt: off
     @overload
     async def get_active_window(self) -> Optional[AsyncWindow]: ...
@@ -768,28 +706,23 @@
     async def get_active_window(self, blocking: bool = True) -> Union[Optional[AsyncWindow], AsyncFutureResult[Optional[AsyncWindow]]]: ...
     # fmt: on
     async def get_active_window(
         self, blocking: bool = True
     ) -> Union[Optional[AsyncWindow], AsyncFutureResult[Optional[AsyncWindow]]]:
         """
         Gets the currently active window.
-
-        :param blocking:
-        :return:
         """
         return await self.win_get(
             title='A', detect_hidden_windows=False, title_match_mode=(1, 'Fast'), blocking=blocking
         )
 
     @property
     def active_window(self) -> AsyncPropertyReturnOptionalAsyncWindow:
         """
-        Gets the currently active window
-
-        :return:
+        Gets the currently active window. Convenience property for :py:meth:`get_active_window`
         """
         warnings.warn(  # unasync: remove
             _PROPERTY_DEPRECATION_WARNING_MESSAGE.format('active_window'), category=DeprecationWarning, stacklevel=2
         )
         return self.get_active_window()
 
     async def find_windows(
@@ -918,14 +851,17 @@
             windows = await self.find_windows_by_title(title=title, exact=exact, title_match_mode=title_match_mode)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return windows[0] if windows else None
 
     async def get_volume(self, device_number: int = 1) -> float:
+        """
+        Analog for `SoundGetWaveVolume <https://www.autohotkey.com/docs/commands/SoundGetWaveVolume.htm>`_
+        """
         args = [str(device_number)]
         response = await self._transport.function_call('AHKGetVolume', args)
         return response
 
     # fmt: off
     @overload
     async def key_down(self, key: Union[str, Key]) -> None: ...
@@ -933,14 +869,17 @@
     async def key_down(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     async def key_down(self, key: Union[str, Key], *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def key_down(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def key_down(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Shortcut for :py:meth:`send_input` but transforms specified key to perform a key "DOWN" only (no release)
+        """
         if isinstance(key, str):
             key = Key(key_name=key)
         if blocking:
             await self.send_input(key.DOWN, blocking=True)
             return None
         else:
             return await self.send_input(key.DOWN, blocking=False)
@@ -954,14 +893,18 @@
     async def key_press(self, key: Union[str, Key], *, blocking: Literal[False], release: bool = True) -> AsyncFutureResult[None]: ...
     @overload
     async def key_press(self, key: Union[str, Key], *, release: bool = True, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def key_press(
         self, key: Union[str, Key], *, release: bool = True, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Press (and release) a key. Sends `:py:meth:`key_down` then, if ``release`` is ``True`` (the default), sends
+        :py:meth:`key_up` subsequently.
+        """
         if blocking:
             await self.key_down(key, blocking=True)
             if release:
                 await self.key_up(key, blocking=True)
             return None
         else:
             d = await self.key_down(key, blocking=False)
@@ -976,14 +919,17 @@
     async def key_release(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     async def key_release(self, key: Union[str, Key], *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def key_release(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def key_release(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Alias for :py:meth:`key_up`
+        """
         if blocking:
             await self.key_up(key=key, blocking=True)
             return None
         else:
             return await self.key_up(key=key, blocking=False)
 
     # fmt: off
@@ -1004,14 +950,17 @@
         str,
         None,
         AsyncFutureResult[str],
         AsyncFutureResult[int],
         AsyncFutureResult[float],
         AsyncFutureResult[None],
     ]:
+        """
+        Analog for `GetKeyState <https://www.autohotkey.com/docs/commands/GetKeyState.htm#command>`_
+        """
         args: List[str] = [key_name]
         if mode is not None:
             if mode not in ('T', 'P'):
                 raise ValueError(f'Invalid value for mode parameter. Mode must be `T` or `P`. Got {mode!r}')
             args.append(mode)
         resp = await self._transport.function_call('AHKKeyState', args, blocking=blocking)
         return resp
@@ -1023,14 +972,18 @@
     async def key_up(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     async def key_up(self, key: Union[str, Key], *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def key_up(self, key: Union[str, Key], blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def key_up(self, key: Union[str, Key], blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Shortcut for :py:meth:`send_input` but transforms specified key to perform a key "UP" only. Useful if the key
+        was previously pressed down but not released.
+        """
         if isinstance(key, str):
             key = Key(key_name=key)
         if blocking:
             await self.send_input(key.UP, blocking=True)
             return None
         else:
             return await self.send_input(key.UP, blocking=False)
@@ -1050,42 +1003,56 @@
         key_name: str,
         *,
         timeout: Optional[int] = None,
         logical_state: bool = False,
         released: bool = False,
         blocking: bool = True,
     ) -> Union[int, AsyncFutureResult[int]]:
+        """
+        Analog for `KeyWait <https://www.autohotkey.com/docs/commands/KeyWait.htm>`_
+        """
         options = ''
         if not released:
             options += 'D'
         if logical_state:
             options += 'L'
         if timeout:
             options += f'T{timeout}'
         args = [key_name]
         if options:
             args.append(options)
 
-        resp = await self._transport.function_call('AHKKeyWait', args)
+        resp = await self._transport.function_call('AHKKeyWait', args, blocking=blocking)
         return resp
 
     async def run_script(
         self, script_text_or_path: str, /, *, blocking: bool = True, timeout: Optional[int] = None
     ) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Run an AutoHotkey script.
+        Can either be a path to a script (``.ahk``) file or a string containing script contents
+        """
         return await self._transport.run_script(script_text_or_path, blocking=blocking, timeout=timeout)
 
     async def set_send_level(self, level: int) -> None:
+        """
+        Analog for `SendLevel <https://www.autohotkey.com/docs/commands/SendLevel.htm>`_
+        """
         if not isinstance(level, int):
             raise TypeError('level must be an integer between 0 and 100')
         if not 0 <= level <= 100:
             raise ValueError('level value must be between 0 and 100')
         args = [str(level)]
         await self._transport.function_call('AHKSetSendLevel', args)
 
     async def get_send_level(self) -> int:
+        """
+        Get the current `SendLevel <https://www.autohotkey.com/docs/commands/SendLevel.htm>`_
+        (I.E. the value of ``A_SendLevel``)
+        """
         resp = await self._transport.function_call('AHKGetSendLevel')
         return resp
 
     # fmt: off
     @overload
     async def send(self, s: str, *, raw: bool = False, key_delay: Optional[int] = None, key_press_duration: Optional[int] = None) -> None: ...
     @overload
@@ -1100,14 +1067,17 @@
         s: str,
         *,
         raw: bool = False,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Send <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         if key_delay:
             args.append(str(key_delay))
         else:
             args.append('')
         if key_press_duration:
             args.append(str(key_press_duration))
@@ -1135,14 +1105,17 @@
         self,
         s: str,
         *,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SendRaw <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         resp = await self.send(
             s, raw=True, key_delay=key_delay, key_press_duration=key_press_duration, blocking=blocking
         )
         return resp
 
     # fmt: off
     @overload
@@ -1151,14 +1124,17 @@
     async def send_input(self, s: str, *, blocking: Literal[True]) -> None: ...
     @overload
     async def send_input(self, s: str, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def send_input(self, s: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def send_input(self, s: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SendInput <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         resp = await self._transport.function_call('AHKSendInput', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     async def type(self, s: str) -> None: ...
@@ -1166,14 +1142,17 @@
     async def type(self, s: str, *, blocking: Literal[True]) -> None: ...
     @overload
     async def type(self, s: str, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def type(self, s: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def type(self, s: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Like :py:meth:`send_input` but performs necessary escapes for you.
+        """
         resp = await self.send_input(type_escape(s), blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     async def send_play(self, s: str, *, key_delay: Optional[int] = None, key_press_duration: Optional[int] = None) -> None: ...
     @overload
@@ -1187,14 +1166,17 @@
         self,
         s: str,
         *,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SendPlay <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         if key_delay:
             args.append(str(key_delay))
         else:
             args.append('')
         if key_press_duration:
             args.append(str(key_press_duration))
@@ -1213,14 +1195,17 @@
     async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def set_capslock_state(
         self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
         args: List[str] = []
         if state is not None:
             if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
                 raise ValueError(
                     f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
                 )
             args.append(str(state))
@@ -1237,14 +1222,17 @@
     async def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[True]) -> None: ...
     @overload
     async def set_volume(self, value: int, device_number: int = 1, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def set_volume(
         self, value: int, device_number: int = 1, *, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SoundSetWaveVolume <https://www.autohotkey.com/docs/commands/SoundSetWaveVolume.htm>`_
+        """
         args = [str(device_number), str(value)]
         return await self._transport.function_call('AHKSetVolume', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def show_traytip(self, title: str, text: str, second: float = 1.0, type_id: int = 1, *, silent: bool = False, large_icon: bool = False) -> None: ...
     @overload
@@ -1261,14 +1249,17 @@
         second: float = 1.0,
         type_id: int = 1,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `TrayTip <https://www.autohotkey.com/docs/commands/TrayTip.htm>`_
+        """
         option = type_id + (16 if silent else 0) + (32 if large_icon else 0)
         args = [title, text, str(second), str(option)]
         return await self._transport.function_call('AHKTrayTip', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def show_error_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1285,14 +1276,17 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for error-style messages
+        """
         return await self.show_traytip(
             title=title, text=text, second=second, type_id=3, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     # fmt: off
     @overload
     async def show_info_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1309,14 +1303,17 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for info-style messages
+        """
         return await self.show_traytip(
             title=title, text=text, second=second, type_id=1, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     # fmt: off
     @overload
     async def show_warning_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1333,25 +1330,31 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for warning-style messages
+        """
         return await self.show_traytip(
             title=title, text=text, second=second, type_id=2, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     async def show_tooltip(
         self,
         text: str = '',
         x: Optional[int] = None,
         y: Optional[int] = None,
         which: int = 1,
     ) -> None:
+        """
+        Analog for `ToolTip <https://www.autohotkey.com/docs/commands/ToolTip.htm>`_
+        """
         if which not in range(1, 21):
             raise ValueError('which must be an integer between 1 and 20')
         args = [text]
         if x is not None:
             args.append(str(x))
         else:
             args.append('')
@@ -1373,14 +1376,17 @@
     async def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[True]) -> None: ...
     @overload
     async def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: bool = True) -> Optional[AsyncFutureResult[None]]: ...
     # fmt: on
     async def sound_beep(
         self, frequency: int = 523, duration: int = 150, *, blocking: bool = True
     ) -> Optional[AsyncFutureResult[None]]:
+        """
+        Analog for `SoundBeep <https://www.autohotkey.com/docs/commands/SoundBeep.htm>`_
+        """
         args = [str(frequency), str(duration)]
         await self._transport.function_call('AHKSoundBeep', args, blocking=blocking)
         return None
 
     # fmt: off
     @overload
     async def sound_get(self, device_number: int = 1, component_type: str = 'MASTER', control_type: str = 'VOLUME') -> str: ...
@@ -1395,39 +1401,48 @@
         self,
         device_number: int = 1,
         component_type: str = 'MASTER',
         control_type: str = 'VOLUME',
         *,
         blocking: bool = True,
     ) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Analog for `SoundGet <https://www.autohotkey.com/docs/commands/SoundGet.htm>`_
+        """
         args = [str(device_number), component_type, control_type]
         return await self._transport.function_call('AHKSoundGet', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def sound_play(self, filename: str) -> None: ...
     @overload
     async def sound_play(self, filename: str, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def sound_play(self, filename: str, *, blocking: Literal[True]) -> None: ...
     @overload
     async def sound_play(self, filename: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def sound_play(self, filename: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SoundPlay <https://www.autohotkey.com/docs/commands/SoundPlay.htm>`_
+        """
         return await self._transport.function_call('AHKSoundPlay', [filename], blocking=blocking)
 
     async def sound_set(
         self,
         value: Union[str, int, float],
         device_number: int = 1,
         component_type: str = 'MASTER',
         control_type: str = 'VOLUME',
         *,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SoundSet <https://www.autohotkey.com/docs/commands/SoundSet.htm>`_
+        """
         args = [str(device_number), component_type, control_type, str(value)]
         return await self._transport.function_call('AHKSoundSet', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def win_get(self, title: str = '', text: str = '', exclude_title: str = '', exclude_text: str = '', *, title_match_mode: Optional[TitleMatchMode] = None, detect_hidden_windows: Optional[bool] = None) -> Union[AsyncWindow, None]: ...
     @overload
@@ -1444,14 +1459,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[AsyncWindow, None, AsyncFutureResult[Union[None, AsyncWindow]]]:
+        """
+        Analog for `WinGet <https://www.autohotkey.com/docs/commands/WinGet.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1540,14 +1558,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Analog for `WinGetClass <https://www.autohotkey.com/docs/commands/WinGetClass.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1572,14 +1593,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Position, None, AsyncFutureResult[Union[Position, None]]]:
+        """
+        Analog for `WinGetPos <https://www.autohotkey.com/docs/commands/WinGetPos.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1604,14 +1628,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[AsyncWindow, None, AsyncFutureResult[Union[AsyncWindow, None]]]:
+        """
+        Like the IDLast subcommand for WinGet
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1636,14 +1663,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[int, None, AsyncFutureResult[Union[int, None]]]:
+        """
+        Get a window by process ID.
+
+        Like the pid subcommand for WinGet
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1668,14 +1700,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, str, AsyncFutureResult[Optional[str]]]:
+        """
+        Get the process name of a window
+
+        Analog for `ProcessName subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ProcessName>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1700,14 +1737,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, None, Union[None, str, AsyncFutureResult[Optional[str]]]]:
+        """
+        Get the process path for a window.
+
+        Analog for the `ProcessPath subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ProcessPath>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1732,14 +1774,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[int, AsyncFutureResult[int]]:
+        """
+        Analog for the `Count subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#Count>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1764,14 +1809,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, int, AsyncFutureResult[Optional[int]]]:
+        """
+        Analog for the `MinMax subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#MinMax>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1796,14 +1844,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[List[AsyncControl], None, AsyncFutureResult[Optional[List[AsyncControl]]]]:
+        """
+        Analog for the `ControlList subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ControlList>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1876,14 +1927,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinActivate <https://www.autohotkey.com/docs/commands/WinActivate.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1909,14 +1963,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinSetTitle <https://www.autohotkey.com/docs/commands/WinSetTitle.htm>`_
+        """
         args = [new_title, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -1964,14 +2021,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `AlwaysOnTop subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#AlwaysOnTop>`_
+        """
         args = [str(toggle), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2018,14 +2078,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Bottom subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Bottom>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2050,14 +2113,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Top subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Top>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2082,14 +2148,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Disable subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Disable>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2114,14 +2183,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Enable subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Enable>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2146,14 +2218,18 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Redraw subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Redraw>`_
+        """
+
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2179,14 +2255,18 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, AsyncFutureResult[bool]]:
+        """
+        Analog for `Style subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Style>`_
+        """
+
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2234,14 +2314,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, AsyncFutureResult[bool]]:
+        """
+        Analog for `ExStyle subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#ExStyle>`_
+        """
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2289,14 +2372,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, AsyncFutureResult[bool]]:
+        """
+        Analog for `Region subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Region>`_
+        """
         args = [options, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2344,14 +2430,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Transparent subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Transparent>`_
+        """
         args = [str(transparency), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2399,14 +2488,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `TransColor subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#TransColor>`_
+        """
         args = [str(color), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2490,14 +2582,17 @@
         click_count: Optional[int] = None,
         direction: Optional[Literal['U', 'D', 'Up', 'Down']] = None,
         *,
         relative: Optional[bool] = None,
         blocking: bool = True,
         coord_mode: Optional[CoordModeRelativeTo] = None,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `Click <https://www.autohotkey.com/docs/commands/Click.htm>`_
+        """
         if x or y:
             if y is None and isinstance(x, tuple) and len(x) == 2:
                 #  allow position to be specified by a two-sequence tuple
                 x, y = x
             assert x is not None and y is not None, 'If provided, position must be specified by x AND y'
         if button is None:
             button = 'L'
@@ -2534,15 +2629,15 @@
         scale_height: Optional[int] = None,
         scale_width: Optional[int] = None,
         transparent: Optional[str] = None,
         icon: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[Tuple[int, int], None, AsyncFutureResult[Optional[Tuple[int, int]]]]:
         """
-        https://www.autohotkey.com/docs/commands/ImageSearch.htm
+        Analog for `ImageSearch <https://www.autohotkey.com/docs/commands/ImageSearch.htm>`_
         """
 
         if scale_height and not scale_width:
             scale_width = -1
         elif scale_width and not scale_height:
             scale_height = -1
 
@@ -2580,14 +2675,17 @@
         from_position: Optional[Tuple[int, int]] = None,
         speed: Optional[int] = None,
         button: MouseButton = 1,
         relative: Optional[bool] = None,
         blocking: bool = True,
         coord_mode: Optional[CoordModeRelativeTo] = None,
     ) -> None:
+        """
+        Analog for `MouseClickDrag <https://www.autohotkey.com/docs/commands/MouseClickDrag.htm>`_
+        """
         if from_position:
             x1, y1 = from_position
             args = [str(button), str(x1), str(y1), str(x), str(y)]
         else:
             args = [str(button), '', '', str(x), str(y)]
 
         if speed:
@@ -2622,14 +2720,17 @@
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         alt: bool = False,
         slow: bool = False,
         rgb: bool = True,
         blocking: bool = True,
     ) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Analog for `PixelGetColor <https://www.autohotkey.com/docs/commands/PixelGetColor.htm>`_
+        """
         args = [str(x), str(y), coord_mode or '']
 
         options = ' '.join(word for word, val in zip(('Alt', 'Slow', 'RGB'), (alt, slow, rgb)) if val)
         args.append(options)
 
         resp = await self._transport.function_call('AHKPixelGetColor', args, blocking=blocking)
         return resp
@@ -2652,14 +2753,17 @@
         variation: int = 0,
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         fast: bool = True,
         rgb: bool = True,
         blocking: bool = True,
     ) -> Union[Optional[Tuple[int, int]], AsyncFutureResult[Optional[Tuple[int, int]]]]:
+        """
+        Analog for `PixelSearch <https://www.autohotkey.com/docs/commands/PixelSearch.htm>`_
+        """
         x1, y1 = search_region_start
         x2, y2 = search_region_end
         args = [str(x1), str(y1), str(x2), str(y2), str(color), str(variation)]
         mode = ' '.join(word for word, val in zip(('Fast', 'RGB'), (fast, rgb)) if val)
         args.append(mode)
         args.append(coord_mode or '')
         resp = await self._transport.function_call('AHKPixelSearch', args, blocking=blocking)
@@ -2683,14 +2787,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         blocking: bool = True,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinClose <https://www.autohotkey.com/docs/commands/WinClose.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2718,14 +2825,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinKill <https://www.autohotkey.com/docs/commands/WinKill.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2752,14 +2862,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinMinimize <https://www.autohotkey.com/docs/commands/WinMinimize.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2784,14 +2897,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinMaximize <https://www.autohotkey.com/docs/commands/WinMaximize.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2816,14 +2932,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinRestore <https://www.autohotkey.com/docs/commands/WinRestore.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2849,14 +2968,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[AsyncWindow, AsyncFutureResult[AsyncWindow]]:
+        """
+        Analog for `WinWait <https://www.autohotkey.com/docs/commands/WinWait.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2883,14 +3005,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[AsyncWindow, AsyncFutureResult[AsyncWindow]]:
+        """
+        Analog for `WinWaitActive <https://www.autohotkey.com/docs/commands/WinWaitActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2917,14 +3042,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[AsyncWindow, AsyncFutureResult[AsyncWindow]]:
+        """
+        Analog for `WinWaitNotActive <https://www.autohotkey.com/docs/commands/WinWaitActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2951,14 +3079,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinWaitClose <https://www.autohotkey.com/docs/commands/WinWaitClose.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2984,14 +3115,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinShow <https://www.autohotkey.com/docs/commands/WinShow.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3016,14 +3150,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinHide <https://www.autohotkey.com/docs/commands/WinHide.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3048,14 +3185,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, AsyncFutureResult[bool]]:
+        """
+        Check if a window is active.
+
+        Uses `WinActive <https://www.autohotkey.com/docs/v1/lib/WinActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3084,14 +3226,17 @@
         text: str = '',
         exclude_title: str = '',
         exclude_text: str = '',
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `WinMove <https://www.autohotkey.com/docs/commands/WinMove.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3110,21 +3255,30 @@
     async def get_clipboard(self, *, blocking: Literal[False]) -> AsyncFutureResult[str]: ...
     @overload
     async def get_clipboard(self, *, blocking: Literal[True]) -> str: ...
     @overload
     async def get_clipboard(self, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]: ...
     # fmt: on
     async def get_clipboard(self, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Get the string contents of the clipboard
+        """
         return await self._transport.function_call('AHKGetClipboard', blocking=blocking)
 
     async def set_clipboard(self, s: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Set the contents of the clipboard
+        """
         args = [s]
         return await self._transport.function_call('AHKSetClipboard', args, blocking=blocking)
 
     async def get_clipboard_all(self, *, blocking: bool = True) -> Union[bytes, AsyncFutureResult[bytes]]:
+        """
+        Get the full binary contents of the keyboard. The return value is intended to be used with :py:meth:`set_clipboard_all`
+        """
         return await self._transport.function_call('AHKGetClipboardAll', blocking=blocking)
 
     # fmt: off
     @overload
     async def set_clipboard_all(self, contents: bytes) -> None: ...
     @overload
     async def set_clipboard_all(self, contents: bytes, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
@@ -3132,14 +3286,17 @@
     async def set_clipboard_all(self, contents: bytes, *, blocking: Literal[True]) -> None: ...
     @overload
     async def set_clipboard_all(self, contents: bytes, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def set_clipboard_all(
         self, contents: bytes, *, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Set the full binary contents of the clipboard. Expects bytes object as returned by :py:meth:`get_clipboard_all`
+        """
         # TODO: figure out how to do this without a tempfile
         if not isinstance(contents, bytes):
             raise ValueError('Malformed data. Can only set bytes as returned by get_clipboard_all')
         if not contents:
             raise ValueError('bytes must be nonempty. If you want to clear the clipboard, use `set_clipboard`')
         with tempfile.NamedTemporaryFile(prefix='ahk-python', suffix='.clip', mode='wb', delete=False) as f:
             f.write(contents)
@@ -3153,14 +3310,18 @@
                 os.remove(f.name)
             except Exception:
                 pass
 
     def on_clipboard_change(
         self, callback: Callable[[int], Any], ex_handler: Optional[Callable[[int, Exception], Any]] = None
     ) -> None:
+        """
+        call a function in response to clipboard change.
+        Uses `OnClipboardChange() <https://www.autohotkey.com/docs/commands/OnClipboardChange.htm#function>`_
+        """
         self._transport.on_clipboard_change(callback, ex_handler)
 
     # fmt: off
     @overload
     async def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False) -> None: ...
     @overload
     async def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
@@ -3168,24 +3329,32 @@
     async def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: Literal[True]) -> None: ...
     @overload
     async def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def clip_wait(
         self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Wait until the clipboard contents change
+
+        Analog for `ClipWait <https://www.autohotkey.com/docs/v1/lib/ClipWait.htm>`_
+        """
         args = [str(timeout) if timeout else '']
         if wait_for_any_data:
             args.append('1')
         return await self._transport.function_call('AHKClipWait', args, blocking=blocking)
 
     async def block_input(
         self,
         value: Literal['On', 'Off', 'Default', 'Send', 'Mouse', 'MouseMove', 'MouseMoveOff', 'SendAndMouse'],
         /,  # flake8: noqa
     ) -> None:
+        """
+        Analog for `BlockInput <https://www.autohotkey.com/docs/commands/BlockInput.htm>`_
+        """
         await self._transport.function_call('AHKBlockInput', args=[value])
 
     # fmt: off
     @overload
     async def reg_delete(self, key_name: str, value_name: Optional[str] = None) -> None: ...
     @overload
     async def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[False]) -> Union[None, AsyncFutureResult[None]]: ...
@@ -3193,14 +3362,17 @@
     async def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[True]) -> None: ...
     @overload
     async def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def reg_delete(
         self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `RegDelete <https://www.autohotkey.com/docs/commands/RegDelete.htm>`_
+        """
         args = [key_name, value_name if value_name is not None else '']
         return await self._transport.function_call('AHKRegDelete', args, blocking=blocking)
 
     # fmt: off
     @overload
     async def reg_write(self, value_type: Literal['REG_SZ', 'REG_EXPAND_SZ', 'REG_MULTI_SZ', 'REG_DWORD', 'REG_BINARY'], key_name: str, value_name: Optional[str] = None, value: Optional[str] = None) -> None: ...
     @overload
@@ -3215,14 +3387,17 @@
         value_type: Literal['REG_SZ', 'REG_EXPAND_SZ', 'REG_MULTI_SZ', 'REG_DWORD', 'REG_BINARY'],
         key_name: str,
         value_name: Optional[str] = None,
         value: Optional[str] = None,
         *,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `RegWrite <https://www.autohotkey.com/docs/commands/RegWrite.htm>`_
+        """
         args = [value_type, key_name]
         if value_name is not None:
             args.append(value_name)
         else:
             args.append('')
         if value is not None:
             args.append(value)
@@ -3237,15 +3412,21 @@
     async def reg_read(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[True]) -> str: ...
     @overload
     async def reg_read(self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]: ...
     # fmt: on
     async def reg_read(
         self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True
     ) -> Union[str, AsyncFutureResult[str]]:
+        """
+        Analog for `RegRead <https://www.autohotkey.com/docs/commands/RegRead.htm>`_
+        """
         args = [key_name]
         if value_name is not None:
             args.append(value_name)
         return await self._transport.function_call('AHKRegRead', args, blocking=blocking)
 
     async def block_forever(self) -> NoReturn:
+        """
+        Blocks (sleeps) forever. Utility method to prevent script from exiting.
+        """
         while True:
             await async_sleep(1)
```

### Comparing `ahk-1.0.0b0/ahk/_async/transport.py` & `ahk-1.0.1/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_async/window.py` & `ahk-1.0.1/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_constants.py` & `ahk-1.0.1/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_hotkey.py` & `ahk-1.0.1/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_sync/engine.py` & `ahk-1.0.1/ahk/_sync/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,17 +185,15 @@
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return None
 
     def set_title_match_mode(self, title_match_mode: TitleMatchMode, /) -> None:
         """
         Sets the default title match mode
 
-        Has no effect for `Window`/`Control` instance methods (these always use hwnd)
-
-        Does not affect methods called with `blocking=True` (because these run in a separate AHK process)
+        Does not affect methods called with ``blocking=True`` (because these run in a separate AHK process)
 
         Reference: https://www.autohotkey.com/docs/commands/SetTitleMatchMode.htm
 
         :param title_match_mode: the match mode (and/or match speed) to set as the default title match mode. Can be 1, 2, 3, 'Regex', 'Fast', 'Slow' or a tuple of these.
         :return: None
         """
 
@@ -217,36 +215,42 @@
         self._transport.function_call('AHKSetTitleMatchMode', args)
         return None
 
     def get_title_match_mode(self) -> str:
         """
         Get the title match mode.
 
-        I.E. the current value of `A_TitleMatchMode`
+        I.E. the current value of ``A_TitleMatchMode``
 
         """
         resp = self._transport.function_call('AHKGetTitleMatchMode')
         return resp
 
     def get_title_match_speed(self) -> str:
         """
         Get the title match mode speed.
 
-        I.E. the current value of `A_TitleMatchModeSpeed`
+        I.E. the current value of ``A_TitleMatchModeSpeed``
 
         """
         resp = self._transport.function_call('AHKGetTitleMatchSpeed')
         return resp
 
     def set_coord_mode(self, target: CoordModeTargets, relative_to: CoordModeRelativeTo = 'Screen') -> None:
+        """
+        Analog of `CoordMode <https://www.autohotkey.com/docs/commands/CoordMode.htm>`_
+        """
         args = [str(target), str(relative_to)]
         self._transport.function_call('AHKSetCoordMode', args)
         return None
 
     def get_coord_mode(self, target: CoordModeTargets) -> str:
+        """
+        Analog for ``A_CoordMode<target>``
+        """
         args = [str(target)]
         resp = self._transport.function_call('AHKGetCoordMode', args)
         return resp
 
     # fmt: off
     @overload
     def control_click(self, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', control: str = '', title: str = '', text: str = '', exclude_title: str = '', exclude_text: str = '', *, title_match_mode: Optional[TitleMatchMode] = None, detect_hidden_windows: Optional[bool] = None) -> None: ...
@@ -269,27 +273,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
         """
-
-        :param button: the mouse button to use
-        :param click_count: how many times to click
-        :param options: options -- same meaning as in AutoHotkey
-        :param control: the control to click
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlClick <https://www.autohotkey.com/docs/commands/ControlClick.htm>`_
         """
         args = [control, title, text, str(button), str(click_count), options, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -340,25 +332,15 @@
         exclude_title: str = '',
         exclude_text: str = '',
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, FutureResult[str]]:
         """
-        Analog to ``ControlGetText``
-
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlGetText <https://www.autohotkey.com/docs/commands/ControlGetText.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -408,25 +390,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Position, FutureResult[Position]]:
         """
-        Analog to ``ControlGetPos``
-
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog to `ControlGetPos <https://www.autohotkey.com/docs/commands/ControlGetPos.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -478,28 +450,15 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
         """
-        Analog for ``ControlSend``
-
-        Reference: https://www.autohotkey.com/docs/commands/ControlSend.htm
-
-        :param keys:
-        :param control:
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `ControlSend <https://www.autohotkey.com/docs/commands/ControlSend.htm>`_
         """
         args = [control, keys, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
@@ -537,25 +496,24 @@
         Start the Autohotkey process for triggering hotkeys
 
         """
         return self._transport.start_hotkeys()
 
     def stop_hotkeys(self) -> None:
         """
-        Stop the Autohotkey process for triggering hotkeys
+        Stop the Autohotkey process for triggering hotkeys/hotstrings
 
         """
         return self._transport.stop_hotkeys()
 
     def set_detect_hidden_windows(self, value: bool) -> None:
         """
-        Analog for AutoHotkey's `DetectHiddenWindows`
-
-        :param value: The setting value. `True` to turn on hidden window detection, `False` to turn it off.
+        Analog for `DetectHiddenWindows <https://www.autohotkey.com/docs/commands/DetectHiddenWindows.htm>`_
 
+        :param value: The setting value. ``True`` to turn on hidden window detection, ``False`` to turn it off.
         """
 
         if value not in (True, False):
             raise TypeError(f'detect hidden windows must be a boolean, got object of type {type(value)}')
         args = []
         if value is True:
             args.append('On')
@@ -625,23 +583,15 @@
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[List[Window], FutureResult[List[Window]]]:
         """
         Enumerate all windows matching the criteria.
 
-
-        :param title:
-        :param text:
-        :param exclude_title:
-        :param exclude_text:
-        :param title_match_mode:
-        :param detect_hidden_windows:
-        :param blocking:
-        :return:
+        Analog for `WinGet List subcommand <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#List>_`
         """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
@@ -660,43 +610,38 @@
     @overload
     def get_mouse_position(self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True) -> Union[Tuple[int, int], FutureResult[Tuple[int, int]]]: ...
     # fmt: on
     def get_mouse_position(
         self, coord_mode: Optional[CoordModeRelativeTo] = None, *, blocking: bool = True
     ) -> Union[Tuple[int, int], FutureResult[Tuple[int, int]]]:
         """
-        Analog for ``MouseGetPos``
-
-        :param coord_mode:
-        :param blocking:
-        :return:
+        Analog for `MouseGetPos <https://www.autohotkey.com/docs/commands/MouseGetPos.htm>`_
         """
         if coord_mode:
             args = [str(coord_mode)]
         else:
             args = []
         resp = self._transport.function_call('AHKMouseGetPos', args, blocking=blocking)
         return resp
 
     @property
     def mouse_position(self) -> SyncPropertyReturnTupleIntInt:
         """
-        Convenience property for ``get_mouse_position``
+        Convenience property for :py:meth:`get_mouse_position`
 
-        :return:
+        Setter accepts a tuple of x,y coordinates passed to :py:meth:`mouse_mouse`
         """
         return self.get_mouse_position()
 
     @mouse_position.setter
     def mouse_position(self, new_position: Tuple[int, int]) -> None:
         """
         Convenience setter for ``mouse_move``
 
         :param new_position: a tuple of x,y coordinates to move to
-        :return:
         """
         x, y = new_position
         return self.mouse_move(x=x, y=y, speed=0, relative=False)
 
     # fmt: off
     @overload
     def mouse_move(self, x: Optional[Union[str, int]] = None, y: Optional[Union[str, int]] = None, *, speed: Optional[int] = None, relative: bool = False) -> None: ...
@@ -713,22 +658,15 @@
         y: Optional[Union[str, int]] = None,
         *,
         speed: Optional[int] = None,
         relative: bool = False,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
         """
-        Analog for ``MouseMove``
-
-        :param x:
-        :param y:
-        :param speed:
-        :param relative:
-        :param blocking:
-        :return:
+        Analog for `MouseMove <https://www.autohotkey.com/docs/commands/MouseMove.htm>`_
         """
         if relative and (x is None or y is None):
             x = x or 0
             y = y or 0
         elif not relative and (x is None or y is None):
             posx, posy = self.get_mouse_position()
             x = x or posx
@@ -740,15 +678,15 @@
         if relative:
             args.append('R')
         resp = self._transport.function_call('AHKMouseMove', args, blocking=blocking)
         return resp
 
     def a_run_script(self, *args: Any, **kwargs: Any) -> Union[str, FutureResult[str]]:
         """
-        Deprecated. Use ``run_script`` instead.
+        Deprecated. Use :py:meth:`run_script` instead.
         """
         warnings.warn('a_run_script is deprecated. Use run_script instead.', DeprecationWarning, stacklevel=2)
         return self.run_script(*args, **kwargs)
 
     # fmt: off
     @overload
     def get_active_window(self) -> Optional[Window]: ...
@@ -760,28 +698,23 @@
     def get_active_window(self, blocking: bool = True) -> Union[Optional[Window], FutureResult[Optional[Window]]]: ...
     # fmt: on
     def get_active_window(
         self, blocking: bool = True
     ) -> Union[Optional[Window], FutureResult[Optional[Window]]]:
         """
         Gets the currently active window.
-
-        :param blocking:
-        :return:
         """
         return self.win_get(
             title='A', detect_hidden_windows=False, title_match_mode=(1, 'Fast'), blocking=blocking
         )
 
     @property
     def active_window(self) -> SyncPropertyReturnOptionalAsyncWindow:
         """
-        Gets the currently active window
-
-        :return:
+        Gets the currently active window. Convenience property for :py:meth:`get_active_window`
         """
         return self.get_active_window()
 
     def find_windows(
         self,
         func: Optional[SyncFilterFunc] = None,
         *,
@@ -907,14 +840,17 @@
             windows = self.find_windows_by_title(title=title, exact=exact, title_match_mode=title_match_mode)
         if caught_warnings:
             for warning in caught_warnings:
                 warnings.warn(warning.message, warning.category, stacklevel=2)
         return windows[0] if windows else None
 
     def get_volume(self, device_number: int = 1) -> float:
+        """
+        Analog for `SoundGetWaveVolume <https://www.autohotkey.com/docs/commands/SoundGetWaveVolume.htm>`_
+        """
         args = [str(device_number)]
         response = self._transport.function_call('AHKGetVolume', args)
         return response
 
     # fmt: off
     @overload
     def key_down(self, key: Union[str, Key]) -> None: ...
@@ -922,14 +858,17 @@
     def key_down(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     def key_down(self, key: Union[str, Key], *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def key_down(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def key_down(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Shortcut for :py:meth:`send_input` but transforms specified key to perform a key "DOWN" only (no release)
+        """
         if isinstance(key, str):
             key = Key(key_name=key)
         if blocking:
             self.send_input(key.DOWN, blocking=True)
             return None
         else:
             return self.send_input(key.DOWN, blocking=False)
@@ -943,14 +882,18 @@
     def key_press(self, key: Union[str, Key], *, blocking: Literal[False], release: bool = True) -> FutureResult[None]: ...
     @overload
     def key_press(self, key: Union[str, Key], *, release: bool = True, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def key_press(
         self, key: Union[str, Key], *, release: bool = True, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Press (and release) a key. Sends `:py:meth:`key_down` then, if ``release`` is ``True`` (the default), sends
+        :py:meth:`key_up` subsequently.
+        """
         if blocking:
             self.key_down(key, blocking=True)
             if release:
                 self.key_up(key, blocking=True)
             return None
         else:
             d = self.key_down(key, blocking=False)
@@ -965,14 +908,17 @@
     def key_release(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     def key_release(self, key: Union[str, Key], *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def key_release(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def key_release(self, key: Union[str, Key], *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Alias for :py:meth:`key_up`
+        """
         if blocking:
             self.key_up(key=key, blocking=True)
             return None
         else:
             return self.key_up(key=key, blocking=False)
 
     # fmt: off
@@ -993,14 +939,17 @@
         str,
         None,
         FutureResult[str],
         FutureResult[int],
         FutureResult[float],
         FutureResult[None],
     ]:
+        """
+        Analog for `GetKeyState <https://www.autohotkey.com/docs/commands/GetKeyState.htm#command>`_
+        """
         args: List[str] = [key_name]
         if mode is not None:
             if mode not in ('T', 'P'):
                 raise ValueError(f'Invalid value for mode parameter. Mode must be `T` or `P`. Got {mode!r}')
             args.append(mode)
         resp = self._transport.function_call('AHKKeyState', args, blocking=blocking)
         return resp
@@ -1012,14 +961,18 @@
     def key_up(self, key: Union[str, Key], *, blocking: Literal[True]) -> None: ...
     @overload
     def key_up(self, key: Union[str, Key], *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def key_up(self, key: Union[str, Key], blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def key_up(self, key: Union[str, Key], blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Shortcut for :py:meth:`send_input` but transforms specified key to perform a key "UP" only. Useful if the key
+        was previously pressed down but not released.
+        """
         if isinstance(key, str):
             key = Key(key_name=key)
         if blocking:
             self.send_input(key.UP, blocking=True)
             return None
         else:
             return self.send_input(key.UP, blocking=False)
@@ -1039,42 +992,56 @@
         key_name: str,
         *,
         timeout: Optional[int] = None,
         logical_state: bool = False,
         released: bool = False,
         blocking: bool = True,
     ) -> Union[int, FutureResult[int]]:
+        """
+        Analog for `KeyWait <https://www.autohotkey.com/docs/commands/KeyWait.htm>`_
+        """
         options = ''
         if not released:
             options += 'D'
         if logical_state:
             options += 'L'
         if timeout:
             options += f'T{timeout}'
         args = [key_name]
         if options:
             args.append(options)
 
-        resp = self._transport.function_call('AHKKeyWait', args)
+        resp = self._transport.function_call('AHKKeyWait', args, blocking=blocking)
         return resp
 
     def run_script(
         self, script_text_or_path: str, /, *, blocking: bool = True, timeout: Optional[int] = None
     ) -> Union[str, FutureResult[str]]:
+        """
+        Run an AutoHotkey script.
+        Can either be a path to a script (``.ahk``) file or a string containing script contents
+        """
         return self._transport.run_script(script_text_or_path, blocking=blocking, timeout=timeout)
 
     def set_send_level(self, level: int) -> None:
+        """
+        Analog for `SendLevel <https://www.autohotkey.com/docs/commands/SendLevel.htm>`_
+        """
         if not isinstance(level, int):
             raise TypeError('level must be an integer between 0 and 100')
         if not 0 <= level <= 100:
             raise ValueError('level value must be between 0 and 100')
         args = [str(level)]
         self._transport.function_call('AHKSetSendLevel', args)
 
     def get_send_level(self) -> int:
+        """
+        Get the current `SendLevel <https://www.autohotkey.com/docs/commands/SendLevel.htm>`_
+        (I.E. the value of ``A_SendLevel``)
+        """
         resp = self._transport.function_call('AHKGetSendLevel')
         return resp
 
     # fmt: off
     @overload
     def send(self, s: str, *, raw: bool = False, key_delay: Optional[int] = None, key_press_duration: Optional[int] = None) -> None: ...
     @overload
@@ -1089,14 +1056,17 @@
         s: str,
         *,
         raw: bool = False,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Send <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         if key_delay:
             args.append(str(key_delay))
         else:
             args.append('')
         if key_press_duration:
             args.append(str(key_press_duration))
@@ -1124,14 +1094,17 @@
         self,
         s: str,
         *,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SendRaw <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         resp = self.send(
             s, raw=True, key_delay=key_delay, key_press_duration=key_press_duration, blocking=blocking
         )
         return resp
 
     # fmt: off
     @overload
@@ -1140,14 +1113,17 @@
     def send_input(self, s: str, *, blocking: Literal[True]) -> None: ...
     @overload
     def send_input(self, s: str, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def send_input(self, s: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def send_input(self, s: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SendInput <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         resp = self._transport.function_call('AHKSendInput', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     def type(self, s: str) -> None: ...
@@ -1155,14 +1131,17 @@
     def type(self, s: str, *, blocking: Literal[True]) -> None: ...
     @overload
     def type(self, s: str, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def type(self, s: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def type(self, s: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Like :py:meth:`send_input` but performs necessary escapes for you.
+        """
         resp = self.send_input(type_escape(s), blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     def send_play(self, s: str, *, key_delay: Optional[int] = None, key_press_duration: Optional[int] = None) -> None: ...
     @overload
@@ -1176,14 +1155,17 @@
         self,
         s: str,
         *,
         key_delay: Optional[int] = None,
         key_press_duration: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SendPlay <https://www.autohotkey.com/docs/v1/lib/Send.htm>`_
+        """
         args = [s]
         if key_delay:
             args.append(str(key_delay))
         else:
             args.append('')
         if key_press_duration:
             args.append(str(key_press_duration))
@@ -1202,14 +1184,17 @@
     def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def set_capslock_state(
         self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
         args: List[str] = []
         if state is not None:
             if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
                 raise ValueError(
                     f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
                 )
             args.append(str(state))
@@ -1226,14 +1211,17 @@
     def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[True]) -> None: ...
     @overload
     def set_volume(self, value: int, device_number: int = 1, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def set_volume(
         self, value: int, device_number: int = 1, *, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SoundSetWaveVolume <https://www.autohotkey.com/docs/commands/SoundSetWaveVolume.htm>`_
+        """
         args = [str(device_number), str(value)]
         return self._transport.function_call('AHKSetVolume', args, blocking=blocking)
 
     # fmt: off
     @overload
     def show_traytip(self, title: str, text: str, second: float = 1.0, type_id: int = 1, *, silent: bool = False, large_icon: bool = False) -> None: ...
     @overload
@@ -1250,14 +1238,17 @@
         second: float = 1.0,
         type_id: int = 1,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `TrayTip <https://www.autohotkey.com/docs/commands/TrayTip.htm>`_
+        """
         option = type_id + (16 if silent else 0) + (32 if large_icon else 0)
         args = [title, text, str(second), str(option)]
         return self._transport.function_call('AHKTrayTip', args, blocking=blocking)
 
     # fmt: off
     @overload
     def show_error_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1274,14 +1265,17 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for error-style messages
+        """
         return self.show_traytip(
             title=title, text=text, second=second, type_id=3, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     # fmt: off
     @overload
     def show_info_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1298,14 +1292,17 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for info-style messages
+        """
         return self.show_traytip(
             title=title, text=text, second=second, type_id=1, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     # fmt: off
     @overload
     def show_warning_traytip(self, title: str, text: str, second: float = 1.0, *, silent: bool = False, large_icon: bool = False) -> None: ...
@@ -1322,25 +1319,31 @@
         text: str,
         second: float = 1.0,
         *,
         silent: bool = False,
         large_icon: bool = False,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Convenience method for :py:meth:`show_traytip` for warning-style messages
+        """
         return self.show_traytip(
             title=title, text=text, second=second, type_id=2, silent=silent, large_icon=large_icon, blocking=blocking
         )
 
     def show_tooltip(
         self,
         text: str = '',
         x: Optional[int] = None,
         y: Optional[int] = None,
         which: int = 1,
     ) -> None:
+        """
+        Analog for `ToolTip <https://www.autohotkey.com/docs/commands/ToolTip.htm>`_
+        """
         if which not in range(1, 21):
             raise ValueError('which must be an integer between 1 and 20')
         args = [text]
         if x is not None:
             args.append(str(x))
         else:
             args.append('')
@@ -1362,14 +1365,17 @@
     def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: Literal[True]) -> None: ...
     @overload
     def sound_beep(self, frequency: int = 523, duration: int = 150, *, blocking: bool = True) -> Optional[FutureResult[None]]: ...
     # fmt: on
     def sound_beep(
         self, frequency: int = 523, duration: int = 150, *, blocking: bool = True
     ) -> Optional[FutureResult[None]]:
+        """
+        Analog for `SoundBeep <https://www.autohotkey.com/docs/commands/SoundBeep.htm>`_
+        """
         args = [str(frequency), str(duration)]
         self._transport.function_call('AHKSoundBeep', args, blocking=blocking)
         return None
 
     # fmt: off
     @overload
     def sound_get(self, device_number: int = 1, component_type: str = 'MASTER', control_type: str = 'VOLUME') -> str: ...
@@ -1384,39 +1390,48 @@
         self,
         device_number: int = 1,
         component_type: str = 'MASTER',
         control_type: str = 'VOLUME',
         *,
         blocking: bool = True,
     ) -> Union[str, FutureResult[str]]:
+        """
+        Analog for `SoundGet <https://www.autohotkey.com/docs/commands/SoundGet.htm>`_
+        """
         args = [str(device_number), component_type, control_type]
         return self._transport.function_call('AHKSoundGet', args, blocking=blocking)
 
     # fmt: off
     @overload
     def sound_play(self, filename: str) -> None: ...
     @overload
     def sound_play(self, filename: str, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def sound_play(self, filename: str, *, blocking: Literal[True]) -> None: ...
     @overload
     def sound_play(self, filename: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def sound_play(self, filename: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SoundPlay <https://www.autohotkey.com/docs/commands/SoundPlay.htm>`_
+        """
         return self._transport.function_call('AHKSoundPlay', [filename], blocking=blocking)
 
     def sound_set(
         self,
         value: Union[str, int, float],
         device_number: int = 1,
         component_type: str = 'MASTER',
         control_type: str = 'VOLUME',
         *,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SoundSet <https://www.autohotkey.com/docs/commands/SoundSet.htm>`_
+        """
         args = [str(device_number), component_type, control_type, str(value)]
         return self._transport.function_call('AHKSoundSet', args, blocking=blocking)
 
     # fmt: off
     @overload
     def win_get(self, title: str = '', text: str = '', exclude_title: str = '', exclude_text: str = '', *, title_match_mode: Optional[TitleMatchMode] = None, detect_hidden_windows: Optional[bool] = None) -> Union[Window, None]: ...
     @overload
@@ -1433,14 +1448,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Window, None, FutureResult[Union[None, Window]]]:
+        """
+        Analog for `WinGet <https://www.autohotkey.com/docs/commands/WinGet.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1529,14 +1547,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, FutureResult[str]]:
+        """
+        Analog for `WinGetClass <https://www.autohotkey.com/docs/commands/WinGetClass.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1561,14 +1582,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Position, None, FutureResult[Union[Position, None]]]:
+        """
+        Analog for `WinGetPos <https://www.autohotkey.com/docs/commands/WinGetPos.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1593,14 +1617,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[Window, None, FutureResult[Union[Window, None]]]:
+        """
+        Like the IDLast subcommand for WinGet
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1625,14 +1652,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[int, None, FutureResult[Union[int, None]]]:
+        """
+        Get a window by process ID.
+
+        Like the pid subcommand for WinGet
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1657,14 +1689,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, str, FutureResult[Optional[str]]]:
+        """
+        Get the process name of a window
+
+        Analog for `ProcessName subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ProcessName>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1689,14 +1726,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[str, None, Union[None, str, FutureResult[Optional[str]]]]:
+        """
+        Get the process path for a window.
+
+        Analog for the `ProcessPath subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ProcessPath>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1721,14 +1763,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[int, FutureResult[int]]:
+        """
+        Analog for the `Count subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#Count>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1753,14 +1798,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, int, FutureResult[Optional[int]]]:
+        """
+        Analog for the `MinMax subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#MinMax>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1785,14 +1833,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[List[Control], None, FutureResult[Optional[List[Control]]]]:
+        """
+        Analog for the `ControlList subcommand for WinGet <https://www.autohotkey.com/docs/v1/lib/WinGet.htm#ControlList>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1865,14 +1916,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinActivate <https://www.autohotkey.com/docs/commands/WinActivate.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -1898,14 +1952,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinSetTitle <https://www.autohotkey.com/docs/commands/WinSetTitle.htm>`_
+        """
         args = [new_title, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -1953,14 +2010,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `AlwaysOnTop subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#AlwaysOnTop>`_
+        """
         args = [str(toggle), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2007,14 +2067,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Bottom subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Bottom>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2039,14 +2102,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Top subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Top>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2071,14 +2137,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Disable subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Disable>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2103,14 +2172,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Enable subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Enable>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2135,14 +2207,18 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Redraw subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Redraw>`_
+        """
+
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2168,14 +2244,18 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, FutureResult[bool]]:
+        """
+        Analog for `Style subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Style>`_
+        """
+
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2223,14 +2303,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, FutureResult[bool]]:
+        """
+        Analog for `ExStyle subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#ExStyle>`_
+        """
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2278,14 +2361,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, FutureResult[bool]]:
+        """
+        Analog for `Region subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Region>`_
+        """
         args = [options, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2333,14 +2419,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Transparent subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Transparent>`_
+        """
         args = [str(transparency), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2388,14 +2477,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `TransColor subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#TransColor>`_
+        """
         args = [str(color), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
                 args.append('On')
             elif detect_hidden_windows is False:
                 args.append('Off')
             else:
@@ -2479,14 +2571,17 @@
         click_count: Optional[int] = None,
         direction: Optional[Literal['U', 'D', 'Up', 'Down']] = None,
         *,
         relative: Optional[bool] = None,
         blocking: bool = True,
         coord_mode: Optional[CoordModeRelativeTo] = None,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `Click <https://www.autohotkey.com/docs/commands/Click.htm>`_
+        """
         if x or y:
             if y is None and isinstance(x, tuple) and len(x) == 2:
                 #  allow position to be specified by a two-sequence tuple
                 x, y = x
             assert x is not None and y is not None, 'If provided, position must be specified by x AND y'
         if button is None:
             button = 'L'
@@ -2523,15 +2618,15 @@
         scale_height: Optional[int] = None,
         scale_width: Optional[int] = None,
         transparent: Optional[str] = None,
         icon: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[Tuple[int, int], None, FutureResult[Optional[Tuple[int, int]]]]:
         """
-        https://www.autohotkey.com/docs/commands/ImageSearch.htm
+        Analog for `ImageSearch <https://www.autohotkey.com/docs/commands/ImageSearch.htm>`_
         """
 
         if scale_height and not scale_width:
             scale_width = -1
         elif scale_width and not scale_height:
             scale_height = -1
 
@@ -2569,14 +2664,17 @@
         from_position: Optional[Tuple[int, int]] = None,
         speed: Optional[int] = None,
         button: MouseButton = 1,
         relative: Optional[bool] = None,
         blocking: bool = True,
         coord_mode: Optional[CoordModeRelativeTo] = None,
     ) -> None:
+        """
+        Analog for `MouseClickDrag <https://www.autohotkey.com/docs/commands/MouseClickDrag.htm>`_
+        """
         if from_position:
             x1, y1 = from_position
             args = [str(button), str(x1), str(y1), str(x), str(y)]
         else:
             args = [str(button), '', '', str(x), str(y)]
 
         if speed:
@@ -2611,14 +2709,17 @@
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         alt: bool = False,
         slow: bool = False,
         rgb: bool = True,
         blocking: bool = True,
     ) -> Union[str, FutureResult[str]]:
+        """
+        Analog for `PixelGetColor <https://www.autohotkey.com/docs/commands/PixelGetColor.htm>`_
+        """
         args = [str(x), str(y), coord_mode or '']
 
         options = ' '.join(word for word, val in zip(('Alt', 'Slow', 'RGB'), (alt, slow, rgb)) if val)
         args.append(options)
 
         resp = self._transport.function_call('AHKPixelGetColor', args, blocking=blocking)
         return resp
@@ -2641,14 +2742,17 @@
         variation: int = 0,
         *,
         coord_mode: Optional[CoordModeRelativeTo] = None,
         fast: bool = True,
         rgb: bool = True,
         blocking: bool = True,
     ) -> Union[Optional[Tuple[int, int]], FutureResult[Optional[Tuple[int, int]]]]:
+        """
+        Analog for `PixelSearch <https://www.autohotkey.com/docs/commands/PixelSearch.htm>`_
+        """
         x1, y1 = search_region_start
         x2, y2 = search_region_end
         args = [str(x1), str(y1), str(x2), str(y2), str(color), str(variation)]
         mode = ' '.join(word for word, val in zip(('Fast', 'RGB'), (fast, rgb)) if val)
         args.append(mode)
         args.append(coord_mode or '')
         resp = self._transport.function_call('AHKPixelSearch', args, blocking=blocking)
@@ -2672,14 +2776,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         blocking: bool = True,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinClose <https://www.autohotkey.com/docs/commands/WinClose.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2707,14 +2814,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinKill <https://www.autohotkey.com/docs/commands/WinKill.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2741,14 +2851,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinMinimize <https://www.autohotkey.com/docs/commands/WinMinimize.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2773,14 +2886,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinMaximize <https://www.autohotkey.com/docs/commands/WinMaximize.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2805,14 +2921,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinRestore <https://www.autohotkey.com/docs/commands/WinRestore.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2838,14 +2957,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[Window, FutureResult[Window]]:
+        """
+        Analog for `WinWait <https://www.autohotkey.com/docs/commands/WinWait.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2872,14 +2994,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[Window, FutureResult[Window]]:
+        """
+        Analog for `WinWaitActive <https://www.autohotkey.com/docs/commands/WinWaitActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2906,14 +3031,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[Window, FutureResult[Window]]:
+        """
+        Analog for `WinWaitNotActive <https://www.autohotkey.com/docs/commands/WinWaitActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2940,14 +3068,17 @@
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         timeout: Optional[int] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinWaitClose <https://www.autohotkey.com/docs/commands/WinWaitClose.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -2973,14 +3104,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinShow <https://www.autohotkey.com/docs/commands/WinShow.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3005,14 +3139,17 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinHide <https://www.autohotkey.com/docs/commands/WinHide.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3037,14 +3174,19 @@
         exclude_title: str = '',
         exclude_text: str = '',
         *,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[bool, FutureResult[bool]]:
+        """
+        Check if a window is active.
+
+        Uses `WinActive <https://www.autohotkey.com/docs/v1/lib/WinActive.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3073,14 +3215,17 @@
         text: str = '',
         exclude_title: str = '',
         exclude_text: str = '',
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `WinMove <https://www.autohotkey.com/docs/commands/WinMove.htm>`_
+        """
         args = self._format_win_args(
             title=title,
             text=text,
             exclude_title=exclude_title,
             exclude_text=exclude_text,
             title_match_mode=title_match_mode,
             detect_hidden_windows=detect_hidden_windows,
@@ -3099,21 +3244,30 @@
     def get_clipboard(self, *, blocking: Literal[False]) -> FutureResult[str]: ...
     @overload
     def get_clipboard(self, *, blocking: Literal[True]) -> str: ...
     @overload
     def get_clipboard(self, *, blocking: bool = True) -> Union[str, FutureResult[str]]: ...
     # fmt: on
     def get_clipboard(self, *, blocking: bool = True) -> Union[str, FutureResult[str]]:
+        """
+        Get the string contents of the clipboard
+        """
         return self._transport.function_call('AHKGetClipboard', blocking=blocking)
 
     def set_clipboard(self, s: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+        """
+        Set the contents of the clipboard
+        """
         args = [s]
         return self._transport.function_call('AHKSetClipboard', args, blocking=blocking)
 
     def get_clipboard_all(self, *, blocking: bool = True) -> Union[bytes, FutureResult[bytes]]:
+        """
+        Get the full binary contents of the keyboard. The return value is intended to be used with :py:meth:`set_clipboard_all`
+        """
         return self._transport.function_call('AHKGetClipboardAll', blocking=blocking)
 
     # fmt: off
     @overload
     def set_clipboard_all(self, contents: bytes) -> None: ...
     @overload
     def set_clipboard_all(self, contents: bytes, *, blocking: Literal[False]) -> FutureResult[None]: ...
@@ -3121,14 +3275,17 @@
     def set_clipboard_all(self, contents: bytes, *, blocking: Literal[True]) -> None: ...
     @overload
     def set_clipboard_all(self, contents: bytes, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def set_clipboard_all(
         self, contents: bytes, *, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Set the full binary contents of the clipboard. Expects bytes object as returned by :py:meth:`get_clipboard_all`
+        """
         # TODO: figure out how to do this without a tempfile
         if not isinstance(contents, bytes):
             raise ValueError('Malformed data. Can only set bytes as returned by get_clipboard_all')
         if not contents:
             raise ValueError('bytes must be nonempty. If you want to clear the clipboard, use `set_clipboard`')
         with tempfile.NamedTemporaryFile(prefix='ahk-python', suffix='.clip', mode='wb', delete=False) as f:
             f.write(contents)
@@ -3142,14 +3299,18 @@
                 os.remove(f.name)
             except Exception:
                 pass
 
     def on_clipboard_change(
         self, callback: Callable[[int], Any], ex_handler: Optional[Callable[[int, Exception], Any]] = None
     ) -> None:
+        """
+        call a function in response to clipboard change.
+        Uses `OnClipboardChange() <https://www.autohotkey.com/docs/commands/OnClipboardChange.htm#function>`_
+        """
         self._transport.on_clipboard_change(callback, ex_handler)
 
     # fmt: off
     @overload
     def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False) -> None: ...
     @overload
     def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: Literal[False]) -> FutureResult[None]: ...
@@ -3157,24 +3318,32 @@
     def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: Literal[True]) -> None: ...
     @overload
     def clip_wait(self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def clip_wait(
         self, timeout: Optional[float] = None, wait_for_any_data: bool = False, *, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Wait until the clipboard contents change
+
+        Analog for `ClipWait <https://www.autohotkey.com/docs/v1/lib/ClipWait.htm>`_
+        """
         args = [str(timeout) if timeout else '']
         if wait_for_any_data:
             args.append('1')
         return self._transport.function_call('AHKClipWait', args, blocking=blocking)
 
     def block_input(
         self,
         value: Literal['On', 'Off', 'Default', 'Send', 'Mouse', 'MouseMove', 'MouseMoveOff', 'SendAndMouse'],
         /,  # flake8: noqa
     ) -> None:
+        """
+        Analog for `BlockInput <https://www.autohotkey.com/docs/commands/BlockInput.htm>`_
+        """
         self._transport.function_call('AHKBlockInput', args=[value])
 
     # fmt: off
     @overload
     def reg_delete(self, key_name: str, value_name: Optional[str] = None) -> None: ...
     @overload
     def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[False]) -> Union[None, FutureResult[None]]: ...
@@ -3182,14 +3351,17 @@
     def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[True]) -> None: ...
     @overload
     def reg_delete(self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def reg_delete(
         self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `RegDelete <https://www.autohotkey.com/docs/commands/RegDelete.htm>`_
+        """
         args = [key_name, value_name if value_name is not None else '']
         return self._transport.function_call('AHKRegDelete', args, blocking=blocking)
 
     # fmt: off
     @overload
     def reg_write(self, value_type: Literal['REG_SZ', 'REG_EXPAND_SZ', 'REG_MULTI_SZ', 'REG_DWORD', 'REG_BINARY'], key_name: str, value_name: Optional[str] = None, value: Optional[str] = None) -> None: ...
     @overload
@@ -3204,14 +3376,17 @@
         value_type: Literal['REG_SZ', 'REG_EXPAND_SZ', 'REG_MULTI_SZ', 'REG_DWORD', 'REG_BINARY'],
         key_name: str,
         value_name: Optional[str] = None,
         value: Optional[str] = None,
         *,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `RegWrite <https://www.autohotkey.com/docs/commands/RegWrite.htm>`_
+        """
         args = [value_type, key_name]
         if value_name is not None:
             args.append(value_name)
         else:
             args.append('')
         if value is not None:
             args.append(value)
@@ -3226,15 +3401,21 @@
     def reg_read(self, key_name: str, value_name: Optional[str] = None, *, blocking: Literal[True]) -> str: ...
     @overload
     def reg_read(self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True) -> Union[str, FutureResult[str]]: ...
     # fmt: on
     def reg_read(
         self, key_name: str, value_name: Optional[str] = None, *, blocking: bool = True
     ) -> Union[str, FutureResult[str]]:
+        """
+        Analog for `RegRead <https://www.autohotkey.com/docs/commands/RegRead.htm>`_
+        """
         args = [key_name]
         if value_name is not None:
             args.append(value_name)
         return self._transport.function_call('AHKRegRead', args, blocking=blocking)
 
     def block_forever(self) -> NoReturn:
+        """
+        Blocks (sleeps) forever. Utility method to prevent script from exiting.
+        """
         while True:
             sleep(1)
```

### Comparing `ahk-1.0.0b0/ahk/_sync/transport.py` & `ahk-1.0.1/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_sync/window.py` & `ahk-1.0.1/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/_utils.py` & `ahk-1.0.1/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/directives.py` & `ahk-1.0.1/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/keys.py` & `ahk-1.0.1/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/message.py` & `ahk-1.0.1/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/templates/daemon.ahk` & `ahk-1.0.1/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk/templates/hotkeys.ahk` & `ahk-1.0.1/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/ahk.egg-info/PKG-INFO` & `ahk-1.0.1/ahk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -15,48 +15,49 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+Provides-Extra: binary
 
 # ahk
 
 A fully typed Python wrapper around AHK.
 
 [![Docs](https://readthedocs.org/projects/ahk/badge/?version=latest)](https://ahk.readthedocs.io/en/latest/?badge=latest)
-[![Build](https://ci.appveyor.com/api/projects/status/2c53x6gglw9nxgj1/branch/master?svg=true)](https://ci.appveyor.com/project/spyoungtech/ahk/branch/master)
+[![Build](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml/badge.svg)](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml)
 [![version](https://img.shields.io/pypi/v/ahk.svg?colorB=blue)](https://pypi.org/project/ahk/)
 [![pyversion](https://img.shields.io/pypi/pyversions/ahk.svg?)](https://pypi.org/project/ahk/)
 [![Coverage](https://coveralls.io/repos/github/spyoungtech/ahk/badge.svg?branch=master)](https://coveralls.io/github/spyoungtech/ahk?branch=master)
 [![Downloads](https://pepy.tech/badge/ahk)](https://pepy.tech/project/ahk)
 
 # Installation
 
 ```
 pip install ahk
 ```
 Requires Python 3.8+
 
-See also [Non-Python dependencies](#non-python-dependencies)
+See also [Non-Python dependencies](#deps)
 
 # Usage
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
 
 ahk.mouse_move(x=100, y=100, blocking=True)  # Blocks until mouse finishes moving (the default)
 ahk.mouse_move(x=150, y=150, speed=10, blocking=True) # Moves the mouse to x, y taking 'speed' seconds to move
 print(ahk.mouse_position)  #  (150, 150)
 ```
 
-![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/master/docs/_static/ahk.gif)
+![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/9d049a327c7a10c9f19dfef89fc63668695023fc/docs/_static/ahk.gif)
 
 # Examples
 
 Non-exhaustive examples of some functions available with this package. Full documentation coming soon!
 
 ## Hotkeys
 
@@ -460,19 +461,36 @@
 This library is fully type-hinted, allowing you to leverage tools like `mypy` to help validate the type-correctness
 of your code. IDEs that implement type-checking features are also able to leverage type hints to help ensure your
 code is safe.
 
 
 ## Run arbitrary AutoHotkey scripts
 
-TBD
+You can also run arbitrary AutoHotkey code either as a `.ahk` script file or as a string containing AHK code.
 
+```python
+from ahk import AHK
+ahk = AHK()
+my_script = '''\
+MouseMove, 100, 100
+; etc...
+'''
+
+ahk.run_script(my_script)
+```
+
+```python
+from ahk import AHK
+ahk = AHK()
+script_path = r'C:\Path\To\myscript.ahk'
+ahk.run_script(script_path)
+```
 
 
-<a name="deps" />
+<a name="deps"></a>
 
 # Non-Python dependencies
 
 To use this package, you need the [AutoHotkey executable](https://www.autohotkey.com/download/). It's expected to be on PATH by default.
 
 Note: this should be AutoHotkey V1. AutoHotkey V2 is not yet supported.
```

### Comparing `ahk-1.0.0b0/ahk.egg-info/SOURCES.txt` & `ahk-1.0.1/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/buildunasync.py` & `ahk-1.0.1/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0b0/docs/README.md` & `ahk-1.0.1/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # ahk
 
 A fully typed Python wrapper around AHK.
 
 [![Docs](https://readthedocs.org/projects/ahk/badge/?version=latest)](https://ahk.readthedocs.io/en/latest/?badge=latest)
-[![Build](https://ci.appveyor.com/api/projects/status/2c53x6gglw9nxgj1/branch/master?svg=true)](https://ci.appveyor.com/project/spyoungtech/ahk/branch/master)
+[![Build](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml/badge.svg)](https://github.com/spyoungtech/ahk/actions/workflows/test.yaml)
 [![version](https://img.shields.io/pypi/v/ahk.svg?colorB=blue)](https://pypi.org/project/ahk/)
 [![pyversion](https://img.shields.io/pypi/pyversions/ahk.svg?)](https://pypi.org/project/ahk/)
 [![Coverage](https://coveralls.io/repos/github/spyoungtech/ahk/badge.svg?branch=master)](https://coveralls.io/github/spyoungtech/ahk?branch=master)
 [![Downloads](https://pepy.tech/badge/ahk)](https://pepy.tech/project/ahk)
 
 # Installation
 
 ```
 pip install ahk
 ```
 Requires Python 3.8+
 
-See also [Non-Python dependencies](#non-python-dependencies)
+See also [Non-Python dependencies](#deps)
 
 # Usage
 
 ```python
 from ahk import AHK
 
 ahk = AHK()
 
 ahk.mouse_move(x=100, y=100, blocking=True)  # Blocks until mouse finishes moving (the default)
 ahk.mouse_move(x=150, y=150, speed=10, blocking=True) # Moves the mouse to x, y taking 'speed' seconds to move
 print(ahk.mouse_position)  #  (150, 150)
 ```
 
-![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/master/docs/_static/ahk.gif)
+![ahk](https://raw.githubusercontent.com/spyoungtech/ahk/9d049a327c7a10c9f19dfef89fc63668695023fc/docs/_static/ahk.gif)
 
 # Examples
 
 Non-exhaustive examples of some functions available with this package. Full documentation coming soon!
 
 ## Hotkeys
 
@@ -438,19 +438,36 @@
 This library is fully type-hinted, allowing you to leverage tools like `mypy` to help validate the type-correctness
 of your code. IDEs that implement type-checking features are also able to leverage type hints to help ensure your
 code is safe.
 
 
 ## Run arbitrary AutoHotkey scripts
 
-TBD
+You can also run arbitrary AutoHotkey code either as a `.ahk` script file or as a string containing AHK code.
 
+```python
+from ahk import AHK
+ahk = AHK()
+my_script = '''\
+MouseMove, 100, 100
+; etc...
+'''
+
+ahk.run_script(my_script)
+```
+
+```python
+from ahk import AHK
+ahk = AHK()
+script_path = r'C:\Path\To\myscript.ahk'
+ahk.run_script(script_path)
+```
 
 
-<a name="deps" />
+<a name="deps"></a>
 
 # Non-Python dependencies
 
 To use this package, you need the [AutoHotkey executable](https://www.autohotkey.com/download/). It's expected to be on PATH by default.
 
 Note: this should be AutoHotkey V1. AutoHotkey V2 is not yet supported.
```

### Comparing `ahk-1.0.0b0/setup.cfg` & `ahk-1.0.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.0.0b
+version = 1.0.1
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords = 
@@ -39,14 +39,17 @@
 	ahk._sync
 install_requires = 
 	typing_extensions; python_version < "3.11"
 	jinja2>=3.0
 cmdclass = 
 	build_py = buildunasync.build_py
 
+[options.extras_require]
+binary = ahk-binary==1.1.33.9
+
 [options.package_data]
 ahk = 
 	py.typed
 	templates/*.ahk
 
 [egg_info]
 tag_build =
```

