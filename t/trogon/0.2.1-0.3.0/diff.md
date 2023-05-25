# Comparing `tmp/trogon-0.2.1.tar.gz` & `tmp/trogon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trogon-0.2.1.tar", max compression
+gzip compressed data, was "trogon-0.3.0.tar", max compression
```

## Comparing `trogon-0.2.1.tar` & `trogon-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     3541 2023-05-20 16:36:51.472017 trogon-0.2.1/README.md
--rw-r--r--   0        0        0     1379 2023-05-20 18:52:52.668873 trogon-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.2.1/trogon/__init__.py
--rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.2.1/trogon/constants.py
--rw-r--r--   0        0        0     6304 2023-05-20 10:29:22.256860 trogon-0.2.1/trogon/introspect.py
--rw-r--r--   0        0        0    11684 2023-05-20 18:52:48.934127 trogon-0.2.1/trogon/run_command.py
--rw-r--r--   0        0        0    10610 2023-05-20 18:52:48.934509 trogon-0.2.1/trogon/trogon.py
--rw-r--r--   0        0        0     3476 2023-05-20 16:34:18.421968 trogon-0.2.1/trogon/trogon.scss
--rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.2.1/trogon/widgets/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.2.1/trogon/widgets/about.py
--rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.2.1/trogon/widgets/command_info.py
--rw-r--r--   0        0        0     1985 2023-05-20 10:29:22.258561 trogon-0.2.1/trogon/widgets/command_tree.py
--rw-r--r--   0        0        0     7846 2023-05-20 10:29:22.258801 trogon-0.2.1/trogon/widgets/form.py
--rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.2.1/trogon/widgets/multiple_choice.py
--rw-r--r--   0        0        0    14891 2023-05-20 10:29:22.259311 trogon-0.2.1/trogon/widgets/parameter_controls.py
--rw-r--r--   0        0        0     5015 1970-01-01 00:00:00.000000 trogon-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3503 2023-05-25 14:54:56.303882 trogon-0.3.0/README.md
+-rw-r--r--   0        0        0     1380 2023-05-25 15:50:10.005159 trogon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.3.0/trogon/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.3.0/trogon/constants.py
+-rw-r--r--   0        0        0     1740 2023-05-25 15:45:10.256944 trogon-0.3.0/trogon/detect_run_string.py
+-rw-r--r--   0        0        0     6423 2023-05-25 14:54:56.305164 trogon-0.3.0/trogon/introspect.py
+-rw-r--r--   0        0        0     9544 2023-05-25 14:54:56.305692 trogon-0.3.0/trogon/run_command.py
+-rw-r--r--   0        0        0    10948 2023-05-25 15:45:10.257290 trogon-0.3.0/trogon/trogon.py
+-rw-r--r--   0        0        0     3535 2023-05-25 15:16:17.479145 trogon-0.3.0/trogon/trogon.scss
+-rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.3.0/trogon/widgets/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.3.0/trogon/widgets/about.py
+-rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.3.0/trogon/widgets/command_info.py
+-rw-r--r--   0        0        0     1811 2023-05-25 14:54:56.305972 trogon-0.3.0/trogon/widgets/command_tree.py
+-rw-r--r--   0        0        0     8097 2023-05-25 15:45:10.257586 trogon-0.3.0/trogon/widgets/form.py
+-rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.3.0/trogon/widgets/multiple_choice.py
+-rw-r--r--   0        0        0    16665 2023-05-25 15:16:17.479998 trogon-0.3.0/trogon/widgets/parameter_controls.py
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 trogon-0.3.0/PKG-INFO
```

### Comparing `trogon-0.2.1/README.md` & `trogon-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+
 <p align="center">
-    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
+    <img src="https://github.com/Textualize/trogon/assets/554369/f4751783-c322-4143-a6c1-d8c564d4e38f" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
     
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
 
 # Trogon
 
@@ -13,68 +14,66 @@
 <details>  
   <summary> 🎬 Video demonstration </summary>
 
 &nbsp;
     
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
-
-https://github.com/Textualize/trogon/assets/554369/5ad8de04-d9f9-45af-aa21-7cb593951eff
+https://github.com/Textualize/trogon/assets/554369/c9e5dabb-5624-45cb-8612-f6ecfde70362
 
 </details>
 
 
