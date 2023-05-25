# Comparing `tmp/cppython-core-0.6.1.dev7.tar.gz` & `tmp/cppython-core-0.6.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-core-0.6.1.dev7.tar", last modified: Sat Oct  8 16:09:27 2022, max compression
+gzip compressed data, was "cppython-core-0.6.1.dev9.tar", last modified: Sun Oct  9 15:14:07 2022, max compression
```

## Comparing `cppython-core-0.6.1.dev7.tar` & `cppython-core-0.6.1.dev9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/plugin_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/plugin_schema/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/plugin_schema/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/plugin_schema/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/plugin_schema/vcs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-10-08 16:09:17.704405 cppython-core-0.6.1.dev7/cppython_core/resolution.py
--rw-r--r--   0 runner    (1001) docker     (121)    10835 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/cppython_core/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/cppython_core/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/unit/test_plugin_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/unit/test_resolution.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-10-08 16:09:17.708405 cppython-core-0.6.1.dev7/tests/unit/test_utility.py
--rw-------   0 runner    (1001) docker     (121)      432 2022-10-08 16:09:27.236578 cppython-core-0.6.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     5301 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10761 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/utility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_plugin_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_utility.py
+-rw-------   0 runner    (1001) docker     (121)      432 2022-10-09 15:14:07.457900 cppython-core-0.6.1.dev9/PKG-INFO
```

### Comparing `cppython-core-0.6.1.dev7/LICENSE.md` & `cppython-core-0.6.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/cppython_core/exceptions.py` & `cppython-core-0.6.1.dev9/cppython_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/cppython_core/plugin_schema/generator.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/generator.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/cppython_core/plugin_schema/interface.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/interface.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/cppython_core/plugin_schema/provider.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/provider.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/cppython_core/plugin_schema/vcs.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/vcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 """Version control data plugin definitions"""
 from __future__ import annotations
 
 from abc import abstractmethod
 from pathlib import Path
 from typing import TypeVar
 
-from pydantic import Field
-from pydantic.types import DirectoryPath
+from cppython_core.schema import Plugin
 
-from cppython_core.schema import DataPlugin, PluginGroupData
 
-
-class VersionControlData(PluginGroupData):
-    """Base class for the configuration data that is set by the project for the version control"""
-
-    root_directory: DirectoryPath = Field(description="The directory where the pyproject.toml lives")
-
-
-class VersionControl(DataPlugin[VersionControlData]):
+class VersionControl(Plugin):
     """Base class for version control systems"""
 
     @abstractmethod
     def is_repository(self, path: Path) -> bool:
         """Queries repository status of a path
 
         Args:
```

### Comparing `cppython-core-0.6.1.dev7/cppython_core/resolution.py` & `cppython-core-0.6.1.dev9/cppython_core/resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 """Data conversion routines"""
 
 from typing import cast
 
+from cppython_core.exceptions import ConfigError
 from cppython_core.plugin_schema.generator import GeneratorData
 from cppython_core.plugin_schema.provider import ProviderData
-from cppython_core.plugin_schema.vcs import VersionControlData
 from cppython_core.schema import (
     CPPythonData,
     CPPythonGlobalConfiguration,
     CPPythonLocalConfiguration,
     CPPythonPluginData,
     DataPluginT,
     PEP621Configuration,
     PEP621Data,
+    ProjectConfiguration,
     ProjectData,
 )
 
 
-def resolve_pep621(pep621_configuration: PEP621Configuration, project_data: ProjectData) -> PEP621Data:
+def resolve_project_configuration(project_configuration: ProjectConfiguration) -> ProjectData:
+    """Creates a resolved type
+
+    Args:
+        project_configuration: Input configuration
+
+    Returns:
+        The resolved data
+    """
+    return ProjectData(pyproject_file=project_configuration.pyproject_file, verbosity=project_configuration.verbosity)
+
+
+def resolve_pep621(
+    pep621_configuration: PEP621Configuration, project_configuration: ProjectConfiguration
+) -> PEP621Data:
     """Creates a resolved type
 
     Args:
         pep621_configuration: Input PEP621 configuration
-        project_data: The input configuration used to aid the resolve
+        project_configuration: The input configuration used to aid the resolve
 
     Raises:
+        ConfigError: Raised when the tooling did not satisfy the configuration request
         ValueError: Raised if there is a broken schema
 
     Returns:
         The resolved type
     """
 
     # Update the dynamic version
     if "version" in pep621_configuration.dynamic:
-        modified_version = project_data.version
+        if project_configuration.version is not None:
+            modified_version = project_configuration.version
+        else:
+            raise ConfigError("'version' is dynamic but the interface did not provide a version value")
 
     elif pep621_configuration.version is not None:
         modified_version = pep621_configuration.version
 
     else:
         raise ValueError("Version can't be resolved. This is an internal schema error")
 
@@ -143,20 +162,7 @@
         project_data: The input project configuration
 
     Returns:
         The plugin specific configuration
     """
     configuration = ProviderData(root_directory=project_data.pyproject_file.parent)
     return configuration
