# Comparing `tmp/crc-event-schemas-0.1.5.tar.gz` & `tmp/crc-event-schemas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-event-schemas-0.1.5.tar", last modified: Thu May 11 12:57:41 2023, max compression
+gzip compressed data, was "crc-event-schemas-0.1.6.tar", last modified: Thu May 25 12:31:33 2023, max compression
```

## Comparing `crc-event-schemas-0.1.5.tar` & `crc-event-schemas-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/crc_event_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-11 12:57:41.000000 crc-event-schemas-0.1.5/crc_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-11 12:57:41.000000 crc-event-schemas-0.1.5/crc_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:57:41.000000 crc-event-schemas-0.1.5/crc_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 12:57:41.000000 crc-event-schemas-0.1.5/crc_event_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/event_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/event_schemas/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/event_schemas/apps/advisor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/advisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/event_schemas/apps/advisor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/advisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/advisor/v1/advisor_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.720126 crc-event-schemas-0.1.5/event_schemas/apps/export_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/export_service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/apps/export_service/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/export_service/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/export_service/v1/export_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/apps/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/apps/policies/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/policies/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/policies/v1/policy_triggered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/apps/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/apps/repositories/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/repositories/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/apps/repositories/v1/repository_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/event_schemas/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/core/v1/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/core/v1/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/event_schemas/core/v1/rhel_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:57:41.724126 crc-event-schemas-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 12:57:28.000000 crc-event-schemas-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.086366 crc-event-schemas-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/crc_event_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 12:31:33.000000 crc-event-schemas-0.1.6/crc_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-25 12:31:33.000000 crc-event-schemas-0.1.6/crc_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:31:33.000000 crc-event-schemas-0.1.6/crc_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 12:31:33.000000 crc-event-schemas-0.1.6/crc_event_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/advisor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/advisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/advisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/advisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/advisor/v1/advisor_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/export_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/export_service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/export_service/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/export_service/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/export_service/v1/resource_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/policies/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/policies/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/policies/v1/policy_triggered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/apps/repositories/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/repositories/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/apps/repositories/v1/repository_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:33.082366 crc-event-schemas-0.1.6/event_schemas/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/core/v1/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/core/v1/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/event_schemas/core/v1/rhel_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:31:33.086366 crc-event-schemas-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-25 12:31:19.000000 crc-event-schemas-0.1.6/setup.py
```

### Comparing `crc-event-schemas-0.1.5/LICENSE.txt` & `crc-event-schemas-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/PKG-INFO` & `crc-event-schemas-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-event-schemas
-Version: 0.1.5
+Version: 0.1.6
 Summary: CloudEvents type bindings for console.redhat.com
 Home-page: https://github.com/RedHatInsights/event-schemas-python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 console.redhat.com CloudEvents for Python
 =======================================
```

### Comparing `crc-event-schemas-0.1.5/README.md` & `crc-event-schemas-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/crc_event_schemas.egg-info/PKG-INFO` & `crc-event-schemas-0.1.6/crc_event_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-event-schemas
-Version: 0.1.5
+Version: 0.1.6
 Summary: CloudEvents type bindings for console.redhat.com
 Home-page: https://github.com/RedHatInsights/event-schemas-python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 console.redhat.com CloudEvents for Python
 =======================================
```

### Comparing `crc-event-schemas-0.1.5/crc_event_schemas.egg-info/SOURCES.txt` & `crc-event-schemas-0.1.6/crc_event_schemas.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 event_schemas/__init__.py
 event_schemas/apps/__init__.py
 event_schemas/apps/advisor/__init__.py
 event_schemas/apps/advisor/v1/__init__.py
 event_schemas/apps/advisor/v1/advisor_recommendations.py
 event_schemas/apps/export_service/__init__.py
 event_schemas/apps/export_service/v1/__init__.py
-event_schemas/apps/export_service/v1/export_request.py
+event_schemas/apps/export_service/v1/resource_request.py
 event_schemas/apps/policies/__init__.py
 event_schemas/apps/policies/v1/__init__.py
 event_schemas/apps/policies/v1/policy_triggered.py
 event_schemas/apps/repositories/__init__.py
 event_schemas/apps/repositories/v1/__init__.py
 event_schemas/apps/repositories/v1/repository_events.py
 event_schemas/core/__init__.py
```

### Comparing `crc-event-schemas-0.1.5/event_schemas/apps/advisor/v1/advisor_recommendations.py` & `crc-event-schemas-0.1.6/event_schemas/apps/advisor/v1/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/event_schemas/apps/export_service/v1/export_request.py` & `crc-event-schemas-0.1.6/event_schemas/apps/export_service/v1/resource_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
-from typing import Dict, Any, Optional, TypeVar, Callable, Type, cast
 from uuid import UUID
+from typing import Dict, Any, Optional, TypeVar, Callable, Type, cast
 
 
 T = TypeVar("T")
 EnumT = TypeVar("EnumT", bound=Enum)
 
 
 def from_str(x: Any) -> str:
@@ -43,79 +43,84 @@
 
 class Format(Enum):
     """The format of the data to be exported"""
     CSV = "csv"
     JSON = "json"
 
 
-class ExportRequestClass:
+class ResourceRequestClass:
     """A request for data to be exported"""
     """The application being requested"""
     application: str
+    """The unique identifier of the export request that triggered the resource request"""
+    export_request_uuid: UUID
     """The filters to be applied to the data"""
     filters: Optional[Dict[str, Any]]
     """The format of the data to be exported"""
     format: Format
     """The resource to be exported"""
     resource: str
-    """A unique identifier for the request"""
+    """A unique identifier for the resource request"""
     uuid: UUID
     """The Base64-encoded JSON identity header of the user making the request"""
     x_rh_identity: str
 
-    def __init__(self, application: str, filters: Optional[Dict[str, Any]], format: Format, resource: str, uuid: UUID, x_rh_identity: str) -> None:
+    def __init__(self, application: str, export_request_uuid: UUID, filters: Optional[Dict[str, Any]], format: Format, resource: str, uuid: UUID, x_rh_identity: str) -> None:
         self.application = application
+        self.export_request_uuid = export_request_uuid
         self.filters = filters
         self.format = format
         self.resource = resource
         self.uuid = uuid
         self.x_rh_identity = x_rh_identity
 
     @staticmethod
-    def from_dict(obj: Any) -> 'ExportRequestClass':
+    def from_dict(obj: Any) -> 'ResourceRequestClass':
         assert isinstance(obj, dict)
         application = from_str(obj.get("application"))
+        export_request_uuid = UUID(obj.get("export_request_uuid"))
         filters = from_union([lambda x: from_dict(lambda x: x, x), from_none], obj.get("filters"))
         format = Format(obj.get("format"))
         resource = from_str(obj.get("resource"))
         uuid = UUID(obj.get("uuid"))
         x_rh_identity = from_str(obj.get("x-rh-identity"))
-        return ExportRequestClass(application, filters, format, resource, uuid, x_rh_identity)
+        return ResourceRequestClass(application, export_request_uuid, filters, format, resource, uuid, x_rh_identity)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["application"] = from_str(self.application)
+        result["export_request_uuid"] = str(self.export_request_uuid)
         if self.filters is not None:
             result["filters"] = from_union([lambda x: from_dict(lambda x: x, x), from_none], self.filters)
         result["format"] = to_enum(Format, self.format)
         result["resource"] = from_str(self.resource)
         result["uuid"] = str(self.uuid)
         result["x-rh-identity"] = from_str(self.x_rh_identity)
         return result
 
 
-class ExportRequest:
-    """Event data for data export requests."""
+class ResourceRequest:
+    """Event data for data export requests"""
     """A request for data to be exported"""
-    export_request: ExportRequestClass
+    resource_request: ResourceRequestClass
 
-    def __init__(self, export_request: ExportRequestClass) -> None:
-        self.export_request = export_request
+    def __init__(self, resource_request: ResourceRequestClass) -> None:
+        self.resource_request = resource_request
 
     @staticmethod
-    def from_dict(obj: Any) -> 'ExportRequest':
+    def from_dict(obj: Any) -> 'ResourceRequest':
         assert isinstance(obj, dict)
-        export_request = ExportRequestClass.from_dict(obj.get("exportRequest"))
-        return ExportRequest(export_request)
+        resource_request = ResourceRequestClass.from_dict(obj.get("resource_request"))
+        return ResourceRequest(resource_request)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        result["exportRequest"] = to_class(ExportRequestClass, self.export_request)
+        result["resource_request"] = to_class(ResourceRequestClass, self.resource_request)
         return result
 
 
-def export_request_from_dict(s: Any) -> ExportRequest:
-    return ExportRequest.from_dict(s)
+def resource_request_from_dict(s: Any) -> ResourceRequest:
+    return ResourceRequest.from_dict(s)
 
 
-def export_request_to_dict(x: ExportRequest) -> Any:
-    return to_class(ExportRequest, x)
+def resource_request_to_dict(x: ResourceRequest) -> Any:
+    return to_class(ResourceRequest, x)
```

### Comparing `crc-event-schemas-0.1.5/event_schemas/apps/policies/v1/policy_triggered.py` & `crc-event-schemas-0.1.6/event_schemas/apps/policies/v1/policy_triggered.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/event_schemas/apps/repositories/v1/repository_events.py` & `crc-event-schemas-0.1.6/event_schemas/apps/repositories/v1/repository_events.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/event_schemas/core/v1/error.py` & `crc-event-schemas-0.1.6/event_schemas/core/v1/error.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/event_schemas/core/v1/notification.py` & `crc-event-schemas-0.1.6/event_schemas/core/v1/notification.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.5/event_schemas/core/v1/rhel_system.py` & `crc-event-schemas-0.1.6/event_schemas/core/v1/rhel_system.py`

 * *Files identical despite different names*

