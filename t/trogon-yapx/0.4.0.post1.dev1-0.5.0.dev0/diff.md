# Comparing `tmp/trogon_yapx-0.4.0.post1.dev1.tar.gz` & `tmp/trogon_yapx-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trogon_yapx-0.4.0.post1.dev1.tar", max compression
+gzip compressed data, was "trogon_yapx-0.5.0.dev0.tar", max compression
```

## Comparing `trogon_yapx-0.4.0.post1.dev1.tar` & `trogon_yapx-0.5.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4097 2023-06-02 05:35:39.979117 trogon_yapx-0.4.0.post1.dev1/README.md
--rw-r--r--   0        0        0     4508 2023-06-02 06:02:13.159266 trogon_yapx-0.4.0.post1.dev1/pyproject.toml
--rw-r--r--   0        0        0       55 2023-06-02 04:54:04.374931 trogon_yapx-0.4.0.post1.dev1/trogon/__init__.py
--rw-r--r--   0        0        0       33 2023-06-02 06:02:23.355255 trogon_yapx-0.4.0.post1.dev1/trogon/__version__.py
--rw-r--r--   0        0        0     5495 2023-06-02 05:04:27.524860 trogon_yapx-0.4.0.post1.dev1/trogon/click.py
--rw-r--r--   0        0        0      149 2023-06-02 05:04:27.536860 trogon_yapx-0.4.0.post1.dev1/trogon/constants.py
--rw-r--r--   0        0        0     1740 2023-05-30 16:37:40.038592 trogon_yapx-0.4.0.post1.dev1/trogon/detect_run_string.py
--rw-r--r--   0        0        0     9759 2023-06-02 05:04:27.548860 trogon_yapx-0.4.0.post1.dev1/trogon/run_command.py
--rw-r--r--   0        0        0     2410 2023-06-02 04:54:04.374931 trogon_yapx-0.4.0.post1.dev1/trogon/schemas.py
--rw-r--r--   0        0        0    11118 2023-06-02 05:04:27.560860 trogon_yapx-0.4.0.post1.dev1/trogon/trogon.py
--rw-r--r--   0        0        0     3859 2023-05-30 16:37:40.038592 trogon_yapx-0.4.0.post1.dev1/trogon/trogon.scss
--rw-r--r--   0        0        0      729 2023-06-02 05:04:27.568860 trogon_yapx-0.4.0.post1.dev1/trogon/typer.py
--rw-r--r--   0        0        0        0 2023-05-30 16:37:40.038592 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/__init__.py
--rw-r--r--   0        0        0     2829 2023-06-02 05:04:27.580860 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/about.py
--rw-r--r--   0        0        0     3937 2023-06-02 05:04:27.592860 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/command_info.py
--rw-r--r--   0        0        0     1683 2023-06-02 05:04:27.604860 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/command_tree.py
--rw-r--r--   0        0        0     8068 2023-06-02 05:04:27.616861 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/form.py
--rw-r--r--   0        0        0     2861 2023-06-02 05:04:27.624861 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/multiple_choice.py
--rw-r--r--   0        0        0    15422 2023-06-02 05:04:27.636861 trogon_yapx-0.4.0.post1.dev1/trogon/widgets/parameter_controls.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 trogon_yapx-0.4.0.post1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     5786 2023-07-13 05:42:46.177504 trogon_yapx-0.5.0.dev0/README.md
+-rw-r--r--   0        0        0     1577 2023-07-13 05:43:49.753346 trogon_yapx-0.5.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-06-21 17:18:28.221349 trogon_yapx-0.5.0.dev0/trogon/__init__.py
+-rw-r--r--   0        0        0     9532 2023-07-13 05:16:10.945668 trogon_yapx-0.5.0.dev0/trogon/argparse.py
+-rw-r--r--   0        0        0     6026 2023-07-13 05:16:10.945668 trogon_yapx-0.5.0.dev0/trogon/click.py
+-rw-r--r--   0        0        0      149 2023-06-29 21:19:45.812847 trogon_yapx-0.5.0.dev0/trogon/constants.py
+-rw-r--r--   0        0        0     1740 2023-06-08 18:26:44.895049 trogon_yapx-0.5.0.dev0/trogon/detect_run_string.py
+-rw-r--r--   0        0        0    10731 2023-07-13 05:16:10.945668 trogon_yapx-0.5.0.dev0/trogon/run_command.py
+-rw-r--r--   0        0        0     3749 2023-07-13 05:16:10.945668 trogon_yapx-0.5.0.dev0/trogon/schemas.py
+-rw-r--r--   0        0        0    12678 2023-07-13 05:16:11.353667 trogon_yapx-0.5.0.dev0/trogon/trogon.py
+-rw-r--r--   0        0        0     3859 2023-06-08 18:26:44.899049 trogon_yapx-0.5.0.dev0/trogon/trogon.scss
+-rw-r--r--   0        0        0      729 2023-06-23 19:37:01.326822 trogon_yapx-0.5.0.dev0/trogon/typer.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:26:44.899049 trogon_yapx-0.5.0.dev0/trogon/widgets/__init__.py
+-rw-r--r--   0        0        0     2829 2023-06-08 18:26:44.899049 trogon_yapx-0.5.0.dev0/trogon/widgets/about.py
+-rw-r--r--   0        0        0     3936 2023-06-21 17:18:28.225349 trogon_yapx-0.5.0.dev0/trogon/widgets/command_info.py
+-rw-r--r--   0        0        0     2213 2023-07-13 05:16:11.149667 trogon_yapx-0.5.0.dev0/trogon/widgets/command_tree.py
+-rw-r--r--   0        0        0     8068 2023-07-01 23:01:47.859293 trogon_yapx-0.5.0.dev0/trogon/widgets/form.py
+-rw-r--r--   0        0        0     2861 2023-06-08 18:26:44.899049 trogon_yapx-0.5.0.dev0/trogon/widgets/multiple_choice.py
+-rw-r--r--   0        0        0    16329 2023-07-13 05:16:10.945668 trogon_yapx-0.5.0.dev0/trogon/widgets/parameter_controls.py
+-rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 trogon_yapx-0.5.0.dev0/PKG-INFO
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/README.md` & `trogon_yapx-0.5.0.dev0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 
 <p align="center">
     <img src="https://github.com/Textualize/trogon/assets/554369/f4751783-c322-4143-a6c1-d8c564d4e38f" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
