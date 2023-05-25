# Comparing `tmp/novu-1.2.0.tar.gz` & `tmp/novu-1.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novu-1.2.0.tar", max compression
+gzip compressed data, was "novu-1.2.1a1.tar", max compression
```

## Comparing `novu-1.2.0.tar` & `novu-1.2.1a1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1079 2023-04-13 09:41:46.445464 novu-1.2.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-13 09:41:46.445464 novu-1.2.0/README.md
--rw-r--r--   0        0        0      475 2023-04-13 09:41:46.445464 novu-1.2.0/novu/__init__.py
--rw-r--r--   0        0        0     1005 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/__init__.py
--rw-r--r--   0        0        0     2209 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/base.py
--rw-r--r--   0        0        0     2263 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/change.py
--rw-r--r--   0        0        0     2148 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/environment.py
--rw-r--r--   0        0        0     6974 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/event.py
--rw-r--r--   0        0        0     1293 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/execution_detail.py
--rw-r--r--   0        0        0     1457 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/feed.py
--rw-r--r--   0        0        0     3690 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/integration.py
--rw-r--r--   0        0        0     2681 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/layout.py
--rw-r--r--   0        0        0     1927 2023-04-13 09:41:46.445464 novu-1.2.0/novu/api/message.py
--rw-r--r--   0        0        0     1391 2023-04-13 09:41:46.449463 novu-1.2.0/novu/api/notification_group.py
--rw-r--r--   0        0        0     4121 2023-04-13 09:41:46.449463 novu-1.2.0/novu/api/notification_template.py
--rw-r--r--   0        0        0     7163 2023-04-13 09:41:46.449463 novu-1.2.0/novu/api/subscriber.py
--rw-r--r--   0        0        0     3910 2023-04-13 09:41:46.449463 novu-1.2.0/novu/api/topic.py
--rw-r--r--   0        0        0      745 2023-04-13 09:41:46.449463 novu-1.2.0/novu/config.py
--rw-r--r--   0        0        0      637 2023-04-13 09:41:46.449463 novu-1.2.0/novu/constants.py
--rw-r--r--   0        0        0     2576 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/__init__.py
--rw-r--r--   0        0        0     5825 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/base.py
--rw-r--r--   0        0        0     2156 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/change.py
--rw-r--r--   0        0        0     1942 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/environment.py
--rw-r--r--   0        0        0      476 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/event.py
--rw-r--r--   0        0        0     2185 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/execution_detail.py
--rw-r--r--   0        0        0     1066 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/feed.py
--rw-r--r--   0        0        0     1213 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/field.py
--rw-r--r--   0        0        0     1925 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/integration.py
--rw-r--r--   0        0        0     2672 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/layout.py
--rw-r--r--   0        0        0     3107 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/message.py
--rw-r--r--   0        0        0     1449 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/notification_group.py
--rw-r--r--   0        0        0     8288 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/notification_template.py
--rw-r--r--   0        0        0      865 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/step_filter.py
--rw-r--r--   0        0        0     4565 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/subscriber.py
--rw-r--r--   0        0        0     1491 2023-04-13 09:41:46.449463 novu-1.2.0/novu/dto/topic.py
--rw-r--r--   0        0        0     1425 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/__init__.py
--rw-r--r--   0        0        0      635 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/change.py
--rw-r--r--   0        0        0     1542 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/channel.py
--rw-r--r--   0        0        0      547 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/event.py
--rw-r--r--   0        0        0     1002 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/execution.py
--rw-r--r--   0        0        0     2171 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/field.py
--rw-r--r--   0        0        0      723 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/notification.py
--rw-r--r--   0        0        0     4038 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/provider.py
--rw-r--r--   0        0        0      762 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/step_filter.py
--rw-r--r--   0        0        0      371 2023-04-13 09:41:46.449463 novu-1.2.0/novu/enums/template.py
--rw-r--r--   0        0        0     1263 2023-04-13 09:41:46.449463 novu-1.2.0/novu/helpers.py
--rw-r--r--   0        0        0        0 2023-04-13 09:41:46.449463 novu-1.2.0/novu/py.typed
--rw-r--r--   0        0        0     2581 2023-04-13 09:41:46.449463 novu-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 novu-1.2.0/setup.py
--rw-r--r--   0        0        0     3925 1970-01-01 00:00:00.000000 novu-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-25 08:47:04.104364 novu-1.2.1a1/LICENSE
+-rw-r--r--   0        0        0     2297 2023-05-25 08:47:04.104364 novu-1.2.1a1/README.md
+-rw-r--r--   0        0        0      475 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/__init__.py
+-rw-r--r--   0        0        0     2209 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/base.py
+-rw-r--r--   0        0        0     2263 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/change.py
+-rw-r--r--   0        0        0     2148 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/environment.py
+-rw-r--r--   0        0        0     6974 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/event.py
+-rw-r--r--   0        0        0     1293 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/execution_detail.py
+-rw-r--r--   0        0        0     1457 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/feed.py
+-rw-r--r--   0        0        0     3690 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/integration.py
+-rw-r--r--   0        0        0     2681 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/layout.py
+-rw-r--r--   0        0        0     1927 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/message.py
+-rw-r--r--   0        0        0     1391 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/notification_group.py
+-rw-r--r--   0        0        0     4121 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/notification_template.py
+-rw-r--r--   0        0        0     7163 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/subscriber.py
+-rw-r--r--   0        0        0     3910 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/api/topic.py
+-rw-r--r--   0        0        0      745 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/config.py
+-rw-r--r--   0        0        0      637 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/constants.py
+-rw-r--r--   0        0        0     2576 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/base.py
+-rw-r--r--   0        0        0     2156 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/change.py
+-rw-r--r--   0        0        0     1942 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/environment.py
+-rw-r--r--   0        0        0      476 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/event.py
+-rw-r--r--   0        0        0     2185 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/execution_detail.py
+-rw-r--r--   0        0        0     1066 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/feed.py
+-rw-r--r--   0        0        0     1213 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/field.py
+-rw-r--r--   0        0        0     1942 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/integration.py
+-rw-r--r--   0        0        0     2672 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/layout.py
+-rw-r--r--   0        0        0     3107 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/message.py
+-rw-r--r--   0        0        0     1449 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/notification_group.py
+-rw-r--r--   0        0        0     8288 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/notification_template.py
+-rw-r--r--   0        0        0      865 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/step_filter.py
+-rw-r--r--   0        0        0     4565 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/subscriber.py
+-rw-r--r--   0        0        0     1491 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/dto/topic.py
+-rw-r--r--   0        0        0     1425 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/__init__.py
+-rw-r--r--   0        0        0      635 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/change.py
+-rw-r--r--   0        0        0     1542 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/channel.py
+-rw-r--r--   0        0        0      547 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/event.py
+-rw-r--r--   0        0        0     1002 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/execution.py
+-rw-r--r--   0        0        0     2171 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/field.py
+-rw-r--r--   0        0        0      723 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/notification.py
+-rw-r--r--   0        0        0     4038 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/provider.py
+-rw-r--r--   0        0        0      762 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/step_filter.py
+-rw-r--r--   0        0        0      371 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/enums/template.py
+-rw-r--r--   0        0        0     1263 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:47:04.104364 novu-1.2.1a1/novu/py.typed
+-rw-r--r--   0        0        0     2589 2023-05-25 08:47:04.108364 novu-1.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 novu-1.2.1a1/setup.py
+-rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 novu-1.2.1a1/PKG-INFO
```

### Comparing `novu-1.2.0/LICENSE` & `novu-1.2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/README.md` & `novu-1.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/__init__.py` & `novu-1.2.1a1/novu/api/__init__.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/base.py` & `novu-1.2.1a1/novu/api/base.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/change.py` & `novu-1.2.1a1/novu/api/change.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/environment.py` & `novu-1.2.1a1/novu/api/environment.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/event.py` & `novu-1.2.1a1/novu/api/event.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/execution_detail.py` & `novu-1.2.1a1/novu/api/execution_detail.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/feed.py` & `novu-1.2.1a1/novu/api/feed.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/integration.py` & `novu-1.2.1a1/novu/api/integration.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/layout.py` & `novu-1.2.1a1/novu/api/layout.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/message.py` & `novu-1.2.1a1/novu/api/message.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/notification_group.py` & `novu-1.2.1a1/novu/api/notification_group.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/notification_template.py` & `novu-1.2.1a1/novu/api/notification_template.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/subscriber.py` & `novu-1.2.1a1/novu/api/subscriber.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/api/topic.py` & `novu-1.2.1a1/novu/api/topic.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/config.py` & `novu-1.2.1a1/novu/config.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/constants.py` & `novu-1.2.1a1/novu/constants.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/__init__.py` & `novu-1.2.1a1/novu/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/base.py` & `novu-1.2.1a1/novu/dto/base.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/change.py` & `novu-1.2.1a1/novu/dto/change.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/environment.py` & `novu-1.2.1a1/novu/dto/environment.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/execution_detail.py` & `novu-1.2.1a1/novu/dto/execution_detail.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/feed.py` & `novu-1.2.1a1/novu/dto/feed.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/field.py` & `novu-1.2.1a1/novu/dto/field.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/integration.py` & `novu-1.2.1a1/novu/dto/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
     provider_id: ProviderIdEnum
     """Provider ID, which is one of predefined available enum"""
 
     channel: Channel
     """Integration channel"""
 
