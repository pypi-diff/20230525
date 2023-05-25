# Comparing `tmp/typer_config-0.4.0.tar.gz` & `tmp/typer_config-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.4.0.tar", max compression
+gzip compressed data, was "typer_config-0.5.0.tar", max compression
```

## Comparing `typer_config-0.4.0.tar` & `typer_config-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.4.0/LICENSE
--rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.4.0/README.md
--rw-r--r--   0        0        0     2612 2023-05-23 03:04:29.520702 typer_config-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3706 2023-05-18 02:25:55.528865 typer_config-0.4.0/typer_config/__init__.py
--rw-r--r--   0        0        0     1355 2023-05-23 02:08:20.889710 typer_config-0.4.0/typer_config/__typing.py
--rw-r--r--   0        0        0     8661 2023-05-23 02:08:20.899710 typer_config-0.4.0/typer_config/loaders.py
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 typer_config-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.5.0/README.md
+-rw-r--r--   0        0        0     2612 2023-05-25 12:59:26.323443 typer_config-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4077 2023-05-25 12:57:11.693626 typer_config-0.5.0/typer_config/__init__.py
+-rw-r--r--   0        0        0     1480 2023-05-25 12:57:02.863636 typer_config-0.5.0/typer_config/__typing.py
+-rw-r--r--   0        0        0     9207 2023-05-25 12:57:02.863636 typer_config-0.5.0/typer_config/loaders.py
+-rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 typer_config-0.5.0/PKG-INFO
```

### Comparing `typer_config-0.4.0/LICENSE` & `typer_config-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.4.0/README.md` & `typer_config-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `typer_config-0.4.0/pyproject.toml` & `typer_config-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.4.0"
+version = "0.5.0"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
```

### Comparing `typer_config-0.4.0/typer_config/__init__.py` & `typer_config-0.5.0/typer_config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """
 Typer Configuration Utilities
 """
 
 from typer import BadParameter, CallbackParam, Context
 
 from .__typing import ConfigLoader, ConfigParameterCallback, TyperParameterValue
-from .loaders import dotenv_loader, json_loader, toml_loader, yaml_loader
+from .loaders import (
+    dotenv_loader,
+    json_loader,
+    loader_transformer,
+    toml_loader,
+    yaml_loader,
+)
 
 
 def conf_callback_factory(loader: ConfigLoader) -> ConfigParameterCallback:
     """Typer configuration callback factory.
 
     Args:
         loader (ConfigLoader): Config loader function that takes the value
@@ -44,15 +50,17 @@
         except Exception as ex:
             raise BadParameter(str(ex), ctx=ctx, param=param) from ex
         return param_value
 
     return _callback
 
 
-yaml_conf_callback: ConfigParameterCallback = conf_callback_factory(yaml_loader)
+yaml_conf_callback: ConfigParameterCallback = conf_callback_factory(
+    loader_transformer(yaml_loader, loader_conditional=lambda param_value: param_value)
+)
 """YAML typer config parameter callback.
 
 Args:
     ctx (typer.Context): typer context (automatically passed)
     param (typer.CallbackParam): typer callback parameter (automatically passed)
     param_value (TyperParameterValue): parameter value passed to typer (automatically
         passed)
@@ -60,15 +68,17 @@
 Raises:
     BadParameter: bad parameter value
 
 Returns:
     TyperParameterValue: must return back the given parameter
 """
 
-json_conf_callback: ConfigParameterCallback = conf_callback_factory(json_loader)
+json_conf_callback: ConfigParameterCallback = conf_callback_factory(
+    loader_transformer(json_loader, loader_conditional=lambda param_value: param_value)
+)
 """JSON typer config parameter callback.
 
 Args:
     ctx (typer.Context): typer context (automatically passed)
     param (typer.CallbackParam): typer callback parameter (automatically passed)
     param_value (TyperParameterValue): parameter value passed to typer (automatically
         passed)
@@ -77,15 +87,17 @@
     BadParameter: bad parameter value
 
 Returns:
     TyperParameterValue: must return back the given parameter
 """
 
 
