# Comparing `tmp/sag-py-auth-brand-0.2.1.tar.gz` & `tmp/sag-py-auth-brand-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-auth-brand-0.2.1.tar", last modified: Thu Apr 20 08:23:33 2023, max compression
+gzip compressed data, was "sag-py-auth-brand-0.2.2.tar", last modified: Thu May 25 12:56:58 2023, max compression
```

## Comparing `sag-py-auth-brand-0.2.1.tar` & `sag-py-auth-brand-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/sag_py_auth_brand/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/brand_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_logging_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 08:23:33.822901 sag-py-auth-brand-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.257049 sag-py-auth-brand-0.2.2/sag_py_auth_brand/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/brand_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_request_brand_logging_filter.py
```

### Comparing `sag-py-auth-brand-0.2.1/LICENSE.txt` & `sag-py-auth-brand-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/PKG-INFO` & `sag-py-auth-brand-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.2.1
+Version: 0.2.2
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
```

### Comparing `sag-py-auth-brand-0.2.1/README.md` & `sag-py-auth-brand-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand/brand_jwt_auth.py` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand/brand_jwt_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,8 +76,8 @@
         if len(accessible_brand_alias_ids) > 1:
             logger.warning(LogMessages.UNAMBIGUOUS_BRAND_ALIAS)
             return None
         if not accessible_brand_alias_ids:
             logger.warning(LogMessages.MISSING_COMPOUND_BRAND)
             return None
 
-        return brand_aliases[0]
+        return brand_aliases[accessible_brand_alias_ids[0]]
```

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand/models.py` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand/models.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_context.py` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_context.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_logging_filter.py` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_logging_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/PKG-INFO` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.2.1
+Version: 0.2.2
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
```

### Comparing `sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/SOURCES.txt` & `sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/setup.py` & `sag-py-auth-brand-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-auth-brand",
-    version="0.2.1",
+    version="0.2.2",
     description="Keycloak brand/instance authentication for python projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_auth_brand",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__call.py` & `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__call.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__init.py` & `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__init.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand.py` & `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand_alias.py` & `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand_alias.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,18 +38,50 @@
         # Assert
 
         # Has to be the brand of the request
         mock_set_brand_to_context.assert_called_once_with("secondalias")
         # Has to be the alias of the brand from the request.
         # The alias is the brand that has originally had access to the api
         # It is used in the entire background logic as brand
+        # Note: Here we always get the brand that is present in both lists, role-brand and role-brand-aliases
         mock_set_brand_alias_to_context.assert_called_once_with("mybrandone")
 
     @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_alias_to_context")
     @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_to_context")
+    def test__verify_brand__where_user_has_brand_alias_at_any_position(
+        self, mock_set_brand_to_context: Mock, mock_set_brand_alias_to_context: Mock
+    ) -> None:
+        # Arrange
+        brand_jwt_auth: BrandJwtAuth = build_sample_jwt_auth(["myEndpoint"])
+
+        resource_access: Optional[Dict[str, Any]] = {
+            "role-brand": {"roles": ["a-random-brand", "another-random-brand", "a-matching-alias"]},
+            "role-brand-alias": {
+                "roles": ["a-random-alias", "a-matching-alias", "another-random-alias", "the-request-alias"]
+            },
+        }
+
+        token: Token = get_token(None, resource_access)
+
+        # Act
+        brand_jwt_auth._verify_brand(token, "the-request-alias")
+
+        # Assert
+
+        # Has to be the brand of the request
+        mock_set_brand_to_context.assert_called_once_with("the-request-alias")
+
+        # Has to be the alias of the brand from the request.
+        # The alias is the brand that has originally had access to the api
+        # It is used in the entire background logic as brand
+        # Note: Here we always get the brand that is present in both lists, role-brand and role-brand-aliases
+        mock_set_brand_alias_to_context.assert_called_once_with("a-matching-alias")
+
+    @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_alias_to_context")
+    @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_to_context")
     def test__verify_brand__with_missing_brand_alias(
         self, mock_set_brand_to_context: Mock, mock_set_brand_alias_to_context: Mock
     ) -> None:
         # Arrange
         brand_jwt_auth: BrandJwtAuth = build_sample_jwt_auth(["myEndpoint"])
 
         resource_access: Optional[Dict[str, Any]] = {
```

### Comparing `sag-py-auth-brand-0.2.1/tests/test_request_brand_context.py` & `sag-py-auth-brand-0.2.2/tests/test_request_brand_context.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.1/tests/test_request_brand_logging_filter.py` & `sag-py-auth-brand-0.2.2/tests/test_request_brand_logging_filter.py`

 * *Files identical despite different names*

