# Comparing `tmp/udc-0.2.1.tar.gz` & `tmp/udc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.2.1.tar", max compression
+gzip compressed data, was "udc-0.2.2.tar", max compression
```

## Comparing `udc-0.2.1.tar` & `udc-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.1/LICENSE
--rw-r--r--   0        0        0     2529 2023-05-24 21:56:51.788254 udc-0.2.1/README.md
--rw-r--r--   0        0        0      749 2023-05-25 04:20:16.302097 udc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-24 21:56:51.803207 udc-0.2.1/udc/__init__.py
--rw-r--r--   0        0        0     5713 2023-05-24 21:56:51.803927 udc-0.2.1/udc/config.py
--rw-r--r--   0        0        0      716 2023-05-24 00:02:24.971861 udc-0.2.1/udc/ignore.py
--rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.1/udc/main.py
--rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.1/udc/types.py
--rw-r--r--   0        0        0     3455 2023-05-25 04:20:16.308758 udc-0.2.1/udc/un/un_cli.py
--rw-r--r--   0        0        0     2125 2023-05-24 21:56:51.806086 udc-0.2.1/udc/un/un_yaml.py
--rw-r--r--   0        0        0     1165 2023-05-24 21:56:51.806817 udc-0.2.1/udc/uri.py
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 udc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.2/README.md
+-rw-r--r--   0        0        0      749 2023-05-25 04:58:47.602247 udc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-24 21:56:51.803207 udc-0.2.2/udc/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-25 04:58:47.604193 udc-0.2.2/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     1234 2023-05-25 04:58:47.604548 udc-0.2.2/udc/benchling/entry.py
+-rw-r--r--   0        0        0     1518 2023-05-25 04:58:47.604868 udc-0.2.2/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2326 2023-05-25 04:58:47.605189 udc-0.2.2/udc/benchling/root.py
+-rw-r--r--   0        0        0      376 2023-05-25 04:58:47.605489 udc-0.2.2/udc/benchling/schema.py
+-rw-r--r--   0        0        0      372 2023-05-25 04:58:47.605787 udc-0.2.2/udc/benchling/sequence.py
+-rw-r--r--   0        0        0     5713 2023-05-24 21:56:51.803927 udc-0.2.2/udc/config.py
+-rw-r--r--   0        0        0      716 2023-05-24 00:02:24.971861 udc-0.2.2/udc/ignore.py
+-rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.2/udc/main.py
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.2/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-25 04:58:47.606461 udc-0.2.2/udc/quilt/resource.py
+-rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.2/udc/types.py
+-rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.2/udc/un/cli.yaml
+-rw-r--r--   0        0        0     3465 2023-05-25 04:58:47.607343 udc-0.2.2/udc/un/un_cli.py
+-rw-r--r--   0        0        0     2125 2023-05-24 21:56:51.806086 udc-0.2.2/udc/un/un_yaml.py
+-rw-r--r--   0        0        0     1165 2023-05-24 21:56:51.806817 udc-0.2.2/udc/uri.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 udc-0.2.2/PKG-INFO
```

### Comparing `udc-0.2.1/LICENSE` & `udc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.2.1/README.md` & `udc-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 Universal Data is an open source initiative to build a decentralized, cryptographically-secure ecosystem containerizing both structured and unstructured data.
 UDC is the initial (alpha) client for that system.
 
 ## Installation
 
 ### Production Package
 
-From PyPi (when published):
+From PyPi:
 
 <!--pytest.mark.skip-->
 ```bash
-python3 -m pip install --upgrade pip
-python3 -m pip install udc
+python3 -m pip install udc # OR
+python3 -m pip install --upgrade udc
+which udc
 ```
 
 ## Development Branch
 
 <!--pytest.mark.skip-->
 ```bash
 python3 -m pip install https://github.com/data-yaml/udc@main
```

### Comparing `udc-0.2.1/pyproject.toml` & `udc-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "udc"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 anyio = "^3.6.2"
```

### Comparing `udc-0.2.1/udc/config.py` & `udc-0.2.2/udc/config.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.1/udc/ignore.py` & `udc-0.2.2/udc/ignore.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.1/udc/un/un_cli.py` & `udc-0.2.2/udc/un/un_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 
 class UnCli(UnYaml):
     CLI_YAML = "cli.yaml"
     CMD = "commands"
 
     def __init__(self, file=CLI_YAML) -> None:
-        yaml_data = UnYaml.load_yaml(file, "tools")
+        yaml_data = UnYaml.load_yaml(file, "udc", "un")
         super().__init__(yaml_data)
         if UnCli.CMD not in self.cfg:
             raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.cfg}")
         self.cmds = self.get(UnCli.CMD)
 
     def cmd_opts(self, cmd: str) -> dict:
         result = self.cmds[cmd]
         result["name"] = cmd
         return result
 
     def parse_version(self, parser: ArgumentParser) -> None:
         __version__ = version('udc')
         parser.add_argument(
-            "--version",
+            "-v", "--version",
             action='store_const',
             const=f"{self.info('doc')} {__version__}",
             help="Show version and exit.",
         )
     def make_parser(self) -> ArgumentParser:
         parser = ArgumentParser(self.get("doc"))
         self.parse_version(parser)
```

### Comparing `udc-0.2.1/udc/un/un_yaml.py` & `udc-0.2.2/udc/un/un_yaml.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.1/udc/uri.py` & `udc-0.2.2/udc/uri.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.1/PKG-INFO` & `udc-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,20 +28,21 @@
 Universal Data is an open source initiative to build a decentralized, cryptographically-secure ecosystem containerizing both structured and unstructured data.
 UDC is the initial (alpha) client for that system.
 
 ## Installation
 
 ### Production Package
 
-From PyPi (when published):
+From PyPi:
 
 <!--pytest.mark.skip-->
 ```bash
-python3 -m pip install --upgrade pip
-python3 -m pip install udc
+python3 -m pip install udc # OR
+python3 -m pip install --upgrade udc
+which udc
 ```
 
 ## Development Branch
 
 <!--pytest.mark.skip-->
 ```bash
 python3 -m pip install https://github.com/data-yaml/udc@main
```

