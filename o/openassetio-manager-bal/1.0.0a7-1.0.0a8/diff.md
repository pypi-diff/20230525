# Comparing `tmp/openassetio_manager_bal-1.0.0a7-py3-none-any.whl.zip` & `tmp/openassetio_manager_bal-1.0.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15644 bytes, number of entries: 9
--rw-r--r--  2.0 unx     9485 b- defN 23-May-09 15:12 openassetio_manager_bal/BasicAssetLibraryInterface.py
--rw-r--r--  2.0 unx     2977 b- defN 23-May-09 15:12 openassetio_manager_bal/__init__.py
--rw-r--r--  2.0 unx    10682 b- defN 23-May-09 15:12 openassetio_manager_bal/bal.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3745 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       80 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      880 b- defN 23-May-09 15:13 openassetio_manager_bal-1.0.0a7.dist-info/RECORD
-9 files, 39322 bytes uncompressed, 14088 bytes compressed:  64.2%
+Zip file size: 16277 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-25 16:18 openassetio_manager_bal/BasicAssetLibraryInterface.py
+-rw-r--r--  2.0 unx     2977 b- defN 23-May-25 16:18 openassetio_manager_bal/__init__.py
+-rw-r--r--  2.0 unx    11567 b- defN 23-May-25 16:18 openassetio_manager_bal/bal.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4016 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       80 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      881 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/RECORD
+9 files, 41300 bytes uncompressed, 14721 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: openassetio_manager_bal/__init__.py
 Comment: 
 
 Filename: openassetio_manager_bal/bal.py
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/LICENSE
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/METADATA
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/METADATA
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/WHEEL
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/entry_points.txt
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/top_level.txt
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a7.dist-info/RECORD
+Filename: openassetio_manager_bal-1.0.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openassetio_manager_bal/BasicAssetLibraryInterface.py

```diff
@@ -18,15 +18,17 @@
 # pylint: disable=invalid-name
 """
 A single-class module, providing the BasicAssetLibraryInterface class.
 """
 
 import itertools
 import os
+import time
 
+from functools import wraps
 from openassetio import constants, BatchElementError, EntityReference, TraitsData
 from openassetio.exceptions import MalformedEntityReference, PluginError
 from openassetio.managerApi import ManagerInterface
 
 from . import bal
 
 __all__ = [
@@ -39,14 +41,28 @@
 # fails for missing abstract methods.
 # pylint: disable=abstract-method
 # Methods in C++ end up with "missing docstring"
 # pylint: disable=missing-docstring
 # pylint: disable=too-many-arguments, unused-argument
 
 
+def simulated_delay(func):
+    @wraps(func)
+    def wrapper_simulated_delay(self, *args, **kwargs):
+        # pylint: disable=protected-access
+        delay_ms = self._BasicAssetLibraryInterface__settings.get(
+            bal.SETTINGS_KEY_SIMULATED_QUERY_LATENCY, 0
+        )
+        if delay_ms > 0:
+            time.sleep(delay_ms / 1000.0)  # sleep takes seconds
+        return func(self, *args, **kwargs)
+
+    return wrapper_simulated_delay
+
+
 class BasicAssetLibraryInterface(ManagerInterface):
     """
     This class exposes the Basic Asset Library through the OpenAssetIO
     ManagerInterface.
     """
 
     __reference_prefix = "bal:///"
@@ -95,35 +111,43 @@
         self.__library = {}
         hostSession.logger().log(
             hostSession.logger().Severity.kDebug,
             f"Loading library from '{library_path}'",
         )
         self.__library = bal.load_library(library_path)
 
+        hostSession.logger().log(
+            hostSession.logger().Severity.kDebug,
+            f"Running with simulated query latency of "
+            f"{self.__settings[bal.SETTINGS_KEY_SIMULATED_QUERY_LATENCY]}ms",
+        )
+
     def managementPolicy(self, traitSets, context, hostSession):
         access = "read" if context.isForRead() else "write"
         return [
             self.__dict_to_traits_data(bal.management_policy(trait_set, access, self.__library))
             for trait_set in traitSets
         ]
 
     def isEntityReferenceString(self, someString, hostSession):
         return someString.startswith(self.__reference_prefix)
 
+    @simulated_delay
     def entityExists(self, entityRefs, context, hostSession):
         results = []
         for ref in entityRefs:
             try:
                 entity_info = bal.parse_entity_ref(ref.toString())
                 result = bal.exists(entity_info, self.__library)
             except bal.MalformedBALReference as exc:
                 result = MalformedEntityReference(str(exc))
             results.append(result)
         return results
 
+    @simulated_delay
     def resolve(
         self, entityReferences, traitSet, context, hostSession, successCallback, errorCallback
     ):
         if context.isForWrite():
             result = BatchElementError(
                 BatchElementError.ErrorCode.kEntityAccessError, "BAL entities are read-only"
             )
@@ -153,14 +177,15 @@
                     for trait in traitSet:
                         trait_data = entity.traits.get(trait)
                         if trait_data is not None:
                             self.__add_trait_to_traits_data(trait, trait_data, result)
 
                     successCallback(idx, result)
 
+    @simulated_delay
     def preflight(
         self, targetEntityRefs, traitSet, context, hostSession, successCallback, errorCallback
     ):
         # Support publishing to any valid entity reference
         for idx, ref in enumerate(targetEntityRefs):
             try:
                 bal.parse_entity_ref(ref.toString())
@@ -168,14 +193,15 @@
                 result = BatchElementError(
                     BatchElementError.ErrorCode.kMalformedEntityReference, str(exc)
                 )
                 errorCallback(idx, result)
             else:
                 successCallback(idx, ref)
 
+    @simulated_delay
     def register(
         self,
         targetEntityRefs,
         entityTraitsDatas,
         context,
         hostSession,
         successCallback,
@@ -192,14 +218,15 @@
             else:
                 traits_dict = self.__traits_data_to_dict(entityTraitsDatas[idx])
                 updated_entity_info = bal.create_or_update_entity(
                     entity_info, traits_dict, self.__library
                 )
                 successCallback(idx, self.__build_entity_ref(updated_entity_info))
 
+    @simulated_delay
     def getRelatedReferences(
         self, entityRefs, relationshipTraitsDatas, context, hostSession, resultTraitSet=None
     ):
         results = []
 
         # The inputs are either equal length arrays with index-wise
         # correspondence, or, one of refs or relationships will have a
```

