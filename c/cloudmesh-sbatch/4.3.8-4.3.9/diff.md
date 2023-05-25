# Comparing `tmp/cloudmesh-sbatch-4.3.8.tar.gz` & `tmp/cloudmesh-sbatch-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-sbatch-4.3.8.tar", last modified: Sat Aug  6 14:01:10 2022, max compression
+gzip compressed data, was "cloudmesh-sbatch-4.3.9.tar", last modified: Mon Dec 12 19:00:03 2022, max compression
```

## Comparing `cloudmesh-sbatch-4.3.8.tar` & `cloudmesh-sbatch-4.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/
--rw-rw-r--   0 green     (1000) green     (1000)      769 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/LICENSE
--rw-rw-r--   0 green     (1000) green     (1000)       99 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/MANIFEST.in
--rw-rw-r--   0 green     (1000) green     (1000)    11905 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)    11125 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/README.md
--rw-rw-r--   0 green     (1000) green     (1000)        5 2022-08-06 14:00:59.000000 cloudmesh-sbatch-4.3.8/VERSION
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/cloudmesh/
--rw-rw-r--   0 green     (1000) green     (1000)       63 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/cloudmesh/__init__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/
--rw-rw-r--   0 green     (1000) green     (1000)      106 2022-08-06 14:00:59.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)       18 2022-08-06 14:00:59.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/__version__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/command/
--rw-rw-r--   0 green     (1000) green     (1000)        0 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/command/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)     8595 2022-08-06 14:00:43.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/command/sbatch.py
--rw-rw-r--   0 green     (1000) green     (1000)    22861 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/sbatch.py
--rw-rw-r--   0 green     (1000) green     (1000)     2090 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/slurm.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/
--rw-rw-r--   0 green     (1000) green     (1000)    11905 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)      589 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/SOURCES.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/dependency_links.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/namespace_packages.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/not-zip-safe
--rw-rw-r--   0 green     (1000) green     (1000)      102 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/requires.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-08-06 14:01:10.000000 cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/top_level.txt
--rw-rw-r--   0 green     (1000) green     (1000)       72 2022-08-05 23:13:08.000000 cloudmesh-sbatch-4.3.8/requirements-dev.txt
--rw-rw-r--   0 green     (1000) green     (1000)      195 2022-08-06 11:22:44.000000 cloudmesh-sbatch-4.3.8/requirements.txt
--rw-rw-r--   0 green     (1000) green     (1000)       67 2022-08-06 14:01:10.027489 cloudmesh-sbatch-4.3.8/setup.cfg
--rw-rw-r--   0 green     (1000) green     (1000)     2837 2022-08-06 11:22:44.000000 cloudmesh-sbatch-4.3.8/setup.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/
+-rw-rw-r--   0 green     (1000) green     (1000)      769 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/LICENSE
+-rw-rw-r--   0 green     (1000) green     (1000)       99 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/MANIFEST.in
+-rw-rw-r--   0 green     (1000) green     (1000)    12079 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)    11319 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/README.md
+-rw-rw-r--   0 green     (1000) green     (1000)        5 2022-12-12 18:59:49.000000 cloudmesh-sbatch-4.3.9/VERSION
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/cloudmesh/
+-rw-rw-r--   0 green     (1000) green     (1000)       63 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/cloudmesh/__init__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/
+-rw-rw-r--   0 green     (1000) green     (1000)      110 2022-12-12 18:59:49.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)       18 2022-12-12 18:59:49.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/__version__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/command/
+-rw-rw-r--   0 green     (1000) green     (1000)        0 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/command/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)    12908 2022-12-12 18:58:01.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/command/sbatch.py
+-rw-rw-r--   0 green     (1000) green     (1000)    22724 2022-12-12 18:56:00.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/sbatch.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2093 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/slurm.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/
+-rw-rw-r--   0 green     (1000) green     (1000)    12079 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)      589 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/namespace_packages.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/not-zip-safe
+-rw-rw-r--   0 green     (1000) green     (1000)      102 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/requires.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-12-12 19:00:03.000000 cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/top_level.txt
+-rw-rw-r--   0 green     (1000) green     (1000)      247 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/requirements-dev.txt
+-rw-rw-r--   0 green     (1000) green     (1000)      196 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/requirements.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       67 2022-12-12 19:00:03.151609 cloudmesh-sbatch-4.3.9/setup.cfg
+-rw-rw-r--   0 green     (1000) green     (1000)     2837 2022-10-19 00:04:05.000000 cloudmesh-sbatch-4.3.9/setup.py
```

### Comparing `cloudmesh-sbatch-4.3.8/LICENSE` & `cloudmesh-sbatch-4.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-sbatch-4.3.8/PKG-INFO` & `cloudmesh-sbatch-4.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cloudmesh-sbatch
-Version: 4.3.8
+Version: 4.3.9
 Summary: A command called sbatch and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-sbatch
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -338,8 +337,12 @@
 
 ```
 
 ### Cheatsheet
 
 * <https://slurm.schedmd.com/pdfs/summary.pdf>
 
+## Acknowledgements
 
+Continued work was in part funded by the NSF
+CyberTraining: CIC: CyberTraining for Students and Technologies
+from Generation Z with the awadrd numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-sbatch-4.3.8/README.md` & `cloudmesh-sbatch-4.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -316,7 +316,13 @@
 Valid states are: NoResp DRAIN FAIL FUTURE RESUME POWER_DOWN POWER_UP UNDRAIN
 
 ```
 
 ### Cheatsheet
 
 * <https://slurm.schedmd.com/pdfs/summary.pdf>
