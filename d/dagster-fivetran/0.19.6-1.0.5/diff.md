# Comparing `tmp/dagster-fivetran-0.19.6.tar.gz` & `tmp/dagster-fivetran-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-fivetran-0.19.6.tar", last modified: Thu May 25 17:27:12 2023, max compression
+gzip compressed data, was "dagster-fivetran-1.0.5.tar", last modified: Fri Aug 26 13:45:23 2022, max compression
```

## Comparing `dagster-fivetran-0.19.6.tar` & `dagster-fivetran-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:12.122236 dagster-fivetran-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-25 17:27:12.122236 dagster-fivetran-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:12.122236 dagster-fivetran-0.19.6/dagster_fivetran/
--rw-r--r--   0 root         (0) root         (0)      854 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20553 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:12.122236 dagster-fivetran-0.19.6/dagster_fivetran/managed/
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/managed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14474 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     7139 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/py.typed
--rw-r--r--   0 root         (0) root         (0)    18113 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/resources.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/types.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/dagster_fivetran/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:27:12.122236 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-25 17:27:12.000000 dagster-fivetran-0.19.6/dagster_fivetran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-25 17:27:12.126236 dagster-fivetran-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1491 2023-05-25 17:16:50.000000 dagster-fivetran-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:23.836434 dagster-fivetran-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      650 2022-08-26 13:45:23.836434 dagster-fivetran-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:23.836434 dagster-fivetran-1.0.5/dagster_fivetran/
+-rw-r--r--   0 root         (0) root         (0)      489 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8469 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18395 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/resources.py
+-rw-r--r--   0 root         (0) root         (0)      932 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/types.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/dagster_fivetran/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:23.836434 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      650 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-08-26 13:45:23.000000 dagster-fivetran-1.0.5/dagster_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2022-08-26 13:45:23.836434 dagster-fivetran-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1301 2022-08-26 13:33:01.000000 dagster-fivetran-1.0.5/setup.py
```

### Comparing `dagster-fivetran-0.19.6/LICENSE` & `dagster-fivetran-1.0.5/LICENSE`

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

### Comparing `dagster-fivetran-0.19.6/PKG-INFO` & `dagster-fivetran-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-fivetran-0.19.6/dagster_fivetran/ops.py` & `dagster-fivetran-1.0.5/dagster_fivetran/ops.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,174 @@
-from typing import Any, Dict, List, Optional
-
-from dagster import (
-    AssetKey,
-    Config,
-    In,
-    Nothing,
-    Out,
-    Output,
-    op,
-)
-from pydantic import Field
-
-from dagster_fivetran.resources import DEFAULT_POLL_INTERVAL, FivetranResource
+from dagster_fivetran.resources import DEFAULT_POLL_INTERVAL
 from dagster_fivetran.types import FivetranOutput
 from dagster_fivetran.utils import generate_materializations
 