## openassetio_manager_bal/bal.py

```diff
@@ -29,14 +29,17 @@
 import os
 import string
 
 from dataclasses import dataclass
 from typing import Dict, List, Set, Optional
 from urllib.parse import urlparse
 
+SETTINGS_KEY_LIBRARY_PATH = "library_path"
+SETTINGS_KEY_SIMULATED_QUERY_LATENCY = "simulated_query_latency_ms"
+
 
 @dataclass
 class EntityInfo:
     """
     Identifies an entity within the BAL library. Convertible to/from
     OpenAssetIO entity references. Used as a key to look up entity data
     or describe a newly created entity.
@@ -70,25 +73,37 @@
 
 def make_default_settings() -> dict:
     """
     Generates a default settings dict for BAL.
     Note: as a library is required, the default settings are not enough
     to initialize the manager.
     """
-    return {"library_path": ""}
+    return {SETTINGS_KEY_LIBRARY_PATH: "", SETTINGS_KEY_SIMULATED_QUERY_LATENCY: 10}
 
 
 def validate_settings(settings: dict):
     """
     Parses the supplied settings dict, raising if there are any
     unrecognized keys present.
     """
 
     defaults = make_default_settings()
 
+    if SETTINGS_KEY_LIBRARY_PATH in settings:
+        if not isinstance(settings[SETTINGS_KEY_LIBRARY_PATH], str):
+            raise ValueError(f"{SETTINGS_KEY_LIBRARY_PATH} must be a str")
+    if SETTINGS_KEY_SIMULATED_QUERY_LATENCY in settings:
+        query_latency = settings[SETTINGS_KEY_SIMULATED_QUERY_LATENCY]
+        # This bool check is because bools are also ints as far as
+        # python is concerned.
+        if isinstance(query_latency, bool) or not isinstance(query_latency, (int, float)):
+            raise ValueError(f"{SETTINGS_KEY_SIMULATED_QUERY_LATENCY} must be a number")
+        if query_latency < 0:
+            raise ValueError(f"{SETTINGS_KEY_SIMULATED_QUERY_LATENCY} must not be negative")
+
     for key in settings:
         if key not in defaults:
             raise KeyError(f"Unknown setting '{key}'")
 
 
 def load_library(path: str) -> dict:
     """
```