-
+    
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
-This fork of Trogon introduces these changes:
+---
+
+This is a fork of Trogon that introduces these features:
 
-- make `click` optional
-- add support for manually constructing schemas for the TUI
-- add support for `typer`
-- add support for `yapx`
-- remove support for sequences with differing types (e.g., click tuples)
-- remove support for custom click types, e.g., `IntRange`, `FloatRange`
+- refactor to make click optional
+- remove support for custom click types `IntRange`, `FloatRange`
+- support for manually constructing schemas
+- support for argparse
+- support for typer
+- add examples for yapx, myke, and sys.argv
+- support ommission of hidden parameters and subcommands from the TUI
+- support the redaction of sensitive "secret" values
+- support for showing required prompts as read-only
 - positional arguments come before keyword arguments in the generated command
 - ability to join list arguments values like this: `-x 1 -x 2 -x 3` (default), or like this: `-x 1 2 3`
+- vim-friendly keybindings
+
+I was motivated to create this fork so I could integrate Trogon into my Python CLI library [Yapx](https://www.f2dv.com/code/r/yapx/i/).
 
+---
 
 # Trogon
 
 Auto-generate friendly terminal user interfaces for command line apps.
 
 
-<details>
+<details>  
   <summary> 🎬 Video demonstration </summary>
 
 &nbsp;
-
+    
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
 https://github.com/Textualize/trogon/assets/554369/c9e5dabb-5624-45cb-8612-f6ecfde70362
 
 </details>
 
 
-Trogon works magically with the [Click](https://click.palletsprojects.com/) library for Python, and also with [Typer](https://github.com/tiangolo/typer) and [yapx](https://github.com/fresh2dev/yapx). You can even build it yourself and use `sys.argv`.
+Trogon works with the popular Python libraries [Argparse](https://docs.python.org/3/library/argparse.html), [Click](https://click.palletsprojects.com/), [Typer](https://github.com/tiangolo/typer), [Yapx](https://www.f2dv.com/code/r/yapx/i/), and [myke](https://www.f2dv.com/code/r/myke/i/), and will support other libraries and languages in the future. You can also manually build your own TUI schema and use it however you like, even in conjunction with `sys.argv`. See the `examples/` directory for examples of each.
 
 ## How it works
 
 Trogon inspects your (command line) app and extracts a *schema* which describes the options / switches / help etc.
-It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command.
+It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command. 
 
 Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps.
 This which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
@@ -97,22 +106,65 @@
 
 ```bash
 pip install trogon
 ```
 
 ## Quickstart
 
-1. Import `from trogon import tui`
+### Click
+
+1. Import `from trogon.click import tui`
 2. Add the `@tui` decorator above your click app. e.g.
     ```python
     @tui()
     @click.group(...)
     def cli():
         ...
     ```
 3. Your click app will have a new `tui` command available.
 
-See also the `examples` folder for two example apps.
+### Argparse
+
+1. Import `from trogon.argparse import add_tui_argument`
+      or, `from trogon.argparse import add_tui_command`
+2. Add the TUI argument/command to your argparse parser. e.g.
+    ```python
+    parser = argparse.ArgumentParser()
+
+    # add tui argument (my-cli --tui)
+    add_tui_argument(parser)
+    # and/or, add tui command (my-cli tui)
+    add_tui_command(parser)
+    ```
+3. Your argparse parser will have a new parameter `--tui` and/or a new command `tui`.
+
+See also the `examples` folder for example apps.
+
+## Custom command name and custom help
+
+By default the command added will be called `tui` and the help text for it will be `Open Textual TUI.`
+
+You can customize one or both of these using the `help=` and `command=` parameters.
+
+### Click
+
+```python
+@tui(command="ui", help="Open terminal UI")
+@click.group(...)
+def cli():
+    ...
+```
+
+### Argparse
+
+```python
+parser = argparse.ArgumentParser()
+
+# add tui argument (my-cli --tui)
+add_tui_argument(parser, option_strings=["--ui"], help="Open terminal UI")
+# and/or, add tui command (my-cli tui)
+add_tui_command(parser, command="ui", help="Open terminal UI")
+```
 
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr) where you can talk to Textual developers / community.
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/click.py` & `trogon_yapx-0.5.0.dev0/trogon/click.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Sequence
+from typing import Type
 
 
 from trogon import Trogon
 
 try:
     import click
     from click import BaseCommand
@@ -15,14 +15,15 @@
 from trogon.constants import DEFAULT_COMMAND_NAME
 from trogon.trogon import Trogon
 from trogon.schemas import (
     ArgumentSchema,
     CommandName,
     CommandSchema,
     OptionSchema,
+    ChoiceSchema,
 )
 from typing import Type, Any
 from uuid import UUID
 from datetime import datetime
 from pathlib import Path
 
 CLICK_TO_PY_TYPES: dict[click.ParamType, Type[Any]] = {
@@ -33,14 +34,21 @@
     click.types.UUIDParameterType: UUID,
     click.IntRange: int,
     click.FloatRange: float,
     click.DateTime: datetime,
     click.Path: Path,
 }
 
+def _convert_click_to_py_type(click_type: Type[Any]) -> Type[Any]:
+    if isinstance(click_type, click.Choice):
+        return ChoiceSchema(choices=click_type.choices)
+
+    return CLICK_TO_PY_TYPES.get(
+        click_type, CLICK_TO_PY_TYPES.get(type(click_type), str)
+    )
 
 def introspect_click_app(
     app: BaseCommand, cmd_ignorelist: list[str] | None = None
 ) -> dict[CommandName, CommandSchema]:
     """
     Introspect a Click application and build a data structure containing
     information about all commands, options, arguments, and subcommands,
@@ -69,53 +77,60 @@
             name=cmd_name,
             docstring=cmd_obj.help,
             options=[],
             arguments=[],
             subcommands={},
             parent=parent,
         )
+
         for param in cmd_obj.params:
-            param_type: Type[Any] = CLICK_TO_PY_TYPES.get(
-                param.type, CLICK_TO_PY_TYPES.get(type(param.type), str)
-            )
-            param_choices: Sequence[str] | None = None
-            if isinstance(param.type, click.Choice):
-                param_choices = param.type.choices
+
+            click_types: list[Type[Any]] = param.type.types if isinstance(param.type, click.Tuple) else [param.type]
+
+            param_types: list[Type[Any]] = [_convert_click_to_py_type(x) for x in click_types]
 
             if isinstance(param, (click.Option, click.core.Group)):
+                if param.hidden:
+                    continue
+
+                prompt_required: bool = param.prompt and param.prompt_required
+
                 option_data = OptionSchema(
                     name=param.opts,
-                    type=param_type,
+                    type=param_types,
                     is_flag=param.is_flag,
                     counting=param.count,
                     secondary_opts=param.secondary_opts,
                     required=param.required,
                     default=param.default,
                     help=param.help,
-                    choices=param_choices,
+                    choices=None,
                     multiple=param.multiple,
                     nargs=param.nargs,
+                    secret=param.hide_input,
+                    read_only=prompt_required,
+                    placeholder="< You will be prompted. >" if prompt_required else "",
                 )
                 cmd_data.options.append(option_data)
 
             elif isinstance(param, click.Argument):
                 argument_data = ArgumentSchema(
                     name=param.name,
-                    type=param_type,
+                    type=param_types,
                     required=param.required,
-                    choices=param_choices,
+                    choices=None,
                     multiple=param.multiple,
                     default=param.default,
                     nargs=param.nargs,
                 )
                 cmd_data.arguments.append(argument_data)
 
         if isinstance(cmd_obj, click.core.Group):
             for subcmd_name, subcmd_obj in cmd_obj.commands.items():
-                if subcmd_name not in cmd_ignorelist:
+                if not subcmd_obj.hidden and subcmd_name not in cmd_ignorelist:
                     cmd_data.subcommands[CommandName(subcmd_name)] = process_command(
                         CommandName(subcmd_name),
                         subcmd_obj,
                         parent=cmd_data,
                     )
 
         return cmd_data
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/detect_run_string.py` & `trogon_yapx-0.5.0.dev0/trogon/detect_run_string.py`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/run_command.py` & `trogon_yapx-0.5.0.dev0/trogon/run_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     CommandName,
     CommandSchema,
     MultiValueParamData,
     OptionSchema,
 )
 from trogon.widgets.parameter_controls import ValueNotSupplied
 
+REDACTED_PLACEHOLDER: str = "<redacted>"
+
 
 @dataclass
 class UserOptionData:
     """
     A dataclass to store user input for a specific option.
 
     Attributes:
@@ -73,38 +75,40 @@
     name: CommandName
     options: List[UserOptionData]
     arguments: List[UserArgumentData]
     subcommand: Optional["UserCommandData"] = None
     parent: Optional["UserCommandData"] = None
     command_schema: Optional["CommandSchema"] = None
 
-    def to_cli_args(self, include_root_command: bool = False) -> List[str]:
+    def to_cli_args(self, include_root_command: bool = False, redact_secret: bool = False) -> List[str]:
         """
         Generates a list of strings representing the CLI invocation based on the user input data.
 
         Returns:
             A list of strings that can be passed to subprocess.run to execute the command.
         """
-        cli_args = self._to_cli_args()
+        cli_args = self._to_cli_args(redact_secret=redact_secret)
         if not include_root_command:
             cli_args = cli_args[1:]
 
         return cli_args
 
-    def _to_cli_args(self):
+    def _to_cli_args(self, redact_secret: bool = False):
         args = [self.name]
 
         for argument in self.arguments:
-            this_arg_values = argument.value
-            for argument_value in this_arg_values:
-                if argument_value != ValueNotSupplied():
-                    args.append(argument_value)
+            this_arg_values = [value for value in argument.value if value != ValueNotSupplied()]
+
+            if redact_secret and argument.argument_schema.secret:
+                args.extend([REDACTED_PLACEHOLDER] * len(this_arg_values))
+            else:
+                args.extend(this_arg_values)
 
         multiples = defaultdict(list)
-        multiples_schemas = {}
+        multiples_schemas: dict[str, OptionSchema] = {}
 
         for option in self.options:
             if option.option_schema.multiple:
                 # We need to gather the items for the same option,
                 #  compare them to the default, then display them all
                 #  if they aren't equivalent to the default.
                 multiples[option.string_name].append(option.value)
@@ -163,16 +167,24 @@
                                 args.append(longest_secondary_name)
                     else:
                         if not option.option_schema.counting:
                             # Although buried away a little, this branch here is
                             # actually the nominal case... single value options e.g.
                             # `--foo bar`.
                             args.append(option_name)
-                            for subvalue_tuple in value_data:
-                                args.extend(subvalue_tuple)
+                            if redact_secret and option.option_schema.secret:
+                                args.extend(
+                                    [REDACTED_PLACEHOLDER] * sum(len(subvalue_tuple) for subvalue_tuple in value_data)
+                                )
+                            else:
+                                args.extend(
+                                    subvalue
+                                    for subvalue_tuple in value_data
+                                    for subvalue in subvalue_tuple
+                                )
                         else:
                             # Get the value of the counting option
                             count = next(itertools.chain.from_iterable(value_data), 1)
                             try:
                                 count = int(count)
                             except ValueError:
                                 # TODO: Not sure if this is the right thing to do
@@ -182,15 +194,16 @@
                                 args.extend([option_name] * count)
                             else:
                                 clean_option_name = option_name.lstrip("-")
                                 args.append(f"-{clean_option_name * count}")
 
         for option_name, values in multiples.items():
             # Check if the values given for this option differ from the default
-            defaults = multiples_schemas[option_name].default or []
+            schema = multiples_schemas[option_name]
+            defaults = schema.default or []
             default_values = list(itertools.chain.from_iterable(defaults.values))
             supplied_defaults = [
                 value for value in default_values if value != ValueNotSupplied()
             ]
             supplied_defaults = list(map(str, supplied_defaults))
             supplied_defaults = sorted(supplied_defaults)
 
@@ -208,32 +221,39 @@
 
             # If the user has supplied any non-default values, include them...
             if values_supplied and not values_are_defaults:
                 for i, value_data in enumerate(values):
                     if not all(value == ValueNotSupplied() for value in value_data):
                         # without multi-value (default): -u x -u y -u z
                         # with multi-value: -u x y z
-                        if i == 0 or not option.option_schema.multi_value:
+                        if i == 0 or not schema.multi_value:
                             args.append(option_name)
-                        args.extend(v for v in value_data)
+
+                        if redact_secret and schema.secret:
+                            args.extend([REDACTED_PLACEHOLDER] * len(value_data))
+                        else:
+                            args.extend(value_data)
 
         if self.subcommand:
-            args.extend(self.subcommand._to_cli_args())
+            args.extend(self.subcommand._to_cli_args(redact_secret=redact_secret))
 
         return args
 
     def to_cli_string(self, include_root_command: bool = False) -> Text:
         """
-        Generates a string representing the CLI invocation as if typed directly into the
-        command line.
+        Generates a redacted string representing the CLI invocation as if typed
+        directly into the command line.
 
         Returns:
             A string representing the command invocation.
         """
-        args = self.to_cli_args(include_root_command=include_root_command)
+        args = self.to_cli_args(
+            include_root_command=include_root_command,
+            redact_secret=True,
+        )
 
         text_renderables = []
         for arg in args:
             text_renderables.append(
                 Text(shlex.quote(str(arg)))
                 if arg != ValueNotSupplied()
                 else Text("???", style="bold black on red")
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/trogon.py` & `trogon_yapx-0.5.0.dev0/trogon/trogon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 from __future__ import annotations
 
 import os
 import shlex
 import sys
 from contextlib import suppress
 from pathlib import Path
+from fnmatch import fnmatch
 from webbrowser import open as open_url
 
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 from rich.text import Text
-from textual import events, on
-from textual.app import App, AutopilotCallbackType, ComposeResult
+from textual import log, events, on
+from textual.app import ComposeResult, App, AutopilotCallbackType
 from textual.binding import Binding
-from textual.containers import Horizontal, Vertical, VerticalScroll
+from textual.containers import Vertical, Horizontal, VerticalScroll
 from textual.css.query import NoMatches
 from textual.screen import Screen
-from textual.widgets import Button, Footer, Label, Static, Tree
+from textual.widgets import (
+    Tree,
+    Label,
+    Static,
+    Button,
+    Footer,
+)
 from textual.widgets.tree import TreeNode
 
 from trogon.detect_run_string import detect_run_string
 from trogon.schemas import CommandName, CommandSchema
 from trogon.run_command import UserCommandData
 from trogon.widgets.command_info import CommandInfo
 from trogon.widgets.command_tree import CommandTree
 from trogon.widgets.form import CommandForm
 from trogon.widgets.multiple_choice import NonFocusableVerticalScroll
+from subprocess import run
 
 if sys.version_info >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
 
 class CommandBuilder(Screen):
     COMPONENT_CLASSES = {"version-string", "prompt", "command-name-syntax"}
 
     BINDINGS = [
-        Binding(key="ctrl+r", action="close_and_run", description="Close & Run"),
+        Binding(key="ctrl+r", action="close_and_run", description="Run Command"),
+        Binding(key="ctrl+y", action="copy_command_string", description="Copy Command"),
         Binding(
-            key="ctrl+t", action="focus_command_tree", description="Focus Command Tree"
+            key="ctrl+t,escape", action="focus_command_tree", description="Focus Command Tree"
         ),
-        Binding(key="ctrl+o", action="show_command_info", description="Command Info"),
-        Binding(key="ctrl+s", action="focus('search')", description="Search"),
+        Binding(key="ctrl+o,?", action="show_command_info", description="Command Info"),
+        Binding(key="ctrl+s,i,/", action="focus('search')", description="Search"),
         Binding(key="f1", action="about", description="About"),
+        Binding("q", "exit", show=False),
     ]
 
     def __init__(
         self,
         command_schemas: dict[CommandName, CommandSchema],
         app_name: str,
         app_version: str | None,
@@ -114,17 +124,42 @@
                 # ),
                 id="home-exec-preview",
             )
 
         yield Footer()
 
     def action_close_and_run(self) -> None:
+        self.app.post_run_command_redacted = self.command_data.to_cli_string()
+        self.app.post_run_command = self.command_data.to_cli_args()
         self.app.execute_on_exit = True
         self.app.exit()
 
+    def action_copy_command_string(self) -> None:
+        cmd: list[str] = (
+            ["copy"]
+            if sys.platform == 'win32'
+            else ["pbcopy"]
+            if sys.platform == 'darwin'
+            else ["xclip", "-selection", "clipboard"]
+            # if linux
+        )
+
+        run(
+            cmd,
+            input=self.app_name + " " + " ".join(
+                shlex.quote(str(x))
+                for x in self.command_data.to_cli_args(redact_secret=True)
+            ),
+            text=True,
+            check=False,
+        )
+
+    def action_exit(self) -> None:
+        self.app.exit()
+
     def action_about(self) -> None:
         from .widgets.about import AboutDialog
 
         self.app.push_screen(AboutDialog())
 
     async def on_mount(self, event: events.Mount) -> None:
         await self._refresh_command_form()
@@ -173,15 +208,15 @@
     ) -> None:
         """Update the preview box showing the command string to be executed"""
         if self.command_data is not None:
             command_name_syntax_style = self.get_component_rich_style(
                 "command-name-syntax"
             )
             prefix = Text(f"{self.app_name} ", command_name_syntax_style)
-            new_value = command_data.to_cli_string(include_root_command=False)
+            new_value = command_data.to_cli_string()
             highlighted_new_value = Text.assemble(prefix, self.highlighter(new_value))
             prompt_style = self.get_component_rich_style("prompt")
             preview_string = Text.assemble(("$ ", prompt_style), highlighted_new_value)
             self.query_one("#home-exec-preview-static", Static).update(preview_string)
 
     async def _update_form_body(self, node: TreeNode[CommandSchema]) -> None:
         # self.query_one(Pretty).update(node.data)
@@ -203,17 +238,35 @@
     CSS_PATH = Path(__file__).parent / "trogon.scss"
 
     def __init__(
         self,
         command_schemas: dict[CommandName, CommandSchema],
         app_name: str | None,
         app_version: str | None = None,
+        command_filter: str | None = None,
     ) -> None:
         super().__init__()
+
         self.post_run_command: list[str] = []
+        self.post_run_command_redacted: str = ""
+
+        root_cmd_name: str = list(command_schemas.keys())[0]
+        if command_filter and command_schemas[root_cmd_name].subcommands:
+            matching_schemas: dict[CommandName, CommandSchema] = {
+                k: v
+                for k, v in command_schemas[root_cmd_name].subcommands.items()
+                if fnmatch(k, command_filter)
+            }
+            if len(matching_schemas) == 1 and not any(x in command_filter for x in ('*', '?')):
+                command_schemas = matching_schemas
+                root_cmd_name = list(command_schemas.keys())[0]
+                #  app_name = app_name + " " + root_cmd_name
+            else:
+                command_schemas[root_cmd_name].subcommands = matching_schemas
+
         self.command_schemas = command_schemas
         self.is_grouped_cli = any(v.subcommands for v in command_schemas.values())
         self.execute_on_exit = False
 
         self.app_name = app_name if app_name else detect_run_string()
         self.app_version = app_version
 
@@ -261,31 +314,25 @@
         try:
             super().run(headless=headless, size=size, auto_pilot=auto_pilot)
         finally:
             if self.post_run_command:
                 console = Console()
                 if self.post_run_command and self.execute_on_exit:
                     console.print(
-                        f"Running [b cyan]{self.app_name} {' '.join(shlex.quote(s) for s in self.post_run_command)}[/]"
+                        f"Running [b cyan]{self.app_name} {self.post_run_command_redacted}[/]"
                     )
 
                     split_app_name = shlex.split(self.app_name)
                     program_name = split_app_name[0]
                     arguments = [*split_app_name, *self.post_run_command]
                     # update PATH to include current working dir.
                     env: dict[str, str] = os.environ.copy()
                     env["PATH"] = os.pathsep.join([os.getcwd(), env["PATH"]])
                     os.execvpe(program_name, arguments, env)
 
-    @on(CommandForm.Changed)
-    def update_command_to_run(self, event: CommandForm.Changed):
-        self.post_run_command = event.command_data.to_cli_args(
-            include_root_command=False
-        )
-
     def action_focus_command_tree(self) -> None:
         try:
             command_tree = self.query_one(CommandTree)
         except NoMatches:
             return
 
         command_tree.focus()
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/trogon.scss` & `trogon_yapx-0.5.0.dev0/trogon/trogon.scss`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/typer.py` & `trogon_yapx-0.5.0.dev0/trogon/typer.py`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/widgets/about.py` & `trogon_yapx-0.5.0.dev0/trogon/widgets/about.py`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/widgets/command_info.py` & `trogon_yapx-0.5.0.dev0/trogon/widgets/command_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 )
                 tabs.focus()
                 yield tabs
 
             command_info = (
                 self.command_schema.docstring.strip()
                 if self.command_schema.docstring
-                else "No description available."
+                else "No description available"
             )
 
             with ContentSwitcher(
                 initial="command-info-text", id="command-info-switcher"
             ):
                 yield Static(
                     command_info, id="command-info-text", classes="command-info-text"
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/widgets/form.py` & `trogon_yapx-0.5.0.dev0/trogon/widgets/form.py`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/widgets/multiple_choice.py` & `trogon_yapx-0.5.0.dev0/trogon/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `trogon_yapx-0.4.0.post1.dev1/trogon/widgets/parameter_controls.py` & `trogon_yapx-0.5.0.dev0/trogon/widgets/parameter_controls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from __future__ import annotations
 
 import functools
 from functools import partial
 from typing import Any, Callable, Iterable, Sequence, Type, TypeVar, Union, cast
 
 from rich.text import Text
-from textual import on
+from textual import log, on
 from textual.app import ComposeResult
-from textual.containers import Horizontal, Vertical
+from textual.containers import Vertical, Horizontal
 from textual.css.query import NoMatches
 from textual.widget import Widget
-from textual.widgets import Button, Checkbox, Input, Label, Select, Static
+from textual.widgets import (
+    RadioButton,
+    Label,
+    Checkbox,
+    Input,
+    Select,
+    Static,
+    Button,
+)
 
-from trogon.schemas import ArgumentSchema, MultiValueParamData, OptionSchema
+
+from trogon.schemas import ArgumentSchema, MultiValueParamData, OptionSchema, ChoiceSchema
 from trogon.widgets.multiple_choice import MultipleChoice
 
 ControlWidgetType: TypeVar = Union[Input, Checkbox, MultipleChoice, Select]
 
 
 class ControlGroup(Vertical):
     pass
@@ -71,15 +80,17 @@
                 name_contains_query = filter_query in name.casefold()
                 should_be_visible = name_contains_query
             else:
                 # Option names are lists since they can have multiple names (e.g. -v and --verbose)
                 name_contains_query = any(
                     filter_query in name.casefold() for name in self.schema.name
                 )
-                help_contains_query = filter_query in help_text.casefold()
+                help_contains_query = (
+                    filter_query in help_text.casefold()
+                )
                 should_be_visible = name_contains_query or help_contains_query
 
             self.display = should_be_visible
 
         # Update the highlighting of the help text
         if help_text:
             try:
@@ -121,15 +132,15 @@
 
             if schema.choices and multiple:
                 # Display a MultipleChoice widget
                 # There's a special case where we have a Choice with multiple=True,
                 # in this case, we can just render a single MultipleChoice widget
                 # instead of multiple radio-sets.
                 control_method = self.get_control_method(
-                    argument_type, choices=schema.choices
+                    param_type=ChoiceSchema(choices=schema.choices)
                 )
                 multiple_choice_widget = control_method(
                     default=default,
                     label=label,
                     multiple=multiple,
                     schema=schema,
                     control_id=schema.key,
@@ -174,15 +185,15 @@
         # Take note of the first form control, so we can easily focus it
         if self.first_control is None:
             self.first_control = first_focus_control
 
         # If it's a multiple, and it's a Choice parameter, then we display
         # our special case MultiChoice widget, and so there's no need for this
         # button.
-        if multiple or nargs == -1 and not schema.choices:
+        if (multiple or nargs == -1) and not schema.choices:
             with Horizontal(classes="add-another-button-container"):
                 yield Button("+ value", variant="success", classes="add-another-button")
 
         # Render the dim help text below the form controls
         if help_text:
             yield Static(help_text, classes="command-form-control-help-text")
 
@@ -196,20 +207,28 @@
         required = schema.required
         is_option = isinstance(schema, OptionSchema)
         label = self._make_command_form_control_label(
             name, parameter_type, is_option, required, multiple
         )
 
         # Get the types of the parameter. We can map these types on to widgets that will be rendered.
-        parameter_types = [parameter_type]
+        parameter_types = [
+            parameter_type[i] if i < len(parameter_type) else parameter_type[-1]
+            for i in range(schema.nargs if schema.nargs > 1 else 1)
+        ]
+        # The above ensures that len(parameter_types) == nargs.
+        # if there are more parameter_types than args, parameter_types is truncated.
+        # if there are fewer parameter_types than args, the *last* parameter type is repeated as much as necessary.
 
         # For each of the these parameters, render the corresponding widget for it.
         # At this point we don't care about filling in the default values.
         for _type in parameter_types:
-            control_method = self.get_control_method(_type, choices=schema.choices)
+            if schema.choices:
+                _type = ChoiceSchema(choices=schema.choices)
+            control_method = self.get_control_method(param_type=_type)
             control_widgets = control_method(
                 default, label, multiple, schema, schema.key
             )
             yield from control_widgets
 
     @on(Button.Pressed, ".add-another-button")
     def add_another_widget_group(self, event: Button.Pressed) -> None:
@@ -284,38 +303,41 @@
                 collected_values.append(control_values)
 
             # Since we fetched a flat list of widgets (and thus a flat list of values
             # from those widgets), we now need to group them into tuples based on nargs.
             # We can safely do this since widgets are added to the DOM in the same order
             # as the types specified in the click Option `type`. We convert a flat list
             # of widget values into a list of tuples, each tuple of length nargs.
-            collected_values = list_to_tuples(collected_values, self.schema.nargs)
+            collected_values = list_to_tuples(collected_values, max(1, self.schema.nargs))
             return MultiValueParamData.process_cli_option(collected_values)
 
     def get_control_method(
-        self, argument_type: Any, choices: Sequence[str] | None
+        self, param_type: Type[Any],
     ) -> Callable[[Any, Text, bool, OptionSchema | ArgumentSchema, str], Widget]:
-        if choices:
-            return partial(self.make_choice_control, choices=choices)
+        if isinstance(param_type, ChoiceSchema):
+            return partial(self.make_choice_control, choices=param_type.choices)
 
-        if argument_type is bool:
+        if param_type is bool:
             return self.make_checkbox_control
 
         return self.make_text_control
 
     @staticmethod
     def make_text_control(
         default: Any,
         label: Text | None,
         multiple: bool,
         schema: OptionSchema | ArgumentSchema,
         control_id: str,
     ) -> Widget:
         control = Input(
             classes=f"command-form-input {control_id}",
+            password=schema.secret,
+            disabled=schema.read_only,
+            placeholder=schema.placeholder,
         )
         yield control
         return control
 
     @staticmethod
     def make_checkbox_control(
         default: MultiValueParamData,
@@ -343,14 +365,18 @@
         default: MultiValueParamData,
         label: Text | None,
         multiple: bool,
         schema: OptionSchema | ArgumentSchema,
         control_id: str,
         choices: list[str],
     ) -> Widget:
+        # The MultipleChoice widget is only for single-valued parameters.
+        if schema.nargs != 1:
+            multiple = False
+
         if multiple:
             multi_choice = MultipleChoice(
                 choices,
                 classes=f"command-form-multiple-choice {control_id}",
                 defaults=default.values,
             )
             yield multi_choice
@@ -362,24 +388,24 @@
             )
             yield select
             return select
 
     @staticmethod
     def _make_command_form_control_label(
         name: str | list[str],
-        type: Type[Any],
+        types: list[Type[Any]],
         is_option: bool,
         is_required: bool,
         multiple: bool,
     ) -> Text:
         names: list[str] = [name] if isinstance(name, str) else name
 
         names = Text(" / ", style="dim").join([Text(n) for n in names])
         text = Text.from_markup(
-            f"{names}[dim]{' multiple' if multiple else ''} <{type.__name__}>[/] {' [b red]*[/]required' if is_required else ''}"
+            f"{names}[dim]{' multiple' if multiple else ''} <{', '.join(x.__name__ for x in types)}>[/] {' [b red]*[/]required' if is_required else ''}"
         )
 
         return text
 
     def focus(self, scroll_visible: bool = True):
         if self.first_control is not None:
             self.first_control.focus()
```

### Comparing `trogon_yapx-0.4.0.post1.dev1/PKG-INFO` & `trogon_yapx-0.5.0.dev0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: trogon-yapx
-Version: 0.4.0.post1.dev1
-Summary: Fork of Trogon for more compatibility
-Home-page: https://github.com/fresh2dev/trogon-yapx
+Version: 0.5.0.dev0
+Summary: Automatically generate a Textual TUI for your Python CLI
+Home-page: https://github.com/Textualize/trogon
 License: MIT
 Author: Donald Mellenbruch
 Author-email: hello@Fresh2.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -23,63 +23,70 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Provides-Extra: click
 Provides-Extra: typer
-Provides-Extra: yapx
 Requires-Dist: click (>=8.0.0) ; extra == "click"
 Requires-Dist: textual (>=0.26.0)
 Requires-Dist: typer (>=0.9.0) ; extra == "typer"
-Requires-Dist: yapx (>=0.1.0) ; extra == "yapx"
 Description-Content-Type: text/markdown
 
 
 <p align="center">
     <img src="https://github.com/Textualize/trogon/assets/554369/f4751783-c322-4143-a6c1-d8c564d4e38f" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
-
+    
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
-This fork of Trogon introduces these changes:
+---
+
+This is a fork of Trogon that introduces these features:
 
-- make `click` optional
-- add support for manually constructing schemas for the TUI
-- add support for `typer`
-- add support for `yapx`
-- remove support for sequences with differing types (e.g., click tuples)
-- remove support for custom click types, e.g., `IntRange`, `FloatRange`
+- refactor to make click optional
+- remove support for custom click types `IntRange`, `FloatRange`
+- support for manually constructing schemas
+- support for argparse
+- support for typer
+- add examples for yapx, myke, and sys.argv
+- support ommission of hidden parameters and subcommands from the TUI
+- support the redaction of sensitive "secret" values
+- support for showing required prompts as read-only
 - positional arguments come before keyword arguments in the generated command
 - ability to join list arguments values like this: `-x 1 -x 2 -x 3` (default), or like this: `-x 1 2 3`
+- vim-friendly keybindings
+
+I was motivated to create this fork so I could integrate Trogon into my Python CLI library [Yapx](https://www.f2dv.com/code/r/yapx/i/).
 
+---
 
 # Trogon
 
 Auto-generate friendly terminal user interfaces for command line apps.
 
 
-<details>
+<details>  
   <summary> 🎬 Video demonstration </summary>
 
 &nbsp;
-
+    
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
 https://github.com/Textualize/trogon/assets/554369/c9e5dabb-5624-45cb-8612-f6ecfde70362
 
 </details>
 
 
-Trogon works magically with the [Click](https://click.palletsprojects.com/) library for Python, and also with [Typer](https://github.com/tiangolo/typer) and [yapx](https://github.com/fresh2dev/yapx). You can even build it yourself and use `sys.argv`.
+Trogon works with the popular Python libraries [Argparse](https://docs.python.org/3/library/argparse.html), [Click](https://click.palletsprojects.com/), [Typer](https://github.com/tiangolo/typer), [Yapx](https://www.f2dv.com/code/r/yapx/i/), and [myke](https://www.f2dv.com/code/r/myke/i/), and will support other libraries and languages in the future. You can also manually build your own TUI schema and use it however you like, even in conjunction with `sys.argv`. See the `examples/` directory for examples of each.
 
 ## How it works
 
 Trogon inspects your (command line) app and extracts a *schema* which describes the options / switches / help etc.
-It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command.
+It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command. 
 
 Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps.
 This which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
@@ -133,23 +140,66 @@
 
 ```bash
 pip install trogon
 ```
 
 ## Quickstart
 
-1. Import `from trogon import tui`
+### Click
+
+1. Import `from trogon.click import tui`
 2. Add the `@tui` decorator above your click app. e.g.
     ```python
     @tui()
     @click.group(...)
     def cli():
         ...
     ```
 3. Your click app will have a new `tui` command available.
 
-See also the `examples` folder for two example apps.
+### Argparse
+
+1. Import `from trogon.argparse import add_tui_argument`
+      or, `from trogon.argparse import add_tui_command`
+2. Add the TUI argument/command to your argparse parser. e.g.
+    ```python
+    parser = argparse.ArgumentParser()
+
+    # add tui argument (my-cli --tui)
+    add_tui_argument(parser)
+    # and/or, add tui command (my-cli tui)
+    add_tui_command(parser)
+    ```
+3. Your argparse parser will have a new parameter `--tui` and/or a new command `tui`.
+
+See also the `examples` folder for example apps.
+
+## Custom command name and custom help
+
+By default the command added will be called `tui` and the help text for it will be `Open Textual TUI.`
+
+You can customize one or both of these using the `help=` and `command=` parameters.
+
+### Click
+
+```python
+@tui(command="ui", help="Open terminal UI")
+@click.group(...)
+def cli():
+    ...
+```
+
+### Argparse
+
+```python
+parser = argparse.ArgumentParser()
+
+# add tui argument (my-cli --tui)
+add_tui_argument(parser, option_strings=["--ui"], help="Open terminal UI")
+# and/or, add tui command (my-cli tui)
+add_tui_command(parser, command="ui", help="Open terminal UI")
+```
 
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr) where you can talk to Textual developers / community.
```

