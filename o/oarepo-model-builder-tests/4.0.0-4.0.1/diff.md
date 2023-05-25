# Comparing `tmp/oarepo-model-builder-tests-4.0.0.tar.gz` & `tmp/oarepo-model-builder-tests-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-tests-4.0.0.tar", last modified: Sat May 20 12:46:47 2023, max compression
+gzip compressed data, was "oarepo-model-builder-tests-4.0.1.tar", last modified: Thu May 25 06:30:29 2023, max compression
```

## Comparing `oarepo-model-builder-tests-4.0.0.tar` & `oarepo-model-builder-tests-4.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/conftest_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/utils.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/test_resource_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/test_service_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/utils_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/conftest_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/utils.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/test_resource_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/test_service_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/utils_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-tests-4.0.0/LICENSE` & `oarepo-model-builder-tests-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/PKG-INFO` & `oarepo-model-builder-tests-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 4.0.0
+Version: 4.0.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-4.0.0/README.md` & `oarepo-model-builder-tests-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/components.py` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/conftest.py.jinja2` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_resource.py.jinja2` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_resource.py.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import datetime
+from urllib.parse import urlencode
 from invenio_records.dictutils import dict_lookup
 {{ vars.resource_config.class|generate_import }}
 from {{ vars.proxy.module }} import {{ vars.service.proxy }}
 from invenio_records_permissions.generators import AuthenticatedUser, AnyUser, SystemProcess
 
 def _get_paths(cur_path, cur_val):
     ret_paths = []
@@ -169,25 +170,27 @@
     with app.test_client() as unauth_client:
         unauth_delete_response = unauth_client.delete(
             f"{BASE_URL}{sample_record['id']}"
         )
         assert response_code_ok("delete", False, unauth_delete_response, 204)
 
 
-@pytest.mark.xfail
 def test_search({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_records, sample_metadata_list, search_clear):
     if is_action_allowed("search", True):
         paths = get_paths("metadata", sample_metadata_list[0]["metadata"])
 
         for record in sample_records:
             for path in paths:
                 field_value = dict_lookup(record, path)
-                path_search_results = client_with_credentials.get(
-                    f'{BASE_URL}?q={path}:"{field_value}"'
-                ).json["hits"]["hits"]
+                encoded_query = urlencode({'q': f'{path}:"{field_value}"'})
+                path_search_response = client_with_credentials.get(
+                    f'{BASE_URL}?{encoded_query}'
+                )
+                assert path_search_response.status_code == 200
+                path_search_results = path_search_response.json["hits"]["hits"]
                 assert len(path_search_results) > 0
                 for field_result in [dict_lookup(res, path) for res in path_search_results]:
                     if field_result == field_value:
                         break
                 else:
                     raise AssertionError("Queried field value not found in search results.")
 
@@ -196,17 +199,20 @@
         start_datetime = (
             datetime.datetime.utcnow() - datetime.timedelta(minutes=5)
         ).isoformat() + "Z"
         end_datetime = (
             datetime.datetime.utcnow() + datetime.timedelta(minutes=5)
         ).isoformat() + "Z"
 
+
+        encoded_query = urlencode({'q': f'created:["{start_datetime}" TO "{end_datetime}"]'})
         res_created = client_with_credentials.get(
-            f'{BASE_URL}?q=created:["{start_datetime}" TO "{end_datetime}"]'
+            f'{BASE_URL}?{encoded_query}'
         )
+
         res_created_fail = client_with_credentials.get(f"{BASE_URL}?q=2022-10-16")
         record_created = sample_records[0].created.isoformat() + "Z"
         res_facets = client_with_credentials.get(f"{BASE_URL}?created={record_created}")
 
         assert len(res_fail.json["hits"]["hits"]) == 0
         assert len(res_created.json["hits"]["hits"]) == 10
         assert len(res_created_fail.json["hits"]["hits"]) == 0
```

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_service.py.jinja2` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_service.py.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     to_delete_record = current_service.read(system_identity, sample_record["id"])
     assert to_delete_record
     current_service.delete(system_identity, sample_record["id"])
     with pytest.raises(PIDDeletedError):
         current_service.read(system_identity, sample_record["id"])
 
 
-@pytest.mark.xfail
 def test_search(
     {{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_records, sample_metadata_list, search_clear
 ):
     paths = get_paths("metadata", sample_metadata_list[0]["metadata"])
 
     for record in sample_records:
         for path in paths:
@@ -124,15 +123,15 @@
     )
     res_facets = list(
         current_service.scan(
             system_identity,
             params={
                 "facets": {
                     "created": [
-                        pytz.utc.localize(sample_records[0].created).isoformat() + "Z"
+                        pytz.utc.localize(sample_records[0].created).isoformat()
                     ]
                 }
             },
         ).hits
     )
 
     res_listing = list(current_service.search(system_identity))
```

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/utils.py.jinja2` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/utils.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/PKG-INFO` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 4.0.0
+Version: 4.0.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/SOURCES.txt` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/entry_points.txt` & `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.0/setup.cfg` & `oarepo-model-builder-tests-4.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = oarepo-model-builder-tests
-version = 4.0.0
+version = 4.0.1
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9
 install_requires = 
-	oarepo-model-builder>=4.0.0
+	oarepo-model-builder>=4.0.3
 packages = find:
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.packages.find]
 exclude = example_model
```

