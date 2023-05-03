# Comparing `tmp/poethepoet-0.8.0.tar.gz` & `tmp/poethepoet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poethepoet-0.8.0.tar", last modified: Wed Sep  2 20:23:22 2020, max compression
+gzip compressed data, was "poethepoet-0.9.0.tar", last modified: Tue Sep 29 21:34:12 2020, max compression
```

## Comparing `poethepoet-0.8.0.tar` & `poethepoet-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
--rw-r--r--   0        0        0     1070 2020-09-02 20:23:16.197889 poethepoet-0.8.0/LICENSE
--rw-r--r--   0        0        0     9371 2020-09-02 20:23:16.197889 poethepoet-0.8.0/README.rst
--rw-r--r--   0        0        0     4138 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/__init__.py
--rw-r--r--   0        0        0       85 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/__main__.py
--rw-r--r--   0        0        0       22 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/__version__.py
--rw-r--r--   0        0        0     2931 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/app.py
--rw-r--r--   0        0        0     5925 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/config.py
--rw-r--r--   0        0        0      366 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/exceptions.py
--rw-r--r--   0        0        0       65 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/executor/__init__.py
--rw-r--r--   0        0        0     1877 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/executor/base.py
--rw-r--r--   0        0        0      809 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/executor/poetry.py
--rw-r--r--   0        0        0      171 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/task/__init__.py
--rw-r--r--   0        0        0    11377 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/task/base.py
--rw-r--r--   0        0        0     1667 2020-09-02 20:23:16.197889 poethepoet-0.8.0/poethepoet/task/cmd.py
--rw-r--r--   0        0        0     1488 2020-09-02 20:23:16.201889 poethepoet-0.8.0/poethepoet/task/ref.py
--rw-r--r--   0        0        0     2670 2020-09-02 20:23:16.201889 poethepoet-0.8.0/poethepoet/task/script.py
--rw-r--r--   0        0        0     2563 2020-09-02 20:23:16.201889 poethepoet-0.8.0/poethepoet/task/sequence.py
--rw-r--r--   0        0        0     2352 2020-09-02 20:23:16.201889 poethepoet-0.8.0/poethepoet/task/shell.py
--rw-r--r--   0        0        0     7353 2020-09-02 20:23:16.201889 poethepoet-0.8.0/poethepoet/ui.py
--rw-r--r--   0        0        0     1588 2020-09-02 20:23:16.201889 poethepoet-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10512 2020-09-02 20:23:22.116302 poethepoet-0.8.0/setup.py
--rw-r--r--   0        0        0    10039 2020-09-02 20:23:22.117033 poethepoet-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-09-29 21:34:03.239265 poethepoet-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9812 2020-09-29 21:34:03.239265 poethepoet-0.9.0/README.rst
+-rw-r--r--   0        0        0     1570 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/__init__.py
+-rw-r--r--   0        0        0       94 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/__main__.py
+-rw-r--r--   0        0        0       22 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/__version__.py
+-rw-r--r--   0        0        0     3232 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/app.py
+-rw-r--r--   0        0        0        0 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/completion/__init__.py
+-rw-r--r--   0        0        0      656 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/completion/bash.py
+-rw-r--r--   0        0        0     1248 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/completion/fish.py
+-rw-r--r--   0        0        0     3048 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/completion/zsh.py
+-rw-r--r--   0        0        0     5925 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/config.py
+-rw-r--r--   0        0        0     1182 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/context.py
+-rw-r--r--   0        0        0      366 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/exceptions.py
+-rw-r--r--   0        0        0       65 2020-09-29 21:34:03.239265 poethepoet-0.9.0/poethepoet/executor/__init__.py
+-rw-r--r--   0        0        0     2018 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/executor/base.py
+-rw-r--r--   0        0        0     4314 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/executor/poetry.py
+-rw-r--r--   0        0        0      171 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/__init__.py
+-rw-r--r--   0        0        0    11230 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/base.py
+-rw-r--r--   0        0        0     1720 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/cmd.py
+-rw-r--r--   0        0        0     1366 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/ref.py
+-rw-r--r--   0        0        0     2656 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/script.py
+-rw-r--r--   0        0        0     2622 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/sequence.py
+-rw-r--r--   0        0        0     2294 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/task/shell.py
+-rw-r--r--   0        0        0     7353 2020-09-29 21:34:03.243265 poethepoet-0.9.0/poethepoet/ui.py
+-rw-r--r--   0        0        0     1596 2020-09-29 21:34:03.243265 poethepoet-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11014 2020-09-29 21:34:12.696087 poethepoet-0.9.0/setup.py
+-rw-r--r--   0        0        0    10480 2020-09-29 21:34:12.697083 poethepoet-0.9.0/PKG-INFO
```

### Comparing `poethepoet-0.8.0/LICENSE` & `poethepoet-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poethepoet-0.8.0/README.rst` & `poethepoet-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,38 @@
+Metadata-Version: 2.1
+Name: poethepoet
+Version: 0.9.0
+Summary: A task runner that works well with poetry.
+Home-page: https://github.com/nat-n/poethepoet
+License: MIT
+Author: Nat Noordanus
+Author-email: n@natn.me
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: pastel (>=0.2.0,<0.3.0)
+Requires-Dist: tomlkit (>=0.6.0,<1.0.0)
+Project-URL: Repository, https://github.com/nat-n/poethepoet
+Description-Content-Type: text/x-rst
+
 ************
 Poe the Poet
 ************
 
 A task runner that works well with poetry.
 
 .. role:: bash(code)
    :language: bash
+.. role:: fish(code)
+   :language: fish
+.. role:: zsh(code)
+   :language: zsh
 
 .. role:: toml(code)
    :language: toml
 
 Features
 ========
 
@@ -23,15 +46,15 @@
 
 ✅  Tasks can specify and reference environment variables as if they were evaluated by a shell
 
 ✅  Tasks are self documenting, with optional help messages (just run poe without arguments)
 
 ✅  Tasks can be defined as a sequence of other tasks
 
-✅  Shell completion of global options and task names (just for zsh so far)
+✅  Shell completion of task names (and global options too for zsh)
 
 Installation
 ============
 
 Into your project (so it works inside poetry shell):
 
 .. code-block:: bash
@@ -40,28 +63,60 @@
 
 And into your default python environment (so it works outside of poetry shell)
 
 .. code-block:: bash
 
   pip install poethepoet
 
-Enable tab completion for zsh
------------------------------
+Enable tab completion for your shell
+------------------------------------
 
-Assuming you have `Oh My Zsh <https://github.com/ohmyzsh/ohmyzsh>`_ installed (or have otherwise enabled completions) you can use poe to generate a zsh completion script to install somewhere in your `$fpath`.
+Poe comes with tab completion scripts for bash, zsh, and fish to save you keystrokes. How to install them will depend on your shell setup.
 
-For example, if you use Oh My Zsh then you can enable tab completion for poe global options and task names just by installing the generated function into the completions dir:
+Zsh
+~~~
 
