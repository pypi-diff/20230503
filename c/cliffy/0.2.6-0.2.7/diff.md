# Comparing `tmp/cliffy-0.2.6.tar.gz` & `tmp/cliffy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.6.tar", max compression
+gzip compressed data, was "cliffy-0.2.7.tar", max compression
```

## Comparing `cliffy-0.2.6.tar` & `cliffy-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1060 2023-04-27 06:27:19.860110 cliffy-0.2.6/LICENSE
--rw-r--r--   0        0        0     5214 2023-04-27 06:27:19.860110 cliffy-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/__init__.py
--rw-r--r--   0        0        0     4429 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     4010 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1832 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     2603 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/helper.py
--rw-r--r--   0        0        0     3459 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/homer.py
--rw-r--r--   0        0        0     1354 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/loader.py
--rw-r--r--   0        0        0      297 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7441 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/merger.py
--rw-r--r--   0        0        0     5179 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/parser.py
--rw-r--r--   0        0        0       47 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/run.py
--rw-r--r--   0        0        0     3406 2023-04-27 06:27:19.860110 cliffy-0.2.6/cliffy/transformer.py
--rw-r--r--   0        0        0      939 2023-04-27 06:27:19.860110 cliffy-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6080 1970-01-01 00:00:00.000000 cliffy-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-03 03:44:33.681462 cliffy-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5131 2023-05-03 03:44:33.685463 cliffy-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/__init__.py
+-rw-r--r--   0        0        0     4281 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     3923 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1835 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     2758 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/helper.py
+-rw-r--r--   0        0        0     3434 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/homer.py
+-rw-r--r--   0        0        0     1361 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/loader.py
+-rw-r--r--   0        0        0      297 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7441 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/merger.py
+-rw-r--r--   0        0        0     4924 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/parser.py
+-rw-r--r--   0        0        0      933 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/run.py
+-rw-r--r--   0        0        0     3533 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/transformer.py
+-rw-r--r--   0        0        0     1060 2023-05-03 03:44:33.685463 cliffy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 cliffy-0.2.7/PKG-INFO
```

### Comparing `cliffy-0.2.6/LICENSE` & `cliffy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.6/README.md` & `cliffy-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 ## Usage
 `cli <command>`
 * `init <cli name>`: Generate a template CLI manifest
 * `load <manifest>`: Add a new CLI based on the manifest
 * `render <manifest>`: Render the YAML manifest into executable code
 * `list` or `ls`: Ouput a list of loaded CLIs 
 * `update <cli name>`: Reloads a CLI
-* `disable <cli name>`: Disable a CLI
-* `enable <cli name>`: Enable a disabled CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 
 ### Basic Example
 
 1. Define a manifest
 ```yaml
 # hello.yaml
```

### Comparing `cliffy-0.2.6/cliffy/cli.py` & `cliffy-0.2.7/cliffy/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 ## CLI to generate CLIs
+import contextlib
 from typing import TextIO
 
-import rich_click as click
-from rich.console import Console
-from rich.syntax import Syntax
-from rich_click.rich_group import RichGroup
+try:
+    import rich_click as click
+    from rich.console import Console
+    from rich.syntax import Syntax
+    from rich_click.rich_group import RichGroup as AliasGroup
+except ImportError:
+    import click
+    from .rich import Console, Syntax
+    from click import Group as AliasGroup
 
 from .helper import print_rich_table, write_to_file
 from .homer import Homer
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
-class RichAliasedGroup(RichGroup):
+class AliasedGroup(AliasGroup):
     def get_command(self, ctx, cmd_name):
-        try:
+        with contextlib.suppress(KeyError):
             cmd_name = ALIASES[cmd_name].name
-        except KeyError:
-            pass
         return super().get_command(ctx, cmd_name or "")
 
 
-@click.group(context_settings=CONTEXT_SETTINGS, cls=RichAliasedGroup)
+@click.group(context_settings=CONTEXT_SETTINGS, cls=AliasedGroup)
 @click.version_option()
 def cli() -> None:
     pass
 
 
 @cli.command()
 @click.argument('manifests', type=click.File('rb'), nargs=-1)
@@ -44,16 +48,15 @@
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 def update(cli_names: list[str]) -> None:
     """Reloads CLI by name"""
     for cli_name in cli_names:
-        cli_metadata = Homer.get_cli_metadata(cli_name)
-        if cli_metadata:
+        if cli_metadata := Homer.get_cli_metadata(cli_name):
             T = Transformer(open(cli_metadata.runner_path, "r"))
             Loader.load_cli(T.cli)
             Homer.save_cli_metadata(cli_metadata.runner_path, T.cli)
             click.secho(f"~ Reloaded {T.cli.name} CLI v{T.cli.version} ~", fg="green")
             click.secho(click.style("$", fg="magenta"), nl=False)
             click.echo(f" {T.cli.name} -h")
         else:
@@ -61,17 +64,16 @@
 
 
 @cli.command()
 @click.argument('manifest', type=click.File('rb'))
 def render(manifest: TextIO) -> None:
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
-    syntax = Syntax(T.cli.code, "python", theme="monokai", line_numbers=False)
     console = Console()
-    console.print(syntax)
+    console.print(T.cli.code, overflow="fold", emoji=False, markup=False)
     click.secho(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
 
 
 @cli.command()
 @click.argument('cli_name', type=str, default="cliffy")
 @click.option('--version', '-v', type=str, show_default=True, default="v1", help="Manifest version")
 @click.option(
@@ -99,18 +101,15 @@
         click.secho(f"+ {cli_name}.yaml", fg="green")
 
 
 @cli.command("list")
 def list_clis() -> None:
     "List all CLIs loaded"
     cols = ["Name", "Version", "Manifest"]
-    rows = []
-    for metadata in Homer.get_clis():
-        rows.append([metadata.cli_name, metadata.version, metadata.runner_path])
-
+    rows = [[metadata.cli_name, metadata.version, metadata.runner_path] for metadata in Homer.get_clis()]
     print_rich_table(cols, rows, styles=["cyan", "magenta", "green"])
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
@@ -119,23 +118,11 @@
             Homer.remove_cli_metadata(cli_name)
             Loader.unload_cli(cli_name)
             click.secho(f"~ {cli_name} unloaded", fg="green")
         else:
             click.secho(f"~ {cli_name} not found", fg="red")
 
 
-@cli.command()
-@click.argument('cli_name', type=str)
-def enable(cli_name) -> None:
-    click.echo("# TODO")
-
-
-@cli.command()
-@click.argument('cli_name', type=str)
-def disable(cli_name) -> None:
-    click.echo("# TODO")
-
-
 ALIASES = {
     "rm": remove,
     "ls": list_clis,
 }
```

### Comparing `cliffy-0.2.6/cliffy/commander.py` & `cliffy-0.2.7/cliffy/commander.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,15 @@
         for greedy_command in self.greedy:
             if greedy_command.name.startswith('(*)'):
                 for group in self.groups:
                     # make it lazy and interpolate
                     lazy_command_name = greedy_command.name.replace('(*)', group)
                     lazy_command_script = greedy_command.script.replace('{(*)}', group)
 
-                    # lazy load the greedy args
-                    greedy_command_args = self.manifest.args.get(greedy_command.name)
-                    if greedy_command_args:
+                    if greedy_command_args := self.manifest.args.get(greedy_command.name):
                         self.manifest.args[lazy_command_name] = greedy_command_args
 
                     # lazy parse
                     self.add_command(Command(lazy_command_name, lazy_command_script))
 
     def is_greedy(self, val: str) -> bool:
         """Greedy strings must contain (*)- marked to be evaluated lazily."""
```

### Comparing `cliffy-0.2.6/cliffy/commanders/click.py` & `cliffy-0.2.7/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.6/cliffy/commanders/typer.py` & `cliffy-0.2.7/cliffy/commanders/typer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         self.cli += f""")
 __version__ = '{self.manifest.version}'
 __cli_name__ = '{self.manifest.name}'
 
 def version_callback(value: bool):
     if value:
-        print(__cli_name__ + ", " + __version__)
+        print(f"{{__cli_name__}}, {{__version__}}")
         raise typer.Exit()
 
 @cli.callback()
 def main(version: Optional[bool] = typer.Option(None, '--version', callback=version_callback, is_eager=True)):
     pass
 """
```

### Comparing `cliffy-0.2.6/cliffy/helper.py` & `cliffy-0.2.7/cliffy/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import operator
 import os
+import platform
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional
 
 from packaging import version
 from pydantic import BaseModel
-from rich.console import Console
-from rich.table import Table
+
+try:
+    from rich.console import Console
+    from rich.table import Table
+except ImportError:
+    from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
-PYTHON_BIN = f"{sys.exec_prefix}/bin"
+PYTHON_BIN = f"{sys.exec_prefix}/Scripts" if platform.system() == "Windows" else f"{sys.exec_prefix}/bin"
 PYTHON_EXECUTABLE = sys.executable
 CLIFFY_CLI_DIR = f"{Path(__file__).parent.resolve()}/clis"
 CLIFFY_HOME_PATH = f"{HOME_PATH}/.cliffy"
 OPERATOR_MAP = {
     '==': operator.eq,
     '!=': operator.ne,
     '>=': operator.ge,
@@ -51,15 +56,15 @@
     mode |= (mode & 0o444) >> 2
     os.chmod(path, mode)
 
 
 def wrap_as_comment(text: str, split_on: Optional[str] = None) -> str:
     if split_on:
         joiner = "\n# "
-        return "# " + joiner.join(text.split(split_on))
+        return f"# {joiner.join(text.split(split_on))}"
 
     return f"# {text}"
 
 
 def wrap_as_var(text: str) -> str:
     return '{{' + text + '}}'
```

### Comparing `cliffy-0.2.6/cliffy/homer.py` & `cliffy-0.2.7/cliffy/homer.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,15 @@
 
         Args:
             cli_name (str): CLI name
 
         Returns:
             Optional[str]: CLI metadata path
         """
-        cli_metadata_path = glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.json")
-        if cli_metadata_path:
+        if cli_metadata_path := glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.json"):
             return cli_metadata_path[0]
         return None
 
     @classmethod
     def get_clis(cls) -> Iterator[CLIMetadata]:
         """Fetches loaded CLIs metadata iteratively
```

### Comparing `cliffy-0.2.6/cliffy/loader.py` & `cliffy-0.2.7/cliffy/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import os
 
 from .commander import CLI
 from .helper import CLIFFY_CLI_DIR, PYTHON_BIN, PYTHON_EXECUTABLE, write_to_file
 
 
 class Loader:
@@ -22,19 +23,17 @@
     def load_cli(cls, cli: CLI) -> None:
         L = cls(cli)
         L.deploy_script()
         L.deploy_cli()
 
     @classmethod
     def unload_cli(cls, cli_name) -> None:
-        try:
+        with contextlib.suppress(FileNotFoundError):
             os.remove(cls.get_cli_script_path(cli_name))
             os.remove(cls.get_cli_path(cli_name))
-        except FileNotFoundError:
-            pass
 
     @staticmethod
     def get_cli_path(cli_name) -> str:
         return f"{CLIFFY_CLI_DIR}/{cli_name}.py"
 
     @staticmethod
     def get_cli_script_path(cli_name) -> str:
```

### Comparing `cliffy-0.2.6/cliffy/manifests/v1.py` & `cliffy-0.2.7/cliffy/manifests/v1.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.6/cliffy/parser.py` & `cliffy-0.2.7/cliffy/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,18 @@
 
         return base_param_name, aliases
 
     def parse_command_block(self, script: str):
         ## Bash commands start with $
         if script.startswith('$'):
             script = script.replace('$ ', '$', 1)
-            script = '>' + script[1:]
+            script = f'>{script[1:]}'
             return " " * 4 + pybash.Transformer.transform_source(script)
 
-        parsed_script = ""
-        for line in script.split('\n'):
-            parsed_script += " " * 4 + line + "\n"
-        return parsed_script
+        return "".join(" " * 4 + line + "\n" for line in script.split('\n'))
 
     def parse_command(self, block: Union[str, list[Union[str, dict[Literal['help'], str]]]]) -> str:
         if isinstance(block, list):
             script_block = []
             help_text = ""
             for block_elem in block:
                 if isinstance(block_elem, dict):
@@ -83,15 +80,14 @@
             for alias in aliases:
                 parsed_arg_type += f', "{alias}"'
 
         parsed_arg_type += '),'
         return parsed_arg_type
 
     def parse_arg(self, arg_name: str, arg_type: str) -> str:
-        parsed_arg_type = ""
         is_required = self.is_param_required(arg_type)
         default_val = self.get_default_param_val(arg_type)
         param_type = 'Option' if self.is_param_option(arg_name) else 'Argument'
         arg_aliases = []
 
         # extract default val before parsing it
         if '=' in arg_type:
@@ -105,56 +101,47 @@
         if is_required:
             arg_type = arg_type[:-1]
 
         # check for a type def that matches arg_type
         if arg_type in self.manifest.types:
             return f"{arg_name}: {self.manifest.types[arg_type]},"
 
-        # otherwise parse it
-        parsed_arg_type = self.build_param_type(
+        return self.build_param_type(
             arg_name,
             arg_type,
             typer_cls=param_type,
             aliases=arg_aliases,
             default_val=default_val,
             is_required=is_required,
         )
 
-        return parsed_arg_type
-
     def parse_args(self, command) -> str:
         if not self.manifest.args:
             return ""
 
         command_args = self.manifest.args.get(command.name)
         if not command_args:
             return ""
 
         parsed_command_args = ""
         for arg in command_args:
             arg_name, arg_type = next(iter(arg.items()))
-            parsed_command_args += self.parse_arg(arg_name.strip(), arg_type.strip()) + ' '
+            parsed_command_args += f'{self.parse_arg(arg_name.strip(), arg_type.strip())} '
 
         # strip the extra ", "
         return parsed_command_args[:-2]
 
     def get_command_func_name(self, command) -> str:
         """land.build -> land_build or sell -> sell"""
         return command.name.replace('.', '_')
 
     def get_parsed_command_name(self, command) -> str:
         """land.build -> build or sell -> sell"""
-        if '.' in command.name:
-            return command.name.split('.')[-1]
-
-        return command.name
+        return command.name.split('.')[-1] if '.' in command.name else command.name
 
     def indent_block(self, block: str) -> str:
         blocklines = block.splitlines()
-        indented_block = "\n".join([" " * 4 + line for line in blocklines])
-        return indented_block
+        return "\n".join([" " * 4 + line for line in blocklines])
 
     def to_args(self, d: dict) -> str:
-        s = ""
-        for k, v in d.items():
-            s += f" {k}={v},"
+        s = "".join(f" {k}={v}," for k, v in d.items())
         return s[:-1]
```

### Comparing `cliffy-0.2.6/cliffy/transformer.py` & `cliffy-0.2.7/cliffy/transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,20 +38,27 @@
 
         installed_pip_packages = get_installed_pip_packages()
         for dep in self.manifest.requires:
             dep_spec = parse_requirement(dep)
             if dep_spec.name not in installed_pip_packages:
                 raise SystemExit(f"MissingRequirement: CLI requires `{dep}`, please install it")
 
-            if dep_spec.version and dep_spec.operator:
-                if not compare_versions(installed_pip_packages[dep_spec.name], dep_spec.version, dep_spec.operator):
-                    raise SystemExit(
-                        f"MissingRequirement: CLI requires `{dep}`, "
-                        f"found version {installed_pip_packages[dep_spec.name]}"
-                    )
+            if (
+                dep_spec.version
+                and dep_spec.operator
+                and not compare_versions(
+                    installed_pip_packages[dep_spec.name],
+                    dep_spec.version,
+                    dep_spec.operator,
+                )
+            ):
+                raise SystemExit(
+                    f"MissingRequirement: CLI requires `{dep}`, "
+                    f"found version {installed_pip_packages[dep_spec.name]}"
+                )
 
     def resolve_includes(self) -> dict:
         include_transforms = map(self.resolve_include_by_path, set(self.command_config['includes']))
         merged_config = {}
         for transformed_include in include_transforms:
             cliffy_merger.merge(merged_config, transformed_include.command_config)
 
@@ -62,19 +69,19 @@
         with open(path, "r") as m:
             return cls(m, as_include=True)
 
     @staticmethod
     def load_manifest(manifest_io: TextIO) -> dict:
         try:
             manifest_path = os.path.realpath(manifest_io.name)
-            vars = yaml.safe_load(open(manifest_path, "r")).get('vars', {})
+            all_vars = yaml.safe_load(open(manifest_path, "r")).get('vars', {})
             var_env = Environment(loader=BaseLoader())
             interpolated_vars = {
-                var_env.from_string(str(k)).render(vars): var_env.from_string(str(v)).render(vars)
-                for k, v in vars.items()
+                var_env.from_string(str(k)).render(all_vars): var_env.from_string(str(v)).render(all_vars)
+                for k, v in all_vars.items()
             }
             manifest_env = Environment(loader=FileSystemLoader(manifest_path)).get_template("")
             return yaml.safe_load(manifest_env.render(interpolated_vars))
         except yaml.YAMLError as e:
             print("load_manifest", e)
             raise
```

### Comparing `cliffy-0.2.6/PKG-INFO` & `cliffy-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.2.6
+Version: 0.2.7
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: pybash (>=0.2.3,<0.3.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: pybash (>=0.2.5,<0.3.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: rich-click (>=1.6.1,<2.0.0)
-Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
+Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
+Requires-Dist: typer (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
 Description-Content-Type: text/markdown
 
 [![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/cliffy/python-app.yaml?branch=main)](https://github.com/jaykv/cliffy/actions)
 [![PyPI](https://img.shields.io/pypi/v/cliffy)](https://pypi.org/project/cliffy/)
 ![GitHub](https://img.shields.io/github/license/jaykv/cliffy)
 
@@ -42,16 +43,14 @@
 ## Usage
 `cli <command>`
 * `init <cli name>`: Generate a template CLI manifest
 * `load <manifest>`: Add a new CLI based on the manifest
 * `render <manifest>`: Render the YAML manifest into executable code
 * `list` or `ls`: Ouput a list of loaded CLIs 
 * `update <cli name>`: Reloads a CLI
-* `disable <cli name>`: Disable a CLI
-* `enable <cli name>`: Enable a disabled CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 
 ### Basic Example
 
 1. Define a manifest
 ```yaml
 # hello.yaml
```

