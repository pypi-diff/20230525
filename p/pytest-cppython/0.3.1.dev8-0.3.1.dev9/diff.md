# Comparing `tmp/pytest-cppython-0.3.1.dev8.tar.gz` & `tmp/pytest-cppython-0.3.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-cppython-0.3.1.dev8.tar", last modified: Fri Oct 14 16:29:13 2022, max compression
+gzip compressed data, was "pytest-cppython-0.3.1.dev9.tar", last modified: Fri Oct 14 19:28:38 2022, max compression
```

## Comparing `pytest-cppython-0.3.1.dev8.tar` & `pytest-cppython-0.3.1.dev9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)    11313 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/pytest_cppython/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/integration/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/integration/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/integration/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/integration/test_version_control.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/unit/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/unit/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/unit/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-10-14 16:29:05.456877 pytest-cppython-0.3.1.dev8/tests/unit/test_version_control.py
--rw-------   0 runner    (1001) docker     (121)      484 2022-10-14 16:29:13.892892 pytest-cppython-0.3.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/pytest_cppython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/pytest_cppython/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/pytest_cppython/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2022-10-14 19:28:29.586529 pytest-cppython-0.3.1.dev9/pytest_cppython/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11363 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/pytest_cppython/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/pytest_cppython/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/integration/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/integration/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/integration/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/integration/test_version_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/unit/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/unit/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/unit/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-10-14 19:28:29.590530 pytest-cppython-0.3.1.dev9/tests/unit/test_version_control.py
+-rw-------   0 runner    (1001) docker     (121)      484 2022-10-14 19:28:38.958734 pytest-cppython-0.3.1.dev9/PKG-INFO
```

### Comparing `pytest-cppython-0.3.1.dev8/LICENSE.md` & `pytest-cppython-0.3.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/pyproject.toml` & `pytest-cppython-0.3.1.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.10"
 dependencies = [
     "cppython-core>=0.4.1.dev13",
     "pydantic>=1.9.2",
 ]
-version = "0.3.1.dev8"
+version = "0.3.1.dev9"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `pytest-cppython-0.3.1.dev8/pytest_cppython/data.py` & `pytest-cppython-0.3.1.dev9/pytest_cppython/data.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/pytest_cppython/fixtures.py` & `pytest-cppython-0.3.1.dev9/pytest_cppython/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/pytest_cppython/mock.py` & `pytest-cppython-0.3.1.dev9/pytest_cppython/mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Shared definitions for testing.
 """
 
 from pathlib import Path
+from typing import Any
 
 from cppython_core.plugin_schema.generator import Generator
 from cppython_core.plugin_schema.interface import Interface
 from cppython_core.plugin_schema.provider import Provider
 from cppython_core.plugin_schema.vcs import VersionControl
 
 
@@ -26,14 +27,17 @@
 
 
 class MockProvider(Provider):
     """A mock provider class for behavior testing"""
 
     downloaded: Path | None = None
 
+    def activate(self, data: dict[str, Any]) -> None:
+        pass
+
     @staticmethod
     def name() -> str:
         """The name of the plugin, canonicalized
 
         Returns:
             The plugin name
         """
@@ -70,14 +74,17 @@
         """The plugin name
 
         Returns:
             The name
         """
         return "mock"
 
+    def activate(self, data: dict[str, Any]) -> None:
+        pass
+
 
 class MockVersionControl(VersionControl):
     """A mock generator class for behavior testing"""
 
     @staticmethod
     def name() -> str:
         """The plugin name
```

### Comparing `pytest-cppython-0.3.1.dev8/pytest_cppython/plugin.py` & `pytest-cppython-0.3.1.dev9/pytest_cppython/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,19 @@
             core_plugin_data: The core metadata
             plugin_data: The data table
 
         Returns:
             A newly constructed provider
         """
 
-        return plugin_type(plugin_group_data, core_plugin_data, plugin_data)
+        plugin = plugin_type(plugin_group_data, core_plugin_data)
+
+        plugin.activate(plugin_data)
+
+        return plugin
 
 
 class DataPluginIntegrationTests(
     PluginIntegrationTests[DataPluginT],
     DataPluginTests[PluginGroupDataT, DataPluginT],
     Generic[PluginGroupDataT, DataPluginT],
 ):
```

### Comparing `pytest-cppython-0.3.1.dev8/tests/integration/test_generator.py` & `pytest-cppython-0.3.1.dev9/tests/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/integration/test_interface.py` & `pytest-cppython-0.3.1.dev9/tests/integration/test_interface.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/integration/test_provider.py` & `pytest-cppython-0.3.1.dev9/tests/integration/test_provider.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/integration/test_version_control.py` & `pytest-cppython-0.3.1.dev9/tests/integration/test_version_control.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/unit/test_generator.py` & `pytest-cppython-0.3.1.dev9/tests/unit/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/unit/test_interface.py` & `pytest-cppython-0.3.1.dev9/tests/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/unit/test_provider.py` & `pytest-cppython-0.3.1.dev9/tests/unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `pytest-cppython-0.3.1.dev8/tests/unit/test_version_control.py` & `pytest-cppython-0.3.1.dev9/tests/unit/test_version_control.py`

 * *Files identical despite different names*

