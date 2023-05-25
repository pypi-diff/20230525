# Comparing `tmp/udc-0.2.0.tar.gz` & `tmp/udc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.2.0.tar", max compression
+gzip compressed data, was "udc-0.2.1.tar", max compression
```

## Comparing `udc-0.2.0.tar` & `udc-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.0/LICENSE
--rw-r--r--   0        0        0     2529 2023-05-24 21:56:51.788254 udc-0.2.0/README.md
--rw-r--r--   0        0        0      749 2023-05-24 21:56:51.791340 udc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-24 21:56:51.803207 udc-0.2.0/udc/__init__.py
--rw-r--r--   0        0        0     5713 2023-05-24 21:56:51.803927 udc-0.2.0/udc/config.py
--rw-r--r--   0        0        0      716 2023-05-24 00:02:24.971861 udc-0.2.0/udc/ignore.py
--rw-r--r--   0        0        0      337 2023-05-24 21:56:51.804600 udc-0.2.0/udc/main.py
--rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.0/udc/types.py
--rw-r--r--   0        0        0     2893 2023-05-24 21:56:51.805417 udc-0.2.0/udc/un/un_cli.py
--rw-r--r--   0        0        0     2125 2023-05-24 21:56:51.806086 udc-0.2.0/udc/un/un_yaml.py
--rw-r--r--   0        0        0     1165 2023-05-24 21:56:51.806817 udc-0.2.0/udc/uri.py
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 udc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2529 2023-05-24 21:56:51.788254 udc-0.2.1/README.md
+-rw-r--r--   0        0        0      749 2023-05-25 04:20:16.302097 udc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-24 21:56:51.803207 udc-0.2.1/udc/__init__.py
+-rw-r--r--   0        0        0     5713 2023-05-24 21:56:51.803927 udc-0.2.1/udc/config.py
+-rw-r--r--   0        0        0      716 2023-05-24 00:02:24.971861 udc-0.2.1/udc/ignore.py
+-rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.1/udc/main.py
+-rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.1/udc/types.py
+-rw-r--r--   0        0        0     3455 2023-05-25 04:20:16.308758 udc-0.2.1/udc/un/un_cli.py
+-rw-r--r--   0        0        0     2125 2023-05-24 21:56:51.806086 udc-0.2.1/udc/un/un_yaml.py
+-rw-r--r--   0        0        0     1165 2023-05-24 21:56:51.806817 udc-0.2.1/udc/uri.py
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 udc-0.2.1/PKG-INFO
```

### Comparing `udc-0.2.0/LICENSE` & `udc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/README.md` & `udc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/pyproject.toml` & `udc-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "udc"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 anyio = "^3.6.2"
 trio = "^0.22.0"
 asyncclick = "^8.1.3.4"
 quilt3 = "^5.3.1"
 urllib3 = "<2"
 typing-extensions = "^4.5.0"
-quiltplus = "^0.8.1"
+quiltplus = "~0.8.1"
 #  quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "main"}
 benchling-sdk = "^1.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
```

### Comparing `udc-0.2.0/udc/config.py` & `udc-0.2.1/udc/config.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/udc/ignore.py` & `udc-0.2.1/udc/ignore.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/udc/un/un_cli.py` & `udc-0.2.1/udc/un/un_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from collections.abc import Sequence
+from importlib.metadata import version
 from sys import stdout
 
+__version__ = version('udc')
+
 from ..types import Listable
 from ..uri import UdcUri
 from .un_yaml import UnYaml
 
 
 class UnCli(UnYaml):
     CLI_YAML = "cli.yaml"
@@ -20,35 +23,49 @@
         self.cmds = self.get(UnCli.CMD)
 
     def cmd_opts(self, cmd: str) -> dict:
         result = self.cmds[cmd]
         result["name"] = cmd
         return result
 
+    def parse_version(self, parser: ArgumentParser) -> None:
+        __version__ = version('udc')
+        parser.add_argument(
+            "--version",
+            action='store_const',
+            const=f"{self.info('doc')} {__version__}",
+            help="Show version and exit.",
+        )
     def make_parser(self) -> ArgumentParser:
         parser = ArgumentParser(self.get("doc"))
+        self.parse_version(parser)
         subparsers = parser.add_subparsers(dest="command")
         for cmd, opts in self.cmds.items():
             if cmd != "list": continue
             subparser = subparsers.add_parser(cmd, help=opts["help"])
             args = opts.get("arguments")
             for arg in args or []:
                 subparser.add_argument(arg["name"], help=arg["help"])
         return parser
 
     async def run(self, argv: Sequence[str] = None, out=stdout):
         args = self.parse(argv)
+        if not args:
+            return False
+        if args.version:
+            print(args.version, file=out)
+            return False
         return await self.execute(args, out)
 
     def parse(self, argv: Sequence[str] = None) -> dict:
         parser = self.make_parser()
         args = parser.parse_args(argv)
-        if args.command is None:
+        if args.command is None and not args.version:
             parser.print_help()
-            exit(0)
+            return False
         return args
 
     async def execute(self, args: Namespace, out=stdout):
         """Invoke Appropriate Command."""
         cmd = args.command
         opts = self.cmd_opts(cmd)
         if not opts:
```

### Comparing `udc-0.2.0/udc/un/un_yaml.py` & `udc-0.2.1/udc/un/un_yaml.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/udc/uri.py` & `udc-0.2.1/udc/uri.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.0/PKG-INFO` & `udc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