+
+## Acknowledgements
+
+Continued work was in part funded by the NSF
+CyberTraining: CIC: CyberTraining for Students and Technologies
+from Generation Z with the awadrd numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/sbatch.py` & `cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/sbatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,627 +1,699 @@
 import itertools
 import json
 import os
 import pathlib
-import tempfile
-import textwrap
 import typing
-import yaml
 import uuid
-
 from collections import OrderedDict
 from datetime import datetime
 from pprint import pprint
 
+import yaml
 from nbconvert.exporters import PythonExporter
 
 from cloudmesh.common.FlatDict import FlatDict
 from cloudmesh.common.Printer import Printer
 from cloudmesh.common.Shell import Shell
 from cloudmesh.common.console import Console
 from cloudmesh.common.parameter import Parameter
-from cloudmesh.common.util import banner, readfile, writefile, yn_choice
+from cloudmesh.common.util import banner, readfile, writefile
 from cloudmesh.common.variables import Variables
 
 PathLike = typing.Union[str, pathlib.Path]
 DictOrList = typing.Union[dict, list]
 OptPath = typing.Optional[PathLike]
 OptStr = typing.Optional[str]
 
 
 class SBatch:
 
     def __init__(self, verbose=False):
-        self.name = None
+        """
+        Initialize the SBatch Object
+
+        :param verbose: If true prints additional infromation when SBatch methods are called
+        :type verbose: bool
+        """
+        self.flat = FlatDict({}, sep=".")
         self.data = dict()
         self.permutations = list()
-        self.template = None
+        self.experiments = None
+        self.dryrun = False
+        self.verbose = False
+        self.execution_mode = "h"
+        self.input_dir = str(Shell.map_filename(".").path)
+        self.output_dir = str(Shell.map_filename(".").path)
+        self.os_variables = None
         self.verbose = verbose
-        # self.gpu = None
-        self.attributes = dict()
-        self.configuration_parameters = None
         self.template_path = None
         self.template_content = None
-        self.out_directory = None
+        self.configuration_parameters = None
         self.script_out = None
-        self.execution_mode = None
-        self.source = None
-        self.dryrun = None
+        # self.gpu = None
 
-    def config_from_cli(self, arguments: typing.Any):
-        """Configures the object from command.sbatch CLI arguments
+    def info(self, verbose=None):
+        """
+        Prints information about the SBatch object for debugging purposes
 
-        Args:
-            arguments: The docopts object from the cms sbatch command.
+        :param verbose:  if True prints even more information
+        :type verbose: bool
+        :return: None
+        :rtype: None
+        """
+        verbose = verbose or self.verbose
+
+        if not verbose:
+            return
+
+        for a in [
+            "dryrun",
+            "verbose",
+            "name",
+            "source",
+            "destination",
+            "attributes",
+            "gpu",
+            "config",
+            "config_files",
+            "directory",
+            "experiment",
+            "execution_mode",
+            "template",
+            "script_output",
+            "output_dir",
+            "input_dir",
+            "script_in",
+            "script_out",
+            "os_variables",
+            "experiments"
+        ]:
+            try:
+                result = getattr(self, a)
+            except:  # noqa: E722
+                result = self.data.get(a)
+            print(f'{a:<12}: {result}')
+        print("permutations:")
 
-        Returns:
-            Fluent API of the current object.
+        result = getattr(self, "permutations")
+        pprint(result)
+
+        print("BEGIN FLAT")
+        pprint(self.flat)
+        print("END FLAT")
+        print()
+
+        print("BEGIN DATA")
+        pprint(self.data)
+        print("END DATA")
+        print()
+
+        print("BEGIN YAML")
+        spec = yaml.dump(self.data, indent=2)
+        print(spec)
+        print("END YAML")
+
+        print("BEGIN SPEC")
+        spec = self.spec_replace(spec)
+        print(spec)
+        print("END SPEC")
+        print("BEGIN PERMUTATION")
+        p = self.permutations
+        pprint(p)
+        print("END PERMUTATION")
+
+        # self.info()
+        #
+        # self.data = result
+        #
+        print("BEGIN DATA")
+        pprint(self.data)
+        print("END DATA")
+
+        banner("BEGIN TEMPLATE")
+        print(self.template_content)
+        banner("END TEMPLATE")
+
+    @staticmethod
+    def update_with_directory(directory, filename):
         """
-        if arguments.get('SOURCE') is not None:
-            self.source = arguments.get('SOURCE')
-            self.register_script(self.source)
-        self.dryrun = arguments.get('dryrun', self.dryrun)
-        if self.execution_mode is None:
-            self.execution_mode = arguments.mode
+        prefix with the directory if the filename is not starting with . / ~
 
