# Comparing `tmp/keycloak_django-1.0.8.tar.gz` & `tmp/keycloak_django-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.8.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.9.tar", max compression
```

## Comparing `keycloak_django-1.0.8.tar` & `keycloak_django-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.8/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.8/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.8/README.md
--rwxr-xr-x   0        0        0      971 2023-05-25 02:05:08.748576 keycloak_django-1.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      114 2023-05-25 02:05:18.312347 keycloak_django-1.0.8/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.8/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.8/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.8/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.8/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.0.8/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.8/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.8/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.8/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    16413 2023-05-25 02:04:39.844129 keycloak_django-1.0.8/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.8/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.0.8/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.8/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.0.8/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.8/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.8/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.8/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.8/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     3086 2023-05-25 02:01:18.519975 keycloak_django-1.0.8/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.8/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.8/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1576 2023-05-25 02:03:00.399252 keycloak_django-1.0.8/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.9/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.9/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.9/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-25 02:36:58.139497 keycloak_django-1.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-05-25 02:37:05.252146 keycloak_django-1.0.9/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.9/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.9/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.9/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.9/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.0.9/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.9/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.9/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.9/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    16413 2023-05-25 02:04:39.844129 keycloak_django-1.0.9/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.9/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.0.9/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.9/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.0.9/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.9/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.9/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.9/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.9/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     3099 2023-05-25 02:36:23.865569 keycloak_django-1.0.9/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.9/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.9/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1576 2023-05-25 02:03:00.399252 keycloak_django-1.0.9/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.9/PKG-INFO
```

### Comparing `keycloak_django-1.0.8/LICENSE` & `keycloak_django-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/pyproject.toml` & `keycloak_django-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.8"
+version = "1.0.9"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.8/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.9/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/authentication.py` & `keycloak_django-1.0.9/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.9/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.9/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/middleware.py` & `keycloak_django-1.0.9/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.9/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/models.py` & `keycloak_django-1.0.9/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/security.py` & `keycloak_django-1.0.9/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.9/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.9/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.9/src/keycloak_django/services/realm_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,24 +45,25 @@
             "port": realm_model.email_realm_config.port,
             "replyTo": realm_model.email_realm_config.replyTo,
             "host": realm_model.email_realm_config.host,
             "from": realm_model.email_realm_config.from_email,
             "fromDisplayName": realm_model.email_realm_config.fromDisplayName,
             "user": realm_model.email_realm_config.user
         }
-        keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
+        keycloak_admin.update_realm(
+            realm_name=realm_model.realm, payload=payload)
 
 
 def delete_realm_by_owner(realm_model):
     keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.delete_realm(realm_name=realm_model.realm)
 
 
 def get_apps_login_by_owner(user):
     keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.set_realm_name(realm_name=user.realm_name)
     logins = set([group.name for group in user.groups if group.name.startswith(
         f'login_{user.realm_name}')])
     clients = keycloak_admin.get_clients()
     clients = [
-        client for client in clients if f"login_{user.realm_name}_{client['client_id']}" in logins]
-    return clients
+        client for client in clients if f"login_{user.realm_name}_{client['clientId']}" in logins]
+    return clients
```

### Comparing `keycloak_django-1.0.8/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.9/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.9/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/src/keycloak_django/tools.py` & `keycloak_django-1.0.9/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.8/PKG-INFO` & `keycloak_django-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.8
+Version: 1.0.9
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