-toml_conf_callback: ConfigParameterCallback = conf_callback_factory(toml_loader)
+toml_conf_callback: ConfigParameterCallback = conf_callback_factory(
+    loader_transformer(toml_loader, loader_conditional=lambda param_value: param_value)
+)
 """TOML typer config parameter callback.
 
 Args:
     ctx (typer.Context): typer context (automatically passed)
     param (typer.CallbackParam): typer callback parameter (automatically passed)
     param_value (TyperParameterValue): parameter value passed to typer (automatically
         passed)
@@ -93,15 +105,19 @@
 Raises:
     BadParameter: bad parameter value
 
 Returns:
     TyperParameterValue: must return back the given parameter
 """
 
-dotenv_conf_callback: ConfigParameterCallback = conf_callback_factory(dotenv_loader)
+dotenv_conf_callback: ConfigParameterCallback = conf_callback_factory(
+    loader_transformer(
+        dotenv_loader, loader_conditional=lambda param_value: param_value
+    )
+)
 """Dotenv typer config parameter callback.
 
 Args:
     ctx (typer.Context): typer context (automatically passed)
     param (typer.CallbackParam): typer callback parameter (automatically passed)
     param_value (TyperParameterValue): parameter value passed to typer (automatically
         passed)
```

### Comparing `typer_config-0.4.0/typer_config/__typing.py` & `typer_config-0.5.0/typer_config/__typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 ConfigDictTransformer: TypeAlias = Callable[[ConfigDict], ConfigDict]
 """ConfigDict transforming function."""
 
 ConfigLoader: TypeAlias = Callable[[TyperParameterValue], ConfigDict]
 """Configuration loader function."""
 
+ConfigLoaderConditional: TypeAlias = Callable[[TyperParameterValue], bool]
+"""Configuration loader conditional function."""
+
 ConfigParameterCallback: TypeAlias = Callable[
     [Context, CallbackParam, TyperParameterValue], TyperParameterValue
 ]
 """Typer config parameter callback function."""
 
 NoArgCallable: TypeAlias = Callable[[], Any]
 """No argument callable."""
```

### Comparing `typer_config-0.4.0/typer_config/loaders.py` & `typer_config-0.5.0/typer_config/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from warnings import warn
 
 from .__typing import (
     ConfigDict,
     ConfigDictAccessorPath,
     ConfigDictTransformer,
     ConfigLoader,
+    ConfigLoaderConditional,
     NoArgCallable,
     TyperParameterValue,
     TyperParameterValueTransformer,
 )
 
 USING_TOMLLIB = False
 TOML_MISSING = True
@@ -54,14 +55,15 @@
     DOTENV_MISSING = False
 except ImportError:  # pragma: no cover
     pass
 
 
 def loader_transformer(
     loader: ConfigLoader,
+    loader_conditional: Optional[ConfigLoaderConditional] = None,
     param_transformer: Optional[TyperParameterValueTransformer] = None,
     config_transformer: Optional[ConfigDictTransformer] = None,
 ) -> ConfigLoader:
     """Configuration loader transformer.
 
     This allows to transform the input and output of a configuration loader.
 
@@ -90,29 +92,38 @@
             param_transformer = lambda param: param if param else "pyproject.toml"
             config_transformer = lambda config: config["tool"]["my_tool"],
         )
         ```
 
     Args:
         loader (ConfigLoader): Loader to transform.
+        loader_condtional (Optional[ConfigLoaderConditional], optional): Function
+            to determine whether to execute loader. Defaults to None (no-op).
         param_transformer (Optional[TyperParameterValueTransformer], optional): Typer
             parameter transformer. Defaults to None (no-op).
         config_transformer (Optional[ConfigDictTransformer], optional): Config
             dictionary transformer. Defaults to None (no-op).
 
     Returns:
         ConfigLoader: Transformed config loader.
     """
 
     def _loader(param_value: TyperParameterValue) -> ConfigDict:
+        # Transform input
         if param_transformer is not None:
             param_value = param_transformer(param_value)
 
-        conf: ConfigDict = loader(param_value)
+        # Decide whether to execute loader
+        # NOTE: bad things can happen when `param_value=''`
+        # such as `--help` not working
+        conf: ConfigDict = {}
+        if loader_conditional is None or loader_conditional(param_value):
+            conf = loader(param_value)
 
+        # Transform output
         if config_transformer is not None:
             conf = config_transformer(conf)
 
         return conf
 
     return _loader
```

### Comparing `typer_config-0.4.0/PKG-INFO` & `typer_config-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
 Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
@@ -15,20 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: python-dotenv
```