-.. code-block:: bash
+.. code-block:: zsh
+
+  # oh-my-zsh
+  mkdir -p ~/.oh-my-zsh/completions
+  poe _zsh_completion > ~/.oh-my-zsh/completions/_poe
 
-  mkdir -p $HOME/.oh-my-zsh/completions
-  poe _zsh_completion > $HOME/.oh-my-zsh/completions/_poe
+  # without oh-my-zsh
+  mkdir -p ~/.zfunc/
+  poe _zsh_completion > ~/.zfunc/_poetry
 
 Note that you'll need to start a new shell for the new completion script to be loaded. If it still doesn't work try adding a call to `compinit` to the end of your zshrc file.
 
+Bash
+~~~~
+
+.. code-block:: bash
+
+  # System bash
+  poe _bash_completion > /etc/bash_completion.d/poe.bash-completion
+
+  # Homebrew bash
+  poe _bash_completion > $(brew --prefix)/etc/bash_completion.d/poe.bash-completion
+
+
+How to ensure installed bash completions are enabled may vary depending on your system.
+
+Fish
+~~~~
+
+.. code-block:: fish
+
+  # Fish
+  poe _fish_completion > ~/.config/fish/completions/poe.fish
+
+  # Homebrew fish
+  poe _fish_completion > (brew --prefix)/share/fish/vendor_completions.d/poe.fish
+
+
 Basic Usage
 ===========
 
 Define tasks in your pyproject.toml
 -----------------------------------
 
 `See a real example <https://github.com/nat-n/poethepoet/blob/master/pyproject.toml>`_
@@ -283,27 +338,26 @@
 ============
 
 There's plenty to do, come say hi in the issues! 👋
 
 TODO
 ====
 
-☐ command line completion for bash & fish
-
 ☐ support declaring specific arguments for a task
 
 ☐ support conditional execution (a bit like make targets)
 
 ☐ support verbose mode for documentation that shows task definitions
 
-☐ support running tasks outside of poetry's virtualenv (or in another?)
+☐ support different task executors such as specifying a non-poetry venv, or working with pipenv,
 
-☐ try to work well without poetry too
+☐ support third party task or executor types as plugins
 
-☐ maybe support plumbum based tasks
+☐ maybe provide poe as a poetry plugin
 
-☐ maybe support third party task types as plugins
+☐ maybe support plumbum based tasks
 
 Licence
 =======
 
 MIT.
+
```

### Comparing `poethepoet-0.8.0/poethepoet/__init__.py` & `poethepoet-0.9.0/poethepoet/completion/zsh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,17 @@
-from .__version__ import __version__
+from typing import Any, Iterable, Set
 
 
-def main():
-    import sys
-
-    if len(sys.argv) == 2 and sys.argv[1].startswith("_"):
-        if sys.argv[1] == "_describe_tasks":
-            _describe_tasks()
-            return
-        if sys.argv[1] == "_zsh_completion":
-            _zsh_completion()
-            return
-
-    from pathlib import Path
-    from .app import PoeThePoet
-
-    app = PoeThePoet(cwd=Path(".").resolve(), output=sys.stdout)
-    result = app(cli_args=sys.argv[1:])
-    if result:
-        raise SystemExit(result)
-
-
-def _describe_tasks():
-    """
-    A special task accessible via `poe _describe_tasks` for use in shell completion
-
-    Note this code path should include minimal imports to avoid slowing down the shell
-    """
-
-    try:
-        from .config import PoeConfig
-
-        config = PoeConfig()
-        config.load()
-        task_names = (task for task in config.tasks.keys() if task and task[0] != "_")
-        print(" ".join(task_names))
-    except Exception:  # pylint: disable=broad-except
-        # this happens if there's no pyproject.toml present
-        pass
-
-
-def _zsh_completion():
+def get_zsh_completion_script() -> str:
     """
     A special task accessible via `poe _zsh_completion` that prints a zsh completion
     script for poe generated from the argparses config
     """
     from pathlib import Path
-    from .app import PoeThePoet
+    from ..app import PoeThePoet
 
     # build and interogate the argument parser as the normal cli would
     app = PoeThePoet(cwd=Path(".").resolve())
     parser = app.ui.build_parser()
     global_options = parser._action_groups[1]._group_actions
     excl_groups = [
         set(excl_group._group_actions)
@@ -70,24 +31,24 @@
                 if len(option.option_strings) == 1
                 else '"{' + ",".join(sorted(option.option_strings)) + '}"'
             )
             args_lines.append(f'"(- *){options_part}[{option.help}]"')
             continue
 
         # collect other options that are exclusive to this one