-
-class SyncConfig(Config):
-    connector_id: str = Field(
-        description=(
-            "The Fivetran Connector ID that this op will sync. You can retrieve this "
-            'value from the "Setup" tab of a given connector in the Fivetran UI.'
-        ),
-    )
-    poll_interval: float = Field(
-        default=DEFAULT_POLL_INTERVAL,
-        description="The time (in seconds) that will be waited between successive polls.",
-    )
-    poll_timeout: Optional[float] = Field(
-        default=None,
-        description=(
-            "The maximum time that will waited before this operation is timed out. By "
-            "default, this will never time out."
-        ),
-    )
-    yield_materializations: bool = Field(
-        default=True,
-        description=(
-            "If True, materializations corresponding to the results of the Fivetran sync will "
-            "be yielded when the op executes."
-        ),
-    )
-    asset_key_prefix: List[str] = Field(
-        default=["fivetran"],
-        description=(
-            "If provided and yield_materializations is True, these components will be used to "
-            "prefix the generated asset keys."
-        ),
-    )
+from dagster import Array, AssetKey, Bool, Field, In, Noneable, Nothing, Out, Output, Permissive, op
 
 
 @op(
+    required_resource_keys={"fivetran"},
     ins={"start_after": In(Nothing)},
     out=Out(
         FivetranOutput,
-        description=(
-            "Parsed json dictionary representing the details of the Fivetran connector after the"
-            " sync successfully completes. See the [Fivetran API"
-            " Docs](https://fivetran.com/docs/rest-api/connectors#retrieveconnectordetails) to see"
-            " detailed information on this response."
-        ),
+        description="Parsed json dictionary representing the details of the Fivetran connector after "
+        "the sync successfully completes. "
+        "See the [Fivetran API Docs](https://fivetran.com/docs/rest-api/connectors#retrieveconnectordetails) "
+        "to see detailed information on this response.",
     ),
+    config_schema={
+        "connector_id": Field(
+            str,
+            is_required=True,
+            description="The Fivetran Connector ID that this op will sync. You can retrieve this "
+            'value from the "Setup" tab of a given connector in the Fivetran UI.',
+        ),
+        "poll_interval": Field(
+            float,
+            default_value=DEFAULT_POLL_INTERVAL,
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
+                "If True, materializations corresponding to the results of the Fivetran sync will "
+                "be yielded when the op executes."
+            ),
+        ),
+        "asset_key_prefix": Field(
+            config=Array(str),
+            default_value=["fivetran"],
+            description=(
+                "If provided and yield_materializations is True, these components will be used to "
+                "prefix the generated asset keys."
+            ),
+        ),
+    },
     tags={"kind": "fivetran"},
 )
-def fivetran_sync_op(config: SyncConfig, fivetran: FivetranResource) -> Any:
-    """Executes a Fivetran sync for a given ``connector_id``, and polls until that sync
+def fivetran_sync_op(context):
+    """
+    Executes a Fivetran sync for a given ``connector_id``, and polls until that sync
     completes, raising an error if it is unsuccessful. It outputs a FivetranOutput which contains
     the details of the Fivetran connector after the sync successfully completes, as well as details
     about which tables the sync updates.
 
     It requires the use of the :py:class:`~dagster_fivetran.fivetran_resource`, which allows it to
     communicate with the Fivetran API.
 
     Examples:
-        .. code-block:: python
 
-            from dagster import job
-            from dagster_fivetran import fivetran_resource, fivetran_sync_op
+    .. code-block:: python
 
-            my_fivetran_resource = fivetran_resource.configured(
-                {
-                    "api_key": {"env": "FIVETRAN_API_KEY"},
-                    "api_secret": {"env": "FIVETRAN_API_SECRET"},
-                }
-            )
+        from dagster import job
+        from dagster_fivetran import fivetran_resource, fivetran_sync_op
+
+        my_fivetran_resource = fivetran_resource.configured(
+            {
+                "api_key": {"env": "FIVETRAN_API_KEY"},
+                "api_secret": {"env": "FIVETRAN_API_SECRET"},
+            }
+        )
 
-            sync_foobar = fivetran_sync_op.configured({"connector_id": "foobar"}, name="sync_foobar")
+        sync_foobar = fivetran_sync_op.configured({"connector_id": "foobar"}, name="sync_foobar")
+
+        @job(resource_defs={"fivetran": my_fivetran_resource})
+        def my_simple_fivetran_job():
+            sync_foobar()
 
