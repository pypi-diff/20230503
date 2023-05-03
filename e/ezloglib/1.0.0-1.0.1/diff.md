# Comparing `tmp/ezloglib-1.0.0.tar.gz` & `tmp/ezloglib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezloglib-1.0.0.tar", last modified: Wed Mar  1 17:00:29 2023, max compression
+gzip compressed data, was "ezloglib-1.0.1.tar", last modified: Wed May  3 17:20:46 2023, max compression
```

## Comparing `ezloglib-1.0.0.tar` & `ezloglib-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 17:00:30.000000 ezloglib-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-02-02 20:54:56.000000 ezloglib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5507 2023-03-01 17:00:30.000000 ezloglib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2023-03-01 16:49:44.000000 ezloglib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezlog/
--rw-rw-rw-   0        0        0      368 2023-02-28 14:59:22.000000 ezloglib-1.0.0/ezlog/__init__.py
--rw-rw-rw-   0        0        0      101 2023-03-01 15:52:58.000000 ezloglib-1.0.0/ezlog/_types.py
--rw-rw-rw-   0        0        0     1660 2023-03-01 16:03:58.000000 ezloglib-1.0.0/ezlog/defaults.py
--rw-rw-rw-   0        0        0      612 2023-03-01 15:35:28.000000 ezloglib-1.0.0/ezlog/exceptions.py
--rw-rw-rw-   0        0        0     4213 2023-02-28 16:28:24.000000 ezloglib-1.0.0/ezlog/handlers.py
--rw-rw-rw-   0        0        0    10606 2023-03-01 15:53:06.000000 ezloglib-1.0.0/ezlog/logger.py
--rw-rw-rw-   0        0        0     2942 2023-02-28 14:57:28.000000 ezloglib-1.0.0/ezlog/loggergroup.py
--rw-rw-rw-   0        0        0     3225 2023-02-28 14:51:20.000000 ezloglib-1.0.0/ezlog/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/
--rw-rw-rw-   0        0        0     5507 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-01 17:00:30.000000 ezloglib-1.0.0/ezloglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1027 2023-03-01 16:59:48.000000 ezloglib-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      118 2023-03-01 17:00:30.000000 ezloglib-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 17:20:46.000000 ezloglib-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-02-02 19:54:56.000000 ezloglib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5519 2023-05-03 17:20:48.000000 ezloglib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3394 2023-05-03 17:18:36.000000 ezloglib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezlog/
+-rw-rw-rw-   0        0        0      368 2023-02-28 13:59:22.000000 ezloglib-1.0.1/ezlog/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-03 16:37:30.000000 ezloglib-1.0.1/ezlog/_types.py
+-rw-rw-rw-   0        0        0     1660 2023-05-03 16:58:38.000000 ezloglib-1.0.1/ezlog/defaults.py
+-rw-rw-rw-   0        0        0      612 2023-03-01 14:35:28.000000 ezloglib-1.0.1/ezlog/exceptions.py
+-rw-rw-rw-   0        0        0     4257 2023-05-03 16:28:56.000000 ezloglib-1.0.1/ezlog/handlers.py
+-rw-rw-rw-   0        0        0    10606 2023-03-01 14:53:06.000000 ezloglib-1.0.1/ezlog/logger.py
+-rw-rw-rw-   0        0        0     2942 2023-02-28 13:57:28.000000 ezloglib-1.0.1/ezlog/loggergroup.py
+-rw-rw-rw-   0        0        0     3116 2023-05-03 16:58:00.000000 ezloglib-1.0.1/ezlog/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/
+-rw-rw-rw-   0        0        0     5519 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 17:20:46.000000 ezloglib-1.0.1/ezloglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1027 2023-05-03 17:18:36.000000 ezloglib-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      118 2023-05-03 17:20:48.000000 ezloglib-1.0.1/setup.cfg
```

### Comparing `ezloglib-1.0.0/LICENSE` & `ezloglib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezloglib-1.0.0/PKG-INFO` & `ezloglib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezloglib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Small modern colored logging library
 Author-email: ftdot <ftdoot@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ftdot
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,15 +51,15 @@
 # ezlog
 
 [![Documentation](https://img.shields.io/readthedocs/ezlog?style=for-the-badge)](https://ezlog.readthedocs.io/)
 [![Issues](https://img.shields.io/github/issues/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/issues)
 [![Latest tag](https://img.shields.io/github/v/tag/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/tags)
 [![PyPI](https://img.shields.io/pypi/v/ezloglib?style=for-the-badge)](https://pypi.org/project/ezloglib)
   
-Modern, simple in use, colored logging library for python.
+Modern, simple in use, fast, colored logging library for python.
 
 * Formatting support
 * Stdout\\Stderr\\File handlers
 * Easy to use & add custom handlers
 * Colored and customizable
 
 
@@ -120,15 +120,15 @@
 except Exception as e:
     # NOTE: You can use also debug, critical and other log levels to print exception
     main_logger.exception('Exception example', exception=e)
 
 main_logger.info('It is continue work')
 ```
 
-File: [examples/presentation.py](examples/groups_filelogging.py)
+File: [examples/groups_filelogging.py](examples/groups_filelogging.py)
 
 ```py
 
 import ezlog
 
 # declare stdout handler with log level - debug
 file_handler = ezlog.FileHandler('example.log', log_level='debug')
```

### Comparing `ezloglib-1.0.0/README.md` & `ezloglib-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # ezlog
 
 [![Documentation](https://img.shields.io/readthedocs/ezlog?style=for-the-badge)](https://ezlog.readthedocs.io/)
 [![Issues](https://img.shields.io/github/issues/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/issues)
 [![Latest tag](https://img.shields.io/github/v/tag/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/tags)
 [![PyPI](https://img.shields.io/pypi/v/ezloglib?style=for-the-badge)](https://pypi.org/project/ezloglib)
   
-Modern, simple in use, colored logging library for python.
+Modern, simple in use, fast, colored logging library for python.
 
 * Formatting support
 * Stdout\\Stderr\\File handlers
 * Easy to use & add custom handlers
 * Colored and customizable
 
 
@@ -75,15 +75,15 @@
 except Exception as e:
     # NOTE: You can use also debug, critical and other log levels to print exception
     main_logger.exception('Exception example', exception=e)
 
 main_logger.info('It is continue work')
 ```
 
-File: [examples/presentation.py](examples/groups_filelogging.py)
+File: [examples/groups_filelogging.py](examples/groups_filelogging.py)
 
 ```py
 
 import ezlog
 
 # declare stdout handler with log level - debug
 file_handler = ezlog.FileHandler('example.log', log_level='debug')
```

### Comparing `ezloglib-1.0.0/ezlog/defaults.py` & `ezloglib-1.0.1/ezlog/defaults.py`

 * *Files identical despite different names*

### Comparing `ezloglib-1.0.0/ezlog/exceptions.py` & `ezloglib-1.0.1/ezlog/exceptions.py`

 * *Files identical despite different names*

### Comparing `ezloglib-1.0.0/ezlog/handlers.py` & `ezloglib-1.0.1/ezlog/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 
 import sys
 import typing
 from os import PathLike
 from typing import TextIO
 
 from .utils import LogLevel, level_names
+from ._types import LogLevelType
 
 __all__ = ['LoggerHandler', 'FileHandler', 'StdoutHandler', 'StderrHandler',]
 
 
 class LoggerHandler:
     """Handler for any IO"""
 
     def __init__(self,
                  io: TextIO | None = None,
-                 log_level: int | str = LogLevel.NOTSET,
+                 log_level: LogLevelType = LogLevel.NOTSET,
                  colors: bool = True,
                  exceptions: bool = True):
         """
         :param io: TextIO to handle
         :type io: TextIO
         :param log_level: Level of logging (by default is LogLevel.NOTSET)
         :type log_level: LogLevel | str
         :param colors: Enable colors for the handler
         :type colors: bool
         :param exceptions: Enable exception handling for this handler
         :type exceptions: bool
         """
 
         self.io          = io
-        self.log_level   = log_level if isinstance(log_level, LogLevel) else {v: k for k, v in level_names.items()}[log_level.upper()]
+        self.log_level   = log_level if isinstance(log_level, int) else {v: k for k, v in level_names.items()}[log_level.upper()]
         self.colors      = colors
         self.exceptions  = exceptions
 
     def write(self, text: str):
         """Writes given text to the IO if it doesn't equal to None
 
         :param text: Text to write into IO
@@ -69,15 +70,15 @@
         :type kwargs: typing.Any
 
         Parameters from the :class:`LoggerHandler`:
 
         :param io: TextIO to handle
         :type io: TextIO
         :param log_level: Level of logging (by default is LogLevel.NOTSET)
-        :type log_level: LogLevel
+        :type log_level: LogLevelType
         :param colors: Enable colors for the handler
         :type colors: bool
         :param exceptions: Enable exception handling for this handler
         :type exceptions: bool
         """
         if 'colors' in kwargs:
             super().__init__(open(path, 'w'), **kwargs)
@@ -100,15 +101,15 @@
         :type kwargs: typing.Any
 
         Parameters from the :class:`LoggerHandler`:
 
         :param io: TextIO to handle
         :type io: TextIO
         :param log_level: Level of logging (by default is LogLevel.NOTSET)
-        :type log_level: LogLevel
+        :type log_level: LogLevelType
         :param colors: Enable colors for the handler
         :type colors: bool
         :param exceptions: Enable exception handling for this handler
         :type exceptions: bool
         """
         super().__init__(sys.stdout, **kwargs)
 
@@ -126,15 +127,15 @@
         :type kwargs: typing.Any
 
         Parameters from the :class:`LoggerHandler`:
 
         :param io: TextIO to handle
         :type io: TextIO
         :param log_level: Level of logging (by default is LogLevel.NOTSET)
-        :type log_level: LogLevel
+        :type log_level: LogLevelType
         :param colors: Enable colors for the handler
         :type colors: bool
         :param exceptions: Enable exception handling for this handler
         :type exceptions: bool
         """
         super().__init__(sys.stderr, **kwargs)
```

### Comparing `ezloglib-1.0.0/ezlog/logger.py` & `ezloglib-1.0.1/ezlog/logger.py`

 * *Files identical despite different names*

### Comparing `ezloglib-1.0.0/ezlog/loggergroup.py` & `ezloglib-1.0.1/ezlog/loggergroup.py`

 * *Files identical despite different names*

### Comparing `ezloglib-1.0.0/ezlog/utils.py` & `ezloglib-1.0.1/ezlog/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,13 +118,8 @@
 
     :param cls: Class (must be Logger class)
     :type cls: Logger
     """
 
     # make bindings to the all log levels
     for level, name in level_names.items():
-        name_l = name.lower()
-
-        if getattr(cls, name_l, None) is not None:
-            continue
-
         setattr(cls, name.lower(), make_logger_binding(level))
```

### Comparing `ezloglib-1.0.0/ezloglib.egg-info/PKG-INFO` & `ezloglib-1.0.1/ezloglib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezloglib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Small modern colored logging library
 Author-email: ftdot <ftdoot@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ftdot
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,15 +51,15 @@
 # ezlog
 
 [![Documentation](https://img.shields.io/readthedocs/ezlog?style=for-the-badge)](https://ezlog.readthedocs.io/)
 [![Issues](https://img.shields.io/github/issues/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/issues)
 [![Latest tag](https://img.shields.io/github/v/tag/ftdot/ezlog?style=for-the-badge)](https://github.com/ftdot/ezlog/tags)
 [![PyPI](https://img.shields.io/pypi/v/ezloglib?style=for-the-badge)](https://pypi.org/project/ezloglib)
   
-Modern, simple in use, colored logging library for python.
+Modern, simple in use, fast, colored logging library for python.
 
 * Formatting support
 * Stdout\\Stderr\\File handlers
 * Easy to use & add custom handlers
 * Colored and customizable
 
 
@@ -120,15 +120,15 @@
 except Exception as e:
     # NOTE: You can use also debug, critical and other log levels to print exception
     main_logger.exception('Exception example', exception=e)
 
 main_logger.info('It is continue work')
 ```
 
-File: [examples/presentation.py](examples/groups_filelogging.py)
+File: [examples/groups_filelogging.py](examples/groups_filelogging.py)
 
 ```py
 
 import ezlog
 
 # declare stdout handler with log level - debug
 file_handler = ezlog.FileHandler('example.log', log_level='debug')
```

### Comparing `ezloglib-1.0.0/pyproject.toml` & `ezloglib-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ezloglib"
-version = "1.0.0"
+version = "1.0.1"
 description = "Small modern colored logging library"
 readme = "README.md"
 authors = [{ name = "ftdot", email = "ftdoot@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Environment :: Plugins",
     "Framework :: Sphinx",
```