-        excl_options = next(
+        excl_options: Iterable[Any] = next(
             (
                 excl_group - {option}
                 for excl_group in excl_groups
                 if option in excl_group
             ),
             tuple(),
         )
         # collect all option strings that are exclusive with this one
-        excl_option_strings = set(
+        excl_option_strings: Set[str] = set(
             [
                 option_string
                 for excl_option in excl_options
                 for option_string in excl_option.option_strings
             ]
         ) | set(option.option_strings)
 
@@ -106,25 +67,23 @@
             )
 
         args_lines.append(f'"{options_part}[{option.help}]"')
 
     args_lines.append('"1: :($TASKS)"')
     args_lines.append('"*::arg:->args"')
 
-    print(
-        "\n".join(
-            [
-                "#compdef _poe poe\n",
-                "function _poe {",
-                '    local ALL_EXLC=("-h" "--help" "--version")',
-                "    local TASKS=($(poe _describe_tasks))",
-                "",
-                " \\\n        ".join(args_lines),
-                "",
-                # Only offer filesystem based autocompletions after a task is specified
-                "    if (($TASKS[(Ie)$line[1]])); then",
-                "        _files",
-                "    fi",
-                "}",
-            ]
-        )
+    return "\n".join(
+        [
+            "#compdef _poe poe\n",
+            "function _poe {",
+            '    local ALL_EXLC=("-h" "--help" "--version")',
+            "    local TASKS=($(poe _list_tasks))",
+            "",
+            " \\\n        ".join(args_lines),
+            "",
+            # Only offer filesystem based autocompletions after a task is specified
+            "    if (($TASKS[(Ie)$line[1]])); then",
+            "        _files",
+            "    fi",
+            "}",
+        ]
     )
```

### Comparing `poethepoet-0.8.0/poethepoet/app.py` & `poethepoet-0.9.0/poethepoet/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import os
 from pathlib import Path
 import sys
 from typing import Any, IO, MutableMapping, Optional, Sequence, Union
 from .config import PoeConfig
+from .context import RunContext
+from .executor import PoetryExecutor
+from .exceptions import ExecutionError, PoeException
 from .task import PoeTask
 from .ui import PoeUi
-from .exceptions import ExecutionError, PoeException
 
 
 class PoeThePoet:
     cwd: Path
     ui: PoeUi
     config: PoeConfig
     task: Optional[PoeTask] = None
@@ -68,21 +71,26 @@
             )
             return False
 
         self.task = PoeTask.from_config(task_name, config=self.config, ui=self.ui)
         return True
 
     def run_task(self) -> Optional[int]:
-        _, *take_args = self.ui["task"]
+        _, *extra_args = self.ui["task"]
         try:
             assert self.task
             return self.task.run(
-                take_args,
-                project_dir=Path(self.config.project_dir),
-                dry=self.ui["dry_run"],
+                context=RunContext(
+                    project_dir=Path(self.config.project_dir),
+                    executor_cls=PoetryExecutor,
+                    env=os.environ,
+                    dry=self.ui["dry_run"],
+                    poe_active=os.environ.get("POE_ACTIVE"),
+                ),
+                extra_args=extra_args,
             )
         except PoeException as error:
             self.print_help(error=error)
             return 1
         except ExecutionError as error:
             self.ui.print_error(error=error)
             return 1
```

### Comparing `poethepoet-0.8.0/poethepoet/config.py` & `poethepoet-0.9.0/poethepoet/config.py`

 * *Files identical despite different names*

### Comparing `poethepoet-0.8.0/poethepoet/executor/base.py` & `poethepoet-0.9.0/poethepoet/executor/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from subprocess import Popen, PIPE
 import sys
 from typing import Any, MutableMapping, Optional, Sequence, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pathlib import Path
+    from ..context import RunContext
 
 
 class PoeExecutor:
     """
     A base class for poe task executors
     """
 
     working_dir: Optional["Path"]
 
     # TODO: maybe recieve a reference to the PoeConfig
     #   Also maybe invert the control so the executor is given a task to run
 
     def __init__(
         self,
+        context: "RunContext",
         env: MutableMapping[str, str],
         working_dir: Optional["Path"] = None,
         dry: bool = False,
     ):
+        self.context = context
         self.working_dir = working_dir
         self.env = env
         self.dry = dry
 
     def execute(self, cmd: Sequence[str], input: Optional[bytes] = None,) -> int:
         raise NotImplementedError
 
     def _exec_via_subproc(
         self,
         cmd: Sequence[str],
         *,
-        env: Optional[MutableMapping[str, str]] = None,
         input: Optional[bytes] = None,
+        env: Optional[MutableMapping[str, str]] = None,
+        shell: bool = False
     ) -> int:
         if self.dry:
             return 0
-        popen_kwargs: MutableMapping[str, Any] = {}
+        popen_kwargs: MutableMapping[str, Any] = {"shell": shell}
         popen_kwargs["env"] = self.env if env is None else env
         if input is not None:
             popen_kwargs["stdin"] = PIPE
         if self.working_dir is not None:
             popen_kwargs["cwd"] = self.working_dir
 
         # TODO: exclude the subprocess from coverage more gracefully
```

### Comparing `poethepoet-0.8.0/poethepoet/task/base.py` & `poethepoet-0.9.0/poethepoet/task/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-import os
-from pathlib import Path
 import re
 import sys
 from typing import (
     Any,
     Dict,
     Iterable,
     List,
     MutableMapping,
     Optional,
     Tuple,
     Type,
     TYPE_CHECKING,
     Union,
 )
-from ..executor import PoetryExecutor
 from ..exceptions import PoeException
 
 if TYPE_CHECKING:
-    from ..executor import PoeExecutor
+    from ..context import RunContext
     from ..config import PoeConfig
     from ..ui import PoeUi
 
 
 TaskDef = Union[str, Dict[str, Any], List[Union[str, Dict[str, Any]]]]
 
 _TASK_NAME_PATTERN = re.compile(r"^\w[\w\d\-\_\+\:]*$")
@@ -128,57 +125,50 @@
             )
 
         # Something is wrong with this task_def
         raise cls.Error(cls.validate_def(task_name, task_def, config))
 
     def run(
         self,
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: Optional[MutableMapping[str, str]] = None,
-        set_cwd: bool = True,
-        dry: bool = False,
     ) -> int:
         """
         Run this task
         """
-        if env is None:
-            env = dict(os.environ)
-        env["POE_ROOT"] = str(project_dir)
-        env = dict(env, **self._config.global_env)
+        env = dict(env or {}, **self._config.global_env)
         if self.options.get("env"):
             env = dict(env, **self.options["env"])
-        executor = PoetryExecutor(
-            env=env, working_dir=project_dir if set_cwd else None, dry=dry
-        )
-        return self._handle_run(executor, list(extra_args), project_dir, env, dry)
+        return self._handle_run(context, extra_args, env)
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
         """
         _handle_run must be implemented by a subclass and return a single executor result.
         """
         raise NotImplementedError
 
     @staticmethod
-    def _resolve_envvars(content: str, env: MutableMapping[str, str]) -> str:
+    def _resolve_envvars(
+        content: str, context: "RunContext", env: MutableMapping[str, str]
+    ) -> str:
         """
         Template in ${environmental} $variables from env as if we were in a shell
 
         Supports escaping of the $ if preceded by an odd number of backslashes, in which
         case the backslash immediately precending the $ is removed. This is an
         intentionally very limited implementation of escaping semantics for the sake of
         usability.
         """
+        env = context.get_env(env)
         cursor = 0
         resolved_parts = []
         for match in _SHELL_VAR_PATTERN.finditer(content):
             groups = match.groups()
             # the first two groups match escaped varnames so should be ignored
             var_name = groups[2] or groups[3]
             escaped_var_name = groups[0] or groups[1]
@@ -205,67 +195,68 @@
         cls, task_name: str, task_def: TaskDef, config: "PoeConfig"
     ) -> Optional[str]:
         """
         Check the given task name and definition for validity and return a message
         describing the first encountered issue if any.
         If raize is True then the issue is raised as an exception.
         """
-        issue = None
         if not (task_name[0].isalpha() or task_name[0] == "_"):