-            @job(resource_defs={"fivetran": my_fivetran_resource})
-            def my_simple_fivetran_job():
-                sync_foobar()
-
-            @job(resource_defs={"fivetran": my_fivetran_resource})
-            def my_composed_fivetran_job():
-                final_foobar_state = sync_foobar(start_after=some_op())
-                other_op(final_foobar_state)
+        @job(resource_defs={"fivetran": my_fivetran_resource})
+        def my_composed_fivetran_job():
+            final_foobar_state = sync_foobar(start_after=some_op())
+            other_op(final_foobar_state)
     """
-    fivetran_output = fivetran.sync_and_poll(
-        connector_id=config.connector_id,
-        poll_interval=config.poll_interval,
-        poll_timeout=config.poll_timeout,
+
+    fivetran_output = context.resources.fivetran.sync_and_poll(
+        connector_id=context.op_config["connector_id"],
+        poll_interval=context.op_config["poll_interval"],
+        poll_timeout=context.op_config["poll_timeout"],
     )
-    if config.yield_materializations:
+    if context.op_config["yield_materializations"]:
         yield from generate_materializations(
-            fivetran_output, asset_key_prefix=config.asset_key_prefix
+            fivetran_output, asset_key_prefix=context.op_config["asset_key_prefix"]
         )
     yield Output(fivetran_output)
 
 
-class FivetranResyncConfig(SyncConfig):
-    resync_parameters: Optional[Dict[str, Any]] = Field(
-        None,
-        description=(
-            "Optional resync parameters to send in the payload to the Fivetran API. You can"
-            " find an example resync payload here:"
-            " https://fivetran.com/docs/rest-api/connectors#request_7"
-        ),
-    )
-
-
 @op(
+    required_resource_keys={"fivetran"},
     ins={"start_after": In(Nothing)},
     out=Out(
         FivetranOutput,
-        description=(
-            "Parsed json dictionary representing the details of the Fivetran connector after the"
-            " resync successfully completes. See the [Fivetran API"
-            " Docs](https://fivetran.com/docs/rest-api/connectors#retrieveconnectordetails) to see"
-            " detailed information on this response."
-        ),
+        description="Parsed json dictionary representing the details of the Fivetran connector after "
+        "the resync successfully completes. "
+        "See the [Fivetran API Docs](https://fivetran.com/docs/rest-api/connectors#retrieveconnectordetails) "
+        "to see detailed information on this response.",
     ),
+    config_schema={
+        "connector_id": Field(
+            str,
+            is_required=True,
+            description="The Fivetran Connector ID that this op will sync. You can retrieve this "
+            'value from the "Setup" tab of a given connector in the Fivetran UI.',
+        ),
+        "resync_parameters": Field(
+            Permissive(),
+            is_required=True,
+            description="The resync parameters to send in the payload to the Fivetran API. You "
+            "can find an example resync payload here: https://fivetran.com/docs/rest-api/connectors#request_6",
+        ),
+        "poll_interval": Field(
+            float,
+            default_value=DEFAULT_POLL_INTERVAL,
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
+                "If True, materializations corresponding to the results of the Fivetran sync will "
+                "be yielded when the op executes."
+            ),
+        ),
+        "asset_key_prefix": Field(
+            config=Array(str),
+            default_value=["fivetran"],
+            description=(
+                "If provided and yield_materializations is True, these components will be used to "
+                "prefix the generated asset keys."
+            ),
+        ),
+    },
     tags={"kind": "fivetran"},
 )
-def fivetran_resync_op(
-    config: FivetranResyncConfig,
-    fivetran: FivetranResource,
-) -> Any:
-    """Executes a Fivetran historical resync for a given ``connector_id``, and polls until that resync
+def fivetran_resync_op(context):
+    """
+    Executes a Fivetran historical resync for a given ``connector_id``, and polls until that resync
     completes, raising an error if it is unsuccessful. It outputs a FivetranOutput which contains
     the details of the Fivetran connector after the resync successfully completes, as well as details
     about which tables the resync updates.
 
     It requires the use of the :py:class:`~dagster_fivetran.fivetran_resource`, which allows it to
     communicate with the Fivetran API.
 
     Examples:
+
     .. code-block:: python
 
         from dagster import job
         from dagster_fivetran import fivetran_resource, fivetran_resync_op
 
         my_fivetran_resource = fivetran_resource.configured(
             {
@@ -173,30 +193,27 @@
             sync_foobar()
 
         @job(resource_defs={"fivetran": my_fivetran_resource})
         def my_composed_fivetran_job():
             final_foobar_state = sync_foobar(start_after=some_op())
             other_op(final_foobar_state)
     """
