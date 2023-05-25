# Comparing `tmp/ckanext-msal-1.4.5.tar.gz` & `tmp/ckanext-msal-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-msal-1.4.5.tar", last modified: Thu May 18 12:20:35 2023, max compression
+gzip compressed data, was "ckanext-msal-1.5.0.tar", last modified: Thu May 25 07:09:33 2023, max compression
```

## Comparing `ckanext-msal-1.4.5.tar` & `ckanext-msal-1.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/LICENSE
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      193 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/MANIFEST.in
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3861 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3308 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/README.md
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/ckanext/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      219 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/ckanext/msal/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/ckanext/msal/assets/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      271 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/assets/webassets.yml
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      865 2022-05-16 12:30:13.000000 ckanext-msal-1.4.5/ckanext/msal/config.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      998 2023-04-07 07:39:55.000000 ckanext-msal-1.4.5/ckanext/msal/middleware.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1652 2023-04-07 07:39:55.000000 ckanext-msal-1.4.5/ckanext/msal/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/ckanext/msal/tests/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/tests/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)       46 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/tests/fixtures.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3854 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/tests/test_user.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1276 2022-04-01 10:37:53.000000 ckanext-msal-1.4.5/ckanext/msal/tests/test_utils.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     8711 2022-05-17 09:24:10.000000 ckanext-msal-1.4.5/ckanext/msal/user.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4132 2022-04-01 11:40:30.000000 ckanext-msal-1.4.5/ckanext/msal/utils.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2307 2023-05-18 12:18:13.000000 ckanext-msal-1.4.5/ckanext/msal/views.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/ckanext_msal.egg-info/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3861 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      637 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/SOURCES.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/dependency_links.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      110 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/entry_points.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/namespace_packages.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-05-18 12:20:35.000000 ckanext-msal-1.4.5/ckanext_msal.egg-info/top_level.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)       65 2022-11-08 12:53:47.000000 ckanext-msal-1.4.5/requirements.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      517 2023-05-18 12:20:35.398291 ckanext-msal-1.4.5/setup.cfg
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3754 2023-05-18 12:20:11.000000 ckanext-msal-1.4.5/setup.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.134211 ckanext-msal-1.5.0/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/LICENSE
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      193 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/MANIFEST.in
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3859 2023-05-25 07:09:33.134211 ckanext-msal-1.5.0/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3306 2023-05-25 07:08:28.000000 ckanext-msal-1.5.0/README.md
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.126211 ckanext-msal-1.5.0/ckanext/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      219 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.126211 ckanext-msal-1.5.0/ckanext/msal/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.126211 ckanext-msal-1.5.0/ckanext/msal/assets/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      271 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/assets/webassets.yml
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      865 2022-05-16 12:30:13.000000 ckanext-msal-1.5.0/ckanext/msal/config.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      998 2023-04-07 07:39:55.000000 ckanext-msal-1.5.0/ckanext/msal/middleware.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1507 2023-05-25 07:07:14.000000 ckanext-msal-1.5.0/ckanext/msal/plugin.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.130211 ckanext-msal-1.5.0/ckanext/msal/tests/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/tests/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       46 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/tests/fixtures.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3854 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/tests/test_user.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1276 2022-04-01 10:37:53.000000 ckanext-msal-1.5.0/ckanext/msal/tests/test_utils.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     8711 2022-05-17 09:24:10.000000 ckanext-msal-1.5.0/ckanext/msal/user.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     4132 2022-04-01 11:40:30.000000 ckanext-msal-1.5.0/ckanext/msal/utils.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2310 2023-05-25 07:07:14.000000 ckanext-msal-1.5.0/ckanext/msal/views.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-05-25 07:09:33.134211 ckanext-msal-1.5.0/ckanext_msal.egg-info/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3859 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      637 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/SOURCES.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/dependency_links.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      110 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/entry_points.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-05-25 07:09:33.000000 ckanext-msal-1.5.0/ckanext_msal.egg-info/top_level.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       65 2022-11-08 12:53:47.000000 ckanext-msal-1.5.0/requirements.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      517 2023-05-25 07:09:33.134211 ckanext-msal-1.5.0/setup.cfg
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3754 2023-05-25 07:07:31.000000 ckanext-msal-1.5.0/setup.py
```

### Comparing `ckanext-msal-1.4.5/LICENSE` & `ckanext-msal-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/PKG-INFO` & `ckanext-msal-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-msal
-Version: 1.4.5
+Version: 1.5.0
 Summary: Login to CKAN using The Microsoft Authentication Library (MSAL)
 Home-page: https://github.com/mutantsan/ckanext-msal
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN SSO,CKAN,Microsoft,SAML,MSAL
 Classifier: Development Status :: 4 - Beta
@@ -21,18 +21,18 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.6 and earlier | not tested    |
-| 2.7             | not tested    |
-| 2.8             | not tested    |
-| 2.9             | yes           |
+| 2.7 and earlier | no            |
+| 2.8             | no            |
+| 2.9             | no            |
+| 2.10.0+         | yes           |
 
 ## Installation
 
 To install ckanext-msal:
 
 1. Activate your CKAN virtual environment, for example:
 