-        if self.script_out is None and arguments.out is None:
-            self.script_out = pathlib.Path(self.source).name.replace(".in.", ".")  #.replace(".in", "")
+        :param directory: the string value of the directory
+        :type directory: str
+        :param filename: the filename
+        :type filename: str
+        :return: directory/filename
+        :rtype: str
+        """
+        if directory is None:
+            return filename
+        elif not filename.startswith("/") and not filename.startswith(".") and not filename.startswith("~"):
+            return f"{directory}/{filename}"
         else:
-            self.script_out = pathlib.Path(arguments.get('out', self.script_out)).name
+            return filename
 
-        if self.source == self.script_out:
-            if not yn_choice("The source and destination filenames are the same. Do you want to continue?"):
-                return ""
-
-        if arguments['--dir']:
-            self.out_directory = arguments['--dir']
-
-        if not arguments["--noos"]:
-            self.update_from_os_environ()
-
-        if not arguments["--nocm"]:
-            self.update_from_cm_variables()
-
-        if arguments.attributes:
-            self.update_from_attributes(arguments.attributes)
-
-        if arguments.experiment:
-            self.permutations = self.generate_experiment_permutations(arguments.experiment)
-
-        if arguments.config:
-            for config_file in Parameter.expand(arguments.config):
-                self.update_from_file(config_file)
-            self.update_from_dict({ 'meta.parent.uuid': str(uuid.uuid4()) })
-        return self
-
-    @classmethod
-    def _apply_leaf(cls, my_dict: DictOrList, my_lambda: typing.Callable, *args, **kwargs) -> dict:
-        """Walks python dictionary and applies a lambda to all leaf nodes.
-        Args:
-            my_dict: The dictionary to process
-            my_lambda: The lambda function to apply to the leaf nodes.
-            *args: positional arguments passed directly to my_lambda
-            **kwargs: keyword arguments passed directoy to my_lambda
-        Returns:
-            A new dictionary that has applied the my_lambda function on
-            each leaf node.
-        """
-        new_dict = dict(my_dict)
-        for key, value in new_dict.items():
-            if isinstance(value, dict):
-                new_dict[key] = cls._apply_leaf(value, my_lambda, *args, **kwargs)
-            elif isinstance(value, list):
-                inner_list = list()
-                for x in value:
-                    if isinstance(x, dict) or isinstance(x, list):
-                        inner_list.append(cls._apply_leaf(x, my_lambda, *args, **kwargs))
-                    else:
-                        inner_list.append(my_lambda(x, **kwargs))
-                    new_dict[key] = inner_list
-            else:
-                new_dict[key] = my_lambda(str(value), *args, **kwargs)
-        return new_dict
+    def get_data(self, flat=False):
+        result = self.data
 
-    def config_from_yaml(self, yaml_file: PathLike):
-        """Configures the object from a standard YAML structure.
+        if flat:
+            from cloudmesh.common.FlatDict import FlatDict
+            result = FlatDict(self.data, sep=".")
+            del result["sep"]
 
-        This supports the following YAML structures:
-            template: path
-            config: path
-            name: str
-            experiments:
-              card_name: Parameter.expand string
-              gpu_count: Parameter.expand string
-              cpu_num: Parameter.expand string
-              mem: Parameter.expand string
-            attributes:
-              property: substitution
-            mode: str
-            dir: path
+        return result
 
-        Args:
-            yaml_file: The path to the yaml file to parse
+    def spec_replace(self, spec):
+        """
+        given a spec in yaml format, replaces all values in the yaml file taht are of the form "{a.b}"
+        with the value of
 
-        Returns:
-            Fluent API of the current object.
+        a:
+           b: value
+
+        if it is defined in the yaml file
+
+        :param spec: yaml string
+        :type spec: str
+        :return: replaced yaml file
+        :rtype: str
         """
+        import re
+        import munch
+        variables = re.findall(r"\{\w.+\}", spec)
 
-        with open(yaml_file, 'rb') as f:
-            yaml_data = yaml.safe_load(f)
+        banner("GGGGGGGGGGGGGGGGGGGGGGG")
 
-        self.read_config_from_dict(yaml_data)
+        data = yaml.load(spec, Loader=yaml.SafeLoader)
 
-        return self
-
-    def read_config_from_dict(self, root):
-        if 'template' in root:
-            self.source = root['template']
-            self.register_script(root['template'])
-        if 'config' in root:
-            self.update_from_file(root['config'])
-        if 'name' in root:
-            self.name = root['name']
-        if 'mode' in root:
-            self.execution_mode = root['mode']
-        if 'dir' in root:
-            self.out_directory = root['dir']
-        if 'experiments' in root:
-            experiments = self._apply_leaf(root['experiments'], Parameter.expand)
-            perms = self.permutation_generator(experiments)
-            self.permutations = self.permutations + perms
-        # if 'attributes' in root:
-        self.update_from_dict(FlatDict(root, sep="."))
-        self.update_from_dict({ 'meta.parent.uuid': str(uuid.uuid4()) })
+        pprint(data)
+        banner("RRRRRRRRRRRRRRRRRRRRRRRRR")
+        m = munch.DefaultMunch.fromDict(data)
 
