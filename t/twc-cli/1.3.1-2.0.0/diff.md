# Comparing `tmp/twc_cli-1.3.1.tar.gz` & `tmp/twc_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-1.3.1.tar", max compression
+gzip compressed data, was "twc_cli-2.0.0.tar", max compression
```

## Comparing `twc_cli-1.3.1.tar` & `twc_cli-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     7474 2023-04-13 18:24:27.742949 twc_cli-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-1.3.1/COPYING
--rw-r--r--   0        0        0      847 2023-02-27 17:17:26.000000 twc_cli-1.3.1/README.md
--rw-r--r--   0        0        0     1078 2023-04-13 18:09:55.234206 twc_cli-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-02-27 15:10:37.000000 twc_cli-1.3.1/twc/__init__.py
--rw-r--r--   0        0        0     2620 2023-04-11 18:52:08.673104 twc_cli-1.3.1/twc/__main__.py
--rw-r--r--   0        0        0      420 2023-04-13 18:10:03.704217 twc_cli-1.3.1/twc/__version__.py
--rw-r--r--   0        0        0       59 2023-02-02 19:40:27.000000 twc_cli-1.3.1/twc/api/__init__.py
--rw-r--r--   0        0        0    40159 2023-04-12 18:59:45.905765 twc_cli-1.3.1/twc/api/client.py
--rw-r--r--   0        0        0      851 2023-03-15 17:12:36.000000 twc_cli-1.3.1/twc/api/exceptions.py
--rw-r--r--   0        0        0     1185 2023-03-31 23:29:24.000000 twc_cli-1.3.1/twc/click_ext.py
--rw-r--r--   0        0        0     7517 2023-04-12 23:56:34.801064 twc_cli-1.3.1/twc/commands/__init__.py
--rw-r--r--   0        0        0     5368 2023-02-20 20:02:22.000000 twc_cli-1.3.1/twc/commands/account.py
--rw-r--r--   0        0        0     5478 2023-04-13 16:44:35.143437 twc_cli-1.3.1/twc/commands/config.py
--rw-r--r--   0        0        0    17457 2023-03-31 22:55:25.000000 twc_cli-1.3.1/twc/commands/database.py
--rw-r--r--   0        0        0     9510 2023-03-27 17:32:43.000000 twc_cli-1.3.1/twc/commands/image.py
--rw-r--r--   0        0        0    11669 2023-03-31 19:42:48.000000 twc_cli-1.3.1/twc/commands/project.py
--rw-r--r--   0        0        0    71079 2023-04-03 11:55:13.000000 twc_cli-1.3.1/twc/commands/server.py
--rw-r--r--   0        0        0     8218 2023-02-20 16:39:53.000000 twc_cli-1.3.1/twc/commands/ssh_key.py
--rw-r--r--   0        0        0    23854 2023-04-13 18:20:28.396938 twc_cli-1.3.1/twc/commands/storage.py
--rw-r--r--   0        0        0     6283 2023-04-12 23:58:02.933876 twc_cli-1.3.1/twc/fmt.py
--rw-r--r--   0        0        0      616 2023-03-31 16:59:37.000000 twc_cli-1.3.1/twc/utils.py
--rw-r--r--   0        0        0      634 2023-04-12 20:15:47.148238 twc_cli-1.3.1/twc/vars.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 twc_cli-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    16236 2023-05-03 11:07:03.459112 twc_cli-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.0.0/COPYING
+-rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.0.0/README.md
+-rw-r--r--   0        0        0     1129 2023-05-03 11:07:09.215746 twc_cli-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.0.0/twc/__init__.py
+-rw-r--r--   0        0        0     1828 2023-05-01 22:28:37.037517 twc_cli-2.0.0/twc/__main__.py
+-rw-r--r--   0        0        0      442 2023-05-03 11:07:19.779020 twc_cli-2.0.0/twc/__version__.py
+-rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.0.0/twc/api/__init__.py
+-rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.0.0/twc/api/base.py
+-rw-r--r--   0        0        0    31988 2023-05-02 19:49:18.973417 twc_cli-2.0.0/twc/api/client.py
+-rw-r--r--   0        0        0     2260 2023-04-17 20:29:36.895547 twc_cli-2.0.0/twc/api/exceptions.py
+-rw-r--r--   0        0        0     3202 2023-05-02 20:00:23.324980 twc_cli-2.0.0/twc/api/types.py
+-rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.0.0/twc/apiwrap.py
+-rw-r--r--   0        0        0      243 2023-05-01 13:40:32.452627 twc_cli-2.0.0/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.0.0/twc/commands/account.py
+-rw-r--r--   0        0        0     7221 2023-05-02 19:57:14.010614 twc_cli-2.0.0/twc/commands/common.py
+-rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.0.0/twc/commands/config.py
+-rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.0.0/twc/commands/database.py
+-rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.0.0/twc/commands/image.py
+-rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.0.0/twc/commands/project.py
+-rw-r--r--   0        0        0    66629 2023-05-02 20:25:09.354176 twc_cli-2.0.0/twc/commands/server.py
+-rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.0.0/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.0.0/twc/commands/storage.py
+-rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.0.0/twc/fmt.py
+-rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.0.0/twc/typerx.py
+-rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.0.0/twc/utils.py
+-rw-r--r--   0        0        0      646 2023-04-30 21:08:17.345278 twc_cli-2.0.0/twc/vars.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.0.0/PKG-INFO
```

### Comparing `twc_cli-1.3.1/COPYING` & `twc_cli-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-1.3.1/twc/commands/__init__.py` & `twc_cli-2.0.0/twc/commands/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,254 +1,257 @@
-"""TWC CLI commands package.
+"""Common functions for commands."""
 
-__init__.py module contains common functions, decorators and variables.
-"""
-
-import os
+import re
 import sys
