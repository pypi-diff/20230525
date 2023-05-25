# Comparing `tmp/pipen_args-0.9.7.tar.gz` & `tmp/pipen_args-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.9.7.tar", max compression
+gzip compressed data, was "pipen_args-0.9.8.tar", max compression
```

## Comparing `pipen_args-0.9.7.tar` & `pipen_args-0.9.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2172 2023-04-18 06:25:41.328574 pipen_args-0.9.7/README.md
--rw-r--r--   0        0        0      969 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/__init__.py
--rw-r--r--   0        0        0     3871 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/defaults.py
--rw-r--r--   0        0        0     9934 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/parser_.py
--rw-r--r--   0        0        0     8053 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/plugin.py
--rw-r--r--   0        0        0     3277 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/version.py
--rw-r--r--   0        0        0     1185 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 pipen_args-0.9.7/setup.py
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 pipen_args-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     2560 2023-05-25 05:33:52.478197 pipen_args-0.9.8/README.md
+-rw-r--r--   0        0        0      969 2023-05-25 05:33:52.478197 pipen_args-0.9.8/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3871 2023-05-25 05:33:52.478197 pipen_args-0.9.8/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9821 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/parser_.py
+-rw-r--r--   0        0        0     8133 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-05-25 05:33:52.482197 pipen_args-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 pipen_args-0.9.8/setup.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 pipen_args-0.9.8/PKG-INFO
```

### Comparing `pipen_args-0.9.7/README.md` & `pipen_args-0.9.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,21 @@
 Optional Arguments:
   -h, --help, -h+, --help+
                         show help message (with + to show more options) and exit
 ```
 
 See more examples in `tests/pipelines/` folder.
 
+## Plugin options
+
+- `args_hide`: (process level) Hide the arguments in the help message. Default: `False`
+- `args_group`: (pipeline level) The group name for the arguments. Default: `pipeline options`
+- `args_flatten`: (pipeline level) Flatten the arguments in the help message when there is only one process in the pipeline. Default: `auto` (flatten if single process, otherwise not)
+
+
 ## Metadata for Proc envs items
 
 The metadata in the docstring of env items determines how the arguments are defined.
 
 ```python
 class Process(Proc):
     """My process
```

### Comparing `pipen_args-0.9.7/pipen_args/__init__.py` & `pipen_args-0.9.8/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.7/pipen_args/defaults.py` & `pipen_args-0.9.8/pipen_args/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.7/pipen_args/parser_.py` & `pipen_args-0.9.8/pipen_args/parser_.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,40 +32,26 @@
         if cls._INST is None:
             cls._INST = super().__call__(*args, **kwds)
 
         return cls._INST
 
 
 class Parser(ArgumentParser, metaclass=ParserMeta):
-    """Subclass of Params to fit for pipen
+    """Subclass of Params to fit for pipen"""
 