@@ -53,18 +53,18 @@
 
      sudo service apache2 reload
 
 
 ## Config settings
 	# The application client id. Mandatory option.
 	ckanext.msal.client_id = 000000-0000-0000-0000-00000000000
-	
+
 	# The client secret. Mandatory option.
 	ckanext.msal.client_secret = 000000-0000-0000-0000-00000000000
-	
+
     # The tenant ID. If it's not provided, the common one for multi-tenant app will be used.
     # In this case, the application is not guaranteed to work properly.
     # (optional, default: 'common').
     ckanext.msal.tenant_id = 000000-0000-0000-0000-00000000000
 
     # The redirect path should be setted up in Azure AD web app config.
     # It handles the response from Microsoft.
```

### Comparing `ckanext-msal-1.4.5/README.md` & `ckanext-msal-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.6 and earlier | not tested    |
-| 2.7             | not tested    |
-| 2.8             | not tested    |
-| 2.9             | yes           |
+| 2.7 and earlier | no            |
+| 2.8             | no            |
+| 2.9             | no            |
+| 2.10.0+         | yes           |
 
 ## Installation
 
 To install ckanext-msal:
 
 1. Activate your CKAN virtual environment, for example:
 
@@ -38,18 +38,18 @@
 
      sudo service apache2 reload
 
 
 ## Config settings
 	# The application client id. Mandatory option.
 	ckanext.msal.client_id = 000000-0000-0000-0000-00000000000
-	
+
 	# The client secret. Mandatory option.
 	ckanext.msal.client_secret = 000000-0000-0000-0000-00000000000
-	
+
     # The tenant ID. If it's not provided, the common one for multi-tenant app will be used.
     # In this case, the application is not guaranteed to work properly.
     # (optional, default: 'common').
     ckanext.msal.tenant_id = 000000-0000-0000-0000-00000000000
 
     # The redirect path should be setted up in Azure AD web app config.
     # It handles the response from Microsoft.
```

### Comparing `ckanext-msal-1.4.5/ckanext/msal/config.py` & `ckanext-msal-1.5.0/ckanext/msal/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/middleware.py` & `ckanext-msal-1.5.0/ckanext/msal/middleware.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/tests/test_user.py` & `ckanext-msal-1.5.0/ckanext/msal/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/tests/test_utils.py` & `ckanext-msal-1.5.0/ckanext/msal/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/user.py` & `ckanext-msal-1.5.0/ckanext/msal/user.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/utils.py` & `ckanext-msal-1.5.0/ckanext/msal/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/ckanext/msal/views.py` & `ckanext-msal-1.5.0/ckanext/msal/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         session["user_exp"] = msal_utils._get_exp_date()
         msal_utils._save_cache(cache)
     except ValueError:
         # Usually caused by CSRF
         # Simply ignore them
         pass
 
-    return h.redirect_to(h.url_for("dashboard.index"))
+    return h.redirect_to(h.url_for("activity.dashboard"))
 
 
 @msal.route("/user/msal-logout")
 def logout():
     if session.get("msal_auth_flow") or session.get("msal_token_cache"):
         msal_utils._clear_session()
         redirect_uri: str = h.url_for("user.logout", _external=True)
```

### Comparing `ckanext-msal-1.4.5/ckanext_msal.egg-info/PKG-INFO` & `ckanext-msal-1.5.0/ckanext_msal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-msal
-Version: 1.4.5
+Version: 1.5.0
 Summary: Login to CKAN using The Microsoft Authentication Library (MSAL)
 Home-page: https://github.com/mutantsan/ckanext-msal
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN SSO,CKAN,Microsoft,SAML,MSAL
 Classifier: Development Status :: 4 - Beta
@@ -21,18 +21,18 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.6 and earlier | not tested    |
-| 2.7             | not tested    |
-| 2.8             | not tested    |
-| 2.9             | yes           |
+| 2.7 and earlier | no            |
+| 2.8             | no            |
+| 2.9             | no            |
+| 2.10.0+         | yes           |
 
 ## Installation
 
 To install ckanext-msal:
 
 1. Activate your CKAN virtual environment, for example:
 
@@ -53,18 +53,18 @@
 
      sudo service apache2 reload
 
 
 ## Config settings
 	# The application client id. Mandatory option.
 	ckanext.msal.client_id = 000000-0000-0000-0000-00000000000
-	
+
 	# The client secret. Mandatory option.
 	ckanext.msal.client_secret = 000000-0000-0000-0000-00000000000
-	
+
     # The tenant ID. If it's not provided, the common one for multi-tenant app will be used.
     # In this case, the application is not guaranteed to work properly.
     # (optional, default: 'common').
     ckanext.msal.tenant_id = 000000-0000-0000-0000-00000000000
 
     # The redirect path should be setted up in Azure AD web app config.
     # It handles the response from Microsoft.
```

### Comparing `ckanext-msal-1.4.5/ckanext_msal.egg-info/SOURCES.txt` & `ckanext-msal-1.5.0/ckanext_msal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/setup.cfg` & `ckanext-msal-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-msal-1.4.5/setup.py` & `ckanext-msal-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='''ckanext-msal''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='1.4.5',
+    version='1.5.0',
 
     description='''Login to CKAN using The Microsoft Authentication Library (MSAL)''',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/mutantsan/ckanext-msal',
```