-    def register_script(self, script):
-        """Registers and reads the template script in for processing
+        for i in range(0, len(variables)):
 
-        This method must be run at least once prior to generating the slurm script output.
+            for variable in variables:
+                text = variable
+                variable = variable[1:-1]
+                try:
+                    value = eval("m.{variable}".format(**locals()))
+                    if "{" not in value:
+                        spec = spec.replace(text, value)
+                except:  # noqa: E722
+                    value = variable
 
-        Args:
-            script: A string that is the path to the template script.
 
-        Returns:
-            The text of the template file unaltered.
+        banner("UUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUU")
+        pprint(spec)
+        return spec
+
+    def update_from_os(self, variables):
+        """
+        LOads all variables from os.environ into self.data with os.name
+
+        :param variables: tha name of the variables such as "HOME"
+        :type variables:  [str]
+        :return: self.data with all variaples added with os.name: value
+        :rtype: dict
+        """
+        if variables is not None:
+            if os not in self.data:
+                self.data["os"] = {}
+            for key in variables:
+                self.data["os"][key] = os.environ[key]
+        return self.data
+
+    def load_source_template(self, script):
+        """
+        Registers and reads the template script in for processing
+
+        This method must be run at least once prior to generating the batch script output.
+
+        :param script: A string that is the path to the template script.
+        :type script: str
+        :return: The text of the template file unaltered.
+        :rtype: str
         """
         self.template_path = script
         self.template_content = readfile(script)
         return self.template_content
 
-    def info(self):
-        for a in ["source",
-                    "destination",
-                    "attributes",
-                    "gpu",
-                    "dryrun",
-                    "config",
-                    "directory",
-                    "experiment",
-                    "mode"
-                  ]:
-            try:
-                result = getattr(self,a)
-            except:
-                result = self.data.get(a)
-            print(f'{a:<12}: {result}')
-        print("permutations:")
-        result = getattr(self, "permutations")
-        # pprint(result)
-        print()
-
-    def set_attribute(self, attribute, value):
-        self.data[attribute] = value
-
     def update_from_dict(self, d):
+        """
+        Add a dict to self. data
+
+        :param d: dictionary
+        :type d: dict
+        :return: self.data with updated dict
+        :rtype: dict
+        """
         self.data.update(d)
+        return self.data
 
     def update_from_attributes(self, attributes: str):
-        """attributes are of the form "a=1,b=3"
-
-        Args:
-            attributes: A string to expand into key-value pairs
-        Returns:
-            dict[str,str]: The expanded dictionary
         """
-        entries = Parameter.arguments_to_dict(attributes)
-        self.update_from_dict(entries)
-        return entries
-
-    def update_from_os_environ(self, load=True):
-        """Updates the config file output to include OS environment variables
-        Args:
-            load: When true, loads the environment variables into the config.
-        Returns:
-            The current value of the data configuration variable
+        attributes are of the form "a=1,b=3"
+
+        :param attributes: A string to expand into key-value pairs
+        :type attributes:
+        :return: self.data with updated dict
+        :rtype: dict
         """
-        if load:
-            self.update_from_dict(dict(os.environ))
+        flatdict = Parameter.arguments_to_dict(attributes)
+
+        d = FlatDict(flatdict, sep=".")
+        d = d.unflatten()
+        del d["sep"]
+
+        self.update_from_dict(d)
         return self.data
 
-    def update_from_cm_variables(self, load: bool = True) -> typing.Dict[str, typing.Any]:
-        """Adds Cloudmesh variables to the class's data parameter as a flat dict.
+    def update_from_os_environ(self):
+        """
+        Updates the config file output to include OS environment variables
+
+        :return: The current value of the data configuration variable
+        :rtype: dict
+        """
+        self.update_from_dict(dict(os.environ))
+        return self.data
 
-        Args:
-            load: Toggles execution; if false, method does nothing.
+    def update_from_cm_variables(self, load=True):
+        """
+        Adds Cloudmesh variables to the class's data parameter as a flat dict.
 
-        Returns:
-            The updated data parameter with the cloudmesh variables set.
+        :param load: Toggles execution; if false, method does nothing.
+        :type load: bool
+        :return: self.data with updated cloudmesh variables
+        :rtype: dict
         """
         if load:
             variables = Variables()
             v = FlatDict({"cloudmesh": variables.dict()}, sep=".")
-
-            self.update_from_dict(dict(v))
+            d = v.unflatten()
+            del d["sep"]
+            self.update_from_dict(d)
         return self.data
 
     @staticmethod
-    def _suffix(path: str) -> str:
-        """Returns the file suffix of a path
-
-        Args:
-            path: The path to process
-
-        Returns:
-            str: The suffix of the string
+    def _suffix(filename):
         """
-        return pathlib.Path(path).suffix
 
-    def update_from_file(self, filename: PathLike):
-        """Updates the run configuration file with the data within the passed file.
+        :param filename: Returns the file suffix of a filename
+        :type filename: str
+        :return: the suffix of the filename
+        :rtype: str
+        """
+        return pathlib.Path(filename).suffix
 
-        Args:
-            filename: The path to the configuration file (json or yaml)
+    def update_from_file(self, filename):
+        """
+        Updates the configuration self.data with the data within the passed file.
 
-        Returns:
-            The modified data object.
+        :param filename: The path to the configuration file (yaml, json, py, ipynb)
+        :type filename: str
+        :return: self.data with updated cloudmesh variables from the specified file
+        :rtype: dict
         """
         if self.verbose:
             print(f"Reading variables from {filename}")
 