-    fivetran_output = fivetran.resync_and_poll(
-        connector_id=config.connector_id,
-        resync_parameters=config.resync_parameters,
-        poll_interval=config.poll_interval,
-        poll_timeout=config.poll_timeout,
-    )
-    if config.yield_materializations:
-        asset_key_filter = (
-            [
-                AssetKey(config.asset_key_prefix + [schema, table])
-                for schema, tables in config.resync_parameters.items()
-                for table in tables
-            ]
-            if config.resync_parameters is not None
-            else None
-        )
+
+    fivetran_output = context.resources.fivetran.resync_and_poll(
+        connector_id=context.op_config["connector_id"],
+        resync_parameters=context.op_config["resync_parameters"],
+        poll_interval=context.op_config["poll_interval"],
+        poll_timeout=context.op_config["poll_timeout"],
+    )
+    if context.op_config["yield_materializations"]:
+        asset_key_filter = [
+            AssetKey(context.op_config["asset_key_prefix"] + [schema, table])
+            for schema, tables in context.op_config["resync_parameters"].items()
+            for table in tables
+        ]
         for mat in generate_materializations(
-            fivetran_output, asset_key_prefix=config.asset_key_prefix
+            fivetran_output, asset_key_prefix=context.op_config["asset_key_prefix"]
         ):
-            if asset_key_filter is None or mat.asset_key in asset_key_filter:
+            if mat.asset_key in asset_key_filter:
                 yield mat
 
     yield Output(fivetran_output)
```

### Comparing `dagster-fivetran-0.19.6/dagster_fivetran/resources.py` & `dagster-fivetran-1.0.5/dagster_fivetran/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,157 +1,131 @@
 import datetime
 import json
 import logging
 import time
-from typing import Any, Mapping, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
 
 import requests
-from dagster import (
-    Failure,
-    InitResourceContext,
-    MetadataValue,
-    __version__,
-    _check as check,
-    get_dagster_logger,
-    resource,
-)
-from dagster._config.pythonic_config import ConfigurableResource
-from dagster._utils.cached_method import cached_method
+from dagster_fivetran.types import FivetranOutput
+from dagster_fivetran.utils import get_fivetran_connector_url, get_fivetran_logs_url
 from dateutil import parser
-from pydantic import Field
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import RequestException
 
-from dagster_fivetran.types import FivetranOutput
-from dagster_fivetran.utils import get_fivetran_connector_url, get_fivetran_logs_url
+from dagster import Failure, Field, MetadataValue, StringSource, __version__
+from dagster import _check as check
+from dagster import get_dagster_logger, resource
 
 FIVETRAN_API_BASE = "https://api.fivetran.com"
-FIVETRAN_API_VERSION_PATH = "v1/"
-FIVETRAN_CONNECTOR_PATH = "connectors/"
+FIVETRAN_CONNECTOR_PATH = "v1/connectors/"
 
 # default polling interval (in seconds)
 DEFAULT_POLL_INTERVAL = 10
 
 
-class FivetranResource(ConfigurableResource):
-    """This class exposes methods on top of the Fivetran REST API."""
+class FivetranResource:
+    """
+    This class exposes methods on top of the Fivetran REST API.
+    """
 
-    api_key: str = Field(description="The Fivetran API key to use for this resource.")
-    api_secret: str = Field(description="The Fivetran API secret to use for this resource.")
-    disable_schedule_on_trigger: bool = Field(
-        default=True,
-        description=(
-            "Specifies if you would like any connector that is sync'd using this "
-            "resource to be automatically taken off its Fivetran schedule."
-        ),
-    )
-    request_max_retries: int = Field(
-        default=3,
-        description=(
-            "The maximum number of times requests to the Fivetran API should be retried "
-            "before failing."
-        ),
-    )
-    request_retry_delay: float = Field(
-        default=0.25,
-        description="Time (in seconds) to wait between each request retry.",
-    )
+    def __init__(
+        self,
+        api_key: str,
+        api_secret: str,
+        disable_schedule_on_trigger: bool = True,
+        request_max_retries: int = 3,
+        request_retry_delay: float = 0.25,
+        log: logging.Logger = get_dagster_logger(),
+    ):
+        self._auth = HTTPBasicAuth(api_key, api_secret)
+        self._disable_schedule_on_trigger = disable_schedule_on_trigger
 
