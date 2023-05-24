# Comparing `tmp/foursight-3.4.7.1b1.tar.gz` & `tmp/foursight-3.4.7.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.4.7.1b1.tar", max compression
+gzip compressed data, was "foursight-3.4.7.1b2.tar", max compression
```

## Comparing `foursight-3.4.7.1b1.tar` & `foursight-3.4.7.1b2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-3.4.7.1b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-3.4.7.1b1/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-01-19 17:19:39.269034 foursight-3.4.7.1b1/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-3.4.7.1b1/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54459 2023-05-16 19:13:56.473217 foursight-3.4.7.1b1/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-3.4.7.1b1/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    60950 2023-05-22 13:38:24.903680 foursight-3.4.7.1b1/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 17:19:39.271725 foursight-3.4.7.1b1/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-3.4.7.1b1/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-3.4.7.1b1/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-3.4.7.1b1/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15609 2023-05-16 19:13:56.473873 foursight-3.4.7.1b1/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2022-11-16 16:53:13.427051 foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 17:19:30.850214 foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2022-11-16 16:53:13.428402 foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 17:19:39.276361 foursight-3.4.7.1b1/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-3.4.7.1b1/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-3.4.7.1b1/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   127978 2023-04-19 19:52:24.092888 foursight-3.4.7.1b1/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 17:19:39.282546 foursight-3.4.7.1b1/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137844 2023-05-23 18:05:48.756394 foursight-3.4.7.1b1/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-3.4.7.1b1/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-3.4.7.1b1/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1261 2023-05-24 20:44:42.395119 foursight-3.4.7.1b1/pyproject.toml
--rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 foursight-3.4.7.1b1/setup.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 foursight-3.4.7.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.7.1b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.7.1b2/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.7.1b2/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.7.1b2/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54459 2023-05-19 14:11:42.736082 foursight-3.4.7.1b2/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.7.1b2/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    60950 2023-05-19 14:11:42.736936 foursight-3.4.7.1b2/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.7.1b2/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.7.1b2/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.7.1b2/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.7.1b2/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15609 2023-05-19 14:11:42.737293 foursight-3.4.7.1b2/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.7.1b2/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.7.1b2/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.4.7.1b2/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.7.1b2/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.7.1b2/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137844 2023-05-24 20:22:32.475168 foursight-3.4.7.1b2/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.7.1b2/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.7.1b2/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1261 2023-05-24 23:14:43.468329 foursight-3.4.7.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 foursight-3.4.7.1b2/setup.py
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 foursight-3.4.7.1b2/PKG-INFO
```

### Comparing `foursight-3.4.7.1b1/LICENSE.txt` & `foursight-3.4.7.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/app_utils.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/check_schedules.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/check_setup.json` & `foursight-3.4.7.1b2/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/chalicelib_fourfront/package.py` & `foursight-3.4.7.1b2/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.7.1b1/pyproject.toml` & `foursight-3.4.7.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight"
-version = "3.4.7.1b1"
+version = "3.4.7.1b2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
```

### Comparing `foursight-3.4.7.1b1/setup.py` & `foursight-3.4.7.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.4.7.1b1',
+    'version': '3.4.7.1b2',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.4.7.1b1/PKG-INFO` & `foursight-3.4.7.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.4.7.1b1
+Version: 3.4.7.1b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

