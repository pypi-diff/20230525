# Comparing `tmp/dagster-airbyte-0.19.6.tar.gz` & `tmp/dagster-airbyte-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.19.6.tar", last modified: Thu May 25 17:25:25 2023, max compression
+gzip compressed data, was "dagster-airbyte-1.0.5.tar", last modified: Fri Aug 26 13:45:14 2022, max compression
```

## Comparing `dagster-airbyte-0.19.6.tar` & `dagster-airbyte-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:25.801717 dagster-airbyte-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-25 17:25:25.801717 dagster-airbyte-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:25.793717 dagster-airbyte-0.19.6/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43942 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:25.797717 dagster-airbyte-0.19.6/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:25.801717 dagster-airbyte-0.19.6/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14161 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    26443 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2633 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:25:25.793717 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:25:25.000000 dagster-airbyte-0.19.6/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-25 17:25:25.801717 dagster-airbyte-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-25 17:16:50.000000 dagster-airbyte-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      596 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)      467 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9354 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      596 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       24 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/setup.py
```

### Comparing `dagster-airbyte-0.19.6/LICENSE` & `dagster-airbyte-1.0.5/LICENSE`

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

### Comparing `dagster-airbyte-0.19.6/PKG-INFO` & `dagster-airbyte-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
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
-Provides-Extra: test
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-airbyte-0.19.6/dagster_airbyte/ops.py` & `dagster-airbyte-1.0.5/dagster_airbyte/ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,106 @@
-from typing import Any, Iterable, List, Optional
-
-from dagster import Config, In, Nothing, Out, Output, op
-from pydantic import Field
-
+from dagster_airbyte.resources import DEFAULT_POLL_INTERVAL_SECONDS
 from dagster_airbyte.types import AirbyteOutput
-from dagster_airbyte.utils import _get_attempt, generate_materializations
-
-from .resources import DEFAULT_POLL_INTERVAL_SECONDS, BaseAirbyteResource
+from dagster_airbyte.utils import generate_materializations
 
-
-class AirbyteSyncConfig(Config):
-    connection_id: str = Field(
-        ...,
-        description=(
-            "Parsed json dictionary representing the details of the Airbyte connector after the"
-            " sync successfully completes. See the [Airbyte API"
-            " Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview)"
-            " to see detailed information on this response."
-        ),
-    )
-    poll_interval: float = Field(
-        DEFAULT_POLL_INTERVAL_SECONDS,
-        description=(
-            "The maximum time that will waited before this operation is timed out. By "
-            "default, this will never time out."
-        ),
-    )
-    poll_timeout: Optional[float] = Field(
-        None,
-        description=(
-            "The maximum time that will waited before this operation is timed out. By "
-            "default, this will never time out."
-        ),
-    )
-    yield_materializations: bool = Field(
-        True,
-        description=(
-            "If True, materializations corresponding to the results of the Airbyte sync will "
-            "be yielded when the op executes."
-        ),
-    )
-    asset_key_prefix: List[str] = Field(
-        ["airbyte"],
-        description=(
-            "If provided and yield_materializations is True, these components will be used to "
-            "prefix the generated asset keys."
-        ),
-    )
+from dagster import Array, Bool, Field, In, Noneable, Nothing, Out, Output, op
 
 
 @op(
+    required_resource_keys={"airbyte"},
     ins={"start_after": In(Nothing)},
     out=Out(
         AirbyteOutput,
-        description=(
-            "Parsed json dictionary representing the details of the Airbyte connector after the"
-            " sync successfully completes. See the [Airbyte API"
-            " Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview)"
-            " to see detailed information on this response."
-        ),
+        description="Parsed json dictionary representing the details of the Airbyte connector after "
+        "the sync successfully completes. "
+        "See the [Airbyte API Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview) "
+        "to see detailed information on this response.",
     ),
+    config_schema={
+        "connection_id": Field(
+            str,
+            is_required=True,
+            description="The Airbyte Connection ID that this op will sync. You can retrieve this "
+            'value from the "Connections" tab of a given connector in the Airbyte UI.',
+        ),
+        "poll_interval": Field(
+            float,
+            default_value=DEFAULT_POLL_INTERVAL_SECONDS,
+            description="The time (in seconds) that will be waited between successive polls.",
+        ),
+        "poll_timeout": Field(
+            Noneable(float),
+            default_value=None,
+            description="The maximum time that will waited before this operation is timed out. By "
+            "default, this will never time out.",
+        ),
+        "yield_materializations": Field(
+            config=Bool,
+            default_value=True,
+            description=(
+                "If True, materializations corresponding to the results of the Airbyte sync will "
+                "be yielded when the op executes."
+            ),
+        ),
+        "asset_key_prefix": Field(
+            config=Array(str),
+            default_value=["airbyte"],
+            description=(
+                "If provided and yield_materializations is True, these components will be used to "
+                "prefix the generated asset keys."
+            ),
+        ),
+    },
     tags={"kind": "airbyte"},
 )
