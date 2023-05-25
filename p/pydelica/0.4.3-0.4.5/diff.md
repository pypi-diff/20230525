# Comparing `tmp/pydelica-0.4.3.tar.gz` & `tmp/pydelica-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelica-0.4.3.tar", max compression
+gzip compressed data, was "pydelica-0.4.5.tar", max compression
```

## Comparing `pydelica-0.4.3.tar` & `pydelica-0.4.5.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0     1085 2022-01-27 10:34:13.422473 pydelica-0.4.3/LICENSE
--rw-r--r--   0        0        0     7619 2022-03-09 11:22:25.410089 pydelica-0.4.3/README.md
--rw-r--r--   0        0        0    19351 2022-03-09 08:38:44.538487 pydelica-0.4.3/pydelica/__init__.py
--rw-r--r--   0        0        0    12057 2022-03-09 11:17:02.910102 pydelica-0.4.3/pydelica/compiler.py
--rw-r--r--   0        0        0       12 2022-03-07 11:12:12.744636 pydelica-0.4.3/pydelica/environment.py
--rw-r--r--   0        0        0     3029 2022-03-08 08:30:01.632873 pydelica-0.4.3/pydelica/exception.py
--rw-r--r--   0        0        0      319 2022-01-27 11:04:56.618619 pydelica-0.4.3/pydelica/logger.py
--rw-r--r--   0        0        0     5659 2022-03-09 08:38:44.538487 pydelica-0.4.3/pydelica/model.py
--rw-r--r--   0        0        0     8518 2022-05-04 06:49:28.478120 pydelica-0.4.3/pydelica/options.py
--rw-r--r--   0        0        0     1685 2022-03-08 08:30:01.632873 pydelica-0.4.3/pydelica/solutions.py
--rw-r--r--   0        0        0     1002 2022-05-04 06:49:37.042136 pydelica-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8564 2022-05-04 06:52:45.203705 pydelica-0.4.3/setup.py
--rw-r--r--   0        0        0     8642 2022-05-04 06:52:45.204171 pydelica-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-11-14 22:38:00.294697 pydelica-0.4.5/LICENSE
+-rw-r--r--   0        0        0    21965 2023-05-25 18:38:06.637421 pydelica-0.4.5/pydelica/__init__.py
+-rw-r--r--   0        0        0    12374 2023-05-21 18:47:27.393941 pydelica-0.4.5/pydelica/compiler.py
+-rw-r--r--   0        0        0     3029 2022-11-14 22:38:00.298145 pydelica-0.4.5/pydelica/exception.py
+-rw-r--r--   0        0        0      319 2022-11-14 22:38:00.298651 pydelica-0.4.5/pydelica/logger.py
+-rw-r--r--   0        0        0     5659 2022-11-14 22:38:00.298651 pydelica-0.4.5/pydelica/model.py
+-rw-r--r--   0        0        0     8512 2023-05-25 18:26:58.362504 pydelica-0.4.5/pydelica/options.py
+-rw-r--r--   0        0        0     1685 2022-11-14 22:38:00.299719 pydelica-0.4.5/pydelica/solutions.py
+-rw-r--r--   0        0        0      939 2023-05-25 18:47:53.618178 pydelica-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     7619 2022-11-14 22:38:00.294919 pydelica-0.4.5/README.md
+-rw-r--r--   0        0        0     8655 1970-01-01 00:00:00.000000 pydelica-0.4.5/PKG-INFO
```

### Comparing `pydelica-0.4.3/LICENSE` & `pydelica-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelica-0.4.3/README.md` & `pydelica-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pydelica-0.4.3/pydelica/__init__.py` & `pydelica-0.4.5/pydelica/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -109,14 +109,18 @@
     def code_profile(self) -> typing.Optional[typing.Dict]:
         return self._current_profile
 
     @property
     def code_info(self) -> typing.Optional[typing.Dict]:
         return self._current_info
 
+    @property
+    def default_model(self) -> str:
+        return list(self._binaries.keys())[0]
+
     def _recover_profile(self, build_dir: str, run_dir: str) -> None:
         """Recovers a profile file if one exists"""
         _prof_files = glob.glob(os.path.join(run_dir, "*_prof.json"))
         _info_files = glob.glob(os.path.join(build_dir, "*_info.json"))
         if _prof_files:
             self._current_profile = json.load(open(_prof_files[0]))
         if _info_files:
@@ -193,28 +197,29 @@
             self._model_parameters[_model_name] = Model(modelica_source_file, xml_file)
 
             _binary = _model_name
 
             if platform.system() == "Windows":
                 _binary += ".exe"
 
-            self._binaries[_model_name] = os.path.join(
-                os.path.abspath(_binary_loc), _binary
-            )
+            _binary_addr = os.path.join(os.path.abspath(_binary_loc), _binary)
 
-            if not os.path.exists(self._binaries[_model_name]):
-                raise RuntimeError(
-                    f"Compilation of model '{_model_name}' failed, "
-                    f"no binary '{self._binaries[_model_name]}' found."
-                )
+            # In later versions of OM the binary name cannot have '.' within the name
+            if not os.path.exists(_binary_addr):
+                if not (
+                    os.path.exists(_binary_addr := _binary_addr.replace(".", "_", 1))
+                ):
+                    raise RuntimeError(
+                        f"Compilation of model '{_model_name}' failed, "
+                        f"no binary for '{_model_name}' found."
+                    )
 
-            self._logger.debug(
-                "Located compiled binary '%s'", self._binaries[_model_name]
-            )
+            self._logger.debug("Located compiled binary '%s'", _binary_addr)
 
+            self._binaries[_model_name] = _binary_addr
             self._solutions[_model_name] = SolutionHandler(self._session_directory)
 
             self._logger.debug(
                 "Extracting default simulation options for model '%s' from XML file",
                 _model_name,
             )
 
@@ -225,20 +230,35 @@
             # absolute path
             if update_input_paths_to:
                 self._set_input_files_directory(_model_name, update_input_paths_to)
 
             # Allows easy creation of a Pandas dataframe for displaying solutions
             self._set_output_to_csv()
 
+    def _get_cache_key(self, model_name: str, member_dict: typing.Dict) -> str:
+        """Retrieve Model Name in cache dictionary
+
+        Retrieves model name as stored within the given dictionary. In some versions of OM
+        '.' in the model name is replaced by '_' in the files.
+        """
+        if (
+            (_model_name := model_name) not in member_dict
+            and (_model_name := model_name.replace(".", "_")) not in member_dict
+        ):
+            raise KeyError(f"Key '{model_name}' not found")
+        return _model_name
+
     def get_binary_location(self, model_name: str):
-        if model_name not in self._binaries:
+        try:
+            _model_name: str = self._get_cache_key(model_name, self._binaries)
+        except KeyError as e:
             raise pde.BinaryNotFoundError(
                 f"Failed to retrieve binary for model '{model_name}'"
-            )
-        return self._binaries[model_name]
+            ) from e
+        return self._binaries[_model_name]
 
     def get_parameters(
         self, model_name: str = None
     ) -> typing.Union[Model, typing.Dict[str, typing.Any]]:
         """Retrieve a full parameter list
 
         Parameters
@@ -248,18 +268,20 @@
 
         Returns
         -------
         typing.Dict[str, typing.Any]
             dictionary containing parameters by name and their values
         """
         if model_name:
-            if model_name not in self._model_parameters:
-                raise pde.UnknownModelError(model_name)
+            try:
+                _model_name: str = self._get_cache_key(model_name, self._model_parameters)
+            except KeyError as e:
+                raise pde.UnknownModelError(model_name) from e
 
-            return self._model_parameters[model_name]
+            return self._model_parameters[_model_name]
         else:
             _out_params: typing.Dict[str, typing.Any] = {}
             for model in self._model_parameters:
                 for param in self._model_parameters[model]:
                     if param in _out_params:
                         continue
                     _out_params[param] = self._model_parameters[model][param]
@@ -275,24 +297,24 @@
 
         Returns
         -------
         typing.Any
             the value of the parameter specified
         """
         for model in self._model_parameters:
-            if param_name in self._model_parameters[model]:
+            if param_name in (_model_params := self.get_parameters(model)):
                 if isinstance(
-                    self._model_parameters[model].get_parameter(param_name),
+                    _param := _model_params.get_parameter(param_name),
                     dict,
                 ):
                     raise AssertionError(
                         "Expected non-mutable value for requested parameter"
                         f"'{param_name}' but got type 'dict'"
                     )
-                return self._model_parameters[model].get_parameter(param_name)
+                return _param
         raise pde.UnknownParameterError(param_name)
 
     def get_simulation_options(self, model_name: str = None) -> SimulationOptions:
         """Retrieve typing.Dictionary of the Simulation Options
 
         Parameters
         ----------
