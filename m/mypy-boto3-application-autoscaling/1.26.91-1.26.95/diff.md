# Comparing `tmp/mypy-boto3-application-autoscaling-1.26.91.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.26.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.26.95.tar", last modified: Mon Mar 20 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.26.91.tar` & `mypy-boto3-application-autoscaling-1.26.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.341219 mypy-boto3-application-autoscaling-1.26.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-03-14 19:48:00.341219 mypy-boto3-application-autoscaling-1.26.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.341219 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21555 2023-03-14 19:46:52.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21512 2023-03-14 19:46:52.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.341219 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-14 19:48:00.000000 mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.341219 mypy-boto3-application-autoscaling-1.26.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-14 19:46:51.000000 mypy-boto3-application-autoscaling-1.26.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-03-20 19:32:25.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-03-20 19:32:25.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/LICENSE` & `mypy-boto3-application-autoscaling-1.26.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/PKG-INFO` & `mypy-boto3-application-autoscaling-1.26.95/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.26.91
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.95
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -358,25 +358,30 @@
     DeregisterScalableTargetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
+    TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
+    UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/README.md` & `mypy-boto3-application-autoscaling-1.26.95/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -326,25 +326,30 @@
     DeregisterScalableTargetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
+    TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
+    UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationAutoScaling 1.26.91\nVersion:        "
-        " 1.26.91\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ApplicationAutoScaling 1.26.95\nVersion:        "
+        " 1.26.95\nBuilder version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.91")
+    print("1.26.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     DescribeScheduledActionsPaginator,
 )
 from .type_defs import (
     DescribeScalableTargetsResponseTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -59,14 +61,16 @@
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
+    ResourceNotFoundException: Type[BotocoreClientError]
+    TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
@@ -226,14 +230,22 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
 
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Returns all the tags on the specified Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
+        """
+
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
@@ -275,23 +287,41 @@
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
         MaxCapacity: int = ...,
         RoleARN: str = ...,
-        SuspendedState: SuspendedStateTypeDef = ...
-    ) -> Dict[str, Any]:
+        SuspendedState: SuspendedStateTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> RegisterScalableTargetResponseTypeDef:
         """
-        Registers or updates a scalable target, the resource that you want to scale.
+        Registers or updates a scalable target, which is the resource that you want to
+        scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
 
+    def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Adds or edits tags on an Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Deletes tags from an Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     DescribeScheduledActionsPaginator,
 )
 from .type_defs import (
     DescribeScalableTargetsResponseTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -56,14 +58,16 @@
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
+    ResourceNotFoundException: Type[BotocoreClientError]
+    TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
     """
@@ -211,14 +215,21 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Returns all the tags on the specified Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
+        """
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
@@ -258,22 +269,38 @@
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
         MaxCapacity: int = ...,
         RoleARN: str = ...,
-        SuspendedState: SuspendedStateTypeDef = ...
-    ) -> Dict[str, Any]:
+        SuspendedState: SuspendedStateTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> RegisterScalableTargetResponseTypeDef:
         """
-        Registers or updates a scalable target, the resource that you want to scale.
+        Registers or updates a scalable target, which is the resource that you want to
+        scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
+    def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Adds or edits tags on an Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
+        """
+    def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Deletes tags from an Application Auto Scaling scalable target.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_application_autoscaling.type_defs import AlarmTypeDef
 
     data: AlarmTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdjustmentTypeType,
     MetricAggregationTypeType,
     MetricStatisticType,
     MetricTypeType,
     PolicyTypeType,
@@ -27,38 +27,42 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "NotScaledReasonTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
     "StepAdjustmentTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricTypeDef",