-import logging
+from enum import Enum
+from typing import Optional, Any
+from pathlib import Path, PurePath
+from logging import basicConfig, debug, DEBUG
 
-import click
 import toml
+import typer
+from typer.core import TyperOption
+from click import UsageError
 
-from twc.__version__ import __version__, __pyversion__
-from twc.api import TimewebCloud
-from twc.api import (
-    UnauthorizedError,
-    NonJSONResponseError,
-    BadResponseError,
-    UnexpectedResponseError,
-)
+from twc.__version__ import __version__
+
+
+class OutputFormat(str, Enum):
+    """Data output formats. See `output_format_option`."""
 
+    DEFAULT = "default"
+    RAW = "raw"
+    JSON = "json"
+    YAML = "yaml"
 
-# -----------------------------------------------------------------------
-# Configuration
 
+def get_root_ctx(ctx: typer.Context) -> typer.Context:
+    """Return the context of the root command. This function allows you
+    to retrieve the `typer.Context` object for the root command using the
+    current context.
 
-def get_default_config_file() -> str:
-    if os.name == "nt":
-        env_home = "USERPROFILE"
-    else:
-        env_home = "HOME"
-    return os.path.join(os.getenv(env_home), ".twcrc")
+    Each command has its own context, which stores data about the command
+    itself, all options and arguments entered by the user, and other service
+    information.
 
+    Each `typer.Context` object has a `parent` field that contains a
+    reference to the parent context. Thus it is possible to collect all
+    available contexts.
+
+    Specifically, this function loops through the objects in the `parent`
+    field until it reaches the root context, whose `parent` is None and
+    returns it.
+
+    See *_callback functions below for examples.
+    """
+    context = ctx
+    while True:
+        debug(f"cli_parser: cmd={context.command}, params={context.params}")
+        if context.parent is None:
+            break
+        context = context.parent
+    return context
+
+
+def default_config_file() -> Path:
+    """Return default configuration file path."""
+    filenames = [
+        ".twcrc",
+        ".twcrc.toml",
+    ]
+    for filename in filenames:
+        filepath = Path(PurePath(Path.home()).joinpath(filename))
+        if filepath.exists():
+            debug(f"Configuration file found: {filepath}")
+            return filepath
+    return Path(PurePath(Path.home()).joinpath(filenames[0]))
 
-def load_config(filepath: str = get_default_config_file()):
+
+def load_config(filepath: Optional[Path] = default_config_file()) -> dict:
     """Load configuration from TOML config file."""
     try:
         with open(filepath, "r", encoding="utf-8") as file:
             return toml.load(file)
     except FileNotFoundError:
         sys.exit(
             f"Configuration file {filepath} not found. Try run 'twc config'"
         )
     except OSError as error:
         sys.exit(f"Error: Cannot read configuration file {filepath}: {error}")
     except toml.TomlDecodeError as error:
         sys.exit(f"Error: Check your TOML syntax in file {filepath}: {error}")
 
 
-def set_value_from_config(ctx, param, value):
-    """Callback for Click to load option values from configuration file."""
+def load_from_config_callback(
+    param: TyperOption, value: Any, ctx: typer.Context
+) -> Any:
+    """Return value from config file. NOTE: This callback doesn't work with
+    custom enumerations such as OutputFormat and may others. Typer will return
+    None instead of actual value returning by this function.
+    """
     if value is None:
-        if not os.path.exists(ctx.params["config"]):
-            return None
         try:
-            value = load_config(ctx.params["config"])[ctx.params["profile"]][
-                param.name
-            ]
-        except KeyError:
+            config = config_callback(ctx.params["config"], ctx)
+            profile = profile_callback(ctx.params["profile"], ctx)
+            debug(
+                f"Set value from file: config={config}, profile={profile},"
+                f" param.name={param.name}"
+            )
+            value = load_config(config)[profile][param.name]
+        except KeyError as err:
+            debug(f"Not found key {err} in: {config}:{profile}")
             return None
