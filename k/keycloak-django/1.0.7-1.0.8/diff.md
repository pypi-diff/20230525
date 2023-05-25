# Comparing `tmp/keycloak_django-1.0.7.tar.gz` & `tmp/keycloak_django-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.7.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.8.tar", max compression
```

## Comparing `keycloak_django-1.0.7.tar` & `keycloak_django-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.7/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.7/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.7/README.md
--rwxr-xr-x   0        0        0      971 2023-05-19 17:44:26.439350 keycloak_django-1.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      114 2023-05-19 17:44:32.418126 keycloak_django-1.0.7/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.7/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.7/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.7/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.7/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.7/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.7/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.7/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.7/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    16285 2023-05-19 17:44:12.415179 keycloak_django-1.0.7/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.7/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.7/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.7/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.7/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.7/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.7/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.7/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.7/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.7/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.7/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.7/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.7/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.8/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.8/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.8/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-25 02:05:08.748576 keycloak_django-1.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-05-25 02:05:18.312347 keycloak_django-1.0.8/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.8/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.8/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.8/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.8/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.0.8/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.8/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.8/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.8/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    16413 2023-05-25 02:04:39.844129 keycloak_django-1.0.8/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.8/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.0.8/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.8/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.0.8/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.8/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.8/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.8/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.8/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     3086 2023-05-25 02:01:18.519975 keycloak_django-1.0.8/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.8/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.8/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1576 2023-05-25 02:03:00.399252 keycloak_django-1.0.8/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.8/PKG-INFO
```

### Comparing `keycloak_django-1.0.7/LICENSE` & `keycloak_django-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/pyproject.toml` & `keycloak_django-1.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.7"
+version = "1.0.8"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.7/src/keycloak_django/authentication.py` & `keycloak_django-1.0.8/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.8/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.8/src/keycloak_django/keycloak.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,16 @@
         :raises KeycloakInvalidTokenError: In case of bad token
         """
         try:
             if public_key_validate == 'auto':
                 kwargs['key'] = self.get_key_rsa(token)
 
             token_info = self._token_info(token, method_token_info, **kwargs)
+            realm_name = token_info.get('iss', 'https/master').split('/')[-1]
+            token_info['realm_name'] = realm_name
         except Exception as e:
             print(str(e))
             raise KeycloakInvalidTokenError("Token expired or invalid.")
 
         if method_token_info == "introspect" and not token_info["active"]:
             raise KeycloakInvalidTokenError("Token expired or invalid.")
```

### Comparing `keycloak_django-1.0.7/src/keycloak_django/middleware.py` & `keycloak_django-1.0.8/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/models.py` & `keycloak_django-1.0.8/src/keycloak_django/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             user.password = make_password(password)
             user.save(using=self._db)
             user_id = create_user_by_owner(user, password=password)
             get_user_model().objects.filter(id=user.id).update(id=user_id)
             user.id = user_id
             return user
 
-
     def create_user(self, username, email=None, password=None, **extra_fields):
         extra_fields.setdefault("is_staff", False)
         extra_fields.setdefault("is_superuser", False)
         return self._create_user(username, email, password, **extra_fields)
 
     def create_superuser(self, username, email=None, password=None, **extra_fields):
         extra_fields.setdefault("is_staff", True)
@@ -108,15 +107,16 @@
     )
     first_name = models.CharField(_("first name"), max_length=150, blank=True)
     last_name = models.CharField(_("last name"), max_length=150, blank=True)
     email = models.EmailField(_("email address"), blank=True, unique=True)
     is_staff = models.BooleanField(
         _("staff status"),
         default=False,
-        help_text=_("Designates whether the user can log into this admin site."),
+        help_text=_(
+            "Designates whether the user can log into this admin site."),
     )
     is_active = models.BooleanField(
         _("active"),
         default=True,
         help_text=_(
             "Designates whether this user should be treated as active. "
             "Unselect this instead of deleting accounts."
@@ -124,50 +124,51 @@
     )
     date_joined = models.DateTimeField(_("date joined"), default=timezone.now)
 
     objects = UserManager()
 
     EMAIL_FIELD = "email"
     USERNAME_FIELD = 'email'
-    REQUIRED_FIELDS = ['username', 'first_name', 'last_name']
+    REQUIRED_FIELDS = ['username', 'first_name', 'last_name', 'realm_name']
 
     """
          Add the fields and methods necessary to support the Group and Permission
          models using the ModelBackend.
          """
 
     is_superuser = models.BooleanField(
         _("superuser status"),
         default=False,
         help_text=_(
             "Designates that this user has all permissions without "
             "explicitly assigning them."
         ),
     )
+    realm_name = models.CharField(
+        _("realm name"), max_length=150, blank=True, null=True)
     permissions: List[Permission] = []
     groups: List[Group] = []
 
     class Meta:
         verbose_name = _("user")
         verbose_name_plural = _("users")
         abstract = True
 
     def get_username(self):
         """Return the username for this User."""
         return getattr(self, self.USERNAME_FIELD)
 
     def clean(self):
-        setattr(self, self.USERNAME_FIELD, self.normalize_username(self.get_username()))
+        setattr(self, self.USERNAME_FIELD,
+                self.normalize_username(self.get_username()))
         self.email = self.__class__.objects.normalize_email(self.email)
 
-
     def natural_key(self):
         return self.get_username(),
 
-
     @property
     def is_anonymous(self):
         """
         Always return False. This is a way of comparing User objects to
         anonymous users.
         """
         return False
@@ -251,15 +252,14 @@
 
     def save(self, *args, **kwargs):
         super().save(*args, **kwargs)
         if self._password is not None:
             password_validation.password_changed(self._password, self)
             self._password = None
 
-
     def get_user_permissions(self, obj=None):
         """
         Return a list of permission strings that this user has directly.
         Query all available auth_panel backends. If an object is passed in,
         return only permissions matching this object.
         """
         return set(self.permissions)
```

### Comparing `keycloak_django-1.0.7/src/keycloak_django/security.py` & `keycloak_django-1.0.8/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.8/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.8/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.8/src/keycloak_django/services/realm_repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,8 +50,19 @@
             "user": realm_model.email_realm_config.user
         }
         keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
 
 
 def delete_realm_by_owner(realm_model):
     keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.delete_realm(realm_name=realm_model.realm)
+    keycloak_admin.delete_realm(realm_name=realm_model.realm)
+
+
+def get_apps_login_by_owner(user):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user.realm_name)
+    logins = set([group.name for group in user.groups if group.name.startswith(
+        f'login_{user.realm_name}')])
+    clients = keycloak_admin.get_clients()
+    clients = [
+        client for client in clients if f"login_{user.realm_name}_{client['client_id']}" in logins]
+    return clients
```

### Comparing `keycloak_django-1.0.7/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.8/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.8/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.7/src/keycloak_django/tools.py` & `keycloak_django-1.0.8/src/keycloak_django/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,26 @@
     """
     Return the User Keycloak model that is active in this project.
     """
     if hasattr(user, 'is_superuser'):
         user.is_superuser = user_info.get('is_superuser', False)
     if hasattr(user, 'is_staff'):
         user.is_staff = user_info.get('is_staff', True)
+    if hasattr(user, 'realm_name'):
+        user.realm_name = user_info.get('realm_name', 'master')
     return user
 
 
 def get_user_model_keycloak():
     """
     Return the User Keycloak model that is active in this project.
     """
     try:
         return django_apps.get_model(settings.KEYCLOAK['KEYCLOAK_USER_MODEL'], require_ready=False)
     except ValueError:
-        raise ImproperlyConfigured("KEYCLOAK_USER_MODEL must be of the form 'app_label.model_name'")
+        raise ImproperlyConfigured(
+            "KEYCLOAK_USER_MODEL must be of the form 'app_label.model_name'")
     except LookupError:
         raise ImproperlyConfigured(
-            "KEYCLOAK_USER_MODEL refers to model '%s' that has not been installed" % settings.KEYCLOAK['KEYCLOAK_USER_MODEL']
-        )
+            "KEYCLOAK_USER_MODEL refers to model '%s' that has not been installed" % settings.KEYCLOAK[
+                'KEYCLOAK_USER_MODEL']
+        )
```

### Comparing `keycloak_django-1.0.7/PKG-INFO` & `keycloak_django-1.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.7
+Version: 1.0.8
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

