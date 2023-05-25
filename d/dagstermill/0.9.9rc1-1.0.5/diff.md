# Comparing `tmp/dagstermill-0.9.9rc1.tar.gz` & `tmp/dagstermill-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagstermill-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:42 2020, max compression
+gzip compressed data, was "dagstermill-1.0.5.tar", last modified: Fri Aug 26 13:45:57 2022, max compression
```

## Comparing `dagstermill-0.9.9rc1.tar` & `dagstermill-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      513 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill/
--rw-r--r--   0 bobchen    (501) staff       (20)      796 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/__main__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4514 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4189 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/context.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2554 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/engine.py
--rw-r--r--   0 bobchen    (501) staff       (20)      323 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/errors.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill/examples/
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/examples/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12664 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/examples/repository.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12003 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1307 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/serialize.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14021 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2026 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/translator.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      513 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      581 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       12 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/top_level.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1163 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:57.560620 dagstermill-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagstermill-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       44 2022-08-26 13:33:01.000000 dagstermill-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      573 2022-08-26 13:45:57.560620 dagstermill-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2022-08-26 13:33:01.000000 dagstermill-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:57.556620 dagstermill-1.0.5/dagstermill/
+-rw-r--r--   0 root         (0) root         (0)      838 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/cli.py
+-rw-r--r--   0 root         (0) root         (0)      516 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/compat.py
+-rw-r--r--   0 root         (0) root         (0)     8368 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/context.py
+-rw-r--r--   0 root         (0) root         (0)     6087 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/engine.py
+-rw-r--r--   0 root         (0) root         (0)      141 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:57.556620 dagstermill-1.0.5/dagstermill/examples/
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13120 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/examples/repository.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/factory.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/io_managers.py
+-rw-r--r--   0 root         (0) root         (0)    16250 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/manager.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/py.typed
+-rw-r--r--   0 root         (0) root         (0)      188 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/translator.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagstermill-1.0.5/dagstermill/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:57.556620 dagstermill-1.0.5/dagstermill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      573 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      652 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:45:57.000000 dagstermill-1.0.5/dagstermill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2022-08-26 13:45:57.560620 dagstermill-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2294 2022-08-26 13:33:01.000000 dagstermill-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagstermill-0.9.9rc1/LICENSE` & `dagstermill-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9rc1/dagstermill/__init__.py` & `dagstermill-1.0.5/dagstermill/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from dagster.core.utils import check_dagster_package_version
+from dagster._core.utils import check_dagster_package_version
 
 from .context import DagstermillExecutionContext
-from .errors import DagstermillError, DagstermillExecutionError
+from .errors import DagstermillError
+from .factory import define_dagstermill_op
+from .io_managers import local_output_notebook_io_manager
 from .manager import MANAGER_FOR_NOTEBOOK_INSTANCE as _MANAGER_FOR_NOTEBOOK_INSTANCE
-from .solids import define_dagstermill_solid
 from .version import __version__
 
 check_dagster_package_version("dagstermill", __version__)
 
 get_context = _MANAGER_FOR_NOTEBOOK_INSTANCE.get_context
 
 yield_result = _MANAGER_FOR_NOTEBOOK_INSTANCE.yield_result
 
 yield_event = _MANAGER_FOR_NOTEBOOK_INSTANCE.yield_event
 
 _reconstitute_pipeline_context = _MANAGER_FOR_NOTEBOOK_INSTANCE.reconstitute_pipeline_context
 
 _teardown = _MANAGER_FOR_NOTEBOOK_INSTANCE.teardown_resources
 
-_load_parameter = _MANAGER_FOR_NOTEBOOK_INSTANCE.load_parameter
+_load_input_parameter = _MANAGER_FOR_NOTEBOOK_INSTANCE.load_input_parameter
```

### Comparing `dagstermill-0.9.9rc1/dagstermill/cli.py` & `dagstermill-1.0.5/dagstermill/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import copy
 import os
 import subprocess
+from typing import Dict, Optional
 
 import click
 import nbformat
 from papermill.iorw import load_notebook_node, write_ipynb
 