@@ -306,18 +328,20 @@
 
         Raises
         ------
         KeyError
             if the given model name is not recognised
         """
         if not model_name:
-            model_name = list(self._binaries.keys())[0]
-        if model_name not in self._simulation_opts:
-            raise pde.UnknownModelError(model_name)
-        return self._simulation_opts[model_name]
+            model_name = self.default_model
+        try:
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
+        except KeyError as e:
+            raise pde.UnknownModelError(model_name) from e
+        return self._simulation_opts[_model_name]
 
     def get_simulation_option(self, option: str, model_name: str = None) -> typing.Any:
         """Retrieve a single option for a given model.
 
         Parameters
         ----------
         option : str
@@ -334,17 +358,17 @@
         ------
         KeyError
             if the given model is not recognised
         KeyError
             if the given option name is not recognised
         """
         if not model_name:
-            return self._simulation_opts[list(self._binaries.keys())[0]][option]
-        else:
-            return self._simulation_opts[model_name][option]
+            return self._simulation_opts[self.default_model][option]
+        model_name = self._get_cache_key(model_name, self._simulation_opts)
+        return self._simulation_opts[model_name][option]
 
     def set_parameter(self, param_name: str, value: typing.Any) -> None:
         """Set a parameter to a given value
 
         Parameters
         ----------
         param_name : str
@@ -397,113 +421,147 @@
         ----------
         model_name : str, optional
             Specify model to execute, by default use first in list
         verbosity : OMLogLevel, optional
             specify level of Modelica outputs, else use default
         """
         if not model_name:
-            model_name = list(self._binaries.keys())[0]
+            model_name = self.default_model
             self._logger.warning(
                 "No model name specified, using first result '%s'", model_name
             )
-        if model_name not in self._binaries:
+        try:
+            _binary_loc: str = self.get_binary_location(model_name)
+            _model_name: str = self._get_cache_key(model_name, self._model_parameters)
+        except KeyError as e:
             raise pde.BinaryNotFoundError(
                 f"Could not find binary for Model '{model_name}',"
                 " did you run 'build_models' on the source file?"
-            )
+            ) from e
 
         self._logger.debug("Launching simulation for model '%s'", model_name)
 
         # Write parameters to the XML file read by the binary
-        self._model_parameters[model_name].write_params()
+        self._model_parameters[_model_name].write_params()
+
+        _binary_dir = os.path.dirname(_binary_loc)
 
-        _binary_dir = os.path.dirname(self._binaries[model_name])
+        _env = os.environ.copy()
 
-        _args = [self._binaries[model_name], f"-inputPath={_binary_dir}"]
+        # If the binary or library directories are not in PATH temporarily add them during
+        # model execution in Windows
+        if platform.system() == "Windows":
+            self._append_locs_to_winpath(_env)
+        _args = [_binary_loc, f"-inputPath={_binary_dir}"]
 
-        if not os.path.exists(self._binaries[model_name]):
+        if not os.path.exists(_binary_loc):
             raise pde.BinaryNotFoundError(
                 f"Failed to retrieve binary for model '{model_name}' "
                 f"from location '{_binary_dir}'"
             )
 
         if verbosity and verbosity.value:
             _args += [verbosity.value]
         elif self._log_level.value:
             _args += [self._log_level.value]
 
         with tempfile.TemporaryDirectory() as run_dir:
-
             _run_sim = subprocess.run(
                 _args,
                 stderr=subprocess.PIPE,
                 stdout=subprocess.PIPE,
                 text=True,
                 shell=False,
                 cwd=run_dir,
+                env=_env,
             )
 
             pde.parse_error_string_simulate(_run_sim.stdout, self._assert_fail_level)
 
             if _run_sim.returncode != 0:
+                _print_msg = _run_sim.stderr or _run_sim.stdout
+                if not _print_msg:
+                    _print_msg = "Cause unknown, no error logs were found."
                 raise pde.OMExecutionError(
-                    f"[{_run_sim.returncode}] Simulation failed with:\n{_run_sim.stderr}"
+                    f"[{_run_sim.returncode}] Simulation failed with: {_print_msg}"
                 )
 
-            self._solutions[model_name].retrieve_session_solutions(run_dir)
-            self._recover_profile(os.path.dirname(self._binaries[model_name]), run_dir)
+            self._solutions[_model_name].retrieve_session_solutions(run_dir)
+            self._recover_profile(_binary_dir, run_dir)
+
+    def _append_locs_to_winpath(self, _env):
+        _om_home = os.environ["OPENMODELICAHOME"]
+        _path: str = os.environ["PATH"]
+        _separator: str = ";" if ";" in _path else ":"
+        _path_entries: typing.List[str] = os.environ["PATH"].split(_separator)
+
+        _required: typing.List[str] = (
+            os.path.join(_om_home, "bin"),
+            os.path.join(_om_home, "lib"),
+        )
+
+        for path in _required:
+            if path not in _path_entries:
+                _path_entries.append(path)
+
+        _env["PATH"] = f"{_separator}".join(_path_entries)
 
     def _set_output_to_csv(self):
         for model in self._simulation_opts:
             self._simulation_opts[model].set_option("outputFormat", "csv")
 
     def set_solver(self, solver: Solver, model_name: str = None) -> None:
         if model_name:
-            self._simulation_opts[model_name].set_option("solver", solver.value)
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
+            self._simulation_opts[_model_name].set_option("solver", solver.value)
         else:
             for model in self._simulation_opts:
                 self._simulation_opts[model].set_option("solver", solver.value)
 
     def set_time_range(
         self,
         start_time: int = None,
         stop_time: int = None,
         model_name: str = None,
     ) -> None:
         if model_name:
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
             if start_time:
-                self._simulation_opts[model_name].set_option("startTime", start_time)
+                self._simulation_opts[_model_name].set_option("startTime", start_time)
             if stop_time:
-                self._simulation_opts[model_name].set_option("stopTime", stop_time)
+                self._simulation_opts[_model_name].set_option("stopTime", stop_time)
         else:
             for model in self._simulation_opts:
                 if start_time:
                     self._simulation_opts[model].set_option("startTime", start_time)
                 if stop_time:
                     self._simulation_opts[model].set_option("stopTime", stop_time)
 
     def set_tolerance(self, tolerance: float, model_name: str = None) -> None:
         if model_name:
-            self._simulation_opts[model_name].set_option("tolerance", tolerance)
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
+            self._simulation_opts[_model_name].set_option("tolerance", tolerance)
         else:
             for model in self._simulation_opts:
                 self._simulation_opts[model].set_option("tolerance", tolerance)
 
     def set_variable_filter(self, filter_str: str, model_name: str = None) -> None:
         if model_name:
-            self._simulation_opts[model_name].set_option("variableFilter", filter_str)
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
+            self._simulation_opts[_model_name].set_option("variableFilter", filter_str)
         else:
             for model in self._simulation_opts:
                 self._simulation_opts[model].set_option("variableFilter", filter_str)
 
     def set_simulation_option(
         self, option_name: str, value: typing.Any, model_name: str = None
     ) -> None:
         if model_name:
-            self._simulation_opts[model_name].set_option(option_name, value)
+            _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
+            self._simulation_opts[_model_name].set_option(option_name, value)
         else:
             for model in self._simulation_opts:
                 self._simulation_opts[model].set_option(option_name, value)
 
     def get_solutions(self) -> pandas.DataFrame:
         """Returns solutions to all simulated models as a dictionary of dataframes
