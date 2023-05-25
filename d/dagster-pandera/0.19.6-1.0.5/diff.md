# Comparing `tmp/dagster-pandera-0.19.6.tar.gz` & `tmp/dagster-pandera-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pandera-0.19.6.tar", last modified: Thu May 25 17:27:45 2023, max compression
+gzip compressed data, was "dagster-pandera-1.0.5.tar", last modified: Fri Aug 26 13:44:34 2022, max compression
```

## Comparing `dagster-pandera-0.19.6.tar` & `dagster-pandera-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:45.414399 dagster-pandera-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-25 17:27:45.414399 dagster-pandera-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:45.414399 dagster-pandera-0.19.6/dagster_pandera/
--rw-r--r--   0 root         (0) root         (0)     9258 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/dagster_pandera/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/dagster_pandera/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/dagster_pandera/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:45.414399 dagster-pandera-0.19.6/dagster_pandera.egg-info/
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-25 17:27:45.000000 dagster-pandera-0.19.6/dagster_pandera.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-25 17:27:45.000000 dagster-pandera-0.19.6/dagster_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:27:45.000000 dagster-pandera-0.19.6/dagster_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-25 17:27:45.000000 dagster-pandera-0.19.6/dagster_pandera.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:27:45.000000 dagster-pandera-0.19.6/dagster_pandera.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-25 17:27:45.418399 dagster-pandera-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-25 17:16:50.000000 dagster-pandera-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:34.908166 dagster-pandera-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      561 2022-08-26 13:44:34.908166 dagster-pandera-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:34.908166 dagster-pandera-1.0.5/dagster_pandera/
+-rw-r--r--   0 root         (0) root         (0)     9293 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/dagster_pandera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/dagster_pandera/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/dagster_pandera/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:34.908166 dagster-pandera-1.0.5/dagster_pandera.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      561 2022-08-26 13:44:34.000000 dagster-pandera-1.0.5/dagster_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2022-08-26 13:44:34.000000 dagster-pandera-1.0.5/dagster_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:34.000000 dagster-pandera-1.0.5/dagster_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2022-08-26 13:44:34.000000 dagster-pandera-1.0.5/dagster_pandera.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:44:34.000000 dagster-pandera-1.0.5/dagster_pandera.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2022-08-26 13:44:34.908166 dagster-pandera-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1330 2022-08-26 13:33:01.000000 dagster-pandera-1.0.5/setup.py
```

### Comparing `dagster-pandera-0.19.6/LICENSE` & `dagster-pandera-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-pandera-0.19.6/PKG-INFO` & `dagster-pandera-1.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.6
+Version: 1.0.5
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-pandera-0.19.6/dagster_pandera/__init__.py` & `dagster-pandera-1.0.5/dagster_pandera/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import itertools
 import re
-from typing import TYPE_CHECKING, Callable, Sequence, Type, Union
+from typing import TYPE_CHECKING, Callable, List, Type, Union
 
-import dagster._check as check
 import pandas as pd
 import pandera as pa
+
+import dagster._check as check
 from dagster import (
     DagsterType,
+    MetadataEntry,
     TableColumn,
     TableColumnConstraints,
     TableConstraints,
     TableSchema,
     TypeCheck,
     TypeCheckContext,
 )
 from dagster._core.definitions.metadata import MetadataValue
-from dagster._core.libraries import DagsterLibraryRegistry
+from dagster._core.utils import check_dagster_package_version
 
 from .version import __version__
 
 # NOTE: Pandera supports multiple dataframe libraries. Most of the alternatives
 # to pandas implement a pandas-like API wrapper around an underlying library
 # that can handle big data (a weakness of pandas). Typically this means the
 # data is only partly loaded into memory, or is distributed across multiple
@@ -31,15 +33,15 @@
 # However, some commented-out scaffolding has been left in place for support of
 # alternatives in the future. These sections are marked with "TODO: pending
 # alternative dataframe support".
 
 if TYPE_CHECKING:
     ValidatableDataFrame = pd.DataFrame
 
-DagsterLibraryRegistry.register("dagster-pandera", __version__)
+check_dagster_package_version("dagster-pandera", __version__)
 
 # ########################
 # ##### VALID DATAFRAME CLASSES
 # ########################
 
 # This layer of indirection is used because we may support alternative dataframe classes in the
 # future.
@@ -50,22 +52,23 @@
 # ##### PANDERA SCHEMA TO DAGSTER TYPE
 # ########################
 
 
 def pandera_schema_to_dagster_type(
     schema: Union[pa.DataFrameSchema, Type[pa.SchemaModel]],
 ) -> DagsterType:
-    """Convert a Pandera dataframe schema to a `DagsterType`.
+    """
+    Convert a Pandera dataframe schema to a `DagsterType`.
 
     The generated Dagster type will be given an automatically generated `name`. The schema's `title`
     property, `name` property, or class name (in that order) will be used. If neither `title` or
     `name` is defined, a name of the form `DagsterPanderaDataframe<n>` is generated.
 
     Additional metadata is also extracted from the Pandera schema and attached to the returned
-    `DagsterType` as a metadata dictionary. The extracted metadata includes:
+    `DagsterType` in an `MetadataEntry` object. The extracted metadata includes:
 
     - Descriptions on the schema and constituent columns and checks.
     - Data types for each column.
     - String representations of all column-wise checks.
     - String representations of all row-wise (i.e. "wide") checks.
 
     The returned `DagsterType` type will call the Pandera schema's `validate()` method in its type