-Trogon works with the popular [Click](https://click.palletsprojects.com/) library for Python, but will support other libraries and even other languages in the future.
+Trogon works with the popular [Click](https://click.palletsprojects.com/) library for Python, but will support other libraries and languages in the future.
 
 ## How it works
 
-Trogon inspects your app and extracts a *schema* which describes the options / switches / help etc.
-It then uses that information to build a form with a familiar control for each option.
-Updating the form generates a command line which you can run with <kbd>ctrl+R</kbd>.
+Trogon inspects your (command line) app and extracts a *schema* which describes the options / switches / help etc.
+It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command. 
 
-Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
+Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps.
+This which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
-
 <table>
 
 <tr>
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 07 31" src="https://github.com/Textualize/trogon/assets/554369/7b67b9ae-d3e3-4e51-b13c-088bc99ad736">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 07 31" src="https://github.com/Textualize/trogon/assets/554369/009cf3f2-f0c4-464b-bd74-60e303864443">
 </td>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 08 21" src="https://github.com/Textualize/trogon/assets/554369/04245bad-4f76-453e-be25-c26d013474db">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 08 21" src="https://github.com/Textualize/trogon/assets/554369/b1039ee6-4ba6-4123-b0dd-aa7b2341672f">
 </td>
 </tr>
 
 <tr>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 08 53" src="https://github.com/Textualize/trogon/assets/554369/8b12fa2e-7d0c-4d21-bdc0-688408cf3cf6">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 08 53" src="https://github.com/Textualize/trogon/assets/554369/c0a42277-e946-4bef-b0d0-3fa87e4ab55b">
 </td>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 09 47" src="https://github.com/Textualize/trogon/assets/554369/c99d487a-7651-40e5-9bd5-7653e3be713a">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 09 47" src="https://github.com/Textualize/trogon/assets/554369/55477f6c-e6b8-49b6-85c1-b01bee006c8e">
 </td>
 
 </tr>
 
 </table>
 
 ## Why?
 
 Command line apps reward repeated use, but they lack in *discoverability*.
 If you don't use a CLI app frequently, or there are too many options to commit to memory, a Trogon TUI interface can help you (re)discover options and switches.
 
 ## What does the name mean?
 
-This project started life as a [Textual](https://github.com/Textualize/textual) experiement, which we have been giving give bird's names to.
+This project started life as a [Textual](https://github.com/Textualize/textual) experiment, which we have been giving give bird's names to.
 A [Trogon](https://www.willmcgugan.com/blog/photography/post/costa-rica-trip-report-2017/#bird) is a beautiful bird I was lucky enough to photograph in 2017.
 
 See also [Frogmouth](https://github.com/Textualize/frogmouth), a Markdown browser for the terminal.
 
 ## Roadmap
 
 Trogon is usable now. It is only 2 lines (!) of code to add to an existing project.
```

### Comparing `trogon-0.2.1/pyproject.toml` & `trogon-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "trogon"
-version = "0.2.1"
-description = "Automatically generate a Textual TUI for your Cick CLI"
+version = "0.3.0"
+description = "Automatically generate a Textual TUI for your Click CLI"
 authors = ["Darren Burns <darrenb900@gmail.com>"]
 readme = "README.md"
 packages = [{include = "trogon"}]
 license = "MIT"
 homepage = "https://github.com/Textualize/trogon"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `trogon-0.2.1/trogon/introspect.py` & `trogon-0.3.0/trogon/introspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,22 +33,22 @@
         return value
 
 
 @dataclass
 class OptionSchema:
     name: list[str]
     type: ParamType
-    default: MultiValueParamData
-    required: bool
-    is_flag: bool
-    is_boolean_flag: bool
-    flag_value: Any
-    opts: list
-    counting: bool
-    secondary_opts: list
+    default: MultiValueParamData | None = None
+    required: bool = False
+    is_flag: bool = False
+    is_boolean_flag: bool = False
+    flag_value: Any = ""
+    opts: list = field(default_factory=list)
+    counting: bool = False
+    secondary_opts: list = field(default_factory=list)
     key: str | tuple[str] = field(default_factory=generate_unique_id)
     help: str | None = None
     choices: Sequence[str] | None = None
     multiple: bool = False
     multi_value: bool = False
     nargs: int = 1
 
@@ -56,15 +56,15 @@
         self.multi_value = isinstance(self.type, click.Tuple)
 
 
 @dataclass
 class ArgumentSchema:
     name: str
     type: str
-    required: bool
+    required: bool = False
     key: str = field(default_factory=generate_unique_id)
     default: MultiValueParamData | None = None
     choices: Sequence[str] | None = None
     multiple: bool = False
     nargs: int = 1
```

### Comparing `trogon-0.2.1/trogon/run_command.py` & `trogon-0.3.0/trogon/run_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Attributes:
         name: The name of the argument.
         value: The user-provided value for the argument.
         argument_schema: The schema corresponding to this argument.
     """
 
     name: str
-    value: Any
+    value: tuple[Any]
     argument_schema: ArgumentSchema
 
 
 @dataclass
 class UserCommandData:
     """
     A dataclass to store user input for a command, its options, and arguments.
@@ -103,15 +103,19 @@
                 #  if they aren't equivalent to the default.
                 multiples[option.string_name].append(option.value)
                 multiples_schemas[option.string_name] = option.option_schema
             else:
                 value_data: list[tuple[Any]] = MultiValueParamData.process_cli_option(
                     option.value
                 ).values
-                default_data: list[tuple[Any]] = option.option_schema.default.values
+
+                if option.option_schema.default is not None:
+                    default_data: list[tuple[Any]] = option.option_schema.default.values
+                else:
+                    default_data = [tuple()]
 
                 flattened_values = sorted(itertools.chain.from_iterable(value_data))
                 flattened_defaults = sorted(itertools.chain.from_iterable(default_data))
 
                 # If the user has supplied values (any values are not None), then
                 # we don't display the value.
                 values_supplied = any(
@@ -163,15 +167,15 @@
                             # Get the value of the counting option
                             count = next(itertools.chain.from_iterable(value_data), 1)
                             try:
                                 count = int(count)
                             except ValueError:
                                 # TODO: Not sure if this is the right thing to do
                                 count = 1
-                            count = max(1, min(count, 3))
+                            count = max(1, min(count, 5))
                             if option_name.startswith("--"):
                                 args.extend([option_name] * count)
                             else:
                                 clean_option_name = option_name.lstrip("-")
                                 args.append(f"-{clean_option_name * count}")
 
         for option_name, values in multiples.items():
@@ -200,16 +204,16 @@
             if values_supplied and not values_are_defaults:
                 for value_data in values:
                     if not all(value == ValueNotSupplied() for value in value_data):
                         args.append(option_name)
                         args.extend(v for v in value_data)
 
         for argument in self.arguments:
-            value_data = argument.value
-            for argument_value in value_data:
+            this_arg_values = argument.value
+            for argument_value in this_arg_values:
                 if argument_value != ValueNotSupplied():
                     args.append(argument_value)
 
         if self.subcommand:
             args.extend(self.subcommand._to_cli_args())
 
         return args
@@ -228,62 +232,7 @@
         for arg in args:
             text_renderables.append(
                 Text(shlex.quote(str(arg)))
                 if arg != ValueNotSupplied()
                 else Text("???", style="bold black on red")
             )
         return Text(" ").join(text_renderables)
-
-    def fill_defaults(self, command_schema: CommandSchema) -> None:
-        """
-        Prefills the UserCommandData instance with default values for options and
-        arguments based on the provided CommandSchema.
-
-        Args:
-            command_schema: A CommandSchema instance representing the schema for
-                the command to prefill defaults.
-        """
-        # Prefill default option values
-        for option_schema in command_schema.options:
-            default = option_schema.default
-            if default is not None and not any(
-                opt.name == option_schema.name for opt in self.options
-            ):
-                # There's a separate UserOptionData instance for each instance of an
-                # option passed. So `--path . --path src` would be 2 UserOptionData
-                # objects. If multiple=True, there'll be many instances. If
-                # multiple=False, then we expect that only a single UserOptionData
-                # will be appended here.
-                for value in default.values:
-                    self.options.append(
-                        UserOptionData(
-                            name=option_schema.name,
-                            value=value,
-                            option_schema=option_schema,
-                        )
-                    )
-
-        # Prefill default argument values
-        for arg_schema in command_schema.arguments:
-            if arg_schema.default is not None and not any(
-                arg.name == arg_schema.name for arg in self.arguments
-            ):
-                self.arguments.append(
-                    UserArgumentData(
-                        name=arg_schema.name,
-                        value=arg_schema.default.values,
-                        argument_schema=arg_schema,
-                    )
-                )
-
-        # Prefill defaults for subcommand if present
-        if self.subcommand:
-            subcommand_schema = next(
-                (
-                    cmd
-                    for cmd in command_schema.subcommands.values()
-                    if cmd.name == self.subcommand.name
-                ),
-                None,
-            )
-            if subcommand_schema:
-                self.subcommand.fill_defaults(subcommand_schema)
```

### Comparing `trogon-0.2.1/trogon/trogon.py` & `trogon-0.3.0/trogon/trogon.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Label,
     Static,
     Button,
     Footer,
 )
 from textual.widgets.tree import TreeNode
 
+from trogon.detect_run_string import detect_run_string
 from trogon.introspect import (
     introspect_click_app,
     CommandSchema,
 )
 from trogon.run_command import UserCommandData
 from trogon.widgets.command_info import CommandInfo
 from trogon.widgets.command_tree import CommandTree
@@ -47,14 +48,19 @@
     BINDINGS = [
         Binding(key="ctrl+r", action="close_and_run", description="Close & Run"),
         Binding(
             key="ctrl+t", action="focus_command_tree", description="Focus Command Tree"
         ),
         Binding(key="ctrl+o", action="show_command_info", description="Command Info"),
         Binding(key="f1", action="about", description="About Trogon"),
+        Binding(
+            key="ctrl+s",
+            action="focus('search')",
+            description="Search",
+        ),
     ]
 
     def __init__(
         self,
         cli: click.BaseCommand,
         click_app_name: str,
         name: str | None = None,
@@ -219,15 +225,15 @@
     ) -> None:
         super().__init__()
         self.cli = cli
         self.post_run_command: list[str] = []
         self.is_grouped_cli = isinstance(cli, click.Group)
         self.execute_on_exit = False
         if app_name is None and click_context is not None:
-            self.app_name = click_context.find_root().info_name
+            self.app_name = detect_run_string()
         else:
             self.app_name = app_name
 
     def on_mount(self):
         self.push_screen(CommandBuilder(self.cli, self.app_name))
 
     @on(Button.Pressed, "#home-exec-button")
@@ -247,15 +253,19 @@
         finally:
             if self.post_run_command:
                 console = Console()
                 if self.post_run_command and self.execute_on_exit:
                     console.print(
                         f"Running [b cyan]{self.app_name} {' '.join(shlex.quote(s) for s in self.post_run_command)}[/]"
                     )
-                    os.execvp(self.app_name, [self.app_name, *self.post_run_command])
+
+                    split_app_name = shlex.split(self.app_name)
+                    program_name = shlex.split(self.app_name)[0]
+                    arguments = [*split_app_name, *self.post_run_command]
+                    os.execvp(program_name, arguments)
 
     @on(CommandForm.Changed)
     def update_command_to_run(self, event: CommandForm.Changed):
         include_root_command = not self.is_grouped_cli
         self.post_run_command = event.command_data.to_cli_args(include_root_command)
 
     def action_focus_command_tree(self) -> None:
```

### Comparing `trogon-0.2.1/trogon/trogon.scss` & `trogon-0.3.0/trogon/trogon.scss`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,18 @@
   align: center middle;
 }
 
 .command-info-header-text {
   padding: 1 1 0 2;
 }
 
+CommandForm .command-form-filter-input {
+  margin: 1 2;
+}
+
 $command-info-header-bg: $primary-darken-1;
 
 .command-info-header {
   dock: top;
   background: $command-info-header-bg;
   color: $text;
   height: auto;
```

### Comparing `trogon-0.2.1/trogon/widgets/about.py` & `trogon-0.3.0/trogon/widgets/about.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.1/trogon/widgets/command_info.py` & `trogon-0.3.0/trogon/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.1/trogon/widgets/command_tree.py` & `trogon-0.3.0/trogon/widgets/command_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from rich.style import Style
 from rich.text import TextType, Text
-from textual.geometry import clamp
 from textual.widgets import Tree
 from textual.widgets._tree import TreeNode, TreeDataType
 
 from trogon.introspect import CommandSchema, CommandName
 
 
 class CommandTree(Tree[CommandSchema]):
@@ -28,19 +27,15 @@
 
     def on_mount(self):
         def build_tree(
             data: dict[CommandName, CommandSchema], node: TreeNode
         ) -> TreeNode:
             data = {key: data[key] for key in sorted(data)}
             for cmd_name, cmd_data in data.items():
-                if (
-                    not cmd_data.subcommands
-                    and not cmd_data.options
-                    and not cmd_data.arguments
-                ):
+                if cmd_name == "tui":
                     continue
                 if cmd_data.subcommands:
                     label = Text(cmd_name)
                     if cmd_data.is_group:
                         group_style = self.get_component_rich_style("group")
                         label.stylize(group_style)
                         label.append(" ")
```

### Comparing `trogon-0.2.1/trogon/widgets/form.py` & `trogon-0.3.0/trogon/widgets/form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import dataclasses
 
+from textual import on
 from textual.app import ComposeResult
 from textual.containers import VerticalScroll, Vertical
 from textual.message import Message
 from textual.widget import Widget
-from textual.widgets import Label
+from textual.widgets import Label, Input
 
 from trogon.introspect import (
     CommandSchema,
     CommandName,
     ArgumentSchema,
     OptionSchema,
 )
@@ -98,19 +99,28 @@
         self.first_control: ParameterControls | None = None
 
     def compose(self) -> ComposeResult:
         path_from_root = iter(reversed(self.command_schema.path_from_root))
         command_node = next(path_from_root)
         with VerticalScroll() as vs:
             vs.can_focus = False
+
+            yield Input(
+                placeholder="Search...",
+                classes="command-form-filter-input",
+                id="search",
+            )
+
             while command_node is not None:
                 options = command_node.options
                 arguments = command_node.arguments
                 if options or arguments:
-                    with Vertical(classes="command-form-command-group") as v:
+                    with Vertical(
+                        classes="command-form-command-group", id=command_node.key
+                    ) as v:
                         is_inherited = command_node is not self.command_schema
                         v.border_title = (
                             f"{'↪ ' if is_inherited else ''}{command_node.name}"
                         )
                         if is_inherited:
                             v.border_title += " [dim not bold](inherited)"
                         if arguments:
@@ -155,60 +165,60 @@
 
         # Sentinel root value to make constructing the tree a little easier.
         parent_command_data = UserCommandData(
             name=CommandName("_"), options=[], arguments=[]
         )
 
         root_command_data = parent_command_data
-        try:
-            for command in path_from_root:
-                option_datas = []
-                # For each of the options in the schema for this command,
-                # lets grab the values the user has supplied for them in the form.
-                for option in command.options:
-                    parameter_control = self.query_one(
-                        f"#{option.key}", ParameterControls
-                    )
-                    value = parameter_control.get_values()
-                    for v in value.values:
-                        assert isinstance(v, tuple)
-                        option_data = UserOptionData(option.name, v, option)
-                        option_datas.append(option_data)
-
-                # Now do the same for the arguments
-                argument_datas = []
-                for argument in command.arguments:
-                    form_control_widget = self.query_one(
-                        f"#{argument.key}", ParameterControls
-                    )
-                    value = form_control_widget.get_values()
-                    # This should only ever loop once since arguments can be multi-value but not multiple=True.
-                    for v in value.values:
-                        assert isinstance(v, tuple)
-                        argument_data = UserArgumentData(argument.name, v, argument)
-                        argument_datas.append(argument_data)
-
-                assert all(isinstance(option.value, tuple) for option in option_datas)
-                assert all(
-                    isinstance(argument.value, tuple) for argument in argument_datas
+        for command in path_from_root:
+            option_datas = []
+            # For each of the options in the schema for this command,
+            # lets grab the values the user has supplied for them in the form.
+            for option in command.options:
+                parameter_control = self.query_one(f"#{option.key}", ParameterControls)
+                value = parameter_control.get_values()
+                for v in value.values:
+                    assert isinstance(v, tuple)
+                    option_data = UserOptionData(option.name, v, option)
+                    option_datas.append(option_data)
+
+            # Now do the same for the arguments
+            argument_datas = []
+            for argument in command.arguments:
+                form_control_widget = self.query_one(
+                    f"#{argument.key}", ParameterControls
                 )
-                command_data = UserCommandData(
-                    name=command.name,
-                    options=option_datas,
-                    arguments=argument_datas,
-                    parent=parent_command_data,
-                    command_schema=command,
-                )
-                parent_command_data.subcommand = command_data
-                parent_command_data = command_data
-        except Exception as e:
-            raise e
+                value = form_control_widget.get_values()
+                # This should only ever loop once since arguments can be multi-value but not multiple=True.
+                for v in value.values:
+                    assert isinstance(v, tuple)
+                    argument_data = UserArgumentData(argument.name, v, argument)
+                    argument_datas.append(argument_data)
+
+            assert all(isinstance(option.value, tuple) for option in option_datas)
+            assert all(isinstance(argument.value, tuple) for argument in argument_datas)
+            command_data = UserCommandData(
+                name=command.name,
+                options=option_datas,
+                arguments=argument_datas,
+                parent=parent_command_data,
+                command_schema=command,
+            )
+            parent_command_data.subcommand = command_data
+            parent_command_data = command_data
 
         # Trim the sentinel
         root_command_data = root_command_data.subcommand
         root_command_data.parent = None
-        root_command_data.fill_defaults(self.command_schema)
         self.post_message(self.Changed(root_command_data))
 
     def focus(self, scroll_visible: bool = True):
         if self.first_control is not None:
             return self.first_control.focus()
+
+    @on(Input.Changed, ".command-form-filter-input")
+    def apply_filter(self, event: Input.Changed) -> None:
+        filter_query = event.value
+        all_controls = self.query(ParameterControls)
+        for control in all_controls:
+            filter_query = filter_query.casefold()
+            control.apply_filter(filter_query)
```

### Comparing `trogon-0.2.1/trogon/widgets/multiple_choice.py` & `trogon-0.3.0/trogon/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.1/trogon/widgets/parameter_controls.py` & `trogon-0.3.0/trogon/widgets/parameter_controls.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Callable, Iterable, TypeVar, Union, cast
 
 import click
 from rich.text import Text
 from textual import log, on
 from textual.app import ComposeResult
 from textual.containers import Vertical, Horizontal
+from textual.css.query import NoMatches
 from textual.widget import Widget
 from textual.widgets import (
     RadioButton,
     Label,
     Checkbox,
     Input,
     Select,
@@ -38,38 +39,81 @@
 class ValueNotSupplied:
     def __eq__(self, other):
         return isinstance(other, ValueNotSupplied)
 
     def __lt__(self, other):
         return False
 
+    def __bool__(self):
+        return False
+
 
 class ParameterControls(Widget):
     def __init__(
         self,
         schema: ArgumentSchema | OptionSchema,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
     ) -> None:
         super().__init__(name=name, id=id, classes=classes, disabled=disabled)
         self.schema = schema
         self.first_control: Widget | None = None
 
+    def apply_filter(self, filter_query: str) -> bool:
+        """Show or hide this ParameterControls depending on whether it matches the filter query or not.
+
+        Args:
+            filter_query: The string to filter on.
+
+        Returns:
+            True if the filter matched (and the widget is visible).
+        """
+        help_text = getattr(self.schema, "help", "")
+        if not filter_query:
+            should_be_visible = True
+            self.display = should_be_visible
+        else:
+            name = self.schema.name
+            if isinstance(name, str):
+                # Argument names are strings, there's only one name
+                name_contains_query = filter_query in name.casefold()
+                should_be_visible = name_contains_query
+            else:
+                # Option names are lists since they can have multiple names (e.g. -v and --verbose)
+                name_contains_query = any(filter_query in name.casefold() for name in self.schema.name)
+                help_contains_query = filter_query in getattr(self.schema, "help", "").casefold()
+                should_be_visible = name_contains_query or help_contains_query
+
+            self.display = should_be_visible
+
+        # Update the highlighting of the help text
+        if help_text:
+            try:
+                help_label = self.query_one(".command-form-control-help-text", Static)
+                new_help_text = Text(help_text)
+                new_help_text.highlight_words(filter_query.split(), "black on yellow", case_sensitive=False)
+                help_label.update(new_help_text)
+            except NoMatches:
+                pass
+
+        return should_be_visible
+
     def compose(self) -> ComposeResult:
         """Takes the schemas for each parameter of the current command, and converts it into a
         form consisting of Textual widgets."""
         schema = self.schema
         name = schema.name
         argument_type = schema.type
         default = schema.default
         help_text = getattr(schema, "help", "") or ""
         multiple = schema.multiple
         is_option = isinstance(schema, OptionSchema)
+        nargs = schema.nargs
 
         label = self._make_command_form_control_label(
             name, argument_type, is_option, schema.required, multiple=multiple
         )
         first_focus_control: Widget | None = (
             None  # The widget that will be focused when the form is focused.
         )
@@ -133,15 +177,15 @@
         # Take note of the first form control, so we can easily focus it
         if self.first_control is None:
             self.first_control = first_focus_control
 
         # If it's a multiple, and it's a Choice parameter, then we display
         # our special case MultiChoice widget, and so there's no need for this
         # button.
-        if multiple and not isinstance(argument_type, click.Choice):
+        if multiple or nargs == -1 and not isinstance(argument_type, click.Choice):
             with Horizontal(classes="add-another-button-container"):
                 yield Button("+ value", variant="primary", classes="add-another-button")
 
         # Render the dim help text below the form controls
         if help_text:
             yield Static(help_text, classes="command-form-control-help-text")
 
@@ -221,15 +265,15 @@
         ) -> list[tuple[int | float | str, ...]]:
             if tuple_size == 0:
                 return [tuple()]
             elif tuple_size == -1:
                 # Unspecified number of arguments as per Click docs.
                 tuple_size = 1
             return [
-                tuple(lst[i : i + tuple_size]) for i in range(0, len(lst), tuple_size)
+                tuple(lst[i: i + tuple_size]) for i in range(0, len(lst), tuple_size)
             ]
 
         controls = list(self.query(f".{self.schema.key}"))
 
         if len(controls) == 1 and isinstance(controls[0], MultipleChoice):
             # Since MultipleChoice widgets are a special case that appear in
             # isolation, our logic to fetch the values out of them is slightly
@@ -277,17 +321,15 @@
         if is_text_type:
             return self.make_text_control
         elif argument_type == click.BOOL:
             return self.make_checkbox_control
         elif isinstance(argument_type, click.types.Choice):
             return partial(self.make_choice_control, choices=argument_type.choices)
         else:
-            log.error(
-                f"Given type {argument_type}, we couldn't determine which form control to render."
-            )
+            return self.make_text_control
 
     @staticmethod
     def make_text_control(
         default: Any,
         label: Text | None,
         multiple: bool,
         schema: OptionSchema | ArgumentSchema,
@@ -305,14 +347,16 @@
         label: Text | None,
         multiple: bool,
         schema: OptionSchema | ArgumentSchema,
         control_id: str,
     ) -> Widget:
         if default.values:
             default = default.values[0][0]
+        else:
+            default = ValueNotSupplied()
 
         control = Checkbox(
             label,
             button_first=True,
             classes=f"command-form-checkbox {control_id}",
             value=default,
         )
```

### Comparing `trogon-0.2.1/PKG-INFO` & `trogon-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: trogon
-Version: 0.2.1
-Summary: Automatically generate a Textual TUI for your Cick CLI
+Version: 0.3.0
+Summary: Automatically generate a Textual TUI for your Click CLI
 Home-page: https://github.com/Textualize/trogon
 License: MIT
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -29,16 +29,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: textual (>=0.26.0)
 Description-Content-Type: text/markdown
 
+
 <p align="center">
-    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
+    <img src="https://github.com/Textualize/trogon/assets/554369/f4751783-c322-4143-a6c1-d8c564d4e38f" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
     
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
 
 # Trogon
 
@@ -48,68 +49,66 @@
 <details>  
   <summary> 🎬 Video demonstration </summary>
 
 &nbsp;
     
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
-
-https://github.com/Textualize/trogon/assets/554369/5ad8de04-d9f9-45af-aa21-7cb593951eff
+https://github.com/Textualize/trogon/assets/554369/c9e5dabb-5624-45cb-8612-f6ecfde70362
 
 </details>
 
 
-Trogon works with the popular [Click](https://click.palletsprojects.com/) library for Python, but will support other libraries and even other languages in the future.
+Trogon works with the popular [Click](https://click.palletsprojects.com/) library for Python, but will support other libraries and languages in the future.
 
 ## How it works
 
-Trogon inspects your app and extracts a *schema* which describes the options / switches / help etc.
-It then uses that information to build a form with a familiar control for each option.
-Updating the form generates a command line which you can run with <kbd>ctrl+R</kbd>.
+Trogon inspects your (command line) app and extracts a *schema* which describes the options / switches / help etc.
+It then uses that information to build a [Textual](https://github.com/textualize/textual) UI you can use to edit and run the command. 
 
-Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
+Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps.
+This which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
-
 <table>
 
 <tr>
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 07 31" src="https://github.com/Textualize/trogon/assets/554369/7b67b9ae-d3e3-4e51-b13c-088bc99ad736">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 07 31" src="https://github.com/Textualize/trogon/assets/554369/009cf3f2-f0c4-464b-bd74-60e303864443">
 </td>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 08 21" src="https://github.com/Textualize/trogon/assets/554369/04245bad-4f76-453e-be25-c26d013474db">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 08 21" src="https://github.com/Textualize/trogon/assets/554369/b1039ee6-4ba6-4123-b0dd-aa7b2341672f">
 </td>
 </tr>
 
 <tr>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 08 53" src="https://github.com/Textualize/trogon/assets/554369/8b12fa2e-7d0c-4d21-bdc0-688408cf3cf6">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 08 53" src="https://github.com/Textualize/trogon/assets/554369/c0a42277-e946-4bef-b0d0-3fa87e4ab55b">
 </td>
 
 <td>
-<img width="100%" alt="Screenshot 2023-05-20 at 12 09 47" src="https://github.com/Textualize/trogon/assets/554369/c99d487a-7651-40e5-9bd5-7653e3be713a">
+<img width="100%" alt="Screenshot 2023-05-20 at 12 09 47" src="https://github.com/Textualize/trogon/assets/554369/55477f6c-e6b8-49b6-85c1-b01bee006c8e">
 </td>
 
 </tr>
 
 </table>
 
 ## Why?
 
 Command line apps reward repeated use, but they lack in *discoverability*.
 If you don't use a CLI app frequently, or there are too many options to commit to memory, a Trogon TUI interface can help you (re)discover options and switches.
 
 ## What does the name mean?
 
-This project started life as a [Textual](https://github.com/Textualize/textual) experiement, which we have been giving give bird's names to.
+This project started life as a [Textual](https://github.com/Textualize/textual) experiment, which we have been giving give bird's names to.
 A [Trogon](https://www.willmcgugan.com/blog/photography/post/costa-rica-trip-report-2017/#bird) is a beautiful bird I was lucky enough to photograph in 2017.
 
 See also [Frogmouth](https://github.com/Textualize/frogmouth), a Markdown browser for the terminal.
 
 ## Roadmap
 
 Trogon is usable now. It is only 2 lines (!) of code to add to an existing project.
```