-        suffix = self._suffix(filename)
+        suffix = self._suffix(filename).lower()
         content = readfile(filename)
 
-        if suffix.lower() in [".json"]:
-            regular_dict = json.loads(content)
-            values = dict(FlatDict(regular_dict, sep="."))
-        elif suffix.lower() in [".yml", ".yaml"]:
+        if suffix in [".json"]:
+            values = json.loads(content)
+
+        elif suffix in [".yml", ".yaml"]:
             content = readfile(filename)
-            regular_dict = yaml.safe_load(content)
-            values = dict(FlatDict(regular_dict, sep="."))
-        elif suffix.lower() in [".py"]:
+            values = yaml.safe_load(content)
 
-            modulename = filename.replace(".py","").replace("/","_").replace("build_", "")
+        elif suffix in [".py"]:
+
+            modulename = filename.replace(".py", "").replace("/", "_").replace("build_", "")
             from importlib.machinery import SourceFileLoader
 
             mod = SourceFileLoader(modulename, filename).load_module()
 
-            regular_dict = {}
+            values = {}
             for name, value in vars(mod).items():
                 if not name.startswith("__"):
-                    print (name, value)
-                    regular_dict[name] = value
-            values = dict(FlatDict(regular_dict, sep="."))
-
-        elif suffix.lower() in [".ipynb"]:
-            # regular_dict = None
-            # values = None
+                    values[name] = value
+
+        elif suffix in [".ipynb"]:
 
             py_name = filename.replace(".ipynb", ".py")
             jupy = PythonExporter()
             body, _ = jupy.from_filename(filename)
             writefile(py_name, body)
             # Shell.run(f"jupyter nbconvert --to python {filename}")
 
             filename = py_name
-            modulename = filename.replace(".py","").replace("/","_").replace("build_", "")
+            modulename = filename.replace(".py", "").replace("/", "_").replace("build_", "")
             from importlib.machinery import SourceFileLoader
 
             mod = SourceFileLoader(modulename, filename).load_module()
 
-            regular_dict = {}
+            values = {}
             for name, value in vars(mod).items():
                 if not name.startswith("__"):
-                    print(name, value)
-                    regular_dict[name] = value
+                    values[name] = value
 
-            values = dict(FlatDict(regular_dict, sep="."))
         else:
             raise RuntimeError(f"Unsupported config type {suffix}")
 
-        self.read_config_from_dict(regular_dict)
-        if regular_dict is not None and 'experiments' in regular_dict:
-            exp_values = regular_dict['experiments']
-
-            banner(str(exp_values))
-
-            if isinstance(exp_values, dict):
-                entries = []
-                for key, value in exp_values.items():
-                    entry = f"{key}={value}"
-                    entries.append(entry)
-                exp_values = " ".join(entries)
+        self.update_from_dict(values)
 
-            elif isinstance(exp_values, str):
-                banner(f"Generate permutations from experiment in {filename}")
-            else:
-                Console.error(f"experiment datatype {type(exp_values)} for {exp_values} not supported")
-            experiments = self._apply_leaf(regular_dict['experiments'], Parameter.expand)
-            perms = self.permutation_generator(experiments)
-            self.permutations = self.permutations + perms
-            # self.generate_experiment_permutations(experiments)
+        # self.read_config_from_dict(regular_dict)
+        if values is not None and 'experiment' in values:
+            experiments = values['experiment']
+
+            for key, value in experiments.items():
+                print (key, value)
+                try:
+                    experiments[key] = Parameter.expand(value)
+                except:
+                    experiments[key] = [value]
 
-        # if values is not None:
-        #     self.update_from_dict(experiments)
+            self.permutations = self.permutation_generator(experiments)
 
         return self.data
 
-    def generate(self, script, data=None, fences=("{", "}")):
-        """Expands the script template given the passed configuration.
+    def generate(self, script=None, variables=None, fences=("{", "}")):
+        """
+        Expands the script template given the passed configuration.
 
-        Args:
-            script: The string contents of the script file.
-            data: A single-level dictionary used to replace strings that match the key with its values.
-            fences: A 2 position tuple, that encloses template variables (start and end).
+        :param script: The string contents of the script file.
+        :type script: str
+        :param variables: the variables to be replaced, if ommitted uses the internal variables found
+        :type variables: dict
+        :param fences: A 2 position tuple, that encloses template variables (start and end).
+        :type fences: (str,str)
+        :return: The script that has expanded its values based on `data`.
+        :rtype: str
+        """
+
+        replaced = {}
+
+        if variables is None:
+            variables = self.data
+        if script is None:
+            script = self.template_content
+        content = str(script)
+        flat = FlatDict(variables, sep=".")
 
-        Returns:
-            The script that has expanded its values based on `data`.
-        """
-        if data is None:
-            data = self.data
-        content = self.template_content
-        for attribute, value in data.items():
+        for attribute in flat:
+            value = flat[attribute]
             frame = fences[0] + attribute + fences[1]
-            if self.verbose:
-                print(f"Expanding {frame} with {value}")
-            # print(content)
             if frame in content:
+                if self.verbose:
+                    print(f"- Expanding {frame} with {value}")
+                replaced[attribute] = value
                 content = content.replace(frame, str(value))