@@ -90,43 +93,42 @@
     ):
         raise TypeError(
             "schema must be a pandera `DataFrameSchema` or a subclass of a pandera `SchemaModel`"
         )
 
     name = _extract_name_from_pandera_schema(schema)
     norm_schema = (
-        schema.to_schema()
+        schema.to_schema()  # type: ignore[attr-defined]
         if isinstance(schema, type) and issubclass(schema, pa.SchemaModel)
         else schema
     )
     tschema = _pandera_schema_to_table_schema(norm_schema)
     type_check_fn = _pandera_schema_to_type_check_fn(norm_schema, tschema)
 
     return DagsterType(
         type_check_fn=type_check_fn,
         name=name,
         description=norm_schema.description,
-        metadata={
-            "schema": MetadataValue.table_schema(tschema),
-        },
-        typing_type=pd.DataFrame,
+        metadata_entries=[
+            MetadataEntry("schema", value=MetadataValue.table_schema(tschema)),
+        ],
     )
 
 
 # call next() on this to generate next unique Dagster Type name for anonymous schemas
 _anonymous_schema_name_generator = (f"DagsterPanderaDataframe{i}" for i in itertools.count(start=1))
 
 
-def _extract_name_from_pandera_schema(
+def _extract_name_from_pandera_schema(  # type: ignore[return]
     schema: Union[pa.DataFrameSchema, Type[pa.SchemaModel]],
 ) -> str:
     if isinstance(schema, type) and issubclass(schema, pa.SchemaModel):
         return (
-            getattr(schema.Config, "title", None)
-            or getattr(schema.Config, "name", None)
+            getattr(schema.Config, "title", None)  # type: ignore[attr-defined]
+            or getattr(schema.Config, "name", None)  # type: ignore[attr-defined]
             or schema.__name__
         )
     elif isinstance(schema, pa.DataFrameSchema):
         return schema.title or schema.name or next(_anonymous_schema_name_generator)
 
 
 def _pandera_schema_to_type_check_fn(
@@ -144,17 +146,15 @@
                 return TypeCheck(
                     success=False,
                     description=f"Unexpected error during validation: {e}",
                 )
         else:
             return TypeCheck(
                 success=False,
-                description=(
-                    f"Must be one of {VALID_DATAFRAME_CLASSES}, not {type(value).__name__}."
-                ),
+                description=f"Must be one of {VALID_DATAFRAME_CLASSES}, not {type(value).__name__}.",
             )
 
         return TypeCheck(success=True)
 
     return type_check_fn
 
 
@@ -198,31 +198,30 @@
 def _pandera_schema_to_table_schema(schema: pa.DataFrameSchema) -> TableSchema:
     df_constraints = _pandera_schema_wide_checks_to_table_constraints(schema.checks)
     columns = [_pandera_column_to_table_column(col) for k, col in schema.columns.items()]
     return TableSchema(columns=columns, constraints=df_constraints)
 
 
 def _pandera_schema_wide_checks_to_table_constraints(
-    checks: Sequence[Union[pa.Check, pa.Hypothesis]]
+    checks: List[Union[pa.Check, pa.Hypothesis]]
 ) -> TableConstraints:
     return TableConstraints(other=[_pandera_check_to_table_constraint(check) for check in checks])
 
 
 def _pandera_check_to_table_constraint(pa_check: Union[pa.Check, pa.Hypothesis]) -> str:
     return _get_pandera_check_identifier(pa_check)
 
 
 def _pandera_column_to_table_column(pa_column: pa.Column) -> TableColumn:
     constraints = TableColumnConstraints(
         nullable=pa_column.nullable,
         unique=pa_column.unique,
         other=[_pandera_check_to_column_constraint(pa_check) for pa_check in pa_column.checks],
     )
-    name = check.not_none(pa_column.name, "name")
-    name = name if isinstance(name, str) else "/".join(name)
+    name: str = check.not_none(pa_column.name, "name")
     return TableColumn(
         name=name,
         type=str(pa_column.dtype),
         description=pa_column.description,
         constraints=constraints,
     )
```

### Comparing `dagster-pandera-0.19.6/dagster_pandera.egg-info/PKG-INFO` & `dagster-pandera-1.0.5/dagster_pandera.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.6
+Version: 1.0.5
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-pandera-0.19.6/setup.py` & `dagster-pandera-1.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_pandera/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_pandera/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=exec-used
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-pandera",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Integration layer for dagster and pandera.",
-    url="https://github.com/dagster-io/dagster",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_pandera_tests*"]),
-    include_package_data=True,
-    install_requires=["dagster==1.3.6", "pandas", "pandera>=0.14.2"],
-    extras_require={
-        "test": [
-            "pytest",
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-pandera",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description=("Integration layer for dagster and pandera."),
+        url="https://github.com/dagster-io/dagster",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
         ],
-    },
-)
+        packages=find_packages(exclude=["dagster_pandera_tests*"]),
+        include_package_data=True,
+        install_requires=["dagster==1.0.5", "pandas", "pandera>=0.9.0"],
+        extras_require={
+            "test": [
+                "pytest",
+            ],
+        },
+    )
```