-from dagster import check
-from dagster.seven.json import loads
-from dagster.utils import mkdir_p, safe_isfile
+import dagster._check as check
+from dagster._seven.json import loads
+from dagster._utils import mkdir_p, safe_isfile
 
 
 def get_import_cell():
     return nbformat.v4.new_code_cell(source="import dagstermill")
 
 
 def get_parameters_cell():
     parameters_cell = nbformat.v4.new_code_cell(source="context = dagstermill.get_context()")
     parameters_cell.metadata["tags"] = ["parameters"]
     return parameters_cell
 
 
-def get_kernelspec(kernel):
+def get_kernelspec(kernel: Optional[str] = None):
     kernelspecs = loads(subprocess.check_output(["jupyter", "kernelspec", "list", "--json"]))
 
     check.invariant(len(kernelspecs["kernelspecs"]) > 0, "No available Jupyter kernelspecs!")
 
     if kernel is None:
         preferred_kernels = list(
             filter(
@@ -49,15 +50,15 @@
     return {
         "name": kernel,
         "language": kernelspecs["kernelspecs"][kernel]["spec"]["language"],
         "display_name": kernelspecs["kernelspecs"][kernel]["spec"]["display_name"],
     }
 
 
-def get_notebook_scaffolding(kernelspec):
+def get_notebook_scaffolding(kernelspec: Dict[str, str]):
     check.dict_param(kernelspec, "kernelspec", key_type=str, value_type=str)
 
     notebook = nbformat.v4.new_notebook()
 
     notebook.cells = [get_import_cell(), get_parameters_cell()]
 
     metadata = {"celltoolbar": "Tags", "kernelspec": kernelspec}
@@ -67,19 +68,19 @@
     return nbformat.writes(notebook)
 
 
 @click.command(
     name="register-notebook", help=("Scaffolds existing notebook for dagstermill compatibility")
 )
 @click.option("--notebook", "-note", type=click.Path(exists=True), help="Path to existing notebook")
-def retroactively_scaffold_notebook(notebook):
+def retroactively_scaffold_notebook(notebook: str):
     execute_retroactive_scaffold(notebook)
 
 
-def execute_retroactive_scaffold(notebook_path):
+def execute_retroactive_scaffold(notebook_path: str):
     nb = load_notebook_node(notebook_path)
     new_nb = copy.deepcopy(nb)
     new_nb.cells = [get_import_cell(), get_parameters_cell()] + nb.cells
     write_ipynb(new_nb, notebook_path)
 
 
 @click.command(name="create-notebook", help=("Creates new dagstermill notebook."))
@@ -94,19 +95,19 @@
     type=click.STRING,
     help=(
         "Specify an existing Jupyter kernel to use. (Run `jupyter kernelspec list` to view "
         "available kernels.) By default a kernel called 'dagster' will be used, if available, "
         "then one called 'python3', then 'python', and then the first available kernel."
     ),
 )
-def create_notebook(notebook, force_overwrite, kernel):
+def create_notebook(notebook: str, force_overwrite: bool, kernel: str):
     execute_create_notebook(notebook, force_overwrite, kernel)
 
 
-def execute_create_notebook(notebook, force_overwrite, kernel):
+def execute_create_notebook(notebook: str, force_overwrite: bool, kernel: str):
     notebook_path = os.path.join(
         os.getcwd(), notebook if notebook.endswith(".ipynb") else notebook + ".ipynb"
     )
 
     notebook_dir = os.path.dirname(notebook_path)
     mkdir_p(notebook_dir)
 
@@ -116,15 +117,15 @@
                 "Warning, {notebook_path} already exists and continuing "
                 "will overwrite the existing notebook. "
                 "Are you sure you want to continue?"
             ).format(notebook_path=notebook_path),
             abort=True,
         )
 