## Comparing `openassetio_manager_bal-1.0.0a7.dist-info/LICENSE` & `openassetio_manager_bal-1.0.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openassetio_manager_bal-1.0.0a7.dist-info/METADATA` & `openassetio_manager_bal-1.0.0a8.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassetio-manager-bal
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: A contrived "asset management system" for OpenAssetIO integration test cases.
 Author-email: Contributors to the OpenAssetIO project <openassetio-discussion@lists.aswf.io>
 Project-URL: OpenAssetIO, https://github.com/OpenAssetIO/OpenAssetIO
 Project-URL: Source, https://github.com/OpenAssetIO/OpenAssetIO-Manager-BAL
 Project-URL: Issues, https://github.com/OpenAssetIO/OpenAssetIO-Manager-BAL/issues
 Keywords: openassetio,manager
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,21 @@
 
 - If no `library_path` has been specified, the `BAL_LIBRARY_PATH` env
   var will be checked to see if it points to a valid library file.
 
 - Persists newly registered data in-memory (the original library JSON is
   not updated).
 
+- Simulate network delay with the `simulated_query_latency_ms` setting.
+  > **Note**
+  >
+  > Pythons [time.sleep](https://docs.python.org/3/library/time.html#time.sleep)
+  > is the mechanism by which the delay is triggered.
+  > Simulated query latency defaults to 10ms.
+
 ## Installation
 
 To use the plugin in an OpenAssetIO host, install via `pip`, or set (or append) the
 `OPENASSETIO_PLUGIN_PATH` env var to include the `plugin` directory in
 a checkout of the [source repository](https://github.com/OpenAssetIO/OpenAssetIO-Manager-BAL).
 
 The plugin provides a manager with the identifier
```

## Comparing `openassetio_manager_bal-1.0.0a7.dist-info/RECORD` & `openassetio_manager_bal-1.0.0a8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-openassetio_manager_bal/BasicAssetLibraryInterface.py,sha256=2CuDt9SGeam0Zwsvt8tdS7jTl3X_v5wTH3y0KlnSwuA,9485
+openassetio_manager_bal/BasicAssetLibraryInterface.py,sha256=6YyQ0SJuQzxWctHGo6DgmmYqN_xg4tJlCwxJap3kScE,10306
 openassetio_manager_bal/__init__.py,sha256=qknWAey9xukBvuiZE_QhPdHLEnKCMVATRaCBJ9nYFk0,2977
-openassetio_manager_bal/bal.py,sha256=HcZCTij30GhXa7TytZ2drSEHCVvf-0qd8cgu5gEP31o,10682
-openassetio_manager_bal-1.0.0a7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-openassetio_manager_bal-1.0.0a7.dist-info/METADATA,sha256=b6-Ti68cTOkyJv-brK4Q-qQEg_7JPxJOinTiYW0eTEs,3745
-openassetio_manager_bal-1.0.0a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openassetio_manager_bal-1.0.0a7.dist-info/entry_points.txt,sha256=fytCZqstf6QK_vvtL6GiB-WS_cVDSbYxpbu39KvH6M4,80
-openassetio_manager_bal-1.0.0a7.dist-info/top_level.txt,sha256=cENM5tr7Znp5WE3vUGZnsNPGR-KOVR9qm54_kNPbyII,24
-openassetio_manager_bal-1.0.0a7.dist-info/RECORD,,
+openassetio_manager_bal/bal.py,sha256=px6uNnYOeJDA3E9PTQI3yEDiP0aiSGqw5yP4ff9E_yM,11567
+openassetio_manager_bal-1.0.0a8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+openassetio_manager_bal-1.0.0a8.dist-info/METADATA,sha256=YlmBYx63kO1tb4maOAP3W9PxKYRSJeeY50MxAGkmlG0,4016
+openassetio_manager_bal-1.0.0a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt,sha256=fytCZqstf6QK_vvtL6GiB-WS_cVDSbYxpbu39KvH6M4,80
+openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt,sha256=cENM5tr7Znp5WE3vUGZnsNPGR-KOVR9qm54_kNPbyII,24
+openassetio_manager_bal-1.0.0a8.dist-info/RECORD,,
```