-
-
-def resolve_vcs(project_data: ProjectData) -> VersionControlData:
-    """Creates an instance from the given project
-
-    Args:
-        project_data: The input project configuration
-
-    Returns:
-        The plugin specific configuration
-    """
-    configuration = VersionControlData(root_directory=project_data.pyproject_file.parent)
-    return configuration
```

### Comparing `cppython-core-0.6.1.dev7/cppython_core/schema.py` & `cppython-core-0.6.1.dev9/cppython_core/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 ModelT = TypeVar("ModelT", bound=CPPythonModel)
 
 
 class ProjectData(CPPythonModel, extra=Extra.forbid):
     """Resolved data of 'ProjectConfiguration'"""
 
     pyproject_file: FilePath = Field(description="The path where the pyproject.toml exists")
-    version: str = Field(description="The version number of the project")
     verbosity: int = Field(default=0, description="The verbosity level as an integer [0,2]")
 
 
 class ProjectConfiguration(CPPythonModel, extra=Extra.forbid):
     """Project-wide configuration"""
 
     pyproject_file: FilePath = Field(description="The path where the pyproject.toml exists")
```

### Comparing `cppython-core-0.6.1.dev7/cppython_core/utility.py` & `cppython-core-0.6.1.dev9/cppython_core/utility.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/pyproject.toml` & `cppython-core-0.6.1.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.10"
 dependencies = [
     "pydantic>=1.10.1",
     "packaging>=21.3",
 ]
-version = "0.6.1.dev7"
+version = "0.6.1.dev9"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `cppython-core-0.6.1.dev7/tests/unit/test_plugin_schema.py` & `cppython-core-0.6.1.dev9/tests/unit/test_plugin_schema.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/tests/unit/test_resolution.py` & `cppython-core-0.6.1.dev9/tests/unit/test_resolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from pytest_mock import MockerFixture
 
 from cppython_core.resolution import (
     resolve_cppython,
     resolve_cppython_plugin,
     resolve_generator,
     resolve_pep621,
+    resolve_project_configuration,
     resolve_provider,
-    resolve_vcs,
 )
 from cppython_core.schema import (
     CPPythonGlobalConfiguration,
     CPPythonLocalConfiguration,
     PEP621Configuration,
+    ProjectConfiguration,
     ProjectData,
 )
 
 
 class TestSchema:
     """Test validation"""
 
@@ -35,15 +36,15 @@
         pyproject = tmp_path / "pyproject.toml"
         pyproject.write_text("")
 
         # Data definition
         local_config = CPPythonLocalConfiguration(**{"install-path": tmp_path})
         global_config = CPPythonGlobalConfiguration()
 
-        project_config = ProjectData(pyproject_file=pyproject, version="0.1.0")
+        project_config = ProjectData(pyproject_file=pyproject)
 
         # Function to test
         resolved = resolve_cppython(local_config, global_config, project_config)
 
         # Test that paths are created successfully
         assert resolved.build_path.exists()
         assert resolved.tool_path.exists()
@@ -67,44 +68,44 @@
         pyproject = tmp_path / "pyproject.toml"
         pyproject.write_text("")
 
         # Data definition
         local_config = CPPythonLocalConfiguration(**{"install-path": tmp_path})
         global_config = CPPythonGlobalConfiguration()
 
-        project_config = ProjectData(pyproject_file=pyproject, version="0.1.0")
+        project_config = ProjectData(pyproject_file=pyproject)
 
         resolved = resolve_cppython(local_config, global_config, project_config)
 
         with mocker.MagicMock() as plugin_type:
             plugin_type.name.return_value = "mock"
             assert resolve_cppython_plugin(resolved, plugin_type)
 
     def test_pep621_resolve(self) -> None:
         """Test the PEP621 schema resolve function"""
 
         data = PEP621Configuration(name="pep621-resolve-test", dynamic=["version"])
-        config = ProjectData(pyproject_file=Path("pyproject.toml"), version="0.1.0")
+        config = ProjectConfiguration(pyproject_file=Path("pyproject.toml"), version="0.1.0")
         resolved = resolve_pep621(data, config)
 
         class_variables = vars(resolved)
 
         assert len(class_variables)
         assert not None in class_variables.values()
 
+    def test_project_resolve(self) -> None:
+        """Tests project configuration resolution"""
+
+        config = ProjectConfiguration(pyproject_file=Path("pyproject.toml"), version="0.1.0")
+        assert resolve_project_configuration(config)
+
     def test_generator_resolve(self) -> None:
         """Tests generator resolution"""
 
-        project_data = ProjectData(pyproject_file=Path("pyproject.toml"), version="0.1.0")
+        project_data = ProjectData(pyproject_file=Path("pyproject.toml"))
         assert resolve_generator(project_data)
 
     def test_provider_resolve(self) -> None:
         """Tests provider resolution"""
 
-        project_data = ProjectData(pyproject_file=Path("pyproject.toml"), version="0.1.0")
+        project_data = ProjectData(pyproject_file=Path("pyproject.toml"))
         assert resolve_provider(project_data)
-
-    def test_vcs_resolve(self) -> None:
-        """Tests vcs resolution"""
-
-        project_data = ProjectData(pyproject_file=Path("pyproject.toml"), version="0.1.0")
-        assert resolve_vcs(project_data)
```

### Comparing `cppython-core-0.6.1.dev7/tests/unit/test_schema.py` & `cppython-core-0.6.1.dev9/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev7/tests/unit/test_utility.py` & `cppython-core-0.6.1.dev9/tests/unit/test_utility.py`

 * *Files identical despite different names*