@@ -142,22 +146,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -179,22 +181,20 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
-
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -205,22 +205,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -231,21 +229,26 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
 
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
@@ -255,40 +258,36 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
-
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
     pass
 
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
-
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -315,27 +314,41 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
-
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Mapping[str, str],
+    },
+)
 
 TargetTrackingMetricDimensionTypeDef = TypedDict(
     "TargetTrackingMetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
 _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
@@ -344,22 +357,20 @@
         "ResourceIds": Sequence[str],
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
     _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
@@ -369,22 +380,20 @@
         "ScalableDimension": ScalableDimensionType,
         "IncludeNotScaledActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
     _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
@@ -394,22 +403,20 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
     _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
@@ -419,31 +426,45 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
     _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -460,19 +481,17 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
-
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
-
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -486,22 +505,20 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredScheduledActionTypeDef = TypedDict(
     "_RequiredScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
         "Schedule": str,
@@ -517,19 +534,17 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-
 class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
-
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
@@ -537,26 +552,25 @@
 _OptionalRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterScalableTargetRequestRequestTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -565,23 +579,22 @@
         "CreationTime": datetime,
     },
 )
 _OptionalScalableTargetTypeDef = TypedDict(
     "_OptionalScalableTargetTypeDef",
     {
         "SuspendedState": SuspendedStateTypeDef,
+        "ScalableTargetARN": str,
     },
     total=False,
 )
 
-
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
-
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
         "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
@@ -638,21 +651,19 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
-
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -662,21 +673,19 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
@@ -700,22 +709,20 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -727,21 +734,19 @@
         "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -756,19 +761,17 @@
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
         "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_application_autoscaling.type_defs import AlarmTypeDef
 
     data: AlarmTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdjustmentTypeType,
     MetricAggregationTypeType,
     MetricStatisticType,
     MetricTypeType,
     PolicyTypeType,
@@ -27,37 +27,43 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "NotScaledReasonTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
     "StepAdjustmentTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricTypeDef",
@@ -141,20 +147,22 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -176,20 +184,22 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
+
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -200,20 +210,22 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -224,20 +236,29 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
+
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -246,36 +267,40 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
+
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
     pass
 
+
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
+
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -302,25 +327,43 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
+
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Mapping[str, str],
+    },
+)
+
 TargetTrackingMetricDimensionTypeDef = TypedDict(
     "TargetTrackingMetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
 _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
@@ -329,20 +372,22 @@
         "ResourceIds": Sequence[str],
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
     _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
@@ -352,20 +397,22 @@
         "ScalableDimension": ScalableDimensionType,
         "IncludeNotScaledActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
     _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
@@ -375,20 +422,22 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
     _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
@@ -398,29 +447,47 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
     _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -437,17 +504,19 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
+
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
+
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -461,20 +530,22 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
+
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredScheduledActionTypeDef = TypedDict(
     "_RequiredScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
         "Schedule": str,
@@ -490,17 +561,19 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
+
 class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
+
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
@@ -508,24 +581,27 @@
 _OptionalRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterScalableTargetRequestRequestTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -534,21 +610,24 @@
         "CreationTime": datetime,
     },
 )
 _OptionalScalableTargetTypeDef = TypedDict(
     "_OptionalScalableTargetTypeDef",
     {
         "SuspendedState": SuspendedStateTypeDef,
+        "ScalableTargetARN": str,
     },
     total=False,
 )
 
+
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
+
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
         "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
@@ -605,19 +684,21 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
+
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -627,19 +708,21 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
+
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
@@ -663,20 +746,22 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -688,19 +773,21 @@
         "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -715,17 +802,19 @@
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
         "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
+
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
+
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.26.91
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.95
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -358,25 +358,30 @@
     DeregisterScalableTargetRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     NotScaledReasonTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
     StepAdjustmentTypeDef,
+    TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
+    UntagResourceRequestRequestTypeDef,
     DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.26.91/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.91/setup.py` & `mypy-boto3-application-autoscaling-1.26.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.26.91",
+    version="1.26.95",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationAutoScaling 1.26.91 service generated with"
+        "Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with"
         " mypy-boto3-builder 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

