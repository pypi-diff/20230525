# Comparing `tmp/zntrack-0.6.0a4.tar.gz` & `tmp/zntrack-0.6.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zntrack-0.6.0a4.tar", max compression
+gzip compressed data, was "zntrack-0.6.0a5.tar", max compression
```

## Comparing `zntrack-0.6.0a4.tar` & `zntrack-0.6.0a5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.0a4/LICENSE
--rw-r--r--   0        0        0     5910 2023-02-27 09:22:05.852929 zntrack-0.6.0a4/README.md
--rw-r--r--   0        0        0     2289 2023-04-05 10:57:41.012663 zntrack-0.6.0a4/pyproject.toml
--rw-r--r--   0        0        0      715 2023-03-28 15:55:39.672257 zntrack-0.6.0a4/zntrack/__init__.py
--rw-r--r--   0        0        0     2686 2023-04-05 10:57:41.022663 zntrack-0.6.0a4/zntrack/cli/__init__.py
--rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.0a4/zntrack/core/__init__.py
--rw-r--r--   0        0        0    10646 2023-04-05 10:56:52.273202 zntrack-0.6.0a4/zntrack/core/node.py
--rw-r--r--   0        0        0    14022 2023-03-16 14:38:52.672721 zntrack-0.6.0a4/zntrack/core/nodify.py
--rw-r--r--   0        0        0     1386 2023-04-05 10:56:52.283202 zntrack-0.6.0a4/zntrack/exceptions/__init__.py
--rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.0a4/zntrack/fields/__init__.py
--rw-r--r--   0        0        0     5036 2023-03-28 20:19:28.007503 zntrack-0.6.0a4/zntrack/fields/dvc/__init__.py
--rw-r--r--   0        0        0     5580 2023-04-04 15:56:57.182464 zntrack-0.6.0a4/zntrack/fields/field.py
--rw-r--r--   0        0        0     3313 2023-04-05 11:21:15.127100 zntrack-0.6.0a4/zntrack/fields/meta/__init__.py
--rw-r--r--   0        0        0    15986 2023-04-05 10:56:52.283202 zntrack-0.6.0a4/zntrack/fields/zn/__init__.py
--rw-r--r--   0        0        0     2647 2023-03-16 14:38:52.692721 zntrack-0.6.0a4/zntrack/notebooks/jupyter.py
--rw-r--r--   0        0        0      133 2023-03-16 14:38:52.692721 zntrack-0.6.0a4/zntrack/project/__init__.py
--rw-r--r--   0        0        0     7024 2023-03-28 15:55:39.712257 zntrack-0.6.0a4/zntrack/project/zntrack_project.py
--rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.0a4/zntrack/tools/__init__.py
--rw-r--r--   0        0        0     6065 2023-03-28 16:02:45.147573 zntrack-0.6.0a4/zntrack/utils/__init__.py
--rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.0a4/zntrack/utils/cli.py
--rw-r--r--   0        0        0     3354 2023-03-17 12:53:04.976998 zntrack-0.6.0a4/zntrack/utils/config.py
--rw-r--r--   0        0        0     4727 2023-03-06 10:02:12.898384 zntrack-0.6.0a4/zntrack/utils/file_io.py
--rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.0a4/zntrack/utils/node_wd.py
--rw-r--r--   0        0        0     7042 1970-01-01 00:00:00.000000 zntrack-0.6.0a4/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.0a5/LICENSE
+-rw-r--r--   0        0        0     6025 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/README.md
+-rw-r--r--   0        0        0     2299 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-03-28 15:55:39.672257 zntrack-0.6.0a5/zntrack/__init__.py
+-rw-r--r--   0        0        0     2940 2023-04-08 19:50:48.755766 zntrack-0.6.0a5/zntrack/cli/__init__.py
+-rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.0a5/zntrack/core/__init__.py
+-rw-r--r--   0        0        0    10646 2023-04-05 10:56:52.273202 zntrack-0.6.0a5/zntrack/core/node.py
+-rw-r--r--   0        0        0    14022 2023-03-16 14:38:52.672721 zntrack-0.6.0a5/zntrack/core/nodify.py
+-rw-r--r--   0        0        0     2078 2023-04-09 21:25:48.681300 zntrack-0.6.0a5/zntrack/exceptions/__init__.py
+-rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.0a5/zntrack/fields/__init__.py
+-rw-r--r--   0        0        0     5135 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/dvc/__init__.py
+-rw-r--r--   0        0        0     9915 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/field.py
+-rw-r--r--   0        0        0     3562 2023-04-08 19:50:48.755766 zntrack-0.6.0a5/zntrack/fields/meta/__init__.py
+-rw-r--r--   0        0        0    16041 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/zn/__init__.py
+-rw-r--r--   0        0        0     2647 2023-03-16 14:38:52.692721 zntrack-0.6.0a5/zntrack/notebooks/jupyter.py
+-rw-r--r--   0        0        0      133 2023-03-16 14:38:52.692721 zntrack-0.6.0a5/zntrack/project/__init__.py
+-rw-r--r--   0        0        0     9694 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/zntrack/project/zntrack_project.py
+-rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.0a5/zntrack/tools/__init__.py
+-rw-r--r--   0        0        0     6065 2023-03-28 16:02:45.147573 zntrack-0.6.0a5/zntrack/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.0a5/zntrack/utils/cli.py
+-rw-r--r--   0        0        0     3354 2023-04-10 11:58:36.429618 zntrack-0.6.0a5/zntrack/utils/config.py
+-rw-r--r--   0        0        0     4727 2023-03-06 10:02:12.898384 zntrack-0.6.0a5/zntrack/utils/file_io.py
+-rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.0a5/zntrack/utils/node_wd.py
+-rw-r--r--   0        0        0     7166 1970-01-01 00:00:00.000000 zntrack-0.6.0a5/PKG-INFO
```

### Comparing `zntrack-0.6.0a4/LICENSE` & `zntrack-0.6.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/README.md` & `zntrack-0.6.0a5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![coeralls](https://coveralls.io/repos/github/zincware/ZnTrack/badge.svg)](https://coveralls.io/github/zincware/ZnTrack)
 [![codecov](https://codecov.io/gh/zincware/ZnTrack/branch/main/graph/badge.svg?token=ZQ67FXN1IT)](https://codecov.io/gh/zincware/ZnTrack)
 [![Maintainability](https://api.codeclimate.com/v1/badges/f25e119bbd5d5ec74e2c/maintainability)](https://codeclimate.com/github/zincware/ZnTrack/maintainability)
-![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/pytest.yaml/badge.svg)
+![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/zntrack.svg)](https://badge.fury.io/py/zntrack)
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
@@ -48,24 +48,26 @@
     
     def run(self):
         """Command to be run by DVC"""
         self.random_number = randrange(self.max_number)
         
 if __name__ == "__main__":
     # Write the computational graph
-    HelloWorld(max_number=512).write_graph()
+    with zntrack.Project() as project:
+        hello_world = HelloWorld(max_number=512)
+    project.run()
 ```
 
 This will create a [DVC](https://dvc.org) stage ``HelloWorld``.
 The workflow is defined in ``dvc.yaml`` and the parameters are stored in ``params.yaml``.
 
-You can run the workflow with ``dvc repro``.
+This will run the workflow with ``dvc repro`` automatically.
 Once the graph is executed, the results, i.e. the random number can be accessed directly by the Node object.
 ```python
-hello_world = HelloWorld.load()
+hello_world.load()
 print(hello_world.random_numer)
 ```
 An overview of all the ZnTrack features as well as more detailed examples can be found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
 
 ## Wrap Python Functions
 ZnTrack also provides tools to convert a Python function into a DVC Node.
 This approach is much more lightweight compared to the class-based approach with only a reduced set of functionality.
@@ -77,15 +79,17 @@
 
 @nodify(outs=pathlib.Path("text.txt"), params={"text": "Lorem Ipsum"})
 def write_text(cfg: NodeConfig):
     cfg.outs.write_text(
         cfg.params.text
     )
 # build the DVC graph
-write_text()
+with zntrack.Project() as project:
+    write_text()
+project.run()
 ````
 
 The ``cfg`` dataclass passed to the function provides access to all configured files
 and parameters via [dot4dict](https://github.com/zincware/dot4dict). The function body
 will be executed by the ``dvc repro`` command or if ran via `write_text(run=True)`.
 All parameters are loaded from or stored in ``params.yaml``.
```

### Comparing `zntrack-0.6.0a4/pyproject.toml` & `zntrack-0.6.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "ZnTrack"
-version = "0.6.0a4"
+version = "0.6.0a5"
 description = "Create, Run and Benchmark DVC Pipelines in Python"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "data-version-control", "machine-learning", "reproducibility", "collaboration"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-dvc = "^2.50.0"
+dvc = "^2.52.0, !=2.53.0"
 pyyaml = "^6.0"
 tqdm = "^4.64.0"
 pandas = "^1.4.3"
 typer = "^0.7.0"
 
 dot4dict = "^0.1.1"
 zninit = "^0.1.9"
 znjson = "^0.2.2"
-znflow = "^0.1.10"
+znflow = "^0.1.11"
 
 
 [tool.poetry.urls]
 documentation = "https://zntrack.readthedocs.io"
 repository = "https://github.com/zincware/ZnTrack"
```

### Comparing `zntrack-0.6.0a4/zntrack/__init__.py` & `zntrack-0.6.0a5/zntrack/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/cli/__init__.py` & `zntrack-0.6.0a5/zntrack/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,19 +51,25 @@
     """Execute a ZnTrack Node.
 
     Use as 'zntrack run module.Node --name node_name'.
     """
     env_file = pathlib.Path("env.yaml")
     if env_file.exists():
         env = yaml.safe_load(env_file.read_text())
-        for key, value in env.get(name, {}).items():
-            if value is None:
-                os.environ.pop(key, None)
-            else:
+        os.environ.update(env.get("global", {}))
+
+        for key, value in env.get("stages", {}).get(name, {}).items():
+            if isinstance(value, str):
                 os.environ[key] = value
+            elif isinstance(value, dict):
+                os.environ.update(value)
+            elif value is None:
+                pass
+            else:
+                raise ValueError(f"Unknown value for env variable {key}: {value}")
 
     sys.path.append(pathlib.Path.cwd().as_posix())
 
     package_and_module, cls = node.rsplit(".", 1)
     module = importlib.import_module(package_and_module)
 
     cls = getattr(module, cls)
```

### Comparing `zntrack-0.6.0a4/zntrack/core/node.py` & `zntrack-0.6.0a5/zntrack/core/node.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/core/nodify.py` & `zntrack-0.6.0a5/zntrack/core/nodify.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/exceptions/__init__.py` & `zntrack-0.6.0a5/zntrack/exceptions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,7 +43,28 @@
         msg += f"""
         >>> {node.name} = ...
         >>> with project:
         >>>    {instance.name}.{field.name} = {node.name}
         """
 
         super().__init__(msg)
+
+
+class DuplicateNodeNameError(Exception):
+    """Raised when a node is not available."""
+
+    def __init__(self, node):
+        """Initialize the exception.
+
+        Parameters
+        ----------
+        node: Node
+            The node that is already on the graph.
+        """
+        msg = (
+            f"Node name {node.name} is already used in the graph. Please use"
+            " 'name=...' to specify a unique name or set the project attribute"
+            " 'automatic_node_names=True' to automatically add a number to"
+            " the name. Alternatively, set the project attribute 'force=True'"
+            " to overwrite existing nodes."
+        )
+        super().__init__(msg)
```

### Comparing `zntrack-0.6.0a4/zntrack/fields/dvc/__init__.py` & `zntrack-0.6.0a5/zntrack/fields/dvc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """DVC fields without serialization of data / for file paths."""
 import json
 import pathlib
 import typing
 
 import znjson
 
-from zntrack.fields.field import Field, FieldGroup
+from zntrack.fields.field import Field, FieldGroup, PlotsMixin
 from zntrack.utils import node_wd
 
 if typing.TYPE_CHECKING:
     from zntrack import Node
 
 
 class DVCOption(Field):
@@ -126,14 +126,18 @@
         """
         if instance is None:
             return self
         value = super().__get__(instance, owner)
         return node_wd.ReplaceNWD()(value, nwd=instance.nwd)
 
 
+class PlotsOption(PlotsMixin, DVCOption):
+    """Field with DVC plots kwargs."""
+
+
 def outs(*args, **kwargs) -> DVCOption:
     """Create a outs field."""
     return DVCOption(*args, dvc_option="outs", **kwargs)
 
 
 def params(*args, **kwargs) -> DVCOption:
     """Create a params field."""
@@ -163,13 +167,13 @@
 def metrics_no_cache(*args, **kwargs) -> DVCOption:
     """Create a metrics_no_cache field."""
     return DVCOption(*args, dvc_option="metrics-no-cache", **kwargs)
 
 
 def plots(*args, **kwargs) -> DVCOption:
     """Create a plots field."""
-    return DVCOption(*args, dvc_option="plots", **kwargs)
+    return PlotsOption(*args, dvc_option="plots", **kwargs)
 
 
 def plots_no_cache(*args, **kwargs) -> DVCOption:
     """Create a plots_no_cache field."""
-    return DVCOption(*args, dvc_option="plots-no-cache", **kwargs)
+    return PlotsOption(*args, dvc_option="plots-no-cache", **kwargs)
```

### Comparing `zntrack-0.6.0a4/zntrack/fields/meta/__init__.py` & `zntrack-0.6.0a5/zntrack/fields/meta/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,25 +75,35 @@
         """Save the field to disk."""
         file = pathlib.Path("env.yaml")
         try:
             context = yaml.safe_load(file.read_text())
         except FileNotFoundError:
             context = {}
 
-        node_context = context.get(instance.name, {})
+        stages = context.get("stages", {})
+        # TODO: when to reset the environment variables?
+
+        node_context = stages.get(instance.name, {})
         value = getattr(instance, self.name)
-        if not isinstance(value, str) and value is not None:
-            raise ValueError(f"Environment value must be a string, not {type(value)}")
-        node_context[self.name] = value
-        context[instance.name] = node_context
+        if isinstance(value, (str, dict)):
+            node_context[self.name] = value
+            stages[instance.name] = node_context
+        elif value is None:
+            return
+        else:
+            raise ValueError(
+                f"Environment value must be a string or dict, not {type(value)}"
+            )
+
+        context["stages"] = stages
         file.write_text(yaml.safe_dump(context))
 
     def get_data(self, instance: "Node") -> any:
         """Get the value of the field from the file."""
         env_dict = yaml.safe_load(instance.state.fs.read_text("env.yaml"))
-        return env_dict.get(instance.name, {}).get(self.name, None)
+        return env_dict.get("stages", {}).get(instance.name, {}).get(self.name, None)
 
     def get_stage_add_argument(self, instance) -> typing.List[tuple]:
         """Get the dvc command for this field."""
         if self.is_parameter:
-            return [("--params", f"env.yaml:{instance.name}.{self.name}")]
+            return [("--params", f"env.yaml:stages.{instance.name}.{self.name}")]
         return []
```

### Comparing `zntrack-0.6.0a4/zntrack/fields/zn/__init__.py` & `zntrack-0.6.0a5/zntrack/fields/zn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import znflow
 import znflow.utils
 import zninit
 import znjson
 from znflow import handler
 
 from zntrack import exceptions
-from zntrack.fields.field import DataIsLazyError, Field, FieldGroup, LazyField
+from zntrack.fields.field import DataIsLazyError, Field, FieldGroup, LazyField, PlotsMixin
 from zntrack.utils import module_handler, update_key_val
 
 if typing.TYPE_CHECKING:
     from zntrack import Node
 log = logging.getLogger(__name__)
 
 
@@ -230,26 +230,27 @@
         list
             A list containing the DVC command for this field.
         """
         file = self.get_files(instance)[0]
         return [(f"--{self.dvc_option}", file.as_posix())]
 
 
-class Plots(LazyField):
+class Plots(PlotsMixin, LazyField):
     """A field that is saved to disk."""
 
     dvc_option: str = "plots"
     group = FieldGroup.RESULT
 
     def get_files(self, instance) -> list:
         """Get the path of the file in the node directory."""
         return [instance.nwd / f"{self.name}.csv"]
 
     def save(self, instance: "Node"):
         """Save the field to disk."""
+        super().save(instance)
         try:
             value = self.get_value_except_lazy(instance)
         except DataIsLazyError:
             return
         if value is None:
             return
```

### Comparing `zntrack-0.6.0a4/zntrack/notebooks/jupyter.py` & `zntrack-0.6.0a5/zntrack/notebooks/jupyter.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/project/zntrack_project.py` & `zntrack-0.6.0a5/zntrack/project/zntrack_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,126 @@
 from __future__ import annotations
 
 import contextlib
 import dataclasses
 import json
 import logging
 import pathlib
+import shutil
 
 import git
 import yaml
 import znflow
 from znflow.handler import UpdateConnectors
 
+from zntrack import exceptions
 from zntrack.core.node import Node, get_dvc_cmd
 from zntrack.utils import capture_run_dvc_cmd, run_dvc_cmd
 
 log = logging.getLogger(__name__)
 
 
-class _ProjectBase(znflow.DiGraph):
+def _initalize():
+    """Initialize the project."""
+    try:
+        _ = git.Repo()
+    except git.exc.InvalidGitRepositoryError:
+        # TODO ASSERT IS EMPTY!
+        repo = git.Repo.init()
+        repo.init()
+        run_dvc_cmd(["init", "--quiet"])
+        # Create required files:
+        pathlib.Path("zntrack.json").write_text(json.dumps({}))
+        pathlib.Path("dvc.yaml").write_text(yaml.safe_dump({}))
+        pathlib.Path("params.yaml").write_text(yaml.safe_dump({}))
+        repo.git.add(A=True)
+        repo.index.commit("Project initialized.")
+
+
+@dataclasses.dataclass
+class Project:
+    """The ZnTrack Project class.
+
+    Attributes
+    ----------
+    graph : znflow.DiGraph
+        the znflow graph of the project.
+    initialize : bool, default = True
+        If True, initialize a git repository and a dvc repository.
+    remove_existing_graph : bool, default = False
+        If True, remove 'dvc.yaml', 'zntrack.json' and 'params.yaml'
+            before writing new nodes.
+    automatic_node_names : bool, default = False
+        If True, automatically add a number to the node name if the name is already
+            used in the graph.
+    force : bool, default = False
+        overwrite existing nodes.
+    """
+
+    graph: znflow.DiGraph = dataclasses.field(default_factory=znflow.DiGraph, init=False)
+    initialize: bool = True
+    remove_existing_graph: bool = False
+    automatic_node_names: bool = False
+    force: bool = False
+
+    def __post_init__(self):
+        """Initialize the Project.
+
+        Attributes
+        ----------
+        initialize : bool, default = True
+            If True, initialize a git repository and a dvc repository.
+        remove_existing_graph : bool, default = False
+            If True, remove 'dvc.yaml', 'zntrack.json' and 'params.yaml'
+              before writing new nodes.
+        """
+        if self.initialize:
+            _initalize()
+        if self.remove_existing_graph:
+            # we remove the files that typically contain the graph definition
+            pathlib.Path("zntrack.json").unlink(missing_ok=True)
+            pathlib.Path("dvc.yaml").unlink(missing_ok=True)
+            pathlib.Path("params.yaml").unlink(missing_ok=True)
+            shutil.rmtree("nodes", ignore_errors=True)
+
+    def __enter__(self, *args, **kwargs):
+        """Enter the graph context."""
+        self.graph.__enter__(*args, **kwargs)
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        """Exit the graph context."""
+        self.graph.__exit__(*args, **kwargs)
+        if not self.force:
+            self.update_node_names()
+
+    def update_node_names(self):
+        """Update the node names to be unique."""
+        node_names = []
+        for node_uuid in self.graph.get_sorted_nodes():
+            node: Node = self.graph.nodes[node_uuid]["value"]
+            if self.automatic_node_names:
+                if node.name in node_names:
+                    idx = 1
+                    while f"{node.name}_{idx}" in node_names:
+                        idx += 1
+                    node.name = f"{node.name}_{idx}"
+                    log.debug(f"Updating {node.name = }")
+
+            elif node.name in node_names:
+                raise exceptions.DuplicateNodeNameError(node)
+            node_names.append(node.name)
+
     def run(
-        self, eager=False, repro: bool = True, optional: dict = None, save: bool = True
+        self,
+        eager=False,
+        repro: bool = True,
+        optional: dict = None,
+        save: bool = True,
+        environment: dict = None,
     ):
         """Run the Project Graph.
 
         Parameters
         ----------
         eager : bool, default = False
             if True, run the nodes in eager mode.
@@ -34,95 +131,75 @@
             Otherwise, the results will only be in memory.
         repro : bool, default = True
             if True, run dvc repro after running the nodes.
         optional : dict, default = None
             A dictionary of optional arguments for each node.
             Use {node_name: {arg_name: arg_value}} to pass arguments to nodes.
             Possible arg_names are e.g. 'always_changed: True'
+        environment : dict, default = None
+            A dictionary of environment variables for all nodes.
         """
         if not save and not eager:
             raise ValueError("Save can only be false if eager is True")
+
+        self._handle_environment(environment)
+
         if optional is None:
             optional = {}
-        for node_uuid in self.get_sorted_nodes():
-            node: Node = self.nodes[node_uuid]["value"]
+
+        for node_uuid in self.graph.get_sorted_nodes():
+            node: Node = self.graph.nodes[node_uuid]["value"]
             if eager:
                 # update connectors
                 log.info(f"Running node {node}")
-                self._update_node_attributes(node, UpdateConnectors())
+                self.graph._update_node_attributes(node, UpdateConnectors())
                 node.run()
                 if save:
                     node.save()
                 node.state.loaded = True
             else:
                 log.info(f"Adding node {node}")
                 cmd = get_dvc_cmd(node, **optional.get(node.name, {}))
                 for x in cmd:
                     run_dvc_cmd(x)
                 node.save(results=False)
         if not eager and repro:
             run_dvc_cmd(["repro"])
             # TODO should we load the nodes here? Maybe, if lazy loading is implemented.
 
+    def _handle_environment(self, environment: dict):
+        """Write global environment variables to the env.yaml file."""
+        if environment is not None:
+            file = pathlib.Path("env.yaml")
+            try:
+                context = yaml.safe_load(file.read_text())
+            except FileNotFoundError:
+                context = {}
+
+            context["global"] = environment
+            file.write_text(yaml.safe_dump(context))
+
     def load(self):
-        for node_uuid in self.get_sorted_nodes():
-            node = self.nodes[node_uuid]["value"]
+        """Load all nodes in the project."""
+        for node_uuid in self.graph.get_sorted_nodes():
+            node = self.graph.nodes[node_uuid]["value"]
             node.load()
 
     def get_nodes(self) -> dict[str, znflow.Node]:
+        """Get the nodes in the project."""
         nodes = {}
-        for node_uuid in self.get_sorted_nodes():
-            node = self.nodes[node_uuid]["value"]
+        for node_uuid in self.graph.get_sorted_nodes():
+            node = self.graph.nodes[node_uuid]["value"]
             nodes[node.name] = node
         return nodes
 
-
-def _initalize():
-    """Initialize the project."""
-    try:
-        _ = git.Repo()
-    except git.exc.InvalidGitRepositoryError:
-        # TODO ASSERT IS EMPTY!
-        repo = git.Repo.init()
-        repo.init()
-        run_dvc_cmd(["init", "--quiet"])
-        # Create required files:
-        pathlib.Path("zntrack.json").write_text(json.dumps({}))
-        pathlib.Path("dvc.yaml").write_text(yaml.safe_dump({}))
-        pathlib.Path("params.yaml").write_text(yaml.safe_dump({}))
-        repo.git.add(A=True)
-        repo.index.commit("Project initialized.")
-
-
-class Project(_ProjectBase):
-    """The ZnTrack Project class."""
-
-    def __init__(
-        self, initialize: bool = True, remove_existing_graph: bool = False
-    ) -> None:
-        """Initialize the Project.
-
-        Attributes
-        ----------
-        initialize : bool, default = True
-            If True, initialize a git repository and a dvc repository.
-        remove_existing_graph : bool, default = False
-            If True, remove 'dvc.yaml', 'zntrack.json' and 'params.yaml'
-              before writing new nodes.
-        """
-        # TODO maybe it is not a good idea to base everything on the DiGraph class.
-        #  It seems to call some class methods
-        super().__init__()
-        if initialize:
-            _initalize()
-        if remove_existing_graph:
-            # we remove the files that typically contain the graph definition
-            pathlib.Path("zntrack.json").unlink(missing_ok=True)
-            pathlib.Path("dvc.yaml").unlink(missing_ok=True)
-            pathlib.Path("params.yaml").unlink(missing_ok=True)
+    @property
+    def nodes(self) -> dict[str, znflow.Node]:
+        """Get the nodes in the project."""
+        return self.get_nodes()
 
     def create_branch(self, name: str) -> "Branch":
         """Create a branch in the project."""
         branch = Branch(self, name)
         branch.create()
         return branch
 
@@ -132,16 +209,16 @@
         # TODO: return an experiment object that allows you to load the results
         # TODO this context manager WILL NOT ADD new nodes to the graph.
 
         exp = Experiment(name, project=self)
 
         yield exp
 
-        for node_uuid in self.get_sorted_nodes():
-            node: Node = self.nodes[node_uuid]["value"]
+        for node_uuid in self.graph.get_sorted_nodes():
+            node: Node = self.graph.nodes[node_uuid]["value"]
             node.save(results=False)
 
         cmd = ["exp", "run"]
         if queue:
             cmd.append("--queue")
         if name is not None:
             cmd.extend(["--name", name])
@@ -150,15 +227,15 @@
     def run_exp(self, jobs: int = 1) -> None:
         """Run all queued experiments."""
         run_dvc_cmd(["exp", "run", "--run-all", "--jobs", str(jobs)])
 
     @property
     def branches(self):
         """Get the branches in the project."""
-        repo = git.Repo()
+        repo = git.Repo()  # todo should be self.repo
         return [Branch(project=self, name=branch.name) for branch in repo.branches]
 
 
 @dataclasses.dataclass
 class Experiment:
     """A DVC Experiment."""
 
@@ -172,26 +249,26 @@
         self.nodes = {
             name: node.from_rev(name=name, rev=self.name)
             for name, node in self.project.get_nodes().items()
         }
 
     def __getitem__(self, key) -> Node:
         """Get the Node from the experiment."""
+        if len(self.nodes) == 0:
+            self.load()
         return self.nodes[key]
 
 
-class Branch(_ProjectBase):
+@dataclasses.dataclass
+class Branch:
     """The ZnTrack Branch class for managing experiments."""
 
-    def __init__(self, project=None, name=None) -> None:
-        """Initialize a Branch."""
-        super().__init__()
-        self.project = project
-        self.name = name
-        self.repo = git.Repo()
+    project: Project
+    name: str
+    repo: git.Repo = dataclasses.field(init=False, repr=False, default_factory=git.Repo)
 
     def create(self):
         """Create the branch."""
         self.repo.create_head(self.name)
 
     def queue(self, name: str):
         """Queue the branch to run."""
@@ -201,11 +278,11 @@
 
         # if self.repo.is_dirty():
         # if len(self.repo.untracked_files) > 0:
         self.repo.git.add(A=True)
         self.repo.index.commit(f"parameters for {name}")
         run_dvc_cmd(["exp", "run", "--name", name, "--queue"])
 
-        for node_uuid in self.get_sorted_nodes():
-            node = self.nodes[node_uuid]["value"]
+        for node_uuid in self.graph.get_sorted_nodes():
+            node = self.graph.nodes[node_uuid]["value"]
             node.state.rev = name
         active_branch.checkout()
```

### Comparing `zntrack-0.6.0a4/zntrack/tools/__init__.py` & `zntrack-0.6.0a5/zntrack/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/utils/__init__.py` & `zntrack-0.6.0a5/zntrack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/utils/cli.py` & `zntrack-0.6.0a5/zntrack/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/utils/config.py` & `zntrack-0.6.0a5/zntrack/utils/config.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/utils/file_io.py` & `zntrack-0.6.0a5/zntrack/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/zntrack/utils/node_wd.py` & `zntrack-0.6.0a5/zntrack/utils/node_wd.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a4/PKG-INFO` & `zntrack-0.6.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: zntrack
-Version: 0.6.0a4
+Version: 0.6.0a5
 Summary: Create, Run and Benchmark DVC Pipelines in Python
 License: Apache-2.0
 Keywords: data-science,data-version-control,machine-learning,reproducibility,collaboration
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dot4dict (>=0.1.1,<0.2.0)
-Requires-Dist: dvc (>=2.50.0,<3.0.0)
+Requires-Dist: dvc (>=2.52.0,<3.0.0,!=2.53.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: znflow (>=0.1.10,<0.2.0)
+Requires-Dist: znflow (>=0.1.11,<0.2.0)
 Requires-Dist: zninit (>=0.1.9,<0.2.0)
 Requires-Dist: znjson (>=0.2.2,<0.3.0)
 Project-URL: documentation, https://zntrack.readthedocs.io
 Project-URL: repository, https://github.com/zincware/ZnTrack
 Description-Content-Type: text/markdown
 
 [![coeralls](https://coveralls.io/repos/github/zincware/ZnTrack/badge.svg)](https://coveralls.io/github/zincware/ZnTrack)
 [![codecov](https://codecov.io/gh/zincware/ZnTrack/branch/main/graph/badge.svg?token=ZQ67FXN1IT)](https://codecov.io/gh/zincware/ZnTrack)
 [![Maintainability](https://api.codeclimate.com/v1/badges/f25e119bbd5d5ec74e2c/maintainability)](https://codeclimate.com/github/zincware/ZnTrack/maintainability)
-![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/pytest.yaml/badge.svg)
+![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/zntrack.svg)](https://badge.fury.io/py/zntrack)
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
@@ -76,24 +76,26 @@
     
     def run(self):
         """Command to be run by DVC"""
         self.random_number = randrange(self.max_number)
         
 if __name__ == "__main__":
     # Write the computational graph
-    HelloWorld(max_number=512).write_graph()
+    with zntrack.Project() as project:
+        hello_world = HelloWorld(max_number=512)
+    project.run()
 ```
 
 This will create a [DVC](https://dvc.org) stage ``HelloWorld``.
 The workflow is defined in ``dvc.yaml`` and the parameters are stored in ``params.yaml``.
 
-You can run the workflow with ``dvc repro``.
+This will run the workflow with ``dvc repro`` automatically.
 Once the graph is executed, the results, i.e. the random number can be accessed directly by the Node object.
 ```python
-hello_world = HelloWorld.load()
+hello_world.load()
 print(hello_world.random_numer)
 ```
 An overview of all the ZnTrack features as well as more detailed examples can be found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
 
 ## Wrap Python Functions
 ZnTrack also provides tools to convert a Python function into a DVC Node.
 This approach is much more lightweight compared to the class-based approach with only a reduced set of functionality.
@@ -105,15 +107,17 @@
 
 @nodify(outs=pathlib.Path("text.txt"), params={"text": "Lorem Ipsum"})
 def write_text(cfg: NodeConfig):
     cfg.outs.write_text(
         cfg.params.text
     )
 # build the DVC graph
-write_text()
+with zntrack.Project() as project:
+    write_text()
+project.run()
 ````
 
 The ``cfg`` dataclass passed to the function provides access to all configured files
 and parameters via [dot4dict](https://github.com/zincware/dot4dict). The function body
 will be executed by the ``dvc repro`` command or if ran via `write_text(run=True)`.
 All parameters are loaded from or stored in ``params.yaml``.
```

