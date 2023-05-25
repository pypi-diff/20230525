# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.26.28.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.26.28.tar", last modified: Mon Dec 12 20:27:27 2022, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.919752 mypy-boto3-migration-hub-refactor-spaces-1.26.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2022-12-12 20:27:27.915752 mypy-boto3-migration-hub-refactor-spaces-1.26.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.911752 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28249 2022-12-12 20:26:53.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28220 2022-12-12 20:26:53.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.915752 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-12 20:27:27.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 20:27:27.919752 mypy-boto3-migration-hub-refactor-spaces-1.26.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2022-12-12 20:26:52.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.998837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-02-09 20:26:49.986837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.982837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28256 2023-02-09 20:26:34.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-02-09 20:26:34.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.986837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-09 20:26:49.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.998837 mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-09 20:26:33.000000 mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.26.28
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.68
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.28\nVersion:        "
-        " 1.26.28\nBuilder version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68\nVersion:        "
+        " 1.26.68\nBuilder version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.28")
+    print("1.26.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import RouteActivationStateType, RouteTypeType, ServiceEndpointTypeType
+from .literals import (
+    NetworkFabricTypeType,
+    RouteActivationStateType,
+    RouteTypeType,
+    ServiceEndpointTypeType,
+)
 from .paginator import (
     ListApplicationsPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentVpcsPaginator,
     ListRoutesPaginator,
     ListServicesPaginator,
 )
@@ -134,15 +139,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_application)
         """
 
     def create_environment(
         self,
         *,
         Name: str,
-        NetworkFabricType: Literal["TRANSIT_GATEWAY"],
+        NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import RouteActivationStateType, RouteTypeType, ServiceEndpointTypeType
+from .literals import (
+    NetworkFabricTypeType,
+    RouteActivationStateType,
+    RouteTypeType,
+    ServiceEndpointTypeType,
+)
 from .paginator import (
     ListApplicationsPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentVpcsPaginator,
     ListRoutesPaginator,
     ListServicesPaginator,
 )
@@ -126,15 +131,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_application)
         """
     def create_environment(
         self,
         *,
         Name: str,
-        NetworkFabricType: Literal["TRANSIT_GATEWAY"],
+        NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 ]
 HttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListEnvironmentVpcsPaginatorName = Literal["list_environment_vpcs"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRoutesPaginatorName = Literal["list_routes"]
 ListServicesPaginatorName = Literal["list_services"]
-NetworkFabricTypeType = Literal["TRANSIT_GATEWAY"]
+NetworkFabricTypeType = Literal["NONE", "TRANSIT_GATEWAY"]
 ProxyTypeType = Literal["API_GATEWAY"]
 RouteActivationStateType = Literal["ACTIVE", "INACTIVE"]
 RouteStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "INACTIVE", "UPDATING"]
 RouteTypeType = Literal["DEFAULT", "URI_PATH"]
 ServiceEndpointTypeType = Literal["LAMBDA", "URL"]
 ServiceStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 MigrationHubRefactorSpacesServiceName = Literal["migration-hub-refactor-spaces"]
@@ -136,24 +136,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -261,30 +263,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 ]
 HttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListEnvironmentVpcsPaginatorName = Literal["list_environment_vpcs"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRoutesPaginatorName = Literal["list_routes"]
 ListServicesPaginatorName = Literal["list_services"]
-NetworkFabricTypeType = Literal["TRANSIT_GATEWAY"]
+NetworkFabricTypeType = Literal["NONE", "TRANSIT_GATEWAY"]
 ProxyTypeType = Literal["API_GATEWAY"]
 RouteActivationStateType = Literal["ACTIVE", "INACTIVE"]
 RouteStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "INACTIVE", "UPDATING"]
 RouteTypeType = Literal["DEFAULT", "URI_PATH"]
 ServiceEndpointTypeType = Literal["LAMBDA", "URL"]
 ServiceStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 MigrationHubRefactorSpacesServiceName = Literal["migration-hub-refactor-spaces"]
@@ -134,24 +134,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -259,30 +261,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
     HttpMethodType,
+    NetworkFabricTypeType,
     RouteActivationStateType,
     RouteStateType,
     RouteTypeType,
     ServiceEndpointTypeType,
     ServiceStateType,
 )
 
@@ -171,15 +172,15 @@
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
     },
 )
 _OptionalCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEnvironmentRequestRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
@@ -584,15 +585,15 @@
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
     },
     total=False,
 )
@@ -646,15 +647,15 @@
     {
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -737,15 +738,15 @@
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
     HttpMethodType,
+    NetworkFabricTypeType,
     RouteActivationStateType,
     RouteStateType,
     RouteTypeType,
     ServiceEndpointTypeType,
     ServiceStateType,
 )
 
@@ -170,15 +171,15 @@
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
     },
 )
 _OptionalCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEnvironmentRequestRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
@@ -567,15 +568,15 @@
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
     },
     total=False,
 )
@@ -629,15 +630,15 @@
     {
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -720,15 +721,15 @@
         "Arn": str,
         "CreatedTime": datetime,
         "Description": str,
         "EnvironmentId": str,
         "Error": ErrorResponseTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
-        "NetworkFabricType": Literal["TRANSIT_GATEWAY"],
+        "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.26.28
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.68
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.26.28/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.26.68/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.26.28",
+    version="1.26.68",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.28 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.26.68 service generated with"
+        " mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