-    @property
-    def _auth(self) -> HTTPBasicAuth:
-        return HTTPBasicAuth(self.api_key, self.api_secret)
+        self._request_max_retries = request_max_retries
+        self._request_retry_delay = request_retry_delay
 
-    @property
-    @cached_method
-    def _log(self) -> logging.Logger:
-        return get_dagster_logger()
+        self._log = log
 
     @property
     def api_base_url(self) -> str:
-        return urljoin(FIVETRAN_API_BASE, FIVETRAN_API_VERSION_PATH)
-
-    @property
-    def api_connector_url(self) -> str:
-        return urljoin(self.api_base_url, FIVETRAN_CONNECTOR_PATH)
-
-    def make_connector_request(
-        self, method: str, endpoint: str, data: Optional[str] = None
-    ) -> Mapping[str, Any]:
-        return self.make_request(method, urljoin(FIVETRAN_CONNECTOR_PATH, endpoint), data)
+        return urljoin(FIVETRAN_API_BASE, FIVETRAN_CONNECTOR_PATH)
 
     def make_request(
         self, method: str, endpoint: str, data: Optional[str] = None
-    ) -> Mapping[str, Any]:
-        """Creates and sends a request to the desired Fivetran Connector API endpoint.
+    ) -> Dict[str, Any]:
+        """
+        Creates and sends a request to the desired Fivetran Connector API endpoint.
 
         Args:
             method (str): The http method to use for this request (e.g. "POST", "GET", "PATCH").
             endpoint (str): The Fivetran API endpoint to send this request to.
             data (Optional[str]): JSON-formatted data string to be included in the request.
 
         Returns:
             Dict[str, Any]: Parsed json data from the response to this request
         """
-        url = urljoin(self.api_base_url, endpoint)
+
         headers = {
             "User-Agent": f"dagster-fivetran/{__version__}",
             "Content-Type": "application/json;version=2",
         }
 
         num_retries = 0
         while True:
             try:
                 response = requests.request(
                     method=method,
-                    url=url,
+                    url=urljoin(self.api_base_url, endpoint),
                     headers=headers,
                     auth=self._auth,
                     data=data,
                 )
                 response.raise_for_status()
                 resp_dict = response.json()
                 return resp_dict["data"] if "data" in resp_dict else resp_dict
             except RequestException as e:
                 self._log.error("Request to Fivetran API failed: %s", e)
-                if num_retries == self.request_max_retries:
+                if num_retries == self._request_max_retries:
                     break
                 num_retries += 1
-                time.sleep(self.request_retry_delay)
+                time.sleep(self._request_retry_delay)
 
-        raise Failure(f"Max retries ({self.request_max_retries}) exceeded with url: {url}.")
+        raise Failure("Exceeded max number of retries.")
 
-    def get_connector_details(self, connector_id: str) -> Mapping[str, Any]:
-        """Gets details about a given connector from the Fivetran Connector API.
+    def get_connector_details(self, connector_id: str) -> Dict[str, Any]:
+        """
+        Gets details about a given connector from the Fivetran Connector API.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
 
         Returns:
             Dict[str, Any]: Parsed json data from the response to this request
         """
-        return self.make_connector_request(method="GET", endpoint=connector_id)
+        return self.make_request(method="GET", endpoint=connector_id)
 
     def _assert_syncable_connector(self, connector_id: str):