-    Args:
-        pipeline_args_group: The group name to gather all the parameters on
-            help page
-        flatten_proc_args: Flatten process arguments to the top level
-    """
-    def __init__(
-        self,
-        *args,
-        pipeline_args_group: str = PIPELINE_ARGS_GROUP,
-        flatten_proc_args: bool | str = FLATTEN_PROC_ARGS,
-        **kwargs,
-    ) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         """Constructor"""
         kwargs["add_help"] = "+"
         kwargs["fromfile_prefix_chars"] = "@"
         kwargs["usage"] = "%(prog)s [-h | -h+] [options]"
         super().__init__(*args, **kwargs)
 
-        self.flatten_proc_args = flatten_proc_args
+        self.flatten_proc_args = None
         self._cli_args = None
-        self._pipeline_args_group = self.add_argument_group(
-            pipeline_args_group,
-            order=-99,
-        )
+        self._pipeline_args_group = None
         self._parsed = None
 
     def set_cli_args(self, args: Any) -> None:
         """Set cli arguments, allows externals to set arguments to parse"""
         self._cli_args = args
 
     def parse_args(self, args: Any = None, namespace: Any = None) -> Namespace:
@@ -78,14 +64,24 @@
                 args = self._cli_args
 
             self._parsed = super().parse_args(args, namespace)
         return self._parsed
 
     def init(self, pipen: Pipen) -> None:
         """Define arguments"""
+
+        self._pipeline_args_group = self.add_argument_group(
+            pipen._kwargs["plugin_opts"].get("args_group", PIPELINE_ARGS_GROUP),
+            order=-99,
+        )
+        self.flatten_proc_args = pipen._kwargs["plugin_opts"].get(
+            "args_flatten",
+            FLATTEN_PROC_ARGS,
+        )
+
         pipen.build_proc_relationships()
         if len(pipen.procs) > 1 and self.flatten_proc_args is True:
             raise ValueError(  # pragma: no cover
                 "Cannot flatten process arguments for multiprocess pipeline."
             )
 
         if self.flatten_proc_args == "auto":
@@ -102,19 +98,19 @@
                 argopt["default"] = pipen.outdir
             elif arg == "name":
                 argopt["default"] = pipen.name
 
             if arg in ("scheduler_opts", "plugin_opts"):
                 if self.flatten_proc_args:
                     argopt["default"] = (
-                        Diot(pipen.config.get(arg, None) or {})
+                        Diot(pipen._kwargs.get(arg, None) or {})
                         | (getattr(pipen.procs[0], arg, None) or {})
                     )
                 else:
-                    argopt["default"] = pipen.config.get(arg, None) or {}
+                    argopt["default"] = pipen._kwargs.get(arg, None) or {}
 
             self._pipeline_args_group.add_argument(f"--{arg}", **argopt)
 
         if self.flatten_proc_args is True:
             self._add_proc_args(
                 pipen.procs[0],
                 is_start=True,
```

### Comparing `pipen_args-0.9.7/pipen_args/plugin.py` & `pipen_args-0.9.8/pipen_args/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from argx import Namespace
 from simpleconf import ProfileConfig
 from pipen import plugin
 from pipen.defaults import CONFIG_FILES
 from pipen.utils import copy_dict, get_logger
 
 from .version import __version__
+from .defaults import FLATTEN_PROC_ARGS
 from .parser_ import Parser
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Pipen
 
 logger = get_logger("args", "info")
 # Save the warnings to print them after the pipeline is initialized
@@ -26,17 +27,16 @@
     """Automatically parse arguments and load configs for pipen pipelines"""
     name = "args"
     version = __version__
 
     @plugin.impl
     async def on_init(pipen: Pipen) -> None:
         """Parse and update the config"""
-        config = pipen.config
-        config.plugin_opts.args_hide = False
-
+        config = pipen._kwargs
+        config["plugin_opts"]["args_hide"] = False
         parser = Parser()
         # Init the parser
         try:
             parser.init(pipen)
         except ArgumentError:
             # The parser is initialized in another pipeline
             raise ValueError(
@@ -78,15 +78,17 @@
                 config[key] = getattr(parsed, key)
 
         # The original name
         pipen_name = pipen.name
         # The default outdir
         pipen_outdir = Path(f"./{pipen_name}-output").resolve()
         # The default workdir
-        pipen_workdir = Path(f"./{config['workdir']}/{pipen_name}").resolve()
+        pipen_workdir = Path(
+            f"./{pipen.config['workdir']}/{pipen_name}"
+        ).resolve()
 
         # Update the name
         if parsed.name not in (None, pipen_name):
             pipen.name = parsed.name
 
         # Update the outdir
         if pipen.outdir in (None, pipen_outdir):
@@ -116,15 +118,15 @@
             # by higher priority (Pipen.workdir, or Pipen(workdir=...))
             # So we can use the value from arguments
             if parsed.workdir is not None:
                 # If it is passed by arguments, use it
                 workdir = parsed.workdir
             else:
                 # Otherwise, use the name to infer the workdir
-                workdir = Path(config['workdir'])
+                workdir = Path(pipen.config['workdir'])
             pipen.workdir = workdir.joinpath(pipen.name).resolve()
             pipen.workdir.mkdir(parents=True, exist_ok=True)
         elif parsed.workdir is not None and parsed.workdir != pipen.workdir:
             # The workdir is set by higher priority, and a value is passed by
             # arguments, so we need to warn the user that the value from
             # arguments will be ignored
             warns.append(
```

### Comparing `pipen_args-0.9.7/pipen_args/procgroup.py` & `pipen_args-0.9.8/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.7/pyproject.toml` & `pipen_args-0.9.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.9.7"
+version = "0.9.8"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
```

### Comparing `pipen_args-0.9.7/setup.py` & `pipen_args-0.9.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pipen-annotate>=0.7.1,<0.8.0']
 
 entry_points = \
 {'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'Command-line argument parser for pipen.',
-    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Plugin options\n\n- `args_hide`: (process level) Hide the arguments in the help message. Default: `False`\n- `args_group`: (pipeline level) The group name for the arguments. Default: `pipeline options`\n- `args_flatten`: (pipeline level) Flatten the arguments in the help message when there is only one process in the pipeline. Default: `auto` (flatten if single process, otherwise not)\n\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pipen_args-0.9.7/PKG-INFO` & `pipen_args-0.9.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.9.7
+Version: 0.9.8
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -65,14 +65,21 @@
 Optional Arguments:
   -h, --help, -h+, --help+
                         show help message (with + to show more options) and exit
 ```
 
 See more examples in `tests/pipelines/` folder.
 
+## Plugin options
+
+- `args_hide`: (process level) Hide the arguments in the help message. Default: `False`
+- `args_group`: (pipeline level) The group name for the arguments. Default: `pipeline options`
+- `args_flatten`: (pipeline level) Flatten the arguments in the help message when there is only one process in the pipeline. Default: `auto` (flatten if single process, otherwise not)
+
+
 ## Metadata for Proc envs items
 
 The metadata in the docstring of env items determines how the arguments are defined.
 
 ```python
 class Process(Proc):
     """My process
```