-    credentials: Dict[CredentialsKeyEnum, Union[str, bool]]
-    """Credentials of the provider"""
-
     active: bool
     """If the provider is active"""
 
+    credentials: Optional[Dict[CredentialsKeyEnum, Union[str, bool]]] = None
+    """Credentials of the provider"""
+
     _id: Optional[str] = None
     """Integration ID in Novu internal storage system"""
 
     _environment_id: Optional[str] = None
     """Environment ID in Novu internal storage system"""
 
     _organization_id: Optional[str] = None
```

### Comparing `novu-1.2.0/novu/dto/layout.py` & `novu-1.2.1a1/novu/dto/layout.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/message.py` & `novu-1.2.1a1/novu/dto/message.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/notification_group.py` & `novu-1.2.1a1/novu/dto/notification_group.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/notification_template.py` & `novu-1.2.1a1/novu/dto/notification_template.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/step_filter.py` & `novu-1.2.1a1/novu/dto/step_filter.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/subscriber.py` & `novu-1.2.1a1/novu/dto/subscriber.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/dto/topic.py` & `novu-1.2.1a1/novu/dto/topic.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/__init__.py` & `novu-1.2.1a1/novu/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/change.py` & `novu-1.2.1a1/novu/enums/change.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/channel.py` & `novu-1.2.1a1/novu/enums/channel.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/event.py` & `novu-1.2.1a1/novu/enums/event.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/execution.py` & `novu-1.2.1a1/novu/enums/execution.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/field.py` & `novu-1.2.1a1/novu/enums/field.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/notification.py` & `novu-1.2.1a1/novu/enums/notification.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/provider.py` & `novu-1.2.1a1/novu/enums/provider.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/enums/step_filter.py` & `novu-1.2.1a1/novu/enums/step_filter.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/novu/helpers.py` & `novu-1.2.1a1/novu/helpers.py`

 * *Files identical despite different names*

### Comparing `novu-1.2.0/pyproject.toml` & `novu-1.2.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 description = "This project aims to provide a wrapper for the Novu API."
 keywords = ["novu", "python", "sdk", "api", "wrapper"]
 name = "novu"