-        """Confirms that a given connector is eligible to sync. Will raise a Failure in the event that
+        """
+        Confirms that a given connector is eligible to sync. Will raise a Failure in the event that
         the connector is either paused or not fully setup.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
         """
         connector_details = self.get_connector_details(connector_id)
         if connector_details["paused"]:
             raise Failure(f"Connector '{connector_id}' cannot be synced as it is currently paused.")
         if connector_details["status"]["setup_state"] != "connected":
             raise Failure(f"Connector '{connector_id}' cannot be synced as it has not been setup")
 
     def get_connector_sync_status(self, connector_id: str) -> Tuple[datetime.datetime, bool, str]:
-        """Gets details about the status of the most recent Fivetran sync operation for a given
+        """
+        Gets details about the status of the most recent Fivetran sync operation for a given
         connector.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
 
         Returns:
@@ -168,117 +142,117 @@
         return (
             max(succeeded_at, failed_at),
             succeeded_at > failed_at,
             connector_details["status"]["sync_state"],
         )
 
     def update_connector(
-        self, connector_id: str, properties: Optional[Mapping[str, Any]] = None
-    ) -> Mapping[str, Any]:
-        """Updates properties of a Fivetran Connector.
+        self, connector_id: str, properties: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """
+        Updates properties of a Fivetran Connector.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
             properties (Dict[str, Any]): The properties to be updated. For a comprehensive list of
                 properties, see the [Fivetran docs](https://fivetran.com/docs/rest-api/connectors#modifyaconnector).
 
         Returns:
             Dict[str, Any]: Parsed json data representing the API response.
         """
-        return self.make_connector_request(
-            method="PATCH", endpoint=connector_id, data=json.dumps(properties)
-        )
+        return self.make_request(method="PATCH", endpoint=connector_id, data=json.dumps(properties))
 
     def update_schedule_type(
         self, connector_id: str, schedule_type: Optional[str] = None
-    ) -> Mapping[str, Any]:
-        """Updates the schedule type property of the connector to either "auto" or "manual".
+    ) -> Dict[str, Any]:
+        """
+        Updates the schedule type property of the connector to either "auto" or "manual".
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
             schedule_type (Optional[str]): Either "auto" (to turn the schedule on) or "manual" (to
                 turn it off).
 
         Returns:
             Dict[str, Any]: Parsed json data representing the API response.
         """
         if schedule_type not in ["auto", "manual"]:
             check.failed(f"schedule_type must be either 'auto' or 'manual': got '{schedule_type}'")
         return self.update_connector(connector_id, properties={"schedule_type": schedule_type})
 
-    def get_connector_schema_config(self, connector_id: str) -> Mapping[str, Any]:
-        return self.make_connector_request("GET", endpoint=f"{connector_id}/schemas")
+    def get_connector_schema_config(self, connector_id: str) -> Dict[str, Any]:
+        return self.make_request("GET", endpoint=f"{connector_id}/schemas")
 
-    def start_sync(self, connector_id: str) -> Mapping[str, Any]:
-        """Initiates a sync of a Fivetran connector.
+    def start_sync(self, connector_id: str) -> Dict[str, Any]:
+        """
+        Initiates a sync of a Fivetran connector.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
 
         Returns:
             Dict[str, Any]: Parsed json data representing the connector details API response after
                 the sync is started.
         """
-        if self.disable_schedule_on_trigger:
+        if self._disable_schedule_on_trigger:
             self._log.info("Disabling Fivetran sync schedule.")
             self.update_schedule_type(connector_id, "manual")
         self._assert_syncable_connector(connector_id)