```

### Comparing `pydelica-0.4.3/pydelica/compiler.py` & `pydelica-0.4.5/pydelica/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,23 +265,32 @@
                 raise pde.ModelicaFileGenerationError(
                     f"Failed to find a Makefile in the directory: {_temp_build_dir}, "
                     "Modelica failed to generated required files."
                 )
 
             # Use the OM included MSYS Mingw32Make for Windows
             if platform.system() == "Windows":
-                _make_cmd = os.path.join(
-                    os.environ["OPENMODELICAHOME"],
-                    "tools",
-                    "msys",
-                    "mingw64",
-                    "bin",
-                    "mingw32-make.exe",
+                _make_binaries = glob.glob(
+                    os.path.join(
+                        os.environ["OPENMODELICAHOME"],
+                        "tools",
+                        "msys",
+                        "mingw*",
+                        "bin",
+                        "mingw*-make.exe",
+                    )
                 )
 
+                if not _make_binaries:
+                    raise pde.BinaryNotFoundError(
+                        "Failed to find Make binary in Modelica directories"
+                    )
+
+                _make_cmd = _make_binaries[0]
+
             elif not shutil.which("make"):
                 raise pde.BinaryNotFoundError("Could not find GNU-Make on this system")
             else:
                 _make_cmd = shutil.which("make")
 
             _make_file = _make_file[0]
```

### Comparing `pydelica-0.4.3/pydelica/exception.py` & `pydelica-0.4.5/pydelica/exception.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.4.3/pydelica/model.py` & `pydelica-0.4.5/pydelica/model.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.4.3/pydelica/options.py` & `pydelica-0.4.5/pydelica/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,17 @@
     def _get_system_libraries(self) -> List[str]:
         if "MODELICAPATH" in os.environ:
             _library_dirs = os.environ["MODELICAPATH"].split(os.pathsep)
             _libs = []
             for library_dir in _library_dirs:
                 _libs += glob.glob(os.path.join(library_dir, "*"))
         elif platform.system() == "Windows":
-            _home = os.environ["HOMEPATH"]
+            _home = os.environ["USERPROFILE"]
             _user_libraries = os.path.join(
-                _home, "Users", "AppData", "Roaming", ".openmodelica", "libraries"
+                _home, "AppData", "Roaming", ".openmodelica", "libraries"
             )
             _library_dir = os.path.join(
                 os.environ["OPENMODELICAHOME"], "lib", "omlibrary"
             )
             _libs = glob.glob(os.path.join(_user_libraries, "*"))
             _libs += glob.glob(os.path.join(_library_dir, "*"))
         else:
```

### Comparing `pydelica-0.4.3/pydelica/solutions.py` & `pydelica-0.4.5/pydelica/solutions.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.4.3/pyproject.toml` & `pydelica-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydelica"
-version = "0.4.3"
+version = "0.4.5"
 description = "Light-weight serverless API for OpenModelica"
 authors = ["Kristian Zarebski <krizar312@gmail.com>"]
 license = "MIT"
 keywords = ["modelica", "openmodelica"]
 repository = "https://gitlab.com/krizar/pydelica"
 readme = "README.md"
 include = [
@@ -18,21 +18,19 @@
     "Topic :: Scientific/Engineering",
     "Natural Language :: English",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-lxml = "^4.6.2"
-pandas = "^1.2.2"
+python = "^3.9,<3.12"
+pandas = "^1.5.1"
 defusedxml = "^0.7.1"
 
-[tool.poetry.dev-dependencies]
-pylint = "^2.7.4"
-black = {version = "^21.6b0", allow-prereleases = true}
-pytest = "^7.0.1"
-pre-commit = "^2.17.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+black = "^22.10.0"
+pylint = "^2.15.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydelica-0.4.3/setup.py` & `pydelica-0.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,223 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydelica
+Version: 0.4.5
+Summary: Light-weight serverless API for OpenModelica
+Home-page: https://gitlab.com/krizar/pydelica
+License: MIT
+Keywords: modelica,openmodelica
+Author: Kristian Zarebski
+Author-email: krizar312@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
+Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Project-URL: Repository, https://gitlab.com/krizar/pydelica
+Description-Content-Type: text/markdown
+
+# PyDelica: Serverless OpenModelica with Python
+
+## About
+
+PyDelica is an API providing a quick and easy to use interface to compile, customise and run OpenModelica models with Python. Unlike OMPython it does not require the launch of a server session to use OMShell but rather dynamically adjusts files produced after model compilation in order to update options and parameters. The lack of server requirement means models can be run in tandem without calling multiple OMC sessions which can be very taxing on CPU. Furthermore PyDelica is able to detect errors during model runs by reading the `stderr` and `stdout` from OpenModelica and throw appropriate exceptions to terminate the program execution.
+
+## Installation
+
+To use PyDelica you will require an installation of OpenModelica on your system, the API has been confirmed to work on both Windows and Linux, but if OM is installable on macOS it should also be possible to still use it. 
+
+To install run:
+
+```bash
+pip install pydelica
+```
+
+## Getting Started
+For the purposes of demonstration the included test model `tests/models/SineCurrent.mo` will be used.
+### PyDelica Session
+All uses of PyDelica require an instance of the `Session` class:
+
+```python
+from pydelica import Session
+
+with Session() as session:
+    ...
+```
+It is strongly recommended that this class be used via the context manager to ensure cleanup of temporary directories.
+
+#### Logging
+The `Session` class has one optional argument which is used to set the log level output within OpenModelica itself. The options are based on the `-lv` flag within OM. By default the level is set to `Normal` which means no log level output.
+
+As an example if you wanted to run with statistics logging `-lv=LOG_STATS` you would setup with the following:
+
+```python
+from pydelica import Session
+from pydelica.logger import OMLogLevel
+
+with Session(log_level=OMLogLevel.STATS) as session:
+    ...
+```
+
+See the source for more options [here](https://gitlab.com/krizar/pydelica/-/blob/master/pydelica/logging.py).
+
+#### Building/Compiling Models
+Before you can run a model you must first compile it. This is done using the `build_model` member function which takes the path to the Modelica source file.
+
+```python
+model_path = os.path.join('tests', 'models', 'SineCurrent.mo')
+session.build_model(model_path)
+```
+
+If the required model is not top level, that is to say it exists within a module or , we can optionally specify the address within Modelica. This is also required if the required model is not the default. For example say model `A` existed within module `M`:
+
+```python
+model_path = 'FictionalModelFile.mo'
+session.build_model(model_path, 'M.A')
+```
+
+The `build_model` function also allows you to specify additional flags/options to hand to the OMC compiler, these are given
+in the form of a dictionary where the value can be `None` if the flag does not take any input. You can also directly set the profiling level for profiling the Modelica code. When set, the profile dictionary is also stored in the session after the simulation and is accessible via the `code_profile` and `code_info` attributes:
+
+```python
+session.build_model(model_path, 'M.A', profiling="all", omc_build_flags={"-g": "MetaModelica"})
+session.simulate()
+print(session.code_profile)
+print(session.code_info)
+```
+
+#### Examining Parameters and Options
+We can examine all parameters for a given model using the `get_parameters` method which will return a Python dictionary:
+
+```python
+session.get_parameters('SineCurrentModel')
+```
+
+if the parameter is unique to a single model then the model name argument can be dropped. Returning the value for a single parameter is as simple as:
+
+```python
+session.get_parameter(<parameter-name>)
+```
+
+For simulation options the analogous methods are `get_simulation_options` and `get_simulation_option` respectively for general case, for more specific see below.
+
+#### Setting Parameters and Options
+Set a parameter to a different value using the `set_parameter` function:
+
+```python
+session.set_parameter(<parameter-name>, <new-value>)
+```
+
+#### Further Configuration
+The output file type can be specified:
+
+```python
+from pydelica.options import OutputFormat
+session.set_output_format(OutputFormat.CSV) # Other options are MAT and PLT
+```
+
+Set the solver:
+
+```python
+from pydelica.options import Solver
+session.set_solver(Solver.DASSL)    # Other options are EULER and RUNGE_KUTTA
+```
+
+Set the time range:
+
+```python
+# Each argument is optional
+session.set_time_range(start_time=0, stop_time=10, model_name='SineCurrentModel')
+```
+
+Set tolerance:
+
+```python
+# Model name is optional
+session.set_tolerance(tolerance=1E-9, model_name='SineCurrentModel')
+```
+
+Set variable filter for outputs:
+
+```python
+# Model name is optional
+session.set_variable_filter(filter_str='output*', model_name='SineCurrentModel')
+```
+
+#### Failing Simulation on Lower Assertion Level
+By default PyDelica will look for the expression `assert | error` as an indication of a Modelica assertion
+failure and then terminate when this is violated. You can override this behaviour using the `fail_on_assert_level`
+method of the `Session` class:
+
+```python
+from pydelica import Session
+
+with Session() as pd_session:
+    pd_session.fail_on_assert_level('warning')
+```
+
+Possible values ranked by order (highest at the top):
+
+|**Value**|**Description**|
+|---|---|
+|`'never'`|Do not throw an exception on Modelica assertion violation|
+|`'error'`|Default. Throw an exception on an assertion of level `AssertionLevel.error`|
+|`'warning'`|Throw an exception on assertion of level `AssertionLevel.warning`|
+|`'info'`|Throw an exception on any `assert | info` statement|
+|`'debug'`|Throw an exception on any `assert | debug` statement|
+
+#### Running the Simulation
+To run the simulation use the `simulate` method. If a model name is specified then that model is run,
+else this is the first model in the model list. At the simulation step parameter values are written to the
+XML file read by the binary before the model binary is executed.
+
+```python
+# Model name is optional, verbosity is also optional and overwrites that of the session
+session.simulate(model_name='SineCurrentModel', verbosity=OMLogLevel.DEBUG)
+```
+
+#### Retrieving Results
+To view the results use the `get_solutions` method which will return a python dictionary containing
+the solutions for all models after a model run:
+
+```python
+solutions = session.get_solutions()
+```
+The variables for each model are stored as a Pandas dataframe.
+
+#### Using Alternative Libraries
+
+**NOTE:** Currently only works in WSL on Windows machines.
+
+You can use an alternative library version via the `use_library` method:
+```python3
+session.use_library("Modelica", "3.2.3")
+```
+you can also optionally specify the location of this library:
+```python3
+session.use_library("Modelica", "3.2.3", library_directory="/home/user/my_om_libraries")
+```
+
+## Troubleshooting
+
+### Simulation fails with no error thrown
+Try setting the assertion level to a lower level, for some reason OM ranks missing input file errors
+as type `debug`, see [here](#failing-simulation-on-lower-assertion-level).
+
+```
+stdout | info | ... loading "data" from "Default/myInput.mat"
+assert | debug | Not possible to open file "Default/myInput.mat": No such file or directory
+assert | info | simulation terminated by an assertion at initialization
+```
 
-packages = \
-['pydelica']
+### PyDelica cannot find OMC
+PyDelica relies on either locating OMC on UNIX using the `which` command, or in the case of Windows using the `OPENMODELICAHOME` environment variable. Ensure at least one of these is available after installating OpenModelica.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['defusedxml>=0.7.1,<0.8.0', 'lxml>=4.6.2,<5.0.0', 'pandas>=1.2.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pydelica',
-    'version': '0.4.3',
-    'description': 'Light-weight serverless API for OpenModelica',
-    'long_description': '# PyDelica: Serverless OpenModelica with Python\n\n## About\n\nPyDelica is an API providing a quick and easy to use interface to compile, customise and run OpenModelica models with Python. Unlike OMPython it does not require the launch of a server session to use OMShell but rather dynamically adjusts files produced after model compilation in order to update options and parameters. The lack of server requirement means models can be run in tandem without calling multiple OMC sessions which can be very taxing on CPU. Furthermore PyDelica is able to detect errors during model runs by reading the `stderr` and `stdout` from OpenModelica and throw appropriate exceptions to terminate the program execution.\n\n## Installation\n\nTo use PyDelica you will require an installation of OpenModelica on your system, the API has been confirmed to work on both Windows and Linux, but if OM is installable on macOS it should also be possible to still use it. \n\nTo install run:\n\n```bash\npip install pydelica\n```\n\n## Getting Started\nFor the purposes of demonstration the included test model `tests/models/SineCurrent.mo` will be used.\n### PyDelica Session\nAll uses of PyDelica require an instance of the `Session` class:\n\n```python\nfrom pydelica import Session\n\nwith Session() as session:\n    ...\n```\nIt is strongly recommended that this class be used via the context manager to ensure cleanup of temporary directories.\n\n#### Logging\nThe `Session` class has one optional argument which is used to set the log level output within OpenModelica itself. The options are based on the `-lv` flag within OM. By default the level is set to `Normal` which means no log level output.\n\nAs an example if you wanted to run with statistics logging `-lv=LOG_STATS` you would setup with the following:\n\n```python\nfrom pydelica import Session\nfrom pydelica.logger import OMLogLevel\n\nwith Session(log_level=OMLogLevel.STATS) as session:\n    ...\n```\n\nSee the source for more options [here](https://gitlab.com/krizar/pydelica/-/blob/master/pydelica/logging.py).\n\n#### Building/Compiling Models\nBefore you can run a model you must first compile it. This is done using the `build_model` member function which takes the path to the Modelica source file.\n\n```python\nmodel_path = os.path.join(\'tests\', \'models\', \'SineCurrent.mo\')\nsession.build_model(model_path)\n```\n\nIf the required model is not top level, that is to say it exists within a module or , we can optionally specify the address within Modelica. This is also required if the required model is not the default. For example say model `A` existed within module `M`:\n\n```python\nmodel_path = \'FictionalModelFile.mo\'\nsession.build_model(model_path, \'M.A\')\n```\n\nThe `build_model` function also allows you to specify additional flags/options to hand to the OMC compiler, these are given\nin the form of a dictionary where the value can be `None` if the flag does not take any input. You can also directly set the profiling level for profiling the Modelica code. When set, the profile dictionary is also stored in the session after the simulation and is accessible via the `code_profile` and `code_info` attributes:\n\n```python\nsession.build_model(model_path, \'M.A\', profiling="all", omc_build_flags={"-g": "MetaModelica"})\nsession.simulate()\nprint(session.code_profile)\nprint(session.code_info)\n```\n\n#### Examining Parameters and Options\nWe can examine all parameters for a given model using the `get_parameters` method which will return a Python dictionary:\n\n```python\nsession.get_parameters(\'SineCurrentModel\')\n```\n\nif the parameter is unique to a single model then the model name argument can be dropped. Returning the value for a single parameter is as simple as:\n\n```python\nsession.get_parameter(<parameter-name>)\n```\n\nFor simulation options the analogous methods are `get_simulation_options` and `get_simulation_option` respectively for general case, for more specific see below.\n\n#### Setting Parameters and Options\nSet a parameter to a different value using the `set_parameter` function:\n\n```python\nsession.set_parameter(<parameter-name>, <new-value>)\n```\n\n#### Further Configuration\nThe output file type can be specified:\n\n```python\nfrom pydelica.options import OutputFormat\nsession.set_output_format(OutputFormat.CSV) # Other options are MAT and PLT\n```\n\nSet the solver:\n\n```python\nfrom pydelica.options import Solver\nsession.set_solver(Solver.DASSL)    # Other options are EULER and RUNGE_KUTTA\n```\n\nSet the time range:\n\n```python\n# Each argument is optional\nsession.set_time_range(start_time=0, stop_time=10, model_name=\'SineCurrentModel\')\n```\n\nSet tolerance:\n\n```python\n# Model name is optional\nsession.set_tolerance(tolerance=1E-9, model_name=\'SineCurrentModel\')\n```\n\nSet variable filter for outputs:\n\n```python\n# Model name is optional\nsession.set_variable_filter(filter_str=\'output*\', model_name=\'SineCurrentModel\')\n```\n\n#### Failing Simulation on Lower Assertion Level\nBy default PyDelica will look for the expression `assert | error` as an indication of a Modelica assertion\nfailure and then terminate when this is violated. You can override this behaviour using the `fail_on_assert_level`\nmethod of the `Session` class:\n\n```python\nfrom pydelica import Session\n\nwith Session() as pd_session:\n    pd_session.fail_on_assert_level(\'warning\')\n```\n\nPossible values ranked by order (highest at the top):\n\n|**Value**|**Description**|\n|---|---|\n|`\'never\'`|Do not throw an exception on Modelica assertion violation|\n|`\'error\'`|Default. Throw an exception on an assertion of level `AssertionLevel.error`|\n|`\'warning\'`|Throw an exception on assertion of level `AssertionLevel.warning`|\n|`\'info\'`|Throw an exception on any `assert | info` statement|\n|`\'debug\'`|Throw an exception on any `assert | debug` statement|\n\n#### Running the Simulation\nTo run the simulation use the `simulate` method. If a model name is specified then that model is run,\nelse this is the first model in the model list. At the simulation step parameter values are written to the\nXML file read by the binary before the model binary is executed.\n\n```python\n# Model name is optional, verbosity is also optional and overwrites that of the session\nsession.simulate(model_name=\'SineCurrentModel\', verbosity=OMLogLevel.DEBUG)\n```\n\n#### Retrieving Results\nTo view the results use the `get_solutions` method which will return a python dictionary containing\nthe solutions for all models after a model run:\n\n```python\nsolutions = session.get_solutions()\n```\nThe variables for each model are stored as a Pandas dataframe.\n\n#### Using Alternative Libraries\n\n**NOTE:** Currently only works in WSL on Windows machines.\n\nYou can use an alternative library version via the `use_library` method:\n```python3\nsession.use_library("Modelica", "3.2.3")\n```\nyou can also optionally specify the location of this library:\n```python3\nsession.use_library("Modelica", "3.2.3", library_directory="/home/user/my_om_libraries")\n```\n\n## Troubleshooting\n\n### Simulation fails with no error thrown\nTry setting the assertion level to a lower level, for some reason OM ranks missing input file errors\nas type `debug`, see [here](#failing-simulation-on-lower-assertion-level).\n\n```\nstdout | info | ... loading "data" from "Default/myInput.mat"\nassert | debug | Not possible to open file "Default/myInput.mat": No such file or directory\nassert | info | simulation terminated by an assertion at initialization\n```\n\n### PyDelica cannot find OMC\nPyDelica relies on either locating OMC on UNIX using the `which` command, or in the case of Windows using the `OPENMODELICAHOME` environment variable. Ensure at least one of these is available after installating OpenModelica.\n',
-    'author': 'Kristian Zarebski',
-    'author_email': 'krizar312@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.com/krizar/pydelica',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