-def airbyte_sync_op(
-    context, config: AirbyteSyncConfig, airbyte: BaseAirbyteResource
-) -> Iterable[Any]:
-    """Executes a Airbyte job sync for a given ``connection_id``, and polls until that sync
+def airbyte_sync_op(context):
+    """
+    Executes a Airbyte job sync for a given ``connection_id``, and polls until that sync
     completes, raising an error if it is unsuccessful. It outputs a AirbyteOutput which contains
     the job details for a given ``connection_id``.
 
     It requires the use of the :py:class:`~dagster_airbyte.airbyte_resource`, which allows it to
     communicate with the Airbyte API.
 
     Examples:
-        .. code-block:: python
 
-            from dagster import job
-            from dagster_airbyte import airbyte_resource, airbyte_sync_op
+    .. code-block:: python
 
-            my_airbyte_resource = airbyte_resource.configured(
-                {
-                    "host": {"env": "AIRBYTE_HOST"},
-                    "port": {"env": "AIRBYTE_PORT"},
-                }
-            )
-
-            sync_foobar = airbyte_sync_op.configured({"connection_id": "foobar"}, name="sync_foobar")
-
-            @job(resource_defs={"airbyte": my_airbyte_resource})
-            def my_simple_airbyte_job():
-                sync_foobar()
-
-            @job(resource_defs={"airbyte": my_airbyte_resource})
-            def my_composed_airbyte_job():
-                final_foobar_state = sync_foobar(start_after=some_op())
-                other_op(final_foobar_state)
+        from dagster import job
+        from dagster_airbyte import airbyte_resource, airbyte_sync_op
+
+        my_airbyte_resource = airbyte_resource.configured(
+            {
+                "host": {"env": "AIRBYTE_HOST"},
+                "port": {"env": "AIRBYTE_PORT"},
+            }
+        )
+
+        sync_foobar = airbyte_sync_op.configured({"connection_id": "foobar"}, name="sync_foobar")
+
+        @job(resource_defs={"airbyte": my_airbyte_resource})
+        def my_simple_airbyte_job():
+            sync_foobar()
+
+        @job(resource_defs={"airbyte": my_airbyte_resource})
+        def my_composed_airbyte_job():
+            final_foobar_state = sync_foobar(start_after=some_op())
+            other_op(final_foobar_state)
     """
-    airbyte_output = airbyte.sync_and_poll(
-        connection_id=config.connection_id,
-        poll_interval=config.poll_interval,
-        poll_timeout=config.poll_timeout,
+
+    airbyte_output = context.resources.airbyte.sync_and_poll(
+        connection_id=context.op_config["connection_id"],
+        poll_interval=context.op_config["poll_interval"],
+        poll_timeout=context.op_config["poll_timeout"],
     )
-    if config.yield_materializations:
+    if context.op_config["yield_materializations"]:
         yield from generate_materializations(
-            airbyte_output, asset_key_prefix=config.asset_key_prefix
+            airbyte_output, asset_key_prefix=context.op_config["asset_key_prefix"]
         )
     yield Output(
         airbyte_output,
         metadata={
-            **_get_attempt(airbyte_output.job_details.get("attempts", [{}])[-1]).get(
-                "totalStats", {}
-            )
+            **airbyte_output.job_details.get("attempts", [{}])[-1]
+            .get("attempt", {})
+            .get("totalStats", {})
         },
     )
```

### Comparing `dagster-airbyte-0.19.6/dagster_airbyte/utils.py` & `dagster-airbyte-1.0.5/dagster_airbyte/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,40 @@
-from typing import Any, Iterator, Mapping, Sequence
-
-from dagster import AssetMaterialization, MetadataValue
-from dagster._core.definitions.metadata.table import TableColumn, TableSchema
+from typing import Any, Dict, Iterator, List
 
 from dagster_airbyte.types import AirbyteOutput
 
-
-def generate_table_schema(stream_schema_props: Mapping[str, Any]) -> TableSchema:
-    return TableSchema(
-        columns=sorted(
-            [
-                TableColumn(name=name, type=str(info.get("type", "unknown")))
-                for name, info in stream_schema_props.items()
-            ],
-            key=lambda col: col.name,
-        )
-    )
-
-
-def is_basic_normalization_operation(operation_def: Mapping[str, Any]) -> bool:
-    return (
-        operation_def.get("operatorType", operation_def.get("operator_type")) == "normalization"
-        and operation_def.get("normalization", {}).get("option") == "basic"
-    )
+from dagster import AssetMaterialization, MetadataValue
+from dagster._core.definitions.metadata.table import TableColumn, TableSchema
 
 
 def _materialization_for_stream(
     name: str,
-    stream_schema_props: Mapping[str, Any],
-    stream_stats: Mapping[str, Any],
-    asset_key_prefix: Sequence[str],
+    stream_schema_props: Dict[str, Any],
+    stream_stats: Dict[str, Any],
+    asset_key_prefix: List[str],
 ) -> AssetMaterialization:
+
     return AssetMaterialization(
-        asset_key=[*asset_key_prefix, name],
+        asset_key=asset_key_prefix + [name],
         metadata={
-            "schema": MetadataValue.table_schema(generate_table_schema(stream_schema_props)),
+            "schema": MetadataValue.table_schema(
+                TableSchema(
+                    columns=[
+                        TableColumn(name=name, type=str(info.get("type", "unknown")))
+                        for name, info in stream_schema_props.items()
+                    ]
+                )
+            ),
             **{k: v for k, v in stream_stats.items() if v is not None},
         },
     )
 
 
-def _get_attempt(attempt: dict):
-    # the attempt field is nested in some API results, and is not in others
-    return attempt.get("attempt") or attempt
-
-
 def generate_materializations(
-    output: AirbyteOutput, asset_key_prefix: Sequence[str]
+    output: AirbyteOutput, asset_key_prefix: List[str]
 ) -> Iterator[AssetMaterialization]:
     prefix = output.connection_details.get("prefix") or ""
     # all the streams that are set to be sync'd by this connection
     all_stream_props = {
         prefix
         + stream["stream"]["name"]: stream.get("stream", {})
         .get("jsonSchema", {})
@@ -58,15 +42,17 @@
         for stream in output.connection_details.get("syncCatalog", {}).get("streams", [])
         if stream.get("config", {}).get("selected")
     }
 
     # stats for each stream that had data sync'd
     all_stream_stats = {
         s["streamName"]: s.get("stats", {})
-        for s in _get_attempt(output.job_details.get("attempts", [{}])[-1]).get("streamStats", [])
+        for s in output.job_details.get("attempts", [{}])[-1]
+        .get("attempt", {})
+        .get("streamStats", [])
     }
     for stream_name, stream_props in all_stream_props.items():
         yield _materialization_for_stream(
             stream_name,
             stream_props,
             # if no records are sync'd, no stats will be avaiable for this stream
             all_stream_stats.get(stream_name, {}),
```

### Comparing `dagster-airbyte-0.19.6/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-1.0.5/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
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
-Provides-Extra: test
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-airbyte-0.19.6/setup.py` & `dagster-airbyte-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,39 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_airbyte/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_airbyte/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-airbyte",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for integrating Airbyte with Dagster.",
-    url=(
-        "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte"
-    ),
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_airbyte_tests*"]),
-    install_requires=[
-        "dagster==1.3.6",
-        "requests",
-    ],
-    zip_safe=False,
-    entry_points={
-        "console_scripts": [
-            "dagster-airbyte = dagster_airbyte.cli:main",
-        ]
-    },
-    extras_require={
-        "test": [
-            "requests-mock",
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-airbyte",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for integrating Airbyte with Dagster.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
         ],
-        "managed": [
-            "dagster-managed-elements==0.19.6",
+        packages=find_packages(exclude=["dagster_airbyte_tests*"]),
+        install_requires=[
+            "dagster==1.0.5",
+            "requests",
         ],
-    },
-)
+        zip_safe=False,
+    )
```