-        return content
+        return content, replaced
 
     @staticmethod
-    def permutation_generator(exp_dict: dict) -> list:
-        """Creates a cartisian product of a {key: list, ...} object.
-
-        Args:
-            exp_dict: The dictionary to process
+    def permutation_generator(exp_dict):
+        """
+        Creates a cartisian product of a {key: list, ...} object.
 
-        Returns:
-            A list of dictionaries containing the resulting cartisian product.
+        :param exp_dict: The dictionary to process
+        :type exp_dict: dict
+        :return: A list of dictionaries containing the resulting cartisian product.
+        :rtype: list
 
         For example
             my_dict = {"key1": ["value1", "value2"], "key2": ["value3", "value4"]}
             out = permutation_generator(my_dict)
             out # [{"key1": "value1", "key2": 'value3"},
                 #  {"key1": "value1", "key2": "value4"},
                 #  {"key1": "value2", "key2": "value3"},
                 #  {"key1": "value2", "key2": "value4"}
+
         """
         keys, values = zip(*exp_dict.items())
         return [dict(zip(keys, value)) for value in itertools.product(*values)]
 
     def generate_experiment_permutations(self, variable_str):
-        """Generates experiment permutations based on the passed string and appends it to the current instance.
-
-        Args:
-            variable_str: A Parameter.expand string (such as epoch=[1-3] x=[1,4] y=[10,11])
+        """
+        Generates experiment permutations based on the passed string and appends it to the current instance.
 
-        Returns:
-            list with permutations over the experiment variables
+        :param variable_str: A Parameter.expand string (such as epoch=[1-3] x=[1,4] y=[10,11])
+        :type variable_str: str
+        :return: list with permutations over the experiment variables
+        :rtype: list
         """
         experiments = OrderedDict()
         entries = variable_str.split(' ')
 
-        # pprint(entries)
         for entry in entries:
             k, v = entry.split("=")
             experiments[k] = Parameter.expand(v)
         self.permutations = self.permutation_generator(experiments)
         return self.permutations
 
-    #for permutation in self.permutations:
-    #    values = ""
-    #    for attribute, value in permutation.items():
-    #        values = values + f"{attribute}={value} "
-    #        script = f"{self.destination}{values}".replace("=", "_")
-    #    print(f"{values} sbatch {self.destination} {script}")
-
     @staticmethod
     def _generate_bootstrapping(permutation):
+        """
+        creates an identifier, a list of assignments, ad values.
+
+        :param permutation: the permutation list
+        :type permutation: list
+        :return: identifier, assignments, values
+        :rtype: str, list, list
+        """
         values = list()
         for attribute, value in permutation.items():
             values.append(f"{attribute}_{value}")
         assignments = list()
         for attribute, value in permutation.items():
             assignments.append(f"{attribute}={value}")
         assignments = " ".join(assignments)
 
         identifier = "_".join(values)
         return identifier, assignments, values
 
-    def _generate_flat_config(self):
-
-        configuration = dict()
-        # self.script_variables = list()
-        suffix = self._suffix(self.script_out)
-        name = self.script_out.replace(suffix, "")
-        # directory = os.path.dirname(name)
-        directory = self.out_directory
-        for permutation in self.permutations:
-            identifier, assignments, values = self._generate_bootstrapping(permutation)
-            print(identifier)
-            script = f"{directory}/{name}_{identifier}{suffix}"
-            config = f"{directory}/config_{identifier}.yaml"
-            variables = dict(self.data)
-            variables.update(FlatDict({'experiments': permutation}, sep="."))
-
-            configuration[identifier] = {
-                "id"        : identifier,
-                "directory" : directory,
-                "experiment": assignments,
-                "script"    : script,
-                "config"    : config,
-                "variables" : variables
-            }
-        return configuration
+    # def _generate_flat_config(self):
+    #     """
+    #     deprecated. IT is no longer supported
+    #
+    #     Creates a flat configuration file.
+    #
+    #     :return: dict with information where the variables are a flatdict
+    #     :rtype: dict
+    #     """
+    #
+    #     configuration = dict()
+    #     # self.script_variables = list()
+    #     suffix = self._suffix(self.script_out)
+    #     spec = yaml.dump(self.data, indent=2)
+    #     spec = self.spec_replace(spec)
+    #
+    #     directory = self.output_dir
+    #     for permutation in self.permutations:
+    #         identifier, assignments, values = self._generate_bootstrapping(permutation)
+    #
+    #         spec = yaml.dump(self.data, indent=2)
+    #         spec = self.spec_replace(spec)
+    #
+    #         variables = yaml.safe_load(spec)
+    #
+    #         name = os.path.basename(self.script_out)
+    #         script = f"{directory}/{name}_{identifier}{suffix}"
+    #         config = f"{directory}/config_{identifier}.yaml"
+    #
+    #         variables.update({'experiment': permutation})
+    #         variables["sbatch"]["idenitfier"] = identifier
+    #
+    #         configuration[identifier] = {
+    #             "id": identifier,
+    #             "directory": directory,
+    #             "experiment": assignments,
+    #             "script": script,
+    #             "config": config,
+    #             "variables": variables
+    #         }
+    #     return configuration
 
     def _generate_hierarchical_config(self):