-version = "1.2.0"
+version = "1.2.1-alpha.1"
 
 documentation = "https://novu-python.readthedocs.io/en/latest"
 homepage = "https://novu-python.readthedocs.io/en/latest"
 repository = "https://github.com/novuhq/novu-python"
 
 authors = ["oscar.marie-taillefer <oscar.marie-taillefer@spikeelabs.fr>"]
 maintainers = ["oscar.marie-taillefer <oscar.marie-taillefer@spikeelabs.fr>"]
```

### Comparing `novu-1.2.0/setup.py` & `novu-1.2.1a1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'novu',
-    'version': '1.2.0',
+    'version': '1.2.1a1',
     'description': 'This project aims to provide a wrapper for the Novu API.',
     'long_description': '# Python Novu SDK\n\n[![PyPI](https://img.shields.io/pypi/v/novu?color=blue)](https://pypi.org/project/novu/)\n![Tests Status](https://github.com/novuhq/novu-python/actions/workflows/.github/workflows/tests.yml/badge.svg)\n[![codecov](https://codecov.io/gh/novuhq/novu-python/branch/main/graph/badge.svg?token=RON7F8QTZX)](https://codecov.io/gh/novuhq/novu-python)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/novu)\n![PyPI - License](https://img.shields.io/pypi/l/novu)\n[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)\n\n---\n\nThe [Python Novu](https://novu.co) SDK and package provides a fluent and expressive interface for interacting with [Novu\'s API](https://api.novu.co/api) and managing notifications.\n\n## Install\n\nTo install this package\n\n```shell\n# Via pip\npip install novu\n\n# Via poetry\npoetry add novu\n```\n\n## Quick start\n\nThis package is a wrapper of all the resources offered by Novu, we will just start by triggering an event on Novu.\n\nTo do this, you will need to:\n\n1. Create your first notification template and keep in mind the identifier to trigger the template: https://docs.novu.co/overview/quick-start#create-a-notification-template\n2. Retrieve your API key from the Novu dashboard directly in the settings section: https://web.novu.co/settings\n3. Write code to trigger your first event:\n\n```python\nfrom novu.api import EventApi\n\nevent_api = EventApi("https://api.novu.co/api/", "<NOVU_API_TOKEN>")\nevent_api.trigger(\n    name="<YOUR_TEMPLATE_NAME>",\n    recipients="<YOUR_SUBSCRIBER_ID>",\n    payload={},  # Your Novu payload goes here\n)\n```\n\nThis will trigger a notification to the subscribers.\n\n## Development\n\n```bash\n# install deps\npoetry install\n\n# pre-commit\npoetry run pre-commit install --install-hook\npoetry run pre-commit install --install-hooks --hook-type commit-msg\n```\n',
     'author': 'oscar.marie-taillefer',
     'author_email': 'oscar.marie-taillefer@spikeelabs.fr',
     'maintainer': 'oscar.marie-taillefer',
     'maintainer_email': 'oscar.marie-taillefer@spikeelabs.fr',
     'url': 'https://novu-python.readthedocs.io/en/latest',
```

### Comparing `novu-1.2.0/PKG-INFO` & `novu-1.2.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novu
-Version: 1.2.0
+Version: 1.2.1a1
 Summary: This project aims to provide a wrapper for the Novu API.
 Home-page: https://novu-python.readthedocs.io/en/latest
 License: MIT
 Keywords: novu,python,sdk,api,wrapper
 Author: oscar.marie-taillefer
 Author-email: oscar.marie-taillefer@spikeelabs.fr
 Maintainer: oscar.marie-taillefer
```