-            issue = (
+            return (
                 f"Invalid task name: {task_name!r}. Task names must start with a letter"
                 " or underscore."
             )
         elif not _TASK_NAME_PATTERN.match(task_name):
-            issue = (
+            return (
                 f"Invalid task name: {task_name!r}. Task names characters must be "
                 "alphanumeric, colon, underscore or dash."
             )
         elif isinstance(task_def, dict):
             task_type_keys = set(task_def.keys()).intersection(cls.__task_types)
             if len(task_type_keys) == 1:
                 task_type_key = next(iter(task_type_keys))
                 task_content = task_def[task_type_key]
                 task_type = cls.__task_types[task_type_key]
                 if not isinstance(task_content, task_type.__content_type__):
-                    issue = (
+                    return (
                         f"Invalid task: {task_name!r}. {task_type} value must be a "
                         f"{task_type.__content_type__}"
                     )
                 else:
                     for key in set(task_def) - {task_type_key}:
                         expected_type = cls.__base_options.get(
                             key, task_type.__options__.get(key)
                         )
                         if expected_type is None:
-                            issue = (
+                            return (
                                 f"Invalid task: {task_name!r}. Unrecognised option "
                                 f"{key!r} for task of type: {task_type_key}."
                             )
-                            break
                         elif not isinstance(task_def[key], expected_type):
-                            issue = (
+                            return (
                                 f"Invalid task: {task_name!r}. Option {key!r} should "
                                 f"have a value of type {expected_type!r}"
                             )
-                            break
                     else:
                         if hasattr(task_type, "_validate_task_def"):
-                            issue = task_type._validate_task_def(
+                            task_type_issue = task_type._validate_task_def(
                                 task_name, task_def, config
                             )
+                            if task_type_issue:
+                                return task_type_issue
+                if "\n" in task_def.get("help", ""):
+                    return (
+                        f"Invalid task: {task_name!r}. Help messages cannot contain "
+                        "line breaks"
+                    )
             else:
-                issue = (
+                return (
                     f"Invalid task: {task_name!r}. Task definition must include exactly"
                     f" one task key from {set(cls.__task_types)!r}"
                 )
-        else:
-            return None
-
-        return issue
+        return None
 
     @classmethod
     def is_task_type(
         cls, task_def_key: str, content_type: Optional[Type] = None
     ) -> bool:
         """
         Checks whether the given key identified a known task type.
```

### Comparing `poethepoet-0.8.0/poethepoet/task/cmd.py` & `poethepoet-0.9.0/poethepoet/task/cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from glob import glob
-from pathlib import Path
 import re
 import shlex
 from typing import (
     Dict,
     Iterable,
     MutableMapping,
     Type,
     TYPE_CHECKING,
 )
 from .base import PoeTask
 
 if TYPE_CHECKING:
     from ..config import PoeConfig
-    from ..executor import PoeExecutor
+    from ..context import RunContext
 
 _GLOBCHARS_PATTERN = re.compile(r".*[\*\?\[]")
 
 
 class CmdTask(PoeTask):
     """
     A task consisting of a reference to a shell command
@@ -26,32 +25,37 @@
     content: str
 
     __key__ = "cmd"
     __options__: Dict[str, Type] = {}
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
-        cmd = self._resolve_args(extra_args, env)
-        self._print_action(" ".join(cmd), dry)
-        return executor.execute(cmd)
+        cmd = self._resolve_args(context, extra_args, env)
+        self._print_action(" ".join(cmd), context.dry)
+        return context.get_executor(env).execute(cmd)
 
-    def _resolve_args(self, extra_args: Iterable[str], env: MutableMapping[str, str]):
+    def _resolve_args(
+        self,
+        context: "RunContext",
+        extra_args: Iterable[str],
+        env: MutableMapping[str, str],
+    ):
         # Parse shell command tokens
         cmd_tokens = shlex.split(
-            self._resolve_envvars(self.content, env),
+            self._resolve_envvars(self.content, context, env),
             comments=True,
             posix=not self._is_windows,
         )
-        extra_args = [self._resolve_envvars(token, env) for token in extra_args]
+        extra_args = [
+            self._resolve_envvars(token, context, env) for token in extra_args
+        ]
         # Resolve any glob pattern paths
         result = []
         for cmd_token in (*cmd_tokens, *extra_args):
             if _GLOBCHARS_PATTERN.match(cmd_token):
                 # looks like a glob path so resolve it
                 result.extend(glob(cmd_token, recursive=True))
             else:
```

### Comparing `poethepoet-0.8.0/poethepoet/task/ref.py` & `poethepoet-0.9.0/poethepoet/task/ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from pathlib import Path
 from typing import (
     Any,
     Dict,
     Iterable,
     MutableMapping,
     Optional,
     Type,
     TYPE_CHECKING,
 )
 from .base import PoeTask
 
 if TYPE_CHECKING:
     from ..config import PoeConfig
-    from ..executor import PoeExecutor
+    from ..context import RunContext
 
 
 class RefTask(PoeTask):
     """
     A task consisting of a reference to another task
     """
 
@@ -25,27 +24,23 @@
     content: str
 
     __key__ = "ref"
     __options__: Dict[str, Type] = {}
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
         """
         Lookup and delegate to the referenced task
         """
         task = self.from_config(self.content, self._config, ui=self._ui)
-        return task.run(
-            extra_args=extra_args, project_dir=project_dir, env=env, dry=dry,
-        )
+        return task.run(context=context, extra_args=extra_args, env=env,)
 
     @classmethod
     def _validate_task_def(
         cls, task_name: str, task_def: Dict[str, Any], config: "PoeConfig"
     ) -> Optional[str]:
         """
         Check the given task definition for validity specific to this task type and
```

### Comparing `poethepoet-0.8.0/poethepoet/task/script.py` & `poethepoet-0.9.0/poethepoet/task/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pathlib import Path
 import re
 from typing import (
     Any,
     Dict,
     Iterable,
     Optional,
     MutableMapping,
@@ -11,15 +10,15 @@
     TYPE_CHECKING,
     Union,
 )
 from .base import PoeTask
 
 if TYPE_CHECKING:
     from ..config import PoeConfig
-    from ..executor import PoeExecutor
+    from ..context import RunContext
 
 
 _FUNCTION_CALL_PATTERN = re.compile(r"^(.+)\((.*)\)\s*;?\s*$")
 
 
 class ScriptTask(PoeTask):
     """
@@ -29,34 +28,35 @@
     content: str
 
     __key__ = "script"
     __options__: Dict[str, Type] = {}
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
         # TODO: check whether the project really does use src layout, and don't do
         #       sys.path.append('src') if it doesn't
         target_module, target_call = self._parse_content(self.content)
-        argv = [self.name, *(self._resolve_envvars(token, env) for token in extra_args)]
+        argv = [
+            self.name,
+            *(self._resolve_envvars(token, context, env) for token in extra_args),
+        ]
         cmd = (
             "python",  # TODO: pre-locate python from the target env?
             "-c",
             "import sys; "
             "from importlib import import_module; "
             f"sys.argv = {argv!r}; sys.path.append('src');"
             f"import_module('{target_module}').{target_call}",
         )
-        self._print_action(" ".join(argv), dry)
-        return executor.execute(cmd)
+        self._print_action(" ".join(argv), context.dry)
+        return context.get_executor(env).execute(cmd)
 
     @classmethod
     def _parse_content(cls, call_ref: str) -> Union[Tuple[str, str], Tuple[None, None]]:
         """
         Parse module and callable call out of a string like one of:
          - "some_module:main"
          - "some.module:main(foo='bar')"
```

### Comparing `poethepoet-0.8.0/poethepoet/task/sequence.py` & `poethepoet-0.9.0/poethepoet/task/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pathlib import Path
 from typing import (
     Any,
     Dict,
     Iterable,
     List,
     MutableMapping,
     Optional,
@@ -11,14 +10,15 @@
     Union,
 )
 from .base import PoeTask, TaskContent
 from ..exceptions import ExecutionError, PoeException
 
 if TYPE_CHECKING:
     from ..config import PoeConfig
+    from ..context import RunContext
     from ..executor import PoeExecutor
     from ..ui import PoeUi
 
 
 class SequenceTask(PoeTask):
     """
     A task consisting of a sequence of other tasks
@@ -48,26 +48,27 @@
                 array_item=self.options.get("default_item_type", True),
             )
             for index, item in enumerate(self.content)
         ]
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
         if any(arg.strip() for arg in extra_args):
             raise PoeException(f"Sequence task {self.name!r} does not accept arguments")
+
+        if len(self.subtasks) > 1:
+            # Indicate on the global context that there are multiple stages
+            context.multistage = True
+
         for subtask in self.subtasks:
-            task_result = subtask.run(
-                extra_args=tuple(), project_dir=project_dir, env=env, dry=dry,
-            )
+            task_result = subtask.run(context=context, extra_args=tuple(), env=env)
             if task_result and not self.options.get("ignore_fail"):
                 raise ExecutionError(
                     f"Sequence aborted after failed subtask {subtask.name!r}"
                 )
         return 0
 
     @classmethod
```

### Comparing `poethepoet-0.8.0/poethepoet/task/shell.py` & `poethepoet-0.9.0/poethepoet/task/shell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
-from pathlib import Path
 import re
 import shutil
 import subprocess
 from typing import Dict, Iterable, MutableMapping, Type, TYPE_CHECKING
 from ..exceptions import PoeException
 from .base import PoeTask
 
 if TYPE_CHECKING:
     from ..config import PoeConfig
-    from ..executor import PoeExecutor
+    from ..context import RunContext
 
 _GLOBCHARS_PATTERN = re.compile(r".*[\*\?\[]")
 
 
 class ShellTask(PoeTask):
     """
     A task consisting of a reference to a shell command
@@ -22,31 +21,29 @@
     content: str
 
     __key__ = "shell"
     __options__: Dict[str, Type] = {}
 
     def _handle_run(
         self,
-        executor: "PoeExecutor",
+        context: "RunContext",
         extra_args: Iterable[str],
-        project_dir: Path,
         env: MutableMapping[str, str],
-        dry: bool = False,
     ) -> int:
         if any(arg.strip() for arg in extra_args):
             raise PoeException(f"Shell task {self.name!r} does not accept arguments")
 
         if self._is_windows:
             shell = self._find_posix_shell_on_windows()
         else:
             # Prefer to use configured shell, otherwise look for bash
             shell = [os.environ.get("SHELL", shutil.which("bash") or "/bin/bash")]
 
-        self._print_action(self.content, dry)
-        return executor.execute(shell, input=self.content.encode())
+        self._print_action(self.content, context.dry)
+        return context.get_executor(env).execute(shell, input=self.content.encode())
 
     @staticmethod
     def _find_posix_shell_on_windows():
         # Try locate a shell from the environment
         shell_from_env = shutil.which(os.environ.get("SHELL", "bash"))
         if shell_from_env:
             return [shell_from_env]
```

### Comparing `poethepoet-0.8.0/poethepoet/ui.py` & `poethepoet-0.9.0/poethepoet/ui.py`

 * *Files identical despite different names*

### Comparing `poethepoet-0.8.0/pyproject.toml` & `poethepoet-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "poethepoet"
-version = "0.8.0"
+version = "0.9.0"
 description = "A task runner that works well with poetry."
 authors = ["Nat Noordanus <n@natn.me>"]
 readme = "README.rst"
 license = "MIT"
 repository =  "https://github.com/nat-n/poethepoet"
 homepage =  "https://github.com/nat-n/poethepoet"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 pastel = "^0.2.0"
-tomlkit = "^0.7.0"
+tomlkit = ">=0.6.0,<1.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^19.10b0"
 bpython = "^0.19"
 mypy = "^0.770"
 pylint = "^2.5.2"
 pytest = "^5.2"
```

### Comparing `poethepoet-0.8.0/setup.py` & `poethepoet-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['poethepoet', 'poethepoet.executor', 'poethepoet.task']
+['poethepoet',
+ 'poethepoet.completion',
+ 'poethepoet.executor',
+ 'poethepoet.task']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pastel>=0.2.0,<0.3.0', 'tomlkit>=0.7.0,<0.8.0']
+['pastel>=0.2.0,<0.3.0', 'tomlkit>=0.6.0,<1.0.0']
 
 entry_points = \
 {'console_scripts': ['poe = poethepoet:main']}
 
 setup_kwargs = {
     'name': 'poethepoet',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A task runner that works well with poetry.',
-    'long_description': '************\nPoe the Poet\n************\n\nA task runner that works well with poetry.\n\n.. role:: bash(code)\n   :language: bash\n\n.. role:: toml(code)\n   :language: toml\n\nFeatures\n========\n\n✅  Straight forward declaration of project tasks in your pyproject.toml (kind of like npm scripts)\n\n✅  Task are run in poetry\'s virtualenv by default\n\n✅  Tasks can be commands (with or without a shell) or references to python functions (like tool.poetry.scripts)\n\n✅  Short and sweet commands with extra arguments passed to the task :bash:`poe [options] task [task_args]`\n\n✅  Tasks can specify and reference environment variables as if they were evaluated by a shell\n\n✅  Tasks are self documenting, with optional help messages (just run poe without arguments)\n\n✅  Tasks can be defined as a sequence of other tasks\n\n✅  Shell completion of global options and task names (just for zsh so far)\n\nInstallation\n============\n\nInto your project (so it works inside poetry shell):\n\n.. code-block:: bash\n\n  poetry add --dev poethepoet\n\nAnd into your default python environment (so it works outside of poetry shell)\n\n.. code-block:: bash\n\n  pip install poethepoet\n\nEnable tab completion for zsh\n-----------------------------\n\nAssuming you have `Oh My Zsh <https://github.com/ohmyzsh/ohmyzsh>`_ installed (or have otherwise enabled completions) you can use poe to generate a zsh completion script to install somewhere in your `$fpath`.\n\nFor example, if you use Oh My Zsh then you can enable tab completion for poe global options and task names just by installing the generated function into the completions dir:\n\n.. code-block:: bash\n\n  mkdir -p $HOME/.oh-my-zsh/completions\n  poe _zsh_completion > $HOME/.oh-my-zsh/completions/_poe\n\nNote that you\'ll need to start a new shell for the new completion script to be loaded. If it still doesn\'t work try adding a call to `compinit` to the end of your zshrc file.\n\nBasic Usage\n===========\n\nDefine tasks in your pyproject.toml\n-----------------------------------\n\n`See a real example <https://github.com/nat-n/poethepoet/blob/master/pyproject.toml>`_\n\n.. code-block:: toml\n\n  [tool.poe.tasks]\n  test       = "pytest --cov=poethepoet"                                # simple command based task\n  mksandwich = { script = "my_package.sandwich:build" }                 # python script based task\n  tunnel     = { shell = "ssh -N -L 0.0.0.0:8080:$PROD:8080 $PROD &" }  # shell script based task\n\nRun tasks with the poe cli\n--------------------------\n\n.. code-block:: bash\n\n  poe test\n\nAdditional arguments are passed to the task so\n\n.. code-block:: bash\n\n  poe test -v tests/favorite_test.py\n\nresults in the following being run inside poetry\'s virtualenv\n\n.. code-block:: bash\n\n  pytest --cov=poethepoet -v tests/favorite_test.py\n\nYou can also run it like so if you fancy\n\n.. code-block:: bash\n\n  python -m poethepoet [options] task [task_args]\n\nOr install it as a dev dependency with poetry and run it like\n\n.. code-block:: bash\n\n  poetry add --dev poethepoet\n  poetry run poe [options] task [task_args]\n\nThough it that case you might like to do :bash:`alias poe=\'poetry run poe\'`.\n\nTypes of task\n=============\n\nThere are four types of task: simple commands (cmd), python scripts (script), shell\nscripts (shell), and composite tasks (sequence).\n\n- **Command tasks** contain a single command that will be executed without a shell.\n  This covers most basic use cases for example:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    format = "black ."  # strings are interpreted as commands by default\n    clean = """\n    # Multiline commands including comments work too. Unescaped whitespace is ignored.\n    rm -rf .coverage\n           .mypy_cache\n           .pytest_cache\n           dist\n           ./**/__pycache__\n    """\n    lint = { "cmd": "pylint poethepoet" }  # Inline tables with a cmd key work too\n    greet = "echo Hello $USER"  # Environment variables work, even though there\'s no shell!\n\n- **Script tasks** contain a reference to a python callable to import and execute, for\n  example:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    fetch-assets = { "script" = "my_package.assets:fetch" }\n    fetch-images = { "script" = "my_package.assets:fetch(only=\'images\')" }\n\n  As in the second example, is it possible to hard code literal arguments to the target\n  callable.\n\n  If extra arguments are passed to task on the command line, then they will be available\n  to the called python function via `sys.argv`.\n\n- **Shell tasks** are similar to simple command tasks except that they are executed\n  inside a new shell, and can consist of multiple separate commands, command\n  substitution, pipes, background processes, etc.\n\n  An example use case for this might be opening some ssh tunnels in the background with\n  one task and closing them with another like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    pfwd = { "shell" = "ssh -N -L 0.0.0.0:8080:$STAGING:8080 $STAGING & ssh -N -L 0.0.0.0:5432:$STAGINGDB:5432 $STAGINGDB &" }\n    pfwdstop = { "shell" = "kill $(pgrep -f "ssh -N -L .*:(8080|5432)")" }\n\n- **Composite tasks** are defined as a sequence of other tasks as an array.\n\n  By default the contents of the array are interpreted as references to other tasks (actually a ref task type), though this behaviour can be altered by setting the global `default_array_item_task_type` option to the name of another task type such as _cmd_, or by setting the `default_item_type` option locally on the sequence task.\n\n  **An example task with references**\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n\n    test = "pytest --cov=src"\n    build = "poetry build"\n    _publish = "poetry publish"\n    release = ["test", "build", "_publish"]\n\n  Note that tasks with names prefixed with `_` are not included in the documentation or directly executable, but can be useful for cases where a task is only needed for a sequence.\n\n  **An example task with inline tasks expressed via inline tables**\n\n  .. code-block:: toml\n\n    release = [\n      { cmd = "pytest --cov=src" },\n      { script = "devtasks:build" },\n      { ref = "_publish" },\n    ]\n\n  **An example task with inline script subtasks using default_item_type**\n\n  .. code-block:: toml\n\n    release.sequence = [\n      "devtasks:run_tests(all=True)",\n      "devtasks:build",\n      "devtasks:publish",\n    ]\n    release.default_item_type = "script"\n\n  A failure (non-zero result) will result in the rest of the tasks in the sequence not being executed, unless the `ignore_fail` option is set on the task like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    attempts.sequence = ["task1", "task2", "task3"]\n    attempts.ignore_fail = true\n\nTask level configuration\n========================\n\nTask help text\n--------------\n\nYou can specifiy help text to be shown alongside the task name in the list of available tasks (such as when executing poe with no arguments), by adding a help key like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    style = {cmd = "black . --check --diff", help = "Check code style"}\n\nEnvironment variables\n---------------------\n\nYou can specify arbitrary environment variables to be set for a task by providing the env key like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    serve.script = "myapp:run"\n    serve.env = { PORT = 9001 }\n\nNotice this example uses deep keys which can be more convenient but aren\'t as well supported by some toml implementations.\n\nProject-wide configuration options\n==================================\n\nGlobal environment variables\n----------------------------\n\nYou can configure environment variables to be set for all poe tasks in the pyproject.toml file by specifying `tool.poe.env` like so\n\n.. code-block:: toml\n\n  [tool.poe.env]\n  VAR1 = "FOO"\n  VAR2 = "BAR"\n\nRun poe from anywhere\n---------------------\n\nBy default poe will detect when you\'re inside a project with a pyproject.toml in the\nroot. However if you want to run it from elsewhere that is supported too by using the\n`--root` option to specify an alternate location for the toml file. The task will run\nwith the given location as the current working directory.\n\nIn all cases the path to project root (where the pyproject.toml resides) will be available\nas `$POE_ROOT` within the command line and process.\n\nChange the default task type\n----------------------------\n\nBy default tasks defined as strings are interpreted as shell commands, and script tasks\nrequire the more verbose table syntax to specify. For example:\n\n.. code-block:: toml\n\n  my_cmd_task = "cmd args"\n  my_script_task = { "script" = "my_package.my_module:run" }\n\nThis behaviour can be reversed by setting the `default_task_type` option in your\npyproject.toml like so:\n\n.. code-block:: toml\n\n  [tool.poe]\n  default_task_type = "script"\n\n  [tool.poe.tasks]\n  my_cmd_task = { "cmd" = "cmd args" }\n  my_script_task = "my_package.my_module:run"\n\nContributing\n============\n\nThere\'s plenty to do, come say hi in the issues! 👋\n\nTODO\n====\n\n☐ command line completion for bash & fish\n\n☐ support declaring specific arguments for a task\n\n☐ support conditional execution (a bit like make targets)\n\n☐ support verbose mode for documentation that shows task definitions\n\n☐ support running tasks outside of poetry\'s virtualenv (or in another?)\n\n☐ try to work well without poetry too\n\n☐ maybe support plumbum based tasks\n\n☐ maybe support third party task types as plugins\n\nLicence\n=======\n\nMIT.\n',
+    'long_description': '************\nPoe the Poet\n************\n\nA task runner that works well with poetry.\n\n.. role:: bash(code)\n   :language: bash\n.. role:: fish(code)\n   :language: fish\n.. role:: zsh(code)\n   :language: zsh\n\n.. role:: toml(code)\n   :language: toml\n\nFeatures\n========\n\n✅  Straight forward declaration of project tasks in your pyproject.toml (kind of like npm scripts)\n\n✅  Task are run in poetry\'s virtualenv by default\n\n✅  Tasks can be commands (with or without a shell) or references to python functions (like tool.poetry.scripts)\n\n✅  Short and sweet commands with extra arguments passed to the task :bash:`poe [options] task [task_args]`\n\n✅  Tasks can specify and reference environment variables as if they were evaluated by a shell\n\n✅  Tasks are self documenting, with optional help messages (just run poe without arguments)\n\n✅  Tasks can be defined as a sequence of other tasks\n\n✅  Shell completion of task names (and global options too for zsh)\n\nInstallation\n============\n\nInto your project (so it works inside poetry shell):\n\n.. code-block:: bash\n\n  poetry add --dev poethepoet\n\nAnd into your default python environment (so it works outside of poetry shell)\n\n.. code-block:: bash\n\n  pip install poethepoet\n\nEnable tab completion for your shell\n------------------------------------\n\nPoe comes with tab completion scripts for bash, zsh, and fish to save you keystrokes. How to install them will depend on your shell setup.\n\nZsh\n~~~\n\n.. code-block:: zsh\n\n  # oh-my-zsh\n  mkdir -p ~/.oh-my-zsh/completions\n  poe _zsh_completion > ~/.oh-my-zsh/completions/_poe\n\n  # without oh-my-zsh\n  mkdir -p ~/.zfunc/\n  poe _zsh_completion > ~/.zfunc/_poetry\n\nNote that you\'ll need to start a new shell for the new completion script to be loaded. If it still doesn\'t work try adding a call to `compinit` to the end of your zshrc file.\n\nBash\n~~~~\n\n.. code-block:: bash\n\n  # System bash\n  poe _bash_completion > /etc/bash_completion.d/poe.bash-completion\n\n  # Homebrew bash\n  poe _bash_completion > $(brew --prefix)/etc/bash_completion.d/poe.bash-completion\n\n\nHow to ensure installed bash completions are enabled may vary depending on your system.\n\nFish\n~~~~\n\n.. code-block:: fish\n\n  # Fish\n  poe _fish_completion > ~/.config/fish/completions/poe.fish\n\n  # Homebrew fish\n  poe _fish_completion > (brew --prefix)/share/fish/vendor_completions.d/poe.fish\n\n\nBasic Usage\n===========\n\nDefine tasks in your pyproject.toml\n-----------------------------------\n\n`See a real example <https://github.com/nat-n/poethepoet/blob/master/pyproject.toml>`_\n\n.. code-block:: toml\n\n  [tool.poe.tasks]\n  test       = "pytest --cov=poethepoet"                                # simple command based task\n  mksandwich = { script = "my_package.sandwich:build" }                 # python script based task\n  tunnel     = { shell = "ssh -N -L 0.0.0.0:8080:$PROD:8080 $PROD &" }  # shell script based task\n\nRun tasks with the poe cli\n--------------------------\n\n.. code-block:: bash\n\n  poe test\n\nAdditional arguments are passed to the task so\n\n.. code-block:: bash\n\n  poe test -v tests/favorite_test.py\n\nresults in the following being run inside poetry\'s virtualenv\n\n.. code-block:: bash\n\n  pytest --cov=poethepoet -v tests/favorite_test.py\n\nYou can also run it like so if you fancy\n\n.. code-block:: bash\n\n  python -m poethepoet [options] task [task_args]\n\nOr install it as a dev dependency with poetry and run it like\n\n.. code-block:: bash\n\n  poetry add --dev poethepoet\n  poetry run poe [options] task [task_args]\n\nThough it that case you might like to do :bash:`alias poe=\'poetry run poe\'`.\n\nTypes of task\n=============\n\nThere are four types of task: simple commands (cmd), python scripts (script), shell\nscripts (shell), and composite tasks (sequence).\n\n- **Command tasks** contain a single command that will be executed without a shell.\n  This covers most basic use cases for example:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    format = "black ."  # strings are interpreted as commands by default\n    clean = """\n    # Multiline commands including comments work too. Unescaped whitespace is ignored.\n    rm -rf .coverage\n           .mypy_cache\n           .pytest_cache\n           dist\n           ./**/__pycache__\n    """\n    lint = { "cmd": "pylint poethepoet" }  # Inline tables with a cmd key work too\n    greet = "echo Hello $USER"  # Environment variables work, even though there\'s no shell!\n\n- **Script tasks** contain a reference to a python callable to import and execute, for\n  example:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    fetch-assets = { "script" = "my_package.assets:fetch" }\n    fetch-images = { "script" = "my_package.assets:fetch(only=\'images\')" }\n\n  As in the second example, is it possible to hard code literal arguments to the target\n  callable.\n\n  If extra arguments are passed to task on the command line, then they will be available\n  to the called python function via `sys.argv`.\n\n- **Shell tasks** are similar to simple command tasks except that they are executed\n  inside a new shell, and can consist of multiple separate commands, command\n  substitution, pipes, background processes, etc.\n\n  An example use case for this might be opening some ssh tunnels in the background with\n  one task and closing them with another like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    pfwd = { "shell" = "ssh -N -L 0.0.0.0:8080:$STAGING:8080 $STAGING & ssh -N -L 0.0.0.0:5432:$STAGINGDB:5432 $STAGINGDB &" }\n    pfwdstop = { "shell" = "kill $(pgrep -f "ssh -N -L .*:(8080|5432)")" }\n\n- **Composite tasks** are defined as a sequence of other tasks as an array.\n\n  By default the contents of the array are interpreted as references to other tasks (actually a ref task type), though this behaviour can be altered by setting the global `default_array_item_task_type` option to the name of another task type such as _cmd_, or by setting the `default_item_type` option locally on the sequence task.\n\n  **An example task with references**\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n\n    test = "pytest --cov=src"\n    build = "poetry build"\n    _publish = "poetry publish"\n    release = ["test", "build", "_publish"]\n\n  Note that tasks with names prefixed with `_` are not included in the documentation or directly executable, but can be useful for cases where a task is only needed for a sequence.\n\n  **An example task with inline tasks expressed via inline tables**\n\n  .. code-block:: toml\n\n    release = [\n      { cmd = "pytest --cov=src" },\n      { script = "devtasks:build" },\n      { ref = "_publish" },\n    ]\n\n  **An example task with inline script subtasks using default_item_type**\n\n  .. code-block:: toml\n\n    release.sequence = [\n      "devtasks:run_tests(all=True)",\n      "devtasks:build",\n      "devtasks:publish",\n    ]\n    release.default_item_type = "script"\n\n  A failure (non-zero result) will result in the rest of the tasks in the sequence not being executed, unless the `ignore_fail` option is set on the task like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    attempts.sequence = ["task1", "task2", "task3"]\n    attempts.ignore_fail = true\n\nTask level configuration\n========================\n\nTask help text\n--------------\n\nYou can specifiy help text to be shown alongside the task name in the list of available tasks (such as when executing poe with no arguments), by adding a help key like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    style = {cmd = "black . --check --diff", help = "Check code style"}\n\nEnvironment variables\n---------------------\n\nYou can specify arbitrary environment variables to be set for a task by providing the env key like so:\n\n  .. code-block:: toml\n\n    [tool.poe.tasks]\n    serve.script = "myapp:run"\n    serve.env = { PORT = 9001 }\n\nNotice this example uses deep keys which can be more convenient but aren\'t as well supported by some toml implementations.\n\nProject-wide configuration options\n==================================\n\nGlobal environment variables\n----------------------------\n\nYou can configure environment variables to be set for all poe tasks in the pyproject.toml file by specifying `tool.poe.env` like so\n\n.. code-block:: toml\n\n  [tool.poe.env]\n  VAR1 = "FOO"\n  VAR2 = "BAR"\n\nRun poe from anywhere\n---------------------\n\nBy default poe will detect when you\'re inside a project with a pyproject.toml in the\nroot. However if you want to run it from elsewhere that is supported too by using the\n`--root` option to specify an alternate location for the toml file. The task will run\nwith the given location as the current working directory.\n\nIn all cases the path to project root (where the pyproject.toml resides) will be available\nas `$POE_ROOT` within the command line and process.\n\nChange the default task type\n----------------------------\n\nBy default tasks defined as strings are interpreted as shell commands, and script tasks\nrequire the more verbose table syntax to specify. For example:\n\n.. code-block:: toml\n\n  my_cmd_task = "cmd args"\n  my_script_task = { "script" = "my_package.my_module:run" }\n\nThis behaviour can be reversed by setting the `default_task_type` option in your\npyproject.toml like so:\n\n.. code-block:: toml\n\n  [tool.poe]\n  default_task_type = "script"\n\n  [tool.poe.tasks]\n  my_cmd_task = { "cmd" = "cmd args" }\n  my_script_task = "my_package.my_module:run"\n\nContributing\n============\n\nThere\'s plenty to do, come say hi in the issues! 👋\n\nTODO\n====\n\n☐ support declaring specific arguments for a task\n\n☐ support conditional execution (a bit like make targets)\n\n☐ support verbose mode for documentation that shows task definitions\n\n☐ support different task executors such as specifying a non-poetry venv, or working with pipenv,\n\n☐ support third party task or executor types as plugins\n\n☐ maybe provide poe as a poetry plugin\n\n☐ maybe support plumbum based tasks\n\nLicence\n=======\n\nMIT.\n',
     'author': 'Nat Noordanus',
     'author_email': 'n@natn.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nat-n/poethepoet',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `poethepoet-0.8.0/PKG-INFO` & `poethepoet-0.9.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-Metadata-Version: 2.1
-Name: poethepoet
-Version: 0.8.0
-Summary: A task runner that works well with poetry.
-Home-page: https://github.com/nat-n/poethepoet
-License: MIT
-Author: Nat Noordanus
-Author-email: n@natn.me
-Requires-Python: >=3.6,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: pastel (>=0.2.0,<0.3.0)
-Requires-Dist: tomlkit (>=0.7.0,<0.8.0)
-Project-URL: Repository, https://github.com/nat-n/poethepoet
-Description-Content-Type: text/x-rst
-
 ************
 Poe the Poet
 ************
 
 A task runner that works well with poetry.
 
 .. role:: bash(code)
    :language: bash
+.. role:: fish(code)
+   :language: fish
+.. role:: zsh(code)
+   :language: zsh
 
 .. role:: toml(code)
    :language: toml
 
 Features
 ========
 
@@ -42,15 +27,15 @@
 
 ✅  Tasks can specify and reference environment variables as if they were evaluated by a shell
 
 ✅  Tasks are self documenting, with optional help messages (just run poe without arguments)
 
 ✅  Tasks can be defined as a sequence of other tasks
 
-✅  Shell completion of global options and task names (just for zsh so far)
+✅  Shell completion of task names (and global options too for zsh)
 
 Installation
 ============
 
 Into your project (so it works inside poetry shell):
 
 .. code-block:: bash
@@ -59,28 +44,60 @@
 
 And into your default python environment (so it works outside of poetry shell)
 
 .. code-block:: bash
 
   pip install poethepoet
 
-Enable tab completion for zsh
------------------------------
+Enable tab completion for your shell
+------------------------------------
 
-Assuming you have `Oh My Zsh <https://github.com/ohmyzsh/ohmyzsh>`_ installed (or have otherwise enabled completions) you can use poe to generate a zsh completion script to install somewhere in your `$fpath`.
+Poe comes with tab completion scripts for bash, zsh, and fish to save you keystrokes. How to install them will depend on your shell setup.
 
-For example, if you use Oh My Zsh then you can enable tab completion for poe global options and task names just by installing the generated function into the completions dir:
+Zsh
+~~~
 
-.. code-block:: bash
+.. code-block:: zsh
+
+  # oh-my-zsh
+  mkdir -p ~/.oh-my-zsh/completions
+  poe _zsh_completion > ~/.oh-my-zsh/completions/_poe
 
-  mkdir -p $HOME/.oh-my-zsh/completions
-  poe _zsh_completion > $HOME/.oh-my-zsh/completions/_poe
+  # without oh-my-zsh
+  mkdir -p ~/.zfunc/
+  poe _zsh_completion > ~/.zfunc/_poetry
 
 Note that you'll need to start a new shell for the new completion script to be loaded. If it still doesn't work try adding a call to `compinit` to the end of your zshrc file.
 
+Bash
+~~~~
+
+.. code-block:: bash
+
+  # System bash
+  poe _bash_completion > /etc/bash_completion.d/poe.bash-completion
+
+  # Homebrew bash
+  poe _bash_completion > $(brew --prefix)/etc/bash_completion.d/poe.bash-completion
+
+
+How to ensure installed bash completions are enabled may vary depending on your system.
+
+Fish
+~~~~
+
+.. code-block:: fish
+
+  # Fish
+  poe _fish_completion > ~/.config/fish/completions/poe.fish
+
+  # Homebrew fish
+  poe _fish_completion > (brew --prefix)/share/fish/vendor_completions.d/poe.fish
+
+
 Basic Usage
 ===========
 
 Define tasks in your pyproject.toml
 -----------------------------------
 
 `See a real example <https://github.com/nat-n/poethepoet/blob/master/pyproject.toml>`_
@@ -302,28 +319,25 @@
 ============
 
 There's plenty to do, come say hi in the issues! 👋
 
 TODO
 ====
 
-☐ command line completion for bash & fish
-
 ☐ support declaring specific arguments for a task
 
 ☐ support conditional execution (a bit like make targets)
 
 ☐ support verbose mode for documentation that shows task definitions
 
-☐ support running tasks outside of poetry's virtualenv (or in another?)
+☐ support different task executors such as specifying a non-poetry venv, or working with pipenv,
 
-☐ try to work well without poetry too
+☐ support third party task or executor types as plugins
 
-☐ maybe support plumbum based tasks
+☐ maybe provide poe as a poetry plugin
 
-☐ maybe support third party task types as plugins
+☐ maybe support plumbum based tasks
 
 Licence
 =======
 
 MIT.
-
```

