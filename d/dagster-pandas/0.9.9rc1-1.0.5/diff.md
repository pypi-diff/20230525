# Comparing `tmp/dagster-pandas-0.9.9rc1.tar.gz` & `tmp/dagster-pandas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-pandas-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:25 2020, max compression
+gzip compressed data, was "dagster-pandas-1.0.5.tar", last modified: Fri Aug 26 13:44:16 2022, max compression
```

## Comparing `dagster-pandas-0.9.9rc1.tar` & `dagster-pandas-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       56 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      846 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/
--rw-r--r--   0 bobchen    (501) staff       (20)     1464 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    49516 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/constraints.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13352 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/data_frame.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/
--rw-r--r--   0 bobchen    (501) staff       (20)     1727 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/env.yaml
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/
--rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_prod.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       88 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_test.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)      111 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_prod.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)     1543 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/pipeline.py
--rw-r--r--   0 bobchen    (501) staff       (20)      124 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/solids.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       77 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/repository.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)    18338 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/validation.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      846 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1198 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2830 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1462 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.680066 dagster-pandas-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       88 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      823 2022-08-26 13:44:16.680066 dagster-pandas-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.672067 dagster-pandas-1.0.5/dagster_pandas/
+-rw-r--r--   0 root         (0) root         (0)     1465 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49418 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/constraints.py
+-rw-r--r--   0 root         (0) root         (0)    13389 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/data_frame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.672067 dagster-pandas-1.0.5/dagster_pandas/examples/
+-rw-r--r--   0 root         (0) root         (0)     2181 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.676066 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       54 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/env.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.676066 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/environments/
+-rw-r--r--   0 root         (0) root         (0)       87 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_prod.yaml
+-rw-r--r--   0 root         (0) root         (0)       82 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_test.yaml
+-rw-r--r--   0 root         (0) root         (0)      108 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_prod.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
+-rw-r--r--   0 root         (0) root         (0)     1212 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/ops.py
+-rw-r--r--   0 root         (0) root         (0)      118 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world/solids.yaml
+-rw-r--r--   0 root         (0) root         (0)       82 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/pandas_hello_world.yaml
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/examples/workspace.yaml
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    19456 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/validation.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/dagster_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:16.672067 dagster-pandas-1.0.5/dagster_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      823 2022-08-26 13:44:16.000000 dagster-pandas-1.0.5/dagster_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-08-26 13:44:16.000000 dagster-pandas-1.0.5/dagster_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:16.000000 dagster-pandas-1.0.5/dagster_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:44:16.000000 dagster-pandas-1.0.5/dagster_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:44:16.000000 dagster-pandas-1.0.5/dagster_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2022-08-26 13:44:16.680066 dagster-pandas-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-08-26 13:33:01.000000 dagster-pandas-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-pandas-0.9.9rc1/LICENSE` & `dagster-pandas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9rc1/PKG-INFO` & `dagster-pandas-1.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: dagster-pandas
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Utilities and examples for working with pandas and dagster, an opinionated framework for expressing data pipelines
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: # dagster-pandas
-        
-        The docs for `dagster-pandas` can be found
-        [here](https://docs.dagster.io/_apidocs/libraries/dagster_pandas).
-        
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dagster-pandas
+
+The docs for `dagster-pandas` can be found
+[here](https://docs.dagster.io/_apidocs/libraries/dagster-pandas).
+
+
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas/__init__.py` & `dagster-pandas-1.0.5/dagster_pandas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dagster.core.utils import check_dagster_package_version
+from dagster._core.utils import check_dagster_package_version
 
 from .constraints import (
     ColumnWithMetadataException,
     ConstraintWithMetadata,
     ConstraintWithMetadataException,
     MultiAggregateConstraintWithMetadata,
     MultiColumnConstraintWithMetadata,
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas/constraints.py` & `dagster-pandas-1.0.5/dagster_pandas/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from collections import defaultdict
 from datetime import datetime
 from functools import wraps
 
 import pandas as pd
 from pandas import DataFrame
 
-from dagster import DagsterType, EventMetadataEntry, TypeCheck, check
-from dagster.utils.backcompat import experimental_class_warning
+from dagster import DagsterType, MetadataEntry, TypeCheck
+from dagster import _check as check
+from dagster._utils.backcompat import experimental_class_warning
 
 
 class ConstraintViolationException(Exception):
     """Indicates that a constraint has been violated."""
 
 
 class ConstraintWithMetadataException(Exception):
@@ -38,28 +39,38 @@
         self.constraint_name = constraint_name
         self.constraint_description = constraint_description
         self.expectation = check.opt_inst_param(expectation, "expectation", (dict, list, str, set))
         self.offending = check.opt_inst_param(offending, "offending", (dict, list, str, set))
         self.actual = check.opt_inst_param(actual, "actual", (dict, list, str, set))
         super(ConstraintWithMetadataException, self).__init__(
             "Violated {} - {}, {} was/were expected, but we received {} which was/were {}".format(
-                constraint_name, constraint_description, expectation, offending, actual,
+                constraint_name,
+                constraint_description,
+                expectation,
+                offending,
+                actual,
             )
         )
 
+    def normalize_metadata_json_value(self, val):
+        if isinstance(val, set):
+            return list(val)
+        else:
+            return val
+
     def convert_to_metadata(self):
-        return EventMetadataEntry.json(
-            {
+        return MetadataEntry(
+            "constraint-metadata",
+            value={
                 "constraint_name": self.constraint_name,
                 "constraint_description": self.constraint_description,
-                "expected": self.expectation,
-                "offending": self.offending,
-                "actual": self.actual,
+                "expected": self.normalize_metadata_json_value(self.expectation),
+                "offending": self.normalize_metadata_json_value(self.offending),
+                "actual": self.normalize_metadata_json_value(self.actual),
             },
-            "constraint-metadata",
         )
 
     def return_as_typecheck(self):
         return TypeCheck(
             success=False, description=self.args[0], metadata_entries=[self.convert_to_metadata()]
         )
 
@@ -89,15 +100,15 @@
         self.constraint_name = constraint_name
         self.constraint_description = constraint_description
         self.column_name = column_name
         self.offending_rows = offending_rows
         super(ColumnConstraintViolationException, self).__init__(self.construct_message())
 
     def construct_message(self):
-        base_message = "Violated {constraint_name} ({constraint_description}) for Column Name ({column_name}) ".format(
+        base_message = 'Violated "{constraint_name}" for column "{column_name}" - {constraint_description}'.format(
             constraint_name=self.constraint_name,
             constraint_description=self.constraint_description,
             column_name=self.column_name,
         )
         if self.offending_rows is not None:
             base_message += "The offending (index, row values) are the following: {}".format(
                 self.offending_rows
@@ -112,30 +123,30 @@
             constraint_description,
             expectation,
             offending,
             actual,
         )
 
 
-class Constraint(object):
+class Constraint:
     """
     Base constraint object that all constraints inherit from.
 
     Args:
         error_description (Optional[str]): The plain string description that is output in the terminal if the constraint fails.
         markdown_description (Optional[str]): A markdown supported description that is emitted by dagit if the constraint fails.
     """
 
     def __init__(self, error_description=None, markdown_description=None):
         self.name = self.__class__.__name__
         self.markdown_description = check.str_param(markdown_description, "markdown_description")
         self.error_description = check.str_param(error_description, "error_description")
 
 
-class ConstraintWithMetadata(object):
+class ConstraintWithMetadata:
     """
     This class defines a base constraint over pandas DFs with organized metadata
 
     args:
         description (str): description of the constraint
         validation_fn (Callable[[DataFrame], Tuple[bool, dict[str, Union[dict,list, str, set]]]]:
                     the validation function to run over inputted data
@@ -188,34 +199,34 @@
             )
         return DagsterType(
             name=self.name,
             description="A Pandas DataFrame with the following validation: {}".format(
                 self.description
             ),
             type_check_fn=lambda x: self.validate(x, *args),
-            **kwargs
+            **kwargs,
         )
 
 
 class MultiConstraintWithMetadata(ConstraintWithMetadata):
     """
-        Use this class if you have multiple constraints to check over the entire dataframe
+    Use this class if you have multiple constraints to check over the entire dataframe
 
-        args:
-            description (str): description of the constraint
-            validation_fn_arr(List[Callable[[DataFrame], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
-                        a list of the validation functions to run over inputted data
-                        Each function should return a tuple of a boolean for success or failure, and a dict containing
-                        metadata about the test -- this metadata will be passed to the resulting exception if validation
-                        fails.
-            resulting_exception (ConstraintWithMetadataException):  what response a failed typecheck should induce
-            raise_or_typecheck (Optional[bool]): whether to raise an exception (if set to True) or emit a failed typecheck event
-                        (if set to False) when validation fails
-            name (Optional[str]): what to call the constraint, defaults to the class name.
-        """
+    args:
+        description (str): description of the constraint
+        validation_fn_arr(List[Callable[[DataFrame], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
+                    a list of the validation functions to run over inputted data
+                    Each function should return a tuple of a boolean for success or failure, and a dict containing
+                    metadata about the test -- this metadata will be passed to the resulting exception if validation
+                    fails.
+        resulting_exception (ConstraintWithMetadataException):  what response a failed typecheck should induce
+        raise_or_typecheck (Optional[bool]): whether to raise an exception (if set to True) or emit a failed typecheck event
+                    (if set to False) when validation fails
+        name (Optional[str]): what to call the constraint, defaults to the class name.
+    """
 
     def __init__(
         self,
         description,
         validation_fn_arr,
         resulting_exception,
         raise_or_typecheck=True,
@@ -485,31 +496,31 @@
                 raise exc
             else:
                 return exc.return_as_typecheck()
 
 
 class MultiColumnConstraintWithMetadata(ColumnConstraintWithMetadata):
     """
-        This class is useful for constructing more complicated relationships between columns
-        and expectations -- i.e. you want some validations on column A, others on column B, etc.
-        This lets you package up the metadata neatly,
-        and also allows for cases like 'fail if any one of these constraints fails but still run all of them'
-
-        Args:
-            description (str): description of the overall set of validations
-            fn_and_columns_dict (Dict[str, List[Callable[[Any], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
-                                        while this is a relatively complex type,
-                                        what it amounts to is 'a dict mapping columns to the functions to
-                                        run on them'
-            resulting_exception (type): the response to generate if validation fails. Subclass of
-                                        ConstraintWithMetadataException
-            raise_or_typecheck (Optional[bool]):  whether to raise an exception (true) or a failed typecheck (false)
-            type_for_internal (Optional[type]): what type to use for internal validators.  Subclass of
-                                                ConstraintWithMetadata
-            name (Optional[str]): what to call the constraint, defaults to the class name.
+    This class is useful for constructing more complicated relationships between columns
+    and expectations -- i.e. you want some validations on column A, others on column B, etc.
+    This lets you package up the metadata neatly,
+    and also allows for cases like 'fail if any one of these constraints fails but still run all of them'
+
+    Args:
+        description (str): description of the overall set of validations
+        fn_and_columns_dict (Dict[str, List[Callable[[Any], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
+                                    while this is a relatively complex type,
+                                    what it amounts to is 'a dict mapping columns to the functions to
+                                    run on them'
+        resulting_exception (type): the response to generate if validation fails. Subclass of
+                                    ConstraintWithMetadataException
+        raise_or_typecheck (Optional[bool]):  whether to raise an exception (true) or a failed typecheck (false)
+        type_for_internal (Optional[type]): what type to use for internal validators.  Subclass of
+                                            ConstraintWithMetadata
+        name (Optional[str]): what to call the constraint, defaults to the class name.
     """
 
     def __init__(
         self,
         description,
         fn_and_columns_dict,
         resulting_exception,
@@ -568,30 +579,30 @@
 
     def validate(self, data, *args, **kwargs):
         return ConstraintWithMetadata.validate(self, data, *args, **kwargs)
 
 
 class MultiAggregateConstraintWithMetadata(MultiColumnConstraintWithMetadata):
     """
-        This class is similar to multicolumn, but takes in functions that operate on the whole column at once
-        rather than ones that operate on each value --
-        consider this similar to the difference between apply-map and apply aggregate.
-
-        Args:
-            description (str): description of the overall set of validations (TODO:  support multiple descriptions)
-            fn_and_columns_dict (Dict[str, List[Callable[[pd.Series], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
-                                        while this is a relatively complex type,
-                                        what it amounts to is a dict mapping columns to the functions to
-                                        run on them'
-            resulting_exception (type): the response to generate if validation fails. Subclass of
-                                        ConstraintWithMetadataException
-            raise_or_typecheck (Optional[bool]):  whether to raise an exception (true) or a failed typecheck (false)
-            type_for_internal (Optional[type]): what type to use for internal validators.  Subclass of
-                                                ConstraintWithMetadata
-            name (Optional[str]): what to call the constraint, defaults to the class name.
+    This class is similar to multicolumn, but takes in functions that operate on the whole column at once
+    rather than ones that operate on each value --
+    consider this similar to the difference between apply-map and apply aggregate.
+
+    Args:
+        description (str): description of the overall set of validations (TODO:  support multiple descriptions)
+        fn_and_columns_dict (Dict[str, List[Callable[[pd.Series], Tuple[bool, dict[str, Union[dict,list, str, set]]]]]):
+                                    while this is a relatively complex type,
+                                    what it amounts to is a dict mapping columns to the functions to
+                                    run on them'
+        resulting_exception (type): the response to generate if validation fails. Subclass of
+                                    ConstraintWithMetadataException
+        raise_or_typecheck (Optional[bool]):  whether to raise an exception (true) or a failed typecheck (false)
+        type_for_internal (Optional[type]): what type to use for internal validators.  Subclass of
+                                            ConstraintWithMetadata
+        name (Optional[str]): what to call the constraint, defaults to the class name.
     """
 
     def __init__(
         self,
         description,
         fn_and_columns_dict,
         resulting_exception,
@@ -629,28 +640,29 @@
     Usage:
         As a validation function for a
         :py:class:'~dagster_pandas.constraints.ColumnAggregateConstraintWithMetadata'
         or :py:class:'~dagster_pandas.constraints.MultiAggregateConstraintWithMetadata'
     Example:
         .. code-block:: python
             aggregate_validator = MultiAggregateConstraintWithMetadata(
-            "confirms all values are unique",
-            {'bar': [all_unique_validator]},
-            ConstraintWithMetadataException,
-            raise_or_typecheck=False,
+                "confirms all values are unique",
+                {'bar': [all_unique_validator]},
+                ConstraintWithMetadataException,
+                raise_or_typecheck=False,
             )
             ntype = create_structured_dataframe_type(
-            "NumericType",
-            columns_aggregate_validator=aggregate_validator
+                "NumericType",
+                columns_aggregate_validator=aggregate_validator
             )
-            @solid(output_defs=[OutputDefinition(name='basic_dataframe', dagster_type=ntype)])
+            @op(out={'basic_dataframe': Out(dagster_type=ntype)})
             def create_dataframe(_):
                 yield Output(
-                DataFrame({'foo': [1, 2, 3], 'bar': [9, 10, 10]}), output_name='basic_dataframe',
-            )
+                    DataFrame({'foo': [1, 2, 3], 'bar': [9, 10, 10]}),
+                    output_name='basic_dataframe',
+                )
             #will fail with
             metadata['offending'] == {'bar': {'all_unique_validator': 'a violation'}}
             metadata['actual'] == {'bar': {'all_unique_validator': [10.0]}}
     """
     column = pd.Series(column)
     duplicated = column.duplicated()
     if ignore_missing_vals:
@@ -694,28 +706,29 @@
         pass returned functions as column validators to
          :py:class:'~dagster_pandas.constraints.ColumnConstraintWithMetadata'
         or :py:class:'~dagster_pandas.constraints.MultiColumnConstraintWithMetadata'
     Examples:
         .. code-block:: python
             in_range_validator = column_range_validation_factory(1, 3, ignore_missing_vals=True)
             column_validator = MultiColumnConstraintWithMetadata(
-                            "confirms values are numbers in a range",
-                            {'foo': [in_range_validator]},
-                            ColumnWithMetadataException,
-                            raise_or_typecheck=False,
-                        )
+                "confirms values are numbers in a range",
+                {'foo': [in_range_validator]},
+                ColumnWithMetadataException,
+                raise_or_typecheck=False,
+            )
             ntype = create_structured_dataframe_type(
-            "NumericType",
-            columns_validator=column_validator
+                "NumericType",
+                columns_validator=column_validator
             )
-            @solid(output_defs=[OutputDefinition(name='basic_dataframe', dagster_type=ntype)])
+            @op(out={'basic_dataframe': Out(dagster_type=ntype)})
             def create_dataframe(_):
                 yield Output(
-                DataFrame({'foo': [1, 2, 7], 'bar': [9, 10, 10]}), output_name='basic_dataframe',
-            )
+                    DataFrame({'foo': [1, 2, 7], 'bar': [9, 10, 10]}),
+                    output_name='basic_dataframe',
+                )
             #will fail with
             metadata['offending'] == {'foo': {'in_range_validation_fn': ['row 2']}}
             metadata['actual'] == {'foo': {'in_range_validation_fn': [7]}}
 
     """
     if minim is None:
         if isinstance(maxim, datetime):
@@ -756,43 +769,44 @@
         :py:class:'~dagster_pandas.constraints.ColumnConstraintWithMetadata'
         or :py:class:'~dagster_pandas.constraints.MultiColumnConstraintWithMetadata'
 
     Example:
         .. code-block:: python
             categorical_validation_fn = categorical_column_validator_factory([1, 2])
             column_validator = MultiColumnConstraintWithMetadata(
-                            "confirms values are numbers in a range",
-                            {'foo': [categorical_validation_fn]},
-                            ColumnWithMetadataException,
-                            raise_or_typecheck=False,
-                        )
+                "confirms values are numbers in a range",
+                {'foo': [categorical_validation_fn]},
+                ColumnWithMetadataException,
+                raise_or_typecheck=False,
+            )
             ntype = create_structured_dataframe_type(
-            "NumericType",
-            columns_validator=column_validator
+                "NumericType",
+                columns_validator=column_validator
             )
-            @solid(output_defs=[OutputDefinition(name='basic_dataframe', dagster_type=ntype)])
+            @op(out={'basic_dataframe': Out(dagster_type=ntype)})
             def create_dataframe(_):
                 yield Output(
-                DataFrame({'foo': [1, 2, 7], 'bar': [9, 10, 10]}), output_name='basic_dataframe',
-            )
+                    DataFrame({'foo': [1, 2, 7], 'bar': [9, 10, 10]}),
+                    output_name='basic_dataframe',
+                )
             #will fail with
             metadata['offending'] == {'foo': {'categorical_validation_fn': ['row 2']}}
             metadata['actual'] == {'foo': {'categorical_validation_fn': [7]}}
 
     """
 
     categories = set(categories)
 
     def categorical_validation_fn(x):
         if ignore_missing_vals and pd.isnull(x):
             return True, {}
         return (x in categories), {}
 
-    categorical_validation_fn.__doc__ = "checks whether values are within this set of values: {}".format(
-        categories
+    categorical_validation_fn.__doc__ = (
+        "checks whether values are within this set of values: {}".format(categories)
     )
     if ignore_missing_vals:
         categorical_validation_fn.__doc__ += ", ignoring nulls"
 
     return categorical_validation_fn
 
 
@@ -810,28 +824,29 @@
         :py:class:'~dagster_pandas.constraints.ColumnConstraintWithMetadata'
         or :py:class:'~dagster_pandas.constraints.MultiColumnConstraintWithMetadata'
 
     Examples:
         .. code-block:: python
             dtype_is_num_validator = dtype_in_set_validation_factory((int, float, int64, float64))
             column_validator = MultiColumnConstraintWithMetadata(
-            "confirms values are numbers in a range",
-            {'foo': [dtype_is_num_validator]},
-            ColumnWithMetadataException,
-            raise_or_typecheck=False,
+                "confirms values are numbers in a range",
+                {'foo': [dtype_is_num_validator]},
+                ColumnWithMetadataException,
+                raise_or_typecheck=False,
             )
             ntype = create_structured_dataframe_type(
-            "NumericType",
-            columns_validator=column_validator
+                "NumericType",
+                columns_validator=column_validator
             )
-            @solid(output_defs=[OutputDefinition(name='basic_dataframe', dagster_type=ntype)])
+            @op(out={'basic_dataframe': Out(dagster_type=ntype)})
             def create_dataframe(_):
                 yield Output(
-                DataFrame({'foo': [1, 'a', 7], 'bar': [9, 10, 10]}), output_name='basic_dataframe',
-            )
+                    DataFrame({'foo': [1, 'a', 7], 'bar': [9, 10, 10]}),
+                    output_name='basic_dataframe',
+                )
             #will fail with
             metadata['offending'] == {'foo': {'categorical_validation_fn': ['row 1']}}
             metadata['actual'] == {'foo': {'categorical_validation_fn': ['a']}}
 
     """
 
     def dtype_in_set_validation_fn(x):
@@ -890,38 +905,34 @@
     @staticmethod
     def get_offending_row_pairs(dataframe, column_name):
         return zip(dataframe.index.tolist(), dataframe[column_name].tolist())
 
 
 class ColumnDTypeFnConstraint(ColumnConstraint):
     """
-    A column constraint that applies a pandas dtype validation function to a columns dtypes.
+    A column constraint that applies a pandas dtype validation function to a columns dtype.
 
     Args:
         type_fn (Callable[[Set[str]], bool]): This is a function that takes the pandas columns dtypes and
             returns if those dtypes match the types it expects. See pandas.core.dtypes.common for examples.
     """
 
     def __init__(self, type_fn):
         self.type_fn = check.callable_param(type_fn, "type_fn")
-        description = "{fn} must evaluate to True for column dtypes".format(
-            fn=self.type_fn.__name__
-        )
+        description = f'Dtype must satisfy "{self.type_fn.__name__}"'
         super(ColumnDTypeFnConstraint, self).__init__(
             error_description=description, markdown_description=description
         )
 
     def validate(self, dataframe, column_name):
-        received_dtypes = dataframe[column_name].dtype
-        if not self.type_fn(received_dtypes):
+        column_dtype = dataframe[column_name].dtype
+        if not self.type_fn(column_dtype):
             raise ColumnConstraintViolationException(
                 constraint_name=self.name,
-                constraint_description="{base_error_message}. Dtypes received: {received_dtypes}.".format(
-                    base_error_message=self.error_description, received_dtypes=received_dtypes
-                ),
+                constraint_description=f'{self.error_description}, but was "{column_dtype}"',
                 column_name=column_name,
             )
 
 
 class ColumnDTypeInSetConstraint(ColumnConstraint):
     """
     A column constraint that validates the pandas column dtypes based on the expected set of dtypes.
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas/data_frame.py` & `dagster-pandas-1.0.5/dagster_pandas/data_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,52 +6,57 @@
 )
 from dagster_pandas.validation import PandasColumn, validate_constraints
 
 from dagster import (
     AssetMaterialization,
     DagsterInvariantViolationError,
     DagsterType,
-    EventMetadataEntry,
     Field,
+    MetadataEntry,
     StringSource,
     TypeCheck,
-    check,
-    dagster_type_loader,
-    dagster_type_materializer,
 )
-from dagster.config.field_utils import Selector
-from dagster.utils import dict_without_keys
-from dagster.utils.backcompat import canonicalize_backcompat_args, experimental
+from dagster import _check as check
+from dagster import dagster_type_loader, dagster_type_materializer
+from dagster._annotations import experimental
+from dagster._check import CheckError
+from dagster._config import Selector
+from dagster._core.definitions.metadata import normalize_metadata
+from dagster._core.errors import DagsterInvalidMetadata
+from dagster._utils import dict_without_keys
 
 CONSTRAINT_BLACKLIST = {ColumnDTypeFnConstraint, ColumnDTypeInSetConstraint}
 
 
 @dagster_type_materializer(
     Selector(
         {
             "csv": {
                 "path": StringSource,
                 "sep": Field(StringSource, is_required=False, default_value=","),
             },
             "parquet": {"path": StringSource},
             "table": {"path": StringSource},
+            "pickle": {"path": StringSource},
         },
     )
 )
 def dataframe_materializer(_context, config, pandas_df):
     check.inst_param(pandas_df, "pandas_df", pd.DataFrame)
     file_type, file_options = list(config.items())[0]
 
     if file_type == "csv":
         path = file_options["path"]
         pandas_df.to_csv(path, index=False, **dict_without_keys(file_options, "path"))
     elif file_type == "parquet":
         pandas_df.to_parquet(file_options["path"])
     elif file_type == "table":
         pandas_df.to_csv(file_options["path"], sep="\t", index=False)
+    elif file_type == "pickle":
+        pandas_df.to_pickle(file_options["path"])
     else:
         check.failed("Unsupported file_type {file_type}".format(file_type=file_type))
 
     return AssetMaterialization.file(file_options["path"])
 
 
 @dagster_type_loader(
@@ -59,54 +64,58 @@
         {
             "csv": {
                 "path": StringSource,
                 "sep": Field(StringSource, is_required=False, default_value=","),
             },
             "parquet": {"path": StringSource},
             "table": {"path": StringSource},
+            "pickle": {"path": StringSource},
         },
     )
 )
 def dataframe_loader(_context, config):
     file_type, file_options = list(config.items())[0]
 
     if file_type == "csv":
         path = file_options["path"]
         return pd.read_csv(path, **dict_without_keys(file_options, "path"))
     elif file_type == "parquet":
         return pd.read_parquet(file_options["path"])
     elif file_type == "table":
         return pd.read_csv(file_options["path"], sep="\t")
+    elif file_type == "pickle":
+        return pd.read_pickle(file_options["path"])
     else:
         raise DagsterInvariantViolationError(
             "Unsupported file_type {file_type}".format(file_type=file_type)
         )
 
 
 def df_type_check(_, value):
     if not isinstance(value, pd.DataFrame):
         return TypeCheck(success=False)
     return TypeCheck(
         success=True,
         metadata_entries=[
-            EventMetadataEntry.text(str(len(value)), "row_count", "Number of rows in DataFrame"),
+            MetadataEntry("row_count", value=str(len(value))),
             # string cast columns since they may be things like datetime
-            EventMetadataEntry.json({"columns": list(map(str, value.columns))}, "metadata"),
+            MetadataEntry("metadata", value={"columns": list(map(str, value.columns))}),
         ],
     )
 
 
 DataFrame = DagsterType(
     name="PandasDataFrame",
     description="""Two-dimensional size-mutable, potentially heterogeneous
     tabular data structure with labeled axes (rows and columns).
     See http://pandas.pydata.org/""",
     loader=dataframe_loader,
     materializer=dataframe_materializer,
     type_check_fn=df_type_check,
+    typing_type=pd.DataFrame,
 )
 
 
 def _construct_constraint_list(constraints):
     def add_bullet(constraint_list, constraint_description):
         return constraint_list + "+ {constraint_description}\n".format(
             constraint_description=constraint_description
@@ -149,38 +158,37 @@
     name,
     description=None,
     columns=None,
     event_metadata_fn=None,
     dataframe_constraints=None,
     loader=None,
     materializer=None,
-    input_hydration_config=None,
-    output_materialization_config=None,
 ):
     """
     Constructs a custom pandas dataframe dagster type.
 
     Args:
         name (str): Name of the dagster pandas type.
         description (Optional[str]): A markdown-formatted string, displayed in tooling.
         columns (Optional[List[PandasColumn]]): A list of :py:class:`~dagster.PandasColumn` objects
             which express dataframe column schemas and constraints.
-        event_metadata_fn (Optional[func]): A callable which takes your dataframe and returns a list of EventMetadata
-            which allow you to express things like summary statistics during runtime.
+        event_metadata_fn (Optional[Callable[[], Union[Dict[str, Union[str, float, int, Dict, MetadataValue]], List[MetadataEntry]]]]):
+            A callable which takes your dataframe and returns a dict with string label keys and
+            MetadataValue values. Can optionally return a List[MetadataEntry].
         dataframe_constraints (Optional[List[DataFrameConstraint]]): A list of objects that inherit from
             :py:class:`~dagster.DataFrameConstraint`. This allows you to express dataframe-level constraints.
         loader (Optional[DagsterTypeLoader]): An instance of a class that
             inherits from :py:class:`~dagster.DagsterTypeLoader`. If None, we will default
             to using `dataframe_loader`.
         materializer (Optional[DagsterTypeMaterializer]): An instance of a class
             that inherits from :py:class:`~dagster.DagsterTypeMaterializer`. If None, we will
             default to using `dataframe_materializer`.
     """
     # We allow for the plugging in of dagster_type_loaders/materializers so that
-    # Users can load and matrerialize their custom dataframes via configuration their own way if the default
+    # Users can load and materialize their custom dataframes via configuration their own way if the default
     # configs don't suffice. This is purely optional.
     check.str_param(name, "name")
     event_metadata_fn = check.opt_callable_param(event_metadata_fn, "event_metadata_fn")
     description = create_dagster_pandas_dataframe_description(
         check.opt_str_param(description, "description", default=""),
         check.opt_list_param(columns, "columns", of_type=PandasColumn),
     )
@@ -192,57 +200,46 @@
                 description="Must be a pandas.DataFrame. Got value of type. {type_name}".format(
                     type_name=type(value).__name__
                 ),
             )
 
         try:
             validate_constraints(
-                value, pandas_columns=columns, dataframe_constraints=dataframe_constraints
+                value,
+                pandas_columns=columns,
+                dataframe_constraints=dataframe_constraints,
             )
         except ConstraintViolationException as e:
             return TypeCheck(success=False, description=str(e))
 
         return TypeCheck(
             success=True,
             metadata_entries=_execute_summary_stats(name, value, event_metadata_fn)
             if event_metadata_fn
             else None,
         )
 
-    loader_ = canonicalize_backcompat_args(
-        loader, "loader", input_hydration_config, "input_hydration_config", "0.10.0",
-    )
-    materializer_ = canonicalize_backcompat_args(
-        materializer,
-        "materializer",
-        output_materialization_config,
-        "output_materialization_config",
-        "0.10.0",
-    )
-
     return DagsterType(
         name=name,
         type_check_fn=_dagster_type_check,
-        loader=loader_ if loader_ else dataframe_loader,
-        materializer=materializer_ if materializer_ else dataframe_materializer,
+        loader=loader if loader else dataframe_loader,
+        materializer=materializer if materializer else dataframe_materializer,
         description=description,
     )
 
 
 @experimental
 def create_structured_dataframe_type(
     name,
     description=None,
     columns_validator=None,
     columns_aggregate_validator=None,
     dataframe_validator=None,
     loader=None,
     materializer=None,
-    input_hydration_config=None,
-    output_materialization_config=None,
 ):
     """
 
     Args:
         name (str): the name of the new type
         description (Optional[str]): the description of the new type
         columns_validator (Optional[Union[ColumnConstraintWithMetadata, MultiColumnConstraintWithMetadata]]):
@@ -294,56 +291,56 @@
         for key, result in individual_result_dict.items():
             result_val = result.success
             if result_val:
                 continue
             typechecks_succeeded = typechecks_succeeded and result_val
             result_dict = result.metadata_entries[0].entry_data.data
             metadata.append(
-                EventMetadataEntry.json(result_dict, "{}-constraint-metadata".format(key),)
+                MetadataEntry(
+                    "{}-constraint-metadata".format(key),
+                    value=result_dict,
+                )
             )
             constraint_clauses.append("{} failing constraints, {}".format(key, result.description))
         # returns aggregates, then column, then dataframe
         return TypeCheck(
             success=typechecks_succeeded,
             description=overall_description.format(constraint_clauses),
             metadata_entries=sorted(metadata, key=lambda x: x.label),
         )
 
     description = check.opt_str_param(description, "description", default="")
-    loader_ = canonicalize_backcompat_args(
-        loader, "loader", input_hydration_config, "input_hydration_config", "0.10.0",
-    )
-    materializer_ = canonicalize_backcompat_args(
-        materializer,
-        "materializer",
-        output_materialization_config,
-        "output_materialization_config",
-        "0.10.0",
-    )
     return DagsterType(
         name=name,
         type_check_fn=_dagster_type_check,
-        loader=loader_ if loader_ else dataframe_loader,
-        materializer=materializer_ if materializer_ else dataframe_materializer,
+        loader=loader if loader else dataframe_loader,
+        materializer=materializer if loader else dataframe_materializer,
         description=description,
     )
 
 
 def _execute_summary_stats(type_name, value, event_metadata_fn):
     if not event_metadata_fn:
         return []
 
-    metadata_entries = event_metadata_fn(value)
+    metadata_or_metadata_entries = event_metadata_fn(value)
 
-    if not (
-        isinstance(metadata_entries, list)
-        and all(isinstance(item, EventMetadataEntry) for item in metadata_entries)
-    ):
-        raise DagsterInvariantViolationError(
-            (
-                "The return value of the user-defined summary_statistics function "
-                "for pandas data frame type {type_name} returned {value}. "
-                "This function must return List[EventMetadataEntry]"
-            ).format(type_name=type_name, value=repr(metadata_entries))
-        )
+    invalid_message = (
+        "The return value of the user-defined summary_statistics function for pandas "
+        f"data frame type {type_name} returned {value}. This function must return "
+        "Union[Dict[str, Union[str, float, int, Dict, MetadataValue]], List[MetadataEntry]]"
+    )
+
+    metadata = None
+    metadata_entries = None
+
+    if isinstance(metadata_or_metadata_entries, list):
+        metadata_entries = metadata_or_metadata_entries
+    elif isinstance(metadata_or_metadata_entries, dict):
+        metadata = metadata_or_metadata_entries
+    else:
+        raise DagsterInvariantViolationError(invalid_message)
 
-    return metadata_entries
+    try:
+        return normalize_metadata(metadata, metadata_entries)
+    except (DagsterInvalidMetadata, CheckError):
+        raise DagsterInvariantViolationError(invalid_message)
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas/validation.py` & `dagster-pandas-1.0.5/dagster_pandas/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     is_bool_dtype,
     is_float_dtype,
     is_integer_dtype,
     is_numeric_dtype,
     is_string_dtype,
 )
 
-from dagster import DagsterInvariantViolationError, check
+from dagster import DagsterInvariantViolationError
+from dagster import _check as check
 
 PANDAS_NUMERIC_TYPES = {"int64", "float"}
 
 
 def _construct_keyword_constraints(non_nullable, unique, ignore_missing_vals):
     non_nullable = check.bool_param(non_nullable, "exists")
     unique = check.bool_param(unique, "unique")
@@ -253,14 +254,15 @@
         name,
         min_datetime=Timestamp.min,
         max_datetime=Timestamp.max,
         non_nullable=False,
         unique=False,
         ignore_missing_vals=False,
         is_required=None,
+        tz=None,
     ):
         """
         Simple constructor for PandasColumns that expresses datetime constraints on 'datetime64[ns]' dtypes.
 
         Args:
             name (str): Name of the column. This must match up with the column name in the dataframe you
                 expect to receive.
@@ -271,19 +273,36 @@
             non_nullable (Optional[bool]): If true, this column will enforce a constraint that all values in the column
                 ought to be non null values.
             unique (Optional[bool]): If true, this column will enforce a uniqueness constraint on the column values.
             ignore_missing_vals (Optional[bool]): A flag that is passed into most constraints. If true, the constraint will
                 only evaluate non-null data. Ignore_missing_vals and non_nullable cannot both be True.
             is_required (Optional[bool]): Flag indicating the optional/required presence of the column.
                 If the column exists the validate function will validate the column. Default to True.
+            tz (Optional[str]): Required timezone for values eg: tz='UTC', tz='Europe/Dublin', tz='US/Eastern'.
+                Defaults to None, meaning naive datetime values.
         """
+        if tz is None:
+            datetime_constraint = ColumnDTypeInSetConstraint({"datetime64[ns]"})
+        else:
+            datetime_constraint = ColumnDTypeInSetConstraint({f"datetime64[ns, {tz}]"})
+            # One day more/less than absolute min/max to prevent OutOfBoundsDatetime errors when converting min/max to be tz aware
+            if min_datetime.tz_localize(None) == Timestamp.min:
+                min_datetime = Timestamp("1677-09-22 00:12:43.145225Z")
+            if max_datetime.tz_localize(None) == Timestamp.max:
+                max_datetime = Timestamp("2262-04-10 23:47:16.854775807Z")
+            # Convert bounds to same tz
+            if Timestamp(min_datetime).tz is None:
+                min_datetime = Timestamp(min_datetime).tz_localize(tz)
+            if Timestamp(max_datetime).tz is None:
+                max_datetime = Timestamp(max_datetime).tz_localize(tz)
+
         return PandasColumn(
             name=check.str_param(name, "name"),
             constraints=[
-                ColumnDTypeInSetConstraint({"datetime64[ns]"}),
+                datetime_constraint,
                 InRangeColumnConstraint(
                     min_datetime, max_datetime, ignore_missing_vals=ignore_missing_vals
                 ),
             ]
             + _construct_keyword_constraints(
                 non_nullable=non_nullable, unique=unique, ignore_missing_vals=ignore_missing_vals
             ),
@@ -317,15 +336,15 @@
             is_required=is_required,
         )
 
     @staticmethod
     def categorical_column(
         name,
         categories,
-        of_types="object",
+        of_types=frozenset({"category", "object"}),
         non_nullable=False,
         unique=False,
         ignore_missing_vals=False,
         is_required=None,
     ):
         """
         Simple constructor for PandasColumns that expresses categorical constraints on specified dtypes.
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/PKG-INFO` & `dagster-pandas-1.0.5/dagster_pandas.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: dagster-pandas
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Utilities and examples for working with pandas and dagster, an opinionated framework for expressing data pipelines
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: # dagster-pandas
-        
-        The docs for `dagster-pandas` can be found
-        [here](https://docs.dagster.io/_apidocs/libraries/dagster_pandas).
-        
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dagster-pandas
+
+The docs for `dagster-pandas` can be found
+[here](https://docs.dagster.io/_apidocs/libraries/dagster-pandas).
+
+
```

### Comparing `dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/SOURCES.txt` & `dagster-pandas-1.0.5/dagster_pandas.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dagster_pandas/__init__.py
 dagster_pandas/constraints.py
 dagster_pandas/data_frame.py
+dagster_pandas/py.typed
 dagster_pandas/validation.py
 dagster_pandas/version.py
 dagster_pandas.egg-info/PKG-INFO
 dagster_pandas.egg-info/SOURCES.txt
 dagster_pandas.egg-info/dependency_links.txt
 dagster_pandas.egg-info/requires.txt
 dagster_pandas.egg-info/top_level.txt
 dagster_pandas/examples/__init__.py
 dagster_pandas/examples/pandas_hello_world.yaml
-dagster_pandas/examples/repository.yaml
+dagster_pandas/examples/workspace.yaml
 dagster_pandas/examples/pandas_hello_world/__init__.py
 dagster_pandas/examples/pandas_hello_world/env.yaml
-dagster_pandas/examples/pandas_hello_world/pipeline.py
+dagster_pandas/examples/pandas_hello_world/ops.py
 dagster_pandas/examples/pandas_hello_world/solids.yaml
 dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_prod.yaml
 dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_test.yaml
 dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_prod.yaml
-dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
-dagster_pandas_tests/pandas_hello_world/__init__.py
-dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py
+dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
```

### Comparing `dagster-pandas-0.9.9rc1/setup.py` & `dagster-pandas-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import os
+from typing import Dict
 
 from setuptools import find_packages, setup
 
 
-def long_description():
+def long_description() -> str:
     here = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(here, "README.md"), "r") as fh:
+    with open(os.path.join(here, "README.md"), "r", encoding="utf8") as fh:
         return fh.read()
 
 
-def get_version():
-    version = {}
-    with open("dagster_pandas/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_pandas/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-pandas",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description=(
             "Utilities and examples for working with pandas and dagster, an opinionated "
             "framework for expressing data pipelines"
         ),
         long_description=long_description(),
         long_description_content_type="text/markdown",
         url="https://github.com/dagster-io/dagster",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["dagster_pandas_tests"]),
+        packages=find_packages(exclude=["dagster_pandas_tests*"]),
         include_package_data=True,
-        install_requires=["dagster", "pandas", "matplotlib"],
+        install_requires=["dagster==1.0.5", "pandas"],
     )
```