-    with open(notebook_path, "w") as f:
+    with open(notebook_path, "w", encoding="utf8") as f:
         f.write(get_notebook_scaffolding(get_kernelspec(kernel)))
         click.echo("Created new dagstermill notebook at {path}".format(path=notebook_path))
 
 
 def create_dagstermill_cli():
     group = click.Group(name="dagstermill")
     group.add_command(create_notebook)
```

### Comparing `dagstermill-0.9.9rc1/dagstermill/translator.py` & `dagstermill-1.0.5/dagstermill/translator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import papermill
 
-from dagster import seven
+from dagster import _seven
 
 RESERVED_INPUT_NAMES = [
     "__dm_context",
     "__dm_dagstermill",
     "__dm_executable_dict",
     "__dm_json",
     "__dm_pipeline_run_dict",
     "__dm_solid_handle_kwargs",
     "__dm_instance_ref_dict",
+    "__dm_step_key",
+    "__dm_input_names",
 ]
 
 INJECTED_BOILERPLATE = """
 # Injected parameters
 from dagster import seven as __dm_seven
 import dagstermill as __dm_dagstermill
 context = __dm_dagstermill._reconstitute_pipeline_context(
@@ -24,40 +26,39 @@
     }}
 )
 """
 
 
 class DagsterTranslator(papermill.translators.PythonTranslator):
     @classmethod
-    def codify(cls, parameters):
+    def codify(cls, parameters):  # pylint: disable=arguments-differ
         assert "__dm_context" in parameters
         assert "__dm_executable_dict" in parameters
         assert "__dm_pipeline_run_dict" in parameters
         assert "__dm_solid_handle_kwargs" in parameters
         assert "__dm_instance_ref_dict" in parameters
+        assert "__dm_step_key" in parameters
+        assert "__dm_input_names" in parameters
 
         context_args = parameters["__dm_context"]
         pipeline_context_args = dict(
             executable_dict=parameters["__dm_executable_dict"],
             pipeline_run_dict=parameters["__dm_pipeline_run_dict"],
             solid_handle_kwargs=parameters["__dm_solid_handle_kwargs"],
             instance_ref_dict=parameters["__dm_instance_ref_dict"],
-            **context_args
+            step_key=parameters["__dm_step_key"],
+            **context_args,
         )
 
         for key in pipeline_context_args:
-            pipeline_context_args[key] = seven.json.dumps(pipeline_context_args[key])
+            pipeline_context_args[key] = _seven.json.dumps(pipeline_context_args[key])
 
         content = INJECTED_BOILERPLATE.format(pipeline_context_args=pipeline_context_args)
 
-        for name, val in parameters.items():
-            if name in RESERVED_INPUT_NAMES:
-                continue
-            dm_unmarshal_call = "__dm_dagstermill._load_parameter('{name}', '{val}')".format(
-                name=name, val=seven.json.dumps(val)
-            )
-            content += "{}\n".format(cls.assign(name, dm_unmarshal_call))
+        for input_name in parameters["__dm_input_names"]:
+            dm_load_input_call = f"__dm_dagstermill._load_input_parameter('{input_name}')"
+            content += "{}\n".format(cls.assign(input_name, dm_load_input_call))
 
         return content
 
 
 papermill.translators.papermill_translators.register("python", DagsterTranslator)
```

### Comparing `dagstermill-0.9.9rc1/dagstermill.egg-info/SOURCES.txt` & `dagstermill-1.0.5/dagstermill.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dagstermill/__init__.py
 dagstermill/__main__.py
 dagstermill/cli.py
+dagstermill/compat.py
 dagstermill/context.py
 dagstermill/engine.py
 dagstermill/errors.py
+dagstermill/factory.py
+dagstermill/io_managers.py
 dagstermill/manager.py
+dagstermill/py.typed
 dagstermill/serialize.py
-dagstermill/solids.py
 dagstermill/translator.py
 dagstermill/version.py
 dagstermill.egg-info/PKG-INFO
 dagstermill.egg-info/SOURCES.txt
 dagstermill.egg-info/dependency_links.txt
 dagstermill.egg-info/entry_points.txt
 dagstermill.egg-info/requires.txt
```