+        """
+        Creates a hierarchical directory with configuration yaml files, and shell script
+
+        :return: directory with configuration and yaml files
+        :rtype: dict
+        """
         """Runs process to build out all templates in a hierarchical-style
 
         Returns:
             None.
 
         Side Effects:
             Writes two files for each established experiment, each in their own directory.
 
         """
-        print("Outputting Hierarchical Experiments")
+        if self.verbose:
+            print("Outputting Hierarchical Experiments")
         configuration = dict()
         self.script_variables = []
         suffix = self._suffix(self.script_out)
-        # name = self.script_out.replace(suffix, "")
-        directory = self.out_directory  # .path.dirname(name)
+        directory = self.output_dir  # .path.dirname(name)
         for permutation in self.permutations:
+
             identifier, assignments, values = self._generate_bootstrapping(permutation)
-            print(identifier)
-            script = f"{directory}/{identifier}/slurm.sh"
+
+            if self.verbose:
+                print(identifier, assignments, values)
+
+            spec = yaml.dump(self.data, indent=2)
+            spec = self.spec_replace(spec)
+
+            variables = yaml.safe_load(spec)
+
+            name = os.path.basename(self.script_out)
+            script = f"{directory}/{identifier}/{name}"
             config = f"{directory}/{identifier}/config.yaml"
-            variables = dict(self.data)
-            variables.update(FlatDict({'experiments': permutation}, sep="."))
+
+            variables.update({'experiment': permutation})
+            variables["sbatch"]["identifier"] = identifier
 
             configuration[identifier] = {
-                "id"        : identifier,
-                "directory" : f"{directory}/{identifier}",
+                "id": identifier,
+                "directory": f"{directory}/{identifier}",
                 "experiment": assignments,
-                "script"    : script,
-                "config"    : config,
-                "variables" : variables
+                "script": script,
+                "config": config,
+                "variables": variables
             }
-            # pprint(configuration)
         return configuration
 
-    def generate_experiment_slurm_scripts(self, out_mode=None):
-        """Utility method to genrerate either hierarchical or flat outputs; or debug.
-
-        Args:
-            mode: The mode of operation.  One of: "debug", "flat", "hierarchical"
+    def generate_experiment_batch_scripts(self, out_mode=None):
+        """
+        Utility method to genrerate either hierarchical or flat outputs; or debug.
 
-        Returns:
+        NOte the falt mode is no longer supported
 