-        self.make_connector_request(method="POST", endpoint=f"{connector_id}/force")
+        self.make_request(method="POST", endpoint=f"{connector_id}/force")
         connector_details = self.get_connector_details(connector_id)
         self._log.info(
             f"Sync initialized for connector_id={connector_id}. View this sync in the Fivetran UI: "
             + get_fivetran_connector_url(connector_details)
         )
         return connector_details
 
     def start_resync(
-        self, connector_id: str, resync_parameters: Optional[Mapping[str, Sequence[str]]] = None
-    ) -> Mapping[str, Any]:
-        """Initiates a historical sync of all data for multiple schema tables within a Fivetran connector.
+        self, connector_id: str, resync_parameters: Dict[str, List[str]]
+    ) -> Dict[str, Any]:
+        """
+        Initiates a historical sync of all data for multiple schema tables within a Fivetran connector.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
-            resync_parameters (Optional[Dict[str, List[str]]]): Optional resync parameters to send to the Fivetran API.
-                An example payload can be found here: https://fivetran.com/docs/rest-api/connectors#request_7
+            resync_parameters (Dict[str, List[str]]): The resync parameters to send to the Fivetran API.
+                An example payload can be found here: https://fivetran.com/docs/rest-api/connectors#request_6
 
         Returns:
             Dict[str, Any]: Parsed json data representing the connector details API response after
                 the resync is started.
         """
-        if self.disable_schedule_on_trigger:
+        if self._disable_schedule_on_trigger:
             self._log.info("Disabling Fivetran sync schedule.")
             self.update_schedule_type(connector_id, "manual")
         self._assert_syncable_connector(connector_id)
-        self.make_connector_request(
+        self.make_request(
             method="POST",
-            endpoint=f"{connector_id}/schemas/tables/resync"
-            if resync_parameters is not None
-            else f"{connector_id}/resync",
-            data=json.dumps(resync_parameters) if resync_parameters is not None else None,
+            endpoint=f"{connector_id}/schemas/tables/resync",
+            data=json.dumps(resync_parameters),
         )
         connector_details = self.get_connector_details(connector_id)
         self._log.info(
-            f"Sync initialized for connector_id={connector_id}. View this resync in the Fivetran"
-            " UI: "
+            f"Sync initialized for connector_id={connector_id}. View this resync in the Fivetran UI: "
             + get_fivetran_connector_url(connector_details)
         )
         return connector_details
 
     def poll_sync(
         self,
         connector_id: str,
         initial_last_sync_completion: datetime.datetime,
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = None,
-    ) -> Mapping[str, Any]:
-        """Given a Fivetran connector and the timestamp at which the previous sync completed, poll
+    ) -> Dict[str, Any]:
+        """
+        Given a Fivetran connector and the timestamp at which the previous sync completed, poll
         until the next sync completes.
 
         The previous sync completion time is necessary because the only way to tell when a sync
         completes is when this value changes.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
@@ -328,15 +302,16 @@
 
     def sync_and_poll(
         self,
         connector_id: str,
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = None,
     ) -> FivetranOutput:
-        """Initializes a sync operation for the given connector, and polls until it completes.
+        """
+        Initializes a sync operation for the given connector, and polls until it completes.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
             poll_interval (float): The time (in seconds) that will be waited between successive polls.
             poll_timeout (float): The maximum time that will waited before this operation is timed
                 out. By default, this will never time out.
@@ -355,19 +330,20 @@
             poll_timeout=poll_timeout,
         )
         return FivetranOutput(connector_details=final_details, schema_config=schema_config)
 
     def resync_and_poll(
         self,
         connector_id: str,
+        resync_parameters: Dict[str, List[str]],
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = None,
-        resync_parameters: Optional[Mapping[str, Sequence[str]]] = None,
     ) -> FivetranOutput:
-        """Initializes a historical resync operation for the given connector, and polls until it completes.
+        """
+        Initializes a historical resync operation for the given connector, and polls until it completes.
 
         Args:
             connector_id (str): The Fivetran Connector ID. You can retrieve this value from the
                 "Setup" tab of a given connector in the Fivetran UI.
             resync_parameters (Dict[str, List[str]]): The payload to send to the Fivetran API.
                 This should be a dictionary with schema names as the keys and a list of tables
                 to resync as the values.
@@ -387,17 +363,51 @@
             init_last_sync_timestamp,
             poll_interval=poll_interval,
             poll_timeout=poll_timeout,
         )
         return FivetranOutput(connector_details=final_details, schema_config=schema_config)
 
 
-@resource(config_schema=FivetranResource.to_config_schema())
-def fivetran_resource(context: InitResourceContext) -> FivetranResource:
-    """This resource allows users to programatically interface with the Fivetran REST API to launch
+@resource(
+    config_schema={
+        "api_key": Field(
+            StringSource,
+            is_required=True,
+            description="Fivetran API Key. You can find this value on the Fivetran settings page: "
+            "https://fivetran.com/account/settings",
+        ),
+        "api_secret": Field(
+            StringSource,
+            is_required=True,
+            description="Fivetran API Secret. You can find this value on the Fivetran settings page: "
+            "https://fivetran.com/account/settings",
+        ),
+        "disable_schedule_on_trigger": Field(
+            bool,
+            default_value=True,
+            description="Specifies if you would like any connector that is sync'd using this "
+            "resource to be automatically taken off its Fivetran schedule.",
+        ),
+        "request_max_retries": Field(
+            int,
+            default_value=3,
+            description="The maximum number of times requests to the Fivetran API should be retried "
+            "before failing.",
+        ),
+        "request_retry_delay": Field(
+            float,
+            default_value=0.25,
+            description="Time (in seconds) to wait between each request retry.",
+        ),
+    },
+    description="This resource helps manage Fivetran connectors",
+)
+def fivetran_resource(context) -> FivetranResource:
+    """
+    This resource allows users to programatically interface with the Fivetran REST API to launch
     syncs and monitor their progress. This currently implements only a subset of the functionality
     exposed by the API.
 
     For a complete set of documentation on the Fivetran REST API, including expected response JSON
     schemae, see the `Fivetran API Docs <https://fivetran.com/docs/rest-api/connectors>`_.
 
     To configure this resource, we recommend using the `configured
@@ -418,8 +428,15 @@
         )
 
         @job(resource_defs={"fivetran":my_fivetran_resource})
         def my_fivetran_job():
             ...
 
     """