+    debug(f"Return value: {value}")
+    if param.name == "output_format":
+        value = value.lower()
     return value
 
 
-# -----------------------------------------------------------------------
-# Logger
+def version_callback(value: bool):
+    """Print version and exit."""
+    if value:
+        print(f"v{__version__}")
+        raise typer.Exit()
 
 
-def set_logger(ctx, param, value):
-    """Click callback for '--verbose' option. Set logger settings.
-    Log HTTP requests and anything else.
-    """
+def verbose_callback(value: bool) -> bool:
+    """Typer callback to enable verbose mode. Set logger settings."""
     if value:
-        logging.basicConfig(
-            level=logging.DEBUG,
-            format="%(asctime)s:%(levelname)s:%(name)s: %(message)s",
+        basicConfig(
+            force=True,
+            level=DEBUG,
+            format="%(asctime)s:%(levelname)s:%(name)s:%(module)s:%(funcName)s: %(message)s",
             datefmt="%Y-%m-%dT%H:%M:%S%z",
         )
+    return value
 
 
-def debug(message: str, *args, **kwargs):
-    """Print DEBUG log message"""
-    logging.debug(message, *args, **kwargs)
+def config_callback(value: Path, ctx: typer.Context) -> Path:
+    """Lookup for '--config' option value and save it into `ctx`."""
+    if not value:
+        root_value = get_root_ctx(ctx).params["config"]
+        debug(f"cli parser: root lvl: config={root_value}")
+        value = root_value or default_config_file()
+    return value
 
 
-def log_request(response: object):
-    """Log data from `requests.PreparedRequest` and `requests.Response`
-    objects. Hide auth Bearer token.
-    """
-    request_headers = response.request.headers
-    request_headers.update(
-        {"Authorization": "Bearer <SENSITIVE_DATA_DELETED>"}
-    )
-
-    for key in list(request_headers.keys()):
-        debug(f"Request header: {key}: {request_headers[key]}")
-
-    if response.request.method in ["POST", "PUT", "PATCH"]:
-        debug(f"Request body (raw): {response.request.body}")
-
-    for key in list(response.headers.keys()):
-        debug(f"Response header: {key}: {response.headers[key]}")
-
-
-# -----------------------------------------------------------------------
-# CLI
-
-
-GLOBAL_OPTIONS = [
-    click.help_option("--help"),
-    click.version_option(__version__, "--version", prog_name="twc"),
-    click.option(
-        "--verbose",
-        "-v",
-        is_flag=True,
-        envvar="TWC_DEBUG",
-        callback=set_logger,
-        help="Enable verbose mode.",
-    ),
-    click.option(
-        "--config",
-        "-c",
-        metavar="FILE",
-        envvar="TWC_CONFIG_FILE",
-        default=get_default_config_file(),
-        is_eager=True,
-        show_default=True,
-        help="Use config file.",
-    ),
-    click.option(
-        "--profile",
-        "-p",
-        envvar="TWC_PROFILE",
-        default="default",
-        show_default=True,
-        is_eager=True,
-        help="Use profile.",
-    ),
-]
-
-OUTPUT_FORMAT_OPTION = [
-    click.option(
-        "--output",
-        "-o",
-        "output_format",
-        type=click.Choice(["default", "raw", "json", "yaml"]),
-        envvar="TWC_OUTPUT_FORMAT",
-        callback=set_value_from_config,
-        help="Output format.",
-    )
-]
-
-
-def options(options_list: list):
-    """Add multiple options to command."""
-
-    def wrapper(func):
-        for option in reversed(options_list):
-            func = option(func)
-        return func
-
-    return wrapper
-
-
-class MutuallyExclusiveOption(click.Option):
-    """Add mutually exclusive options support for Click. Example::
-
-    @click.option(
-        "--dry",
-        is_flag=True,
-        cls=MutuallyExclusiveOption,
-        mutually_exclusive=["wet"],
-    )
-    @click.option("--wet", is_flag=True)
-    """
+def profile_callback(value: str, ctx: typer.Context) -> str:
+    """Lookup for '--profile' option value and save it into `ctx`."""
+    if not value:
+        root_value = get_root_ctx(ctx).params["profile"]
+        debug(f"cli parser: root lvl: profile={root_value}")
+        value = root_value or "default"
+    return value
 
-    def __init__(self, *args, **kwargs):
-        self.mutually_exclusive = set(kwargs.pop("mutually_exclusive", []))
-        help = kwargs.get("help", "")  # pylint: disable=redefined-builtin
-        if self.mutually_exclusive:
-            kwargs["help"] = help + (
-                " NOTE: This argument is mutually exclusive with "
-                f"arguments: [{', '.join(self.mutually_exclusive)}]."
-            )
-        super().__init__(*args, **kwargs)
 
-    def handle_parse_result(self, ctx, opts, args):
-        if self.mutually_exclusive.intersection(opts) and self.name in opts:
-            raise click.UsageError(
-                f"Illegal usage: '{self.name}' is mutually exclusive with "
-                f"arguments: [{', '.join(self.mutually_exclusive)}]."
+def filter_callback(value: str) -> str:
+    """Validate filters format."""
+    if value:
+        if not re.match(r"^(([a-z0-9._-]+:[a-z0-9._-]+),?)+$", value, re.I):
+            raise UsageError(
+                "Invalid filter format. Filter must contain comma separated "
+                + "KEY:VALUE pairs. Allowed characters: [a-zA-Z0-9_.]"
             )
-        return super().handle_parse_result(ctx, opts, args)
+        # Make alias 'region=location'
+        value = value.replace("region", "location")
+    return value
 
 
-# -----------------------------------------------------------------------
-# API interaction
+# ------------------------------------------------------------- #
+# Very common CLI options.                                      #
+# ------------------------------------------------------------- #
 
 
-def handle_request(func):
-    def wrapper(*args, **kwargs):
-        try:
-            response = func(*args, **kwargs)
+# version: Optional[bool] = version_option,
+
+version_option = typer.Option(
+    None,
+    "--version",
+    callback=version_callback,
+    is_eager=True,
+    help="Show version and exit.",
+)
 
-            log_request(response)
-            if not response.text:
-                debug("No response body")
-
-            if response.status_code not in [200, 201, 204]:
-                raise BadResponseError
-        except UnauthorizedError:
-            print(
-                "Error: Unauthorized. "
-                + "Please check your API access token. Try run 'twc config'",
-                file=sys.stderr,
-            )
-            sys.exit(1)
-        except BadResponseError:
-            resp = response.json()
-            print("Error occurred. Details:", file=sys.stderr)
-            print(f"Status code: {resp['status_code']}", file=sys.stderr)
-            print(f" Error code: {resp['error_code']}", file=sys.stderr)
-            if isinstance(resp["message"], list):
-                for message in resp["message"]:
-                    print(f"    Message: {message}", file=sys.stderr)
-            else:
-                print(f"    Message: {resp['message']}", file=sys.stderr)
-            print(f"Response ID: {resp['response_id']}", file=sys.stderr)
-            sys.exit(1)
-        except (NonJSONResponseError, UnexpectedResponseError) as error:
-            sys.exit(f"Error: {error}")
-        return response
-
-    return wrapper
-
-
-def create_client(config, profile):
-    """Create API client instance with access token."""
-
-    debug(f"TWC CLI {__version__} Python {__pyversion__}")
-    debug(f"Args: {sys.argv[1:]}")
-
-    env_token = os.getenv("TWC_TOKEN")
-    user_agent = f"TWC-CLI/{__version__} Python {__pyversion__}"
-
-    if env_token:
-        debug("Get Timeweb Cloud token from environment variable")
-        return TimewebCloud(env_token, user_agent=user_agent)
 
-    try:
-        debug(f"Configuration: config file={config}; profile={profile}")
-        token = load_config(config)[profile]["token"]
-        return TimewebCloud(token, user_agent=user_agent)
-    except KeyError:
-        sys.exit(f"Profile '{profile}' not found in {config}")
+# verbose: Optional[bool] = verbose_option,
+
+verbose_option = typer.Option(
+    False,
+    "--verbose",
+    "-v",
+    envvar="TWC_DEBUG",
+    show_envvar=False,
+    callback=verbose_callback,
+    help="Enable verbose mode.",
+    rich_help_panel="Global options",
+)
+
+
+# Do not use following 'config' and 'profile' options in __main__.py.
+# They callbacks doesn't works properly at root level command e.g. twc -c ...
+
+
+# config: Optional[Path] = config_option,
+
+config_option = typer.Option(
+    None,
+    "--config",
+    "-c",
+    envvar="TWC_CONFIG_FILE",
+    show_envvar=False,
+    show_default=False,
+    exists=True,
+    dir_okay=False,
+    callback=config_callback,
+    help="Use config.",
+    rich_help_panel="Global options",
+)
+
+
+# profile: Optional[str] = profile_option,
+
+profile_option = typer.Option(
+    None,
+    "--profile",
+    "-p",
+    metavar="NAME",
+    envvar="TWC_PROFILE",
+    show_envvar=False,
+    show_default=False,
+    callback=profile_callback,
+    help="Use profile.",
+    rich_help_panel="Global options",
+)
+
+
+# output_format: Optional[str] = output_format_option,
+
+output_format_option = typer.Option(
+    None,
+    "--output",
+    "-o",
+    metavar="FORMAT",
+    envvar="TWC_OUTPUT_FORMAT",
+    show_default=False,
+    show_envvar=False,
+    callback=load_from_config_callback,
+    help=f"Output format, one of: [{'|'.join([k.value for k in OutputFormat])}].",
+)
+
+
+# filters: Optional[str] = filter_option,
+
+filter_option = typer.Option(
+    None,
+    "--filter",
+    "-f",
+    metavar="KEY:VALUE",
+    callback=filter_callback,
+    help="Filter output.",
+)
+
+
+# yes: Optional[bool] = yes_option,
+
+yes_option = typer.Option(
+    False, "--yes", "-y", help="Confirm the action without prompting."
+)
```

### Comparing `twc_cli-1.3.1/twc/commands/image.py` & `twc_cli-2.0.0/twc/commands/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,47 @@
-"""Image management commands."""
+"""Manage disk images."""
 
 import re
 import sys
-
-import click
-from click_aliases import ClickAliasedGroup
+from logging import debug
+from typing import Optional, List
+from pathlib import Path
+from uuid import UUID
+
+import typer
+from click import UsageError
+from requests import Response
 
 from twc import fmt
-from . import (
-    create_client,
-    handle_request,
-    options,
-    debug,
-    GLOBAL_OPTIONS,
-    OUTPUT_FORMAT_OPTION,
+from twc.typerx import TyperAlias
+from twc.apiwrap import create_client
+from twc.api import ServiceRegion, ServerOSType
+from .common import (
+    verbose_option,
+    config_option,
+    profile_option,
+    filter_option,
+    yes_option,
+    output_format_option,
 )
 
 
-@handle_request
-def _image_list(client, *args, **kwargs):
-    return client.get_images(*args, **kwargs)
-
-
-@handle_request
-def _image_get(client, *args, **kwargs):
-    return client.get_image(*args, **kwargs)
-
-
-@handle_request
-def _image_create(client, *args, **kwargs):
-    return client.create_image(*args, **kwargs)
-
-
-@handle_request
-def _image_remove(client, *args, **kwargs):
-    return client.delete_image(*args, **kwargs)
-
-
-@handle_request
-def _image_set_property(client, *args, **kwargs):
-    return client.update_image(*args, **kwargs)
-
-
-@handle_request
-def _image_upload(client, *args, **kwargs):
-    return client.upload_image(*args, **kwargs)
-
-
-# ------------------------------------------------------------- #
-# $ twc image                                                   #
-# ------------------------------------------------------------- #
-
-
-@click.group("image", cls=ClickAliasedGroup)
-@options(GLOBAL_OPTIONS[:2])
-def image():
-    """Manage disk images."""
+image = TyperAlias(help=__doc__)
 
 
 # ------------------------------------------------------------- #
 # $ twc image list                                              #
 # ------------------------------------------------------------- #
 
 
-def print_images(response: object, filters: str):
+def print_images(response: Response, filters: Optional[str] = None):
+    """Print table with images list."""
+    images = response.json()["images"]
     if filters:
-        images = fmt.filter_list(response.json()["images"], filters)
-    else:
-        images = response.json()["images"]
+        images = fmt.filter_list(images, filters)
 
     table = fmt.Table()
     table.header(
         [
             "UUID",
             "NAME",
             "REGION",
@@ -90,65 +60,53 @@
                 img["disk_id"],
                 str(round(img["size"] / 1024)) + "G",
             ]
         )
     table.print()
 
 
-@image.command("list", aliases=["ls"], help="List images.")
-@options(GLOBAL_OPTIONS)
-@options(OUTPUT_FORMAT_OPTION)
-@click.option(
-    "--limit",
-    type=int,
-    default=500,
-    show_default=True,
-    help="Items to display.",
-)
-@click.option("--filter", "-f", "filters", default="", help="Filter output.")
-@click.option("--region", help="Use region (location).")
-@click.option(
-    "--with-deleted",
-    is_flag=True,
-    help="Show all images including deleted images.",
-)
+@image.command("list", "ls")
 def image_list(
-    config,
-    profile,
-    verbose,
-    output_format,
-    limit,
-    filters,
-    region,
-    with_deleted,
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    output_format: Optional[str] = output_format_option,
+    limit: int = typer.Option(500, help="Items to display."),
+    filters: Optional[str] = filter_option,
+    region: Optional[ServiceRegion] = typer.Option(
+        None,
+        case_sensitive=False,
+        help="Use region (location).",
+    ),
+    with_deleted: Optional[bool] = typer.Option(
+        False,
+        "--with-deleted",
+        help="Show all images including deleted images.",
+    ),
 ):
-    if filters:
-        filters = filters.replace("region", "location")
+    """List images."""
     if region:
-        if filters:
-            filters = filters + f",location:{region}"
-        else:
-            filters = f"location:{region}"
-
+        filters = f"{filters},location:{region}"
     client = create_client(config, profile)
-    response = _image_list(client, limit=limit, with_deleted=with_deleted)
+    response = client.get_images(limit=limit, with_deleted=with_deleted)
     fmt.printer(
         response,
         output_format=output_format,
         filters=filters,
         func=print_images,
     )
 
 
 # ------------------------------------------------------------- #
 # $ twc image get                                               #
 # ------------------------------------------------------------- #
 
 
-def print_image(response: object):
+def print_image(response: Response):
+    """Print table with image info."""
     table = fmt.Table()
     table.header(
         [
             "UUID",
             "NAME",
             "REGION",
             "STATUS",
@@ -166,186 +124,167 @@
             img["disk_id"],
             str(round(img["size"] / 1024)) + "G",
         ]
     )
     table.print()
 
 
-@image.command("get", help="Get image.")
-@options(GLOBAL_OPTIONS)
-@options(OUTPUT_FORMAT_OPTION)
-@click.option("--status", is_flag=True, help="Print image status only.")
-@click.argument("image_id", required=True)
-def image_get(config, profile, verbose, output_format, status, image_id):
+@image.command("get")
+def image_get(
+    image_id: UUID,
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    output_format: Optional[str] = output_format_option,
+    status: Optional[bool] = typer.Option(
+        False,
+        "--status",
+        help="Display status and exit with 0 if status is 'created'.",
+    ),
+):
+    """Get image info."""
     client = create_client(config, profile)
-    response = _image_get(client, image_id)
+    response = client.get_image(image_id)
     if status:
-        _status = response.json()["image"]["status"]
-        if _status == "created":
-            click.echo(_status)
-            sys.exit(0)
-        else:
-            sys.exit(_status)
+        state = response.json()["image"]["status"]
+        if state == "created":
+            print(state)
+            raise typer.Exit()
+        sys.exit(state)
     fmt.printer(response, output_format=output_format, func=print_image)
 
 
 # ------------------------------------------------------------- #
 # $ twc image create                                            #
 # ------------------------------------------------------------- #
 
 
-@image.command("create", help="Create image.")
-@options(GLOBAL_OPTIONS)
-@options(OUTPUT_FORMAT_OPTION)
-@click.option(
-    "--name", type=str, default=None, help="Image human readable name."
-)
-@click.option("--desc", type=str, default=None, help="Image description.")
-@click.argument("disk_id", type=int, required=True)
-def image_create(config, profile, verbose, output_format, name, desc, disk_id):
+@image.command("create")
+def image_create(
+    disk_id: int,
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    output_format: Optional[str] = output_format_option,
+    name: Optional[str] = typer.Option(
+        None, help="Image human readable name."
+    ),
+    desc: Optional[str] = typer.Option(None, help="Image description."),
+):
+    """Create image from existing Cloud Server disk."""
     client = create_client(config, profile)
-    response = _image_create(
-        client, disk_id=disk_id, name=name, description=desc
+    response = client.create_image(
+        disk_id=disk_id, name=name, description=desc
     )
     fmt.printer(
         response,
         output_format=output_format,
-        func=lambda response: click.echo(response.json()["image"]["id"]),
+        func=lambda response: print(response.json()["image"]["id"]),
     )
 
 
 # ------------------------------------------------------------- #
 # $ twc image remove                                            #
 # ------------------------------------------------------------- #
 
 
-@image.command("remove", aliases=["rm"], help="Remove image.")
-@options(GLOBAL_OPTIONS)
-@click.confirmation_option(
-    prompt="This action cannot be undone. Are you sure?"
-)
-@click.argument("image_id", nargs=-1, required=True)
-def image_remove(config, profile, verbose, image_id):
+@image.command("remove", "rm")
+def image_remove(
+    image_ids: List[UUID] = typer.Argument(..., metavar="IMAGE_ID..."),
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    yes: Optional[bool] = yes_option,
+):
+    """Remove image."""
+    if not yes:
+        typer.confirm(
+            "This action cannot be undone. Continue?",
+            abort=True,
+        )
     client = create_client(config, profile)
-
-    for img in image_id:
-        response = _image_remove(client, img)
+    for image_id in image_ids:
+        response = client.delete_image(image_id)
         if response.status_code == 204:
-            click.echo(img)
+            print(image_id)
         else:
-            fmt.printer(response)
+            sys.exit(fmt.printer(response))
 
 
 # ------------------------------------------------------------- #
-# $ twc image set-property                                      #
+# $ twc image set                                               #
 # ------------------------------------------------------------- #
 
 
-@image.command("set-property", help="Change image name and description.")
-@options(GLOBAL_OPTIONS)
-@options(OUTPUT_FORMAT_OPTION)
-@click.option(
-    "--name", type=str, default=None, help="Image human readable name."
-)
-@click.option("--desc", type=str, default=None, help="Image description.")
-@click.argument("image_id", required=True)
+@image.command("set")
 def image_set_property(
-    config, profile, verbose, output_format, name, desc, image_id
+    image_id: UUID,
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    output_format: Optional[str] = output_format_option,
+    name: Optional[str] = typer.Option(
+        None, help="Image human readable name."
+    ),
+    desc: Optional[str] = typer.Option(None, help="Image description."),
 ):
+    """Change image name and description."""
+    if not name and not desc:
+        raise UsageError(
+            "Nothing to do. Set one of options: ['--name', '--desc']"
+        )
     client = create_client(config, profile)
-    response = _image_set_property(
-        client, image_id, name=name, description=desc
-    )
+    response = client.update_image(image_id, name=name, description=desc)
     fmt.printer(
         response,
         output_format=output_format,
-        func=lambda response: click.echo(response.json()["image"]["id"]),
+        func=lambda response: print(response.json()["image"]["id"]),
     )
 
 
 # ------------------------------------------------------------- #
 # $ twc image upload                                            #
 # ------------------------------------------------------------- #
 
 
-def draw_progressbar(monitor):
-    print("Bytes:", monitor.bytes_read)
-
-
-@image.command("upload", help="Upload image from URL.")
-@options(GLOBAL_OPTIONS)
-@options(OUTPUT_FORMAT_OPTION)
-@click.option(
-    "--name", type=str, default=None, help="Image human readable name."
-)
-@click.option("--desc", type=str, default=None, help="Image description.")
-@click.option(
-    "--os",
-    "os_type",
-    type=click.Choice(
-        [
-            "centos",
-            "almalinux",
-            "debian",
-            "bitrix",
-            "ubuntu",
-            "brainycp",
-            "archlinux",
-            "astralinux",
-            "windows",
-            "custom_os",
-            "other",
-        ]
-    ),
-    default="other",
-    show_default=True,
-    help="OS type.",
-)
-@click.option(
-    "--location",
-    type=click.Choice(["ru-1", "ru-2", "pl-1", "kz-1", "nl-1"]),
-    default="ru-1",
-    show_default=True,
-    help="Region to upload image.",
-)
-@click.argument("file", required=True)
+@image.command("upload")
 def image_upload(
-    config,
-    profile,
-    verbose,
-    output_format,
-    name,
-    desc,
-    os_type,
-    location,
-    file,
+    file: str = typer.Argument(..., help="Direct HTTP(S) link to image."),
+    verbose: Optional[bool] = verbose_option,
+    config: Optional[Path] = config_option,
+    profile: Optional[str] = profile_option,
+    output_format: Optional[str] = output_format_option,
+    name: Optional[str] = typer.Option(
+        None, help="Image human readable name."
+    ),
+    desc: Optional[str] = typer.Option(None, help="Image description."),
+    os_type: ServerOSType = typer.Option(
+        ServerOSType.OTHER.value,
+        metavar="OS_TYPE",
+        case_sensitive=False,
+        help="OS type. This value is formal and not affects on server/image.",
+    ),
+    region: Optional[ServiceRegion] = typer.Option(
+        ServiceRegion.RU_1.value,
+        case_sensitive=False,
+        help="Region (location) to upload image.",
+    ),
 ):
+    """Upload image from URL."""
     client = create_client(config, profile)
-    payload = {
-        "name": name,
-        "description": desc,
-        "location": location,
-        "os": os_type,
-    }
-
     if re.match(r"https?://", file):
         debug(f"Upload URL: {file}")
-        payload["upload_url"] = file
-        response = _image_create(client, **payload)
-    #    else:
-    #        filepath = os.path.realpath(file)
-    #        if os.path.exists(filepath):
-    #            filesize = os.path.getsize(file)
-    #            debug(f"Upload file: {filepath}")
-    #            debug(f"File size (bytes): {filesize}")
-    #            if filesize > 107374182400:
-    #                sys.exit(f"Error: File is too large (>100G): {file}")
-    #            image_id = _image_create(client, **payload).json()["image"]["id"]
-    #            response = _image_upload(client, image_id, filepath)
-    #        else:
-    #            sys.exit(f"Error: No such file: {file}")
+        response = client.create_image(
+            upload_url=file,
+            name=name,
+            description=desc,
+            os_type=os_type,
+            location=region,
+        )
+
+    # FUTURE: Implement file upload from local disk
 
     fmt.printer(
         response,
         output_format=output_format,
-        func=lambda response: click.echo(response.json()["image"]["id"]),
+        func=lambda response: print(response.json()["image"]["id"]),
     )
```

### Comparing `twc_cli-1.3.1/twc/fmt.py` & `twc_cli-2.0.0/twc/fmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Format console output."""
+
 # pylint: disable=no-name-in-module
 # See https://github.com/PyCQA/pylint/issues/491
 
 import re
-import sys
 import json
 
-import click
+import typer
 import yaml
 
 from pygments import highlight
 from pygments.lexers import JsonLexer, YamlLexer, IniLexer, TOMLLexer
 from pygments.formatters import TerminalFormatter
 
 
@@ -48,34 +48,34 @@
         for row in rows:
             self.row(row)
 
     def print(self):
         """Print table content to terminal."""
         widths = [max(map(len, col)) for col in zip(*self.__rows)]
         for row in self.__rows:
-            click.echo(
+            typer.echo(
                 self.__whitespace.join(
                     (val.ljust(width) for val, width in zip(row, widths))
                 )
             )
 
 
 class Printer:
     """Display data in different formats."""
 
     def __init__(self, data: object):
         self._data = data
 
     def raw(self):
         """Print raw API response text (mostly raw JSON)."""
-        click.echo(self._data.text)
+        typer.echo(self._data.text)
 
     def colorize(self, data: str, lexer: object = JsonLexer()):
         """Print colorized output. Fallback to non-color."""
-        click.echo(highlight(data, lexer, TerminalFormatter()).strip())
+        typer.echo(highlight(data, lexer, TerminalFormatter()).strip())
 
     def pretty_json(self):
         """Print colorized JSON output. Fallback to non-color output if
         Pygments not installed and fallback to raw output on JSONDecodeError.
         """
         try:
             json_data = json.dumps(
@@ -111,15 +111,15 @@
         elif output_format == "yaml":
             self.pretty_yaml()
         else:
             try:
                 if func:
                     func(self._data, **kwargs)
             except KeyError:  # fallback to 'json' or 'raw' on error
-                click.echo(
+                typer.echo(
                     "Error: Cannot represent output. Fallback to JSON.",
                     err=True,
                 )
                 self.pretty_json()
 
 
 def printer(response: object, output_format: str = "raw", func=None, **kwargs):
@@ -154,22 +154,19 @@
 
 
 def filter_list(objects: list, filters: str) -> list:
     """Filter list of objects. Return filtered list.
 
     `filters` is a string with following format::
 
-        ``<key>:<value>,<key>:<value>``
+        <key>:<value>,<key>:<value>,...
 
     Key-Value pairs count is unlimited. Available filter keys and
     values depends on passed object.
     """
-    if not re.match(r"^(([a-zA-Z0-9._-]+:[a-zA-Z0-9._-]+),?)+$", filters):
-        sys.exit("Error: Invalid filter format")
-
     for key_val in filters.split(","):
         try:
             key, val = key_val.split(":")
 
             # Allow search in megabytes or gigabytes, e.g. 1024m, 1g.
             if key in ["ram", "disk", "size"]:
                 if val.lower().endswith("m"):
@@ -196,8 +193,8 @@
         "json": JsonLexer(),
         "yaml": YamlLexer(),
         "toml": TOMLLexer(),
         "ini": IniLexer(),
     }
     if lang not in lexers:
         raise ValueError(f"Unsupported lexer: '{lang}'")
-    click.echo(highlight(data, lexers[lang], TerminalFormatter()).strip())
+    typer.echo(highlight(data, lexers[lang], TerminalFormatter()).strip())
```

### Comparing `twc_cli-1.3.1/twc/utils.py` & `twc_cli-2.0.0/twc/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Common non TWC-specific functions."""
 
 
 def merge_dicts(a: dict, b: dict, path=None) -> dict:
     """Merge b into a. Return modified a.
     Ref: https://stackoverflow.com/a/7205107
     """
+    # pylint: disable=invalid-name
     if path is None:
         path = []
     for key in b:
         if key in a:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
                 merge_dicts(a[key], b[key], path + [str(key)])
             elif a[key] == b[key]:
```

### Comparing `twc_cli-1.3.1/PKG-INFO` & `twc_cli-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 1.3.1
+Version: 2.0.0
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
-Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
-Requires-Dist: pygments (>=2.14.0,<3.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: pygments (>=2.15.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/timeweb-cloud/twc
 Description-Content-Type: text/markdown
 
 ![TWC CLI](https://github.com/timeweb-cloud/twc/blob/master/artwork/logo.svg)
 
 Timeweb Cloud Command Line Interface and simple SDK 💫
 
-> [Документация на русском](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/README.md) 🇷🇺
+> [Документация на русском](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/README.md) 🇷🇺  
+> [Command Line Interface (CLI) Reference](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/CLI_REFERENCE.md) 📜
 
 # Installation
 
 ```
 pip install twc-cli
 ```
 
@@ -50,31 +51,16 @@
 
 ```
 twc --help
 ```
 
 # Shell completion
 
-## Bash
-
-Add this to **~/.bashrc**:
+To install completion script run:
 
 ```
-eval "$(_TWC_COMPLETE=bash_source twc)"
+twc --install-completion
 ```
 
-## Zsh
-
-Add this to **~/.zshrc**:
-
-```
-eval "$(_TWC_COMPLETE=zsh_source twc)"
-```
+**twc** automatically detect your shell. Supported: Bash, Zsh, Fish, PowerShell.
 
-## Fish
-
-Add this to **~/.config/fish/completions/tw.fish**:
-
-```
-eval (env _TWC_COMPLETE=fish_source twc)
-```
```