+        :param out_mode: The mode of operation.  One of: "debug", "flat", "hierarchical"
+        :type out_mode: string
+        :return: generates the batch scripts
+        :rtype: None
         """
         mode = self.execution_mode if out_mode is None else out_mode.lower()
         if mode.startswith("d"):
             Console.warning("This is just debug mode")
             print()
             for permutation in self.permutations:
                 values = ""
                 for attribute, value in permutation.items():
                     values = values + f"{attribute}={value} "
-                script = f"{self.out_directory}/{self.script_out}{values}".replace("=", "_")
+                script = f"{self.output_dir}/{self.script_out}{values}".replace("=", "_")
         else:
             if mode.startswith("f"):
-                configuration = self._generate_flat_config()
+                Console.error("Flat mode is no longer supported", traceflag=True)
+                # configuration = self._generate_flat_config()
             elif mode.startswith("h"):
                 configuration = self._generate_hierarchical_config()
             else:
                 raise RuntimeError(f"Invalid generator mode {mode}")
+            if self.verbose:
+                banner("Script generation")
 
-            banner("Script generation")
             print(Printer.write(configuration, order=["id", "experiment", "script", "config", "directory"]))
 
             self.configuration_parameters = configuration
+
             self.generate_setup_from_configuration(configuration)
 
-    def generate_submit(self, name=None, type_='slurm'):
-        if type_ == 'slurm':
+    def generate_submit(self, name=None, job_type='slurm'):
+        """
+        Generates a list of commands based on the permutations for submission
+
+        :param name: Name of the experiments
+        :type name: str
+        :param job_type: name of the job type used at submission such as
+                         sbatch, slurm, jsrun, mpirun, sh, bash
+        :type job_type: str
+        :param verbose: prints the generated command lines
+        :type verbose: bool
+        :return: prepars the internal data for the experiments, if set to verbose, prints them
+        :rtype: None
+        """
+
+        if ".json" not in name:
+            name = f"{name}.json"
+
+        if job_type == 'slurm':
             cmd = 'sbatch'
-        elif type_ == 'lsf':
+        elif job_type == 'lsf':
             cmd = 'bsub'
         else:
-            raise RuntimeError(f"Unsupported submission type {type_}")
+            cmd = job_type
+
+        # else:
+        #    raise RuntimeError(f"Unsupported submission type {type_}")
 
         experiments = json.loads(readfile(name))
 
+       #  print (experiments)
+
         if experiments is None:
             Console.error("please define the experiment parameters")
             return ""
 
         for entry in experiments:
+            if self.verbose:
+                print(f"# Generate {entry}")
             experiment = experiments[entry]
             parameters = experiment["experiment"]
             directory = experiment["directory"]
             script = os.path.basename(experiment["script"])
-            print(f"( {parameters} cd {directory} && {cmd} {script} )")
+            print(f"{parameters} cd {directory} && {cmd} {script}")
 
     def generate_setup_from_configuration(self, configuration):
-        # pprint(configuration)
         for identifier in configuration:
-            perm_uuid = str(uuid.uuid4())
-            Console.info(f"setup experiment {identifier}")
             experiment = configuration[identifier]
             Shell.mkdir(experiment["directory"])
-            print(f"Making dir {experiment['directory']}")
-            #
-            # Generate config.yml
-            #
-            Console.info(f"* write file {experiment['config']}")
+            if self.verbose:
+                print()
+                Console.info(f"Setup experiment {identifier}")
+                print(f"- Making dir {experiment['directory']}")
+                print(f"- write file {experiment['config']}")
 
             # Generate UUID for each perm
-            experiment["variables"].update({ 'meta.uuid': perm_uuid })
+            experiment["variables"]['sbatch']['uuid'] = str(uuid.uuid4())
+
             writefile(experiment["config"], yaml.dump(experiment["variables"], indent=2))
             content_config = readfile(experiment["config"])
             try:
                 check = yaml.safe_load(content_config)
             except Exception as e:
-                print (e)
+                print(e)
                 Console.error("We had issues with our check for the config.yaml file")
-            #
-            # Generate slurm.sh
-            #
-            content_script = readfile(self.source)
-            content_script = self.generate(content_script, experiment["variables"])
+
+            content_script, replaced = self.generate(self.template_content, variables=experiment["variables"])
+
+            # if self.verbose:
+            #    for attribute, value in replaced.items():
+            #        print (f"- replaced {attribute}={value}")
+
             writefile(experiment["script"], content_script)
 
     @property
     def now(self):
+        """
+        The time of now in the format "%Y-m-%d"
+        :return: "%Y-m-%d"
+        :rtype: str
+        """
         return datetime.now().strftime("%Y-m-%d")
 
-    def debug_state(self, key=""):
-        """Outputs the current state of persistent values in class.
-        Args:
-            key: A string to prefix the string with.
-        Returns:
-            A mutliline string with all class variables in a key = value pattern.
+    def save_experiment_configuration(self, name=None):
         """
-        return textwrap.dedent(f"""
-        {key}===OBJ===
-        {key}   {self.name = }
-        {key}   {self.data = }
-        {key}   {self.verbose = }
-        {key}   {self.source = }
-        {key}   {self.script_out = }
-        {key}   {self.out_directory = }
-        {key}   {self.attributes = }
-        {key}   {self.dryrun = }
-        {key}   {self.execution_mode = }
-        {key}   {self.permutations = }
-        {key}   {self.configuration_parameters = }
-        {key}   {self.template_path = }
-        {key}===END===""")
+        Saves the experiment configuration in a json file
 
-    # def __str__(self):
-    #     return self.content
-    #
-    # def save_slurm_script(self, filename):
-    #     """
-    #     Writes the custom slurm script to a file for submission
-    #     If the file already exists, the user will be prompted to override
-    #     """
-    #     if os.path.exists(path_expand(filename)):
-    #         if yn_choice(f"{filename} exists, would you like to overwrite?"):
-    #             writefile(filename, self.content)
-    #     else:
-    #         writefile(filename, self.content)
-
-    def save_experiment_configuration(self, name=None):
+        :param name: name of the configuration file
+        :type name: str
+        :return: writes into the file with given name the json content
+        :rtype: None
+        """
         if name is not None:
             content = json.dumps(self.configuration_parameters, indent=2)
             writefile(name, content)
```

### Comparing `cloudmesh-sbatch-4.3.8/cloudmesh/sbatch/slurm.py` & `cloudmesh-sbatch-4.3.9/cloudmesh/sbatch/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 The API reflects what we do on the commandline and we have the methods::
 
     Slurm.start()
     Slurm.stop()
     Slurm.status()
 """
 import os
+
 from cloudmesh.common.util import banner
 
+
 class Slurm:
 
     @staticmethod
     def start():
         """
         Starts the SLurm service oon your local machine.
 
@@ -75,8 +77,8 @@
             On stdout prints the action information
         """
 
         for command in ["sudo tail /var/log/slurm-llnl/slurmd.log",
                         "sudo tail /var/log/slurm-llnl/slurmctld.log",
                         "sinfo -R"]:
             banner(command)
-            os.system(command)
+            os.system(command)
```

### Comparing `cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/PKG-INFO` & `cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cloudmesh-sbatch
-Version: 4.3.8
+Version: 4.3.9
 Summary: A command called sbatch and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-sbatch
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -338,8 +337,12 @@
 
 ```
 
 ### Cheatsheet
 
 * <https://slurm.schedmd.com/pdfs/summary.pdf>
 
+## Acknowledgements
 
+Continued work was in part funded by the NSF
+CyberTraining: CIC: CyberTraining for Students and Technologies
+from Generation Z with the awadrd numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-sbatch-4.3.8/cloudmesh_sbatch.egg-info/SOURCES.txt` & `cloudmesh-sbatch-4.3.9/cloudmesh_sbatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-sbatch-4.3.8/setup.py` & `cloudmesh-sbatch-4.3.9/setup.py`

 * *Files identical despite different names*