-    return FivetranResource.from_resource_context(context)
+    return FivetranResource(
+        api_key=context.resource_config["api_key"],
+        api_secret=context.resource_config["api_secret"],
+        disable_schedule_on_trigger=context.resource_config["disable_schedule_on_trigger"],
+        request_max_retries=context.resource_config["request_max_retries"],
+        request_retry_delay=context.resource_config["request_retry_delay"],
+        log=context.log,
+    )
```

### Comparing `dagster-fivetran-0.19.6/dagster_fivetran/types.py` & `dagster-fivetran-1.0.5/dagster_fivetran/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Any, Mapping, NamedTuple
+from typing import Any, Dict, NamedTuple
 
 
 class FivetranOutput(
     NamedTuple(
         "_FivetranOutput",
         [
-            ("connector_details", Mapping[str, Any]),
-            ("schema_config", Mapping[str, Any]),
+            ("connector_details", Dict[str, Any]),
+            ("schema_config", Dict[str, Any]),
         ],
     )
 ):
-    """Contains recorded information about the state of a Fivetran connector after a sync completes.
+    """
+    Contains recorded information about the state of a Fivetran connector after a sync completes.
 
     Attributes:
         connector_details (Dict[str, Any]):
             The raw Fivetran API response containing the details of the sync'd connector. For info
             on the schema of this dictionary, see: https://fivetran.com/docs/rest-api/connectors#retrieveconnectordetails
         schema_config (Dict[str, Any]):
             The raw Fivetran API response containing information about the tables created by the
```

### Comparing `dagster-fivetran-0.19.6/dagster_fivetran.egg-info/PKG-INFO` & `dagster-fivetran-1.0.5/dagster_fivetran.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-fivetran-0.19.6/setup.py` & `dagster-fivetran-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,37 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_fivetran/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_fivetran/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-fivetran",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for integrating Fivetran with Dagster.",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_fivetran_tests*"]),
-    install_requires=["dagster==1.3.6"],
-    zip_safe=False,
-    entry_points={
-        "console_scripts": [
-            "dagster-fivetran = dagster_fivetran.cli:main",
-        ]
-    },
-    extras_require={
-        "managed": [
-            "dagster-managed-elements==0.19.6",
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-fivetran",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for integrating Fivetran with Dagster.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
         ],
-    },
-)
+        packages=find_packages(exclude=["dagster_fivetran_tests*"]),
+        install_requires=["dagster==1.0.5"],
+        zip_safe=False,
+    )
```

