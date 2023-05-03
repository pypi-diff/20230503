# Comparing `tmp/cli3-1.0.2.tar.gz` & `tmp/cli3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cli3-1.0.2.tar", last modified: Mon Dec 26 20:22:14 2022, max compression
+gzip compressed data, was "cli3-1.1.0.tar", last modified: Wed May  3 00:29:46 2023, max compression
```

## Comparing `cli3-1.0.2.tar` & `cli3-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-12-26 20:22:14.566556 cli3-1.0.2/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1794 2022-12-26 20:22:14.566556 cli3-1.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-12-26 20:22:14.562556 cli3-1.0.2/cli/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      911 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6628 2022-12-26 20:20:07.000000 cli3-1.0.2/cli/app.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3991 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/argument.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     8539 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/command.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4665 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/context.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4991 2022-12-26 19:04:05.000000 cli3-1.0.2/cli/flag.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5017 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/help.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5323 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/parser.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-12-26 20:22:14.562556 cli3-1.0.2/cli/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3515 2022-12-26 20:18:43.000000 cli3-1.0.2/cli/tests/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-12-26 20:22:14.562556 cli3-1.0.2/cli/tests/app/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/tests/app/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2592 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/tests/app/v1.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1968 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/tests/app/v2.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       62 2022-11-16 03:04:43.000000 cli3-1.0.2/cli/tests/cli.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    12789 2022-12-26 19:24:44.000000 cli3-1.0.2/cli/wraps.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-12-26 20:22:14.562556 cli3-1.0.2/cli3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1794 2022-12-26 20:22:14.000000 cli3-1.0.2/cli3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      386 2022-12-26 20:22:14.000000 cli3-1.0.2/cli3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-12-26 20:22:14.000000 cli3-1.0.2/cli3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2022-12-26 20:22:14.000000 cli3-1.0.2/cli3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2022-12-26 20:22:14.000000 cli3-1.0.2/cli3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2022-12-26 20:22:14.566556 cli3-1.0.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      762 2022-12-26 20:21:53.000000 cli3-1.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1064 2020-10-21 03:10:04.000000 cli3-1.1.0/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-03 00:29:46.302776 cli3-1.1.0/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.1.0/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1343 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    13785 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6825 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/app.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4274 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/argument.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7041 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/command.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4501 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/flag.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4997 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/help.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7434 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/parser.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      111 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5816 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/app.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/tests/content/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2599 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/v1.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2002 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/v2.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    13997 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/wraps.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      402 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-03 00:29:46.302776 cli3-1.1.0/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      762 2023-05-03 00:28:52.000000 cli3-1.1.0/setup.py
```

### Comparing `cli3-1.0.2/PKG-INFO` & `cli3-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.0.2
+Version: 1.1.0
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
-Description: cli
-        ===
-        
-        [![forthebadge](https://forthebadge.com/images/badges/you-didnt-ask-for-this.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
-        
-        A highly configurable, dynamic, fast, and easy solution to managing
-        a command-line application. The goal is to make cli development as simple
-        and effective as possible for any configuration enabling the developer to
-        focus on function over form.
-        
-        Supports Python >= 3.7 and can run asynchronously or synchronously.
-        
-        This library took heavy initial inspiration by [urfave/cli](https://github.com/urfave/cli)
-        so credit to them for their work as well.
-        
-        ## Install
-        
-        ```bash
-        $ pip install cli3
-        ```
-        
-        ## Documentation
-        
-        More documentation is available in [`./docs`](https://github.com/imgurbot12/cli/tree/master/docs) or the hosted
-        documentation site at <https://cli3.readthedocs.org>.
-        
-        ## License
-        
-        See [`LICENSE`](./LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+cli
+===
+
+[![forthebadge](https://forthebadge.com/images/badges/you-didnt-ask-for-this.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
+
+A highly configurable, dynamic, fast, and easy solution to managing
+a command-line application. The goal is to make cli development as simple
+and effective as possible for any configuration enabling the developer to
+focus on function over form.
+
+Supports Python >= 3.7 and can run asynchronously or synchronously.
+
+This library took heavy initial inspiration by [urfave/cli](https://github.com/urfave/cli)
+so credit to them for their work as well.
+
+## Install
+
+```bash
+$ pip install cli3
+```
+
+## Documentation
+
+More documentation is available in [`./docs`](https://github.com/imgurbot12/cli/tree/master/docs) or the hosted
+documentation site at <https://cli3.readthedocs.org>.
+
+## License
+
+See [`LICENSE`](./LICENSE)
```

### Comparing `cli3-1.0.2/README.md` & `cli3-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cli3-1.0.2/cli/app.py` & `cli3-1.1.0/cli/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 """
-application definition which determines behavior and handling of arguments
+CLI Application Definition/Implementation
 """
 import sys
 import asyncio
-from io import RawIOBase
-from dataclasses import dataclass, field, InitVar
-from typing import Callable, Optional, List, Coroutine
+from typing import Callable, Optional, List, TextIO
 
+from .abc import *
 from .flag import Flags
-from .context import Context
-from .command import Action, Commands, CommandBase, Command
+from .command import Command
 from .help import help_action, help_flag, help_command
-from .parser import run_app, EX_USAGE, EX_UNAVAILABLE
+from .parser import run_app, EX_USAGE, EX_UNAVAILABLE, EX_CONFIG
 
 #** Variables **#
 __all__ = [
     'UsageErrorFunc',
     'ExitErrorFunc',
     'NotFoundFunc',
 
     'App'
 ]
 
 #: definition for usage-error function
-UsageErrorFunc = Callable[[Context, Command, str], None]
+UsageErrorFunc = Callable[[UsageError], None]
 
 #: definition for exit-error function
-ExitErrorFunc  = Callable[[Context, Command, str, int], None]
+ExitErrorFunc  = Callable[[ExitError], None]
 
 #: defintion for command-not-found function
-NotFoundFunc = Callable[[Context, Command, str], None]
+NotFoundFunc = Callable[[NotFoundError], None]
 
 #** Functions **#
 
-def get_event_loop() -> asyncio.BaseEventLoop:
+def get_event_loop() -> asyncio.AbstractEventLoop:
     """retrieve asyncio event loop"""
     try:
         loop = asyncio.get_running_loop()
     except:
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
     return loop
 
 #** Classes **#
 
-@dataclass
-class App(CommandBase):
+class App(AbsApplication, Command):
     """
     application determines handling of arguments and stores metadata
 
     :param name:              name of application
     :param usage:             specified usage description
     :param version:           symantic version number
     :param argsusage:         argument usage description
@@ -69,115 +66,114 @@
     :param after:             after-action function
     :param on_usage_error:    override usage-error function
     :param exit_with_error:   override exit-with-error function
     :param not_found_error:   override not-found-error function
     :param run_async:         return co-routine on run if true
     """
 
-    name:         str
-    usage:        str
-    version:      str           = '0.0.1'
-    argsusage:    Optional[str] = None
-    description:  Optional[str] = None
-    flags:        Flags         = field(default_factory=list, repr=False)
-    commands:     Commands      = field(default_factory=list, repr=False)
-    allow_parent: bool          = False
-
-    authors:   List[str]     = field(default_factory=list)
-    email:     Optional[str] = None
-    copyright: Optional[str] = None
-
-    writer:     RawIOBase = field(default=sys.stdout, repr=False)
-    err_writer: RawIOBase = field(default=sys.stderr, repr=False)
-
-    help_app_template: Optional[str] = field(default=None, repr=False)
-    help_cmd_template: Optional[str] = field(default=None, repr=False)
-
-    before: InitVar[Action]
-    action: InitVar[Action]
-    after:  InitVar[Action]
-
-    on_usage_error:  InitVar[UsageErrorFunc]
-    exit_with_error: InitVar[ExitErrorFunc]
-    not_found_error: InitVar[NotFoundFunc]
-
-    run_async: bool = False
-
-    def __post_init__(self,
-        before:          Action,
-        action:          Action,
-        after:           Action,
-        on_usage_error:  UsageErrorFunc,
-        exit_with_error: ExitErrorFunc,
-        not_found_error: NotFoundFunc,
+    def __init__(self,
+        name:              str,
+        version:           str                      = '0.0.1',
+        usage:             Optional[str]            = None,
+        argsusage:         Optional[str]            = None,
+        description:       Optional[str]            = None,
+        flags:             Optional[Flags]          = None,
+        commands:          Optional[Commands]       = None,
+        allow_parent:      bool                     = False,
+        authors:           Optional[List[str]]      = None,
+        email:             Optional[str]            = None,
+        copyright:         Optional[str]            = None,
+        writer:            TextIO                   = sys.stdout,
+        err_writer:        TextIO                   = sys.stderr,
+        help_app_template: Optional[str]            = None,
+        help_cmd_template: Optional[str]            = None,
+        before:            OptAction                = None,
+        action:            OptAction                = None,
+        after:             OptAction                = None,
+        on_usage_error:    Optional[UsageErrorFunc] = None,
+        exit_with_error:   Optional[ExitErrorFunc]  = None,
+        not_found_error:   Optional[NotFoundFunc]   = None,
     ):
-        """make modifications to inputs after init"""
-        super().__post_init__(before, action, after)
-        self.on_usage_error  = on_usage_error or self.on_usage_error
-        self.exit_with_error = exit_with_error or self.exit_with_error
-        self.not_found_error = not_found_error or self.not_found_error
-        # add help command/flag to system
+        super().__init__(
+            name=name,
+            usage=usage,
+            argsusage=argsusage,
+            flags=flags,
+            commands=commands,
+            allow_parent=allow_parent,
+            before=before,
+            action=action,
+            after=after,
+        )
+        self.version           = version
+        self.description       = description
+        self.authors           = authors or []
+        self.email             = email
+        self.copyright         = copyright
+        self.writer            = writer
+        self.err_writer        = err_writer
+        self.help_app_template = help_app_template
+        self.help_cmd_template = help_cmd_template
+        setattr(self, 'on_usage_error',  on_usage_error or self.on_usage_error)
+        setattr(self, 'exit_with_error', exit_with_error or self.exit_with_error)
+        setattr(self, 'not_found_error', not_found_error or self.not_found_error)
         self.flags.insert(0, help_flag)
         self.commands.insert(0, help_command)
 
-    def on_usage_error(ctx: Context, cmd: Command, error: str):
+    def on_usage_error(self, err: UsageError):
         """
         handles usage errors during parsing or from context
 
-        :param ctx: context of command that raised a usage error
-        :param cmd: command that raised a usage error
-        :param err: message of usage error raised
+        :param err: usage-exception contianing details on error
         """
-        print(f'Incorrect Usage: {error}\n', file=ctx.app.err_writer)
-        help_action(ctx, cmd)
+        print(f'Incorrect Usage: {err.message}\n', file=self.err_writer)
+        help_action(err.context, err.command)
         raise SystemExit(EX_USAGE)
 
-    def exit_with_error(ctx: Context, cmd: Command, err: str, code: int):
+    def exit_with_error(self, err: ExitError):
         """
         handles unrecoverable exceptions that must lead to complete exit
 
-        :param ctx:  context of command that raised an exit error
-        :param cmd:  command that raised an exit error
-        :param err:  message of exit error
-        :param code: exit-code of exit error
+        :param err: exit-exception contianing details on error
         """
-        print(f"App-Error: {err}", file=ctx.app.err_writer)
-        raise SystemExit(code)
+        print(f"App-Error: {err}", file=self.err_writer)
+        raise SystemExit(err.code)
 
-    def not_found_error(ctx: Context, cmd: Command, arg: str):
+    def not_found_error(self, err: NotFoundError):
         """
         handles issues with invalid flags and bad command paths on help
 
-        :param ctx: context of command that raised a not-found error
-        :param cmd: command that raised a not found error
-        :param arg: argument that was not found
-        """
-        if arg.startswith('-'):
-            msg = f'Command: {cmd.name}, Invalid Flag: {arg}'
-        else:
-            msg = f'No Help topic for: {arg}'
-        print(msg, file=ctx.app.err_writer)
+        :param err: not-found-exception contianing details on error
+        """
+        msg = f'No Help topic for: {"->".join(err.path)}'
+        if err.message.startswith('-'):
+            msg = f'Command: {err.command.name}, Invalid Flag: {err.message}'
+        print(msg, file=self.err_writer)
         raise SystemExit(EX_UNAVAILABLE)
+ 
+    def config_error(self, err: ConfigError):
+        """
+        handles issues with app/command configuration errors
 
-    def run(self, 
-        args:      Optional[List[str]] = None,
-        run_async: Optional[bool]      = None,
-    ) -> Optional[Coroutine[None, None, None]]:
+        :param err: config-exception containing details on error
+        """
+        print(f'ConfigError: {err.message}', file=self.err_writer)
+        raise SystemExit(EX_CONFIG)
+
+    def run(self, args: OptStrList = None, run_async: bool = False) -> OptCoroutine:
         """
         run the relevant actions based on the arguments given and app defintions
 
         :param args:      args being parsed and passed into relevant actions
         :param run_async: override app run_async setting
         :return:          asyncio coroutine if run_async=True
         """
         args   = args if args is not None else sys.argv.copy()
         future = run_app(self, args)
-        rasync = run_async if run_async is not None else self.run_async
-        if rasync:
+        if run_async:
             return future
         # generate new loop and ensure closure reguardless of error
+        loop = get_event_loop()
         try:
-            loop = get_event_loop()
             loop.run_until_complete(future)
         finally:
             loop.close()
-
```

### Comparing `cli3-1.0.2/cli/argument.py` & `cli3-1.1.0/cli/argument.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 argument parsers and implementations for special types
 """
 import os
 import re
 from typing import *
 from datetime import timedelta
 
+from .abc import Context, CliError
+
 #** Variables **#
 __all__ = [
     'TypeFunc',
     'ArgumentError',
 
     'parse_bool',
     'parse_decimal',
@@ -33,16 +35,20 @@
 )
 
 #: type defintion for typehint translation for cli
 TypeFunc = Callable[[str], Any]
 
 #** Exceptions **#
 
-class ArgumentError(ValueError):
-    pass
+class ArgumentError(CliError):
+    def __init__(self, msg: str):
+        self.message = msg
+
+    def __str__(self) -> str:
+        return self.message
 
 #** Functions **#
 
 def parse_bool(boolean: str) -> bool:
     """
     parse boolean string into bool value
 
@@ -67,16 +73,19 @@
 def parse_duration(duration: str) -> timedelta:
     """
     parse duration string into timedelta value
 
     :param duration: duration string
     :return:         parsed timedelta value
     """
-    match  = re_duration.match(duration).groupdict()
-    kwargs = {k:int(v.strip('wdhms') if v else 0) for k,v in match.items()}
+    match = re_duration.match(duration)
+    if match is None:
+        raise ArgumentError(f'Invalid Duration: {duration!r}')
+    groups = match.groupdict()
+    kwargs = {k:int(v.strip('wdhms') if v else 0) for k,v in groups.items()}
     return timedelta(**kwargs)
 
 def parse_new_file(file: str) -> str:
     """
     retrieve new filepath for a not yet existing file
 
     :param file: filepath of new file
@@ -111,23 +120,24 @@
     """
     generate before action function to validate the number of arguments
 
     :param min: minimum number of arguments
     :param max: maximum number of arguments
     :return:    function used to regulate argument numbers
     """
-    def validate_range_args(ctx: 'Context'):
+    def validate_range_args(ctx: Context):
+        cmd = ctx.command.name
         if min < 0 and len(ctx.args) > 0:
-            ctx.on_usage_error('action does not take any arguments')
+            ctx.on_usage_error(f'{cmd!r} does not take any arguments')
         if min > 0 and min == max and len(ctx.args) != min:
-            ctx.on_usage_error(f'action must have exactly {min} arguments')
+            ctx.on_usage_error(f'{cmd!r} must have exactly {min} arguments')
         if min > 0 and len(ctx.args) < min:
-            ctx.on_usage_error(f'action must have at least {min} arguments')
+            ctx.on_usage_error(f'{cmd!r} must have at least {min} arguments')
         if max and len(ctx.args) > max:
-            ctx.on_usage_error(f'action can have at maximum {max} arguments')
+            ctx.on_usage_error(f'{cmd!r} can have at maximum {max} arguments')
     return validate_range_args
 
 def exact_args(num: int) -> Callable:
     """
     generate before action function to validate the exact of arguments
 
     :param num: number of allowed arguments
```

### Comparing `cli3-1.0.2/cli/command.py` & `cli3-1.1.0/cli/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,103 @@
 """
 single command defintions used as part of application definition
 """
 import asyncio
 import functools
-from typing import *
-from dataclasses import dataclass, field, InitVar
+from typing import Dict, Optional, List, Callable, Union, cast, overload
 
-from .flag import Flags
-from .context import NO_ACTION, Context, ConfigError
+from .abc import *
 
 #** Variables **#
-__all__ = [
-    'Action',
-    'Commands',
-    'CommandBase',
-    'Command'
-]
-
-#: defintion for any action called in commands
-Action = Callable[[Context], None]
-
-#: defintion for list of commands
-Commands = List['Command']
+__all__ = ['Command']
 
 #** Functions **#
 
 #TODO: run sync cli things in event executor?
 
-def wrap_async(func: Callable) -> Callable:
+def wrap_async(func: Action) -> AsyncAction:
     """ensure actions are run async"""
     if not asyncio.iscoroutinefunction(func):
+        func = cast(SyncAction, func)
         @functools.wraps(func)
         async def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
         return wrapper
     return func
 
-def get_action(obj: object, name: str, func: Optional[Callable]) -> Callable:
+def get_action(obj: object, name: str, func: OptAction) -> AsyncAction:
     """ensure action assignment is not pulled from command-base default"""
-    if not func or func is getattr(CommandBase, name):
+    if func is None:
         func = getattr(obj, f'run_{name}')
-        return wrap_async(func)
-    return wrap_async(func)
+    if isinstance(func, Action):
+        return wrap_async(cast(Action, func))
+    raise RuntimeError(f'Invalid Action {name!r} {func!r}')
 
 #** Classes **#
 
-class CommandBase:
-    """baseclass for command handling and attribute retrieval"""
-    flags:    Flags
-    commands: Commands
-
-    def __post_init__(self, before: Action, action: Action, after: Action):
-        """value validation to ensure correctness"""
-        self.run_before = get_action(self, 'before', before)
-        self.run_action = get_action(self, 'action', action)
-        self.run_after  = get_action(self, 'after',  after)
+class Command(AbsCommand):
+    """
+    Controls Specifications and Behavior of a CLI Command
+
+    :param name:         name of command
+    :param aliases:      name aliases for command
+    :param usage:        usage description 
+    :param argsusage:    argument usage description
+    :param category:     assigned command category
+    :param hidden:       hide command in help if true
+    :param flags:        configured command flags
+    :param commands:     configured subcommands of command
+    :param allow_parent: allow parent to run on child command run
+    :param before:       command before-action function
+    :param action:       command action function
+    :param after:        command after-action function
+    """
+
+    def __init__(self,
+        name:         str,
+        aliases:      Optional[List[str]] = None,
+        usage:        Optional[str]       = None,
+        argsusage:    Optional[str]       = None,
+        category:     Optional[str]       = None,
+        hidden:       bool                = False,
+        flags:        Optional[Flags]     = None,
+        commands:     Optional[Commands]  = None,
+        allow_parent: bool                = False,
+        before:       OptAction           = None,
+        action:       OptAction           = None,
+        after:        OptAction           = None,
+    ):
+        self.name         = name
+        self.aliases      = aliases or []
+        self.usage        = usage
+        self.argsuage     = argsusage
+        self.category     = category or '*'
+        self.hidden       = hidden
+        self.flags        = flags or []
+        self.commands     = commands or []
+        self.allow_parent = allow_parent
+        #NOTE: using setattr to keep mypy from bitching about a func override
+        # related-issue: (https://github.com/python/mypy/issues/2427)
+        setattr(self, 'run_before', wrap_async(before or self.run_before))
+        setattr(self, 'run_action', wrap_async(action or self.run_action))
+        setattr(self, 'run_after',  wrap_async(after or self.run_after))
+ 
+    def __repr__(self) -> str:
+        return f'Command(name={self.name}, aliases={self.aliases!r})'
 
     @property
     def categories(self) -> Dict[str, 'Command']:
         """
-        organize commands into categories
+        organize sub-commands into categories
+
+        :return: dictionary of category names associated w/ sub-commands
         """
         categories = {}
         for cmd in self.commands:
-            if cmd.category not in categories:
-                categories[cmd.category] = []
+            categories.setdefault(cmd.category, [])
             categories[cmd.category].append(cmd)
         return categories
 
     def visible_flags(self) -> Flags:
         """
         retrieve visable flags
 
@@ -90,158 +119,80 @@
 
     def visible_categories(self) -> List[str]:
         """
         retrieve category names
         """
         return [category for category in self.categories.keys()]
 
-    async def run_before(self, ctx: Context):
-        """default before command function"""
+    async def run_before(self, _: Context):
+        """default before-action function when executing command"""
         pass
 
-    async def run_action(self, ctx: Context):
-        """default action command function"""
-        return NO_ACTION
-
-    async def run_after(self, ctx: Context):
-        """default after command function"""
+    async def run_after(self, _: Context):
+        """default after-action function when executing command"""
         pass
 
-    def before(self, func: Callable) -> Action:
+    async def run_action(self, _: Context) -> Result:
+        """default action function when executing command"""
+        return NO_ACTION
+
+    def before(self, func: Action) -> AsyncAction:
         """
         decorate the specified function and assign to command `before` action
 
         :param func: function being assigned to before function
         :return:     wrapped before function
         """
-        self.run_before = wrap_async(func)
+        setattr(self, 'run_before', wrap_async(func))
         return self.run_before
 
-    def action(self, func: Callable) -> Action:
+    def action(self, func: Action) -> AsyncAction:
         """
         decorate the specified function and assign to command action
 
         :param func: function being assigned to action function
         :return:     wrapped action function
         """
         from . import wraps
         # preserve original flags
         if not hasattr(self, 'original_flags'):
             self.original_flags = self.flags
         # generate new action
-        action = wraps.action(func)
+        action, ctx = wraps.action(func)
         # save changes to command
-        self.flags      = [*self.original_flags, *action.flags]
-        self.run_action = action
+        self.flags = [*self.original_flags, *ctx.flags]
+        setattr(self, 'run_action', action)
         return self.run_action
 
-    def after(self, func: Callable) -> Action:
+    def after(self, func: Action) -> AsyncAction:
         """
         decorate the specified function and assign to command `after` action
 
         :param func: function being assigned to after function
         :return:     wrapped after function
         """
-        self.run_after = wrap_async(func)
+        setattr(self, 'run_after', wrap_async(func))
         return self.run_after
 
-    def command(self, *args: Any, **kwargs: Any) -> 'Command':
+    @overload
+    def command(self, func: Callable) -> AbsCommand:
+        ...
+    
+    @overload
+    def command(self, *args, **kwargs) -> CommandFunc:
+        ...
+
+    def command(self, *args, **kwargs) -> Union[AbsCommand, CommandFunc]:
         """
         add the specified function as a subcommand to the current parent
 
         :param args:   positional arguments to pass to command wrapping
         :param kwargs: keyword arguments to pass to command wrapping
         :return:       newly wrapped command object attached to parent
         """
         from . import wraps
         # allow decorator to act as normal wrapper without any args
         if not kwargs and len(args) == 1 and callable(args[0]):
             decorator = wraps.command(self)
             return decorator(args[0])
         # otherwise call decorator as normal
         return wraps.command(self, *args, **kwargs)
-
-    def validate(self):
-        """
-        validate command settings before being run
-        """
-        # ensure flag-names dont overlap
-        for n, flag in enumerate(self.flags[::-1], 1):
-            for other in self.flags[:-n]:
-                for name in flag.names:
-                    if name in other.names:
-                        raise ConfigError(
-                            f'command {self.name!r} > '
-                            f'flag {flag.name!r} name overlaps {other.name!r}')
-        # ensure command-names don't overlap
-        for n, cmd in enumerate(self.commands[::-1], 1):
-            for other in self.commands[:-n]:
-                if cmd.name == other.name:
-                    raise ConfigError(
-                        f'command {self.name!r} > '
-                        f'subcmd {cmd.name!r} name overlaps: {other.name!r}')
-                for alias in cmd.aliases:
-                    if alias == other.name or alias in other.aliases:
-                        raise ConfigError(
-                            f'cmd {self.name!r} > subcmd {cmd.name!r} '
-                            f'alias {alias!r} overlaps: {other.name!r}')
-        # validate subcommands as well
-        for cmd in self.commands:
-            cmd.validate()
-
-@dataclass
-class Command(CommandBase):
-    """
-    controls specifications and behavior of a cli command
-    
-    :param name:         name of command
-    :param aliases:      name aliases for command
-    :param usage:        usage description 
-    :param argsusage:    argument usage description
-    :param category:     assigned command category
-    :param hidden:       hide command in help if true
-    :param flags:        configured command flags
-    :param commands:     configured subcommands of command
-    :param allow_parent: allow parent to run on child command run
-    :param before:       command before-action function
-    :param action:       command action function
-    :param after:        command after-action function
-    """
-
-    name:         str
-    aliases:      List[str]     = field(default_factory=list)
-    usage:        Optional[str] = None
-    argsusage:    Optional[str] = None
-    category:     str           = '*'
-    hidden:       bool          = False
-    flags:        Flags         = field(default_factory=list, repr=False)
-    commands:     Commands      = field(default_factory=list, repr=False)
-    allow_parent: bool          = False
-
-    before: InitVar[Action]
-    action: InitVar[Action]
-    after:  InitVar[Action]
-
-    def to_string(self):
-        """convert command names/alises to string for help formatting"""
-        return ', '.join([self.name, *self.aliases])
-
-    def has_name(self, name: str) -> bool:
-        """
-        return true if command has the given name
-
-        :param name: name being compared to command
-        :return:     true if any names/aliases match
-        """
-        return name == self.name or name in self.aliases
-
-    def index(self, values: List[str]) -> int:
-        """
-        return earliest index of where a command name/alias was found
-
-        :param values: list of strings to be searched
-        :return:       index-num (if found); -1 (if missing)
-        """
-        for n, value in enumerate(values, 0):
-            if value == self.name or value in self.aliases:
-                return n
-        return -1
```

### Comparing `cli3-1.0.2/cli/flag.py` & `cli3-1.1.0/cli/flag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,158 @@
 """
 all possible flags allowed to be passed into application and parsed from args
 """
-from datetime import timedelta
 from contextlib import contextmanager
-from dataclasses import dataclass
-from typing import List, Optional, Any, Union
+from datetime import timedelta
+from dataclasses import dataclass, field
+from typing import Optional, Any, Union, Type, List, ClassVar
 
+from .abc import *
 from .argument import *
 
 #** Variables **#
 __all__ = [
-    'Flags',
-
     'Flag',
-
     'BoolFlag',
     'IntFlag',
     'StringFlag',
     'FloatFlag',
     'DecimalFlag',
     'ListFlag',
     'DurationFlag',
     'EnumFlag',
     'FilePathFlag',
 ]
 
-#: defintion for list of flags
-Flags = List['Flag']
-
 #** Functions **#
 
 @contextmanager
 def capture_errors():
     """simple context-manager to capture any conversion errors"""
     try:
         yield None
     except Exception:
         pass
 
 #** Classes **#
 
+#TODO: move flag validation to app setup and execution
+
 @dataclass
-class Flag:
+class Flag(AbsFlag[T]):
     """
     baseclass Flag declaration
     
     :param name:      name of flag
     :param usage:     usage description
     :param default:   default value
     :param hidden:    hide flag in help if true
     :param required:  ensure flag has value before allowing action
     :param type:      supported type for flag
     :param has_value: internal tracker if flag does not have a value
     """
-
     name:      str
-    usage:     Optional[str] = None
-    default:   Any           = None
-    hidden:    bool          = False
-    required:  bool          = False
-    type:      Any           = str
-    has_value: bool          = True
+    type:      Type[T]
+    usage:     Optional[str]      = field(default=None,  kw_only=True)
+    default:   Any                = field(default=None,  kw_only=True)
+    hidden:    bool               = field(default=False, kw_only=True)
+    required:  bool               = field(default=False, kw_only=True)
+    has_value: bool               = field(default=True,  kw_only=True)
+    parser:    Optional[TypeFunc] = field(default=None,  kw_only=True) #type: ignore
 
     def __post_init__(self):
-        """ensure all flag settings are validated or raise error"""
-        if self.default is not None and isinstance(self.type, type):
-            if not isinstance(self.default, self.type):
-                raise ValueError('default=%r not type=%s' % (
-                    self.default, self.type.__name__))
-
-    def to_string(self) -> str:
-        """convert flag names to string for help formatting"""
-        return self.name
-
-    @property
-    def names(self) -> List[str]:
-        """retrieve list of possible flag names"""
-        return self.name.split(', ', 1)
-
-    def index(self, values: List[str]) -> int:
-        """
-        return index of flag in values if found
-
-        :param values: list of values to search
-        :return:       index-num (if found); -1 (if missing)
-        """
-        names = self.names
-        for n, value in enumerate(values, 0):
-            if value.lstrip('-') in names and value.startswith('-'):
-                return n
-        return -1
+        self.parser: TypeFunc = self.parser or self.type
 
-    def convert(self, value: str) -> Any:
+    def parse(self, value: str) -> T:
         """convert cli-value into the correct-type"""
         with capture_errors():
-            return self.type(value)
+            return self.parser(value)
 
 @dataclass
-class BoolFlag(Flag):
+class BoolFlag(Flag[bool]):
     """implementation for supporting boolean flags"""
-    type:      Any  = bool
-    default:   Any  = False
-    has_value: bool = False
+    type:      ClassVar[Type] = bool
+    default:   bool           = False
+    has_value: bool           = False
 
 @dataclass
-class IntFlag(Flag):
+class IntFlag(Flag[int]):
     """implementation for supporting integer flags"""
-    type: Any = int
+    type: ClassVar[Type] = int
 
 @dataclass
-class StringFlag(Flag):
+class StringFlag(Flag[str]):
     """implementation for supporting string flags"""
-    type: Any = str
+    type: ClassVar[Type] = str
 
 @dataclass
-class FloatFlag(Flag):
+class FloatFlag(Flag[float]):
     """implementation for supporting flag flags"""
-    type: Any = float
+    type: ClassVar[Type] = float
 
 @dataclass
-class DecimalFlag(Flag):
+class DecimalFlag(Flag[float]):
     """
     implementation for supporting controlable decimal flags
 
     :param decimal: number of allowed decimal places
     """
-    type:    Any = float
-    decimal: int = 2
+    type:    ClassVar[Type] = float
+    decimal: int            = 2
 
-    def convert(self, value: str) -> Optional[float]:
+    def parse(self, value: str):
         """handle float founding based on decimal setting"""
         with capture_errors():
-            return parse_decimal(value)
+            return parse_decimal(value, self.decimal)
 
 @dataclass
-class ListFlag(Flag):
+class ListFlag(Flag[List[str]]):
     """implementatin for supporting list flags"""
-    type: Any = list
+    type: ClassVar[Type] = list
 
-    def convert(self, value: str) -> Optional[list]:
+    def parse(self, value: str):
         """convert value into list object"""
         with capture_errors():
             return [c.strip() for c in value.split(',')]
 
 @dataclass
-class DurationFlag(Flag):
+class DurationFlag(Flag[timedelta]):
     """implementation for supporting time-duration flags"""
-    type: Any = timedelta
+    type: ClassVar[Type] = timedelta
 
-    def convert(self, value: str) -> Optional[timedelta]:
+    def parse(self, value: str):
         """convert string-value into timedelta"""
         with capture_errors():
             return parse_duration(value)
 
 @dataclass
-class EnumFlag:
+class EnumFlag(Flag[Any]):
     """
     implementation for supporting enum-value flags
 
     :param enum: enumeration allowed of allowed values in flag
     """
+    type: ClassVar[Type] = Any
     enum: Union[set, dict]
-    type: Any = str
-
-    def convert(self, value: str) -> Optional[str]:
+    
+    def parse(self, value: str) -> Optional[Any]:
         """ensure the specified value is included in the enum"""
         with capture_errors():
             if value not in self.enum:
                 return
             return self.enum[value] if isinstance(self.enum, dict) else value
 
 @dataclass
-class FilePathFlag(Flag):
+class FilePathFlag(Flag[str]):
     """
     implementation for supporting existing/new file-paths
 
     :param exists: ensure file exists if true
     """
-    type:   Any  = str
-    exists: bool = True
+    type:   ClassVar[Type] = str
+    exists: bool           = True
 
-    def convert(self, value: str) -> str:
+    def parse(self, value: str) -> str:
         """ensure filepath exists or doesn't exist based on `exists` setting"""
         if self.exists:
             return parse_existing_file(value)
         return parse_new_file(value)
```

### Comparing `cli3-1.0.2/cli/help.py` & `cli3-1.1.0/cli/help.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 all functions and definitons used to render help page
 """
 from typing import Any, List, Optional
 
 from jinja2 import Environment
 
+from .abc import Context, AbsCommand
 from .flag import BoolFlag
-from .context import Context
-from .command import CommandBase, Command
+from .command import Command
 
 #** Variables **#
 __all__ = [
     'help_app_template',
     'help_cmd_template',
 
     'help_action',
@@ -58,26 +58,26 @@
         {%- if active_category %}
 
     {{ category }}:
         {%- endif %}
         {%- for cmd in visible_commands %}
             {%- if cmd.category == category %}
     {% if active_category %}    {% endif -%}
-    {{ cmd.to_string()|buffer(cbuffer) }} - {{ cmd.usage or default_usage }}
+    {{ cmd.display|buffer(cbuffer) }} - {{ cmd.usage or default_usage }}
             {%- endif %}
         {%- endfor %}
     {%- endfor %}
 {%- endif %}
 
 {%- if visible_flags %}
 
 GLOBAL OPTIONS:
 {%- set fbuffer = calc_buffer(visible_flags) %}
 {%- for flag in visible_flags %}
-    {{ flag.to_string()|buffer(fbuffer) }} - {{ flag.usage or default_usage }}
+    {{ flag.display|buffer(fbuffer) }} - {{ flag.usage or default_usage }}
 {%- endfor %}
 {%- endif %}
 
 {%- if copyright %}
 
 COPYRIGHT:
     {{ copyright }}
@@ -103,26 +103,26 @@
         {%- if active_category %}
 
     {{ category }}:
         {%- endif %}
         {%- for cmd in visible_commands %}
             {%- if cmd.category == category %}
     {% if active_category %}    {% endif -%}
-    {{ cmd.to_string()|buffer(cbuffer) }} - {{ cmd.usage or default_usage }}
+    {{ cmd.display|buffer(cbuffer) }} - {{ cmd.usage or default_usage }}
             {%- endif %}
         {%- endfor %}
     {%- endfor %}
 {%- endif %}
 
 {%- if visible_flags %}
 
 GLOBAL OPTIONS:
 {%- set fbuffer = calc_buffer(visible_flags) %}
 {%- for flag in visible_flags %}
-    {{ flag.to_string()|buffer(fbuffer) }} - {{ flag.usage or default_usage }}
+    {{ flag.display|buffer(fbuffer) }} - {{ flag.usage or default_usage }}
 {%- endfor %}
 {%- endif %}
 """
 
 #: jinja2 template environment object
 env = Environment()
 
@@ -132,41 +132,41 @@
     """add buffer to end of string based on length of value"""
     return value + ' '*(buffer-len(value))
 
 def jinja_calc_buffer(fields: List[Any], category: Optional[str] = None) -> int:
     """calculate buffer for list of fields based on their length"""
     if category:
         fields = [f for f in fields if f.category == category]
-    return max(len(f.to_string()) for f in fields)
+    return max(len(f.display) for f in fields)
 
-def get_vars(cmd: CommandBase) -> dict:
+def get_vars(cmd: AbsCommand) -> dict:
     """collect variables to use for template generation"""
     kwargs = vars(cmd).copy()
     kwargs.update({
         'visible_flags':      cmd.visible_flags(),
         'visible_commands':   cmd.visible_commands(),
         'visible_categories': cmd.visible_categories(),
     })
     return kwargs
 
-def help_action(ctx: Context, command: Optional[Command] = None):
+def help_action(ctx: Context, command: Optional[AbsCommand] = None):
     """action used to render help content"""
     # recurse arguments to find sub-command
     cmd = command or ctx.app
     if ctx.args.present():
-        path = 'app'
+        path = [ctx.app.name]
         for arg in ctx.args:
             for c in cmd.commands:
                 if c.has_name(arg):
-                    path += '->' + c.name
+                    path.append(c.name)
                     cmd   = c
                     break
             else:
                 if command is None:
-                    ctx.app.not_found_error(ctx, cmd, path+'->'+arg)
+                    ctx.not_found_error('invalid command', path)
     # set template based on given command
     template = ctx.app.help_app_template or help_app_template
     if cmd != ctx.app:
         template = ctx.app.help_cmd_template or help_cmd_template
     # get arguments from command and render template
     kwargs    = get_vars(cmd)
     jtemplate = env.from_string(template.strip())
```

### Comparing `cli3-1.0.2/cli/parser.py` & `cli3-1.1.0/cli/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,203 @@
 """
 argument parsing logic and handling to run application as defined
 """
-from typing import List, Tuple, Optional
+from typing import List, Optional, NamedTuple
 
-from .flag import Flags
-from .context import *
-from .command import CommandBase, Command
+from .abc import *
 from .help import help_flag, help_action
 
 #** Variables **#
 __all__ = [
+    'validate_cmd',
+    'exec_app',
     'run_app',
 
     'EX_USAGE',
     'EX_UNAVAILABLE',
     'EX_CONFIG'
 ]
 
 # exit codes stolen from sysexists.h (/usr/include/sysexits.h)
 EX_USAGE       = 64  #- command line usage error -#
 EX_UNAVAILABLE = 69  #- service unavailable -#
 EX_CONFIG      = 78  #- configuration error -#
 
+class SplitArgs(NamedTuple):
+    next:      Optional[AbsCommand]
+    collected: List[str]
+    remaining: List[str]
+
 #** Functions **#
 
-def split_arguments(
-    cmd:  CommandBase,
-    args: Args
-) -> Tuple[Optional[Command], Args, Args]:
+def validate_cmd(command: AbsCommand):
+    """
+    validate command object to avoid configuration errors
+
+    :param cmd: command object to validate
+    """
+    # ensure flag-names dont overlap
+    for n in range(len(command.flags)-1, 0, -1):
+        flag = command.flags[n]
+        for other in command.flags[:n]:
+            for name in flag.names:
+                if name in other.names:
+                    raise ConfigError(
+                        f'command {command.name!r} > flag {flag.display!r} '
+                        f'name overlaps {other.display!r}', command)
+    # ensure command-names don't overlap
+    for n in range(len(command.commands)-1, 0, -1):
+        cmd = command.commands[n]
+        for other in command.commands[:n]:
+            if cmd.name == other.name:
+                raise ConfigError(
+                    f'command {command.name!r} > subcmd '
+                    f'{cmd.name!r} name overlaps: {other.name!r}', command)
+            for alias in cmd.aliases:
+                if alias == other.name or alias in other.aliases:
+                    raise ConfigError(
+                        f'cmd {command.name!r} > subcmd {cmd.name!r} '
+                        f'alias {alias!r} overlaps: {other.name!r}', command)
+    # validate subcommands as well
+    for cmd in command.commands:
+        validate_cmd(cmd)
+
+def split_arguments(cmd: AbsCommand, args: List[str]) -> SplitArgs:
     """
     split arguments into current command values and next command arguments
 
     :param cmd:  command being evaluated for currently
     :param args: args to split into related values and non-related values
     :return:     (next-command <if any>, related-values, unrelated-values)
     """
     args.pop(0)
-    indexes = sorted([
-        (c,i)
-        for c,i in ((c,c.index(args)) for c in cmd.commands)
-        if i != -1
-    ], key=lambda x: x[1])
-    next_cmd, idx = indexes[0] if indexes else (None, len(args))
-    return (next_cmd, args[:idx], args[idx:])
+    next:  Optional[AbsCommand] = None
+    index: int = len(args)
+    for command in cmd.commands:
+        idx = command.index(args)
+        if idx is not None and idx <= index:
+            next  = command
+            index = idx
+    return SplitArgs(next, args[:index], args[index:])
 
-def parse_flags(flags: Flags, args: Args) -> FlagDict:
+def parse_flags(
+    flags: Flags, args: List[str], ctx: Context, cmd: AbsCommand) -> FlagDict:
     """
     parse values for flag-values based on flag definitions
 
     :param flags: flags to scan arguments for
     :param args:  all arguments to be parsed for flag-values
     :return:      dictionary of flag-names to flag-values
     """
     # collect indexes or defaults
     (fdict, indexes) = ({}, [])
     for flag in flags:
         index = flag.index(args)
-        # if flag is present
-        if index != -1:
-            # check if flag appears more than once
-            if flag.index(args[index+1:]) != -1:
-                raise UsageError(f'flag: {flag.name} declared more than once')
-            # raise error if indexes overlap or value isnt given
-            if flag.has_value and (len(args) <= index+1 or index+1 in indexes):
-                raise UsageError(f'flag: {flag.name} no value specified')
-            # append index otherwise
-            indexes.append((flag, index))
-        # if flag has default
-        elif flag.default is not None:
-            fdict[flag.names[0]] = flag.default
-        # if flag is required
-        elif flag.required:
-            raise UsageError(f'flag: {flag.name} is required')
+        # if flag is not present
+        if index is None:
+            # if flag has default
+            if flag.default is not None:
+                fdict[flag.long] = flag.default
+            # if flag is required
+            elif flag.required:
+                raise UsageError(f'flag {flag.display!r} is required', ctx, cmd)
+            continue
+        # check if flag appears more than once
+        plusone = index+1
+        if flag.index(args[plusone:]) is not None:
+            raise UsageError(
+                f'flag {flag.display!r} declared more than once', ctx, cmd)
+        # raise error if indexes overlap or value isnt given
+        if flag.has_value and (len(args) <= plusone or plusone in indexes):
+            raise UsageError(
+                f'flag {flag.display!r} no value specified', ctx, cmd)
+        # append index otherwise
+        indexes.append((flag, index))
     # collect values from indexes (from highest to lowest)
     for flag, idx in sorted(indexes, key=lambda x: x[1], reverse=True):
         # attempt to get value, convert, and set in values
         if flag.has_value:
             # attempt to parse value
             raw = args.pop(idx+1)
-            val = flag.convert(raw)
+            val = flag.parse(raw)
             if val is None:
-                raise UsageError(f'flag: {flag.name} decode failure: {raw}')
-            fdict[flag.names[0]] = val
+                raise UsageError(
+                    f'flag {flag.display!r} decode fail: {raw!r}', ctx, cmd)
+            fdict[flag.long] = val
         # if no-value is possible, set to true
         else:
-            fdict[flag.names[0]] = True
+            fdict[flag.long] = True
         args.pop(idx)
     # iterate the arguments for any non-parsed flags
     for arg in args:
         if arg.startswith('-'):
-            raise NotFoundError(arg)
+            raise NotFoundError(arg, [], ctx, cmd)
     # return parsed values
     return fdict
 
 def has_help_flag(gflags: dict) -> bool:
     """
     check if the given global flags contain the help flag
 
     :param gflags: parsed global flags
     :return:       true if `help` flag is found
     """
-    return bool(gflags.get(help_flag.names[0]))
+    return bool(gflags.get(help_flag.long))
 
-async def run_app(app: 'App', args: List[str]):
+async def exec_app(app: AbsApplication, args: List[str]):
     """
     iterate args until given commands and correlated flags are executed
 
+    :param app:     application w/ flag/command definitions
+    :param args:    arguments to parse according to app definition
+    """
+    # validate application configuration before executing
+    validate_cmd(app)
+    # run application
+    context: Context    = Context(app, app)
+    command: AbsCommand = app
+    # evaluate and run commands based on cli data
+    next_cmd:     Optional[AbsCommand] = app
+    funcret:      Result               = None
+    global_flags: Optional[FlagDict]   = None
+    help_flag:    bool                 = False
+    while next_cmd is not None:
+        (command, parent) = (next_cmd, context)
+        # split args into next-command args and current args
+        next_cmd, values, args = split_arguments(command, args)
+        # collect flags from values
+        flags = parse_flags(command.flags, values, context, command)
+        # pass content into new context
+        if global_flags is None:
+            global_flags = flags
+        values  = Args(values)
+        context = Context(app, command, parent, global_flags, flags, values)
+        # only run command if no subcommand is present or parent is allowed
+        help_flag = help_flag or has_help_flag(global_flags)
+        if (next_cmd is None and not help_flag) or command.allow_parent:
+            await command.run_before(context)
+            funcret = await command.run_action(context)
+            await command.run_after(context)
+    # raise help if help-flag was given
+    if help_flag:
+        help_action(context, command)
+    # raise help if no action was taken at all
+    elif funcret == NO_ACTION:
+        raise UsageError('no action taken', context, command)
+
+async def run_app(app: AbsApplication, args: List[str]):
+    """
+    wrap app execution/iteration w/ standard application error-handlers
+
     :param app:  application w/ flag/command definitions
     :param args: arguments to parse according to app definition
     """
     try:
-        # validate application configuration before executing
-        app.validate()
-        # evaluate and run commands based on cli data
-        (next_cmd, ctx, ret, gflags) = (app, Context(app, app), None, None)
-        while next_cmd is not None:
-            (cmd, parent) = (next_cmd, ctx)
-            # split args into next-command args and current args
-            next_cmd, values, args = split_arguments(cmd, args)
-            # collect flags from values
-            flags = parse_flags(cmd.flags, values)
-            # pass content into new context
-            if gflags is None:
-                gflags = flags
-            ctx = Context(app, cmd, parent, gflags, flags, Args(values))
-            # only run command if no subcommand is present or parent is allowed
-            if (next_cmd is None and not has_help_flag(gflags)) or cmd.allow_parent:
-                await cmd.run_before(ctx)
-                ret = await cmd.run_action(ctx)
-                await cmd.run_after(ctx)
-        # raise help if help-flag was given
-        if has_help_flag(gflags):
-            help_action(ctx, cmd)
-        # raise help if no action was taken at all
-        elif ret == NO_ACTION:
-            raise UsageError('no action taken')
+        await exec_app(app, args) 
     except UsageError as e:
-        app.on_usage_error(ctx, cmd, str(e))
+        app.on_usage_error(e)
     except ExitError as e:
-        app.exit_with_error(ctx, cmd, e.args[0], e.args[1])
+        app.exit_with_error(e)
     except NotFoundError as e:
-        app.not_found_error(ctx, cmd, str(e))
+        app.not_found_error(e)
     except ConfigError as e:
-        print(f'ConfigError: {e}', file=app.err_writer)
-        raise SystemExit(EX_CONFIG)
+        app.config_error(e)
```

### Comparing `cli3-1.0.2/cli/tests/app/v1.py` & `cli3-1.1.0/cli/tests/content/v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """
 V1 API Application Implementation
 """
 import logging
 
-from ... import (
-    range_args,
-    exact_args,
-    App, Command, 
-    StringFlag, IntFlag, BoolFlag, FilePathFlag,
-)
+from ... import * 
 
 #** Variables **#
 __all__ = ['v1']
 
 #** App **#
 
 v1 = App(
@@ -36,16 +31,18 @@
         )
     ],
     commands=[
         Command(
             name='echo',
             usage='repeat something back to user',
             argsusage='<message...>',
+            before=exact_args(1),
+            action=lambda ctx: print(ctx.args.get(0), file=ctx.app.writer),
             flags=[
-                StringFlag(
+                BoolFlag(
                     name='dry, d',
                     usage='run dry run',
                 ),
                 FilePathFlag(
                     name='file, f',
                     usage='file to echo content to'
                 )
```

### Comparing `cli3-1.0.2/cli/tests/app/v2.py` & `cli3-1.1.0/cli/tests/content/v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 V2 API Application Implementation
 """
 import logging
+from typing import Optional
 
 from ... import NO_ACTION, Context, app
 
 #** Variables **#
 __all__ = ['v2']
 
 #** App **#
@@ -17,16 +18,16 @@
     
     :param user:  user to run application as
     :param log:   specify loglevel for whole application
     :param debug: same as --log 0
     """
     return NO_ACTION
 
-@v2.command()
-def echo(ctx: Context, message: str, *, dry: bool = False, file: str = None):
+@v2.command
+def echo(ctx: Context, message: str, *, dry: bool = False, file: Optional[str] = None):
     """
     repeat something back to the user
 
     :param message: message to echo
     :param dry:     run dry run
     :param file:    file to echo content to
     """
@@ -52,15 +53,15 @@
     print('running', file=ctx.app.writer)
     user    = ctx.get_global('user')
     measure = 'kilometers' if km else 'miles'
     print(f'{user} ran {miles} {measure}', file=ctx.app.writer)
     if ctx.parent.get('kill'):
         print('and dies...', file=ctx.app.writer)
 
-@docmd.command()
+@docmd.command
 def fly(ctx: Context, miles: int, miles2: int = 0, *, km: bool = False):
     """
     fly x number of miles
     
     :param miles:  number of miles to run
     :param miles2: number of miles to add to miles
     :param km:     use kilometers rather than miles
```

### Comparing `cli3-1.0.2/cli/wraps.py` & `cli3-1.1.0/cli/wraps.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Function Command Wrapper Utilities
 """
 import inspect
 import functools
 from typing import *
 from datetime import timedelta
 
+from .abc import *
 from .app import App
 from .flag import Flag
-from .context import Context
 from .command import Action, Command, wrap_async
 from .argument import *
 
 #** Variables **#
 __all__ = [
     'Decimal',
     'Duration',
@@ -20,31 +20,43 @@
     'ExistingFile',
 
     'app',
     'action',
     'command',
 ]
 
-null = type(None)
+#: typehint for none-type
+Null = type(None)
 
 # custom typevars for associated translation functions
-Decimal      = TypeVar('Decimal')
-Duration     = TypeVar('Duration')
-NewFile      = TypeVar('NewFile')
-ExistingFile = TypeVar('ExistingFile')
+Decimal      = NewType('Decimal', float)
+Duration     = NewType('Duration', str)
+NewFile      = NewType('NewFile', str)
+ExistingFile = NewType('ExistingFile', str)
+
+class Inspected(NamedTuple):
+    args:      List[str]
+    kwargs:    List[str]
+    defaults:  Dict[str, Any]
+    typehints: Dict[str, Type]
+
+class ActionCtx(NamedTuple):
+    flags:     Flags
+    defaults:  Dict[str, Any]
+    arguments: List[str]
 
 #** Functions **#
 
 def is_union(origin: type) -> bool:
     """
     python3 compatable way of searching for union types
     """
     return 'Union' in str(origin) or 'Union' in type(origin).__name__
 
-def inspectfunc(func: Callable) -> Tuple[list, dict, dict, dict]:
+def inspectfunc(func: Callable) -> Inspected:
     """
     parse and retrieve list of argument names alongside argument typehints
 
     :param func: function being inspected for argument details
     :return:     (list of args, list of kwargs, defaults-dict, typehint-dict)
     """
     sig       = inspect.signature(func)
@@ -52,17 +64,17 @@
     args      = [p.name for p in params if p.kind == p.POSITIONAL_OR_KEYWORD]
     kwargs    = [p.name for p in params if p.kind == p.KEYWORD_ONLY]
     defaults  = {p.name:p.default for p in params if p.default != p.empty}
     typehints = {p.name:p.annotation for p in params if p.annotation != p.empty}
     # determine typehint of arg based on default if not already specified
     for name in (name for name in args if name not in typehints):
         typehints[name] = type(defaults.get(name, ''))
-    return args, kwargs, defaults, typehints
+    return Inspected(args, kwargs, defaults, typehints)
 
-def compile_typehint(attr: str, hint: Any, depth: int = 0) -> TypeFunc:
+def compile_typehint(attr: str, hint: Any, depth: int = 0) -> Optional[TypeFunc]:
     """
     compile the given attribute's typehint into a string-to-type function
 
     :param attr:  attribute name associated w/ typehint
     :param hint:  typehint being compiled into typefunc
     :param depth: recursion depth of function (used for debug)
     :return:      compiled typefunction
@@ -85,39 +97,42 @@
         return parse_new_file
     if hint == ExistingFile:
         return parse_existing_file
     # parse complex typehints
     origin, args = get_origin(hint), get_args(hint)
     if origin in (set, list, tuple):
         func = compile_typehint(attr, args[0], depth+1)
+        if func is None:
+            raise ValueError(f'{attr!r} uses invalid typehint: {args[0]!r}')
         return parse_list_function(func, origin)
     # support `Optional[<hint>]` or `<hint> | None` types
-    if is_union(origin) and len(args) == 2 and args[1] is type(None):
+    if is_union(origin) and len(args) == 2 and args[1] is Null:
         return compile_typehint(attr, args[0], depth=depth+1)
     raise ValueError(f'{attr!r} uses an unsupported typehint: {hint}')
 
 def compile_command_arg_validator(
     names: List[str],
     hints: List[Any],
-    funcs: List[TypeFunc]
-) -> Action:
+    funcs: List[Optional[TypeFunc]]
+) -> Callable[[Context], List[Any]]:
     """
     convert values according to their typefunctions
 
     :param names: argument names associated w/ values
     :param hints: typehints associated with values
     :param funcs: functions used to translate values accordingly
     :return:      command action that parses and saves argument values
     """
     def validate_values(ctx: Context) -> List[Any]:
         values, tracked = [], 0
         for (name, hint, func) in zip(names, hints, funcs):
             # pass context in if hint is for context
-            if hint == Context:
-                values.append(ctx)
+            if func is None:
+                if hint == Context:
+                    values.append(ctx)
                 continue
             # retrieve value from args if exists
             val = ctx.args.get(tracked)
             if val is None:
                 continue
             # attempt convert args as standard
             try:
@@ -133,18 +148,18 @@
         return values
     return validate_values
 
 def compile_command_flags(
     func:     Callable,
     names:    List[str],
     hints:    List[Any],
-    funcs:    List[TypeFunc],
+    funcs:    List[Optional[TypeFunc]],
     defaults: Dict[str, Any],
     is_app:   bool = False
-) -> List[Flag]:
+) -> Flags:
     """
     compile command flags based on given configuration
 
     :param names:    list of parameter names
     :param hints:    list of typehints for parameters
     :param funcs:    parse functions to use in flag object
     :param defaults: default values for associated parameter names
@@ -165,29 +180,32 @@
         tlbl         = any(details[1].startswith(c) for c in '{<[:')
         param, usage = details[2].split(' ', 1) if tlbl else tuple(details[1:])
         # assign param/usage to description table
         descriptions[param.strip(strip)] = usage.strip(strip)
     # generate flags
     flags  = []
     shorts = [] if not is_app else ['h']
-    for name, hint, func in zip(names, hints, funcs):
+    for name, hint, parser in zip(names, hints, funcs):
+        if func is None:
+            continue
         # set shortform if first letter is unique
         fname = name.strip('_')
         short = fname.lower()[0]
         short = short if short not in shorts else ''
         shorts.append(short)
         # generate flag object
         is_bool = hint == bool
         flags.append(Flag(
             name=f'{fname}, {short}' if short else fname,
             usage=descriptions.get(name),
             default=defaults.get(name),
             hidden=name.startswith('_'),
-            type=bool if is_bool else func,
+            type=hint,
             has_value=not is_bool,
+            parser=parser,
         ))
     return flags
 
 def compile_command_usage(action: Action) -> str:
     """
     compile command usage from action docstring
 
@@ -197,121 +215,137 @@
     usage, doc = '', action.__doc__ or ''
     for line in (line.strip() for line in doc.splitlines()):
         if not line or any(line.startswith(c) for c in '@:'):
             continue
         usage += line + ' '
     return usage.strip()
 
-def compile_command_argsusage(action: Action) -> str:
+def compile_command_argsusage(action_ctx: ActionCtx) -> str:
     """
     compile command argsusage from action argument information
 
     :param action: action function being evaluated
     :return:              generated command argsusage
     """
     usage = []
-    for arg in action.arguments:
-        if arg in action.defaults:
+    for arg in action_ctx.arguments:
+        if arg in action_ctx.defaults:
             usage.append('[arguments...]')
             break
         usage.append(f'[{arg}]')
     usage.append('[flags...]')
     return ' '.join(usage)
 
-def action(func: Callable, is_app: bool = False) -> Action:
+def action(func: Callable, is_app: bool = False) -> Tuple[AsyncAction, ActionCtx]:
     """
     wrap python function as standard command action
 
     :param func:   function being wrapped and converted into command action
     :param is_app: tweak command and flag generation when building app action
     :return:       generated function command action
     """
     func = wrap_async(func)
-    args, kwargs, dfaults, typehints = inspectfunc(func)
+    spec = inspectfunc(func)
     # generate argument type converters/validators
-    argtypes      = [typehints[name] for name in args]
-    arglist       = [compile_typehint(name, typehints[name]) for name in args]
-    validate_args = compile_command_arg_validator(args, argtypes, arglist)
+    arghints      = [spec.typehints[name] for name in spec.args]
+    arglist       = [compile_typehint(*args) for args in zip(spec.args, arghints)]
+    validate_args = compile_command_arg_validator(spec.args, arghints, arglist)
     # fill out any flag fields w/ their associated data
-    ftypes = [typehints[name] for name in kwargs]
-    flist  = [compile_typehint(name, typehints[name]) for name in kwargs]
-    flags  = compile_command_flags(func, kwargs, ftypes, flist, dfaults, is_app)
+    fhints = [spec.typehints[name] for name in spec.kwargs] 
+    flist  = [compile_typehint(*args) for args in zip(spec.kwargs, fhints)]
+    flags  = compile_command_flags(func, spec.kwargs, fhints, flist, spec.defaults, is_app)
     # generate argument number validator
     max_args        = sum(1 for func in arglist if func is not None)
     arg_diff        = len(arglist) - max_args
     max_args        = len([f for f in arglist if f])
-    min_args        = sum(1 for a in args if a not in dfaults) - arg_diff
+    min_args        = sum(1 for a in spec.args if a not in spec.defaults) - arg_diff
     validate_argnum = range_args(min_args, max_args)
     # complete action translation
     @functools.wraps(func)
     async def action(ctx: Context):
         validate_argnum(ctx)
         args   = validate_args(ctx)
-        names  = [flag.names[0] for flag in flags]
+        names  = [flag.long for flag in flags]
         kwargs = {name:ctx.get(name) for name in names}
         return await func(*args, **kwargs)
-    # export a few variables for command generation
-    action.flags     = flags.copy()
-    action.defaults  = dfaults
-    action.arguments = [arg for n, arg in enumerate(args, 0) if arglist[n]]
     # return generated action function
-    return action
+    arguments = [arg for arg, hint in zip(spec.args, arglist) if hint]
+    return action, ActionCtx(flags.copy(), spec.defaults, arguments)
 
 def command(
-    parent:       Command,
+    parent:       AbsCommand,
     name:         Optional[str]  = None,
     aliases:      Optional[list] = None,
     usage:        Optional[str]  = None,
     argsusage:    Optional[str]  = None,
     category:     str            = '*',
     hidden:       Optional[bool] = None,
     allow_parent: bool           = False
-):
+) -> CommandFunc:
     """
     dynamically generate a cli-command from the decorated function
 
     :param name:         name override for command
     :param aliases:      name aliases assigned to command
     :param usage:        specified command usage description
     :param argsusage:    specified command argsusage description
     :param category:     command category assignment
     :param hidden:       control if command is hidden from help
     :param allow_parent: allow parent to run if subcommand is also run
     :return:             decorator that returns generated command object
     """
     def decorator(func: Callable) -> Command:
-        fname   = func.__name__
-        main    = action(func)
+        fname     = func.__name__
+        main, ctx = action(func)
         command = Command(
             name=name or fname.strip('_'),
             aliases=aliases or [],
             category=category,
             usage=usage or compile_command_usage(main),
-            argsusage=argsusage or compile_command_argsusage(main),
+            argsusage=argsusage or compile_command_argsusage(ctx),
             hidden=fname.startswith('_') if hidden is None else hidden,
             allow_parent=allow_parent,
             action=main,
-            flags=main.flags,
+            flags=ctx.flags,
         )
         parent.commands.append(command)
         return command
     return decorator
 
+@overload
+def app(name_or_func: Callable) -> App:
+    ...
+
+@overload
 def app(
-    name:         Optional[str]  = None,
+    name_or_func: Optional[str]  = None,
     usage:        Optional[str]  = None,
     version:      Optional[str]  = None,
     argsusage:    Optional[str]  = None,
     description:  Optional[str]  = None,
     email:        Optional[str]  = None,
     authors:      Optional[list] = None,
     copyright:    Optional[str]  = None,
     allow_parent: bool           = False,
     **kwargs:     Any,
-) -> App:
+) -> AppFunc:
+    ...
+
+def app(
+    name_or_func: Union[Callable, Optional[str]] = None,
+    usage:        Optional[str]  = None,
+    version:      Optional[str]  = None,
+    argsusage:    Optional[str]  = None,
+    description:  Optional[str]  = None,
+    email:        Optional[str]  = None,
+    authors:      Optional[list] = None,
+    copyright:    Optional[str]  = None,
+    allow_parent: bool           = False,
+    **kwargs:     Any,
+) -> Union[App, AppFunc]:
     """
     dynamically generate a simple cli-application from the decorated function
 
     :param name:         assigned name of application
     :param usage:        specified application usage description
     :param version:      symantic version of application
     :param argsusage:    specified application argsusage description
@@ -319,25 +353,27 @@
     :param email:        primary email associated w/ application
     :param authors:      list of authors associated w/ application
     :param copyright:    copyright linked with application
     :param allow_parent: allow base parent app to run when child command is run
     :param kwargs:       additonal keyword arguments to pass to app definiton
     :return:             decorator that returns generated application object
     """
+    func = name_or_func if callable(name_or_func) else None
+    name = None if callable(name_or_func) else name_or_func
     def decorator(func: Callable) -> App:
-        cname = name or func.__name__.strip('_')
-        main  = action(func, is_app=True)
+        cname     = name or func.__name__.strip('_')
+        main, ctx = action(func, is_app=True)
         return App(
             name=cname,
             usage=usage or compile_command_usage(main),
             version=version or '0.0.1',
-            argsusage=argsusage or compile_command_argsusage(main),
+            argsusage=argsusage or compile_command_argsusage(ctx),
             description=description,
             authors=authors or [],
             email=email,
             copyright=copyright,
             allow_parent=allow_parent,
             action=main,
-            flags=main.flags,
+            flags=ctx.flags,
             **kwargs,
         )
-    return decorator
+    return decorator if func is None else decorator(func)
```

### Comparing `cli3-1.0.2/cli3.egg-info/PKG-INFO` & `cli3-1.1.0/cli3.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.0.2
+Version: 1.1.0
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
-Description: cli
-        ===
-        
-        [![forthebadge](https://forthebadge.com/images/badges/you-didnt-ask-for-this.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
-        
-        A highly configurable, dynamic, fast, and easy solution to managing
-        a command-line application. The goal is to make cli development as simple
-        and effective as possible for any configuration enabling the developer to
-        focus on function over form.
-        
-        Supports Python >= 3.7 and can run asynchronously or synchronously.
-        
-        This library took heavy initial inspiration by [urfave/cli](https://github.com/urfave/cli)
-        so credit to them for their work as well.
-        
-        ## Install
-        
-        ```bash
-        $ pip install cli3
-        ```
-        
-        ## Documentation
-        
-        More documentation is available in [`./docs`](https://github.com/imgurbot12/cli/tree/master/docs) or the hosted
-        documentation site at <https://cli3.readthedocs.org>.
-        
-        ## License
-        
-        See [`LICENSE`](./LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+cli
+===
+
+[![forthebadge](https://forthebadge.com/images/badges/you-didnt-ask-for-this.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
+
+A highly configurable, dynamic, fast, and easy solution to managing
+a command-line application. The goal is to make cli development as simple
+and effective as possible for any configuration enabling the developer to
+focus on function over form.
+
+Supports Python >= 3.7 and can run asynchronously or synchronously.
+
+This library took heavy initial inspiration by [urfave/cli](https://github.com/urfave/cli)
+so credit to them for their work as well.
+
+## Install
+
+```bash
+$ pip install cli3
+```
+
+## Documentation
+
+More documentation is available in [`./docs`](https://github.com/imgurbot12/cli/tree/master/docs) or the hosted
+documentation site at <https://cli3.readthedocs.org>.
+
+## License
+
+See [`LICENSE`](./LICENSE)
```

### Comparing `cli3-1.0.2/setup.py` & `cli3-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='cli3',
-    version='1.0.2',
+    version='1.1.0',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/cli',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description=(
         'A highly configurable, dynamic, fast, and easy '
```

